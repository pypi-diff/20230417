# Comparing `tmp/zigzag-dse-2.3.1.tar.gz` & `tmp/zigzag-dse-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag-dse-2.3.1.tar", last modified: Mon Mar 27 15:23:37 2023, max compression
+gzip compressed data, was "zigzag-dse-2.3.2.tar", last modified: Mon Apr 17 10:08:11 2023, max compression
```

## Comparing `zigzag-dse-2.3.1.tar` & `zigzag-dse-2.3.2.tar`

### file list

```diff
@@ -1,276 +1,271 @@
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.369112 zigzag-dse-2.3.1/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/LICENSE
--rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/MANIFEST.in
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-03-27 15:23:37.369112 zigzag-dse-2.3.1/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6596 2023-03-14 15:21:48.000000 zigzag-dse-2.3.1/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.079112 zigzag-dse-2.3.1/docs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.109112 zigzag-dse-2.3.1/docs/source/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2594 2023-03-14 15:21:19.000000 zigzag-dse-2.3.1/docs/source/conf.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.079112 zigzag-dse-2.3.1/inputs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.079112 zigzag-dse-2.3.1/inputs/examples/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.119112 zigzag-dse-2.3.1/inputs/examples/hardware/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7986 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7920 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Ascend_like_DF.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5611 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6889 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Edge_TPU_like_DF.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5242 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6778 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6908 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Meta_prototype_DF.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4958 2022-11-06 21:24:55.000000 zigzag-dse-2.3.1/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5977 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/TPU_like_DF.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6974 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Tesla_NPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7944 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/inputs/examples/hardware/Tesla_NPU_like_DF.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.119112 zigzag-dse-2.3.1/inputs/examples/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1183 2022-09-19 16:35:57.000000 zigzag-dse-2.3.1/inputs/examples/mapping/alexnet_on_eyeriss_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      194 2022-11-06 21:27:07.000000 zigzag-dse-2.3.1/inputs/examples/mapping/default.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.119112 zigzag-dse-2.3.1/inputs/examples/workloads/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    16898 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/inputs/examples/workloads/resnet18.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1587 2023-03-27 15:23:11.000000 zigzag-dse-2.3.1/pyproject.toml
--rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-03-27 15:23:37.369112 zigzag-dse-2.3.1/setup.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.129112 zigzag-dse-2.3.1/zigzag/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-03-27 15:23:11.000000 zigzag-dse-2.3.1/zigzag/__init__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.1/zigzag/__main__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4671 2023-03-14 15:21:48.000000 zigzag-dse-2.3.1/zigzag/api.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.129112 zigzag-dse-2.3.1/zigzag/classes/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.1/zigzag/classes/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.129112 zigzag-dse-2.3.1/zigzag/classes/cacti/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.129112 zigzag-dse-2.3.1/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3258 2023-03-27 15:20:55.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.199112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/Ucache.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.209112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/__pycache__/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-03-27 15:21:11.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    13989 2023-03-22 14:21:52.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-38.pyc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-03-27 15:21:12.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.259112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.279112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.279112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-03-27 15:21:11.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-03-27 15:21:12.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.279112 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4864 2023-03-27 09:38:39.000000 zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.279112 zigzag-dse-2.3.1/zigzag/classes/cost_model/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    55157 2023-03-15 14:29:14.000000 zigzag-dse-2.3.1/zigzag/classes/cost_model/cost_model.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.089112 zigzag-dse-2.3.1/zigzag/classes/hardware/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.289112 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1899 2022-11-06 20:14:47.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8810 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5555 2022-11-17 21:58:36.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      893 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11254 2023-01-17 08:57:11.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3377 2023-03-27 15:20:49.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    11645 2022-11-05 20:51:19.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3709 2022-10-27 21:29:08.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/operand_spatial_sharing.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3088 2022-11-01 21:49:29.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1778 2022-11-01 21:49:48.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/operational_unit.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1625 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/runtime_mode.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.089112 zigzag-dse-2.3.1/zigzag/classes/io/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.289112 zigzag-dse-2.3.1/zigzag/classes/io/accelerator/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.1/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/io/onnx/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8505 2023-02-28 21:36:12.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      846 2023-02-28 21:36:47.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5102 2023-02-28 21:36:55.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3527 2023-02-28 21:37:01.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4786 2022-11-06 18:48:47.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1154 2023-02-02 17:09:08.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4248 2023-01-17 11:07:28.000000 zigzag-dse-2.3.1/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 20:40:14.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/__init__.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    37466 2023-03-14 15:21:48.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      636 2022-10-28 03:28:17.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8710 2023-02-01 20:58:34.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/mapping/memory/
--rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/mapping/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7077 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/mapping/temporal/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      383 2022-10-28 03:28:15.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6679 2022-10-27 21:47:50.000000 zigzag-dse-2.3.1/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.099112 zigzag-dse-2.3.1/zigzag/classes/opt/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/opt/spatial/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6678 2023-01-18 08:27:19.000000 zigzag-dse-2.3.1/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.099112 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.299112 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 asymons   (1000) asymons   (1000)    12175 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      488 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    14874 2023-01-17 08:56:40.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2694 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.309112 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8288 2023-01-16 14:56:45.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3499 2023-01-16 14:56:45.000000 zigzag-dse-2.3.1/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.329112 zigzag-dse-2.3.1/zigzag/classes/stages/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1951 2023-03-15 14:29:05.000000 zigzag-dse-2.3.1/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1551 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3107 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1968 2022-12-15 01:23:01.000000 zigzag-dse-2.3.1/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2989 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      911 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1571 2022-11-07 04:52:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5860 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6053 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6386 2023-01-16 14:56:45.000000 zigzag-dse-2.3.1/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6812 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7971 2022-12-09 23:35:35.000000 zigzag-dse-2.3.1/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4496 2023-01-19 16:11:29.000000 zigzag-dse-2.3.1/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2538 2022-06-17 07:16:25.000000 zigzag-dse-2.3.1/zigzag/classes/stages/Stage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4180 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1246 2023-02-13 15:36:32.000000 zigzag-dse-2.3.1/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3214 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.329112 zigzag-dse-2.3.1/zigzag/classes/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2447 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     2206 2023-02-28 21:39:12.000000 zigzag-dse-2.3.1/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    20065 2023-02-28 21:38:57.000000 zigzag-dse-2.3.1/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1524 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)    12928 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.099112 zigzag-dse-2.3.1/zigzag/inputs/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.099112 zigzag-dse-2.3.1/zigzag/inputs/examples/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.339112 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     7986 2022-11-06 21:24:44.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5611 2022-11-06 21:24:44.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     5242 2022-11-06 21:24:44.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6778 2022-11-06 21:24:44.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4961 2022-11-06 23:17:46.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6974 2022-11-06 21:24:44.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.339112 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/
--rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/alexnet_on_tpu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      440 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/assend_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      194 2022-11-06 21:26:14.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/default.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      651 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      439 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      606 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      292 2023-03-14 15:21:48.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/test.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.349112 zigzag-dse-2.3.1/zigzag/inputs/examples/workload/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 asymons   (1000) asymons   (1000)    16898 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/workload/resnet18.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      548 2023-03-14 15:21:48.000000 zigzag-dse-2.3.1/zigzag/inputs/examples/workload/test.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.1/zigzag/utils.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.109112 zigzag-dse-2.3.1/zigzag/visualization/
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.359112 zigzag-dse-2.3.1/zigzag/visualization/graph/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1439 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     1270 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.359112 zigzag-dse-2.3.1/zigzag/visualization/results/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     6989 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons   (1000) asymons   (1000)     3813 2023-02-13 14:30:34.000000 zigzag-dse-2.3.1/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-03-27 15:23:37.369112 zigzag-dse-2.3.1/zigzag_dse.egg-info/
--rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons   (1000) asymons   (1000)    10491 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)      137 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons   (1000) asymons   (1000)       12 2023-03-27 15:23:37.000000 zigzag-dse-2.3.1/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.392251 zigzag-dse-2.3.2/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1522 2022-06-17 07:16:25.000000 zigzag-dse-2.3.2/LICENSE
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       88 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/MANIFEST.in
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-17 10:08:11.392251 zigzag-dse-2.3.2/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6596 2023-03-14 15:21:48.000000 zigzag-dse-2.3.2/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.822251 zigzag-dse-2.3.2/docs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.862251 zigzag-dse-2.3.2/docs/source/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2594 2023-03-14 15:21:19.000000 zigzag-dse-2.3.2/docs/source/conf.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.822251 zigzag-dse-2.3.2/inputs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.832251 zigzag-dse-2.3.2/inputs/examples/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.872251 zigzag-dse-2.3.2/inputs/examples/hardware/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7986 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7920 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Ascend_like_DF.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5611 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6889 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Edge_TPU_like_DF.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5242 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6778 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6908 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Meta_prototype_DF.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4958 2022-11-06 21:24:55.000000 zigzag-dse-2.3.2/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5977 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/TPU_like_DF.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6974 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Tesla_NPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7944 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/inputs/examples/hardware/Tesla_NPU_like_DF.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/inputs/examples/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1183 2022-09-19 16:35:57.000000 zigzag-dse-2.3.2/inputs/examples/mapping/alexnet_on_eyeriss_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      194 2022-11-06 21:27:07.000000 zigzag-dse-2.3.2/inputs/examples/mapping/default.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/inputs/examples/workloads/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    16898 2023-02-13 14:30:34.000000 zigzag-dse-2.3.2/inputs/examples/workloads/resnet18.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1587 2023-04-17 10:07:47.000000 zigzag-dse-2.3.2/pyproject.toml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       38 2023-04-17 10:08:11.392251 zigzag-dse-2.3.2/setup.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/zigzag/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       22 2023-04-17 10:07:47.000000 zigzag-dse-2.3.2/zigzag/__init__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2497 2022-11-06 07:09:28.000000 zigzag-dse-2.3.2/zigzag/__main__.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4451 2023-04-15 15:25:43.000000 zigzag-dse-2.3.2/zigzag/api.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/zigzag/classes/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2022-11-06 21:40:40.000000 zigzag-dse-2.3.2/zigzag/classes/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/zigzag/classes/cacti/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      291 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/README.md
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.882251 zigzag-dse-2.3.2/zigzag/classes/cacti/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3258 2023-04-07 09:43:32.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.122251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6576 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6555 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6920 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5324 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/README
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9282 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/TSV.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3322 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/TSV.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41184 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/Ucache.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3607 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/Ucache.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.122251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/__pycache__/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    13713 2023-04-16 14:07:27.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/arbiter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2771 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/arbiter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2057 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/area.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/area.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8474 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/bank.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2664 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/bank.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29279 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/basic_circuit.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7364 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/basic_circuit.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11041 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cache.cfg_temp
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    32713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      173 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti.i
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1334 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti.mk
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    25297 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5586 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_interface.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    27215 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_interface.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3569 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7561 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/component.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/component.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9565 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/const.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5001 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/contention.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7349 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/crossbar.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3204 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/crossbar.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9849 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/ddr3.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62337 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/decoder.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7405 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/decoder.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3712 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/dram.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9750 2023-04-17 10:07:29.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    17411 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      878 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    46185 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio_technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9068 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio_technology.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23772 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/htree2.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3595 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/htree2.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   133713 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/io.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2116 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/io.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9850 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/lpddr.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7217 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/main.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      407 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/makefile
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    94813 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/mat.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6122 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/mat.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    16630 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      553 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11483 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4490 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad_parameters.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29014 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memorybus.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5426 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memorybus.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19629 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/nuca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/nuca.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.272251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   134304 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   352744 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   157960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124352 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   156624 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   155192 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)  2421320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   159768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   160680 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   207224 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   145592 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   180464 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   178384 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   411960 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   192248 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   270320 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   569648 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   280416 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   204480 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   256824 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   313848 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   124400 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   175432 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   128080 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   144976 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   228000 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   232752 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
+-rw-r--r--   0 asymons   (1000) asymons   (1000)   111980 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/parameter.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    20306 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/parameter.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5286 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/powergating.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3055 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/powergating.h
+-rwxr-xr-x   0 asymons   (1000) asymons   (1000)     1886 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/regression.test
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    10212 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/router.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3721 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/router.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.282251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8781 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8768 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8780 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8784 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.282251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/self_gen/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9545 2023-04-17 10:07:29.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      579 2023-04-17 10:07:29.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8332 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/subarray.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2542 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/subarray.h
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.322251 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       25 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    23666 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3842 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4575 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4759 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4755 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24571 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4758 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    24570 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4742 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15087 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/technology.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    41317 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/uca.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4035 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/uca.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2064 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/version_cacti.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    29856 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/wire.cc
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4375 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/wire.h
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4864 2023-03-27 09:38:39.000000 zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.322251 zigzag-dse-2.3.2/zigzag/classes/cost_model/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    62023 2023-04-16 12:43:30.000000 zigzag-dse-2.3.2/zigzag/classes/cost_model/cost_model.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.842251 zigzag-dse-2.3.2/zigzag/classes/hardware/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1278 2023-04-16 13:43:29.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/accelerator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9441 2023-04-07 09:22:11.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/adder_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6031 2023-04-07 09:22:16.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/core.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      918 2023-04-07 09:22:20.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/dimension.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11764 2023-04-07 09:22:26.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3351 2023-04-07 09:22:31.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_instance.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    12231 2023-04-07 09:22:36.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3014 2023-04-07 09:22:40.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1874 2023-04-07 09:22:44.000000 zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.842251 zigzag-dse-2.3.2/zigzag/classes/io/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/io/accelerator/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2805 2022-11-06 21:24:03.000000 zigzag-dse-2.3.2/zigzag/classes/io/accelerator/parser.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/io/onnx/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9127 2023-04-15 11:49:50.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/conv.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      884 2023-04-07 09:12:40.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5382 2023-04-07 09:12:45.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/gemm.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3679 2023-04-07 09:12:49.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/matmul.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4912 2023-04-07 09:12:53.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/model.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1163 2023-04-07 09:12:58.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/parser.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4391 2023-04-07 09:13:02.000000 zigzag-dse-2.3.2/zigzag/classes/io/onnx/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    40951 2023-04-07 09:24:31.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/combined_mapping.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      637 2023-04-07 09:24:42.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     9386 2023-04-07 09:24:55.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/mapping_assist_funcs.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/mapping/memory/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        0 2023-04-07 09:25:08.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/memory/data_layout.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/mapping/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7607 2023-04-07 09:25:03.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/spatial/spatial_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/mapping/temporal/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      380 2023-04-07 09:25:12.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/temporal/temporal_loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7412 2023-04-07 09:25:16.000000 zigzag-dse-2.3.2/zigzag/classes/mapping/temporal/temporal_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.842251 zigzag-dse-2.3.2/zigzag/classes/opt/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/opt/spatial/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7044 2023-04-07 09:30:21.000000 zigzag-dse-2.3.2/zigzag/classes/opt/spatial/generator.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.852251 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    11591 2023-04-07 09:29:56.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      489 2023-04-07 09:30:00.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/loop.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    15479 2023-04-07 09:30:04.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/memory_allocator.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2837 2023-04-07 09:30:07.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/multipermute.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.332251 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/salsa/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8726 2023-04-07 09:30:11.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/salsa/engine.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3616 2023-04-07 09:30:15.000000 zigzag-dse-2.3.2/zigzag/classes/opt/temporal/salsa/state.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.352251 zigzag-dse-2.3.2/zigzag/classes/stages/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2054 2023-04-07 09:02:40.000000 zigzag-dse-2.3.2/zigzag/classes/stages/CostModelStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1552 2023-04-07 09:03:00.000000 zigzag-dse-2.3.2/zigzag/classes/stages/DumpStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3240 2023-04-07 09:02:56.000000 zigzag-dse-2.3.2/zigzag/classes/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2105 2023-04-07 09:02:49.000000 zigzag-dse-2.3.2/zigzag/classes/stages/LomaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2163 2023-04-07 09:27:10.000000 zigzag-dse-2.3.2/zigzag/classes/stages/MainInputParserStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      966 2023-04-07 09:03:11.000000 zigzag-dse-2.3.2/zigzag/classes/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1568 2023-04-07 09:03:29.000000 zigzag-dse-2.3.2/zigzag/classes/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6204 2023-04-07 09:03:44.000000 zigzag-dse-2.3.2/zigzag/classes/stages/ReduceStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6260 2023-04-07 09:03:58.000000 zigzag-dse-2.3.2/zigzag/classes/stages/RunOptStages.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6546 2023-04-07 09:04:04.000000 zigzag-dse-2.3.2/zigzag/classes/stages/SalsaStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     6997 2023-04-15 12:05:47.000000 zigzag-dse-2.3.2/zigzag/classes/stages/SaveStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8158 2023-04-07 09:04:25.000000 zigzag-dse-2.3.2/zigzag/classes/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3906 2023-04-07 09:05:11.000000 zigzag-dse-2.3.2/zigzag/classes/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2593 2023-04-07 09:05:30.000000 zigzag-dse-2.3.2/zigzag/classes/stages/Stage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4046 2023-04-07 09:05:44.000000 zigzag-dse-2.3.2/zigzag/classes/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1187 2023-04-07 09:05:50.000000 zigzag-dse-2.3.2/zigzag/classes/stages/WorkloadStage.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2821 2023-04-07 09:28:15.000000 zigzag-dse-2.3.2/zigzag/classes/stages/__init__.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.352251 zigzag-dse-2.3.2/zigzag/classes/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2468 2023-04-07 09:17:48.000000 zigzag-dse-2.3.2/zigzag/classes/workload/dnn_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     2210 2023-04-07 09:17:53.000000 zigzag-dse-2.3.2/zigzag/classes/workload/dummy_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    21102 2023-04-07 09:19:32.000000 zigzag-dse-2.3.2/zigzag/classes/workload/layer_node.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1542 2023-04-07 09:18:04.000000 zigzag-dse-2.3.2/zigzag/classes/workload/onnx_workload.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    14521 2023-04-07 09:18:09.000000 zigzag-dse-2.3.2/zigzag/classes/workload/test_layer_node.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.852251 zigzag-dse-2.3.2/zigzag/inputs/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.852251 zigzag-dse-2.3.2/zigzag/inputs/examples/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.372251 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8448 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5849 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5746 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7098 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     5112 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     7287 2023-04-16 14:01:57.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.372251 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:48:40.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/alexnet_on_tpu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      561 2023-04-15 09:48:43.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/assend_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      196 2023-04-15 09:48:46.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/default.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      832 2023-04-15 09:48:50.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/edge_tpu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      560 2023-04-15 09:48:52.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/meta_prototype_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      610 2023-04-15 09:48:56.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/tesla_npu_like.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      557 2023-04-15 09:49:08.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/mapping/tpu_like.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.382251 zigzag-dse-2.3.2/zigzag/inputs/examples/workload/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     4067 2023-01-16 14:56:40.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/workload/alexnet.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    71724 2022-12-09 21:20:28.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/workload/mobilenetv2.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    18600 2023-04-15 09:55:05.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/workload/resnet18.onnx
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    19065 2023-04-15 09:49:14.000000 zigzag-dse-2.3.2/zigzag/inputs/examples/workload/resnet18.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      504 2022-10-27 21:43:16.000000 zigzag-dse-2.3.2/zigzag/utils.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:10.862251 zigzag-dse-2.3.2/zigzag/visualization/
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.382251 zigzag-dse-2.3.2/zigzag/visualization/graph/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1527 2023-04-15 09:49:36.000000 zigzag-dse-2.3.2/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     1280 2023-04-15 09:49:41.000000 zigzag-dse-2.3.2/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.382251 zigzag-dse-2.3.2/zigzag/visualization/results/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8773 2023-04-16 16:18:26.000000 zigzag-dse-2.3.2/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     3951 2023-04-15 09:49:53.000000 zigzag-dse-2.3.2/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons   (1000) asymons   (1000)        0 2023-04-17 10:08:11.392251 zigzag-dse-2.3.2/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons   (1000) asymons   (1000)     8918 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons   (1000) asymons   (1000)    10224 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)        1 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       52 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)      137 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons   (1000) asymons   (1000)       27 2023-04-17 10:08:10.000000 zigzag-dse-2.3.2/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag-dse-2.3.1/LICENSE` & `zigzag-dse-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/PKG-INFO` & `zigzag-dse-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.1
+Version: 2.3.2
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.1/README.md` & `zigzag-dse-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/docs/source/conf.py` & `zigzag-dse-2.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Ascend_like.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Ascend_like_DF.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Ascend_like_DF.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Edge_TPU_like_DF.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Edge_TPU_like_DF.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Eyeriss_like.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Meta_prototype.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Meta_prototype.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Meta_prototype_DF.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Meta_prototype_DF.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/TPU_like.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/TPU_like_DF.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/TPU_like_DF.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Tesla_NPU_like.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/hardware/Tesla_NPU_like_DF.py` & `zigzag-dse-2.3.2/inputs/examples/hardware/Tesla_NPU_like_DF.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/mapping/alexnet_on_eyeriss_like.py` & `zigzag-dse-2.3.2/inputs/examples/mapping/alexnet_on_eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/inputs/examples/workloads/resnet18.py` & `zigzag-dse-2.3.2/inputs/examples/workloads/resnet18.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/pyproject.toml` & `zigzag-dse-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "2.3.1"
+version = "2.3.2"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -40,15 +40,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "2.3.1"
+current_version = "2.3.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag-dse-2.3.1/zigzag/__main__.py` & `zigzag-dse-2.3.2/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/api.py` & `zigzag-dse-2.3.2/zigzag/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 from zigzag.classes.stages import *
 import re
 
-def get_hardware_performance_zigzag(workload,
-                                    accelerator,
-                                    mapping,
-                                    opt='latency',
-                                    dump_filename_pattern="outputs/{datetime}.json",
-                                    pickle_filename="outputs/list_of_cmes.pickle"):
+
+def get_hardware_performance_zigzag(
+    workload,
+    accelerator,
+    mapping,
+    opt="latency",
+    dump_filename_pattern="outputs/{datetime}.json",
+    pickle_filename="outputs/list_of_cmes.pickle",
+):
     # Initialize the logger
     import logging as _logging
+
     _logging_level = _logging.INFO
-    _logging_format = '%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s'
-    _logging.basicConfig(level=_logging_level,
-                         format=_logging_format)
+    _logging_format = (
+        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
+    )
+    _logging.basicConfig(level=_logging_level, format=_logging_format)
 
     # Sanity check on the optimization criterion
-    if opt == 'energy':
+    if opt == "energy":
         opt_stage = MinimalEnergyStage
-    elif opt == 'latency':
+    elif opt == "latency":
         opt_stage = MinimalLatencyStage
-    elif opt == 'EDP':
+    elif opt == "EDP":
         opt_stage = MinimalEDPStage
     else:
-        raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
+        raise NotImplementedError(
+            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
+        )
 
     # Check workload format and based on it select the correct workload parser stage
     try:
-        if workload.split('.')[-1] == 'onnx':
+        if workload.split(".")[-1] == "onnx":
             workload_parser_stage = ONNXModelParserStage
         else:
             workload_parser_stage = WorkloadParserStage
     except:
         workload_parser_stage = WorkloadParserStage
 
-    mainstage = MainStage([  # Initialize the MainStage as entry point
-        workload_parser_stage,  # Parse the ONNX Model into the workload
-        AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
-        SimpleSaveStage,  # Save the summed CME energy and latency to a json
-        PickleSaveStage,  # Save all received CMEs in a list to a pickle file
-        SumStage,  # Sum up the received best CME across all layers of the workload
-        WorkloadStage,  # Iterate through the different layers in the workload
-        CompleteSaveStage,  # Save each processed layer to a json
-        opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
-        SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
-        opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
-        LomaStage,  # Generate multiple temporal mappings (TM)
-        # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
-        CostModelStage  # Evaluate generated SM and TM through cost model
-    ],
+    mainstage = MainStage(
+        [  # Initialize the MainStage as entry point
+            workload_parser_stage,  # Parse the ONNX Model into the workload
+            AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
+            SimpleSaveStage,  # Save the summed CME energy and latency to a json
+            PickleSaveStage,  # Save all received CMEs in a list to a pickle file
+            SumStage,  # Sum up the received best CME across all layers of the workload
+            WorkloadStage,  # Iterate through the different layers in the workload
+            CompleteSaveStage,  # Save each processed layer to a json
+            opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
+            SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
+            opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
+            LomaStage,  # Generate multiple temporal mappings (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            CostModelStage,  # Evaluate generated SM and TM through cost model
+        ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=6,  # required by LomaStage
         loma_show_progress_bar=True,
@@ -66,32 +74,34 @@
     # Get CME from answer
     cmes = answers
 
     return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes
 
 
 if __name__ == "__main__":
-    workload = 'inputs/examples/workload/mobilenetv2.onnx'
+    workload = "zigzag/inputs/examples/workload/mobilenetv2.onnx"
     # workload = 'inputs.examples.workload.resnet18'
-    accelerator = 'inputs.examples.hardware.TPU_like'
-    mapping = 'inputs.examples.mapping.tpu_like'
+    accelerator = "zigzag.inputs.examples.hardware.TPU_like"
+    mapping = "zigzag.inputs.examples.mapping.tpu_like"
 
     hw_name = accelerator.split(".")[-1]
     wl_name = re.split(r"/|\.", workload)[-1]
-    if wl_name == 'onnx':
+    if wl_name == "onnx":
         wl_name = re.split(r"/|\.", workload)[-2]
     experiment_id = f"{hw_name}-{wl_name}"
-    pkl_name = f'{experiment_id}-saved_list_of_cmes'
+    pkl_name = f"{experiment_id}-saved_list_of_cmes"
 
-    answer = get_hardware_performance_zigzag(workload,
-                                             accelerator,
-                                             mapping,
-                                             opt='EDP',
-                                             dump_filename_pattern=f"outputs/{experiment_id}-layer_?.json",
-                                             pickle_filename=f"outputs/{pkl_name}.pickle")
+    answer = get_hardware_performance_zigzag(
+        workload,
+        accelerator,
+        mapping,
+        opt="EDP",
+        dump_filename_pattern=f"outputs/{experiment_id}-layer_?.json",
+        pickle_filename=f"outputs/{pkl_name}.pickle",
+    )
     # print(f'Answer = {answer}')
 
     # import pickle
     # path = f"outputs/{pkl_name}.pickle"
     # with open(path, 'rb') as f:
     #     data = pickle.load(f)
-    # f.close()
+    # f.close()
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar 27 09:38:39 2023 UTC, .py size: 4864 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 00000590: 7274 7a0c 2d2d 7264 5f77 725f 706f 7274  rtz.--rd_wr_port
 000005a0: 7a0c 2d2d 6261 6e6b 5f63 6f75 6e74 7a0f  z.--bank_countz.
 000005b0: 2d2d 6d65 6d5f 706f 6f6c 5f70 6174 6872  --mem_pool_pathr
 000005c0: 0100 0000 7a2f 4361 6374 6920 7375 6270  ....z/Cacti subp
 000005d0: 726f 6365 7373 2063 616c 6c20 6661 696c  rocess call fail
 000005e0: 6564 2077 6974 6820 7265 7475 726e 2076  ed with return v
 000005f0: 616c 7565 20da 012e 2905 da0a 7375 6270  alue ...)...subp
-00000600: 726f 6365 7373 5a04 6361 6c6c da03 7374  rocessZ.call..st
+00000600: 726f 6365 7373 da04 6361 6c6c da03 7374  rocess..call..st
 00000610: 7272 1600 0000 da11 4368 696c 6450 726f  rr......ChildPro
 00000620: 6365 7373 4572 726f 7229 0b72 0400 0000  cessError).r....
 00000630: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
 00000640: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
 00000650: 0000 0072 1e00 0000 da0e 6361 6374 695f  ...r......cacti_
 00000660: 746f 705f 7061 7468 da01 7072 0300 0000  top_path..pr....
 00000670: 7203 0000 0072 0500 0000 da0b 6372 6561  r....r......crea
@@ -141,15 +141,15 @@
 000008c0: 0264 1a7c 059b 0264 1b7c 069b 0264 1c7c  .d.|...d.|...d.|
 000008d0: 079b 029d 0c83 0182 0129 1d4e 7a1e 4361  .........).Nz.Ca
 000008e0: 6374 6920 746f 7020 6669 6c65 2064 6f65  cti top file doe
 000008f0: 736e 2774 2065 7869 7374 3a20 7227 0000  sn't exist: r'..
 00000900: 007a 2e45 7874 7261 6374 696e 6720 6d65  .z.Extracting me
 00000910: 6d6f 7279 2063 6f73 7473 2077 6974 6820  mory costs with 
 00000920: 4341 4354 4920 666f 7220 7369 7a65 203d  CACTI for size =
-00000930: 207a 0c20 616e 6420 725f 6277 203d 20da   z. and r_bw = .
+00000930: 207a 0c20 616e 6420 725f 6277 203d 205a   z. and r_bw = Z
 00000940: 0272 66da 0473 7261 6de9 8000 0000 7a35  .rf..sram.....z5
 00000950: 6d65 6d5f 7479 7065 2069 7320 7265 6769  mem_type is regi
 00000960: 7374 6572 2066 696c 6521 2043 6861 6e67  ster file! Chang
 00000970: 6564 2074 6f20 2773 7261 6d27 2061 6e64  ed to 'sram' and
 00000980: 2073 697a 657a 0a69 6e73 7465 6164 206f   sizez.instead o
 00000990: 6672 0700 0000 7208 0000 0072 0900 0000  fr....r....r....
 000009a0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
@@ -162,20 +162,20 @@
 00000a10: 2c20 725f 706f 7274 3d7a 092c 2077 5f70  , r_port=z., w_p
 00000a20: 6f72 743d 7a0a 2c20 7277 5f70 6f72 743d  ort=z., rw_port=
 00000a30: 7a07 2c20 6261 6e6b 3d29 0eda 026f 73da  z., bank=)...os.
 00000a40: 0470 6174 68da 0665 7869 7374 73da 1146  .path..exists..F
 00000a50: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
 00000a60: da06 6c6f 6767 6572 da04 696e 666f 7216  ..logger..infor.
 00000a70: 0000 00da 0570 7269 6e74 7225 0000 0072  .....printr%...r
-00000a80: 2d00 0000 7213 0000 0072 1400 0000 7215  -...r....r....r.
+00000a80: 2e00 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
 00000a90: 0000 00da 134d 6f64 756c 654e 6f74 466f  .....ModuleNotFo
 00000aa0: 756e 6445 7272 6f72 2917 7204 0000 0072  undError).r....r
 00000ab0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
 00000ac0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000ad0: 0000 721e 0000 0072 2b00 0000 721f 0000  ..r....r+...r...
+00000ad0: 0000 721e 0000 0072 2c00 0000 721f 0000  ..r....r,...r...
 00000ae0: 0072 2000 0000 7221 0000 0072 0800 0000  .r ...r!...r....
 00000af0: 7209 0000 0072 0a00 0000 7222 0000 0072  r....r....r"...r
 00000b00: 2300 0000 720f 0000 0072 1000 0000 7211  #...r....r....r.
 00000b10: 0000 0072 2400 0000 7231 0000 0072 0300  ...r$...r1...r..
 00000b20: 0000 7203 0000 0072 0500 0000 da08 6765  ..r....r......ge
 00000b30: 745f 6974 656d 3900 0000 733a 0000 000c  t_item9...s:....
 00000b40: 0110 0116 0208 0204 010c 0108 0116 0218  ................
@@ -187,18 +187,18 @@
 00000ba0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000bb0: 6e61 6d65 5f5f 7232 0000 0072 3300 0000  name__r2...r3...
 00000bc0: da07 6469 726e 616d 65da 0872 6561 6c70  ..dirname..realp
 00000bd0: 6174 68da 085f 5f66 696c 655f 5f5a 0a63  ath..__file__Z.c
 00000be0: 6163 7469 5f70 6174 685a 0d4d 454d 5f50  acti_pathZ.MEM_P
 00000bf0: 4f4f 4c5f 5041 5448 5a0e 4341 4354 495f  OOL_PATHZ.CACTI_
 00000c00: 544f 505f 5041 5448 7206 0000 0072 2500  TOP_PATHr....r%.
-00000c10: 0000 722d 0000 0072 3a00 0000 7203 0000  ..r-...r:...r...
+00000c10: 0000 722e 0000 0072 3a00 0000 7203 0000  ..r....r:...r...
 00000c20: 0072 0300 0000 7203 0000 0072 0500 0000  .r....r....r....
 00000c30: 7202 0000 0008 0000 0073 1000 0000 0800  r........s......
 00000c40: 1402 0a01 0a01 0802 0c03 0e16 1212 7202  ..............r.
 00000c50: 0000 0029 0872 1400 0000 7232 0000 0072  ...).r....r2...r
-00000c60: 2800 0000 5a07 6c6f 6767 696e 675a 0967  (...Z.loggingZ.g
+00000c60: 2800 0000 da07 6c6f 6767 696e 67da 0967  (.....logging..g
 00000c70: 6574 4c6f 6767 6572 723b 0000 0072 3600  etLoggerr;...r6.
 00000c80: 0000 7202 0000 0072 0300 0000 7203 0000  ..r....r....r...
 00000c90: 0072 0300 0000 7205 0000 00da 083c 6d6f  .r....r......<mo
 00000ca0: 6475 6c65 3e01 0000 0073 0c00 0000 0800  dule>....s......
 00000cb0: 0801 0801 0802 0a01 1202                 ..........
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/README` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/README`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/TSV.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/TSV.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/TSV.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/TSV.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/Ucache.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/Ucache.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/Ucache.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/Ucache.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/arbiter.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/arbiter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/arbiter.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/arbiter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/area.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/area.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/area.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/area.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/bank.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/bank.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/bank.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/bank.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/basic_circuit.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/basic_circuit.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/basic_circuit.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/basic_circuit.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cache.cfg_temp` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cache.cfg_temp`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cache_old.cfg.out` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cache_old.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti.mk` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti.mk`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_interface.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_interface.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_interface.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_interface.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/component.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/component.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/component.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/component.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/const.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/const.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/contention.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/contention.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/crossbar.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/crossbar.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/crossbar.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/crossbar.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/ddr3.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/ddr3.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/decoder.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/decoder.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/decoder.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/decoder.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/dram.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/dram.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio_technology.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio_technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/extio_technology.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/extio_technology.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/htree2.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/htree2.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/htree2.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/htree2.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/io.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/io.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/io.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/io.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/lpddr.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/lpddr.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/main.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/main.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/mat.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/mat.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/mat.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/mat.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad_parameters.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad_parameters.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memcad_parameters.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memcad_parameters.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memorybus.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memorybus.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/memorybus.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/memorybus.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/nuca.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/nuca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/nuca.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/nuca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/area.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/area.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/component.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/component.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/io.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/io.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/main.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/main.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/router.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/router.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/parameter.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/parameter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/parameter.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/parameter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/powergating.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/powergating.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/powergating.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/powergating.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/regression.test` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/regression.test`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/router.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/router.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/router.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/router.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/subarray.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/subarray.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/subarray.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/subarray.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/technology.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/uca.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/uca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/uca.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/uca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/version_cacti.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/version_cacti.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/wire.cc` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/wire.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_master/wire.h` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_master/wire.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cacti/cacti_parser.py` & `zigzag-dse-2.3.2/zigzag/classes/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/cost_model/cost_model.py` & `zigzag-dse-2.3.2/zigzag/classes/cost_model/cost_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import logging
 from typing import Dict, List, Tuple
 from math import ceil
 import numpy as np
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
+
 from zigzag.classes.mapping.combined_mapping import Mapping
 from zigzag.classes.mapping.combined_mapping import FourWayDataMoving
-from zigzag.classes.workload.layer_node import LayerNode
 from zigzag.utils import pickle_deepcopy
 
 logger = logging.getLogger(__name__)
 
 
 class PortActivity:
-    """ Class that collects all the data transfer rate (periodic) information for each DTL (data transfer link). """
+    """Class that collects all the data transfer rate (periodic) information for each DTL (data transfer link)."""
 
-    def __init__(self, real_cycle: int, allowed_cycle: int, period: int, period_count: int,
-                 layer_op: str, mem_lv: int, mov_dir: str):
+    def __init__(
+        self,
+        real_cycle: int,
+        allowed_cycle: int,
+        period: int,
+        period_count: int,
+        layer_op: str,
+        mem_lv: int,
+        mov_dir: str,
+    ):
         """
         - real_cycle: within each period, the actual number of cycles used for transferring the amount of data,
                       depended on the memory bw and the data amount to be transferred at that memory level.
         - required_cycle: within each period, the maximal allowed number of cycles for transferring the amount of data,
                           depended on temporal mapping, effective data size and memory size at that memory level.
         - period: the turnaround cycle at that memory level, which equals to the product of all the temporal loops
                   of current and below memory level.
         - period_count: the total number of period across the whole NN layer computation.
         """
         self.real_cycle = real_cycle
         self.allowed_cycle = allowed_cycle
         self.period = period
         self.period_count = period_count
         self.served_op_lv_dir = (layer_op, mem_lv, mov_dir)
-        ''' stalling (+) or slacking (-) cycle in one period '''
+        """ stalling (+) or slacking (-) cycle in one period """
         self.SS_per_period = real_cycle - allowed_cycle
-        ''' stalling (+) or slacking (-) cycle in total computation '''
+        """ stalling (+) or slacking (-) cycle in total computation """
         self.SS = (real_cycle - allowed_cycle) * (period_count - 1)
-        ''' total memory updating window allowed '''
+        """ total memory updating window allowed """
         self.MUW = allowed_cycle * (period_count - 1)
 
     def __str__(self):
         return str(self.served_op_lv_dir)
 
     def __repr__(self):
         return str(self.served_op_lv_dir)
@@ -49,17 +54,25 @@
         return str(self.served_op_lv_dir) == other
 
     def __hash__(self):
         return str(self.served_op_lv_dir)
 
 
 class PortBeginOrEndActivity:
-    """ Class that collects all the data transfer rate information for each DTL (data transfer link). """
+    """Class that collects all the data transfer rate information for each DTL (data transfer link)."""
 
-    def __init__(self, real_cycle: int, data_in_charge: int, mem_bw: int, layer_op: str, mem_lv: int, mov_dir: str):
+    def __init__(
+        self,
+        real_cycle: int,
+        data_in_charge: int,
+        mem_bw: int,
+        layer_op: str,
+        mem_lv: int,
+        mov_dir: str,
+    ):
         """
         - real_cycle: the actual number of cycles used for transferring the amount of data,
                       depended on the memory bw and the data amount to be transferred at that memory level
         - data_in_change: one-period data transfer amount (bit)
         - mem_bw: bit/cycle
         - mov_dir: data moving direction
         """
@@ -72,25 +85,25 @@
         return str(self.served_op_lv_dir)
 
     def __repr__(self):
         return str(self.served_op_lv_dir)
 
 
 def get_shared_mem_list(mem_op, mem_lv, memory_sharing_list) -> List[Tuple]:
-    """ Given a certain operand's storage level (e.g. (A,1): operand A's 1st memory level),
-    return a list of the rest operand's storage levels that share physical memory with the former one (A1) """
+    """Given a certain operand's storage level (e.g. (A,1): operand A's 1st memory level),
+    return a list of the rest operand's storage levels that share physical memory with the former one (A1)"""
     for mem_share_group in memory_sharing_list:
         mem_share_grp = list(mem_share_group.items())
         mem_target = (mem_op, mem_lv)
         if mem_target in mem_share_grp:
             return mem_share_grp
 
 
 def spatial_mapping_fractional_to_int(spatial_mapping: Dict):
-    """ generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
+    """generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
     Later the fractional one is used for calculating energy, and the integer one is used for calculating latency"""
     spatial_mapping_int = pickle_deepcopy(spatial_mapping)
     for op, su_all_lv in spatial_mapping.items():
         if not su_all_lv:
             continue
         for lv, su_one_level in enumerate(su_all_lv):
             for idx, su in enumerate(su_one_level):
@@ -104,58 +117,72 @@
     """
     This function calculates the union length of all the share-port MUW (memory updating window).
     'P' for single period length
     'A' for allowed MUW per period
     'PC' for period count within the whole layer computation
     """
 
-    ''' pre-process the port_duty_list to generate input_dict, which looks like:
-    input_dict = {'O1': {'P': 3, 'A': 1, 'PC': 8}, 'O2': {'P': 6, 'A': 2, 'PC': 4}, 'O3': {'P': 12, 'A': 4, 'PC': 2}}'''
+    """ pre-process the port_duty_list to generate input_dict, which looks like:
+    input_dict = {'O1': {'P': 3, 'A': 1, 'PC': 8}, 'O2': {'P': 6, 'A': 2, 'PC': 4}, 'O3': {'P': 12, 'A': 4, 'PC': 2}}"""
 
     input_dict = {}
     for port_duty in port_duty_list:
-        ''' as long as one of the port duty can make use of the whole computation time, the MUW union is set to 
-        the whole computation time'''
+        """as long as one of the port duty can make use of the whole computation time, the MUW union is set to
+        the whole computation time"""
         if port_duty.period == port_duty.allowed_cycle:
             return port_duty.period * port_duty.period_count
         key = str(port_duty.served_op_lv_dir)
-        input_dict[key] = {'P': port_duty.period, 'A': port_duty.allowed_cycle, 'PC': port_duty.period_count}
+        input_dict[key] = {
+            "P": port_duty.period,
+            "A": port_duty.allowed_cycle,
+            "PC": port_duty.period_count,
+        }
 
     max_period = 0
     max_period_operand = None
     for op in input_dict:
-        if input_dict[op]['P'] > max_period:
-            max_period = input_dict[op]['P']
+        if input_dict[op]["P"] > max_period:
+            max_period = input_dict[op]["P"]
             max_period_operand = op
 
     indicators = np.zeros((len(input_dict), max_period), dtype=np.int8)
     for i, op in enumerate(input_dict):
-        ''' reshape to period of this operand '''
-        indicators_reshape = indicators.reshape((len(input_dict), -1, input_dict[op]['P']))
-        ''' fill in first few time units as used '''
-        indicators_reshape[i, :, :input_dict[op]['A']] = 1
+        """reshape to period of this operand"""
+        indicators_reshape = indicators.reshape(
+            (len(input_dict), -1, input_dict[op]["P"])
+        )
+        """ fill in first few time units as used """
+        indicators_reshape[i, :, : input_dict[op]["A"]] = 1
 
     union = max_period - (~indicators.any(0)).sum(dtype=np.uint64)
 
     # take sum across operands => how many operand need memory for every time unit
     # Subtract 1 => number of stalls
     # Clip by 0 (-1 is not -1 stall)
     # Sum across time units (only remaining axis)
     # stall = (indicators.sum(0, dtype=np.int8) - 1).clip(min=0).sum()
 
-    ''' Multiply with number of periods of largest period (as it was normalized to largest period) '''
-    return union * input_dict[max_period_operand]['PC']
+    """ Multiply with number of periods of largest period (as it was normalized to largest period) """
+    return union * input_dict[max_period_operand]["PC"]
 
 
 class CostModelEvaluation:
     """
     Class that stores inputs and runs them through the zigzag cost model.
     """
 
-    def __init__(self, *, accelerator, layer, spatial_mapping, temporal_mapping, access_same_data_considered_as_no_access=True):
+    def __init__(
+        self,
+        *,
+        accelerator,
+        layer,
+        spatial_mapping,
+        temporal_mapping,
+        access_same_data_considered_as_no_access=True,
+    ):
         """
         Initialize the cost model evaluation with the following inputs:
         - accelerator: the accelerator that includes the core on which to run the layer
         - layer: the layer to run
         - spatial_mapping: the spatial mapping
         - temporal_mapping: the temporal mapping
 
@@ -170,37 +197,65 @@
         After initialization, the cost model evaluation is run.
         """
 
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
         self.temporal_mapping = temporal_mapping
-        self.access_same_data_considered_as_no_access = access_same_data_considered_as_no_access
+        self.access_same_data_considered_as_no_access = (
+            access_same_data_considered_as_no_access
+        )
 
         self.core_id = layer.core_allocation
-        self.mem_instance_list = accelerator.get_core(self.core_id).get_memory_hierarchy().mem_instance_list
-        self.mem_hierarchy_dict = accelerator.get_core(self.core_id).get_memory_hierarchy_dict()
+        self.mem_instance_list = (
+            accelerator.get_core(self.core_id).get_memory_hierarchy().mem_instance_list
+        )
+        self.mem_hierarchy_dict = accelerator.get_core(
+            self.core_id
+        ).get_memory_hierarchy_dict()
         self.mem_size_dict = accelerator.get_core(self.core_id).get_memory_size_dict()
-        self.mem_r_bw_dict, self.mem_w_bw_dict = accelerator.get_core(self.core_id).get_memory_bw_dict()
-        self.mem_r_bw_min_dict, self.mem_w_bw_min_dict = accelerator.get_core(self.core_id).get_memory_bw_min_dict()
-        self.mem_sharing_list = accelerator.get_core(self.core_id).get_memory_sharing_list()
+        self.mem_r_bw_dict, self.mem_w_bw_dict = accelerator.get_core(
+            self.core_id
+        ).get_memory_bw_dict()
+        self.mem_r_bw_min_dict, self.mem_w_bw_min_dict = accelerator.get_core(
+            self.core_id
+        ).get_memory_bw_min_dict()
+        self.mem_sharing_list = accelerator.get_core(
+            self.core_id
+        ).get_memory_sharing_list()
         self.layer_op_to_mem_op = layer.memory_operand_links
-        self.mem_op_to_layer_op = dict([(value, key) for key, value in self.layer_op_to_mem_op.items()])
-
-        ''' generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
-        Later the fractional one is used for calculating energy, and the integer one is used for calculating latency'''
-        self.spatial_mapping_dict_int = spatial_mapping_fractional_to_int(self.spatial_mapping.mapping_dict_origin)
+        self.mem_op_to_layer_op = dict(
+            [(value, key) for key, value in self.layer_op_to_mem_op.items()]
+        )
+
+        """ generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
+        Later the fractional one is used for calculating energy, and the integer one is used for calculating latency"""
+        self.spatial_mapping_dict_int = spatial_mapping_fractional_to_int(
+            self.spatial_mapping.mapping_dict_origin
+        )
 
         # For constructing Mapping object,  the last parameter "self.access_same_data_considered_as_no_access" is optional
-        self.mapping = Mapping(self.accelerator, self.spatial_mapping, self.temporal_mapping, self.layer, self.access_same_data_considered_as_no_access)
-        self.mapping_int = Mapping(self.accelerator, self.spatial_mapping_dict_int, self.temporal_mapping, self.layer, self.access_same_data_considered_as_no_access)
+        self.mapping = Mapping(
+            self.accelerator,
+            self.spatial_mapping,
+            self.temporal_mapping,
+            self.layer,
+            self.access_same_data_considered_as_no_access,
+        )
+        self.mapping_int = Mapping(
+            self.accelerator,
+            self.spatial_mapping_dict_int,
+            self.temporal_mapping,
+            self.layer,
+            self.access_same_data_considered_as_no_access,
+        )
 
         self.active_mem_level = self.mapping.mem_level
 
-        ''' Run the cost model evaluation '''
+        """ Run the cost model evaluation """
         self.run()
 
     def __str__(self):
         return f"CostModelEvaluation(layer={self.layer}, core={self.core_id})"
 
     def __repr__(self):
         return str(self)
@@ -208,46 +263,49 @@
     def __jsonrepr__(self):
         """
         JSON representation used for saving this object to a json file.
         """
         return {
             "outputs": {
                 "memory": {
-                    "utilization": self.mem_utili_shared if hasattr(self, "mem_utili_shared") else None,
-                    "word_accesses": self.memory_word_access
+                    "utilization": self.mem_utili_shared
+                    if hasattr(self, "mem_utili_shared")
+                    else None,
+                    "word_accesses": self.memory_word_access,
                 },
                 "energy": {
-                    "energy_total": self.energy_total, 
+                    "energy_total": self.energy_total,
                     "operational_energy": self.MAC_energy,
                     "memory_energy": self.mem_energy,
                     "energy_breakdown_per_level": self.energy_breakdown,
-                    "energy_breakdown_per_level_per_operand": self.energy_breakdown_further
+                    "energy_breakdown_per_level_per_operand": self.energy_breakdown_further,
                 },
                 "latency": {
-                    "latency_without_onloading_without_offloading": self.latency_total0,
-                    "latency_with_onloading_without_offloading": self.latency_total1,
-                    "latency_with_onloading_with_offloading": self.latency_total2
-                }
+                    "data_onloading": self.latency_total1 - self.latency_total0,
+                    "computation": self.latency_total0,
+                    "data_offloading": self.latency_total2 - self.latency_total1,
+                },
             },
             "inputs": {
                 "accelerator": self.accelerator,
                 "layer": self.layer,
-                "spatial_mapping": self.spatial_mapping if hasattr(self, "spatial_mapping") else None,
-                "temporal_mapping": self.temporal_mapping if hasattr(self, "temporal_mapping") else None,
+                "spatial_mapping": self.spatial_mapping
+                if hasattr(self, "spatial_mapping")
+                else None,
+                "temporal_mapping": self.temporal_mapping
+                if hasattr(self, "temporal_mapping")
+                else None,
             },
         }
 
     def __simplejsonrepr__(self):
         """
         Simple JSON representation used for saving this object to a simple json file.
         """
-        return {
-            "energy": self.energy_total,
-            "latency": self.latency_total2
-        }
+        return {"energy": self.energy_total, "latency": self.latency_total2}
 
     def run(self):
         """
         Run the cost model evaluation.
         - Energy breakdown and energy total through calculate_energy_cost()
         - TODO: Latency calculation
         """
@@ -264,41 +322,53 @@
         """
         mem_utili_individual = {}
         effective_mem_utili_individual = {}
         for layer_op in self.layer.operand_list:
             mem_utili_individual[layer_op] = []
             effective_mem_utili_individual[layer_op] = []
             for mem_lv in range(self.active_mem_level[layer_op]):
-                mem_utilization = self.mapping.data_bit_per_level_unrolled[layer_op][mem_lv + 1] / \
-                                  self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                assert mem_utilization <= 1, f"Operand {layer_op} memory level {mem_lv}'s individual memory utilization is " \
-                                             f"{mem_utilization}, which is larger than 1 " \
-                                             f"(memory level starts from 0)"
+                mem_utilization = (
+                    self.mapping.data_bit_per_level_unrolled[layer_op][mem_lv + 1]
+                    / self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
+                )
+                assert mem_utilization <= 1, (
+                    f"Operand {layer_op} memory level {mem_lv}'s individual memory utilization is "
+                    f"{mem_utilization}, which is larger than 1 "
+                    f"(memory level starts from 0)"
+                )
                 mem_utili_individual[layer_op].append(mem_utilization)
 
                 # if we do not count copied data in parallel memories as effective, what is the utilization then? =>
-                effective_mem_utilization = self.mapping.effective_data_bit[layer_op][mem_lv + 1] / \
-                                            self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                effective_mem_utili_individual[layer_op].append(effective_mem_utilization)
+                effective_mem_utilization = (
+                    self.mapping.effective_data_bit[layer_op][mem_lv + 1]
+                    / self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
+                )
+                effective_mem_utili_individual[layer_op].append(
+                    effective_mem_utilization
+                )
 
         mem_utili_shared = pickle_deepcopy(mem_utili_individual)
         effective_mem_utili_shared = pickle_deepcopy(effective_mem_utili_individual)
         for mem_share_dict in self.mem_sharing_list:
             mem_utilization = 0
             effective_mem_utilization = 0
             for mem_op, mem_lv in mem_share_dict.items():
                 try:
                     layer_op = self.mem_op_to_layer_op[mem_op]
                 except:  # mem to layer op might not contain this mem op (e.g. pooling layer)
                     continue
                 mem_utilization += mem_utili_individual[layer_op][mem_lv]
-                effective_mem_utilization += effective_mem_utili_individual[layer_op][mem_lv]
-            assert mem_utilization <= 1, f"Memory shared by {mem_share_dict} (memory operand, memory level) has shared utilization of " \
-                                        f"{mem_utilization}, which is > 1 " \
-                                        f"(memory level starts from 0)."
+                effective_mem_utilization += effective_mem_utili_individual[layer_op][
+                    mem_lv
+                ]
+            assert mem_utilization <= 1, (
+                f"Memory shared by {mem_share_dict} (memory operand, memory level) has shared utilization of "
+                f"{mem_utilization}, which is > 1 "
+                f"(memory level starts from 0)."
+            )
             for mem_op, mem_lv in mem_share_dict.items():
                 try:
                     layer_op = self.mem_op_to_layer_op[mem_op]
                 except:  # mem to layer op might not contain this mem op (e.g. pooling layer)
                     continue
                 mem_utili_shared[layer_op][mem_lv] = mem_utilization
                 effective_mem_utili_shared[layer_op][mem_lv] = effective_mem_utilization
@@ -312,105 +382,191 @@
         """
         Calculates the memory word access based on unit memory's data element move count and the physical memory bw.
         """
         memory_word_access = {}
         for layer_op in self.layer.operand_list:
             memory_word_access[layer_op] = []
             for mem_lv in range(self.mapping.mem_level[layer_op]):
-                ''' wr_in_by_low '''
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.wr_in_by_low
-                data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_low
+                """wr_in_by_low"""
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
+                    layer_op
+                ][mem_lv].data_trans_amount_per_period.wr_in_by_low
+                data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.wr_in_by_low
                 if data_elem_move_per_period == 0 or data_precision == 0:
                     wr_in_by_low = 0
                 else:
-                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count.wr_in_by_low
-                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
+                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period_count.wr_in_by_low
+                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
                     if mem_lv > 0:
-                        another_side_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv - 1] * \
-                                          (self.spatial_mapping.unit_unique[layer_op][mem_lv] / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1])
-                        data_elem_move_per_cycle_in_a_period = min((another_side_bw/data_precision), (max_bw/data_precision), data_elem_move_per_period)
-                        cycle_in_a_period = ceil(data_elem_move_per_period / data_elem_move_per_cycle_in_a_period)
+                        another_side_bw = self.mem_r_bw_dict[
+                            self.layer_op_to_mem_op[layer_op]
+                        ][mem_lv - 1] * (
+                            self.spatial_mapping.unit_unique[layer_op][mem_lv]
+                            / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1]
+                        )
+                        data_elem_move_per_cycle_in_a_period = min(
+                            (another_side_bw / data_precision),
+                            (max_bw / data_precision),
+                            data_elem_move_per_period,
+                        )
+                        cycle_in_a_period = ceil(
+                            data_elem_move_per_period
+                            / data_elem_move_per_cycle_in_a_period
+                        )
                     else:
                         data_elem_move_per_cycle_in_a_period = data_elem_move_per_period
                         cycle_in_a_period = 1
-                    wr_in_by_low = ceil((data_elem_move_per_cycle_in_a_period * data_precision) / min_bw) * \
-                                   (min_bw / max_bw) * \
-                                   total_period_count * cycle_in_a_period * \
-                                   self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
-
-                ''' rd_out_to_low '''
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.rd_out_to_low
-                data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_low
+                    wr_in_by_low = (
+                        ceil(
+                            (data_elem_move_per_cycle_in_a_period * data_precision)
+                            / min_bw
+                        )
+                        * (min_bw / max_bw)
+                        * total_period_count
+                        * cycle_in_a_period
+                        * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
+                    )
+
+                """ rd_out_to_low """
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
+                    layer_op
+                ][mem_lv].data_trans_amount_per_period.rd_out_to_low
+                data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.rd_out_to_low
                 if data_elem_move_per_period == 0 or data_precision == 0:
                     rd_out_to_low = 0
                 else:
-                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count.rd_out_to_low
-                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
+                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period_count.rd_out_to_low
+                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
                     if mem_lv > 0:
-                        another_side_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv - 1] * \
-                                          (self.spatial_mapping.unit_unique[layer_op][mem_lv] / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1])
-                        data_elem_move_per_cycle_in_a_period = min((another_side_bw/data_precision), (max_bw/data_precision), data_elem_move_per_period)
-                        cycle_in_a_period = ceil(data_elem_move_per_period / data_elem_move_per_cycle_in_a_period)
-                        rd_out_to_low = ceil((data_elem_move_per_cycle_in_a_period * data_precision) / min_bw) * \
-                                        (min_bw / max_bw) * \
-                                        total_period_count * cycle_in_a_period * \
-                                        self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
+                        another_side_bw = self.mem_w_bw_dict[
+                            self.layer_op_to_mem_op[layer_op]
+                        ][mem_lv - 1] * (
+                            self.spatial_mapping.unit_unique[layer_op][mem_lv]
+                            / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1]
+                        )
+                        data_elem_move_per_cycle_in_a_period = min(
+                            (another_side_bw / data_precision),
+                            (max_bw / data_precision),
+                            data_elem_move_per_period,
+                        )
+                        cycle_in_a_period = ceil(
+                            data_elem_move_per_period
+                            / data_elem_move_per_cycle_in_a_period
+                        )
+                        rd_out_to_low = (
+                            ceil(
+                                (data_elem_move_per_cycle_in_a_period * data_precision)
+                                / min_bw
+                            )
+                            * (min_bw / max_bw)
+                            * total_period_count
+                            * cycle_in_a_period
+                            * self.mapping.spatial_mapping.unit_count[layer_op][
+                                mem_lv + 1
+                            ]
+                        )
                     else:
-                        rd_out_to_low = ceil((data_elem_move_per_period * data_precision) / min_bw) * \
-                                        (min_bw / max_bw) * \
-                                        total_period_count * \
-                                        self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
+                        rd_out_to_low = (
+                            ceil((data_elem_move_per_period * data_precision) / min_bw)
+                            * (min_bw / max_bw)
+                            * total_period_count
+                            * self.mapping.spatial_mapping.unit_count[layer_op][
+                                mem_lv + 1
+                            ]
+                        )
 
-                ''' rd_out_to_high '''
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.rd_out_to_high
+                """ rd_out_to_high """
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
+                    layer_op
+                ][mem_lv].data_trans_amount_per_period.rd_out_to_high
                 if data_elem_move_per_period == 0:
                     rd_out_to_high = 0
                 else:
-                    data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_high
-                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count.rd_out_to_high
-                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    rd_out_to_high = ceil((data_elem_move_per_period * data_precision) / min_bw) * \
-                                     (min_bw / max_bw) * \
-                                     total_period_count * \
-                                     self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
-
-                ''' wr_in_by_high '''
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.wr_in_by_high
+                    data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_precision.rd_out_to_high
+                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period_count.rd_out_to_high
+                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    rd_out_to_high = (
+                        ceil((data_elem_move_per_period * data_precision) / min_bw)
+                        * (min_bw / max_bw)
+                        * total_period_count
+                        * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
+                    )
+
+                """ wr_in_by_high """
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
+                    layer_op
+                ][mem_lv].data_trans_amount_per_period.wr_in_by_high
                 if data_elem_move_per_period == 0:
                     wr_in_by_high = 0
                 else:
-                    data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_high
-                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count.wr_in_by_high
-                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                    wr_in_by_high = ceil((data_elem_move_per_period * data_precision) / min_bw) * \
-                                    (min_bw / max_bw) * \
-                                    total_period_count * \
-                                    self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
-
-                ''' All '''
-                memory_word_access_single = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+                    data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_precision.wr_in_by_high
+                    total_period_count = self.mapping.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period_count.wr_in_by_high
+                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
+                        mem_lv
+                    ]
+                    wr_in_by_high = (
+                        ceil((data_elem_move_per_period * data_precision) / min_bw)
+                        * (min_bw / max_bw)
+                        * total_period_count
+                        * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
+                    )
+
+                """ All """
+                memory_word_access_single = FourWayDataMoving(
+                    rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+                )
                 memory_word_access[layer_op].append(memory_word_access_single)
 
         self.memory_word_access = memory_word_access
 
     def calc_energy(self):
         """
         Calculates the energy cost of this cost model evaluation by:
         - calculating the memory reading/writing energy
         - TODO: Interconnection energy
         """
         self.calc_MAC_energy_cost()
         self.calc_memory_energy_cost()
 
     def calc_MAC_energy_cost(self):
-        """ Calculate the dynamic MAC energy """
+        """Calculate the dynamic MAC energy"""
         core = self.accelerator.get_core(self.core_id)
         single_MAC_energy = core.operational_array.unit.cost
         self.MAC_energy = single_MAC_energy * self.layer.total_MAC_count
 
     def calc_memory_energy_cost(self):
         """
         Computes the memories reading/writing energy by converting the access patterns in self.mapping to
@@ -421,35 +577,61 @@
         core = self.accelerator.get_core(self.core_id)
         mem_hierarchy = core.memory_hierarchy
 
         energy_breakdown = {}
         energy_breakdown_further = {}
         energy_total = 0
         for (layer_op, mem_access_list_per_op) in self.memory_word_access.items():
-            ''' Retrieve the memory levels in the hierarchy for this memory operand '''
+            """Retrieve the memory levels in the hierarchy for this memory operand"""
             mem_op = self.layer_op_to_mem_op[layer_op]
             memory_levels = mem_hierarchy.get_memory_levels(mem_op=mem_op)
 
-            breakdown = []  # Stores the energy breakdown of a single layer operand (W, I, ...)
+            breakdown = (
+                []
+            )  # Stores the energy breakdown of a single layer operand (W, I, ...)
             breakdown_further = []  # Stores
-            for (access_count, memory_level) in zip(mem_access_list_per_op, memory_levels):
+            for (access_count, memory_level) in zip(
+                mem_access_list_per_op, memory_levels
+            ):
                 energy_cost_per_read_out = memory_level.read_energy
                 energy_cost_per_write_in = memory_level.write_energy
-                read_out_energy_to_above = access_count.get_total_read_outs_to_above(scaling=energy_cost_per_read_out)
-                write_in_energy_from_above = access_count.get_total_write_ins_from_above(scaling=energy_cost_per_write_in)
-                read_out_energy_to_below = access_count.get_total_read_outs_to_below(scaling=energy_cost_per_read_out)
-                write_in_energy_from_below = access_count.get_total_write_ins_from_below(scaling=energy_cost_per_write_in)
-                total_read_out_energy = read_out_energy_to_above + read_out_energy_to_below
-                total_write_in_energy = write_in_energy_from_above + write_in_energy_from_below
+                read_out_energy_to_above = access_count.get_total_read_outs_to_above(
+                    scaling=energy_cost_per_read_out
+                )
+                write_in_energy_from_above = (
+                    access_count.get_total_write_ins_from_above(
+                        scaling=energy_cost_per_write_in
+                    )
+                )
+                read_out_energy_to_below = access_count.get_total_read_outs_to_below(
+                    scaling=energy_cost_per_read_out
+                )
+                write_in_energy_from_below = (
+                    access_count.get_total_write_ins_from_below(
+                        scaling=energy_cost_per_write_in
+                    )
+                )
+                total_read_out_energy = (
+                    read_out_energy_to_above + read_out_energy_to_below
+                )
+                total_write_in_energy = (
+                    write_in_energy_from_above + write_in_energy_from_below
+                )
                 total_energy_cost_memory = total_read_out_energy + total_write_in_energy
-                breakdown.append(total_energy_cost_memory)  # Here the breakdown only saves the total energy cost per memory level
-                breakdown_further.append(FourWayDataMoving(read_out_energy_to_below,
-                                                           write_in_energy_from_below,
-                                                           read_out_energy_to_above,
-                                                           write_in_energy_from_above))  # here it contains the full split
+                breakdown.append(
+                    total_energy_cost_memory
+                )  # Here the breakdown only saves the total energy cost per memory level
+                breakdown_further.append(
+                    FourWayDataMoving(
+                        read_out_energy_to_below,
+                        write_in_energy_from_below,
+                        read_out_energy_to_above,
+                        write_in_energy_from_above,
+                    )
+                )  # here it contains the full split
                 energy_total += total_energy_cost_memory
             energy_breakdown[layer_op] = breakdown
             energy_breakdown_further[layer_op] = breakdown_further
         self.energy_breakdown = energy_breakdown
         self.energy_breakdown_further = energy_breakdown_further
         self.mem_energy = energy_total
         self.energy_total = self.mem_energy + self.MAC_energy
@@ -476,148 +658,220 @@
         self.calc_double_buffer_flag()
         self.calc_allowed_and_real_data_transfer_cycle_per_DTL()
         self.combine_data_transfer_rate_per_physical_port()
         self.calc_data_loading_offloading_latency()
         self.calc_overall_latency()
 
     def calc_double_buffer_flag(self):
-        """ This function checks the double-buffer possibility for each operand at each memory level
+        """This function checks the double-buffer possibility for each operand at each memory level
         (minimal memory BW requirement case) by comparing the physical memory size with the effective
-        data size, taking into account the memory sharing between operands. """
+        data size, taking into account the memory sharing between operands."""
         double_buffer_true = {}
         for layer_op in self.layer.operand_list:
             mem_op = self.layer_op_to_mem_op[layer_op]
-            ''' start with False for each operand at the lowest arch level (MAC array level) '''
+            """ start with False for each operand at the lowest arch level (MAC array level) """
             double_buffer_true[layer_op] = [False]
             for mem_lv in range(0, self.mapping_int.mem_level[layer_op]):
                 if self.effective_mem_utili_shared[layer_op][mem_lv] <= 0.5:
                     double_buffer_true[layer_op].append(True)
-                elif self.effective_mem_utili_individual[layer_op][mem_lv] <= 1 - self.effective_mem_utili_shared[layer_op][mem_lv]:
+                elif (
+                    self.effective_mem_utili_individual[layer_op][mem_lv]
+                    <= 1 - self.effective_mem_utili_shared[layer_op][mem_lv]
+                ):
                     double_buffer_true[layer_op].append(True)
-                    shared_mem_list = get_shared_mem_list(mem_op, mem_lv, self.mem_sharing_list)
-                    ''' When one of the operand in the shared memory get the "double-buffer" chance, 
+                    shared_mem_list = get_shared_mem_list(
+                        mem_op, mem_lv, self.mem_sharing_list
+                    )
+                    """ When one of the operand in the shared memory get the "double-buffer" chance, 
                     all operands of that shared memory level need to update the memory utilization 
-                    for later memory free space evaluation '''
+                    for later memory free space evaluation """
                     for shared_mem_op, shared_mem_lv in shared_mem_list:
                         try:
                             shared_layer_op = self.mem_op_to_layer_op[shared_mem_op]
                         except:  # mem op to layer op might not have this mem op (e.g. pooling layer)
                             continue
-                        self.effective_mem_utili_shared[shared_layer_op][shared_mem_lv] += \
-                            self.effective_mem_utili_individual[layer_op][mem_lv]
+                        self.effective_mem_utili_shared[shared_layer_op][
+                            shared_mem_lv
+                        ] += self.effective_mem_utili_individual[layer_op][mem_lv]
                 else:
                     double_buffer_true[layer_op].append(False)
 
         self.double_buffer_true = double_buffer_true
 
     def calc_allowed_and_real_data_transfer_cycle_per_DTL(self):
         """
         Construct a 4-way data transfer pattern for each unit mem, calculate
         {allowed_mem_updating_cycle, real_data_trans_cycle, DTL_SS_cycle} per period
         """
         allowed_mem_updat_cycle = {}
         real_data_trans_cycle = {}
-        ''' stall (+) or slack (-) cycle within each period per virtual data transfer link (DTL) '''
+        """ stall (+) or slack (-) cycle within each period per virtual data transfer link (DTL) """
         DTL_SS_cycle = {}
 
         for layer_op in self.layer.operand_list:
             allowed_mem_updat_cycle[layer_op] = []
             real_data_trans_cycle[layer_op] = []
             DTL_SS_cycle[layer_op] = []
             mem_op = self.layer_op_to_mem_op[layer_op]
             for mem_lv in range(self.mapping_int.mem_level[layer_op]):
-                ''' ======================================allowed_mem_updating_cycle(below)===================================== '''
-                ''' wr_in_by_low & rd_out_to_low'''
+                """======================================allowed_mem_updating_cycle(below)====================================="""
+                """ wr_in_by_low & rd_out_to_low"""
                 if self.double_buffer_true[layer_op][mem_lv]:
-                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period.wr_in_by_low
-                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period.rd_out_to_low
+                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].data_trans_period.wr_in_by_low
+                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].data_trans_period.rd_out_to_low
                 else:
-                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].inst_data_trans_window.wr_in_by_low
-                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].inst_data_trans_window.rd_out_to_low
+                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].inst_data_trans_window.wr_in_by_low
+                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].inst_data_trans_window.rd_out_to_low
 
-                ''' wr_in_by_high & rd_out_to_high '''
+                """ wr_in_by_high & rd_out_to_high """
                 if self.double_buffer_true[layer_op][mem_lv + 1]:
-                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period.wr_in_by_high
-                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period.rd_out_to_high
+                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].data_trans_period.wr_in_by_high
+                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].data_trans_period.rd_out_to_high
                 else:
-                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].inst_data_trans_window.wr_in_by_high
-                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].inst_data_trans_window.rd_out_to_high
-
-                ''' All '''
-                updating_window = FourWayDataMoving(rd_out_to_low_allowed, wr_in_by_low_allowed,
-                                                    rd_out_to_high_allowed, wr_in_by_high_allowed)
+                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].inst_data_trans_window.wr_in_by_high
+                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[
+                        layer_op
+                    ][mem_lv].inst_data_trans_window.rd_out_to_high
+
+                """ All """
+                updating_window = FourWayDataMoving(
+                    rd_out_to_low_allowed,
+                    wr_in_by_low_allowed,
+                    rd_out_to_high_allowed,
+                    wr_in_by_high_allowed,
+                )
                 allowed_mem_updat_cycle[layer_op].append(updating_window)
-                ''' ======================================allowed_mem_updating_cycle(above)===================================== '''
+                """ ======================================allowed_mem_updating_cycle(above)===================================== """
 
-                ''' =========================================real_data_trans_cycle(below)======================================== '''
-                ''' wr_in_by_low '''
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_low
-                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.wr_in_by_low
+                """ =========================================real_data_trans_cycle(below)======================================== """
+                """ wr_in_by_low """
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.wr_in_by_low
+                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.wr_in_by_low
                 mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                 wr_in_by_low_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                ''' rd_out_to_low '''
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_low
-                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.rd_out_to_low
+                """ rd_out_to_low """
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.rd_out_to_low
+                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.rd_out_to_low
                 mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                 rd_out_to_low_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                ''' rd_out_to_high '''
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_high
-                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.rd_out_to_high
+                """ rd_out_to_high """
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.rd_out_to_high
+                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.rd_out_to_high
                 mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                 rd_out_to_high_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                ''' wr_in_by_high '''
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_high
-                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period.wr_in_by_high
+                """ wr_in_by_high """
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_precision.wr_in_by_high
+                data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.wr_in_by_high
                 mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                 wr_in_by_high_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                ''' All '''
-                real_data_trans = FourWayDataMoving(rd_out_to_low_real, wr_in_by_low_real,
-                                                    rd_out_to_high_real, wr_in_by_high_real)
+                """ All """
+                real_data_trans = FourWayDataMoving(
+                    rd_out_to_low_real,
+                    wr_in_by_low_real,
+                    rd_out_to_high_real,
+                    wr_in_by_high_real,
+                )
                 real_data_trans_cycle[layer_op].append(real_data_trans)
-                ''' =========================================real_data_trans_cycle(above)======================================= '''
+                """ =========================================real_data_trans_cycle(above)======================================= """
 
         self.allowed_mem_updat_cycle = allowed_mem_updat_cycle
         self.real_data_trans_cycle = real_data_trans_cycle
 
     def combine_data_transfer_rate_per_physical_port(self):
-        """ Consider memory sharing and port sharing, combine the data transfer activity """
+        """Consider memory sharing and port sharing, combine the data transfer activity"""
 
-        ''' Step 1: collect port activity per memory instance per physical memory port '''
+        """ Step 1: collect port activity per memory instance per physical memory port """
         port_activity_collect = []
         for mem_instance in self.mem_instance_list:
             port_activity_single = {}
             port_list = mem_instance.port_list
             for port in port_list:
                 port_activity_single[str(port)] = []
                 for mem_op, mem_lv, mov_dir in port.served_op_lv_dir:
                     try:
                         layer_op = self.mem_op_to_layer_op[mem_op]
                     except:  # mem op to layer might not have this mem op (e.g. pooling layer)
                         continue
-                    period_count = getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count, mov_dir)
+                    period_count = getattr(
+                        self.mapping_int.unit_mem_data_movement[layer_op][
+                            mem_lv
+                        ].data_trans_period_count,
+                        mov_dir,
+                    )
                     if period_count == 0:
-                        ''' skip the inactive data movement activities because they won't impact SS '''
+                        """skip the inactive data movement activities because they won't impact SS"""
                         continue
-                    period = getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period, mov_dir)
-                    real_cycle = getattr(self.real_data_trans_cycle[layer_op][mem_lv], mov_dir)
-                    allowed_cycle = getattr(self.allowed_mem_updat_cycle[layer_op][mem_lv], mov_dir)
-                    port_activity = PortActivity(real_cycle, allowed_cycle, period, period_count, layer_op, mem_lv, mov_dir)
+                    period = getattr(
+                        self.mapping_int.unit_mem_data_movement[layer_op][
+                            mem_lv
+                        ].data_trans_period,
+                        mov_dir,
+                    )
+                    real_cycle = getattr(
+                        self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
+                    )
+                    allowed_cycle = getattr(
+                        self.allowed_mem_updat_cycle[layer_op][mem_lv], mov_dir
+                    )
+                    port_activity = PortActivity(
+                        real_cycle,
+                        allowed_cycle,
+                        period,
+                        period_count,
+                        layer_op,
+                        mem_lv,
+                        mov_dir,
+                    )
                     port_activity_single[str(port)].append(port_activity)
             port_activity_collect.append(port_activity_single)
         self.port_activity_collect = port_activity_collect
 
-        ''' Step 2: calculate SS combine and MUW union parameters per physical memory port '''
-        SS_comb_collect = [{port: None for port in mem_ports} for mem_ports in port_activity_collect]
+        """ Step 2: calculate SS combine and MUW union parameters per physical memory port """
+        SS_comb_collect = [
+            {port: None for port in mem_ports} for mem_ports in port_activity_collect
+        ]
         SS_comb_list = [0]
         # intermediate parameters saved for debugging purpose
-        MUW_union_collect = [{port: None for port in mem_ports} for mem_ports in port_activity_collect]
+        MUW_union_collect = [
+            {port: None for port in mem_ports} for mem_ports in port_activity_collect
+        ]
 
         for idx, mem_ports in enumerate(port_activity_collect):
             for port_name, port_activity in mem_ports.items():
                 if len(port_activity) == 1:
                     MUW_union_collect[idx][port_name] = port_activity[0].allowed_cycle
                     SS_comb_collect[idx][port_name] = port_activity[0].SS
                     SS_comb_list.append(port_activity[0].SS)
@@ -628,171 +882,241 @@
                     MUW_sum = 0
                     for port_d in port_activity:
                         if port_d.SS > 0:
                             SS_positive_sum += port_d.SS
                         else:
                             SS_negative_sum += port_d.SS
                         MUW_sum += port_d.MUW
-                    SS_comb = SS_positive_sum + max(0, SS_negative_sum + MUW_sum - MUW_union_collect[idx][port_name])
+                    SS_comb = SS_positive_sum + max(
+                        0, SS_negative_sum + MUW_sum - MUW_union_collect[idx][port_name]
+                    )
                     SS_comb_collect[idx][port_name] = SS_comb
                     SS_comb_list.append(SS_comb)
 
         self.MUW_union_collect = MUW_union_collect
         self.SS_comb_collect = SS_comb_collect
-        ''' Assuming all the memory ports can work in parallel '''
+        """ Assuming all the memory ports can work in parallel """
         self.SS_comb = max(SS_comb_list)
 
     def calc_data_loading_offloading_latency(self):
-        """ Calculate the initial/final data loading/off-loading cycle by separating out
+        """Calculate the initial/final data loading/off-loading cycle by separating out
         the first-time input operands' / the last-time output operand's data movement
-        on corresponding ports. """
+        on corresponding ports."""
 
-        ''' Collect ports' initial data-loading and final data-offloading activities '''
+        """ Collect ports' initial data-loading and final data-offloading activities """
         data_loading_per_mem_inst = []
         data_loading_cc_per_op = {op: {} for op in self.layer.input_operands}
         data_offloading_per_mem_inst = []
         data_offloading_cc_per_op = {}
         for mem_inst_idx, mem_instance in enumerate(self.mem_instance_list):
             data_loading_single = {}
             data_offloading_single = {}
             port_list = mem_instance.port_list
             for port in port_list:
                 data_loading_single[str(port)] = []
                 data_offloading_single[str(port)] = []
-                served_operands = set(s[0] for s in port.served_op_lv_dir if s[0] in ['I1', 'I2'])
+                served_operands = set(
+                    s[0] for s in port.served_op_lv_dir if s[0] in ["I1", "I2"]
+                )
                 port_is_shared_by_two_input_operands = len(served_operands) > 1
                 for mem_op, mem_lv, mov_dir in port.served_op_lv_dir:
                     try:
                         layer_op = self.mem_op_to_layer_op[mem_op]
                     except:  # mem op to layer op might not have this mem op (e.g. pooling layer)
                         continue
-                    period_count = getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count, mov_dir)
+                    period_count = getattr(
+                        self.mapping_int.unit_mem_data_movement[layer_op][
+                            mem_lv
+                        ].data_trans_period_count,
+                        mov_dir,
+                    )
                     if period_count == 0:
-                        ''' skip for the inactive data movement '''
+                        """skip for the inactive data movement"""
                         continue
-                    if mem_op in ['I1', 'I2']:
-                        real_cycle = getattr(self.real_data_trans_cycle[layer_op][mem_lv], mov_dir)
-                        data_in_charge = \
-                            getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period, mov_dir) * \
-                            getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision, mov_dir)
-                        if mov_dir[:2] == 'rd':
+                    if mem_op in ["I1", "I2"]:
+                        real_cycle = getattr(
+                            self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
+                        )
+                        data_in_charge = getattr(
+                            self.mapping_int.unit_mem_data_movement[layer_op][
+                                mem_lv
+                            ].data_trans_amount_per_period,
+                            mov_dir,
+                        ) * getattr(
+                            self.mapping_int.unit_mem_data_movement[layer_op][
+                                mem_lv
+                            ].data_precision,
+                            mov_dir,
+                        )
+                        if mov_dir[:2] == "rd":
                             mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                         else:
                             mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                         port_activity = PortBeginOrEndActivity(
-                            real_cycle, data_in_charge, mem_bw, layer_op, mem_lv, mov_dir
+                            real_cycle,
+                            data_in_charge,
+                            mem_bw,
+                            layer_op,
+                            mem_lv,
+                            mov_dir,
                         )
                         data_loading_single[str(port)].append(port_activity)
-                        data_loading_cc_per_op[layer_op][layer_op + str(mem_lv) + '_' + mov_dir] = \
-                            (real_cycle, port_is_shared_by_two_input_operands)
+                        data_loading_cc_per_op[layer_op][
+                            layer_op + str(mem_lv) + "_" + mov_dir
+                        ] = (real_cycle, port_is_shared_by_two_input_operands)
                     else:
-                        if mov_dir in ['rd_out_to_low', 'wr_in_by_high']:
-                            ''' don't consider partial sum flowing in the final data off-loading stage '''
+                        if mov_dir in ["rd_out_to_low", "wr_in_by_high"]:
+                            """don't consider partial sum flowing in the final data off-loading stage"""
                             continue
-                        real_cycle = getattr(self.real_data_trans_cycle[layer_op][mem_lv], mov_dir)
-                        data_in_charge = \
-                            getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_amount_per_period, mov_dir) * \
-                            getattr(self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision, mov_dir)
-                        if mov_dir[:2] == 'rd':
+                        real_cycle = getattr(
+                            self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
+                        )
+                        data_in_charge = getattr(
+                            self.mapping_int.unit_mem_data_movement[layer_op][
+                                mem_lv
+                            ].data_trans_amount_per_period,
+                            mov_dir,
+                        ) * getattr(
+                            self.mapping_int.unit_mem_data_movement[layer_op][
+                                mem_lv
+                            ].data_precision,
+                            mov_dir,
+                        )
+                        if mov_dir[:2] == "rd":
                             mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                         else:
                             mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                         port_activity = PortBeginOrEndActivity(
-                            real_cycle, data_in_charge, mem_bw, layer_op, mem_lv, mov_dir
+                            real_cycle,
+                            data_in_charge,
+                            mem_bw,
+                            layer_op,
+                            mem_lv,
+                            mov_dir,
                         )
                         data_offloading_single[str(port)].append(port_activity)
-                        data_offloading_cc_per_op[layer_op + str(mem_lv) + '_' + mov_dir] = real_cycle
+                        data_offloading_cc_per_op[
+                            layer_op + str(mem_lv) + "_" + mov_dir
+                        ] = real_cycle
 
             data_loading_per_mem_inst.append(data_loading_single)
             data_offloading_per_mem_inst.append(data_offloading_single)
         self.data_loading_per_mem_inst = data_loading_per_mem_inst
         self.data_loading_cc_per_op = data_loading_cc_per_op
         self.data_offloading_per_mem_inst = data_offloading_per_mem_inst
         self.data_offloading_per_op = data_offloading_cc_per_op
 
-        ''' Combine ports' initial data-loading activities to get the data loading cycle amount '''
-        data_loading_cc_pair_combined_per_op = {op: [] for op in self.layer.input_operands}
+        """ Combine ports' initial data-loading activities to get the data loading cycle amount """
+        data_loading_cc_pair_combined_per_op = {
+            op: [] for op in self.layer.input_operands
+        }
         data_loading_individual_part = {op: 0 for op in self.layer.input_operands}
         data_loading_half_shared_part = {op: 0 for op in self.layer.input_operands}
         data_loading_shared_part = {op: 0 for op in self.layer.input_operands}
         for layer_op in self.layer.input_operands:
             for mem_lv in range(self.active_mem_level[layer_op] - 1):
-                elem1 = data_loading_cc_per_op[layer_op][layer_op + str(mem_lv) + '_' + 'wr_in_by_high']
-                elem2 = data_loading_cc_per_op[layer_op][layer_op + str(mem_lv + 1) + '_' + 'rd_out_to_low']
+                elem1 = data_loading_cc_per_op[layer_op][
+                    layer_op + str(mem_lv) + "_" + "wr_in_by_high"
+                ]
+                elem2 = data_loading_cc_per_op[layer_op][
+                    layer_op + str(mem_lv + 1) + "_" + "rd_out_to_low"
+                ]
                 completely_shared = elem1[1] and elem2[1]
                 completely_separate = not (elem1[1]) and not (elem2[1])
                 longest_loading_cc = max(elem1[0], elem2[0])
-                ''' for the ports that serve the same data movement purpose, take the longest data loading cycle '''
+                """ for the ports that serve the same data movement purpose, take the longest data loading cycle """
                 data_loading_cc_pair_combined = longest_loading_cc
-                data_loading_cc_pair_combined_per_op[layer_op].append(data_loading_cc_pair_combined)
+                data_loading_cc_pair_combined_per_op[layer_op].append(
+                    data_loading_cc_pair_combined
+                )
                 if completely_separate:
                     data_loading_individual_part[layer_op] += longest_loading_cc
                 elif completely_shared:
                     data_loading_shared_part[layer_op] += longest_loading_cc
                 else:
-                    ''' the data transfer link between two memory levels is half-shared, 
-                    i.e. on one memory side, the port is shared, while on another memory side, 
-                    there are different memories with separate ports '''
+                    """the data transfer link between two memory levels is half-shared,
+                    i.e. on one memory side, the port is shared, while on another memory side,
+                    there are different memories with separate ports"""
                     data_loading_half_shared_part[layer_op] = longest_loading_cc
 
         if len(self.layer.input_operands) == 1:
-            data_loading_cycle = data_loading_individual_part[self.layer.input_operands[0]]
+            data_loading_cycle = data_loading_individual_part[
+                self.layer.input_operands[0]
+            ]
         else:
             op1 = self.layer.input_operands[0]
             op2 = self.layer.input_operands[1]
-            possible1 = data_loading_shared_part[op1] + \
-                        max(data_loading_shared_part[op2] + data_loading_half_shared_part[op2] + data_loading_individual_part[op2],
-                            data_loading_half_shared_part[op1] + data_loading_individual_part[op1])
-            possible2 = data_loading_shared_part[op2] + \
-                        max(data_loading_shared_part[op1] + data_loading_half_shared_part[op1] + data_loading_individual_part[op1],
-                            data_loading_half_shared_part[op2] + data_loading_individual_part[op2])
+            possible1 = data_loading_shared_part[op1] + max(
+                data_loading_shared_part[op2]
+                + data_loading_half_shared_part[op2]
+                + data_loading_individual_part[op2],
+                data_loading_half_shared_part[op1] + data_loading_individual_part[op1],
+            )
+            possible2 = data_loading_shared_part[op2] + max(
+                data_loading_shared_part[op1]
+                + data_loading_half_shared_part[op1]
+                + data_loading_individual_part[op1],
+                data_loading_half_shared_part[op2] + data_loading_individual_part[op2],
+            )
             data_loading_cycle = min(possible1, possible2)
 
         self.data_loading_cc_pair_combined_per_op = data_loading_cc_pair_combined_per_op
         self.data_loading_individual_part = data_loading_individual_part
         self.data_loading_half_shared_part = data_loading_half_shared_part
         self.data_loading_shared_part = data_loading_shared_part
         self.data_loading_cycle = data_loading_cycle
 
-        ''' Combine ports' final data-offloading activities to get the data offloading cycle amount '''
+        """ Combine ports' final data-offloading activities to get the data offloading cycle amount """
         # TODO Only considered the worst case for now
         #  (assumed that all the ports are working in series during the final data off-loading phase)
         data_offloading_cc_pair_combined = []
         layer_op = self.layer.output_operand
         for mem_lv in range(self.active_mem_level[layer_op] - 1):
-            elem1 = data_offloading_cc_per_op[layer_op + str(mem_lv) + '_' + 'rd_out_to_high']
-            elem2 = data_offloading_cc_per_op[layer_op + str(mem_lv + 1) + '_' + 'wr_in_by_low']
+            elem1 = data_offloading_cc_per_op[
+                layer_op + str(mem_lv) + "_" + "rd_out_to_high"
+            ]
+            elem2 = data_offloading_cc_per_op[
+                layer_op + str(mem_lv + 1) + "_" + "wr_in_by_low"
+            ]
             longest_offloading_cc = max(elem1, elem2)
-            ''' for the ports that serve the same data movement purpose, take the longest data loading cycle '''
+            """ for the ports that serve the same data movement purpose, take the longest data loading cycle """
             data_offloading_cc_pair_combined.append(longest_offloading_cc)
         data_offloading_cycle = sum(data_offloading_cc_pair_combined)
 
         self.data_offloading_cc_pair_combined = data_offloading_cc_pair_combined
         self.data_offloading_cycle = data_offloading_cycle
 
     def calc_overall_latency(self):
-        """ This function integrates the previous calculated SScomb, data loading and off-loading cycle to get the overall latency """
+        """This function integrates the previous calculated SScomb, data loading and off-loading cycle to get the overall latency"""
 
-        ''' the ideal cycle count assuming the MAC array is 100% utilized '''
-        ideal_cycle = ceil(self.layer.total_MAC_count / self.accelerator.get_core(self.core_id).operational_array.total_unit_count)
+        """ the ideal cycle count assuming the MAC array is 100% utilized """
+        ideal_cycle = ceil(
+            self.layer.total_MAC_count
+            / self.accelerator.get_core(self.core_id).operational_array.total_unit_count
+        )
 
-        ''' the ideal temporal cycle count given the spatial mapping (the spatial mapping can be non-ideal) '''
+        """ the ideal temporal cycle count given the spatial mapping (the spatial mapping can be non-ideal) """
         ideal_temporal_cycle = self.mapping_int.temporal_mapping.total_cycle
         MAC_spatial_utilization = ideal_cycle / ideal_temporal_cycle
 
-        ''' Total latency without the initial data loading and the final data off-loading '''
+        """ Total latency without the initial data loading and the final data off-loading """
         latency_total0 = ideal_temporal_cycle + self.SS_comb
         MAC_utilization0 = ideal_cycle / latency_total0
 
-        ''' Total latency with the initial data loading, but without the final data off-loading '''
+        """ Total latency with the initial data loading, but without the final data off-loading """
         latency_total1 = ideal_temporal_cycle + self.SS_comb + self.data_loading_cycle
         MAC_utilization1 = ideal_cycle / latency_total1
 
-        ''' Total latency with both the initial data loading and the final data off-loading '''
-        latency_total2 = ideal_temporal_cycle + self.SS_comb + self.data_loading_cycle + self.data_offloading_cycle
+        """ Total latency with both the initial data loading and the final data off-loading """
+        latency_total2 = (
+            ideal_temporal_cycle
+            + self.SS_comb
+            + self.data_loading_cycle
+            + self.data_offloading_cycle
+        )
         MAC_utilization2 = ideal_cycle / latency_total2
 
         self.ideal_cycle = ideal_cycle
         self.ideal_temporal_cycle = ideal_temporal_cycle
         self.MAC_spatial_utilization = MAC_spatial_utilization
         self.latency_total0 = latency_total0
         self.latency_total1 = latency_total1
@@ -806,27 +1130,42 @@
 
         ## Energy
         sum.MAC_energy += other.MAC_energy
         sum.mem_energy += other.mem_energy
         for op in sum.energy_breakdown.keys():
             if op in other.energy_breakdown.keys():
                 l = []
-                for i in range(min(len(self.energy_breakdown[op]), len(other.energy_breakdown[op]))):
-                    l.append(self.energy_breakdown[op][i] + other.energy_breakdown[op][i])
+                for i in range(
+                    min(len(self.energy_breakdown[op]), len(other.energy_breakdown[op]))
+                ):
+                    l.append(
+                        self.energy_breakdown[op][i] + other.energy_breakdown[op][i]
+                    )
                 i = min(len(self.energy_breakdown[op]), len(other.energy_breakdown[op]))
                 l += self.energy_breakdown[op][i:]
                 l += other.energy_breakdown[op][i:]
                 sum.energy_breakdown[op] = l
 
         for op in sum.energy_breakdown_further.keys():
             if op in other.energy_breakdown_further.keys():
                 l = []
-                for i in range(min(len(self.energy_breakdown_further[op]), len(other.energy_breakdown_further[op]))):
-                    l.append(self.energy_breakdown_further[op][i] + other.energy_breakdown_further[op][i])
-                i = min(len(self.energy_breakdown_further[op]), len(other.energy_breakdown_further[op]))
+                for i in range(
+                    min(
+                        len(self.energy_breakdown_further[op]),
+                        len(other.energy_breakdown_further[op]),
+                    )
+                ):
+                    l.append(
+                        self.energy_breakdown_further[op][i]
+                        + other.energy_breakdown_further[op][i]
+                    )
+                i = min(
+                    len(self.energy_breakdown_further[op]),
+                    len(other.energy_breakdown_further[op]),
+                )
                 l += self.energy_breakdown_further[op][i:]
                 l += other.energy_breakdown_further[op][i:]
                 sum.energy_breakdown_further[op] = l
 
         # Get all the operands from other that are not in self and add them to the energy breakdown aswell
         op_diff = set(other.energy_breakdown.keys()) - set(self.energy_breakdown.keys())
         for op in op_diff:
@@ -835,17 +1174,26 @@
 
         sum.energy_total += other.energy_total
 
         ## Memory access
         for op in sum.memory_word_access.keys():
             if op in other.memory_word_access.keys():
                 l = []
-                for i in range(min(len(self.memory_word_access[op]), len(other.memory_word_access[op]))):
-                    l.append(self.memory_word_access[op][i] + other.memory_word_access[op][i])
-                i = min(len(self.memory_word_access[op]), len(other.memory_word_access[op]))
+                for i in range(
+                    min(
+                        len(self.memory_word_access[op]),
+                        len(other.memory_word_access[op]),
+                    )
+                ):
+                    l.append(
+                        self.memory_word_access[op][i] + other.memory_word_access[op][i]
+                    )
+                i = min(
+                    len(self.memory_word_access[op]), len(other.memory_word_access[op])
+                )
                 l += self.memory_word_access[op][i:]
                 l += other.memory_word_access[op][i:]
                 sum.memory_word_access[op] = l
         for op in op_diff:
             sum.memory_word_access[op] = other.memory_word_access[op]
 
         ## Latency
@@ -874,59 +1222,94 @@
         if type(sum.core_id) != list:
             sum.core_id = [sum.core_id]
         if type(other.layer) != list:
             other_core_id = [other.core_id]
         sum.core_id += other_core_id
 
         ## Not addable
-        func = ['calc_allowed_and_real_data_transfer_cycle_per_DTL', 'calc_data_loading_offloading_latency', 'calc_double_buffer_flag',
-                'calc_overall_latency', 'calc_MAC_energy_cost', 'calc_energy', 'calc_latency', 'calc_memory_energy_cost',
-                'calc_memory_utilization', 'calc_memory_word_access', 'combine_data_transfer_rate_per_physical_port', 'run']
-        add_attr = ['MAC_energy', 'mem_energy', 'energy_breakdown', 'energy_breakdown_further', 'energy_total', 'memory_word_access',
-                    'data_loading_cycle', 'data_offloading_cycle', 'ideal_cycle', 'ideal_temporal_cycle', 'latency_total0', 'latency_total1',
-                    'latency_total2', 'MAC_spatial_utilization', 'MAC_utilization0', 'MAC_utilization1', 'MAC_utilization2', 'layer', 'core_id']
+        func = [
+            "calc_allowed_and_real_data_transfer_cycle_per_DTL",
+            "calc_data_loading_offloading_latency",
+            "calc_double_buffer_flag",
+            "calc_overall_latency",
+            "calc_MAC_energy_cost",
+            "calc_energy",
+            "calc_latency",
+            "calc_memory_energy_cost",
+            "calc_memory_utilization",
+            "calc_memory_word_access",
+            "combine_data_transfer_rate_per_physical_port",
+            "run",
+        ]
+        add_attr = [
+            "MAC_energy",
+            "mem_energy",
+            "energy_breakdown",
+            "energy_breakdown_further",
+            "energy_total",
+            "memory_word_access",
+            "data_loading_cycle",
+            "data_offloading_cycle",
+            "ideal_cycle",
+            "ideal_temporal_cycle",
+            "latency_total0",
+            "latency_total1",
+            "latency_total2",
+            "MAC_spatial_utilization",
+            "MAC_utilization0",
+            "MAC_utilization1",
+            "MAC_utilization2",
+            "layer",
+            "core_id",
+        ]
 
-        if hasattr(self, 'accelerator') and hasattr(other, 'accelerator'):
+        if hasattr(self, "accelerator") and hasattr(other, "accelerator"):
             if self.accelerator.name.startswith(other.accelerator.name):
                 sum.accelerator = other.accelerator
-                add_attr.append('accelerator')
+                add_attr.append("accelerator")
             elif other.accelerator.name.startswith(self.accelerator.name):
-                add_attr.append('accelerator')
+                add_attr.append("accelerator")
         else:
             pass
 
         for attr in dir(sum):
-            if attr not in (func + add_attr) and attr[0] != '_':
+            if attr not in (func + add_attr) and attr[0] != "_":
                 delattr(sum, attr)
 
         return sum
 
     def __mul__(self, number):
         mul = pickle_deepcopy(self)
 
         # Energy
         mul.MAC_energy *= number
         mul.mem_energy *= number
         mul.energy_breakdown = {
             op: [
-                mul.energy_breakdown[op][i] * number for i in range(len(mul.energy_breakdown[op]))
-            ] for op in mul.energy_breakdown.keys()
+                mul.energy_breakdown[op][i] * number
+                for i in range(len(mul.energy_breakdown[op]))
+            ]
+            for op in mul.energy_breakdown.keys()
         }
         mul.energy_breakdown_further = {
             op: [
-                mul.energy_breakdown_further[op][i] * number for i in range(len(mul.energy_breakdown_further[op]))
-            ] for op in mul.energy_breakdown_further.keys()
+                mul.energy_breakdown_further[op][i] * number
+                for i in range(len(mul.energy_breakdown_further[op]))
+            ]
+            for op in mul.energy_breakdown_further.keys()
         }
         mul.energy_total *= number
 
         # Memory access
         mul.memory_word_access = {
             op: [
-                mul.memory_word_access[op][i] * number for i in range(len(mul.memory_word_access[op]))
-            ] for op in mul.memory_word_access.keys()
+                mul.memory_word_access[op][i] * number
+                for i in range(len(mul.memory_word_access[op]))
+            ]
+            for op in mul.memory_word_access.keys()
         }
 
         # Latency
         mul.data_loading_cycle *= number
         mul.data_offloading_cycle *= number
         mul.ideal_cycle *= number
         mul.ideal_temporal_cycle *= number
@@ -937,20 +1320,48 @@
         # MAC utilization
         mul.MAC_spatial_utilization = mul.ideal_cycle / mul.ideal_temporal_cycle
         mul.MAC_utilization0 = mul.ideal_cycle / mul.latency_total0
         mul.MAC_utilization1 = mul.ideal_cycle / mul.latency_total1
         mul.MAC_utilization2 = mul.ideal_cycle / mul.latency_total2
 
         # Not addable
-        func = ['calc_allowed_and_real_data_transfer_cycle_per_DTL', 'calc_data_loading_offloading_latency', 'calc_double_buffer_flag',
-                'calc_overall_latency', 'calc_MAC_energy_cost', 'calc_energy', 'calc_latency', 'calc_memory_energy_cost',
-                'calc_memory_utilization', 'calc_memory_word_access', 'combine_data_transfer_rate_per_physical_port', 'run']
-        mul_attr = ['MAC_energy', 'mem_energy', 'energy_breakdown', 'energy_breakdown_further', 'energy_total', 'memory_word_access',
-                    'data_loading_cycle', 'data_offloading_cycle', 'ideal_cycle', 'ideal_temporal_cycle', 'latency_total0', 'latency_total1',
-                    'latency_total2', 'MAC_spatial_utilization', 'MAC_utilization0', 'MAC_utilization1', 'MAC_utilization2', 'layer',
-                    'accelerator']
+        func = [
+            "calc_allowed_and_real_data_transfer_cycle_per_DTL",
+            "calc_data_loading_offloading_latency",
+            "calc_double_buffer_flag",
+            "calc_overall_latency",
+            "calc_MAC_energy_cost",
+            "calc_energy",
+            "calc_latency",
+            "calc_memory_energy_cost",
+            "calc_memory_utilization",
+            "calc_memory_word_access",
+            "combine_data_transfer_rate_per_physical_port",
+            "run",
+        ]
+        mul_attr = [
+            "MAC_energy",
+            "mem_energy",
+            "energy_breakdown",
+            "energy_breakdown_further",
+            "energy_total",
+            "memory_word_access",
+            "data_loading_cycle",
+            "data_offloading_cycle",
+            "ideal_cycle",
+            "ideal_temporal_cycle",
+            "latency_total0",
+            "latency_total1",
+            "latency_total2",
+            "MAC_spatial_utilization",
+            "MAC_utilization0",
+            "MAC_utilization1",
+            "MAC_utilization2",
+            "layer",
+            "accelerator",
+        ]
 
         for attr in dir(mul):
-            if attr not in (func + mul_attr) and attr[0] != '_':
+            if attr not in (func + mul_attr) and attr[0] != "_":
                 delattr(mul, attr)
 
         return mul
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/adder_hierarchy.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/adder_hierarchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-from typing import Dict, List, Tuple
+from typing import Dict, List
 from math import log2, ceil, prod
-from zigzag.classes.hardware.architecture.operational_array import Multiplier, MultiplierArray
+from zigzag.classes.hardware.architecture.operational_array import (
+    Multiplier,
+    MultiplierArray,
+)
 
 
 class Adder:
-    def __init__(self, fan_in: int, unit_cost: float, unit_area: float, input_precision: List[int] or int, output_precision: int):
+    def __init__(
+        self,
+        fan_in: int,
+        unit_cost: float,
+        unit_area: float,
+        input_precision: List[int] or int,
+        output_precision: int,
+    ):
         """
         Initiate Adder class. The adder can be used in aggregation (AG) adder level or accumulation (AC) adder level.
         :param fan_in: the number of input data to be added together.
         :param unit_cost: one addition energy.
         :param unit_area: one adder area.
         :param input_precision: input data precision. If it is 'int' format, it means the same precision is applied to all input data;
         if it is 'list' format, it allows to define for different input data the different precision.
@@ -20,145 +30,197 @@
         self.input_precision = input_precision
         self.output_precision = output_precision
 
 
 class AdderLevel:
     def __init__(self, index: int, name: str, details: Dict[str, str or int]):
         """
-        Adder Level is the basic building block for Adder Hierarchy. 
+        Adder Level is the basic building block for Adder Hierarchy.
         It can be an array of aggregators (AG, addition over space) or accumulators (AC, addition over time).
         :param index: Adder Level index.
         :param name: Adder Level name's default format: 'ALi' (i = 1,2,3,...).
         :param details: Adder Level's type, fan-in, and so on.
         """
         self.id = index
         self.name = name
-        self.type = details['type']
-        self.unit = Adder(details['fan_in'], details['unit_cost'], details['unit_area'], details['input_precision'], details['output_precision'])
-        self.one_instance_unit_count = details['one_instance_unit_count']
-        self.total_unit_count = details['total_unit_count']
+        self.type = details["type"]
+        self.unit = Adder(
+            details["fan_in"],
+            details["unit_cost"],
+            details["unit_area"],
+            details["input_precision"],
+            details["output_precision"],
+        )
+        self.one_instance_unit_count = details["one_instance_unit_count"]
+        self.total_unit_count = details["total_unit_count"]
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return str(self)
 
 
 class AdderHierarchy:
-    def __init__(self, adder_hierarchy: Dict[str, Dict[str, str or int]], multiplier_array: MultiplierArray):
+    def __init__(
+        self,
+        adder_hierarchy: Dict[str, Dict[str, str or int]],
+        multiplier_array: MultiplierArray,
+    ):
         """
         Construct AdderHierarchy class based on user-defined adder hierarchy. It will check if users' definition is valid,
         and extract all the related info, e.g. unit count for each adder level and total area.
         :param adder_hierarchy: user-defined adder hierarchy.
         For aggregation level (AG), it should contain 'type', 'fan_in', 'unit_cost', 'unit_area';
         for accumulation level (AC), it should contain 'type', output_precision', 'unit_cost', 'unit_area'.
         :param multiplier_array: MultiplierArray object, check in "architecture/operational_array.py" for more info.
         """
         self.calc_output_reduction_size(multiplier_array)
         self.assert_valid(adder_hierarchy)
         multiplier_output_precision = multiplier_array.unit.output_precision
         self.construct_adder_levels(multiplier_output_precision, adder_hierarchy)
-        self.total_area = prod([adder_level.unit.area * adder_level.total_unit_count for adder_level in self.adder_levels])
+        self.total_area = prod(
+            [
+                adder_level.unit.area * adder_level.total_unit_count
+                for adder_level in self.adder_levels
+            ]
+        )
 
     def calc_output_reduction_size(self, multiplier_array: MultiplierArray):
         """
         From dimensions and operand_spatial_sharing defined by user, calculate total output-sharing dimension size.
         :param multiplier_array: MultiplierArray object, check in "architecture/operational_array.py" for more info.
         :return: update self.output_reduction_size and self.output_non_reduction_size
         """
         total_dimension_size = multiplier_array.total_unit_count
         output_reduction_size = 1
         for os in multiplier_array.operand_spatial_sharing:
-            if os.operand == 'O':
+            if os.operand == "O":
                 output_reduction_size *= int(os.size)
         self.output_reduction_size = output_reduction_size
         self.output_non_reduction_size = total_dimension_size // output_reduction_size
 
     def assert_valid(self, adder_hierarchy: Dict[str, Dict[str, str or int]]):
         """
         A valid adder hierarchy need to match operand_spatial_sharing (especially the output reduction dimension).
         :param adder_hierarchy: user-defined adder hierarchy.
         :return: none
         """
-        assert all([adder_level['type'] in ['AG', 'AC'] for adder_level in adder_hierarchy.values()]), \
-            "Some adder type not recognized. Adder type can only be 'AG' or 'AC'."
+        assert all(
+            [
+                adder_level["type"] in ["AG", "AC"]
+                for adder_level in adder_hierarchy.values()
+            ]
+        ), "Some adder type not recognized. Adder type can only be 'AG' or 'AC'."
 
         total_fan_in = 1
         fan_in_list = []
         acc_flag = False
 
         for adder_level in adder_hierarchy.values():
-            if adder_level['type'] == 'AG':
-                total_fan_in *= adder_level['fan_in']
-                fan_in_list.append(adder_level['fan_in'])
+            if adder_level["type"] == "AG":
+                total_fan_in *= adder_level["fan_in"]
+                fan_in_list.append(adder_level["fan_in"])
             else:
                 acc_flag = True
 
         num = self.output_reduction_size
         output_reduction_size_factors = [n for n in range(1, num + 1) if num % n == 0]
 
-        assert set(fan_in_list).issubset(set(output_reduction_size_factors)), \
-            f"Invalid adder hierarchy due to at least 1 element in adder tree's fan-in ({fan_in_list}) " \
+        assert set(fan_in_list).issubset(set(output_reduction_size_factors)), (
+            f"Invalid adder hierarchy due to at least 1 element in adder tree's fan-in ({fan_in_list}) "
             f"is not in the factor list of total output-reduction size ({output_reduction_size_factors})."
-        assert (total_fan_in in output_reduction_size_factors), \
-            f"Invalid adder hierarchy due to adder tree's total fan-in ({total_fan_in}) is not a factor " \
+        )
+        assert total_fan_in in output_reduction_size_factors, (
+            f"Invalid adder hierarchy due to adder tree's total fan-in ({total_fan_in}) is not a factor "
             f"of output reduction size ({output_reduction_size_factors})."
-        assert (self.output_reduction_size == total_fan_in or acc_flag), \
-            f"Invalid adder hierarchy due to adder tree's total fan-in ({total_fan_in}) < total output " \
+        )
+        assert self.output_reduction_size == total_fan_in or acc_flag, (
+            f"Invalid adder hierarchy due to adder tree's total fan-in ({total_fan_in}) < total output "
             f"reduction size ({self.output_reduction_size}) and no accumulator found."
+        )
 
-    def construct_adder_levels(self, multiplier_output_precision: int, adder_hierarchy: Dict[str, Dict[str, str or int]]):
+    def construct_adder_levels(
+        self,
+        multiplier_output_precision: int,
+        adder_hierarchy: Dict[str, Dict[str, str or int]],
+    ):
         """
         Construct adder level from the innermost level (close to multiplier) to the outermost.
         Calculate adder count and precision at each adder level.
         :param multiplier_output_precision: treated as the innermost-level adder's input precision.
         :param adder_hierarchy: user-defined adder hierarchy.
         :return: update self.adder_levels
         """
         precision_counter = multiplier_output_precision
         unit_counter = self.output_reduction_size
 
         for name, adder_details in adder_hierarchy.items():
-            if adder_details['type'] == 'AG':
-                adder_details['input_precision'] = precision_counter
-                adder_details['output_precision'] = precision_counter + ceil(log2(adder_details['fan_in']))
-                adder_details['one_instance_unit_count'] = unit_counter//adder_details['fan_in']
-                adder_details['total_unit_count'] = adder_details['one_instance_unit_count'] * self.output_non_reduction_size
-
-                ''' update precision and unit count when encounter aggregation (AG) adder level '''
-                precision_counter = adder_details['output_precision']
-                unit_counter = adder_details['one_instance_unit_count']
+            if adder_details["type"] == "AG":
+                adder_details["input_precision"] = precision_counter
+                adder_details["output_precision"] = precision_counter + ceil(
+                    log2(adder_details["fan_in"])
+                )
+                adder_details["one_instance_unit_count"] = (
+                    unit_counter // adder_details["fan_in"]
+                )
+                adder_details["total_unit_count"] = (
+                    adder_details["one_instance_unit_count"]
+                    * self.output_non_reduction_size
+                )
+
+                """ update precision and unit count when encounter aggregation (AG) adder level """
+                precision_counter = adder_details["output_precision"]
+                unit_counter = adder_details["one_instance_unit_count"]
             else:
-                adder_details['fan_in'] = 2
-                adder_details['input_precision'] = [precision_counter, adder_details['output_precision']]
-                adder_details['one_instance_unit_count'] = unit_counter
-                adder_details['total_unit_count'] = adder_details['one_instance_unit_count'] * self.output_non_reduction_size
-
-                ''' only update precision when encounter accumulation (AC) adder level '''
-                precision_counter = adder_details['output_precision']
-
-        adder_levels_obj = [AdderLevel(idx, name, details) for idx, (name, details) in enumerate(adder_hierarchy.items())]
+                adder_details["fan_in"] = 2
+                adder_details["input_precision"] = [
+                    precision_counter,
+                    adder_details["output_precision"],
+                ]
+                adder_details["one_instance_unit_count"] = unit_counter
+                adder_details["total_unit_count"] = (
+                    adder_details["one_instance_unit_count"]
+                    * self.output_non_reduction_size
+                )
+
+                """ only update precision when encounter accumulation (AC) adder level """
+                precision_counter = adder_details["output_precision"]
+
+        adder_levels_obj = [
+            AdderLevel(idx, name, details)
+            for idx, (name, details) in enumerate(adder_hierarchy.items())
+        ]
         self.adder_levels = adder_levels_obj
 
 
 if __name__ == "__main__":
 
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.5
     multiplier_area = 0.1
-    dimensions = {'D1': 8, 'D2': 3, 'D3': 2}
-    operand_spatial_sharing = {'OS1': ((1, 0, 0), 'O'),
-                       'OS2': ((0, 1, 0), 'I1'),
-                       'OS3': ((0, 0, 1), 'I1'),
-                       'OS4': ((1, 1, 0), 'I2')}
-
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {"D1": 8, "D2": 3, "D3": 2}
+    operand_spatial_sharing = {
+        "OS1": ((1, 0, 0), "O"),
+        "OS2": ((0, 1, 0), "I1"),
+        "OS3": ((0, 0, 1), "I1"),
+        "OS4": ((1, 1, 0), "I2"),
+    }
+
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
 
-    user_defined_adder_hierarchy = {'AL1': {'type': 'AG', 'fan_in': 4, 'unit_cost': 0.08, 'unit_area': 0.03},
-                                    'AL2': {'type': 'AC', 'output_precision': 24, 'unit_cost': 0.1, 'unit_area': 0.05},
-                                    'AL3': {'type': 'AG', 'fan_in': 2, 'unit_cost': 0.13, 'unit_area': 0.07}}
+    user_defined_adder_hierarchy = {
+        "AL1": {"type": "AG", "fan_in": 4, "unit_cost": 0.08, "unit_area": 0.03},
+        "AL2": {
+            "type": "AC",
+            "output_precision": 24,
+            "unit_cost": 0.1,
+            "unit_area": 0.05,
+        },
+        "AL3": {"type": "AG", "fan_in": 2, "unit_cost": 0.13, "unit_area": 0.07},
+    }
 
     ah = AdderHierarchy(user_defined_adder_hierarchy, multiplier_array)
-    a=1
-
+    a = 1
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/core.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 from zigzag.classes.hardware.architecture.operational_array import OperationalArray
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 import networkx as nx
 
+
 class Core:
     """
     The Core class houses the array of multipliers and the attached memory hierarchy.
     This class supports a singular multiplier array and memory hierarchy, runtime flexibility should be implemented on top.
     """
-    def __init__(self, id: int, operational_array: OperationalArray, memory_hierarchy: MemoryHierarchy, dataflows: list=None):
+
+    def __init__(
+        self,
+        id: int,
+        operational_array: OperationalArray,
+        memory_hierarchy: MemoryHierarchy,
+        dataflows: list = None,
+    ):
         self.id = id
         self.operational_array = operational_array
         self.memory_hierarchy = memory_hierarchy
-        self.dataflows = dataflows  # save the possible spatial dataflows inside the Core
+        self.dataflows = (
+            dataflows  # save the possible spatial dataflows inside the Core
+        )
         self.check_valid()
-        
+
         self.recalculate_memory_hierarchy_information()
 
     def __str__(self) -> str:
         return f"Core({self.id})"
 
     def __repr__(self) -> str:
         return str(self)
@@ -30,18 +40,26 @@
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, Core):
             return False
-        return self.id == __o.id and self.operational_array == __o.operational_array and self.memory_hierarchy == __o.memory_hierarchy
+        return (
+            self.id == __o.id
+            and self.operational_array == __o.operational_array
+            and self.memory_hierarchy == __o.memory_hierarchy
+        )
 
     def equals(self, other: object) -> bool:
-        return isinstance(other, Core) and self.operational_array == other.operational_array and self.memory_hierarchy == other.memory_hierarchy
+        return (
+            isinstance(other, Core)
+            and self.operational_array == other.operational_array
+            and self.memory_hierarchy == other.memory_hierarchy
+        )
 
     def check_valid(self):
         # TODO
         pass
 
     def recalculate_memory_hierarchy_information(self):
         self.generate_memory_hierarchy_dict()
@@ -52,26 +70,44 @@
         mem_hierarchy_dict = {}
         mem_size_dict = {}
         mem_r_bw_dict = {}
         mem_w_bw_dict = {}
         mem_r_bw_min_dict = {}
         mem_w_bw_min_dict = {}
         for mem_op in mem_operands:
-            mem_hierarchy_dict[mem_op] = [node for node in nx.topological_sort(self.memory_hierarchy)
-                                          if mem_op in node.operands]
-            mem_size_dict[mem_op] = [node.memory_instance.size for node in nx.topological_sort(self.memory_hierarchy)
-                                     if mem_op in node.operands]
-            mem_r_bw_dict[mem_op] = [node.memory_instance.r_bw for node in nx.topological_sort(self.memory_hierarchy)
-                                     if mem_op in node.operands]
-            mem_w_bw_dict[mem_op] = [node.memory_instance.w_bw for node in nx.topological_sort(self.memory_hierarchy)
-                                     if mem_op in node.operands]
-            mem_r_bw_min_dict[mem_op] = [node.memory_instance.r_bw_min for node in nx.topological_sort(self.memory_hierarchy)
-                                         if mem_op in node.operands]
-            mem_w_bw_min_dict[mem_op] = [node.memory_instance.w_bw_min for node in nx.topological_sort(self.memory_hierarchy)
-                                         if mem_op in node.operands]
+            mem_hierarchy_dict[mem_op] = [
+                node
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
+            mem_size_dict[mem_op] = [
+                node.memory_instance.size
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
+            mem_r_bw_dict[mem_op] = [
+                node.memory_instance.r_bw
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
+            mem_w_bw_dict[mem_op] = [
+                node.memory_instance.w_bw
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
+            mem_r_bw_min_dict[mem_op] = [
+                node.memory_instance.r_bw_min
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
+            mem_w_bw_min_dict[mem_op] = [
+                node.memory_instance.w_bw_min
+                for node in nx.topological_sort(self.memory_hierarchy)
+                if mem_op in node.operands
+            ]
         self.mem_hierarchy_dict = mem_hierarchy_dict
         self.mem_size_dict = mem_size_dict
         self.mem_r_bw_dict = mem_r_bw_dict
         self.mem_w_bw_dict = mem_w_bw_dict
         self.mem_r_bw_min_dict = mem_r_bw_min_dict
         self.mem_w_bw_min_dict = mem_w_bw_min_dict
 
@@ -79,15 +115,18 @@
         """
         Generates a list of dictionary that indicates which operand's which memory levels are sharing the same physical memory
         """
         memory_sharing_list = []
         for mem_lv in self.mem_hierarchy_dict.values():
             for mem in mem_lv:
                 operand_mem_share = mem.mem_level_of_operands
-                if len(operand_mem_share) > 1 and operand_mem_share not in memory_sharing_list:
+                if (
+                    len(operand_mem_share) > 1
+                    and operand_mem_share not in memory_sharing_list
+                ):
                     memory_sharing_list.append(operand_mem_share)
 
         self.mem_sharing_list = memory_sharing_list
 
     def get_memory_hierarchy(self):
         return self.memory_hierarchy
 
@@ -107,19 +146,28 @@
         return self.mem_sharing_list
 
     def get_memory_level(self, mem_op: str, mem_lv: int):
         """
         Returns a specific memory level in the memory hierarchy for the memory operand.
         """
         # Sort the nodes topologically and filter out all memories that don't store mem_op
-        memory = [node for node in nx.topological_sort(self.memory_hierarchy) if mem_op in node.operands]
+        memory = [
+            node
+            for node in nx.topological_sort(self.memory_hierarchy)
+            if mem_op in node.operands
+        ]
         return memory[mem_lv]
 
     def get_lowest_shared_mem_level_above(self, mem_op1, mem_lv1, mem_op2, mem_lv2):
         """
         Get the lowest shared memory level between mem_op1 (>= mem_lv1) and mem_op2 (>= mem_lv2).
         """
         for lv, mem in enumerate(self.mem_hierarchy_dict[mem_op1][mem_lv1:]):
-            if mem_op2 in mem.operands and mem_lv2 <= mem.mem_level_of_operands[mem_op2]:
+            if (
+                mem_op2 in mem.operands
+                and mem_lv2 <= mem.mem_level_of_operands[mem_op2]
+            ):
                 return mem
 
-        raise Exception(f"{mem_op1}'s level {mem_lv1} and {mem_op2}'s level {mem_lv2} don't have a shared memory above!")
+        raise Exception(
+            f"{mem_op1}'s level {mem_lv1} and {mem_op2}'s level {mem_lv2} don't have a shared memory above!"
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/dimension.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/dimension.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,11 +20,13 @@
     def __jsonrepr__(self):
         """
         JSON representation of this class to save it to a json file.
         """
         return self.__dict__
 
     def __eq__(self, other):
-        return other.id == self.id and self.name == other.name and self.size == other.size
+        return (
+            other.id == self.id and self.name == other.name and self.size == other.size
+        )
 
     def __hash__(self):
-        return hash(self.id) ^ hash(self.name)
+        return hash(self.id) ^ hash(self.name)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_hierarchy.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,101 +10,136 @@
 
 class MemoryHierarchy(DiGraph):
     """
     Class that represents a memory hierarchy as a directed networkx graph.
     The memory hierarchy graph is directed, with the root nodes representing the lowest level
     in the memory hierarchy.
     """
-    def __init__(self, operational_array: OperationalArray, name: str = "Memory Hierarchy", **attr):
+
+    def __init__(
+        self,
+        operational_array: OperationalArray,
+        name: str = "Memory Hierarchy",
+        **attr,
+    ):
         """
         Initialize the memory hierarchy graph.
         The initialization sets the operational array this memory hierarchy will connect to.
         The graph nodes are the given nodes. The edges are extracted from the operands the memory levels store.
         :param nodes: a list of MemoryLevels. Entries need to be provided from lowest to highest memory level.
         """
         super().__init__(**attr)
         self.name = name
         self.operational_array = operational_array
         self.operands = set()  # Initialize the set that will store all memory operands
-        self.nb_levels = {}  # Initialize the dict that will store how many memory levels an operand has
+        self.nb_levels = (
+            {}
+        )  # Initialize the dict that will store how many memory levels an operand has
         self.mem_instance_list = []
         self.memory_level_id = 0
 
     def __jsonrepr__(self):
         """
         JSON Representation of this object to save it to a json file.
         """
         return {"memory_levels": [node for node in nx.topological_sort(self)]}
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, MemoryHierarchy):
             return False
-        return all([self_ml == __o_ml for (self_ml, __o_ml) in zip(self.nodes(), __o.nodes())])
-
-    def add_memory(self, 
-                memory_instance: MemoryInstance, 
-                operands: Tuple[str, ...], 
-                port_alloc: Tuple[dict, ...] = None,
-                served_dimensions: Set or str = "all"):
+        return all(
+            [self_ml == __o_ml for (self_ml, __o_ml) in zip(self.nodes(), __o.nodes())]
+        )
+
+    def add_memory(
+        self,
+        memory_instance: MemoryInstance,
+        operands: Tuple[str, ...],
+        port_alloc: Tuple[dict, ...] = None,
+        served_dimensions: Set or str = "all",
+    ):
         """
         Adds a memory to the memory hierarchy graph.
 
         !!! NOTE: memory level need to be added from bottom level (e.g., Reg) to top level (e.g., DRAM) for each operand !!!
 
         Internally a MemoryLevel object is built, which represents the memory node.
         Edges are added from all sink nodes in the graph to this node if the memory operands match
         :param memory_instance: The MemoryInstance containing the different memory characteristics.
         :param operands: The memory operands the memory level stores.
-        :param served_dimensions: The operational array dimensions this memory level serves. 
+        :param served_dimensions: The operational array dimensions this memory level serves.
         Each vector in the set is a direction that is served.
         Use 'all' to represent all dimensions (i.e. the memory level is not unrolled).
         """
 
         if port_alloc is None:
             # Define the standard port allocation scheme (this assumes one read port and one write port)
-            if not (memory_instance.r_port == 1 and memory_instance.w_port == 1 and memory_instance.rw_port == 0):
-                raise ValueError(f"No port allocation was provided for memory level of instance {memory_instance} and doesn't match with standard port allocation generation of 1 read and 1 write port.")
+            if not (
+                memory_instance.r_port == 1
+                and memory_instance.w_port == 1
+                and memory_instance.rw_port == 0
+            ):
+                raise ValueError(
+                    f"No port allocation was provided for memory level of instance {memory_instance} and doesn't match with standard port allocation generation of 1 read and 1 write port."
+                )
             port_alloc = []
             for operand in operands:
-                if operand == 'O':
-                    port_alloc.append({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'})
+                if operand == "O":
+                    port_alloc.append(
+                        {
+                            "fh": "w_port_1",
+                            "tl": "r_port_1",
+                            "fl": "w_port_1",
+                            "th": "r_port_1",
+                        }
+                    )
                 else:
-                    port_alloc.append({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None})
+                    port_alloc.append(
+                        {"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None}
+                    )
             port_alloc = tuple(port_alloc)
-        
+
         # Assert that if served_dimensions is a string, it is "all"
         if type(served_dimensions) == str:
-            assert served_dimensions == "all", "Served dimensions is a string, but is not all."
+            assert (
+                served_dimensions == "all"
+            ), "Served dimensions is a string, but is not all."
 
         # Add the memory operands to the self.operands set attribute that stores all memory operands.
         for mem_op in operands:
             if mem_op not in self.operands:
                 self.nb_levels[mem_op] = 1
                 self.operands.add(mem_op)
             else:
                 self.nb_levels[mem_op] += 1
             self.operands.add(mem_op)
 
         # Parse the served_dimensions by replicating it into a tuple for each memory operand
         # as the MemoryLevel constructor expects this.
-        served_dimensions_repl = tuple([served_dimensions for _ in range(len(operands))])
+        served_dimensions_repl = tuple(
+            [served_dimensions for _ in range(len(operands))]
+        )
 
         # Compute which memory level this is for all the operands
         mem_level_of_operands = {}
         for operand in operands:
-            nb_levels_so_far = len([node for node in self.nodes() if operand in node.operands])
+            nb_levels_so_far = len(
+                [node for node in self.nodes() if operand in node.operands]
+            )
             mem_level_of_operands[operand] = nb_levels_so_far
 
-        memory_level = MemoryLevel(memory_instance=memory_instance, 
-                                   operands=operands,
-                                   mem_level_of_operands=mem_level_of_operands,
-                                   port_alloc=port_alloc,
-                                   served_dimensions=served_dimensions_repl,
-                                   operational_array=self.operational_array,
-                                   id=self.memory_level_id)
+        memory_level = MemoryLevel(
+            memory_instance=memory_instance,
+            operands=operands,
+            mem_level_of_operands=mem_level_of_operands,
+            port_alloc=port_alloc,
+            served_dimensions=served_dimensions_repl,
+            operational_array=self.operational_array,
+            id=self.memory_level_id,
+        )
         self.mem_instance_list.append(memory_level)
         self.memory_level_id += 1
 
         # Precompute appropriate edges
         to_edge_from = set()
         for mem_op in operands:
             # Find top level memories of the operands
@@ -120,15 +155,17 @@
 
     def get_memory_levels(self, mem_op: str):
         """
         Returns a list of memories in the memory hierarchy for the memory operand.
         The first entry in the returned list is the innermost memory level.
         """
         # Sort the nodes topologically and filter out all memories that don't store mem_op
-        memories = [node for node in nx.topological_sort(self) if mem_op in node.operands]
+        memories = [
+            node for node in nx.topological_sort(self) if mem_op in node.operands
+        ]
         return memories
 
     def get_operands(self):
         """
         Returns all the memory operands this memory hierarchy graph contains as a set.
         """
         return self.operands
@@ -151,15 +188,15 @@
 
     def get_top_memories(self) -> Tuple[List[MemoryLevel], int]:
         """
         Returns the 'top'-most MemoryLevels, where 'the' level of MemoryLevel is considered to be the largest
         level it has across its assigned operands
         :return: (list_of_memories_on_top_level, top_level)
         """
-        level_to_mems = defaultdict(lambda: [] )
+        level_to_mems = defaultdict(lambda: [])
         for node in self.nodes():
             level_to_mems[max(node.mem_level_of_operands.values())].append(node)
         top_level = max(level_to_mems.keys())
         return level_to_mems[top_level], top_level
 
     def remove_top_level(self) -> Tuple[List[MemoryLevel], int]:
         """
@@ -170,27 +207,32 @@
         """
         to_remove, top_level = self.get_top_memories()
         for tr in to_remove:
             self.mem_instance_list.remove(tr)
             self.remove_node(tr)
 
         for k in self.nb_levels:
-            self.nb_levels[k] = len(set(node.mem_level_of_operands.get(k)
-                                        for node in self.nodes() if k in node.mem_level_of_operands))
+            self.nb_levels[k] = len(
+                set(
+                    node.mem_level_of_operands.get(k)
+                    for node in self.nodes()
+                    if k in node.mem_level_of_operands
+                )
+            )
         return to_remove, max(self.nb_levels.keys())
 
     def get_operator_top_level(self, operand) -> Tuple[List[MemoryLevel], int]:
         """
         Finds the highest level of memories that have the given operand assigned to it, and returns the MemoryLevel
         instance on this level that have the operand assigned to it.
         'The' level of a MemoryLevel is considered to be the largest
         level it has across its assigned operands.
         :return: (list of MemoryLevel instances, top_level)
         """
-        level_to_mems = defaultdict(lambda: [] )
+        level_to_mems = defaultdict(lambda: [])
         for node in self.nodes():
             if operand in node.operands[:]:
                 level_to_mems[max(node.mem_level_of_operands.values())].append(node)
         top_level = max(level_to_mems.keys()) if level_to_mems else -1
         return level_to_mems[top_level], top_level
 
     def get_operand_top_level(self, operand) -> MemoryLevel:
@@ -223,14 +265,17 @@
                 for so in p.served_op_lv_dir[:]:
                     if so[0] == operand:
                         p.served_op_lv_dir.remove(so)
             if len(tr.mem_level_of_operands) == 0:
                 self.mem_instance_list.remove(tr)
                 self.remove_node(tr)
 
-
         for k in self.nb_levels:
-            self.nb_levels[k] = len(set(node.mem_level_of_operands.get(k)
-                                        for node in self.nodes() if k in node.mem_level_of_operands))
+            self.nb_levels[k] = len(
+                set(
+                    node.mem_level_of_operands.get(k)
+                    for node in self.nodes()
+                    if k in node.mem_level_of_operands
+                )
+            )
 
         return to_remove, self.nb_levels[operand]
-
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from zigzag.classes.cacti.cacti_parser import CactiParser
 
 
 class MemoryInstance:
     def __init__(
         self,
         name: str,
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/memory_level.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/memory_level.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from typing import Dict, Tuple, List
 from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
 from zigzag.classes.hardware.architecture.operational_array import OperationalArray
 from math import prod
 import numpy as np
 
+
 class MemoryPort:
     port_id_counter = 0
 
-    def __init__(self, port_name: str, port_bw: int, port_bw_min: int, port_attr: str, port_id=None):
+    def __init__(
+        self,
+        port_name: str,
+        port_bw: int,
+        port_bw_min: int,
+        port_attr: str,
+        port_id=None,
+    ):
         """
         Collect all the physical memory port related information here.
 
         :param port_id: port index per memory
         :param port_bw: bit/cc
         :param port_attr: read_only (r), write_only (w), read_write (rw)
         :param served_op_and_dir: [(I1, rd_out_to_low), (O, wr_in_by_low), (O, rd_out_to_low)]
         """
         self.name = port_name
         self.bw = port_bw
         self.bw_min = port_bw_min
         self.attr = port_attr
         self.served_op_lv_dir = []
 
-        ''' to give each port a unique id number '''
+        """ to give each port a unique id number """
         if port_id is None:
             self.port_id = MemoryPort.port_id_counter
             MemoryPort.port_id_counter += 1
         else:
             self.port_id = port_id
             MemoryPort.port_id_counter = port_id + 1
 
@@ -36,23 +44,36 @@
     def __str__(self):
         return str(self.name)
 
     def __repr__(self):
         return str(self.name)
 
     def __eq__(self, other) -> bool:
-        return isinstance(other, MemoryPort) and self.bw == other.bw and self.bw_min == other.bw_min and self.attr == other.attr
+        return (
+            isinstance(other, MemoryPort)
+            and self.bw == other.bw
+            and self.bw_min == other.bw_min
+            and self.attr == other.attr
+        )
 
     def __hash__(self):
         return self.port_id
 
-class MemoryLevel:
 
-    def __init__(self, memory_instance: MemoryInstance, operands: List[str], mem_level_of_operands: Dict,
-                 port_alloc: Tuple[dict, ...], served_dimensions: set or str, operational_array: OperationalArray, id):
+class MemoryLevel:
+    def __init__(
+        self,
+        memory_instance: MemoryInstance,
+        operands: List[str],
+        mem_level_of_operands: Dict,
+        port_alloc: Tuple[dict, ...],
+        served_dimensions: set or str,
+        operational_array: OperationalArray,
+        id,
+    ):
         """
         Initialize the memory level in the hierarchy with the physical memory instance.
 
         :param memory_instance:
         :param operands:
         :param port_alloc: memory port allocation (physical memory port -> functional memory port)
         :param served_dimensions:
@@ -66,90 +87,102 @@
         self.dimensions = operational_array.dimensions
         self.nb_dimensions = operational_array.nb_dimensions
         self.dimension_sizes = operational_array.dimension_sizes
         self.id = id
         self.check_served_dimensions()
         self.assert_valid()
 
-        ''' for each operand that current memory level holds, allocate 
-        physical memory ports to its 4 potential data movement '''
+        """ for each operand that current memory level holds, allocate 
+        physical memory ports to its 4 potential data movement """
         self.port_alloc_raw = port_alloc
         self.port_allocation()
 
-        ''' memory access bandwidth and energy extraction '''
+        """ memory access bandwidth and energy extraction """
 
         self.read_energy = memory_instance.r_cost
         self.write_energy = memory_instance.w_cost
         self.read_bw = memory_instance.r_bw
         self.write_bw = memory_instance.w_bw
 
-        ''' calculate memory unrolling count '''
+        """ calculate memory unrolling count """
         # Todo: for memory level using diagonal dimension, only allow it to have an unrolling count of '1'.
         self.calc_unroll_count()
 
-        ''' calculate in ideal case memory's total fanout and per-data fanout '''
+        """ calculate in ideal case memory's total fanout and per-data fanout """
         # Todo: not consider systolic array for now.
         self.calc_fanout()
 
     def __update_formatted_string(self):
         self.formatted_string = f"MemoryLevel(instance={self.memory_instance.name},operands={self.operands},served_dimensions={self.served_dimensions})"
 
     def __str__(self):
         self.__update_formatted_string()
         return self.formatted_string
 
     def __repr__(self):
         return str(self)
 
     def __eq__(self, other) -> bool:
-        return isinstance(other, MemoryLevel) and self.memory_instance == other.memory_instance and self.operands == other.operands and \
-            self.mem_level_of_operands == other.mem_level_of_operands and self.port_list == other.port_list and self.served_dimensions_vec == other.served_dimensions_vec
+        return (
+            isinstance(other, MemoryLevel)
+            and self.memory_instance == other.memory_instance
+            and self.operands == other.operands
+            and self.mem_level_of_operands == other.mem_level_of_operands
+            and self.port_list == other.port_list
+            and self.served_dimensions_vec == other.served_dimensions_vec
+        )
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def port_allocation(self):
-        """ Create port object """
+        """Create port object"""
 
-        ''' 
+        """ 
         Step 1: according to the port count of the memory instance, initialize the physical port object 
         (so far, we don't know what the port will be used for. But we do know the port's id/bw/attribute) 
-        '''
+        """
         port_list = []
         r_port = self.memory_instance.r_port
         w_port = self.memory_instance.w_port
         rw_port = self.memory_instance.rw_port
-        for i in range(1, r_port+1):
-            port_name = 'r_port_' + str(i)
+        for i in range(1, r_port + 1):
+            port_name = "r_port_" + str(i)
             port_bw = self.memory_instance.r_bw
             port_bw_min = self.memory_instance.r_bw_min
-            port_attr = 'r'
+            port_attr = "r"
             new_port = MemoryPort(port_name, port_bw, port_bw_min, port_attr)
             port_list.append(new_port)
-        for i in range(1, w_port+1):
-            port_name = 'w_port_' + str(i)
+        for i in range(1, w_port + 1):
+            port_name = "w_port_" + str(i)
             port_bw = self.memory_instance.w_bw
             port_bw_min = self.memory_instance.w_bw_min
-            port_attr = 'w'
+            port_attr = "w"
             new_port = MemoryPort(port_name, port_bw, port_bw_min, port_attr)
             port_list.append(new_port)
-        for i in range(1, rw_port+1):
-            port_name = 'rw_port_' + str(i)
-            port_bw = self.memory_instance.r_bw  # we assume the read-write port has the same bw for read and write
+        for i in range(1, rw_port + 1):
+            port_name = "rw_port_" + str(i)
+            port_bw = (
+                self.memory_instance.r_bw
+            )  # we assume the read-write port has the same bw for read and write
             port_bw_min = self.memory_instance.r_bw_min
-            port_attr = 'rw'
+            port_attr = "rw"
             new_port = MemoryPort(port_name, port_bw, port_bw_min, port_attr)
             port_list.append(new_port)
         port_names = [port.name for port in port_list]
 
-        ''' 
+        """ 
         Step 2: add operand, memory level, and served data movement direction for each port.
-        '''
-        mov_LUT = {'fh': 'wr_in_by_high', 'fl': 'wr_in_by_low',
-                   'th': 'rd_out_to_high', 'tl': 'rd_out_to_low'}
+        """
+        mov_LUT = {
+            "fh": "wr_in_by_high",
+            "fl": "wr_in_by_low",
+            "th": "rd_out_to_high",
+            "tl": "rd_out_to_low",
+        }
         for idx, (op, lv) in enumerate(list(self.mem_level_of_operands.items())):
             for mov, port in self.port_alloc_raw[idx].items():
                 if port is None:
                     continue
                 port_idx = port_names.index(port)
                 port_list[port_idx].add_port_function((op, lv, mov_LUT[mov]))
 
@@ -172,26 +205,37 @@
         Assert if the served_dimension of this MemoryLevel is valid.
         - in served_dimension tuple set, each dimension should only show up once, e.g. {(1,0), (1,1)} is not valid
         since the '1' in the first position showed up twice.
         """
         sum_served_dims = []
         for op_served_dimensions in self.served_dimensions_vec:
             sum_op_served_dimensions = [sum(x) for x in zip(*op_served_dimensions)]
-            assert not any(dim > 1 for dim in sum_op_served_dimensions), f"Invalid served dimensions for MemoryLevel of Memory {self}"
+            assert not any(
+                dim > 1 for dim in sum_op_served_dimensions
+            ), f"Invalid served dimensions for MemoryLevel of Memory {self}"
             sum_served_dims.append(sum_op_served_dimensions)
         self.sum_served_dims = sum_served_dims
 
     def calc_unroll_count(self):
         unroll_count = []
         for sum_op_served_dimensions in self.sum_served_dims:
-            sum_served_dims_invert = [not sum_dim for sum_dim in sum_op_served_dimensions]
-            op_unroll_count = prod([prod(x) for x in zip(self.dimension_sizes, sum_served_dims_invert) if prod(x) != 0])
+            sum_served_dims_invert = [
+                not sum_dim for sum_dim in sum_op_served_dimensions
+            ]
+            op_unroll_count = prod(
+                [
+                    prod(x)
+                    for x in zip(self.dimension_sizes, sum_served_dims_invert)
+                    if prod(x) != 0
+                ]
+            )
             unroll_count.append(op_unroll_count)
-        assert all(op_unroll_count == unroll_count[0] for op_unroll_count in
-                   unroll_count), f"Not all memory unrolling counts {unroll_count} are equal for MemoryLevel of Memory {str(self)}"
+        assert all(
+            op_unroll_count == unroll_count[0] for op_unroll_count in unroll_count
+        ), f"Not all memory unrolling counts {unroll_count} are equal for MemoryLevel of Memory {str(self)}"
         self.unroll_count = unroll_count[0]
 
     def calc_fanout(self):
         """
         Calculates the total fanout of this MemoryLevel.
         This equals the total amount of multipliers all instances in this level combined serve.
         To calculate the number of lower-level instances a single instance of this level serves,
@@ -209,44 +253,50 @@
         'all' signals that the MemoryLevel's served_dimensions are all dimensions, thus there is only one instance of the MemoryNode at this level.
 
         """
         served_dimensions = self.served_dimensions_vec
         operands = self.operands
         # Modify served_dimensions to list to be able to change it if empty set or None.
         served_dimensions = list(served_dimensions)
-        for op_idx, (op, op_served_dimensions) in enumerate(zip(operands, served_dimensions)):
+        for op_idx, (op, op_served_dimensions) in enumerate(
+            zip(operands, served_dimensions)
+        ):
             # If served_dimensions is an empty set, it means this memory level is fully unrolled wrt operational_array
             # We then convert it to be consistent with used notation
             if op_served_dimensions == set():
                 op_served_dimensions = {(0,) * self.nb_dimensions}
                 served_dimensions[op_idx] = tuple(op_served_dimensions)
             # If served_dimensions is 'all', it means this memory level is not unrolled
             # We then convert it to a set containing all base dimensions of the operational_array (corresponds to a flat identity matrix)
-            if op_served_dimensions == 'all':
+            if op_served_dimensions == "all":
                 identity_array = np.eye(self.nb_dimensions, dtype=int)
                 flat_identity_tuple = tuple([tuple(row) for row in identity_array])
                 op_served_dimensions = set(flat_identity_tuple)
                 served_dimensions[op_idx] = tuple(op_served_dimensions)
         served_dimensions = tuple(served_dimensions)
         self.served_dimensions_vec = served_dimensions
 
         # Based on the vector representation of the served dimensions,
         # we also save all the dimension objects this memory level serves.
         served_dimensions = []
         for op_served_dimensions_vec in self.served_dimensions_vec:
             for served_dimension_vec in op_served_dimensions_vec:
-                non_zero_idxs = [idx for idx, elem in enumerate(served_dimension_vec) if elem != 0]  # vector indices that are non-zero
-                served_dimensions += [self.find_dimension_with_idx(idx) for idx in non_zero_idxs]
+                non_zero_idxs = [
+                    idx for idx, elem in enumerate(served_dimension_vec) if elem != 0
+                ]  # vector indices that are non-zero
+                served_dimensions += [
+                    self.find_dimension_with_idx(idx) for idx in non_zero_idxs
+                ]
         self.served_dimensions = set(served_dimensions)
 
     def find_dimension_with_idx(self, idx: int):
         """
         Find the dimension object with idx 'idx'.
         """
         dimension = None
         for dim in self.dimensions:
             if dim.id == idx:
                 dimension = dim
                 break
         if dimension is None:
             raise ValueError("idx passed to function is not a valid dimension id.")
-        return dimension
+        return dimension
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/operational_array.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import Dict, Set
+from typing import Dict
 import numpy as np
 from zigzag.classes.hardware.architecture.dimension import Dimension
-from zigzag.classes.hardware.architecture.operand_spatial_sharing import OperandSpatialSharing
-from zigzag.classes.hardware.architecture.operational_unit import OperationalUnit, Multiplier
+from zigzag.classes.hardware.architecture.operational_unit import (
+    OperationalUnit,
+    Multiplier,
+)
+
 
 class OperationalArray:
     def __init__(self, operational_unit: OperationalUnit, dimensions: Dict[str, int]):
         """
         This class captures multi-dimensional operational array size.
 
         :param operational_unit: an OperationalUnit object including precision and single operation energy, later we
@@ -14,15 +17,18 @@
 
         :param dimensions: define the name and size of each multiplier array dimensions, e.g. {'D1': 3, 'D2': 5}.
         """
         self.unit = operational_unit
         self.total_unit_count = int(np.prod(list(dimensions.values())))
         self.total_area = operational_unit.area * self.total_unit_count
 
-        base_dims = [Dimension(idx, name, size) for idx, (name, size) in enumerate(dimensions.items())]
+        base_dims = [
+            Dimension(idx, name, size)
+            for idx, (name, size) in enumerate(dimensions.items())
+        ]
         self.dimensions = base_dims
         self.dimension_sizes = [dim.size for dim in base_dims]
         self.nb_dimensions = len(base_dims)
 
     def __jsonrepr__(self):
         """
         JSON Representation of this class to save it to a json file.
@@ -36,40 +42,46 @@
 
 
 class MultiplierArray(OperationalArray):
     pass
 
 
 def multiplier_array_example1():
-    '''Multiplier array variables'''
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.5
     multiplier_area = 0.1
-    dimensions = {'D1': 14, 'D2': 3, 'D3': 4}
-    operand_spatial_sharing = {'I1': {(1, 0, 0)},
-                       'O': {(0, 1, 0)},
-                       'I2': {(0, 0, 1), (1, 1, 0)}}
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {"D1": 14, "D2": 3, "D3": 4}
+    operand_spatial_sharing = {
+        "I1": {(1, 0, 0)},
+        "O": {(0, 1, 0)},
+        "I2": {(0, 0, 1), (1, 1, 0)},
+    }
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
 
     return multiplier_array
 
 
 def multiplier_array_example2():
-    '''Multiplier array variables'''
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.5
     multiplier_area = 0.1
-    dimensions = {'D1': 14, 'D2': 12}
-    operand_spatial_sharing = {'I1': {(1, 0)},
-                             'O': {(0, 1)},
-                             'I2': {(1, 1)}}
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {"D1": 14, "D2": 12}
+    operand_spatial_sharing = {"I1": {(1, 0)}, "O": {(0, 1)}, "I2": {(1, 1)}}
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
 
     return multiplier_array
 
 
 if __name__ == "__main__":
     multiplier_array = multiplier_array_example1()
     for os in multiplier_array.operand_spatial_sharing:
-        print(f'{os}\tdirection: {os.direction} operand: {os.operand} instances: {os.instances}')
+        print(
+            f"{os}\tdirection: {os.direction} operand: {os.operand} instances: {os.instances}"
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag-dse-2.3.2/zigzag/classes/hardware/architecture/operational_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from typing import List
 
 
 class OperationalUnit:
-    def __init__(self, input_precision: List[int], output_precision: int, unit_cost: float, unit_area: float):
+    def __init__(
+        self,
+        input_precision: List[int],
+        output_precision: int,
+        unit_cost: float,
+        unit_area: float,
+    ):
         """
         General class for a unit that performs a certain operation. For example: a multiplier unit.
 
         :param input_precision: The bit precision of the operation inputs.
         :param output_precision: The bit precision of the operation outputs.
         :param unit_cost: The energy cost of performing a single operation.
         :param unit_area: The area of a single operational unit.
@@ -22,22 +28,26 @@
         JSON Representation of this class to save it to a json file.
         """
         return self.__dict__
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, OperationalUnit):
             return False
-        return self.precision == __o.precision and self.cost == __o.cost and self.area == __o.area
+        return (
+            self.precision == __o.precision
+            and self.cost == __o.cost
+            and self.area == __o.area
+        )
 
 
 class Multiplier(OperationalUnit):
     def __init__(self, input_precision: List[int], energy_cost: float, area: float):
         """
         Initialize the Multiplier object.
 
         :param input_precision: The bit precision of the multiplication inputs.
         :param output_precision: The bit precision of the multiplication outputs.
         :param energy_cost: The energy cost of performing a single multiplication.
         :param area: The area of a single multiplier.
         """
         output_precision = sum(input_precision)
-        super().__init__(input_precision, output_precision, energy_cost, area)
+        super().__init__(input_precision, output_precision, energy_cost, area)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/accelerator/parser.py` & `zigzag-dse-2.3.2/zigzag/classes/io/accelerator/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/conv.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/conv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 from math import ceil
 
 from zigzag.classes.io.onnx.parser import Parser
-from zigzag.classes.io.onnx.utils import get_attribute_ints_with_name, get_node_input_output_dimension_shapes
+from zigzag.classes.io.onnx.utils import (
+    get_attribute_ints_with_name,
+    get_node_input_output_dimension_shapes,
+)
 from zigzag.classes.workload.layer_node import LayerNode
 from zigzag.utils import pickle_deepcopy
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class ConvParser(Parser):
-    """Parser for ONNX Conv and QLinearConv nodes into LayerNode.
-    """
+    """Parser for ONNX Conv and QLinearConv nodes into LayerNode."""
+
     def __init__(self, node_id, node, nodes_outputs, mapping, onnx_model) -> None:
         super().__init__(node_id, node, nodes_outputs, mapping, onnx_model)
-    
+
     def run(self):
-        """Run the parser and return the created LayerNode object.
-        """
+        """Run the parser and return the created LayerNode object."""
         layer_node = self.generate_layer_node_for_conv()
         return layer_node
 
     def generate_layer_node_for_conv(self):
-
         def get_weight_name(node):
             """Return the name of the weight input of this node depending on its operator type.
             Args:
                 node (NodeProto): The node
             """
             op_type = node.op_type  # 'Conv', 'QLinearConv', ...
             if op_type == "Conv":
                 return node.input[1]
             elif op_type == "QLinearConv":
                 return node.input[3]
             else:
-                raise NotImplementedError(f"Retrieving weight name for onnx node of type {op_type} is not supported.")
-
+                raise NotImplementedError(
+                    f"Retrieving weight name for onnx node of type {op_type} is not supported."
+                )
 
         def get_input_output_weight_data_type(node, model):
             """
             Return the data type of the input, output and weight tensors of this node.
             """
             value_info = model.graph.value_info
             if not value_info:
-                raise ValueError("value_info of model is empty. Make sure you are loading in an inferred model." \
-                "See https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#running-shape-inference-on-an-onnx-model")
+                raise ValueError(
+                    "value_info of model is empty. Make sure you are loading in an inferred model."
+                    "See https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#running-shape-inference-on-an-onnx-model"
+                )
             # get tensor names of the inputs and outputs of the model
             model_input_names = [input.name for input in model.graph.input]
             model_output_names = [output.name for output in model.graph.output]
             # get tensor names of the tensors in shapes
             shapes_names = [shape.name for shape in value_info]
             # get input and output activation dimension sizes
             # get input activation name
-            ia_name = node.input[0]  # assumed it is the first input, don't see a way to otherwise know
+            ia_name = node.input[
+                0
+            ]  # assumed it is the first input, don't see a way to otherwise know
             # check if this is a global input of the model, if so, retrieve dimension shape from model inputs
             if ia_name in model_input_names:
                 # Find index of this input in list of input names
                 ia_index = model_input_names.index(ia_name)
                 ia_elem_type = model.graph.input[ia_index].type.tensor_type.elem_type
             else:  # it should be present in the shapes variable as it's not an input or output of the model
                 ia_index = shapes_names.index(ia_name)
@@ -72,107 +79,149 @@
                 oa_elem_type = value_info[oa_index].type.tensor_type.elem_type
 
             # Get the weight name for this node (for QLinearConv this is the fourth input)
             w_name = get_weight_name(node)
             # w_name = node.input[3]
             # Get the weight data type through the graph initializers
             initializer_names = [i.name for i in model.graph.initializer]
-            w_data_type = model.graph.initializer[initializer_names.index(w_name)].data_type
+            w_data_type = model.graph.initializer[
+                initializer_names.index(w_name)
+            ].data_type
 
             return ia_elem_type, oa_elem_type, w_data_type
 
-
-        def get_layer_node_input_format(kernel_shape, strides, dilations, groups, padding, ia_shape, oa_shape, node_mapping):
+        def get_layer_node_input_format(
+            kernel_shape,
+            strides,
+            dilations,
+            groups,
+            padding,
+            ia_shape,
+            oa_shape,
+            node_mapping,
+        ):
             """
             Generate the necessary dictionary items required for the LayerNode creation.
             """
             # convert the data types to precisions based on the onnx definition
 
-
             # Equation
             d = {}
             # IMPORTANT: If any of the input loops require padding, they should be defined as the rightmost dimensions in the equation
             # This is because we construct the dimensionality order and then add the padding to those last dimensions in the order
-            d["equation"] = 'O[b][g][k][oy][ox]+=W[g][k][c][fy][fx]*I[b][g][c][iy][ix]'
+            d["equation"] = "O[b][g][k][oy][ox]+=W[g][k][c][fy][fx]*I[b][g][c][iy][ix]"
 
             # Get dimension sizes from input parameters
-            assert ia_shape[0] == oa_shape[0], "Batch size is different for input and output activations."
+            assert (
+                ia_shape[0] == oa_shape[0]
+            ), "Batch size is different for input and output activations."
             B = oa_shape[0]
             if B == 0:
                 B = 1
             G = groups
-            K = ceil(oa_shape[1]/G)
+            K = ceil(oa_shape[1] / G)
             OX = oa_shape[2]
             OY = oa_shape[3]
-            C = ceil(ia_shape[1]/G)
+            C = ceil(ia_shape[1] / G)
             IX = ia_shape[2]
             IY = ia_shape[3]
             FX = kernel_shape[0]
             FY = kernel_shape[1]
-            d["loop_dim_size"] = {'B': B, 'K': K, 'G': G, "OX": OX, "OY": OY, "C": C, "FX": FX, "FY": FY}
-            d["pr_loop_dim_size"] = {'IX': IX, 'IY': IY}
-            d["dimension_relations"] = [f'ix={strides[0]}*ox+{dilations[0]}*fx', f'iy={strides[1]}*oy+{dilations[1]}*fy']
-            d["operand_precision"] =  {'O': 16, 'O_final': 8, 'W': 8, 'I': 8}
+            d["loop_dim_size"] = {
+                "B": B,
+                "K": K,
+                "G": G,
+                "OX": OX,
+                "OY": OY,
+                "C": C,
+                "FX": FX,
+                "FY": FY,
+            }
+            d["pr_loop_dim_size"] = {"IX": IX, "IY": IY}
+            d["dimension_relations"] = [
+                f"ix={strides[0]}*ox+{dilations[0]}*fx",
+                f"iy={strides[1]}*oy+{dilations[1]}*fy",
+            ]
+            d["operand_precision"] = {"O": 16, "O_final": 8, "W": 8, "I": 8}
             # d["operand_source"] =  {'W': [], 'I': []}
-            d["constant_operands"] =  ['W']
+            d["constant_operands"] = ["W"]
 
-            d["core_allocation"] =  node_mapping["core_allocation"]
-            d["spatial_mapping"] =  node_mapping["spatial_mapping"]
+            d["core_allocation"] = node_mapping["core_allocation"]
+            d["spatial_mapping"] = node_mapping["spatial_mapping"]
             d["temporal_ordering"] = node_mapping.get("temporal_ordering", None)
-            d["memory_operand_links"] =  node_mapping["memory_operand_links"]
+            d["memory_operand_links"] = node_mapping["memory_operand_links"]
 
             # Find the previous layer(s) that should be this node's parent(s)
             node_inputs = self.node.input
             preds = []
             for node_input in node_inputs:
                 for n in self.nodes_outputs:
                     if node_input in self.nodes_outputs[n]:
                         preds.append(n)
-            d["operand_source"] = {'I': preds}
+            d["operand_source"] = {"I": preds}
 
             # Add padding information
-            
-            d["padding"] = {'IY': (padding[0], padding[2]), 'IX': (padding[1], padding[3])}
 
-            return d
+            d["padding"] = {
+                "IY": (padding[0], padding[2]),
+                "IX": (padding[1], padding[3]),
+            }
 
+            return d
 
         attrs = self.node.attribute
         # Find kernel shape in attrs
         kernel_shape = get_attribute_ints_with_name("kernel_shape", attrs, default=None)
         # Find strides in attrs
         strides = get_attribute_ints_with_name("strides", attrs, default=[1, 1])
         # Find dilation rate in attrs
         dilations = get_attribute_ints_with_name("dilations", attrs, default=[1, 1])
         # Find number of groups in attrs
         groups = get_attribute_ints_with_name("group", attrs, default=1)
         # Find padding in attrs
-        padding = get_attribute_ints_with_name("pads", attrs, default=[0,0,0,0])
-        
+        padding = get_attribute_ints_with_name("pads", attrs, default=[0, 0, 0, 0])
+
         # Get the input and output activation shapes
-        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(self.node, self.onnx_model)
+        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(
+            self.node, self.onnx_model
+        )
 
         # Get the input and output activation and weight data type (precision)
-        ia_data_type, oa_data_type, w_data_type = get_input_output_weight_data_type(self.node, self.onnx_model)
+        ia_data_type, oa_data_type, w_data_type = get_input_output_weight_data_type(
+            self.node, self.onnx_model
+        )
 
-        # Get the hw mapping of this node. 
+        # Get the hw mapping of this node.
         if self.node.name in self.mapping:
             node_mapping = self.mapping[self.node.name]
         else:
             try:
                 node_mapping = self.mapping["default"]
             except:
-                raise ValueError(f"There is no mapping provided for node {self.node.name}, nor a default one.")
+                raise ValueError(
+                    f"There is no mapping provided for node {self.node.name}, nor a default one."
+                )
 
         # Take a deepcopy of the mapping, otherwise it will be changed for other layers if using default
         node_mapping = pickle_deepcopy(node_mapping)
 
-        node_attrs = get_layer_node_input_format(kernel_shape, strides, dilations, groups, padding,
-                                                ia_dimension_shape, oa_dimension_shape,
-                                                node_mapping)
+        node_attrs = get_layer_node_input_format(
+            kernel_shape,
+            strides,
+            dilations,
+            groups,
+            padding,
+            ia_dimension_shape,
+            oa_dimension_shape,
+            node_mapping,
+        )
+
+        node_obj = LayerNode(
+            self.node_id,
+            node_attrs,
+            node_name=self.node.name,
+            type=self.node.op_type.lower(),
+        )
 
-        node_obj = LayerNode(self.node_id, node_attrs, node_name=self.node.name, type=self.node.op_type.lower())
-        
         logger.info(f"Parsed Conv node {self.node.name}")
 
         return node_obj
-
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/default.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from zigzag.classes.io.onnx.parser import Parser
 from zigzag.classes.workload.dummy_node import DummyNode
 
 
 class DefaultNodeParser(Parser):
-    """Parse an ONNX node into a DummyNode.
-    """
+    """Parse an ONNX node into a DummyNode."""
+
     def __init__(self, node_id, node, nodes_outputs) -> None:
         super().__init__(node_id, node, nodes_outputs, mapping=None, onnx_model=None)
 
     def run(self):
-        """Run the parser
-        """
+        """Run the parser"""
         dummy_node = self.generate_dummy_node()
         return dummy_node
 
     def generate_dummy_node(self):
         preds = []
         for node_input in self.node.input:
             for n in self.nodes_outputs:
                 if node_input in self.nodes_outputs[n]:
                     preds.append(n)
-        
-        node_obj = DummyNode(self.node_id, preds, node_name=self.node.name, type=self.node.op_type.lower())
+
+        node_obj = DummyNode(
+            self.node_id,
+            preds,
+            node_name=self.node.name,
+            type=self.node.op_type.lower(),
+        )
 
         return node_obj
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/gemm.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/gemm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 from zigzag.classes.io.onnx.parser import Parser
-from zigzag.classes.io.onnx.utils import get_node_input_output_dimension_shapes, get_attribute_ints_with_name
+from zigzag.classes.io.onnx.utils import (
+    get_node_input_output_dimension_shapes,
+    get_attribute_ints_with_name,
+)
 from zigzag.classes.workload.layer_node import LayerNode
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class GemmParser(Parser):
-    """Parses an ONNX Gemm operator into a LayerNode
-    """
+    """Parses an ONNX Gemm operator into a LayerNode"""
 
     def __init__(self, node_id, node, nodes_outputs, mapping, onnx_model) -> None:
         super().__init__(node_id, node, nodes_outputs, mapping, onnx_model)
 
     def run(self):
-        """Run the parser
-        """
+        """Run the parser"""
         layer_node = self.generate_layer_node_for_gemm()
         return layer_node
 
     def generate_layer_node_for_gemm(self):
-
         def get_layer_node_input_format(B, C, K, node_mapping, nodes_outputs):
             """
             Generate the necessary dictionary items required for the Node creation.
             """
             # convert the data types to precisions based on the onnx definition
 
             # Equation
             d = {}
-            d["equation"] = 'O[b][k]+=W[k][c]*I[b][c]'
+            d["equation"] = "O[b][k]+=W[k][c]*I[b][c]"
 
             # Get dimension sizes from input parameters
             K = K
             C = C
             B = B  # Not to be confused with operand 'B' which is the weights
-            d["loop_dim_size"] = {'K': K, 'C': C, 'B': B}
+            d["loop_dim_size"] = {"K": K, "C": C, "B": B}
             d["dimension_relations"] = []
-            d["operand_precision"] = {'O': 16, 'O_final': 8, 'W': 8, 'I': 8}
-            d["operand_source"] = {'W': [], 'I': []}
-            d["constant_operands"] = ['W']
+            d["operand_precision"] = {"O": 16, "O_final": 8, "W": 8, "I": 8}
+            d["operand_source"] = {"W": [], "I": []}
+            d["constant_operands"] = ["W"]
 
             d["core_allocation"] = node_mapping["core_allocation"]
             d["spatial_mapping"] = node_mapping["spatial_mapping"]
             d["temporal_ordering"] = node_mapping.get("temporal_ordering", None)
-            d["memory_operand_links"] = {'O': 'O', 'W': 'I2', 'I': 'I1'}
+            d["memory_operand_links"] = {"O": "O", "W": "I2", "I": "I1"}
 
             # Find the previous layer(s) that should be this node's parent(s)
             node_inputs = self.node.input
             preds = []
             for node_input in node_inputs:
                 for n in nodes_outputs:
                     if node_input in nodes_outputs[n]:
                         preds.append(n)
-            d["operand_source"] = {'I': preds}
+            d["operand_source"] = {"I": preds}
 
             return d
 
-        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(self.node, self.onnx_model)
+        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(
+            self.node, self.onnx_model
+        )
 
         # The Gemm node includes flags for transpose of both of its inputs.
         # If the first input is transposed, we need to transpose its shape here.
         transA = get_attribute_ints_with_name("transA", self.node.attribute, default=0)
         if transA:
             assert len(ia_dimension_shape) == 2
             ia_dimension_shape = (ia_dimension_shape[1], ia_dimension_shape[0])
@@ -72,43 +74,62 @@
         if not ia_dimension_shape:
             weight_name = self.node.input[1]
             initializer_names = [i.name for i in self.onnx_model.graph.initializer]
             weight_name_index = initializer_names.index(weight_name)
             # Get the weight dimensions
             weights = self.onnx_model.graph.initializer[weight_name_index]
             weight_dims = list(weights.dims)
-            assert len(weight_dims) == 2, f"There are {len(weight_dims)} weight dimensions for Gemm node {self.node.name}"
+            assert (
+                len(weight_dims) == 2
+            ), f"There are {len(weight_dims)} weight dimensions for Gemm node {self.node.name}"
             # Check if the weights are transposed
-            transB = get_attribute_ints_with_name("transB", self.node.attribute, default=0)
+            transB = get_attribute_ints_with_name(
+                "transB", self.node.attribute, default=0
+            )
             if transB:
                 weight_dims = [weight_dims[1], weight_dims[0]]
-            assert len(oa_dimension_shape) == 2, "Can't infer ia_dimension_shape if oa_dimension_shape is also not known."
+            assert (
+                len(oa_dimension_shape) == 2
+            ), "Can't infer ia_dimension_shape if oa_dimension_shape is also not known."
             B = oa_dimension_shape[0]
             C = weight_dims[0]
             ia_dimension_shape = [B, C]
 
-        assert len(ia_dimension_shape) == len(oa_dimension_shape) == 2  # First element is batch size, second is input/output channel
-        assert ia_dimension_shape[0] == oa_dimension_shape[0]  # Batch size should be the same for input and output
+        assert (
+            len(ia_dimension_shape) == len(oa_dimension_shape) == 2
+        )  # First element is batch size, second is input/output channel
+        assert (
+            ia_dimension_shape[0] == oa_dimension_shape[0]
+        )  # Batch size should be the same for input and output
         # If the batch size is 0, we discard it by setting it to 1 internally inside ZigZag
         batch_size = ia_dimension_shape[0]
         if batch_size == 0:
             B = 1
         else:
             B = batch_size
         C = ia_dimension_shape[1]
         K = oa_dimension_shape[1]
 
-        # Get the hw mapping of this node. 
+        # Get the hw mapping of this node.
         if self.node.name in self.mapping:
             node_mapping = self.mapping[self.node.name]
         else:
             try:
                 node_mapping = self.mapping["default"]
             except:
-                raise ValueError(f"There is no mapping provided for node {self.node.name}, nor a default one.")
-
-        node_attrs = get_layer_node_input_format(B, C, K, node_mapping, self.nodes_outputs)
-        node_obj = LayerNode(self.node_id, node_attrs, node_name=self.node.name, type=self.node.op_type.lower())
+                raise ValueError(
+                    f"There is no mapping provided for node {self.node.name}, nor a default one."
+                )
+
+        node_attrs = get_layer_node_input_format(
+            B, C, K, node_mapping, self.nodes_outputs
+        )
+        node_obj = LayerNode(
+            self.node_id,
+            node_attrs,
+            node_name=self.node.name,
+            type=self.node.op_type.lower(),
+        )
 
         logger.info(f"Parsed Gemm node {self.node.name}")
 
         return node_obj
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/matmul.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/matmul.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,102 @@
 import onnx
 
 from zigzag.classes.io.onnx.parser import Parser
 from zigzag.classes.io.onnx.utils import get_node_input_output_dimension_shapes
 from zigzag.classes.workload.layer_node import LayerNode
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class MatMulParser(Parser):
-    """Parses an ONNX MatMul operator into a LayerNode
-    """
+    """Parses an ONNX MatMul operator into a LayerNode"""
+
     def __init__(self, node_id, node, nodes_outputs, mapping, onnx_model) -> None:
         super().__init__(node_id, node, nodes_outputs, mapping, onnx_model)
-    
+
     def run(self):
-        """Run the parser
-        """
+        """Run the parser"""
         layer_node = self.generate_layer_node_for_matmul()
         return layer_node
 
     def generate_layer_node_for_matmul(self):
-    
         def get_layer_node_input_format(B, C, K, node_mapping, nodes_outputs):
             """
             Generate the necessary dictionary items required for the Node creation.
             """
             # convert the data types to precisions based on the onnx definition
 
-
             # Equation
             d = {}
-            d["equation"] = 'O[b][k]+=B[k][c]*A[b][c]'
+            d["equation"] = "O[b][k]+=B[k][c]*A[b][c]"
 
             # Get dimension sizes from input parameters
             K = K
             C = C
             B = B  # Not to be confused with operand 'B' which is the weights
-            d["loop_dim_size"] = {'K': K, 'C': C, 'B': B}
+            d["loop_dim_size"] = {"K": K, "C": C, "B": B}
             d["dimension_relations"] = []
-            d["operand_precision"] =  {'O': 16, 'O_final': 8, 'B': 8, 'A': 8}
-            d["operand_source"] =  {'B': [], 'A': []}
-            d["constant_operands"] =  ['B']
+            d["operand_precision"] = {"O": 16, "O_final": 8, "B": 8, "A": 8}
+            d["operand_source"] = {"B": [], "A": []}
+            d["constant_operands"] = ["B"]
 
-            d["core_allocation"] =  node_mapping["core_allocation"]
-            d["spatial_mapping"] =  node_mapping["spatial_mapping"]
+            d["core_allocation"] = node_mapping["core_allocation"]
+            d["spatial_mapping"] = node_mapping["spatial_mapping"]
             d["temporal_ordering"] = node_mapping.get("temporal_ordering", None)
-            d["memory_operand_links"] =  {'O': 'O', 'B': 'I2', 'A': 'I1'}
+            d["memory_operand_links"] = {"O": "O", "B": "I2", "A": "I1"}
 
             # Find the previous layer(s) that should be this node's parent(s)
             node_inputs = self.node.input
             preds = []
             for node_input in node_inputs:
                 for n in nodes_outputs:
                     if node_input in nodes_outputs[n]:
                         preds.append(n)
-            d["operand_source"] = {'A': preds}
+            d["operand_source"] = {"A": preds}
 
             return d
-        
-        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(self.node, self.onnx_model)
 
-        assert len(ia_dimension_shape) == len(oa_dimension_shape) == 2  # First element is batch size, second is input/output channel
-        assert ia_dimension_shape[0] == oa_dimension_shape[0]  # Batch size should be the same for input and output
+        ia_dimension_shape, oa_dimension_shape = get_node_input_output_dimension_shapes(
+            self.node, self.onnx_model
+        )
+
+        assert (
+            len(ia_dimension_shape) == len(oa_dimension_shape) == 2
+        )  # First element is batch size, second is input/output channel
+        assert (
+            ia_dimension_shape[0] == oa_dimension_shape[0]
+        )  # Batch size should be the same for input and output
         # If the batch size is 0, we discard it by setting it to 1 internally inside ZigZag
         batch_size = ia_dimension_shape[0]
         if batch_size == 0:
             B = 1
         else:
             B = batch_size
         C = ia_dimension_shape[1]
         K = oa_dimension_shape[1]
 
-        # Get the hw mapping of this node. 
+        # Get the hw mapping of this node.
         if self.node.name in self.mapping:
             node_mapping = self.mapping[self.node.name]
         else:
             try:
                 node_mapping = self.mapping["default"]
             except:
-                raise ValueError(f"There is no mapping provided for node {self.node.name}, nor a default one.")
-
-        node_attrs = get_layer_node_input_format(B, C, K, node_mapping, self.nodes_outputs)
-        node_obj = LayerNode(self.node_id, node_attrs, node_name=self.node.name, type=self.node.op_type.lower())
+                raise ValueError(
+                    f"There is no mapping provided for node {self.node.name}, nor a default one."
+                )
+
+        node_attrs = get_layer_node_input_format(
+            B, C, K, node_mapping, self.nodes_outputs
+        )
+        node_obj = LayerNode(
+            self.node_id,
+            node_attrs,
+            node_name=self.node.name,
+            type=self.node.op_type.lower(),
+        )
 
         logger.info(f"Parsed MatMul node {self.node.name}")
 
         return node_obj
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/model.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from onnx import ModelProto
 
 from zigzag.classes.io.onnx.default import DefaultNodeParser
 from zigzag.classes.io.onnx.gemm import GemmParser
 from zigzag.classes.io.onnx.matmul import MatMulParser
 from zigzag.classes.io.onnx.conv import ConvParser
-from zigzag.classes.io.onnx.utils import parse_mapping_from_path, parse_onnx_model_from_path
+from zigzag.classes.io.onnx.utils import (
+    parse_mapping_from_path,
+    parse_onnx_model_from_path,
+)
 from zigzag.classes.workload.onnx_workload import ONNXWorkload
 
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class ONNXModelParser:
-    """Parse the ONNX model into a workload.
-    """
+    """Parse the ONNX model into a workload."""
+
     def __init__(self, onnx_model, mapping_path) -> None:
         # Sanity checks on given onnx_model
         if isinstance(onnx_model, str):
             self.onnx_model_path = onnx_model
             self.onnx_model = None
         elif isinstance(onnx_model, ModelProto):
             self.onnx_model_path = None
@@ -83,31 +87,38 @@
         workload = ONNXWorkload()
 
         for node_id, node in enumerate(self.onnx_model.graph.node):
             nodes_inputs[node_id] = node.input
             nodes_outputs[node_id] = node.output
 
             if node.op_type in ["QLinearConv", "Conv"]:
-                parser = ConvParser(node_id, node, nodes_outputs, self.mapping, self.onnx_model)
+                parser = ConvParser(
+                    node_id, node, nodes_outputs, self.mapping, self.onnx_model
+                )
             elif node.op_type in ["MatMul"]:
-                parser = MatMulParser(node_id, node, nodes_outputs, self.mapping, self.onnx_model)
+                parser = MatMulParser(
+                    node_id, node, nodes_outputs, self.mapping, self.onnx_model
+                )
             elif node.op_type in ["Gemm"]:
-                parser = GemmParser(node_id, node, nodes_outputs, self.mapping, self.onnx_model)
+                parser = GemmParser(
+                    node_id, node, nodes_outputs, self.mapping, self.onnx_model
+                )
             else:  # it is not a convolutional node, so create a DummyNode
                 parser = DefaultNodeParser(node_id, node, nodes_outputs)
             node_obj = parser.run()
             # Add the node_obj to the ONNXWorkload
             workload.add(node_id, node_obj)
 
         logger.info(
-            f"Created ONNXWorkload graph with {workload.number_of_nodes()} nodes and {workload.number_of_edges()} edges.")
+            f"Created ONNXWorkload graph with {workload.number_of_nodes()} nodes and {workload.number_of_edges()} edges."
+        )
 
         return workload
 
     def get_onnx_model(self):
         return self.onnx_model
-    
+
     def get_mapping(self):
         return self.mapping
-    
+
     def get_workload(self):
-        return self.workload
+        return self.workload
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/parser.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from abc import ABCMeta, abstractmethod
 
 
 class Parser(metaclass=ABCMeta):
     """Abstract base class that represents a parser of an onnx operator.
     Example: Conv, MatMul, etc.
     """
-    def __init__(self, node_id, node, nodes_outputs, mapping, onnx_model, accelerator=None) -> None:
+
+    def __init__(
+        self, node_id, node, nodes_outputs, mapping, onnx_model, accelerator=None
+    ) -> None:
         self.node_id = node_id
         self.node = node
         self.nodes_outputs = nodes_outputs
         self.mapping = mapping
         self.onnx_model = onnx_model
         self.accelerator = accelerator
-    
+
     @abstractmethod
     def run(self):
         ...
 
     @staticmethod
     def get_spatial_mappings(accelerator, core_allocation):
         # If there is only one possible core allocation, set the spatial mapping as the one(s) of that core
         if isinstance(core_allocation, int):
             core = accelerator.get_core(core_allocation)
             spatial_mappings = core.dataflows
-        elif (isinstance(core_allocation, list) and len(core_allocation) == 1):
+        elif isinstance(core_allocation, list) and len(core_allocation) == 1:
             core = accelerator.get_core(core_allocation[0])
             spatial_mappings = core.dataflows
         else:
             spatial_mappings = None
         return spatial_mappings
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/io/onnx/utils.py` & `zigzag-dse-2.3.2/zigzag/classes/io/onnx/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import importlib
 from os import path
 import onnx
 from onnx import AttributeProto
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 def parse_mapping_from_path(mapping_path):
     """
     Parse the input accelerator residing in accelerator_path.
     """
     # Sanity check on mapping_path
     if mapping_path is None:
         # Update the mapping_path to the default mapping file
         if path.exists("inputs/examples/mapping/default.py"):
             mapping_path = "zigzag.inputs.examples.mapping.default"
         else:
-            raise ValueError("No mapping path/dict provided, and default was not found.")
+            raise ValueError(
+                "No mapping path/dict provided, and default was not found."
+            )
     global module
     module = importlib.import_module(mapping_path)
     mapping = module.mapping
     if "default" in mapping:
         default_present = "\u2705"
     else:
         default_present = "\u274C"
-    logger.debug(f"Parsed mapping with {len(mapping)} different entries. Default: {default_present}.")
+    logger.debug(
+        f"Parsed mapping with {len(mapping)} different entries. Default: {default_present}."
+    )
     return mapping
 
+
 def parse_onnx_model_from_path(onnx_model_path):
     return onnx.load(onnx_model_path, load_external_data=False)
 
 
 def get_attribute_ints_with_name(name, attrs, default=None):
     """
     Retrieves the attrs[name_idx].ints from attrs.
@@ -45,48 +51,68 @@
         name_idx = attrs_names.index(name)
         attr_type = attrs[name_idx].type
         if attr_type == AttributeProto.AttributeType.INT:
             return attrs[name_idx].i
         elif attr_type == AttributeProto.AttributeType.INTS:
             return attrs[name_idx].ints
         else:
-            raise NotImplementedError(f"Attribute extraction of type {attr_type} not supported.")
+            raise NotImplementedError(
+                f"Attribute extraction of type {attr_type} not supported."
+            )
     except ValueError:
         if default is not None:
             return default
         else:
-            raise ValueError(f"attrs has no attribute called {name} and no default was given. Names = {attrs_names}.")
+            raise ValueError(
+                f"attrs has no attribute called {name} and no default was given. Names = {attrs_names}."
+            )
+
 
 from onnx import AttributeProto
 
+
 def get_node_input_output_dimension_shapes(node, model):
-        value_info = model.graph.value_info
-        if not value_info:
-            raise ValueError("value_info of model is empty. Make sure you are loading in an inferred model. " \
-            "See https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#running-shape-inference-on-an-onnx-model")
-        # get tensor names of the inputs and outputs of the model
-        model_input_names = [input.name for input in model.graph.input]
-        model_output_names = [output.name for output in model.graph.output]
-        # get tensor names of the tensors in shapes
-        shapes_names = [shape.name for shape in value_info]
-        # get input and output activation dimension sizes
-        # get input activation name
-        ia_name = node.input[0]  # assumed it is the first input, don't see a way to otherwise know
-        # check if this is a global input of the model, if so, retrieve dimension shape from model inputs
-        if ia_name in model_input_names:
-            # Find index of this input in list of input names
-            ia_index = model_input_names.index(ia_name)
-            ia_dimension_shape = [dim.dim_value for dim in model.graph.input[ia_index].type.tensor_type.shape.dim]
-        else:  # it should be present in the shapes variable as it's not an input or output of the model
-            ia_index = shapes_names.index(ia_name)
-            ia_dimension_shape = [dim.dim_value for dim in value_info[ia_index].type.tensor_type.shape.dim]
-
-        # repeat the same for the output activation of this layer
-        oa_name = node.output[0]
-        if oa_name in model_output_names:
-            oa_index = model_output_names.index(oa_name)
-            oa_dimension_shape = [dim.dim_value for dim in model.graph.output[oa_index].type.tensor_type.shape.dim]
-        else:
-            oa_index = shapes_names.index(oa_name)
-            oa_dimension_shape = [dim.dim_value for dim in value_info[oa_index].type.tensor_type.shape.dim]
+    value_info = model.graph.value_info
+    if not value_info:
+        raise ValueError(
+            "value_info of model is empty. Make sure you are loading in an inferred model. "
+            "See https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#running-shape-inference-on-an-onnx-model"
+        )
+    # get tensor names of the inputs and outputs of the model
+    model_input_names = [input.name for input in model.graph.input]
+    model_output_names = [output.name for output in model.graph.output]
+    # get tensor names of the tensors in shapes
+    shapes_names = [shape.name for shape in value_info]
+    # get input and output activation dimension sizes
+    # get input activation name
+    ia_name = node.input[
+        0
+    ]  # assumed it is the first input, don't see a way to otherwise know
+    # check if this is a global input of the model, if so, retrieve dimension shape from model inputs
+    if ia_name in model_input_names:
+        # Find index of this input in list of input names
+        ia_index = model_input_names.index(ia_name)
+        ia_dimension_shape = [
+            dim.dim_value
+            for dim in model.graph.input[ia_index].type.tensor_type.shape.dim
+        ]
+    else:  # it should be present in the shapes variable as it's not an input or output of the model
+        ia_index = shapes_names.index(ia_name)
+        ia_dimension_shape = [
+            dim.dim_value for dim in value_info[ia_index].type.tensor_type.shape.dim
+        ]
+
+    # repeat the same for the output activation of this layer
+    oa_name = node.output[0]
+    if oa_name in model_output_names:
+        oa_index = model_output_names.index(oa_name)
+        oa_dimension_shape = [
+            dim.dim_value
+            for dim in model.graph.output[oa_index].type.tensor_type.shape.dim
+        ]
+    else:
+        oa_index = shapes_names.index(oa_name)
+        oa_dimension_shape = [
+            dim.dim_value for dim in value_info[oa_index].type.tensor_type.shape.dim
+        ]
 
-        return ia_dimension_shape, oa_dimension_shape
+    return ia_dimension_shape, oa_dimension_shape
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/mapping/combined_mapping.py` & `zigzag-dse-2.3.2/zigzag/classes/mapping/combined_mapping.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,20 +13,26 @@
     """
 
     def __init__(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
         self.rd_out_to_low = rd_out_to_low
         self.wr_in_by_low = wr_in_by_low
         self.rd_out_to_high = rd_out_to_high
         self.wr_in_by_high = wr_in_by_high
-        ''' format used in the original ZigZag version '''
-        self.info_list = [(self.rd_out_to_low, self.wr_in_by_low), (self.rd_out_to_high, self.wr_in_by_high)]
+        """ format used in the original ZigZag version """
+        self.info_list = [
+            (self.rd_out_to_low, self.wr_in_by_low),
+            (self.rd_out_to_high, self.wr_in_by_high),
+        ]
 
     def update_single_dir_data(self, dir: str, new_value):
         setattr(self, dir, new_value)
-        self.info_list = [(self.rd_out_to_low, self.wr_in_by_low), (self.rd_out_to_high, self.wr_in_by_high)]
+        self.info_list = [
+            (self.rd_out_to_low, self.wr_in_by_low),
+            (self.rd_out_to_high, self.wr_in_by_high),
+        ]
 
     def get_total_read_outs_to_above(self, scaling: float = 1):
         """
         Return the total amount of times this memory interface is read from to the level above.
         If scaling is the energy cost per read, this returns the total read energy.
         """
         return scaling * self.rd_out_to_high
@@ -49,27 +55,31 @@
         """
         Return the total amount of times this memory interface is written to from the level below.
         If scaling is the energy cost per write, this returns the total read energy.
         """
         return scaling * self.wr_in_by_low
 
     def __add__(self, other):
-        return FourWayDataMoving(self.rd_out_to_low + other.rd_out_to_low,
-                                 self.wr_in_by_low + other.wr_in_by_low,
-                                 self.rd_out_to_high + other.rd_out_to_high,
-                                 self.wr_in_by_high + other.wr_in_by_high)
+        return FourWayDataMoving(
+            self.rd_out_to_low + other.rd_out_to_low,
+            self.wr_in_by_low + other.wr_in_by_low,
+            self.rd_out_to_high + other.rd_out_to_high,
+            self.wr_in_by_high + other.wr_in_by_high,
+        )
 
     def __mul__(self, other):
-        return FourWayDataMoving(self.rd_out_to_low * other,
-                                 self.wr_in_by_low * other,
-                                 self.rd_out_to_high * other,
-                                 self.wr_in_by_high * other)
+        return FourWayDataMoving(
+            self.rd_out_to_low * other,
+            self.wr_in_by_low * other,
+            self.rd_out_to_high * other,
+            self.wr_in_by_high * other,
+        )
 
     def __iter__(self):
-        for e in ['rd_out_to_low', 'wr_in_by_low', 'rd_out_to_high', 'wr_in_by_high']:
+        for e in ["rd_out_to_low", "wr_in_by_low", "rd_out_to_high", "wr_in_by_high"]:
             yield e
 
     def __repr__(self):
         return f"4waydatamoving (rd /\\: {self.rd_out_to_high}, wr V: {self.wr_in_by_high}, rd V: {self.rd_out_to_low}, wr /\\: {self.wr_in_by_low})"
 
     def __jsonrepr__(self):
         return repr(self)
@@ -93,48 +103,80 @@
         self.req_mem_bw_aver = FourWayDataMoving(0, 0, 0, 0)
         self.req_mem_bw_inst = FourWayDataMoving(0, 0, 0, 0)
         self.data_trans_period = FourWayDataMoving(0, 0, 0, 0)
         self.data_trans_period_count = FourWayDataMoving(0, 0, 0, 0)
         self.data_trans_amount_per_period = FourWayDataMoving(0, 0, 0, 0)
         self.inst_data_trans_window = FourWayDataMoving(0, 0, 0, 0)
 
-    ''' For every memory, there are 4 data transfer link in the hierarchy: 
-    rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high '''
+    """ For every memory, there are 4 data transfer link in the hierarchy: 
+    rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high """
 
-    def set_data_elem_move_count(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        self.data_elem_move_count = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_data_elem_move_count(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        self.data_elem_move_count = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_data_precision(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        self.data_precision = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_data_precision(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        self.data_precision = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_req_mem_bw_aver(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        self.req_mem_bw_aver = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_req_mem_bw_aver(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        self.req_mem_bw_aver = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_req_mem_bw_inst(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        self.req_mem_bw_inst = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_req_mem_bw_inst(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        self.req_mem_bw_inst = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_data_trans_period(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        """ data_trans_period: every how many cycle, the memory link need to be activated for a certain duration """
-        self.data_trans_period = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_data_trans_period(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        """data_trans_period: every how many cycle, the memory link need to be activated for a certain duration"""
+        self.data_trans_period = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_data_trans_period_count(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        """ data_trans_period_count: to finish all the for-loop computation, how many such ideal_period is required """
-        self.data_trans_period_count = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_data_trans_period_count(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        """data_trans_period_count: to finish all the for-loop computation, how many such ideal_period is required"""
+        self.data_trans_period_count = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_data_trans_amount_per_period(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        """ data_trans_amount_per_period: data amount that being transferred for each single period """
-        self.data_trans_amount_per_period = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_data_trans_amount_per_period(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        """data_trans_amount_per_period: data amount that being transferred for each single period"""
+        self.data_trans_amount_per_period = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
-    def set_inst_data_trans_window(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        """ inst_data_trans_window: the allowed memory updating window, assuming the served memory level
-        is non-double buffered (thus need to avoid the data overwriting issue) """
-        self.inst_data_trans_window = FourWayDataMoving(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
+    def set_inst_data_trans_window(
+        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+    ):
+        """inst_data_trans_window: the allowed memory updating window, assuming the served memory level
+        is non-double buffered (thus need to avoid the data overwriting issue)"""
+        self.inst_data_trans_window = FourWayDataMoving(
+            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+        )
 
     def update_single_dir_data(self, direction, new_value):
-        """ update a single direction value for all data move attributes """
+        """update a single direction value for all data move attributes"""
         self.data_elem_move_count.update_single_dir_data(direction, new_value)
         self.data_precision.update_single_dir_data(direction, new_value)
         self.req_mem_bw_aver.update_single_dir_data(direction, new_value)
         self.req_mem_bw_inst.update_single_dir_data(direction, new_value)
         self.data_trans_period.update_single_dir_data(direction, new_value)
         self.data_trans_period_count.update_single_dir_data(direction, new_value)
         self.data_trans_amount_per_period.update_single_dir_data(direction, new_value)
@@ -150,217 +192,288 @@
 class Mapping:
     """
     Collect information of a complete mapping (spatial and temporal)
     NOTE: Mapping is HW-unaware, i.e. Mapping doesn't take in HW information
     like memory bw, access cost, size and so on.
     """
 
-    def __init__(self, accelerator: Accelerator, spatial_mapping: Dict or SpatialMapping, temporal_mapping: Dict or TemporalMapping,
-                 layer_node: LayerNode, access_same_data_considered_as_no_access: bool = False):
+    def __init__(
+        self,
+        accelerator: Accelerator,
+        spatial_mapping: Dict or SpatialMapping,
+        temporal_mapping: Dict or TemporalMapping,
+        layer_node: LayerNode,
+        access_same_data_considered_as_no_access: bool = False,
+    ):
         """
         Mapping object can be initialized with separate spatial and temporal mappings
         """
         self.accelerator = accelerator
         if type(spatial_mapping) is SpatialMapping:
             self.spatial_mapping = spatial_mapping
         else:
             self.spatial_mapping = SpatialMapping(spatial_mapping, layer_node)
         if type(temporal_mapping) is TemporalMapping:
             self.temporal_mapping = temporal_mapping
         else:
             self.temporal_mapping = TemporalMapping(temporal_mapping, layer_node)
         self.layer_node = layer_node
         self.operand_list = layer_node.operand_list
-        self.access_same_data_considered_as_no_access = access_same_data_considered_as_no_access
+        self.access_same_data_considered_as_no_access = (
+            access_same_data_considered_as_no_access
+        )
         self.mem_level = self.temporal_mapping.mem_level
-        ''' Initialize unit_mem_data_movement, which collects all the important data movement info 
+        """ Initialize unit_mem_data_movement, which collects all the important data movement info 
         related to each unit memory, such as data access count, data precision, required memory BW to 
-        prevent stall, data transfer rate, etc. '''
+        prevent stall, data transfer rate, etc. """
         self.unit_mem_data_movement = {
-            op: [[] for _ in range(self.mem_level[op])]
-            for op in self.operand_list
+            op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list
         }
 
-        ''' Combine spatial and temporal mapping dictionary into "joint_mapping_dict" in order to 
-        enable decoupling pr loops into r and ir loops in one go '''
+        """ Combine spatial and temporal mapping dictionary into "joint_mapping_dict" in order to 
+        enable decoupling pr loops into r and ir loops in one go """
         self.combine_spatial_temporal_mapping_dict()
 
-        ''' Decouple pr loops into r and ir loops, preparing for later mapping info extraction '''
+        """ Decouple pr loops into r and ir loops, preparing for later mapping info extraction """
         self.combined_mapping_dict_1s1t_reform = mapping_assist_funcs.decouple_pr_loop(
             self.combined_mapping_dict_1s1t, layer_node
         )
         self.combined_mapping_dict_1s2t_reform = mapping_assist_funcs.decouple_pr_loop(
             self.combined_mapping_dict_1s2t, layer_node
         )
 
-        ''' Distinguish final output from partial output: "psum_flag" '''
+        """ Distinguish final output from partial output: "psum_flag" """
         self.distinguish_output()
 
-        ''' Generate a dictionary that collect data precision for each operand at each arch level '''
+        """ Generate a dictionary that collect data precision for each operand at each arch level """
         self.gen_data_precision_dict()
 
-        ''' Generate r/ir loop size list at each level for each operand '''
+        """ Generate r/ir loop size list at each level for each operand """
         self.gen_r_ir_loop_list()
 
-        ''' Calculate data size at each memory level, including total data size and 
-        unrolled data size (data at each unrolled memory unit). Unit used: # element '''
+        """ Calculate data size at each memory level, including total data size and 
+        unrolled data size (data at each unrolled memory unit). Unit used: # element """
         self.calc_data_size()
 
-        ''' Calculate the effective data size at each unrolled memory unit.
+        """ Calculate the effective data size at each unrolled memory unit.
         Effective data size: the unrolled data size divided by all top r loops at that level.
-        Unit used: # element '''
+        Unit used: # element """
         self.calc_effective_data_size()
 
-        ''' Calculate data access count at each memory level. Unit used: # element 
-        NOTE: this data access is not memory word access! '''
+        """ Calculate data access count at each memory level. Unit used: # element 
+        NOTE: this data access is not memory word access! """
         self.calc_data_access()
 
-        ''' Calculate required memory bandwidth and the periodic data transfer pattern '''
+        """ Calculate required memory bandwidth and the periodic data transfer pattern """
         self.calc_req_mem_bw_and_data_transfer_rate()
 
-        ''' Ignore the data traffic between the top level memory and the external world '''
+        """ Ignore the data traffic between the top level memory and the external world """
         self.disable_data_traffic_external()
 
     def combine_spatial_temporal_mapping_dict(self):
-        """ Combine spatial and temporal mapping dictionary into combined_mapping_dict by
+        """Combine spatial and temporal mapping dictionary into combined_mapping_dict by
         inserting spatial loops above temporal loops at each level.
 
         - combined_mapping_dict_1s1t: corresponding level's smap and tmap are merged together.
         Each level's data size is the total data size.
 
         - combined_mapping_dict_1s2t: each level's smap is merged to level+1's tmap.
         Each level's data size is the unrolled data size.
         """
 
-        ''' Initialization '''
-        combined_mapping_dict_1s1t = {op: [
-            [] for _ in range(self.spatial_mapping.arch_level[op])
-        ] for op in self.operand_list}
-        combined_mapping_dict_1s2t = {op: [
-            [] for _ in range(self.spatial_mapping.arch_level[op] + 1)
-        ] for op in self.operand_list}
+        """ Initialization """
+        combined_mapping_dict_1s1t = {
+            op: [[] for _ in range(self.spatial_mapping.arch_level[op])]
+            for op in self.operand_list
+        }
+        combined_mapping_dict_1s2t = {
+            op: [[] for _ in range(self.spatial_mapping.arch_level[op] + 1)]
+            for op in self.operand_list
+        }
         su_dict_seed = self.spatial_mapping.mapping_dict_origin
-        ''' Add an empty innermost level and an empty outermost level '''
+        """ Add an empty innermost level and an empty outermost level """
         tm_dict_seed = {
-            op: [[]] + tm_list + [[]] for op, tm_list in self.temporal_mapping.mapping_dic_stationary.items()}
+            op: [[]] + tm_list + [[]]
+            for op, tm_list in self.temporal_mapping.mapping_dic_stationary.items()
+        }
 
-        ''' Combining '''
+        """ Combining """
         for operand in self.operand_list:
             for level, current_level_su_loops in enumerate(su_dict_seed[operand]):
                 current_level_tm_loops = tm_dict_seed[operand][level]
                 above_level_tm_loops = tm_dict_seed[operand][level + 1]
-                combined_mapping_dict_1s1t[operand][level] = current_level_tm_loops + current_level_su_loops
-                combined_mapping_dict_1s2t[operand][level + 1] = above_level_tm_loops + current_level_su_loops
+                combined_mapping_dict_1s1t[operand][level] = (
+                    current_level_tm_loops + current_level_su_loops
+                )
+                combined_mapping_dict_1s2t[operand][level + 1] = (
+                    above_level_tm_loops + current_level_su_loops
+                )
 
         self.combined_mapping_dict_1s1t = combined_mapping_dict_1s1t
         self.combined_mapping_dict_1s2t = combined_mapping_dict_1s2t
 
     def distinguish_output(self):
         """
         This function generates an list "psum_flag" that identify whether an output memory
         level holds partial or final output.
         E.g., psum_flag = [True, True, False] means that there are 3 memory levels for output and only the outermost
         memory level hold the final output, the 1st and 2nd memory levels need to store partial output for some time.
         For indexing convenience, we add an extra False to the end of the psum_flag list.
         """
         output_operand = self.layer_node.output_operand
-        output_loop_dim_relevancy = self.layer_node.operand_loop_dim_reform[output_operand]
-        ''' output_ir_flag indicate whether at an architectural level, there is output's ir loop in it.
-        True for yes, there is. '''
+        output_loop_dim_relevancy = self.layer_node.operand_loop_dim_reform[
+            output_operand
+        ]
+        """ output_ir_flag indicate whether at an architectural level, there is output's ir loop in it.
+        True for yes, there is. """
         output_arch_level = self.spatial_mapping.arch_level[output_operand]
         output_ir_flag = [False] * output_arch_level
-        for level, current_level_loops in enumerate(self.combined_mapping_dict_1s1t_reform[output_operand]):
+        for level, current_level_loops in enumerate(
+            self.combined_mapping_dict_1s1t_reform[output_operand]
+        ):
             for loop_type, loop_dim in current_level_loops:
-                if loop_type in output_loop_dim_relevancy['ir'] and loop_dim > 1:
+                if loop_type in output_loop_dim_relevancy["ir"] and loop_dim > 1:
                     output_ir_flag[level] = True
                     break
-        ''' reversely check from current level to the top level whether there is ir loop shows up in the middle, 
-        False means final output is present at current level '''
-        psum_flag_H2L = [any(output_ir_flag[lv:output_arch_level]) for lv in reversed(range(output_arch_level))]
+        """ reversely check from current level to the top level whether there is ir loop shows up in the middle, 
+        False means final output is present at current level """
+        psum_flag_H2L = [
+            any(output_ir_flag[lv:output_arch_level])
+            for lv in reversed(range(output_arch_level))
+        ]
         psum_flag_L2H = list(reversed(psum_flag_H2L))
-        self.psum_flag = psum_flag_L2H[1:] + [False]  # add an extra False on top for later indexing convenience
+        self.psum_flag = psum_flag_L2H[1:] + [
+            False
+        ]  # add an extra False on top for later indexing convenience
 
     def gen_data_precision_dict(self):
         """
         This function generates a dictionary that collect data precision for each operand at each arch level
         """
         input_operands = self.layer_node.input_operands
         output_operand = self.layer_node.output_operand
         data_precision_dict = {
-            op: [self.layer_node.operand_precision[op]] * (self.mem_level[op] + 1) for op in input_operands
+            op: [self.layer_node.operand_precision[op]] * (self.mem_level[op] + 1)
+            for op in input_operands
         }
         data_precision_dict[output_operand] = []
         for i in range(self.mem_level[output_operand] + 1):
             if self.psum_flag[i]:
-                data_precision_dict[output_operand].append(self.layer_node.operand_precision[output_operand])
+                data_precision_dict[output_operand].append(
+                    self.layer_node.operand_precision[output_operand]
+                )
             else:
-                data_precision_dict[output_operand].append(self.layer_node.operand_precision[output_operand + '_final'])
+                data_precision_dict[output_operand].append(
+                    self.layer_node.operand_precision[output_operand + "_final"]
+                )
         self.data_precision_dict = data_precision_dict
 
     def gen_r_ir_loop_list(self):
         """
         Given the combined mapping, generate r/ir loop size list at each level for each operand
         """
         combined_mapping = self.combined_mapping_dict_1s1t_reform
         combined_mapping2 = self.combined_mapping_dict_1s2t_reform
         relevancy_table = self.layer_node.operand_loop_dim_reform
         r_loop_size_per_level = {
             op: [
-                prod([lp_dim for lp_type, lp_dim in combined_mapping[op][lv] if lp_type in relevancy_table[op]['r']])
+                prod(
+                    [
+                        lp_dim
+                        for lp_type, lp_dim in combined_mapping[op][lv]
+                        if lp_type in relevancy_table[op]["r"]
+                    ]
+                )
                 for lv in range(self.spatial_mapping.arch_level[op])
-            ] for op in self.operand_list
+            ]
+            for op in self.operand_list
         }
         r_loop_size_per_level2 = {
             op: [
-                prod([lp_dim for lp_type, lp_dim in combined_mapping2[op][lv] if lp_type in relevancy_table[op]['r']])
+                prod(
+                    [
+                        lp_dim
+                        for lp_type, lp_dim in combined_mapping2[op][lv]
+                        if lp_type in relevancy_table[op]["r"]
+                    ]
+                )
                 for lv in range(self.spatial_mapping.arch_level[op])
-            ] for op in self.operand_list
+            ]
+            for op in self.operand_list
         }
         ir_loop_size_per_level = {
             op: [
-                prod([lp_dim for lp_type, lp_dim in combined_mapping[op][lv] if lp_type in relevancy_table[op]['ir']])
+                prod(
+                    [
+                        lp_dim
+                        for lp_type, lp_dim in combined_mapping[op][lv]
+                        if lp_type in relevancy_table[op]["ir"]
+                    ]
+                )
                 for lv in range(self.spatial_mapping.arch_level[op])
-            ] for op in self.operand_list
+            ]
+            for op in self.operand_list
         }
         ir_loop_size_per_level2 = {
             op: [
-                prod([lp_dim for lp_type, lp_dim in combined_mapping2[op][lv] if lp_type in relevancy_table[op]['ir']])
+                prod(
+                    [
+                        lp_dim
+                        for lp_type, lp_dim in combined_mapping2[op][lv]
+                        if lp_type in relevancy_table[op]["ir"]
+                    ]
+                )
                 for lv in range(self.spatial_mapping.arch_level[op])
-            ] for op in self.operand_list
+            ]
+            for op in self.operand_list
         }
 
-        ''' current and below levels (cabl) r loop size '''
+        """ current and below levels (cabl) r loop size """
         r_loop_size_cabl = {
-            op: [round(prod(r_loop_size_per_level[op][0:lv + 1]))
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(prod(r_loop_size_per_level[op][0 : lv + 1]))
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
         r_loop_size_cabl2 = {
-            op: [round(prod(r_loop_size_per_level2[op][0:lv + 1]))
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(prod(r_loop_size_per_level2[op][0 : lv + 1]))
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
-        ''' current and below levels (cabl) ir loop size '''
+        """ current and below levels (cabl) ir loop size """
         ir_loop_size_cabl = {
-            op: [prod(ir_loop_size_per_level[op][0:lv + 1])
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                prod(ir_loop_size_per_level[op][0 : lv + 1])
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
-        ''' current and below levels (cabl) ir loop size '''
+        """ current and below levels (cabl) ir loop size """
         ir_loop_size_cabl2 = {
-            op: [prod(ir_loop_size_per_level2[op][0:lv + 1])
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                prod(ir_loop_size_per_level2[op][0 : lv + 1])
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
-        ''' current and above levels (caal) ir loop size, only for output operand for calculating psum backflow access count '''
+        """ current and above levels (caal) ir loop size, only for output operand for calculating psum backflow access count """
         output_operand = self.layer_node.output_operand
-        O_ir_loop_size_caal = [prod(ir_loop_size_per_level[output_operand][lv:self.spatial_mapping.arch_level[output_operand]])
-                               for lv in range(self.spatial_mapping.arch_level[output_operand])]
-        ''' append two extra 1 to the list to facilitate the psum bcakflow access calculation later
-        We can see it as adding two output memory levels on top with no data reuse. '''
+        O_ir_loop_size_caal = [
+            prod(
+                ir_loop_size_per_level[output_operand][
+                    lv : self.spatial_mapping.arch_level[output_operand]
+                ]
+            )
+            for lv in range(self.spatial_mapping.arch_level[output_operand])
+        ]
+        """ append two extra 1 to the list to facilitate the psum bcakflow access calculation later
+        We can see it as adding two output memory levels on top with no data reuse. """
         O_ir_loop_size_caal.extend([1, 1])
 
         self.r_loop_size_per_level = r_loop_size_per_level
         self.r_loop_size_per_level2 = r_loop_size_per_level2
         self.ir_loop_size_per_level = ir_loop_size_per_level
         self.r_loop_size_cabl = r_loop_size_cabl
         self.r_loop_size_cabl2 = r_loop_size_cabl2
@@ -372,252 +485,351 @@
         """
         Based on the r loop size list, calculate the data size held by each architectural level.
 
         data_elem_per_level_unrolled: data size held inside of each unrolled unit at each architectural level
         data_elem_per_level: total data size at each architectural level (= data_elem_per_level_unrolled * unique unit count)
         """
         data_elem_per_level_unrolled = {
-            op: [round(self.r_loop_size_cabl2[op][lv])
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(self.r_loop_size_cabl2[op][lv])
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
 
         data_bit_per_level_unrolled = {
-            op: [round(self.r_loop_size_cabl2[op][lv]) * self.data_precision_dict[op][lv]
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(self.r_loop_size_cabl2[op][lv]) * self.data_precision_dict[op][lv]
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
 
         data_elem_per_level = {
-            op: [round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv])
-                 for lv, data_elem_unrolled in enumerate(data_elem_per_level_unrolled[op])]
+            op: [
+                round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv])
+                for lv, data_elem_unrolled in enumerate(
+                    data_elem_per_level_unrolled[op]
+                )
+            ]
             for op in self.operand_list
         }
 
         data_bit_per_level = {
-            op: [round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv]) * self.data_precision_dict[op][lv]
-                 for lv, data_elem_unrolled in enumerate(data_elem_per_level_unrolled[op])]
+            op: [
+                round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv])
+                * self.data_precision_dict[op][lv]
+                for lv, data_elem_unrolled in enumerate(
+                    data_elem_per_level_unrolled[op]
+                )
+            ]
             for op in self.operand_list
         }
 
         self.data_elem_per_level_unrolled = data_elem_per_level_unrolled
         self.data_bit_per_level_unrolled = data_bit_per_level_unrolled
         self.data_elem_per_level = data_elem_per_level
         self.data_bit_per_level = data_bit_per_level
 
     def calc_effective_data_size(self):
         """
         Calculate the effective data size for getting the allowed memory updating window in latency calculation.
         The effective data size is calculated by using data_elem_per_level_unrolled divided by the top r loops.
         """
         effective_data_elem = {
-            op: [data_elem_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
-                 for lv, data_elem_unrolled in enumerate(self.data_elem_per_level_unrolled[op])]
+            op: [
+                data_elem_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
+                for lv, data_elem_unrolled in enumerate(
+                    self.data_elem_per_level_unrolled[op]
+                )
+            ]
             for op in self.operand_list
         }
 
         effective_data_bit = {
-            op: [data_bit_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
-                 for lv, data_bit_unrolled in enumerate(self.data_bit_per_level_unrolled[op])]
+            op: [
+                data_bit_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
+                for lv, data_bit_unrolled in enumerate(
+                    self.data_bit_per_level_unrolled[op]
+                )
+            ]
             for op in self.operand_list
         }
         self.effective_data_elem = effective_data_elem
         self.effective_data_bit = effective_data_bit
 
     def calc_data_access(self):
         """
         Based on the ir loop size list and the total MAC Op count, calculate the data access
         at each memory level in a bottom-up way.
         """
         total_MAC_count = self.layer_node.total_MAC_count
 
-        ''' 
+        """ 
         data_access_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand 
         data_access_raw: each memory levels' spatial loops and temporal loops are put together (combined_mapping_dict_1s1t)
         data_access_raw2: each memory levels' spatial loops are put to memory level + 1s' temporal loops location (combined_mapping_dict_1s2t)
-        '''
+        """
         data_access_raw = {
-            op: [round(total_MAC_count / self.ir_loop_size_cabl[op][lv])
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(total_MAC_count / self.ir_loop_size_cabl[op][lv])
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
         data_access_raw2 = {
-            op: [round(total_MAC_count / self.ir_loop_size_cabl2[op][lv])
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                round(total_MAC_count / self.ir_loop_size_cabl2[op][lv])
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
         self.data_access_raw = data_access_raw
         self.data_access_raw2 = data_access_raw2
 
-        ''' Distinguish read and write, unify input operands and output operand '''
-        ''' For input operands '''
+        """ Distinguish read and write, unify input operands and output operand """
+        """ For input operands """
         for operand in self.layer_node.input_operands:
             for mem_level in range(self.mem_level[operand]):
                 unit_mem_data_movement = DataMovePattern(operand, mem_level)
 
-                ''' data access count '''
-                if self.access_same_data_considered_as_no_access and mem_level == 0 and \
-                        self.accelerator.get_core(self.layer_node.get_core_allocation()).mem_r_bw_dict[self.layer_node.memory_operand_links[operand]][mem_level] >= \
-                        self.data_bit_per_level[operand][mem_level] // self.spatial_mapping.unit_unique[operand][mem_level+1]:
+                """ data access count """
+                if (
+                    self.access_same_data_considered_as_no_access
+                    and mem_level == 0
+                    and self.accelerator.get_core(
+                        self.layer_node.get_core_allocation()
+                    ).mem_r_bw_dict[self.layer_node.memory_operand_links[operand]][
+                        mem_level
+                    ]
+                    >= self.data_bit_per_level[operand][mem_level]
+                    // self.spatial_mapping.unit_unique[operand][mem_level + 1]
+                ):
                     # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
                     # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
-                    rd_out_to_low = data_access_raw[operand][mem_level] // self.temporal_mapping.MAC_level_data_stationary_cycle[operand]
+                    rd_out_to_low = (
+                        data_access_raw[operand][mem_level]
+                        // self.temporal_mapping.MAC_level_data_stationary_cycle[
+                            operand
+                        ]
+                    )
                 else:
                     rd_out_to_low = data_access_raw[operand][mem_level]
                 wr_in_by_low = 0
                 rd_out_to_high = 0
                 wr_in_by_high = data_access_raw2[operand][mem_level + 1]
-                unit_mem_data_movement.set_data_elem_move_count(rd_out_to_low, wr_in_by_low,
-                                                                rd_out_to_high, wr_in_by_high)
-                ''' data precision '''
+                unit_mem_data_movement.set_data_elem_move_count(
+                    rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+                )
+                """ data precision """
                 rd_out_to_low_pre = self.layer_node.operand_precision[operand]
                 wr_in_by_low_pre = 0
                 rd_out_to_high_pre = 0
                 wr_in_by_high_pre = self.layer_node.operand_precision[operand]
-                unit_mem_data_movement.set_data_precision(rd_out_to_low_pre, wr_in_by_low_pre,
-                                                          rd_out_to_high_pre, wr_in_by_high_pre)
+                unit_mem_data_movement.set_data_precision(
+                    rd_out_to_low_pre,
+                    wr_in_by_low_pre,
+                    rd_out_to_high_pre,
+                    wr_in_by_high_pre,
+                )
 
                 self.unit_mem_data_movement[operand][mem_level] = unit_mem_data_movement
 
-        ''' For output operand '''
+        """ For output operand """
         output_operand = self.layer_node.output_operand
         for mem_level in range(self.mem_level[output_operand]):
             unit_mem_data_movement = DataMovePattern(output_operand, mem_level)
 
-            ''' Note that the index for data_access_raw is arch_level, which is one level more than mem_level. 
+            """ Note that the index for data_access_raw is arch_level, which is one level more than mem_level. 
             the first arch_level means the operational array level (e.g. MAC array level); 
-            the first mem_level means the innermost memory level (e.g. register file level).'''
+            the first mem_level means the innermost memory level (e.g. register file level)."""
 
-            ''' data access count '''
+            """ data access count """
             wr_in_by_low = data_access_raw[output_operand][mem_level]
-            rd_out_to_low = self.layer_node.operand_size_elem[output_operand] * \
-                            (self.O_ir_loop_size_caal[mem_level + 1] - 1)
+            rd_out_to_low = self.layer_node.operand_size_elem[output_operand] * (
+                self.O_ir_loop_size_caal[mem_level + 1] - 1
+            )
 
             rd_out_to_high = data_access_raw2[output_operand][mem_level + 1]
-            wr_in_by_high = self.layer_node.operand_size_elem[output_operand] * \
-                            (self.O_ir_loop_size_caal[mem_level + 2] - 1)
+            wr_in_by_high = self.layer_node.operand_size_elem[output_operand] * (
+                self.O_ir_loop_size_caal[mem_level + 2] - 1
+            )
 
-            unit_mem_data_movement.set_data_elem_move_count(rd_out_to_low, wr_in_by_low,
-                                                            rd_out_to_high, wr_in_by_high)
+            unit_mem_data_movement.set_data_elem_move_count(
+                rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
+            )
 
-            ''' data precision '''
+            """ data precision """
             if rd_out_to_low != 0:
-                ''' partial output data precision '''
+                """partial output data precision"""
                 wr_in_by_low_pre = self.layer_node.operand_precision[output_operand]
                 rd_out_to_low_pre = self.layer_node.operand_precision[output_operand]
             else:
-                ''' final output data precision '''
-                wr_in_by_low_pre = self.layer_node.operand_precision[output_operand + '_final']
+                """final output data precision"""
+                wr_in_by_low_pre = self.layer_node.operand_precision[
+                    output_operand + "_final"
+                ]
                 rd_out_to_low_pre = 0
             if wr_in_by_high != 0:
-                ''' partial output data precision '''
+                """partial output data precision"""
                 wr_in_by_high_pre = self.layer_node.operand_precision[output_operand]
                 rd_out_to_high_pre = self.layer_node.operand_precision[output_operand]
             else:
-                ''' final output data precision '''
+                """final output data precision"""
                 wr_in_by_high_pre = 0
-                rd_out_to_high_pre = self.layer_node.operand_precision[output_operand + '_final']
-
-            unit_mem_data_movement.set_data_precision(rd_out_to_low_pre, wr_in_by_low_pre,
-                                                      rd_out_to_high_pre, wr_in_by_high_pre)
+                rd_out_to_high_pre = self.layer_node.operand_precision[
+                    output_operand + "_final"
+                ]
+
+            unit_mem_data_movement.set_data_precision(
+                rd_out_to_low_pre,
+                wr_in_by_low_pre,
+                rd_out_to_high_pre,
+                wr_in_by_high_pre,
+            )
 
-            self.unit_mem_data_movement[output_operand][mem_level] = unit_mem_data_movement
+            self.unit_mem_data_movement[output_operand][
+                mem_level
+            ] = unit_mem_data_movement
 
     def calc_req_mem_bw_and_data_transfer_rate(self):
         """
         This function calculates the average & instant required memory bw and the periodic data transfer pattern.
         """
 
         if self.access_same_data_considered_as_no_access:
-            ''' For input operands, add operational array level's 'MAC_level_data_stationary_cycle' cycle in the below to align with the list length of data_each_level '''
-            cycle_each_level = {op: [self.temporal_mapping.MAC_level_data_stationary_cycle[op]] + self.temporal_mapping.cycle_cabl_level[op] for op in self.layer_node.input_operands}
-            ''' For output operands, add operational array level's 1 cycle in the below to align with the list length of data_each_level '''
-            cycle_each_level[self.layer_node.output_operand] = [1] + self.temporal_mapping.cycle_cabl_level[self.layer_node.output_operand]
+            """For input operands, add operational array level's 'MAC_level_data_stationary_cycle' cycle in the below to align with the list length of data_each_level"""
+            cycle_each_level = {
+                op: [self.temporal_mapping.MAC_level_data_stationary_cycle[op]]
+                + self.temporal_mapping.cycle_cabl_level[op]
+                for op in self.layer_node.input_operands
+            }
+            """ For output operands, add operational array level's 1 cycle in the below to align with the list length of data_each_level """
+            cycle_each_level[self.layer_node.output_operand] = [
+                1
+            ] + self.temporal_mapping.cycle_cabl_level[self.layer_node.output_operand]
         else:
-            cycle_each_level = {op: [1] + self.temporal_mapping.cycle_cabl_level[op] for op in self.operand_list}
+            cycle_each_level = {
+                op: [1] + self.temporal_mapping.cycle_cabl_level[op]
+                for op in self.operand_list
+            }
         data_each_level_unrolled = self.data_elem_per_level_unrolled
 
-        ''' Add the mem BW boost factor 1 on the top (the memory BW boost factor from outside to top memory) 
-        to align with the list length of data_each_level '''
-        mem_bw_boost_factor = {op: self.spatial_mapping.mem_bw_boost[op] + [1] for op in self.operand_list}
+        """ Add the mem BW boost factor 1 on the top (the memory BW boost factor from outside to top memory) 
+        to align with the list length of data_each_level """
+        mem_bw_boost_factor = {
+            op: self.spatial_mapping.mem_bw_boost[op] + [1] for op in self.operand_list
+        }
 
-        ''' req_mem_bw_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand '''
-        ''' "_L/_H" indicates for each data transfer link (DTL), the lower/higher memory level's required BW, 
+        """ req_mem_bw_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand """
+        """ "_L/_H" indicates for each data transfer link (DTL), the lower/higher memory level's required BW, 
         e.g. for the DTL of Global Buffer (Weight) talking to spatially unrolled Weight Reg File, 
         each Weight Reg File's required write BW is indicated by "_L", 
-        while Global Buffer (Weight)'s required read BW is indicate by "_H" '''
+        while Global Buffer (Weight)'s required read BW is indicate by "_H" """
         req_mem_bw_L_raw = {
-            op: [data_each_level_unrolled[op][lv] / cycle_each_level[op][lv]
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                data_each_level_unrolled[op][lv] / cycle_each_level[op][lv]
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
         req_mem_bw_H_raw = {
-            op: [req_mem_bw_L_raw[op][lv] * mem_bw_boost_factor[op][lv]
-                 for lv in range(self.spatial_mapping.arch_level[op])]
+            op: [
+                req_mem_bw_L_raw[op][lv] * mem_bw_boost_factor[op][lv]
+                for lv in range(self.spatial_mapping.arch_level[op])
+            ]
             for op in self.operand_list
         }
 
         """
         Calculates the average required memory bw.
         """
 
-        ''' Distinguish read and write, unify input operands and output operand '''
-        ''' For input operands '''
+        """ Distinguish read and write, unify input operands and output operand """
+        """ For input operands """
         for operand in self.layer_node.input_operands:
             for mem_level in range(self.mem_level[operand]):
-                ''' average required memory BW '''
+                """average required memory BW"""
                 rd_out_to_low_bw = req_mem_bw_H_raw[operand][mem_level]
                 wr_in_by_low_bw = 0
                 rd_out_to_high_bw = 0
                 wr_in_by_high_bw = req_mem_bw_L_raw[operand][mem_level + 1]
                 self.unit_mem_data_movement[operand][mem_level].set_req_mem_bw_aver(
-                    rd_out_to_low_bw, wr_in_by_low_bw,
-                    rd_out_to_high_bw, wr_in_by_high_bw
+                    rd_out_to_low_bw,
+                    wr_in_by_low_bw,
+                    rd_out_to_high_bw,
+                    wr_in_by_high_bw,
                 )
-                ''' data transfer period '''
+                """ data transfer period """
                 rd_out_to_low_pd = cycle_each_level[operand][mem_level]
                 wr_in_by_low_pd = 0
                 rd_out_to_high_pd = 0
                 wr_in_by_high_pd = cycle_each_level[operand][mem_level + 1]
                 self.unit_mem_data_movement[operand][mem_level].set_data_trans_period(
-                    rd_out_to_low_pd, wr_in_by_low_pd,
-                    rd_out_to_high_pd, wr_in_by_high_pd
+                    rd_out_to_low_pd,
+                    wr_in_by_low_pd,
+                    rd_out_to_high_pd,
+                    wr_in_by_high_pd,
+                )
+                """ data transfer period count """
+                rd_out_to_low_pc = (
+                    self.temporal_mapping.total_cycle
+                    // cycle_each_level[operand][mem_level]
                 )
-                ''' data transfer period count '''
-                rd_out_to_low_pc = self.temporal_mapping.total_cycle // cycle_each_level[operand][mem_level]
                 wr_in_by_low_pc = 0
                 rd_out_to_high_pc = 0
-                wr_in_by_high_pc = self.temporal_mapping.total_cycle // cycle_each_level[operand][mem_level + 1]
-                self.unit_mem_data_movement[operand][mem_level].set_data_trans_period_count(
-                    rd_out_to_low_pc, wr_in_by_low_pc,
-                    rd_out_to_high_pc, wr_in_by_high_pc
-                )
-                ''' per-period data transfer amount '''
-                rd_out_to_low_da = data_each_level_unrolled[operand][mem_level] * \
-                                   mem_bw_boost_factor[operand][mem_level]
+                wr_in_by_high_pc = (
+                    self.temporal_mapping.total_cycle
+                    // cycle_each_level[operand][mem_level + 1]
+                )
+                self.unit_mem_data_movement[operand][
+                    mem_level
+                ].set_data_trans_period_count(
+                    rd_out_to_low_pc,
+                    wr_in_by_low_pc,
+                    rd_out_to_high_pc,
+                    wr_in_by_high_pc,
+                )
+                """ per-period data transfer amount """
+                rd_out_to_low_da = (
+                    data_each_level_unrolled[operand][mem_level]
+                    * mem_bw_boost_factor[operand][mem_level]
+                )
                 wr_in_by_low_da = 0
                 rd_out_to_high_da = 0
                 wr_in_by_high_da = data_each_level_unrolled[operand][mem_level + 1]
 
-                self.unit_mem_data_movement[operand][mem_level].set_data_trans_amount_per_period(
-                    rd_out_to_low_da, wr_in_by_low_da,
-                    rd_out_to_high_da, wr_in_by_high_da
+                self.unit_mem_data_movement[operand][
+                    mem_level
+                ].set_data_trans_amount_per_period(
+                    rd_out_to_low_da,
+                    wr_in_by_low_da,
+                    rd_out_to_high_da,
+                    wr_in_by_high_da,
                 )
 
-        ''' For output operand '''
+        """ For output operand """
         output_operand = self.layer_node.output_operand
         for mem_level in range(self.mem_level[output_operand]):
             wr_in_by_low_bw = req_mem_bw_H_raw[output_operand][mem_level]
             rd_out_to_high_bw = req_mem_bw_L_raw[output_operand][mem_level + 1]
             wr_in_by_low_pd = cycle_each_level[output_operand][mem_level]
             rd_out_to_high_pd = cycle_each_level[output_operand][mem_level + 1]
-            wr_in_by_low_pc = self.temporal_mapping.total_cycle // cycle_each_level[output_operand][mem_level]
-            rd_out_to_high_pc = self.temporal_mapping.total_cycle // cycle_each_level[output_operand][mem_level + 1]
-            wr_in_by_low_da = data_each_level_unrolled[output_operand][mem_level] * \
-                              mem_bw_boost_factor[output_operand][mem_level]
+            wr_in_by_low_pc = (
+                self.temporal_mapping.total_cycle
+                // cycle_each_level[output_operand][mem_level]
+            )
+            rd_out_to_high_pc = (
+                self.temporal_mapping.total_cycle
+                // cycle_each_level[output_operand][mem_level + 1]
+            )
+            wr_in_by_low_da = (
+                data_each_level_unrolled[output_operand][mem_level]
+                * mem_bw_boost_factor[output_operand][mem_level]
+            )
             rd_out_to_high_da = data_each_level_unrolled[output_operand][mem_level + 1]
 
             if self.psum_flag[mem_level]:
                 rd_out_to_low_bw = wr_in_by_low_bw
                 rd_out_to_low_pd = wr_in_by_low_pd
                 rd_out_to_low_pc = wr_in_by_low_pc
                 rd_out_to_low_da = wr_in_by_low_da
@@ -634,61 +846,96 @@
                 wr_in_by_high_da = rd_out_to_high_da
             else:
                 wr_in_by_high_bw = 0
                 wr_in_by_high_pd = 0
                 wr_in_by_high_pc = 0
                 wr_in_by_high_da = 0
 
-            ''' average required memory BW '''
+            """ average required memory BW """
             self.unit_mem_data_movement[output_operand][mem_level].set_req_mem_bw_aver(
-                rd_out_to_low_bw, wr_in_by_low_bw,
-                rd_out_to_high_bw, wr_in_by_high_bw
+                rd_out_to_low_bw, wr_in_by_low_bw, rd_out_to_high_bw, wr_in_by_high_bw
+            )
+            """ data transfer period """
+            self.unit_mem_data_movement[output_operand][
+                mem_level
+            ].set_data_trans_period(
+                rd_out_to_low_pd, wr_in_by_low_pd, rd_out_to_high_pd, wr_in_by_high_pd
             )
-            ''' data transfer period '''
-            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_period(
-                rd_out_to_low_pd, wr_in_by_low_pd,
-                rd_out_to_high_pd, wr_in_by_high_pd
-            )
-            ''' data transfer period count '''
-            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_period_count(
-                rd_out_to_low_pc, wr_in_by_low_pc,
-                rd_out_to_high_pc, wr_in_by_high_pc
-            )
-            ''' per-period data transfer amount '''
-            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_amount_per_period(
-                rd_out_to_low_da, wr_in_by_low_da,
-                rd_out_to_high_da, wr_in_by_high_da
+            """ data transfer period count """
+            self.unit_mem_data_movement[output_operand][
+                mem_level
+            ].set_data_trans_period_count(
+                rd_out_to_low_pc, wr_in_by_low_pc, rd_out_to_high_pc, wr_in_by_high_pc
+            )
+            """ per-period data transfer amount """
+            self.unit_mem_data_movement[output_operand][
+                mem_level
+            ].set_data_trans_amount_per_period(
+                rd_out_to_low_da, wr_in_by_low_da, rd_out_to_high_da, wr_in_by_high_da
             )
 
         """
         Calculate the instant memory updating behavior.
         """
         top_ir_loop_size = self.temporal_mapping.top_ir_loop_size
         for operand in self.operand_list:
-            for level, data_movement_item in enumerate(self.unit_mem_data_movement[operand]):
+            for level, data_movement_item in enumerate(
+                self.unit_mem_data_movement[operand]
+            ):
                 req_mem_bw_aver = data_movement_item.req_mem_bw_aver
-                ''' calculate "instant required memory BW" based on "average required memory BW" '''
-                rd_out_to_low_bw = req_mem_bw_aver.rd_out_to_low * top_ir_loop_size[operand][level]
-                wr_in_by_low_bw = req_mem_bw_aver.wr_in_by_low * top_ir_loop_size[operand][level]
-                rd_out_to_high_bw = req_mem_bw_aver.rd_out_to_high * top_ir_loop_size[operand][level + 1]
-                wr_in_by_high_bw = req_mem_bw_aver.wr_in_by_high * top_ir_loop_size[operand][level + 1]
-                data_movement_item.set_req_mem_bw_inst(rd_out_to_low_bw, wr_in_by_low_bw,
-                                                       rd_out_to_high_bw, wr_in_by_high_bw)
+                """ calculate "instant required memory BW" based on "average required memory BW" """
+                rd_out_to_low_bw = (
+                    req_mem_bw_aver.rd_out_to_low * top_ir_loop_size[operand][level]
+                )
+                wr_in_by_low_bw = (
+                    req_mem_bw_aver.wr_in_by_low * top_ir_loop_size[operand][level]
+                )
+                rd_out_to_high_bw = (
+                    req_mem_bw_aver.rd_out_to_high
+                    * top_ir_loop_size[operand][level + 1]
+                )
+                wr_in_by_high_bw = (
+                    req_mem_bw_aver.wr_in_by_high * top_ir_loop_size[operand][level + 1]
+                )
+                data_movement_item.set_req_mem_bw_inst(
+                    rd_out_to_low_bw,
+                    wr_in_by_low_bw,
+                    rd_out_to_high_bw,
+                    wr_in_by_high_bw,
+                )
 
                 data_trans_period = data_movement_item.data_trans_period
-                ''' calculate "instant data transferring window", assuming non-double buffered memory '''
-                rd_out_to_low_wd = data_trans_period.rd_out_to_low // top_ir_loop_size[operand][level]
-                wr_in_by_low_wd = data_trans_period.wr_in_by_low // top_ir_loop_size[operand][level]
-                rd_out_to_high_wd = data_trans_period.rd_out_to_high // top_ir_loop_size[operand][level + 1]
-                wr_in_by_high_wd = data_trans_period.wr_in_by_high // top_ir_loop_size[operand][level + 1]
-                data_movement_item.set_inst_data_trans_window(rd_out_to_low_wd, wr_in_by_low_wd,
-                                                              rd_out_to_high_wd, wr_in_by_high_wd)
+                """ calculate "instant data transferring window", assuming non-double buffered memory """
+                rd_out_to_low_wd = (
+                    data_trans_period.rd_out_to_low // top_ir_loop_size[operand][level]
+                )
+                wr_in_by_low_wd = (
+                    data_trans_period.wr_in_by_low // top_ir_loop_size[operand][level]
+                )
+                rd_out_to_high_wd = (
+                    data_trans_period.rd_out_to_high
+                    // top_ir_loop_size[operand][level + 1]
+                )
+                wr_in_by_high_wd = (
+                    data_trans_period.wr_in_by_high
+                    // top_ir_loop_size[operand][level + 1]
+                )
+                data_movement_item.set_inst_data_trans_window(
+                    rd_out_to_low_wd,
+                    wr_in_by_low_wd,
+                    rd_out_to_high_wd,
+                    wr_in_by_high_wd,
+                )
 
     def disable_data_traffic_external(self):
         """
         This function set all the data traffic between the top level memory and the external world to 0
         in unit_mem_data_movement.
         """
         for operand in self.operand_list:
             mem_level = self.mem_level[operand] - 1
-            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data('rd_out_to_high', 0)
-            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data('wr_in_by_high', 0)
+            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(
+                "rd_out_to_high", 0
+            )
+            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(
+                "wr_in_by_high", 0
+            )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/mapping/loop.py` & `zigzag-dse-2.3.2/zigzag/classes/mapping/loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from abc import ABCMeta
 
 
 class Loop(metaclass=ABCMeta):
     """Abstract base class that represents a loop.
     Could be spatial or temporal loop.
     """
+
     def __init__(self, dimension, size) -> None:
         """Initialize this Loop object.
 
         Args:
             dimension (str): The dimension, e.g. "K"
-            size (float): The loop size, e.g. 16.0 
+            size (float): The loop size, e.g. 16.0
 
         Returns:
             None: None
         """
         self.type = None
         self.dimension = dimension
         self.size = size
 
     # def __str__(self):
     #     return f"Loop({self.dimension},{self.size})"
 
     # def __repr__(self):
-    #     return str(self)
+    #     return str(self)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag-dse-2.3.2/zigzag/classes/mapping/mapping_assist_funcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from zigzag.utils import pickle_deepcopy
 
 if TYPE_CHECKING:
     from zigzag.classes.workload.layer_node import LayerNode
 
 
-
 class Loop:
     """
     Collect information of each single loop tuple in mapping.
     Applied range: from the lowest architectural level to the current level.
     """
 
     def __init__(self, loop: tuple, MAC_op: int, data_elem: int):
@@ -25,146 +24,200 @@
     def __str__(self):
         return str(self.loop)
 
     def __repr__(self):
         return str(self.loop)
 
 
-def decouple_pr_loop(mapping_dict: Dict, layer_node: 'LayerNode'):
+def decouple_pr_loop(mapping_dict: Dict, layer_node: "LayerNode"):
     """
     This function decouples the pr loops into data size (r loops) and data reuse (ir loops).
     It also provides a transferred mapping dictionary in which the pr loops are replaced by r and ir loops.
     """
 
-    operand_loop_dim = {op: layer_node.operand_loop_dim[op] for op in mapping_dict.keys()}
-    r_ir_operand_loop_LUT = {op: relevance['r']+relevance['ir'] for (op, relevance) in operand_loop_dim.items()}
-    pr_operand_loop_LUT = {op: relevance['pr'] for (op, relevance) in operand_loop_dim.items() if relevance['pr'] != {}}
+    operand_loop_dim = {
+        op: layer_node.operand_loop_dim[op] for op in mapping_dict.keys()
+    }
+    r_ir_operand_loop_LUT = {
+        op: relevance["r"] + relevance["ir"]
+        for (op, relevance) in operand_loop_dim.items()
+    }
+    pr_operand_loop_LUT = {
+        op: relevance["pr"]
+        for (op, relevance) in operand_loop_dim.items()
+        if relevance["pr"] != {}
+    }
     pr_operand_list = list(pr_operand_loop_LUT.keys())
     mapping_dict_reform = pickle_deepcopy(mapping_dict)
 
-    ''' current and below level pr data size '''
+    """ current and below level pr data size """
     cabl_pr_data_size = {}
-    ''' current and below level pr data reuse '''
+    """ current and below level pr data reuse """
     cabl_pr_data_reuse = {}
 
-    ''' each single pr loop data size '''
+    """ each single pr loop data size """
     per_pr_data_size = {}
-    ''' each single pr loop data reuse '''
+    """ each single pr loop data reuse """
     per_pr_data_reuse = {}
 
     for operand in pr_operand_list:
 
-        ''' initialize current and below level pr loop size '''
+        """initialize current and below level pr loop size"""
         cabl_pr_lp_size = {
-            pr_data_dim: {pr_loop_dim: 1 for pr_loop_dim in pr_operand_loop_LUT[operand][pr_data_dim]}
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()}
+            pr_data_dim: {
+                pr_loop_dim: 1
+                for pr_loop_dim in pr_operand_loop_LUT[operand][pr_data_dim]
+            }
+            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        }
 
-        ''' initialize current and below level pr data size '''
+        """ initialize current and below level pr data size """
         cabl_pr_data_size[operand] = {
             pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()}
+            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        }
 
-        ''' initialize current and below level pr data reuse '''
+        """ initialize current and below level pr data reuse """
         cabl_pr_data_reuse[operand] = {
             pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()}
+            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        }
 
-        ''' initialize per pr loop data size '''
+        """ initialize per pr loop data size """
         per_pr_data_size[operand] = {
             pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()}
+            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        }
 
-        ''' initialize per pr loop data reuse '''
+        """ initialize per pr loop data reuse """
         per_pr_data_reuse[operand] = {
             pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()}
+            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        }
 
-        ''' update the cabl_pr_lp_size by multiply pr loop size across architectural level '''
+        """ update the cabl_pr_lp_size by multiply pr loop size across architectural level """
         for level, loop_list in enumerate(mapping_dict[operand]):
             for loop_type, loop_size in loop_list:
                 if loop_type in r_ir_operand_loop_LUT[operand]:
                     continue
                 for pr_data_dim in pr_operand_loop_LUT[operand].keys():
-                    if any(lp_type == loop_type for lp_type in pr_operand_loop_LUT[operand][pr_data_dim]):
+                    if any(
+                        lp_type == loop_type
+                        for lp_type in pr_operand_loop_LUT[operand][pr_data_dim]
+                    ):
                         cabl_pr_lp_size[pr_data_dim][loop_type] *= loop_size
 
-                        ''' compute pr related data dimension size and data dimension reuse at current and below joint levels
-                        based on pr_funcs (dynamic functions extracted in LayerNode). Each pr loop is decoupled into r and ir loops. '''
-                        pr_loop_combined_to_r = layer_node.calc_tensor_dim(cabl_pr_lp_size[pr_data_dim], pr_data_dim)
-                        pr_loop_combined_to_ir = prod(cabl_pr_lp_size[pr_data_dim].values()) / pr_loop_combined_to_r
-                        cabl_pr_data_size[operand][pr_data_dim][level].append(pr_loop_combined_to_r)
-                        cabl_pr_data_reuse[operand][pr_data_dim][level].append(pr_loop_combined_to_ir)
+                        """ compute pr related data dimension size and data dimension reuse at current and below joint levels
+                        based on pr_funcs (dynamic functions extracted in LayerNode). Each pr loop is decoupled into r and ir loops. """
+                        pr_loop_combined_to_r = layer_node.calc_tensor_dim(
+                            cabl_pr_lp_size[pr_data_dim], pr_data_dim
+                        )
+                        pr_loop_combined_to_ir = (
+                            prod(cabl_pr_lp_size[pr_data_dim].values())
+                            / pr_loop_combined_to_r
+                        )
+                        cabl_pr_data_size[operand][pr_data_dim][level].append(
+                            pr_loop_combined_to_r
+                        )
+                        cabl_pr_data_reuse[operand][pr_data_dim][level].append(
+                            pr_loop_combined_to_ir
+                        )
 
-        ''' compute pr related data dimension size and data dimension reuse at each level for each pr loop
-         based on cabl_pr_data_size/cabl_pr_data_reuse '''
+        """ compute pr related data dimension size and data dimension reuse at each level for each pr loop
+         based on cabl_pr_data_size/cabl_pr_data_reuse """
         for pr_data_dim in cabl_pr_data_size[operand].keys():
             data_size_list = cabl_pr_data_size[operand][pr_data_dim]
             data_reuse_list = cabl_pr_data_reuse[operand][pr_data_dim]
             previous_data_size = 1
             previous_data_data_reuse = 1
             for level, va_list in enumerate(data_size_list):
                 for idx in range(len(va_list)):
                     per_pr_data_size[operand][pr_data_dim][level].append(
-                        data_size_list[level][idx] / previous_data_size)
+                        data_size_list[level][idx] / previous_data_size
+                    )
                     per_pr_data_reuse[operand][pr_data_dim][level].append(
-                        data_reuse_list[level][idx] / previous_data_data_reuse)
+                        data_reuse_list[level][idx] / previous_data_data_reuse
+                    )
                     previous_data_size = data_size_list[level][idx]
                     previous_data_data_reuse = data_reuse_list[level][idx]
 
-        mapping_dict_reform[operand] = replace_pr_loop_in_mapping(mapping_dict[operand], per_pr_data_size[operand],
-                                                                  per_pr_data_reuse[operand], pr_operand_loop_LUT[operand],
-                                                                  r_ir_operand_loop_LUT[operand])
+        mapping_dict_reform[operand] = replace_pr_loop_in_mapping(
+            mapping_dict[operand],
+            per_pr_data_size[operand],
+            per_pr_data_reuse[operand],
+            pr_operand_loop_LUT[operand],
+            r_ir_operand_loop_LUT[operand],
+        )
 
     # return mapping_dict_reform, cabl_pr_data_size, cabl_pr_data_reuse, per_pr_data_size, per_pr_data_reuse
     return mapping_dict_reform
 
 
-def replace_pr_loop_in_mapping(single_operand_mapping: Dict, per_pr_data_size: Dict, per_pr_data_reuse: Dict,
-                               pr_operand_loop_LUT: Dict, r_ir_operand_loop_LUT: List):
+def replace_pr_loop_in_mapping(
+    single_operand_mapping: Dict,
+    per_pr_data_size: Dict,
+    per_pr_data_reuse: Dict,
+    pr_operand_loop_LUT: Dict,
+    r_ir_operand_loop_LUT: List,
+):
     """
     This function replaces all pr loops in a mapping of a single operand with r and ir loops.
     """
     mapping_new = pickle_deepcopy(single_operand_mapping)
 
     for level, loop_list in enumerate(single_operand_mapping):
-        ''' Introduce the current level pr loop index to distinguish different pr loops at the same architectural level '''
-        cl_pr_lp_idx_local = {pr_data_dim: 0 for pr_data_dim in pr_operand_loop_LUT.keys()}
+        """Introduce the current level pr loop index to distinguish different pr loops at the same architectural level"""
+        cl_pr_lp_idx_local = {
+            pr_data_dim: 0 for pr_data_dim in pr_operand_loop_LUT.keys()
+        }
         cl_pr_lp_idx_global = 0
         for idx, (loop_type, loop_size) in enumerate(loop_list):
             if loop_type in r_ir_operand_loop_LUT:
                 continue
             for pr_data_dim in pr_operand_loop_LUT.keys():
-                if any(lp_type == loop_type for lp_type in pr_operand_loop_LUT[pr_data_dim]):
-                    ''' replace the pr loop in the mapping by r loop '''
+                if any(
+                    lp_type == loop_type for lp_type in pr_operand_loop_LUT[pr_data_dim]
+                ):
+                    """replace the pr loop in the mapping by r loop"""
                     pr_idx_local = cl_pr_lp_idx_local[pr_data_dim]
                     pr_idx_global = cl_pr_lp_idx_global
-                    mapping_new[level][idx + pr_idx_global] = \
-                        (pr_data_dim + '_r', per_pr_data_size[pr_data_dim][level][pr_idx_local])
-                    ''' insert ir loop after the r loop '''
+                    mapping_new[level][idx + pr_idx_global] = (
+                        pr_data_dim + "_r",
+                        per_pr_data_size[pr_data_dim][level][pr_idx_local],
+                    )
+                    """ insert ir loop after the r loop """
                     # NOTE: Here we insert the ir loop after/above the r loop, which indicates that we ignore the input FIFO effect
                     # during current level feeds data to below level. We could also insert the ir loop before/below the r loop,
                     # which leads to more energy-efficient mapping if the innermost ir loop merging down is enabled.
-                    mapping_new[level].insert(idx + pr_idx_global + 1,
-                                              (pr_data_dim + '_ir', per_pr_data_reuse[pr_data_dim][level][pr_idx_local]))
-                    ''' update the pr loop index '''
+                    mapping_new[level].insert(
+                        idx + pr_idx_global + 1,
+                        (
+                            pr_data_dim + "_ir",
+                            per_pr_data_reuse[pr_data_dim][level][pr_idx_local],
+                        ),
+                    )
+                    """ update the pr loop index """
                     cl_pr_lp_idx_local[pr_data_dim] += 1
                     cl_pr_lp_idx_global += 1
 
     return mapping_new
 
 
-def calc_data_size_MAC_count_per_loop(mapping_dict_reform: Dict, operand_loop_dim_reform: Dict):
+def calc_data_size_MAC_count_per_loop(
+    mapping_dict_reform: Dict, operand_loop_dim_reform: Dict
+):
     """
     This function generates detailed information for each single loop item for each operand.
     """
     detailed_mapping_dict = deepcopy(mapping_dict_reform)
     for operand, mapping_list in mapping_dict_reform.items():
         MAC_count = 1
         data_elem = 1
         for level, loop_list in enumerate(mapping_dict_reform[operand]):
             for idx, (loop_type, loop_size) in enumerate(loop_list):
                 MAC_count *= loop_size
-                if loop_type in operand_loop_dim_reform[operand]['r']:
+                if loop_type in operand_loop_dim_reform[operand]["r"]:
                     data_elem *= loop_size
-                detailed_mapping_dict[operand][level][idx] = \
-                    Loop((loop_type, loop_size), round(MAC_count), round(data_elem))
+                detailed_mapping_dict[operand][level][idx] = Loop(
+                    (loop_type, loop_size), round(MAC_count), round(data_elem)
+                )
     return detailed_mapping_dict
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag-dse-2.3.2/zigzag/classes/mapping/spatial/spatial_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,38 +8,40 @@
 
 
 class SpatialMapping:
     """
     Class that collect all the info related to spatial mapping.
     """
 
-    def __init__(self, spatial_mapping_dict: Dict, layer_node: 'LayerNode'):
+    def __init__(self, spatial_mapping_dict: Dict, layer_node: "LayerNode"):
         self.mapping_dict_origin = spatial_mapping_dict
-        self.mapping_dict_reform = mapping_assist_funcs.decouple_pr_loop(spatial_mapping_dict, layer_node)
+        self.mapping_dict_reform = mapping_assist_funcs.decouple_pr_loop(
+            spatial_mapping_dict, layer_node
+        )
         self.layer_node = layer_node
         self.operand_list = layer_node.operand_list
 
-        ''' Extract architecture level count for each operand from spatial mapping definition, starting from MAC level '''
+        """ Extract architecture level count for each operand from spatial mapping definition, starting from MAC level """
         self.arch_level = {op: len(smap) for (op, smap) in spatial_mapping_dict.items()}
 
-        ''' Calculate unrolled loop size for different loop types (r/ir/total) '''
+        """ Calculate unrolled loop size for different loop types (r/ir/total) """
         self.calc_unroll_size()
 
-        ''' Calculate total/unique/duplicate unit count '''
+        """ Calculate total/unique/duplicate unit count """
         self.calc_unit_count()
 
-        ''' Calculate data serve scope: each data element serves/(is served by) how many unit at below level 
-        NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes. '''
+        """ Calculate data serve scope: each data element serves/(is served by) how many unit at below level 
+        NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes. """
         self.calc_data_serve_scope()
 
-        ''' Calculate memory bandwidth incremental factor between architectural levels
-        NOTE: mem_bw_boost_factor doesn't include MAC level, thus is one level less than other spatial mapping attributes. '''
+        """ Calculate memory bandwidth incremental factor between architectural levels
+        NOTE: mem_bw_boost_factor doesn't include MAC level, thus is one level less than other spatial mapping attributes. """
         self.calc_mem_bw_boost_factor()
 
-        ''' Added for loma: Get list of the spatially unrolled loops, without any information about arch levels'''
+        """ Added for loma: Get list of the spatially unrolled loops, without any information about arch levels"""
         self.save_spatial_loop_dim_size()
 
     def __str__(self):
         return f"SpatialMapping({self.mapping_dict_origin})"
 
     def __repr__(self):
         return str(self)
@@ -57,91 +59,125 @@
         """
         return self.mapping_dict_origin[op][level]
 
     def calc_unroll_size(self):
         """
         Calculate unrolled loop size for different loop types (r/ir/total) per operand per architecture level
         """
-        ''' Initialization '''
+        """ Initialization """
         unroll_size_r = {op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()}
-        unroll_size_ir = {op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()}
-        unroll_size_total = {op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()}
+        unroll_size_ir = {
+            op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()
+        }
+        unroll_size_total = {
+            op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()
+        }
 
-        ''' Go through the reformed spatial mapping and extract the unroll size '''
+        """ Go through the reformed spatial mapping and extract the unroll size """
         for operand in self.operand_list:
-            for level, current_level_loops in enumerate(self.mapping_dict_reform[operand]):
+            for level, current_level_loops in enumerate(
+                self.mapping_dict_reform[operand]
+            ):
                 for loop_type, loop_dim in current_level_loops:
-                    if loop_type in self.layer_node.operand_loop_dim_reform[operand]['r']:
+                    if (
+                        loop_type
+                        in self.layer_node.operand_loop_dim_reform[operand]["r"]
+                    ):
                         unroll_size_r[operand][level] *= loop_dim
                     else:
                         unroll_size_ir[operand][level] *= loop_dim
                     unroll_size_total[operand][level] *= loop_dim
 
         self.unroll_size_r = unroll_size_r
         self.unroll_size_ir = unroll_size_ir
         self.unroll_size_total = unroll_size_total
 
     def calc_unit_count(self):
         """
         Calculate total/unique/duplicate unit count per operand per architecture level
         """
-        ''' Number of unit at each level (for each operand) '''
+        """ Number of unit at each level (for each operand) """
         # Added round call as number doesn't remain integer due to self.mapping_dict_reform number instability
-        unit_count = {op: [
-            round(prod(self.unroll_size_total[op][lv:self.arch_level[op]])) for lv in range(self.arch_level[op])
-        ] for op in self.operand_list}
+        unit_count = {
+            op: [
+                round(prod(self.unroll_size_total[op][lv : self.arch_level[op]]))
+                for lv in range(self.arch_level[op])
+            ]
+            for op in self.operand_list
+        }
 
-        ''' ASSERT: The bottom level (MAC level) unit count must be the same for all operand '''
+        """ ASSERT: The bottom level (MAC level) unit count must be the same for all operand """
         bottom_unit_count = [unit_count[op][0] for op in unit_count.keys()]
-        assert all(x == bottom_unit_count[0] for x in bottom_unit_count), \
-            f"The MAC level unit count is not the same for all operand {bottom_unit_count}, please correct the spatial mapping."
-
-        ''' Number of unit at each level that hold unique data (for each operand) '''
-        unit_unique = {op: [
-            prod(self.unroll_size_r[op][lv:self.arch_level[op]]) for lv in range(self.arch_level[op])
-        ] for op in self.operand_list}
-
-        ''' Number of unit at each level that hold the same data (for each operand) '''
-        unit_duplicate = {op: [
-            prod(self.unroll_size_ir[op][lv:self.arch_level[op]]) for lv in range(self.arch_level[op])
-        ] for op in self.operand_list}
+        assert all(
+            x == bottom_unit_count[0] for x in bottom_unit_count
+        ), f"The MAC level unit count is not the same for all operand {bottom_unit_count}, please correct the spatial mapping."
+
+        """ Number of unit at each level that hold unique data (for each operand) """
+        unit_unique = {
+            op: [
+                prod(self.unroll_size_r[op][lv : self.arch_level[op]])
+                for lv in range(self.arch_level[op])
+            ]
+            for op in self.operand_list
+        }
+
+        """ Number of unit at each level that hold the same data (for each operand) """
+        unit_duplicate = {
+            op: [
+                prod(self.unroll_size_ir[op][lv : self.arch_level[op]])
+                for lv in range(self.arch_level[op])
+            ]
+            for op in self.operand_list
+        }
 
         self.unit_count = unit_count
         self.unit_unique = unit_unique
         self.unit_duplicate = unit_duplicate
 
     def calc_data_serve_scope(self):
         """
         Calculate data serve scope, i.e.,
         for input operands, it means that each data element is broadcast to how many unit at below level;
         for output operand, it means that how many unit add/collect their output values to one result, and push it to above level '''
 
         NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes.
         """
-        ''' data_serve_scope is calculated by dividing unit_duplicate at current level by unit_count at one level above. '''
-        data_serve_scope = {op: [
-            self.unit_duplicate[op][lv]/self.unit_duplicate[op][lv+1] for lv in range(self.arch_level[op]-1)
-        ] for op in self.operand_list}
+        """ data_serve_scope is calculated by dividing unit_duplicate at current level by unit_count at one level above. """
+        data_serve_scope = {
+            op: [
+                self.unit_duplicate[op][lv] / self.unit_duplicate[op][lv + 1]
+                for lv in range(self.arch_level[op] - 1)
+            ]
+            for op in self.operand_list
+        }
 
         self.data_serve_scope = data_serve_scope
 
     def calc_mem_bw_boost_factor(self):
         """
         Calculate memory bandwidth incremental factor between architectural levels.
 
         NOTE: mem_bw_boost doesn't include MAC level, thus is one level less than other spatial mapping attributes.
         """
-        ''' mem_bw_boost can calculated by either dividing unit_unique at current level by unit_count at one level above. '''
-        mem_bw_boost = {op: [
-            int(self.unit_unique[op][lv]/self.unit_unique[op][lv+1]) for lv in range(self.arch_level[op]-1)
-        ] for op in self.operand_list}
+        """ mem_bw_boost can calculated by either dividing unit_unique at current level by unit_count at one level above. """
+        mem_bw_boost = {
+            op: [
+                int(self.unit_unique[op][lv] / self.unit_unique[op][lv + 1])
+                for lv in range(self.arch_level[op] - 1)
+            ]
+            for op in self.operand_list
+        }
 
         self.mem_bw_boost = mem_bw_boost
 
     def save_spatial_loop_dim_size(self):
         """
         Save the loops that were unrolled spatially in a list without any arch level information for easy access in loma.
         """
         # We take one of the input operands and go through the spatial mapping dict for that operand.
         # Which operand shouldn't matter as all operands store the same loops, but possibly at different arch levels.
         op = self.layer_node.input_operands[0]
-        self.spatial_loop_dim_size = [loop for spatial_loops in self.mapping_dict_origin[op] for loop in spatial_loops]
+        self.spatial_loop_dim_size = [
+            loop
+            for spatial_loops in self.mapping_dict_origin[op]
+            for loop in spatial_loops
+        ]
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag-dse-2.3.2/zigzag/classes/mapping/temporal/temporal_mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import Dict
-from copy import deepcopy
 from math import prod
 from zigzag.classes.workload.layer_node import LayerNode
 from zigzag.utils import pickle_deepcopy
 
+
 class TemporalMapping:
     """
     Class that collect all the info related to temporal mapping.
     """
 
     def __init__(self, temporal_mapping_dict: Dict, layer_node: LayerNode):
         self.mapping_dic_origin = temporal_mapping_dict
         self.layer_node = layer_node
         self.operand_list = layer_node.operand_list
 
-        ''' Extract memory hierarchy level count for each operand from temporal mapping definition '''
+        """ Extract memory hierarchy level count for each operand from temporal mapping definition """
         self.mem_level = {op: len(tmap) for (op, tmap) in temporal_mapping_dict.items()}
 
-        ''' For each memory level, if the innermost/bottom loop is ir loop, merge it down to the below level '''
+        """ For each memory level, if the innermost/bottom loop is ir loop, merge it down to the below level """
         self.innermost_stationary_loop_merge_down()
 
-        ''' Calculate the current and below level (cabl) iteration cycle for each memory level, 
-        i.e., each memory level refreshes once, how many cycles it covers '''
+        """ Calculate the current and below level (cabl) iteration cycle for each memory level, 
+        i.e., each memory level refreshes once, how many cycles it covers """
         self.calc_cycle_cabl_level()
 
         # ''' Calculate the current and below loop (cabl) iteration cycle for each loop,
         # i.e., each loop iterates once, how many cycles it covers '''
         # self.calc_cycle_cabl_loop()
 
-        ''' Calculate the top-ir loop size at each memory level, which will be used 
-        to compute instant required memory BW in combined_mapping.py '''
+        """ Calculate the top-ir loop size at each memory level, which will be used 
+        to compute instant required memory BW in combined_mapping.py """
         self.calc_top_r_and_ir_loop()
 
     def __str__(self):
         return str(self.mapping_dic_stationary)
 
     def __repr__(self):
         return str(self)
@@ -45,38 +45,55 @@
         return {"temporal_mapping": self.mapping_dic_stationary}
 
     def innermost_stationary_loop_merge_down(self):
         """
         Iteratively merging down the ir loops which located at the bottom position of each memory level.
         Also calculate the MAC level data stationary cycle, i,e., the innermost memory level's bottom ir loops.
         """
-        ''' Initialization '''
+        """ Initialization """
         mapping_current = pickle_deepcopy(self.mapping_dic_origin)
         mapping_previous = pickle_deepcopy(self.mapping_dic_origin)
         done = False
 
         while not done:
-            mapping_st = {op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list}
+            mapping_st = {
+                op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list
+            }
             MAC_level_st = {op: 1 for op in self.operand_list}
             for operand in self.mem_level.keys():
                 for level, current_level_loops in enumerate(mapping_previous[operand]):
                     if not current_level_loops:
-                        mapping_st[operand][level] = pickle_deepcopy(current_level_loops)
+                        mapping_st[operand][level] = pickle_deepcopy(
+                            current_level_loops
+                        )
                     else:
                         for loop_type, loop_dim in current_level_loops:
-                            if loop_type in self.layer_node.operand_loop_dim[operand]['ir']:
+                            if (
+                                loop_type
+                                in self.layer_node.operand_loop_dim[operand]["ir"]
+                            ):
                                 if level == 0:
                                     MAC_level_st[operand] *= loop_dim
-                                    mapping_st[operand][level].append((loop_type, loop_dim))
-                                    mapping_current[operand][level].remove((loop_type, loop_dim))
+                                    mapping_st[operand][level].append(
+                                        (loop_type, loop_dim)
+                                    )
+                                    mapping_current[operand][level].remove(
+                                        (loop_type, loop_dim)
+                                    )
                                 else:
-                                    mapping_st[operand][level - 1].append((loop_type, loop_dim))
-                                    mapping_current[operand][level].remove((loop_type, loop_dim))
+                                    mapping_st[operand][level - 1].append(
+                                        (loop_type, loop_dim)
+                                    )
+                                    mapping_current[operand][level].remove(
+                                        (loop_type, loop_dim)
+                                    )
                             else:
-                                mapping_st[operand][level].extend(mapping_current[operand][level])
+                                mapping_st[operand][level].extend(
+                                    mapping_current[operand][level]
+                                )
                                 break
             if mapping_st != mapping_previous:
                 mapping_previous = pickle_deepcopy(mapping_st)
                 mapping_current = pickle_deepcopy(mapping_st)
                 continue
             else:
                 done = True
@@ -84,58 +101,71 @@
         self.mapping_dic_stationary = mapping_st
         self.MAC_level_data_stationary_cycle = MAC_level_st
 
     def calc_cycle_cabl_level(self):
         """
         Calculate the iteration cycles that each memory level covers
         """
-        ''' iteration_each_level only counts for the current level for-loops '''
-        iteration_each_level = {op: [
-            prod([loop_dim for (_, loop_dim) in self.mapping_dic_stationary[op][lv]]) for lv in range(self.mem_level[op])
-        ] for op in self.operand_list}
-        ''' cycle_per_level count for current and below levels' for-loops '''
-        cycle_cabl_level = {op: [
-            prod(iteration_each_level[op][0:lv+1]) for lv in range(self.mem_level[op])
-        ] for op in self.operand_list}
+        """ iteration_each_level only counts for the current level for-loops """
+        iteration_each_level = {
+            op: [
+                prod(
+                    [loop_dim for (_, loop_dim) in self.mapping_dic_stationary[op][lv]]
+                )
+                for lv in range(self.mem_level[op])
+            ]
+            for op in self.operand_list
+        }
+        """ cycle_per_level count for current and below levels' for-loops """
+        cycle_cabl_level = {
+            op: [
+                prod(iteration_each_level[op][0 : lv + 1])
+                for lv in range(self.mem_level[op])
+            ]
+            for op in self.operand_list
+        }
 
-        ''' ASSERT: The total cycle count must be the same for all operand '''
+        """ ASSERT: The total cycle count must be the same for all operand """
         total_cycle = [cycle_cabl_level[op][-1] for op in self.operand_list]
-        assert all(x == total_cycle[0] for x in total_cycle), \
-            f"The total cycle count is not the same for all operand {total_cycle}, please correct the temporal mapping."
+        assert all(
+            x == total_cycle[0] for x in total_cycle
+        ), f"The total cycle count is not the same for all operand {total_cycle}, please correct the temporal mapping."
 
         self.cycle_cabl_level = cycle_cabl_level
         self.total_cycle = total_cycle[0]
 
     def calc_top_r_and_ir_loop(self):
         """
         top_ir_loop_size: For each memory level, from top to bottom, the product of top few irrelevant loops.
         top_ir is used for later required instant memory bandwidth calculation.
         """
-        ''' Initialization '''
-        ''' self.mem_level[op] + 1 to add the placeholder for operational array level '''
-        top_r_loop_size = {op: [
-            1 for _ in range(self.mem_level[op] + 1)
-        ] for op in self.operand_list}
-
-        top_ir_loop_size = {op: [
-            1 for _ in range(self.mem_level[op] + 1)
-        ] for op in self.operand_list}
+        """ Initialization """
+        """ self.mem_level[op] + 1 to add the placeholder for operational array level """
+        top_r_loop_size = {
+            op: [1 for _ in range(self.mem_level[op] + 1)] for op in self.operand_list
+        }
+
+        top_ir_loop_size = {
+            op: [1 for _ in range(self.mem_level[op] + 1)] for op in self.operand_list
+        }
 
-        ''' Check and extract the top ir loops '''
+        """ Check and extract the top ir loops """
         for operand in self.operand_list:
-            for level, current_level_loops in enumerate(self.mapping_dic_stationary[operand]):
+            for level, current_level_loops in enumerate(
+                self.mapping_dic_stationary[operand]
+            ):
                 if not current_level_loops:
                     continue
                 else:
                     for loop_type, loop_dim in reversed(current_level_loops):
-                        if loop_type in self.layer_node.operand_loop_dim[operand]['r']:
+                        if loop_type in self.layer_node.operand_loop_dim[operand]["r"]:
                             top_r_loop_size[operand][level + 1] *= loop_dim
                         else:
                             break
                     for loop_type, loop_dim in reversed(current_level_loops):
-                        if loop_type in self.layer_node.operand_loop_dim[operand]['ir']:
+                        if loop_type in self.layer_node.operand_loop_dim[operand]["ir"]:
                             top_ir_loop_size[operand][level + 1] *= loop_dim
                         else:
                             break
 
         self.top_r_loop_size = top_r_loop_size
         self.top_ir_loop_size = top_ir_loop_size
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/spatial/generator.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/spatial/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from zigzag.classes.hardware.architecture.core import Core
 from zigzag.classes.hardware.architecture.dimension import Dimension
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 from zigzag.classes.hardware.architecture.operational_array import OperationalArray
 
 
 class UserSpatialMappingGenerator:
-    """Class that generates valid user-format spatial mappings.
-    """
+    """Class that generates valid user-format spatial mappings."""
+
     def __init__(self, layer, accelerator) -> None:
         self.layer = layer
         self.accelerator = accelerator
 
     def run(self):
         return self.generate_user_spatial_mappings()
 
@@ -39,42 +39,59 @@
         operational_array: OperationalArray = core.operational_array
         oa_dims = operational_array.dimensions
         memory_hierarchy: MemoryHierarchy = core.memory_hierarchy
         innermost_levels = memory_hierarchy.get_inner_memories()
 
         # For every operational array dimension, we initialize it by maximally unrolling all layer dimensions.
         # Later these will be restricted if the memory structure doesn't allow for this unrolling
-        oa_dim_unrolling = {oa_dim: {layer_dim: int(min(layer_size, oa_dim.size)) for layer_dim, layer_size in
-                                     self.layer.loop_dim_size.items()} for oa_dim in oa_dims}
+        oa_dim_unrolling = {
+            oa_dim: {
+                layer_dim: int(min(layer_size, oa_dim.size))
+                for layer_dim, layer_size in self.layer.loop_dim_size.items()
+            }
+            for oa_dim in oa_dims
+        }
 
         for memory_level in innermost_levels:
             served_dimensions: Set[Dimension] = memory_level.served_dimensions
             mem_ops = memory_level.operands
             for mem_op in mem_ops:
-                layer_op = self.layer.get_layer_operand(mem_op=mem_op)  # get the layer operand
-                if layer_op == 'O':
-                    mem_bandwidth = memory_level.write_bw  # partial outputs are written to the memory
+                layer_op = self.layer.get_layer_operand(
+                    mem_op=mem_op
+                )  # get the layer operand
+                if layer_op == "O":
+                    mem_bandwidth = (
+                        memory_level.write_bw
+                    )  # partial outputs are written to the memory
                 else:
-                    mem_bandwidth = memory_level.read_bw  # inputs are read from the memory
-                precision = self.layer.operand_precision[layer_op]  # bit precision of layer operand
-                irrelevant_dimensions = self.layer.get_operand_irrelevant_dimensions(layer_op)
+                    mem_bandwidth = (
+                        memory_level.read_bw
+                    )  # inputs are read from the memory
+                precision = self.layer.operand_precision[
+                    layer_op
+                ]  # bit precision of layer operand
+                irrelevant_dimensions = self.layer.get_operand_irrelevant_dimensions(
+                    layer_op
+                )
                 for oa_dim in oa_dims:
                     if oa_dim not in served_dimensions:
                         continue
                     # If the operational array dimension is a served dimension of the lowest memory level,
                     # we ought to limit the unrolling for the relevant and partially relevant loop dimensions
                     for (layer_dim, unrolling_size) in oa_dim_unrolling[oa_dim].items():
                         if layer_dim in irrelevant_dimensions:
                             continue
                         # If not irrelevant, it is (partially) relevant. Limit based on BW and operand precision.
                         try:
                             max_multicast_elements = mem_bandwidth // precision
                         except ZeroDivisionError:
                             max_multicast_elements = unrolling_size
-                        oa_dim_unrolling[oa_dim][layer_dim] = min(max_multicast_elements, unrolling_size)
+                        oa_dim_unrolling[oa_dim][layer_dim] = min(
+                            max_multicast_elements, unrolling_size
+                        )
 
         # At this point the unrolled layer dimensions are maximal (wrt the served dimensions and bandwidth of the lowest memory level).
         # The unrolling size might not be a factor of the layer dimension size, which is required (for non greedy mapping).
         # Convert the unrolling size to be a factor of the layer dimension size. At the same time convert them to a list.
         unrollings = []
         for oa_dim in oa_dims:
             oa_dim_unrollings = []
@@ -101,13 +118,17 @@
             unrollings.append(oa_dim_unrollings)
 
         # Now we have for each operational array dimension the layer dimensions and size they can be unrolled without fractional remainder.
         # Now we have to combine them into user-defined spatial mappings.
         for combination in itertools.product(*unrollings):
             # Zip the combination (which is a (layer_dim, layer_size) for each oa_dim with the oa_dim names.
             oa_dim_names = [oa_dim.name for oa_dim in oa_dims]
-            user_spatial_mapping = {oa_dim_name: unrolling for (oa_dim_name, unrolling) in zip(oa_dim_names, combination) if unrolling is not None}
+            user_spatial_mapping = {
+                oa_dim_name: unrolling
+                for (oa_dim_name, unrolling) in zip(oa_dim_names, combination)
+                if unrolling is not None
+            }
             yield user_spatial_mapping
 
     @staticmethod
     def all_unique(items):
-        return len(set(items)) == len(items)
+        return len(set(items)) == len(items)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-"""
-This file contains the core code of the temporal mapping optimization method
-called loma: loop order based memory allocation.
-
-TODO: Get a layers' dimensions to generate the multiset permutations for all loop types
-TODO: Write generator that takes loop-type-specific multiset permutations and generates loop order permutation
-TODO: Write uneven memory allocator, that allocates the loops of the loop order bottom-up to the memories in the hierarchy
-TODO: (optional) Write even memory allocator
-TODO: Once we have allocated the loops to the different hierarchy levels, call the cost model to get energy, latency
-TODO: Save the best found loop order (and its associated allocated mapping)
-"""
 from math import factorial
 import operator
 from tqdm import tqdm
-
 import numpy as np
 from sympy.ntheory import factorint
 import logging
 
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
-from zigzag.classes.workload.layer_node import LayerNode
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 from zigzag.classes.opt.temporal.loma.multipermute import permutations
-from zigzag.classes.opt.temporal.loma.memory_allocator import MemoryHierarchyTooSmallException, MemoryTooSmallException, MemoryAllocator
+from zigzag.classes.opt.temporal.loma.memory_allocator import (
+    MemoryHierarchyTooSmallException,
+    MemoryTooSmallException,
+    MemoryAllocator,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class NoValidLoopOrderingFoundException(Exception):
     pass
 
@@ -40,15 +28,17 @@
     - a memory hierarchy
     This optimization is carried out through loop order based memory allocation.
     For each ordering of the temporal loops, they are allocated bottom-up to the
     levels in the memory hierarchy.
     See https://ieeexplore.ieee.org/document/9458493 for more details.
     """
 
-    def __init__(self, *, accelerator, layer, spatial_mapping, loma_lpf_limit=np.inf,  **kwargs):
+    def __init__(
+        self, *, accelerator, layer, spatial_mapping, loma_lpf_limit=np.inf, **kwargs
+    ):
         """
         Initialize the engine with the given:
         - Accelerator
         - LayerNode
         - SpatialMapping
 
         The memory hierarchy from the correct core is extracted from the accelerator.
@@ -65,80 +55,94 @@
         self.spatial_mapping = spatial_mapping
 
         # Extract the memory hierarchy from the accelerator
         # TODO: Take into account that data might be stored in lower level,
         # TODO: thus adapt the memory hierarchy.
         # TODO: The fact that there is a global buffer above the cores requires attention.
         core_id = layer.core_allocation
-        self.memory_hierarchy: MemoryHierarchy = accelerator.get_core(core_id).memory_hierarchy
+        self.memory_hierarchy: MemoryHierarchy = accelerator.get_core(
+            core_id
+        ).memory_hierarchy
 
         self.show_progress_bar = kwargs.get("loma_show_progress_bar", False)
 
-
     def run(self):
         """
         :returns : Generator that yields all temporal mappings
         TODO: add the criterion(s) as inputs to this function.
         """
-        logger.info('Running temporal mapping search engine...')
+        logger.info("Running temporal mapping search engine...")
 
         self.get_temporal_loops()  # get all the temporal loops
         self.get_prime_factors()  # convert these to LPFs (loop prime factors)
 
         if self.show_progress_bar:
             pbar = tqdm(total=self.nb_permutations)
         else:
             pbar = None
 
         yielded = False
         for ordering in self.og():  # ordering generator
-            allocator = MemoryAllocator(self.accelerator, self.layer, self.spatial_mapping, ordering)
+            allocator = MemoryAllocator(
+                self.accelerator, self.layer, self.spatial_mapping, ordering
+            )
             # using try catch here because in the depth-first mode the highest level might not be big enough
             try:
-                temporal_mapping = allocator.run()  # allocate this ordering to the memories
+                temporal_mapping = (
+                    allocator.run()
+                )  # allocate this ordering to the memories
                 yielded = True
                 yield temporal_mapping
             except MemoryHierarchyTooSmallException:
                 pass
             except MemoryTooSmallException:
                 pass  # Skip the ordering that crashed due to ordering (+su) not fitting in memory
             if self.show_progress_bar:
                 pbar.update(1)
 
         if self.show_progress_bar:
             pbar.close()
 
         if not yielded:
-            raise NoValidLoopOrderingFoundException(f"No valid loop ordering was found for layer {self.layer}. Please make sure the spatial mapping is compatible with the architecture.")
-
+            raise NoValidLoopOrderingFoundException(
+                f"No valid loop ordering was found for layer {self.layer}. Please make sure the spatial mapping is compatible with the architecture."
+            )
 
     def get_temporal_loops(self):
         """
         Get all loops that have to be temporally scheduled given layer and spatial mapping.
         """
-        temporal_loop_dim_size = self.layer.loop_dim_size.copy()  # init with all loop sizes
+        temporal_loop_dim_size = (
+            self.layer.loop_dim_size.copy()
+        )  # init with all loop sizes
         for spatial_loop in self.spatial_mapping.spatial_loop_dim_size:
             (spatial_loop_dim, spatial_loop_size) = spatial_loop
             # Allow greedy mapping. If the spatial unrolling is not a multiple of the layer dimension size,
             # we take the ceil of the division, so there can be one extra temporal iteration.
-            q = int(np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size))
+            q = int(
+                np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size)
+            )
             # q, rem = divmod(temporal_loop_dim_size[spatial_loop_dim], spatial_loop_size)
             # assert rem == 0, "Division of dimension size by spatial unrolling size is not an integer"
             if q == 1:
                 del temporal_loop_dim_size[spatial_loop_dim]
             else:
                 temporal_loop_dim_size[spatial_loop_dim] = q
 
         # Remove all dimensions with a temporal loop size of 1
-        temporal_loop_dim_size_no_1s = {key: val for (key, val) in temporal_loop_dim_size.items() if val > 1}
+        temporal_loop_dim_size_no_1s = {
+            key: val for (key, val) in temporal_loop_dim_size.items() if val > 1
+        }
 
         self.temporal_loop_dim_size = temporal_loop_dim_size_no_1s
         min_nb_temporal_loops = len(self.temporal_loop_dim_size)
         if self.lpf_limit < min_nb_temporal_loops:
-            logger.debug(f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs.")
+            logger.debug(
+                f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs."
+            )
             self.lpf_limit = min_nb_temporal_loops
 
     def get_prime_factors(self):
         """
         Get the prime factors for all temporal loops.
 
         This is saved in three separate class attributes:
@@ -146,15 +150,18 @@
         temporal_loop_pf_counts: a dict that for each temporal loop dimension contains the prime factor multiplicities
         temporal_loop_pf_count_sums: a dict that for each temporal loop dimension contains the total amount of prime factors
         """
         temporal_loop_pfs = {}
         temporal_loop_pf_counts = {}
         temporal_loop_pf_count_sums = {}
         lpfs = []
-        for (tl_dim, tl_size) in self.temporal_loop_dim_size.items():  # tl = temporal loop
+        for (
+            tl_dim,
+            tl_size,
+        ) in self.temporal_loop_dim_size.items():  # tl = temporal loop
             factors = factorint(tl_size)
             pfs = []
             counts = []
             for pf, multiplicity in factors.items():
                 pfs.append(pf)
                 counts.append(multiplicity)
                 for i in range(multiplicity):
@@ -182,38 +189,40 @@
         # Limit the number of lpfs (if this is set in the settings)
         self.limit_lpfs()
 
         # Compute how many total permuatations we will have to consider
         self.compute_nb_permutations()
 
     def compute_nb_permutations(self):
-        """Compute the number of permutations that will have to be considered given the LPF distribution.
-        """
+        """Compute the number of permutations that will have to be considered given the LPF distribution."""
         nb_permutations = factorial(sum(self.temporal_loop_pf_count_sums.values()))
         for nb_duplicated_pfs in self.temporal_loop_pf_counts.values():
             for nb_duplicated_pf in nb_duplicated_pfs:
                 nb_permutations = int(nb_permutations / factorial(nb_duplicated_pf))
         self.nb_permutations = nb_permutations
-        logger.debug(f"Launching {self.nb_permutations:,} temporal loop order permutations.")
-        
+        logger.debug(
+            f"Launching {self.nb_permutations:,} temporal loop order permutations."
+        )
 
     def limit_lpfs(self):
         """
         Function to limit the total number of loop prime factors present in this instance.
         This function scans the lpfs and while the number of lpfs is greater than self.lpf_limit it:
         - picks the loop dimension that has the most lpfs
         - merges the smallest two lpfs of that loop dimension (multiplying their values)
         """
         n_pf = sum(self.temporal_loop_pf_count_sums.values())
         if n_pf <= self.lpf_limit:
             logger.debug(f"No lpf limiting performed for layer {self.layer}")
             return
         while n_pf > self.lpf_limit:
             # Find the loop dimension with the most lpfs
-            max_ld = max(self.temporal_loop_pf_count_sums.items(), key=operator.itemgetter(1))[0]
+            max_ld = max(
+                self.temporal_loop_pf_count_sums.items(), key=operator.itemgetter(1)
+            )[0]
             # Get the prime factors of this loop dimension
             max_pfs = list(self.temporal_loop_pfs[max_ld])
             # Get the multiplicity of these prime factors
             max_counts = list(self.temporal_loop_pf_counts[max_ld])
 
             if max_counts[0] == 1:  # multiplicity of smallest pf is 1
                 new_factor = max_pfs[0] * max_pfs[1]
@@ -225,15 +234,17 @@
 
             if new_factor in max_pfs:  # possible if not first iteration of while loop
                 new_factor_idx = max_pfs.index(new_factor)
                 max_counts[new_factor_idx] += 1
             else:  # the new factor is not yet present in the factors, insert so list remains sorted
                 new_factor_idx = len([pf for pf in max_pfs if pf < new_factor])
                 max_pfs.insert(new_factor_idx, new_factor)
-                max_counts.insert(new_factor_idx, 1)  # first time this factor occured, count = 1
+                max_counts.insert(
+                    new_factor_idx, 1
+                )  # first time this factor occured, count = 1
 
             # Sanitize max_pfs and max_counts to remove all elements with multiplicity 0
             non_zero_idxs = [idx for idx, count in enumerate(max_counts) if count != 0]
             max_pfs = [max_pfs[non_zero_idx] for non_zero_idx in non_zero_idxs]
             max_counts = [max_counts[non_zero_idx] for non_zero_idx in non_zero_idxs]
 
             # Update the appropriate variables with these new factors and multiplicities
@@ -243,15 +254,17 @@
 
             # Decrease the total number of factors by 1
             n_pf -= 1
 
         # Update self.lpfs for these new factors
         lpfs = []
         for dim in self.temporal_loop_pfs.keys():
-            for (pf, count) in zip(self.temporal_loop_pfs[dim], self.temporal_loop_pf_counts[dim]):
+            for (pf, count) in zip(
+                self.temporal_loop_pfs[dim], self.temporal_loop_pf_counts[dim]
+            ):
                 lpfs += list(((dim, pf),) * count)
         self.lpfs = lpfs
 
         logger.debug(f"Limited layer {self.layer} to {len(self.lpfs)} lpfs.")
         return
 
     def og(self):
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/memory_allocator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import List
 import numpy as np
+from math import prod
+
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 from zigzag.classes.hardware.architecture.memory_level import MemoryLevel
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
 from zigzag.classes.opt.temporal.loma.loop import Loop
-from zigzag.classes.workload.layer_node import LayerNode
-from math import prod
+
 
 class MemoryHierarchyTooSmallException(Exception):
     pass
 
+
 class MemoryTooSmallException(Exception):
     pass
 
+
 class MemoryAllocator:
     """
     Class that handles allocation of a loop ordering to the memories in the hierarchy.
     """
 
     def __init__(self, accelerator, layer, spatial_mapping, ordering: List):
         """
@@ -35,56 +37,75 @@
         self.spatial_mapping = spatial_mapping
         self.ordering = ordering
 
         # Initialize the different operands
         # On the HW side, these are always called 'I1' 'I2' and 'O',
         # but on the layer side, they can be anything.
         layer_ops = self.layer.operand_list
-        self.mem_ops = [self.layer.memory_operand_links[layer_op] for layer_op in layer_ops]
+        self.mem_ops = [
+            self.layer.memory_operand_links[layer_op] for layer_op in layer_ops
+        ]
         # Translation dict from layer op to mem op
         self.layer_to_mem_op = self.layer.memory_operand_links.copy()
         # Translation dict from mem op to layer op
-        self.mem_to_layer_op = {mem_op: layer_op for (layer_op, mem_op) in self.layer_to_mem_op.items()}
+        self.mem_to_layer_op = {
+            mem_op: layer_op for (layer_op, mem_op) in self.layer_to_mem_op.items()
+        }
         # Bit precision for the different mem ops
-        self.precision = {mem_op: self.layer.operand_precision[layer_op] for (layer_op, mem_op) in self.layer_to_mem_op.items()}
-        self.precision["O_final"] = self.layer.operand_precision.get("O_final", self.precision['O'])  # Final output precision
+        self.precision = {
+            mem_op: self.layer.operand_precision[layer_op]
+            for (layer_op, mem_op) in self.layer_to_mem_op.items()
+        }
+        self.precision["O_final"] = self.layer.operand_precision.get(
+            "O_final", self.precision["O"]
+        )  # Final output precision
         # Initialize the unallocated loops with the ordering for each operand
         self.unallocated = {}
         for mem_op in self.mem_ops:
-            self.unallocated[mem_op] = [Loop(dim, size) for (dim, size) in self.ordering]
+            self.unallocated[mem_op] = [
+                Loop(dim, size) for (dim, size) in self.ordering
+            ]
 
         # Initialize the allocated loops with the spatial mapping at the operand level for each operand
         self.allocated = {}
         for (layer_op, mem_op) in self.layer_to_mem_op.items():
-            self.allocated[mem_op] = [Loop(dim, size, "spatial") for (dim, size) in
-                                      self.spatial_mapping.get_unrolling(op=layer_op, level=0)]
+            self.allocated[mem_op] = [
+                Loop(dim, size, "spatial")
+                for (dim, size) in self.spatial_mapping.get_unrolling(
+                    op=layer_op, level=0
+                )
+            ]
 
         # Initialize the level of memory hierarchy for each layer operand at 1 (first memory level).
         # This information is required to fetch the correct spatial loops after we have allocated temporal loops.
         self.mem_level = {layer_op: 1 for layer_op in layer_ops}
 
         # Initialize the temporal mapping dict, which is appended to throughout the allocation process.
         # It is a dictionary with keys the different layer operands and values a list of lists.
         # The sublists represent the memory levels for that operand and contain the loops allocated to that level.
         self.temporal_mapping_dict = {layer_op: [] for layer_op in layer_ops}
 
-
     def run(self):
         """
         Run the memory allocation process.
 
         Start by the lowest memory hierarchy level and allocate as much loops as possible
         for the different operands. The spatial unrolling has to be taken into account at
         each memory level in the hierarchy.
         """
 
         # self.nodes contains the different memory nodes in bottom-up fashion
         core_id = self.layer.core_allocation
-        memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(core_id).memory_hierarchy
-        top_levels = {mem_op: memory_hierarchy.get_operand_top_level(mem_op) for mem_op in self.mem_ops}
+        memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(
+            core_id
+        ).memory_hierarchy
+        top_levels = {
+            mem_op: memory_hierarchy.get_operand_top_level(mem_op)
+            for mem_op in self.mem_ops
+        }
         nodes = memory_hierarchy.nodes
         for node in nodes:
             self.allocate_node(node, top_levels)
 
         # After all the nodes have been allocated, we can creat the TemporalMapping
         # object from the dictionary we have built
         temporal_mapping = TemporalMapping(self.temporal_mapping_dict, self.layer)
@@ -110,43 +131,53 @@
         all_sizes = {}
         for mem_op in mem_ops:
             sizes = self.calc_size_slices(mem_op, mem_capacity)
             all_sizes[mem_op] = sizes
 
         # Now that we have this for all the mem_ops, call function that finds the best
         # combination of loops to minimize the number of accesses to the level above
-        best_loop_idxs = self.find_best_loop_combination(mem_ops, all_sizes, node, top_levels)
+        best_loop_idxs = self.find_best_loop_combination(
+            mem_ops, all_sizes, node, top_levels
+        )
 
         for (best_loop_idx, mem_op) in zip(best_loop_idxs, mem_ops):
             # Now that we have the combination of loop_idx for each mem_op, add them
             # to the allocated loops and remove them from the unallocated loops
             loops_to_allocate = self.unallocated[mem_op][:best_loop_idx].copy()
             self.allocated[mem_op] += loops_to_allocate
             del self.unallocated[mem_op][:best_loop_idx]
 
             # Add the loops to allocate to the level-by-level temporal_mapping_dict
             # The key of this dict is the layer_op and not the mem_op
             layer_op = self.mem_to_layer_op[mem_op]
-            self.temporal_mapping_dict[layer_op].append([(loop.dimension, loop.size) for loop in loops_to_allocate])
+            self.temporal_mapping_dict[layer_op].append(
+                [(loop.dimension, loop.size) for loop in loops_to_allocate]
+            )
 
             # This memory node that stores one or more mem_ops might be
             # spatially unrolled, add these spatially unrolled loops to
             # the list of allocated loops now, so that the next memory nodes
             # correctly see this spatial unrolling.
             # For this we require the level of memory we are evaluating for this op.
             mem_level_op = self.mem_level[layer_op]
-            spatial_loops = self.spatial_mapping.get_unrolling(op=layer_op, level=mem_level_op)
+            spatial_loops = self.spatial_mapping.get_unrolling(
+                op=layer_op, level=mem_level_op
+            )
             for (loop_dim, loop_size) in spatial_loops:
                 spatial_loop = Loop(dimension=loop_dim, size=loop_size, type="spatial")
                 self.allocated[mem_op].append(spatial_loop)
 
             # Check if this node (i.e. MemoryLevel) is the highest level of memory hierarchy.
             # If this is the case and we haven't allocated all loops, raise an exception.
-            if node == top_levels[mem_op] and self.unallocated[mem_op]:  # if top level and unallocated not empty
-                raise MemoryHierarchyTooSmallException(f"Highest MemoryLevel for {mem_op} = {node} too small to store all loops.")
+            if (
+                node == top_levels[mem_op] and self.unallocated[mem_op]
+            ):  # if top level and unallocated not empty
+                raise MemoryHierarchyTooSmallException(
+                    f"Highest MemoryLevel for {mem_op} = {node} too small to store all loops."
+                )
 
             # Increment the mem_level we are currently at for this layer_op by 1
             self.mem_level[layer_op] += 1
 
     def calc_size_slices(self, mem_op: str, mem_capacity: int):
         """
         Calculate the required memory size to store different
@@ -156,23 +187,31 @@
         # Already allocated loops for this mem_op
         allocated_loops = self.allocated[mem_op]
 
         # Unallocated loops for this mem_op
         unallocated_loops = self.unallocated[mem_op]
         sizes = []
 
-        for i in range(len(unallocated_loops) + 1):  # Go through all slices (includes empty slice)
-            unallocated_slice = unallocated_loops[:i]  # Grab a slice of the unallocated loops
-            loops = allocated_loops + unallocated_slice  # Join them with already allocated loops
+        for i in range(
+            len(unallocated_loops) + 1
+        ):  # Go through all slices (includes empty slice)
+            unallocated_slice = unallocated_loops[
+                :i
+            ]  # Grab a slice of the unallocated loops
+            loops = (
+                allocated_loops + unallocated_slice
+            )  # Join them with already allocated loops
             size = self.calc_loops_size(loops, mem_op, unallocated_loops)
             if size <= mem_capacity:
                 sizes.append(size)
             else:
                 if i == 0:  # This means we can't even store the already allocated loops
-                    raise MemoryTooSmallException(f"Memory capacity overflow for mem_op {mem_op}. loops={loops} size={size} mem_capacity={mem_capacity}")
+                    raise MemoryTooSmallException(
+                        f"Memory capacity overflow for mem_op {mem_op}. loops={loops} size={size} mem_capacity={mem_capacity}"
+                    )
                 break  # Stop as soon as we have added a loop that overflows the memory
         return sizes
 
     def calc_loops_size(self, loops: List, mem_op: str, all_unallocated_loops: List):
         """
         Calculate the 'mem_op' tensor size required for all the loops in 'loops'.
         :param loops: The loops we want to calculate the size for.
@@ -190,20 +229,22 @@
         layer_op = self.mem_to_layer_op[mem_op]
         tensor_size = self.layer.calc_tensor_size(layer_op, all_dim_sizes)
 
         # Get the precision at which this tensor will have to be stored in the MemoryLevel node.
         # For output it can be either the partial sum precision, or the final sum precision.
         # This depends on if all the irrelevant loops were allocated in a previous MemoryLevel.
         # Which in turn means all remaining unallocated loops for this MemoryLevel must not contain any ir loops.
-        if mem_op == 'O':
-            ir_dims = op_dimensions['ir']  # Irrelevant dimensions
-            unallocated_dims = [unallocated_loop.dimension for unallocated_loop in all_unallocated_loops]
+        if mem_op == "O":
+            ir_dims = op_dimensions["ir"]  # Irrelevant dimensions
+            unallocated_dims = [
+                unallocated_loop.dimension for unallocated_loop in all_unallocated_loops
+            ]
             # If there is still an irrelevant unallocated loop dimension, pick the full precision
             if any([dim in ir_dims for dim in unallocated_dims]):
-                precision = self.precision['O']
+                precision = self.precision["O"]
             else:
                 precision = self.precision["O_final"]
         else:
             precision = self.precision[mem_op]
 
         tensor_size_bits = tensor_size * precision
 
@@ -214,39 +255,45 @@
         Find the best combination of loops from different mem_ops.
         Best is defined as the combination that minimizes the number of accesses
         to the memory level above.
         :param TODO
         TODO: Take into account the operand precision which can change based on the loops picked
         """
         mem_capacity = node.memory_instance.size
-        
+
         # nb_operations = self.__main_inputs.layer.total_MAC_count
         # all_accesses = {mem_op: [nb_operations//size for size in all_sizes[mem_op]] for mem_op in mem_ops}
 
         # If for one of the mem_ops this is the top level memory, we have to enforce that all unallocated loops
         # will be allocated for this operand. We do this by changing the sizes for this mem_op to only include
         # the last number (which represents the size to store all the ops).
         # Because we modify the sizes, we add an offset to the loop_idx for this mem_op.
         loop_idx_offsets = {mem_op: 0 for mem_op in mem_ops}
         for mem_op, sizes in all_sizes.items():
             if node == top_levels[mem_op]:
-                loop_idx_offsets[mem_op] = len(sizes) - 1  # offset is number of original sizes - 1
+                loop_idx_offsets[mem_op] = (
+                    len(sizes) - 1
+                )  # offset is number of original sizes - 1
                 all_sizes[mem_op] = [sizes[-1]]
-        
+
         all_accesses = {mem_op: [] for mem_op in mem_ops}
         for mem_op in mem_ops:
             # The number of accesses to the level above is determined through the reuse we have for the different
             # choices of temporal loops. accesses = # total temporal loop iterations / temporal reuse
             # The temporal reuse = # allocated loop iterations / operand size
             # Thus: accesses = # total iterations / (# allocated iterations / size)
             # Thus: accesses = (# total iterations / # allocated iterations) * size
             # Thus: accesses = # unallocated iterations * size
             for i, size in enumerate(all_sizes[mem_op]):
-                unallocated_loops = self.unallocated[mem_op][(i + loop_idx_offsets[mem_op]):]  # slice of unallocated loops for this operand size
-                unallocated_iterations = prod((unallocated_loop.size for unallocated_loop in unallocated_loops))
+                unallocated_loops = self.unallocated[mem_op][
+                    (i + loop_idx_offsets[mem_op]) :
+                ]  # slice of unallocated loops for this operand size
+                unallocated_iterations = prod(
+                    (unallocated_loop.size for unallocated_loop in unallocated_loops)
+                )
                 if node == top_levels[mem_op]:
                     accesses = 0
                 else:
                     accesses = unallocated_iterations * size
                 all_accesses[mem_op].append(accesses)
 
         all_max_nb_loops = {mem_op: len(all_sizes[mem_op]) for mem_op in mem_ops}
@@ -256,19 +303,23 @@
         nb_combinations = prod(len(sizes) for sizes in all_sizes.values())
         for i in range(nb_combinations):
             size_comb = 0
             accesses_comb = 0
             current_loop_idxs = []
             for mem_op_idx, mem_op in enumerate(mem_ops):
                 this_max_nb_loops = all_max_nb_loops_list[mem_op_idx]
-                current_loop_idx = (i // prod(all_max_nb_loops_list[mem_op_idx+1:])) % this_max_nb_loops
+                current_loop_idx = (
+                    i // prod(all_max_nb_loops_list[mem_op_idx + 1 :])
+                ) % this_max_nb_loops
                 current_loop_idxs.append(current_loop_idx + loop_idx_offsets[mem_op])
                 size_comb += all_sizes[mem_op][current_loop_idx]
                 accesses_comb += all_accesses[mem_op][current_loop_idx]
             if size_comb > mem_capacity:
                 if i == 0:
-                    raise MemoryTooSmallException("The memory can't store all loops assigned to lower level memories. Likely due to spatial unrolling.")
+                    raise MemoryTooSmallException(
+                        "The memory can't store all loops assigned to lower level memories. Likely due to spatial unrolling."
+                    )
                 continue
             if accesses_comb <= best_accesses:
                 best_accesses = accesses_comb
                 best_loop_idxs = current_loop_idxs
-        return best_loop_idxs
+        return best_loop_idxs
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/temporal/loma/multipermute.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/temporal/loma/multipermute.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,42 +31,47 @@
     h←t
     visit(h)
 end while
 ... from "Loopless Generation of Multiset Permutations using a Constant Number
 of Variables by Prefix Shifts."  Aaron Williams, 2009
 """
 
+
 class ListElement:
     def __init__(self, value, next):
         self.value = value
         self.next = next
+
     def nth(self, n):
         o = self
         i = 0
         while i < n and o.next is not None:
             o = o.next
             i += 1
         return o
 
+
 def init(multiset):
-    multiset.sort() # ensures proper non-increasing order
+    multiset.sort()  # ensures proper non-increasing order
     h = ListElement(multiset[0], None)
     for item in multiset[1:]:
         h = ListElement(item, h)
     return h, h.nth(len(multiset) - 2), h.nth(len(multiset) - 1)
 
+
 def visit(h):
     """Converts our bespoke linked list to a python list."""
     o = h
     l = []
     while o is not None:
         l.append(o.value)
         o = o.next
     return l
 
+
 def permutations(multiset):
     """Generator providing all multiset permutations of a multiset."""
     h, i, j = init(multiset)
     yield visit(h)
     while j.next is not None or j.value < h.value:
         if j.next is not None and i.value >= j.next.value:
             s = j
@@ -77,14 +82,32 @@
         t.next = h
         if t.value < h.value:
             i = t
         j = i.next
         h = t
         yield visit(h)
 
+
 if __name__ == "__main__":
-    multiset = [('OX', 2), ('OX', 2), ('OX', 3), ('OY', 2), ('K', 2), ('K', 2), ('K', 2), ('K', 3), ('K', 3), ('K', 3), ('K', 3), ('C', 2), ('C', 2), ('C', 2), ('C', 2), ('C', 2)]
+    multiset = [
+        ("OX", 2),
+        ("OX", 2),
+        ("OX", 3),
+        ("OY", 2),
+        ("K", 2),
+        ("K", 2),
+        ("K", 2),
+        ("K", 3),
+        ("K", 3),
+        ("K", 3),
+        ("K", 3),
+        ("C", 2),
+        ("C", 2),
+        ("C", 2),
+        ("C", 2),
+        ("C", 2),
+    ]
     i = 0
     for ordering in permutations(multiset):
         # print(ordering)
         i += 1
-    print(i)
+    print(i)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/temporal/salsa/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #   =====================================================================
 #   Title:        engine.py
-#   Description: This file contains the engine class that handles the 
+#   Description: This file contains the engine class that handles the
 #   optimization of temporal mapping of SALSA.
-#  
+#
 #   Date:        02.01.2023
-#  
+#
 #   =====================================================================
-# 
+#
 #   Copyright (C) 2020 ETH Zurich and University of Bologna.
-#  
+#
 #   Author: Victor Jung, ETH Zurich
-#  
+#
 #   SPDX-License-Identifier: Apache-2.0
-#  
+#
 #   Licensed under the Apache License, Version 2.0 (the License); you may
 #   not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
-#  
+#
 #   www.apache.org/licenses/LICENSE-2.0
-#  
+#
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-#  
+#
 
 from copy import deepcopy
 from sympy.ntheory import factorint
 import numpy as np
 import logging
 import random
 
@@ -52,140 +52,177 @@
     - number of iterations
     - start temperature
     This optimization is carried out through simulated annealing loop order based.
     Each loop is broken down to the smallest possible part (prime factors), then a runtime
     estimation is performed to choose the fastest engine to use (LOMA or SALSA).
     """
 
-    def __init__(self, *, accelerator: Accelerator, layer: LayerNode, spatial_mapping: SpatialMapping, **kwargs):
-    
-    #iteration_number, start_temperature, opt_criterion_name
+    def __init__(
+        self,
+        *,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMapping,
+        **kwargs,
+    ):
+
+        # iteration_number, start_temperature, opt_criterion_name
         """
         Initialize the engine with the given:
         - LayerNode
         - SpatialMapping
         - Accelerator
         - Number of iterations
         - Start temperature
         The memory hierarchy from the correct core is extracted from the accelerator.
         """
         # Hardware and mapping related inputs
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
-        #self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(layer.core_allocation).memory_hierarchy
+        # self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(layer.core_allocation).memory_hierarchy
 
         # Algorithm related inputs
         self.iteration_number = kwargs.get("salsa_iteration_number", 1000)
         self.start_temperature = kwargs.get("salsa_start_temperature", 0.05)
         self.opt_criterion_name = kwargs.get("salsa_opt_criterion", "energy")
         self.lpf_limit = kwargs.get("loma_lpf_limit", 4)
 
-
     def run(self, cme_queue):
         """
         Call the necessary methods, start the processes and collect the best temporal mapping found during the run.
         """
-        self.cme_queue = cme_queue  
+        self.cme_queue = cme_queue
         self.get_temporal_loops()
         self.get_prime_factors()
         self.run_simulated_annealing_opt(self.cme_queue)
-    
 
     def run_simulated_annealing_opt(self, cme_queue):
         """
         Run a simulated annealing optimiation on the loop ordering using a loma memory allocation strategy.
         """
         temperature = self.start_temperature
-        start_ordering = self.temporal_mapping_lpf # tmo stands for temporal mapping ordering
+        start_ordering = (
+            self.temporal_mapping_lpf
+        )  # tmo stands for temporal mapping ordering
 
         # Initialize the algorithm with a random starting point
         random.shuffle(start_ordering)
 
         # Initialize variables to store current, next and best state
-        best_state = SalsaState(self.accelerator, self.layer, self.spatial_mapping, start_ordering, self.opt_criterion_name)
-        current_state = SalsaState(self.accelerator, self.layer, self.spatial_mapping, start_ordering, self.opt_criterion_name)
-        next_state = SalsaState(self.accelerator, self.layer, self.spatial_mapping, start_ordering, self.opt_criterion_name)
+        best_state = SalsaState(
+            self.accelerator,
+            self.layer,
+            self.spatial_mapping,
+            start_ordering,
+            self.opt_criterion_name,
+        )
+        current_state = SalsaState(
+            self.accelerator,
+            self.layer,
+            self.spatial_mapping,
+            start_ordering,
+            self.opt_criterion_name,
+        )
+        next_state = SalsaState(
+            self.accelerator,
+            self.layer,
+            self.spatial_mapping,
+            start_ordering,
+            self.opt_criterion_name,
+        )
 
         for it in range(self.iteration_number):
 
-            temperature = self.start_temperature*(0.995**it)
+            temperature = self.start_temperature * (0.995**it)
 
             # Get the index of the loop to swap
             i = np.random.randint(0, len(current_state.ordering))
             j = np.random.randint(0, len(current_state.ordering))
 
             # Swap the loops
-            next_state = current_state.swap(i,j)
+            next_state = current_state.swap(i, j)
 
-            x = np.random.rand() # x belongs to [0, 1]
-            p = np.exp(((current_state.opt_criterion / next_state.opt_criterion) - 1) / temperature) # probability of accepting the next state
+            x = np.random.rand()  # x belongs to [0, 1]
+            p = np.exp(
+                ((current_state.opt_criterion / next_state.opt_criterion) - 1)
+                / temperature
+            )  # probability of accepting the next state
 
             if x < p:
                 # Replace the current state by the next state and compare the energy with the best state
                 current_state = deepcopy(next_state)
-                
-                if current_state.opt_criterion< best_state.opt_criterion:
+
+                if current_state.opt_criterion < best_state.opt_criterion:
                     best_state = deepcopy(current_state)
-        
-        cme_queue.put(best_state.cme)
 
+        cme_queue.put(best_state.cme)
 
     def get_temporal_loops(self):
         """
         Get all loops that have to be temporally scheduled given layer and spatial mapping.
         """
-        temporal_loop_dim_size = self.layer.loop_dim_size.copy()  # init with all loop sizes
+        temporal_loop_dim_size = (
+            self.layer.loop_dim_size.copy()
+        )  # init with all loop sizes
         for spatial_loop in self.spatial_mapping.spatial_loop_dim_size:
             (spatial_loop_dim, spatial_loop_size) = spatial_loop
             # Allow greedy mapping. If the spatial unrolling is not a multiple of the layer dimension size,
             # we take the ceil of the division, so there can be one extra temporal iteration.
-            q = int(np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size))
+            q = int(
+                np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size)
+            )
             # q, rem = divmod(temporal_loop_dim_size[spatial_loop_dim], spatial_loop_size)
             # assert rem == 0, "Division of dimension size by spatial unrolling size is not an integer"
             if q == 1:
                 del temporal_loop_dim_size[spatial_loop_dim]
             else:
                 temporal_loop_dim_size[spatial_loop_dim] = q
 
         # Remove all dimensions with a temporal loop size of 1
-        temporal_loop_dim_size_no_1s = {key: val for (key, val) in temporal_loop_dim_size.items() if val > 1}
+        temporal_loop_dim_size_no_1s = {
+            key: val for (key, val) in temporal_loop_dim_size.items() if val > 1
+        }
 
         self.temporal_loop_dim_size = temporal_loop_dim_size_no_1s
         min_nb_temporal_loops = len(self.temporal_loop_dim_size)
         if self.lpf_limit < min_nb_temporal_loops:
-            logger.debug(f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs.")
+            logger.debug(
+                f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs."
+            )
             self.lpf_limit = min_nb_temporal_loops
-    
 
     def get_prime_factors(self):
         """
         Get the prime factors for all temporal loops in the following format:
         [('C', 2), ('OY', 2), ('OX', 2), ('K', 7), ...]
         """
         temporal_loop_pfs = {}
         temporal_loop_pf_counts = {}
         temporal_loop_pf_count_sums = {}
         lpfs = []
 
         self.temporal_mapping_lpf = []
 
-        for (tl_dim, tl_size) in self.temporal_loop_dim_size.items():  # tl = temporal loop
+        for (
+            tl_dim,
+            tl_size,
+        ) in self.temporal_loop_dim_size.items():  # tl = temporal loop
             factors = factorint(tl_size)
             pfs = []
             counts = []
             for pf, multiplicity in factors.items():
                 pfs.append(pf)
                 counts.append(multiplicity)
                 for i in range(multiplicity):
                     lpfs.append((tl_dim, pf))
             temporal_loop_pfs[tl_dim] = tuple(pfs)
             temporal_loop_pf_counts[tl_dim] = tuple(counts)
             temporal_loop_pf_count_sums[tl_dim] = sum(counts)
 
-        #logger.info(f"Generated {len(lpfs)} LPFs for layer {self.layer}.")
+        # logger.info(f"Generated {len(lpfs)} LPFs for layer {self.layer}.")
 
         for loop_type in list(temporal_loop_pfs.keys()):
-          for i in range(len(temporal_loop_pfs[loop_type])):
-               loop_size = temporal_loop_pfs[loop_type]
-               for number_of_loop in range(temporal_loop_pf_counts[loop_type][i]):
-                    self.temporal_mapping_lpf.append((loop_type, loop_size[i]))
+            for i in range(len(temporal_loop_pfs[loop_type])):
+                loop_size = temporal_loop_pfs[loop_type]
+                for number_of_loop in range(temporal_loop_pf_counts[loop_type][i]):
+                    self.temporal_mapping_lpf.append((loop_type, loop_size[i]))
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag-dse-2.3.2/zigzag/classes/opt/temporal/salsa/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,105 @@
 #   =====================================================================
 #   Title:        state.py
-#   Description: This file contains the state class that represents a 
+#   Description: This file contains the state class that represents a
 #   state of SALSA's makrov chain.
-#  
+#
 #   Date:        02.01.2023
-#  
+#
 #   =====================================================================
-# 
+#
 #   Copyright (C) 2020 ETH Zurich and University of Bologna.
-#  
+#
 #   Author: Victor Jung, ETH Zurich
-#  
+#
 #   SPDX-License-Identifier: Apache-2.0
-#  
+#
 #   Licensed under the Apache License, Version 2.0 (the License); you may
 #   not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
-#  
+#
 #   www.apache.org/licenses/LICENSE-2.0
-#  
+#
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-#  
+#
 
 from copy import deepcopy
 from zigzag.classes.opt.temporal.loma.memory_allocator import MemoryAllocator
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.workload.layer_node import LayerNode
 from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 
+
 class SalsaState:
     """
     State of SALSA, storing an ordering, his temporal mapping and his energy value.
     """
 
-    def __init__(self, accelerator: Accelerator, layer: LayerNode, spatial_mapping: SpatialMapping, ordering, opt_criterion_name):
+    def __init__(
+        self,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMapping,
+        ordering,
+        opt_criterion_name,
+    ):
         self.ordering = ordering
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
-        self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(layer.core_allocation).memory_hierarchy
+        self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(
+            layer.core_allocation
+        ).memory_hierarchy
         self.opt_criterion_name = opt_criterion_name
 
-        allocator = MemoryAllocator(self.accelerator, self.layer, self.spatial_mapping, ordering) 
-        
+        allocator = MemoryAllocator(
+            self.accelerator, self.layer, self.spatial_mapping, ordering
+        )
+
         # allocator = MemoryAllocator(layer=self.layer,
         #                                 ordering=ordering,
         #                                 spatial_mapping=self.spatial_mapping)
 
-        self.temporal_mapping = allocator.run()  # allocate this ordering to the memories 
-
-        self.cme = CostModelEvaluation(accelerator=self.accelerator,
-                                  layer=self.layer,
-                                  spatial_mapping=self.spatial_mapping,
-                                  temporal_mapping=self.temporal_mapping)
+        self.temporal_mapping = (
+            allocator.run()
+        )  # allocate this ordering to the memories
+
+        self.cme = CostModelEvaluation(
+            accelerator=self.accelerator,
+            layer=self.layer,
+            spatial_mapping=self.spatial_mapping,
+            temporal_mapping=self.temporal_mapping,
+        )
 
         # The optimization criterion will be minimized
         if self.opt_criterion_name == "energy":
-            self.opt_criterion = self.cme.energy_total 
+            self.opt_criterion = self.cme.energy_total
         elif self.opt_criterion_name == "latency":
-            self.opt_criterion = self.cme.latency_total0 
+            self.opt_criterion = self.cme.latency_total0
         else:
-            self.opt_criterion = None   
-
+            self.opt_criterion = None
 
     def swap(self, i, j):
         """
-        Swap between the element at positon i and j in the ordering 
+        Swap between the element at positon i and j in the ordering
         and return the new resulting state.
         """
 
         swapped_ordering = deepcopy(self.ordering)
         temp = swapped_ordering[i]
         swapped_ordering[i] = swapped_ordering[j]
         swapped_ordering[j] = temp
 
-        return SalsaState(self.accelerator, self.layer, self.spatial_mapping, swapped_ordering, self.opt_criterion_name)
+        return SalsaState(
+            self.accelerator,
+            self.layer,
+            self.spatial_mapping,
+            swapped_ordering,
+            self.opt_criterion_name,
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/CostModelStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/CostModelStage.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,36 +4,61 @@
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
 from zigzag.classes.workload.layer_node import LayerNode
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class CostModelStage(Stage):
     """
     Pipeline stage that calls a cost model to evaluate a mapping on a HW config.
     """
-    def __init__(self, list_of_callables:List[Callable], *, accelerator, layer, spatial_mapping, temporal_mapping, access_same_data_considered_as_no_access=True, **kwargs):
+
+    def __init__(
+        self,
+        list_of_callables: List[Callable],
+        *,
+        accelerator,
+        layer,
+        spatial_mapping,
+        temporal_mapping,
+        access_same_data_considered_as_no_access=True,
+        **kwargs
+    ):
         """
         Initializes the cost model stage given main inputs
         """
         super().__init__(list_of_callables, **kwargs)
-        self.accelerator, self.layer, self.spatial_mapping, self.temporal_mapping, self.access_same_data_considered_as_no_access =\
-            accelerator, layer, spatial_mapping, temporal_mapping, access_same_data_considered_as_no_access
+        (
+            self.accelerator,
+            self.layer,
+            self.spatial_mapping,
+            self.temporal_mapping,
+            self.access_same_data_considered_as_no_access,
+        ) = (
+            accelerator,
+            layer,
+            spatial_mapping,
+            temporal_mapping,
+            access_same_data_considered_as_no_access,
+        )
 
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the cost model stage by calling the internal zigzag cost model with the correct inputs.
         """
-        self.cme = CostModelEvaluation(accelerator=self.accelerator,
-                                       layer=self.layer,
-                                       spatial_mapping=self.spatial_mapping,
-                                       temporal_mapping=self.temporal_mapping,
-                                       # the below parameter is optional
-                                       access_same_data_considered_as_no_access=self.access_same_data_considered_as_no_access)
+        self.cme = CostModelEvaluation(
+            accelerator=self.accelerator,
+            layer=self.layer,
+            spatial_mapping=self.spatial_mapping,
+            temporal_mapping=self.temporal_mapping,
+            # the below parameter is optional
+            access_same_data_considered_as_no_access=self.access_same_data_considered_as_no_access,
+        )
         yield (self.cme, None)
 
     def is_leaf(self) -> bool:
-        return True
+        return True
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/DumpStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/DumpStage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pickle
 from typing import Generator, Any, Tuple
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 import os
 
+
 class DumpStage(Stage):
     """
     Class that passes through all results yielded by substages, but dumps the results as a pickled list to a file
     at the end of the iteration
     """
 
     def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
@@ -28,9 +29,9 @@
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
         list = []
         filename = self.dump_filename_pattern.format(**self.kwargs)
         for cme, extra_info in substage.run():
             list.append((cme, extra_info))
             yield cme, extra_info
         os.makedirs(os.path.dirname(filename), exist_ok=True)
-        with open(filename, 'wb') as f:
+        with open(filename, "wb") as f:
             pickle.dump(list, f, -1)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/GeneralParameterIteratorStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/GeneralParameterIteratorStage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 
 from typing import Generator, Callable, List, Tuple, Any
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+
 logger = logging.getLogger(__name__)
 
 
 class GeneralParameterIteratorStage(Stage):
     """
     General iterator over any parameter whose values can be set from a predetermined list
     """
+
     def __init__(self, list_of_callables, *, general_parameter_iterations, **kwargs):
         """
 
         :param list_of_callables: see Stage
         :param general_parameter_iterations: dictionary with:
                 - keys: variables to iterate over, or tuples of variables to iterate over
                         With K1 and K2 both keys, all combinations of K1 values and K2 values are tried.
@@ -35,36 +37,49 @@
                 if isinstance(key, (list, tuple)):
                     for kk, vv in zip(key, v):
                         runparams[kk] = vv
                     iterable = True
                 else:
                     runparams[key] = v
                     iterable = False
-                for cme, extra_info in self.recursive_run( reduced_param_iters_reduced, runparams):
-                    yield cme, ( (tuple((kk, vv) for kk, vv in zip(key, v)) + extra_info[0],) + extra_info[1:] \
-                                 if iterable else \
-                               (((key, v),) + extra_info[0],) + extra_info[1:] )
+                for cme, extra_info in self.recursive_run(
+                    reduced_param_iters_reduced, runparams
+                ):
+                    yield cme, (
+                        (tuple((kk, vv) for kk, vv in zip(key, v)) + extra_info[0],)
+                        + extra_info[1:]
+                        if iterable
+                        else (((key, v),) + extra_info[0],) + extra_info[1:]
+                    )
         else:
             # trivial case, no more extra parameters to iterate over
-            sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **runparams)
+            sub_stage = self.list_of_callables[0](
+                self.list_of_callables[1:], **runparams
+            )
             for cme, extra_info in sub_stage.run():
                 yield cme, (tuple(), extra_info)
 
     def run(self):
         return self.recursive_run(self.param_iters, self.kwargs)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
+
     class Dummy(Stage):
         def is_leaf(self):
             return True
+
         def run(self):
             yield None, self.kwargs
+
     from zigzag.classes.stages.Stage import MainStage
-    DUT = MainStage([GeneralParameterIteratorStage, Dummy],
-                       general_parameter_iterations = {
-        ('arg1.1', 'arg1.2'): ((111, 121), (112, 122), (113, 123)),
-        'arg2': (21, 22, 23, 24, 25),
-        'arg3': (31, 32)
-        })
+
+    DUT = MainStage(
+        [GeneralParameterIteratorStage, Dummy],
+        general_parameter_iterations={
+            ("arg1.1", "arg1.2"): ((111, 121), (112, 122), (113, 123)),
+            "arg2": (21, 22, 23, 24, 25),
+            "arg3": (31, 32),
+        },
+    )
     for l in DUT.run():
-        print(l)
+        print(l)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/LomaStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/LomaStage.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,33 +8,50 @@
 
 
 class LomaStage(Stage):
     """
     Class that iterates through the different temporal mappings generated through
     the loop order based memory allocation (loma) engine
     """
-    def __init__(self, list_of_callables: List[Callable], *, accelerator, layer, spatial_mapping, **kwargs):
+
+    def __init__(
+        self,
+        list_of_callables: List[Callable],
+        *,
+        accelerator,
+        layer,
+        spatial_mapping,
+        **kwargs
+    ):
         """Initialize the LomaStage by setting the accelerator, layer, and spatial mapping.
 
         Args:
             list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
             accelerator (Accelerator): The accelerator object.
             layer (Layer): The layer object.
             spatial_mapping (SpatialMapping): The spatial mapping object.
         """
         super().__init__(list_of_callables, **kwargs)
-        self.accelerator, self.layer, self.spatial_mapping = accelerator, layer, spatial_mapping
+        self.accelerator, self.layer, self.spatial_mapping = (
+            accelerator,
+            layer,
+            spatial_mapping,
+        )
         self.engine = None
 
     def run(self):
-        self.engine = LomaEngine(accelerator=self.accelerator, layer=self.layer, spatial_mapping=self.spatial_mapping,
-                                 **self.kwargs)
+        self.engine = LomaEngine(
+            accelerator=self.accelerator,
+            layer=self.layer,
+            spatial_mapping=self.spatial_mapping,
+            **self.kwargs
+        )
 
         for tm in self.engine.run():
             kwargs = self.kwargs.copy()
-            kwargs['accelerator'] = self.accelerator
-            kwargs['layer'] = self.layer
-            kwargs['spatial_mapping'] = self.spatial_mapping
-            kwargs['temporal_mapping'] = tm
+            kwargs["accelerator"] = self.accelerator
+            kwargs["layer"] = self.layer
+            kwargs["spatial_mapping"] = self.spatial_mapping
+            kwargs["temporal_mapping"] = tm
             sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
             for cme, extra_info in sub_stage.run():
                 yield cme, (tm, extra_info)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/MainInputParserStages.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/MainInputParserStages.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,25 +52,7 @@
 
     def run(self):
         workload = parse_workload_from_path_or_from_module(self.workload, self.mapping)
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], workload=workload, **self.kwargs)
         for cme, extra_info in sub_stage.run():
             yield cme, extra_info
 
-
-class WorkloadAndAcceleratorParserStage(Stage):
-    """
-    Convenience class to parse both the workload and accelerator
-    """
-    def __init__(self, list_of_callables, *, workload_path, accelerator_path, **kwargs):
-        super().__init__(list_of_callables, **kwargs)
-        self.workload_path = workload_path
-        self.accelerator_path = accelerator_path
-
-    def run(self):
-        workload = parse_workload_from_path(self.workload_path)
-        accelerator_parser = AcceleratorParser(self.accelerator_path)
-        accelerator_parser.run()
-        accelerator = accelerator_parser.get_accelerator()
-        sub_stage = self.list_of_callables[0](self.list_of_callables[1:], accelerator=accelerator, workload=workload, **self.kwargs)
-        for cme, extra_info in sub_stage.run():
-            yield cme, extra_info
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/ONNXModelParserStage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import Generator
 
 from zigzag.classes.io.onnx.model import ONNXModelParser
 from zigzag.classes.stages.Stage import Stage
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 
 class ONNXModelParserStage(Stage):
     def __init__(self, list_of_callables, *, workload, mapping, **kwargs):
         super().__init__(list_of_callables, **kwargs)
         self.onnx_model_parser = ONNXModelParser(workload, mapping)
-    
+
     def run(self) -> Generator:
         self.onnx_model_parser.run()
         onnx_model = self.onnx_model_parser.get_onnx_model()
         workload = self.onnx_model_parser.get_workload()
 
-        sub_stage = self.list_of_callables[0](self.list_of_callables[1:], onnx_model=onnx_model, workload=workload, **self.kwargs)
+        sub_stage = self.list_of_callables[0](
+            self.list_of_callables[1:],
+            onnx_model=onnx_model,
+            workload=workload,
+            **self.kwargs
+        )
         for cme, extra_info in sub_stage.run():
             yield cme, extra_info
 
     # # For testing purposes
     # def is_leaf(self) -> bool:
     #     return True
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/PlotTemporalMappingsStage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import pickle
+import os
+
 from typing import Generator, Any, Tuple
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
-from zigzag.visualization.results.plot_cme import bar_plot_cost_model_evaluations_breakdown
-import os
+from zigzag.visualization.results.plot_cme import (
+    bar_plot_cost_model_evaluations_breakdown,
+)
+
 
 class PlotTemporalMappingsStage(Stage):
     """
     Class that passes through all results yielded by substages, but keeps the TMs cme's and saves a plot.
     """
 
     def __init__(self, list_of_callables, *, plot_filename_pattern, **kwargs):
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/ReduceStages.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/ReduceStages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,119 +1,146 @@
 import logging
 
-from typing import Generator, Callable, List, Tuple, Any
+from typing import Generator, Tuple, Any
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+
 logger = logging.getLogger(__name__)
 
 
 class MinimalEnergyStage(Stage):
     """
     Class that keeps yields only the cost model evaluation that has minimal energy of all cost model evaluations
     generated by it's substages created by list_of_callables
     """
-    def __init__(self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs):
+
+    def __init__(
+        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
+    ):
         """
         Initialize the compare stage.
         """
         super().__init__(list_of_callables, **kwargs)
         self.best_cme = None
         # Visualization stuff
         self.energies = []
         self.keep_others = reduce_minimal_keep_others
 
-
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the compare stage by comparing a new cost model output with the current best found result.
         """
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
         other_cmes = []
         for cme, extra_info in substage.run():
             self.energies.append(cme.energy_total)
-            if self.best_cme is None or cme.energy_total < self.best_cme.energy_total or (cme.energy_total == self.best_cme.energy_total and cme.latency_total2 < self.best_cme.latency_total2):
+            if (
+                self.best_cme is None
+                or cme.energy_total < self.best_cme.energy_total
+                or (
+                    cme.energy_total == self.best_cme.energy_total
+                    and cme.latency_total2 < self.best_cme.latency_total2
+                )
+            ):
                 self.best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
         yield (self.best_cme, other_cmes)
 
 
 class MinimalLatencyStage(Stage):
     """
     Class that keeps yields only the cost model evaluation that has minimal latency of all cost model evaluations
     generated by it's substages created by list_of_callables
     """
-    def __init__(self, list_of_callables,*, reduce_minimal_keep_others=False, **kwargs):
+
+    def __init__(
+        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
+    ):
         """
         Initialize the compare stage.
         """
         super().__init__(list_of_callables, **kwargs)
         self.best_cme = None
         self.keep_others = reduce_minimal_keep_others
 
-
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the compare stage by comparing a new cost model output with the current best found result.
         """
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
         other_cmes = []
         for cme, extra_info in substage.run():
-            if self.best_cme is None or cme.latency_total2 < self.best_cme.latency_total2 or (cme.latency_total2 == self.best_cme.latency_total2 and cme.energy_total < self.best_cme.energy_total):
+            if (
+                self.best_cme is None
+                or cme.latency_total2 < self.best_cme.latency_total2
+                or (
+                    cme.latency_total2 == self.best_cme.latency_total2
+                    and cme.energy_total < self.best_cme.energy_total
+                )
+            ):
                 self.best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
         yield (self.best_cme, other_cmes)
 
+
 class MinimalEDPStage(Stage):
     """
     Class that keeps yields only the cost model evaluation that has minimal EDP of all cost model evaluations
     generated by it's substages created by list_of_callables
     """
-    def __init__(self, list_of_callables,*, reduce_minimal_keep_others=False, **kwargs):
+
+    def __init__(
+        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
+    ):
         """
         Initialize the compare stage.
         """
         super().__init__(list_of_callables, **kwargs)
         self.best_cme = None
         self.keep_others = reduce_minimal_keep_others
 
-
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the compare stage by comparing a new cost model output with the current best found result.
         """
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
         other_cmes = []
         for cme, extra_info in substage.run():
-            if self.best_cme is None or cme.latency_total2*cme.energy_total < self.best_cme.latency_total2*self.best_cme.energy_total:
+            if (
+                self.best_cme is None
+                or cme.latency_total2 * cme.energy_total
+                < self.best_cme.latency_total2 * self.best_cme.energy_total
+            ):
                 self.best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
         yield (self.best_cme, other_cmes)
 
+
 class SumStage(Stage):
     """
     Class that keeps yields only the sum of all cost model evaluations generated by its
     substages created by list_of_callables
     """
+
     def __init__(self, list_of_callables, **kwargs):
         """
         Initialize the compare stage.
         """
         super().__init__(list_of_callables, **kwargs)
         self.total_cme = None
 
-
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the compare stage by comparing a new cost model output with the current best found result.
         """
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
 
         all_cmes = []
@@ -121,24 +148,25 @@
             if self.total_cme is None:
                 self.total_cme = cme
             else:
                 self.total_cme += cme
             all_cmes.append((cme, extra_info))
         yield self.total_cme, all_cmes
 
+
 class ListifyStage(Stage):
     """Class yields all the cost model evaluations yielded by its substages as a single list instead of as a generator."""
+
     def __init__(self, list_of_callables, **kwargs):
         """
         Initialize the compare stage.
         """
         super().__init__(list_of_callables, **kwargs)
         self.list = []
 
-
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the compare stage by comparing a new cost model output with the current best found result.
         """
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
 
         for cme, extra_info in substage.run():
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/RunOptStages.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/RunOptStages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-from typing import Generator, Callable, List, Tuple, Any
+from typing import Generator, Tuple, Any
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 
 import logging
 import os
+
 logger = logging.getLogger(__name__)
 
 
 class RemoveExtraInfoStage(Stage):
     """
     Strips extra info for subcallables to save memory
     """
+
     def __init__(self, list_of_callables, **kwargs):
         """
         Initialize the remove extra info stage.
         """
         super().__init__(list_of_callables, **kwargs)
 
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the remove extra info stage by running the substage and discarding the extra_info.
         """
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
         for cme, extra_info in substage.run():
-           yield cme, None
+            yield cme, None
+
 
 class CacheBeforeYieldStage(Stage):
     """
     Caches results in a list and then yields them.
     This breaks the yield flow from top to bottom.
     """
+
     def __init__(self, list_of_callables, **kwargs):
         """
         Initialize the cache before yield stage.
         """
         super().__init__(list_of_callables, **kwargs)
 
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
@@ -43,123 +47,145 @@
         Run the cache before yield stage by running the substage and caching everything it yields, then yielding everything.
         """
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
         to_yield = []
         for ty in substage.run():
-           to_yield.append(ty)
+            to_yield.append(ty)
         for ty in to_yield:
             yield ty
 
+
 class SkipIfDumpExistsStage(Stage):
     """
     Check if the output file is already generated, skip the run if so.
     """
+
     def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
         super().__init__(list_of_callables, **kwargs)
         self.dump_filename_pattern = dump_filename_pattern
 
     def run(self):
         filename = self.dump_filename_pattern.format(**self.kwargs)
         if os.path.isfile(filename):
-            print(f"==================================Dump {filename} already existed. Skip! ==================================")
+            print(
+                f"==================================Dump {filename} already existed. Skip! =================================="
+            )
             return
-        substage = self.list_of_callables[0](self.list_of_callables[1:], dump_filename_pattern=self.dump_filename_pattern, **self.kwargs)
+        substage = self.list_of_callables[0](
+            self.list_of_callables[1:],
+            dump_filename_pattern=self.dump_filename_pattern,
+            **self.kwargs,
+        )
         for cme, extra in substage.run():
             yield cme, extra
 
 
-
-
 import multiprocessing
 
 
 threadpool = None
 
+
 def get_threadpool(nb_threads_if_non_existent):
     global threadpool
     if threadpool is None:
         threadpool = multiprocessing.Pool(nb_threads_if_non_existent)
     return threadpool
 
+
 def close_threadpool():
     global threadpool
     threadpool.close()
     threadpool = None
 
+
 def terminate_threadpool():
     global threadpool
     threadpool.terminate()
     threadpool = None
 
 
 def raise_exception(e):
     terminate_threadpool()
     raise e
 
+
 class MultiProcessingSpawnStage(Stage):
     """
     Multiprocessing support stage.
     Warning: does not yield (CostModelEvaluation, extra_info) pairs.
     Use as follows in a list_of_callables:
     [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
      every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
     Note: list of callables may not contain lambda functions, as this will break pickling which is required for
           by multiprocessing
     Note: there is quite some overhead in spawning these parallel processes (python...; it needs to copy through pickle
           all variables), so best to do this at some high level loop (early in list of callables)
     """
-    def __init__(self, list_of_callables, *, multiprocessing_callback, nb_multiprocessing_threads=multiprocessing.cpu_count(), **kwargs):
+
+    def __init__(
+        self,
+        list_of_callables,
+        *,
+        multiprocessing_callback,
+        nb_multiprocessing_threads=multiprocessing.cpu_count(),
+        **kwargs,
+    ):
         """
 
         :param list_of_callables: may not contain lambda functions, as this will break pickling which is required for
           by multiprocessing.
         :param multiprocessing_callback: intended to be set by MultiProcessingGatherStage
         :param kwargs:
         """
         super().__init__(list_of_callables, **kwargs)
         self.nb_multiprocessing_threads = nb_multiprocessing_threads
         self.callback = multiprocessing_callback
 
     def _to_run(self):
         return list(self.sub_stage.run())
 
-
-
     def run(self):
-        self.sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        get_threadpool(self.nb_multiprocessing_threads).apply_async(self._to_run, callback=self.callback, error_callback=raise_exception)
+        self.sub_stage = self.list_of_callables[0](
+            self.list_of_callables[1:], **self.kwargs
+        )
+        get_threadpool(self.nb_multiprocessing_threads).apply_async(
+            self._to_run, callback=self.callback, error_callback=raise_exception
+        )
         yield None, None
 
+
 class MultiProcessingGatherStage(Stage):
     """
     Multiprocessing support stage.
     Use as follows in a list_of_callables:
     [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
      every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
     Note: list of callables may not contain lambda functions, as this will break pickling which is required for
           by multiprocessing
     """
+
     def _callback(self, ans):
         self.queue.put(ans)
 
     def run(self):
         self.queue = multiprocessing.Manager().Queue()
         kwargs = self.kwargs.copy()
-        kwargs['multiprocessing_callback'] = self._callback
+        kwargs["multiprocessing_callback"] = self._callback
 
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
         count_to_get = 0
         for i in sub_stage.run():
             count_to_get += 1
-        logger.info(f'Multiprocessing results to get: {count_to_get}')
+        logger.info(f"Multiprocessing results to get: {count_to_get}")
         count = 0
         while count < count_to_get:
             for ans in self.queue.get(block=True):
                 yield ans
             count += 1
             if count % (count_to_get // 10) == 0:
-                logger.info(f'Multiprocessing results received: {count} of {count_to_get}')
+                logger.info(
+                    f"Multiprocessing results received: {count} of {count_to_get}"
+                )
         close_threadpool()
-
-
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/SalsaStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/SalsaStage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #   =====================================================================
 #   Title:        SalsaStage.py
 #   Description:
-#  
+#
 #   Date:        02.01.2023
-#  
+#
 #   =====================================================================
-# 
+#
 #   Copyright (C) 2020 ETH Zurich and University of Bologna.
-#  
+#
 #   Author: Victor Jung, ETH Zurich
-#  
+#
 #   SPDX-License-Identifier: Apache-2.0
-#  
+#
 #   Licensed under the Apache License, Version 2.0 (the License); you may
 #   not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
-#  
+#
 #   www.apache.org/licenses/LICENSE-2.0
-#  
+#
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-#  
+#
 
 import multiprocessing_on_dill as multiprocessing
 from sympy.ntheory import factorint
 from copy import deepcopy
 import logging
 
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
@@ -39,117 +39,139 @@
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 
 from zigzag.classes.stages.ReduceStages import MinimalEnergyStage
 from zigzag.classes.stages.ReduceStages import MinimalLatencyStage
 
 logger = logging.getLogger(__name__)
 
+
 class SalsaStage(Stage):
     """
     Class that return the best temporal mapping found by the Simulated Annealing
     Loop-ordering Scheduler for Accelerators (SALSA) for a single layer.
     """
-    def __init__(self, list_of_callables: List[Callable], *, accelerator, layer, spatial_mapping, **kwargs):
+
+    def __init__(
+        self,
+        list_of_callables: List[Callable],
+        *,
+        accelerator,
+        layer,
+        spatial_mapping,
+        **kwargs,
+    ):
         """Initialize the LomaStage by setting the accelerator, layer, and spatial mapping.
 
         Args:
             list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
             accelerator (Accelerator): The accelerator object.
             layer (Layer): The layer object.
             spatial_mapping (SpatialMapping): The spatial mapping object.
         """
         super().__init__(list_of_callables, **kwargs)
-        self.accelerator, self.layer, self.spatial_mapping = accelerator, layer, spatial_mapping
+        self.accelerator, self.layer, self.spatial_mapping = (
+            accelerator,
+            layer,
+            spatial_mapping,
+        )
         self.engine = None
         self.best_cme = None
 
         self.opt_criterion_name = kwargs.get("salsa_opt_criterion", "energy")
         self.number_of_core_allocated = kwargs.get("salsa_number_of_core", 1)
-        
+
         # Multiprocessing parameters
         self.worker_list = []
         self.cme_queue = multiprocessing.Queue()
 
         if self.opt_criterion_name == "energy":
             self.compare_stage = self.compare_cme_energy
         elif self.opt_criterion_name == "latency":
             self.compare_stage = self.compare_cme_latency
-        else:  
-            raise Exception("Invalid optimization criterion for SALSA. Must be either 'energy' or 'latency'.")
-
+        else:
+            raise Exception(
+                "Invalid optimization criterion for SALSA. Must be either 'energy' or 'latency'."
+            )
 
     def run(self):
         """
         Set up and start salsa engine, then collect and return the best cost model evaluation
         """
 
-        logger.info(f"Running SALSA Temporal Mapping Optimizer with {self.number_of_core_allocated} core(s).")
-
-        self.engine = SalsaEngine(accelerator=self.accelerator, 
-                                    layer=self.layer, 
-                                    spatial_mapping=self.spatial_mapping, 
-                                    **self.kwargs)
+        logger.info(
+            f"Running SALSA Temporal Mapping Optimizer with {self.number_of_core_allocated} core(s)."
+        )
+
+        self.engine = SalsaEngine(
+            accelerator=self.accelerator,
+            layer=self.layer,
+            spatial_mapping=self.spatial_mapping,
+            **self.kwargs,
+        )
 
         # self.best_cme = self.engine.run(self.cme_queue)
 
         # Get the number of core the user wants to allocate
         if self.number_of_core_allocated <= multiprocessing.cpu_count():
             self.number_of_core = self.number_of_core_allocated
         else:
             self.number_of_core = multiprocessing.cpu_count()
 
         # Create processes
-        for core_id in range(0,self.number_of_core):
+        for core_id in range(0, self.number_of_core):
             p = multiprocessing.Process(target=self.engine.run, args=(self.cme_queue,))
             self.worker_list.append(p)
 
         # Start the processes
-        for core_id in range(0,self.number_of_core):
+        for core_id in range(0, self.number_of_core):
             logger.debug(f"Starting SALSA Process #{core_id}.")
             self.worker_list[core_id].start()
 
         # For every core we gather the ouput
-        for core_id in range(0,self.number_of_core):
+        for core_id in range(0, self.number_of_core):
             cme = self.cme_queue.get()
             self.compare_stage(cme)
 
         # Then join them to make sure they all end before continuing the execution
-        for core_id in range(0,self.number_of_core):
+        for core_id in range(0, self.number_of_core):
             self.worker_list[core_id].join()
 
-
         kwargs = self.kwargs.copy()
-        kwargs['accelerator'] = self.accelerator
-        kwargs['layer'] = self.layer
-        kwargs['spatial_mapping'] = self.spatial_mapping
-        kwargs['temporal_mapping'] = self.best_cme.mapping.temporal_mapping
+        kwargs["accelerator"] = self.accelerator
+        kwargs["layer"] = self.layer
+        kwargs["spatial_mapping"] = self.spatial_mapping
+        kwargs["temporal_mapping"] = self.best_cme.mapping.temporal_mapping
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
 
         for cme, extra_info in sub_stage.run():
             yield cme, (self.best_cme.mapping.temporal_mapping, extra_info)
 
-
     def compare_cme_latency(self, cme):
         """
         Compare the latency of the current cost model evaluation with the best latency found so far.
         Then replace the current best cme if the current cme has a lower latency.
         """
 
         if self.best_cme is None:
             self.best_cme = cme
-        elif cme.latency_total2 == self.best_cme.latency_total2 and cme.energy_total < self.best_cme.energy_total:
+        elif (
+            cme.latency_total2 == self.best_cme.latency_total2
+            and cme.energy_total < self.best_cme.energy_total
+        ):
             self.best_cme = cme
         elif cme.latency_total2 < self.best_cme.latency_total2:
             self.best_cme = cme
 
-
     def compare_cme_energy(self, cme):
         """
         Compare the energy of the current cost model evaluation with the best energy found so far.
         Then replace the best cme if the current cme has a lower energy.
         """
         if self.best_cme is None:
             self.best_cme = cme
-        elif cme.energy_total == self.best_cme.energy_total and cme.latency_total2 < self.best_cme.latency_total2:
+        elif (
+            cme.energy_total == self.best_cme.energy_total
+            and cme.latency_total2 < self.best_cme.latency_total2
+        ):
             self.best_cme = cme
         elif cme.energy_total < self.best_cme.energy_total:
-            self.best_cme = cme
+            self.best_cme = cme
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/SaveStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/SaveStage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Generator, Any, Tuple
 from zigzag.classes.stages.Stage import Stage
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 import os
 import pickle
 import json
-from datetime import datetime
 import numpy as np
 
 import logging
+
 logger = logging.getLogger(__name__)
 
+
 class CompleteSaveStage(Stage):
     """
     Class that passes through all results yielded by substages, but saves the results as a json list to a file
     at the end of the iteration.
     """
 
     def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
@@ -28,42 +29,50 @@
 
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the complete save stage by running the substage and saving the CostModelEvaluation json representation.
         """
         self.kwargs["dump_filename_pattern"] = self.dump_filename_pattern
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        
+
         for id, (cme, extra_info) in enumerate(substage.run()):
             cme: CostModelEvaluation
             # filename = self.dump_filename_pattern.format(datetime=datetime.now().isoformat().replace(":", "-"))
             if type(cme.layer) == list:
-                filename = self.dump_filename_pattern.replace('?', 'overall_completeSave')
+                filename = self.dump_filename_pattern.replace(
+                    "?", "overall_complete"
+                )
             else:
-                filename = self.dump_filename_pattern.replace('?', str(cme.layer) + '_completeSave')
+                filename = self.dump_filename_pattern.replace(
+                    "?", f"{cme.layer}_complete"
+                )
             self.save_to_json(cme, filename=filename)
-            logger.info(f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}")
+            logger.info(
+                f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}"
+            )
             yield cme, extra_info
 
     def save_to_json(self, obj, filename):
         os.makedirs(os.path.dirname(filename), exist_ok=True)
-        with open(filename, 'w') as fp:
+        with open(filename, "w") as fp:
             json.dump(obj, fp, default=self.complexHandler, indent=4)
 
     @staticmethod
     def complexHandler(obj):
         # print(type(obj))
         if isinstance(obj, set):
             return list(obj)
         if isinstance(obj, np.int32):
             return int(obj)
-        if hasattr(obj, '__jsonrepr__'):
+        if hasattr(obj, "__jsonrepr__"):
             return obj.__jsonrepr__()
         else:
-            raise TypeError(f"Object of type {type(obj)} is not serializable. Create a __jsonrepr__ method.")
+            raise TypeError(
+                f"Object of type {type(obj)} is not serializable. Create a __jsonrepr__ method."
+            )
 
 
 class SimpleSaveStage(Stage):
     """
     Class that passes through results yielded by substages, but saves the results as a json list to a file
     at the end of the iteration.
     In this simple version, only the energy total and latency total are saved.
@@ -81,44 +90,48 @@
 
     def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
         """
         Run the simple save stage by running the substage and saving the CostModelEvaluation simple json representation.
         """
         self.kwargs["dump_filename_pattern"] = self.dump_filename_pattern
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        
+
         for id, (cme, extra_info) in enumerate(substage.run()):
             cme: CostModelEvaluation
             # filename = self.dump_filename_pattern.format(datetime=datetime.now().isoformat().replace(":", "-"))
             if type(cme.layer) == list:
-                filename = self.dump_filename_pattern.replace('?', 'overall_simpleSave')
+                filename = self.dump_filename_pattern.replace("?", "overall_simple")
             else:
-                filename = self.dump_filename_pattern.replace('?', str(cme.layer) + '_simpleSave')
+                filename = self.dump_filename_pattern.replace(
+                    "?", f"{cme.layer}_simple"
+                )
             self.save_to_json(cme, filename=filename)
-            logger.info(f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}")
+            logger.info(
+                f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}"
+            )
             yield cme, extra_info
 
-
     def save_to_json(self, obj, filename):
         os.makedirs(os.path.dirname(filename), exist_ok=True)
-        with open(filename, 'w') as fp:
+        with open(filename, "w") as fp:
             json.dump(obj, fp, default=self.complexHandler, indent=4)
 
-
     @staticmethod
     def complexHandler(obj):
         # print(type(obj))
         if isinstance(obj, set):
             return list(obj)
         if isinstance(obj, np.int32):
             return int(obj)
-        if hasattr(obj, '__simplejsonrepr__'):
+        if hasattr(obj, "__simplejsonrepr__"):
             return obj.__simplejsonrepr__()
         else:
-            raise TypeError(f"Object of type {type(obj)} is not serializable. Create a __simplejsonrepr__ method.")
+            raise TypeError(
+                f"Object of type {type(obj)} is not serializable. Create a __simplejsonrepr__ method."
+            )
 
 
 class PickleSaveStage(Stage):
     """
     Class that dumps all received CMEs into a list and saves that list to a pickle file.
     """
 
@@ -142,8 +155,10 @@
             yield cme, extra_info
         # After we have received all the CMEs, save them to the specified output location.
         dirname = os.path.dirname(self.pickle_filename)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         with open(self.pickle_filename, "wb") as handle:
             pickle.dump(all_cmes, handle, protocol=pickle.HIGHEST_PROTOCOL)
-        logger.info(f"Saved pickled list of {len(all_cmes)} CMEs to {self.pickle_filename}.")
+        logger.info(
+            f"Saved pickled list of {len(all_cmes)} CMEs to {self.pickle_filename}."
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/SpatialMappingConversionStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/SpatialMappingConversionStage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import logging
 
 import numpy as np
 
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.workload.layer_node import LayerNode
 
 logger = logging.getLogger(__name__)
 
 
 class SpatialMappingConversionStage(Stage):
     """
     Pipeline stage that converts the spatial mapping from a
@@ -38,26 +36,28 @@
         :return: True
         """
         if not isinstance(layer.core_allocation, int):
             logger.critical(f"Layer {layer} has no core allocation.")
             raise ValueError(f"Missing core allocation for {layer}.")
         if not layer.user_spatial_mapping:
             logger.critical(f"Layer {layer} has no user-defined spatial mapping.")
-            raise ValueError("Missing spatial mapping for {layer}. Please provide 'spatial_mapping' for {layer}.")
+            raise ValueError(
+                "Missing spatial mapping for {layer}. Please provide 'spatial_mapping' for {layer}."
+            )
 
         return True
 
     def run(self):
 
         user_spatial_mapping = self.layer.user_spatial_mapping
         spatial_mapping = self.convert_user_spatial_mapping(user_spatial_mapping)
         kwargs = self.kwargs.copy()
-        kwargs['spatial_mapping'] = spatial_mapping
-        kwargs['accelerator'] = self.accelerator
-        kwargs['layer'] = self.layer
+        kwargs["spatial_mapping"] = spatial_mapping
+        kwargs["accelerator"] = self.accelerator
+        kwargs["layer"] = self.layer
 
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
         for cme, extra_info in sub_stage.run():
             yield cme, extra_info
 
     def convert_user_spatial_mapping(self, user_spatial_mapping):
         """
@@ -67,15 +67,15 @@
         - the user defined spatial mapping
         - the core (i.e. operational array) on which the unrolling happens,
           and the memory hierarchy that is connected to that operational array.
         :param user_spatial_mapping: The user-defined spatial mapping to be converted.
         Returns: A SpatialMapping object with the converted spatial mapping.
         """
         # Adjust the user defined spatial mapping size based on the operational array dimension and the layer dimension:
-        # E.g. user-provided unrolling is 16 but operational array dimension size iso only 12: change unrolling to 12 
+        # E.g. user-provided unrolling is 16 but operational array dimension size iso only 12: change unrolling to 12
         # E.g. user-provided unrolling is 16 but layer dimension is only 12: change unrolling to 12
         # E.g. user-provided unrolling is 16 but layer dimension is not a multiple of 16: change unrolling to fractional number
         # so that the temporal remainder is an integer.
         core_id = self.layer.core_allocation
         core = self.accelerator.get_core(core_id)
         mem_hierarchy = core.memory_hierarchy
         oa_dims = core.operational_array.dimensions
@@ -83,43 +83,62 @@
         limited_user_spatial_mapping = {}  # init dict we will be filling
         for oa_dim_name, spatial_loop in user_spatial_mapping.items():
             (loop_dim_unrolled, loop_size_unrolled) = spatial_loop
             # Check 0: Skip this spatial dimension if it doesn't exist in the layer
             if loop_dim_unrolled not in layer_dim_sizes.keys():
                 continue
             # Check 1: Limit unrolling if operational array dimension is smaller than provided unrolling
-            oa_dim_size = next((oa_dim for oa_dim in oa_dims if oa_dim.name == oa_dim_name)).size
+            oa_dim_size = next(
+                (oa_dim for oa_dim in oa_dims if oa_dim.name == oa_dim_name)
+            ).size
             loop_size_unrolled = min(oa_dim_size, loop_size_unrolled)
             # Check 2: Limit unrolling if layer dimension is smaller than provided unrolling or if the loop dim doesn't exist
             layer_dim_size = layer_dim_sizes.get(loop_dim_unrolled, 1)
             loop_size_unrolled = min(layer_dim_size, loop_size_unrolled)
             # Check 3: Adjust unrolling if it is not a multiple of the layer dimension size
-            temporal_remainder = int(np.ceil(layer_dim_size/loop_size_unrolled))
+            temporal_remainder = int(np.ceil(layer_dim_size / loop_size_unrolled))
             loop_size_unrolled = layer_dim_size / temporal_remainder
             # Set the adjusted unrolling size in the original user_spatial_mapping dict if it is greater than 1
-            limited_user_spatial_mapping[oa_dim_name] = (loop_dim_unrolled, loop_size_unrolled)
+            limited_user_spatial_mapping[oa_dim_name] = (
+                loop_dim_unrolled,
+                loop_size_unrolled,
+            )
             # Update the layer_dim_size to support multiple oa dims unrolling the same loop dim but not unrolling it more than the total layer dim
-            if temporal_remainder == 1:  # Remove it from the dict if we have unrolled the entirely layer dim onto the array dimension(s)
+            if (
+                temporal_remainder == 1
+            ):  # Remove it from the dict if we have unrolled the entirely layer dim onto the array dimension(s)
                 del layer_dim_sizes[loop_dim_unrolled]
-            else: # Update the dict if we have some layer dims left to potentially unroll onto the next oa dims
+            else:  # Update the dict if we have some layer dims left to potentially unroll onto the next oa dims
                 layer_dim_sizes[loop_dim_unrolled] = temporal_remainder
 
-        user_spatial_mapping_for_log = {array_dim: (loop_dim, f"{loop_size:.2f}") for (array_dim, (loop_dim, loop_size)) in limited_user_spatial_mapping.items()}
-        logger.debug(f"User-provided spatial mapping converted to: {user_spatial_mapping_for_log}")
+        user_spatial_mapping_for_log = {
+            array_dim: (loop_dim, f"{loop_size:.2f}")
+            for (
+                array_dim,
+                (loop_dim, loop_size),
+            ) in limited_user_spatial_mapping.items()
+        }
+        logger.debug(
+            f"User-provided spatial mapping converted to: {user_spatial_mapping_for_log}"
+        )
 
         spatial_mapping_dict = {}
         layer_to_mem_op = self.layer.memory_operand_links
-        mem_to_layer_op = {mem_op: layer_op for (layer_op, mem_op) in layer_to_mem_op.items()}
+        mem_to_layer_op = {
+            mem_op: layer_op for (layer_op, mem_op) in layer_to_mem_op.items()
+        }
         core_id = self.layer.core_allocation
         mem_hierarchy = self.accelerator.get_core(core_id).memory_hierarchy
         for mem_op, layer_op in mem_to_layer_op.items():
             user_sm_copy = limited_user_spatial_mapping.copy()
             # layer_op = mem_to_layer_op[mem_op]
             spatial_mapping_dict[layer_op] = []
-            memory_levels = mem_hierarchy.get_memory_levels(mem_op, )
+            memory_levels = mem_hierarchy.get_memory_levels(
+                mem_op,
+            )
 
             for memory_level in memory_levels:
                 spatial_mapping_lvl = []
                 served_dimensions = memory_level.served_dimensions
                 for dimension in served_dimensions:
                     dim_name = dimension.name
                     if dim_name in user_sm_copy:
@@ -131,12 +150,15 @@
                         # as the spatial mapping representation is a level-by-level one.
                         del user_sm_copy[dim_name]
                 spatial_mapping_dict[layer_op].append(spatial_mapping_lvl)
 
             # After we have gone through the memory levels, if there are still user-defined dimensions
             # present, add them as the top level. Otherwise add an empty list to make arch levels correct:
             # because first list we added was the operational array level.
-            top_level_spatial_mapping = [spatial_loop for (dim_name, spatial_loop) in user_sm_copy.items()]
+            top_level_spatial_mapping = [
+                spatial_loop for (dim_name, spatial_loop) in user_sm_copy.items()
+            ]
             spatial_mapping_dict[layer_op].append(top_level_spatial_mapping)
 
-        return SpatialMapping(spatial_mapping_dict=spatial_mapping_dict,
-                              layer_node=self.layer)
+        return SpatialMapping(
+            spatial_mapping_dict=spatial_mapping_dict, layer_node=self.layer
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/SpatialMappingGeneratorStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/SpatialMappingGeneratorStage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-import itertools
 import logging
-from typing import Set
-import bisect
 
-from sympy import factorint
-
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.hardware.architecture.core import Core
-from zigzag.classes.hardware.architecture.dimension import Dimension
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.classes.hardware.architecture.operational_array import OperationalArray
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
 from zigzag.classes.opt.spatial.generator import UserSpatialMappingGenerator
 from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.stages.SpatialMappingConversionStage import SpatialMappingConversionStage
-from zigzag.classes.workload.layer_node import LayerNode
+from zigzag.classes.stages.SpatialMappingConversionStage import (
+    SpatialMappingConversionStage,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class SpatialMappingGeneratorStage(Stage):
     """
     Pipeline stage that finds spatial mappings given a:
@@ -28,25 +18,25 @@
     - layer
     The spatial mappings are found using the interconnection pattern present on the core.
     The inner-most memory level served dimensions is used,
     as this is how the memories connect to the operational array.
 
     :param main_inputs: MainInputs, NOT copied
     """
+
     def __init__(self, list_of_callables, *, accelerator, layer, **kwargs):
         """
         Note: list_of_callables does NOT need to include SpatialMappingConversionStage. Although this is used,
         this usage is done automatically.
         """
         super().__init__(list_of_callables, **kwargs)
         self.accelerator = accelerator
         self.check_layer(layer)
         self.layer = layer
 
-
     @staticmethod
     def check_layer(layer):
         """
         Check that the layer includes:
         - the core which it is allocated to
         If not, a ValueError is raised.
         If the layer in main_inputs is not set, False is returned
@@ -61,31 +51,43 @@
 
     def run(self):
         """
         Run this stage by generating user-formatted spatial mappings which are converted
         to the memory-level based spatial mapping representation.
         """
         user_provided_spatial_mappings = self.layer.user_spatial_mapping
-        if isinstance(user_provided_spatial_mappings, dict):  # There is a single USM provided
+        if isinstance(
+            user_provided_spatial_mappings, dict
+        ):  # There is a single USM provided
             user_spatial_mappings = [user_provided_spatial_mappings]
-        elif isinstance(user_provided_spatial_mappings, list):  # There are multiple USMs provided
+        elif isinstance(
+            user_provided_spatial_mappings, list
+        ):  # There are multiple USMs provided
             user_spatial_mappings = user_provided_spatial_mappings
         else:  # There is no USM provided
             # Initialize the UserSpatialMappingGenerator which will automatically generate SMs
-            user_spatial_mapping_generator = UserSpatialMappingGenerator(self.layer, self.accelerator)
+            user_spatial_mapping_generator = UserSpatialMappingGenerator(
+                self.layer, self.accelerator
+            )
             # Get all the USMs by running the generator
-            user_spatial_mappings = list((usm for usm in user_spatial_mapping_generator.run()))
+            user_spatial_mappings = list(
+                (usm for usm in user_spatial_mapping_generator.run())
+            )
             logger.debug(f"No user-provided spatial mappings found. Auto-generating..")
         nb_user_spatial_mappings = len(user_spatial_mappings)
 
         for i, user_spatial_mapping in enumerate(user_spatial_mappings):
-            logger.info(f"Launching spatial mapping {i+1}/{nb_user_spatial_mappings}: {user_spatial_mapping}.")
+            logger.info(
+                f"Launching spatial mapping {i+1}/{nb_user_spatial_mappings}: {user_spatial_mapping}."
+            )
             # Set the user_spatial_mapping in the layer, as this is required by SpatialMappingConversionStage
             self.layer.user_spatial_mapping = user_spatial_mapping
             # Note: manual instantiation of spatial mapping conversion stage here. We let that class deal with
             # everything else, including instantion of the actual substages
-            spatial_mapping_conversion_stage = SpatialMappingConversionStage(self.list_of_callables,
-                                                                             accelerator=self.accelerator,
-                                                                             layer=self.layer,
-                                                                             **self.kwargs)
+            spatial_mapping_conversion_stage = SpatialMappingConversionStage(
+                self.list_of_callables,
+                accelerator=self.accelerator,
+                layer=self.layer,
+                **self.kwargs,
+            )
             for cme, extra_info in spatial_mapping_conversion_stage.run():
                 yield cme, (user_spatial_mapping, extra_info)
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/Stage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/Stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Generator, Callable, List
 
 
 class Stage:
     """Abstract superclass for Runnables"""
-    def __init__(self, list_of_callables:List[Callable], **kwargs):
+
+    def __init__(self, list_of_callables: List[Callable], **kwargs):
         """
         :param list_of_callables: a list of callables, that must have a signature compatible with this __init__ function
         (list_of_callables, *, required_kwarg1, required_kwarg2, kwarg_with_default=default, **kwargs)
         and return a Stage instance. This is used to flexibly build iterators upon other iterators.
         :param kwargs: any keyword arguments, irrelevant to the specific class in question but passed on down
         """
         self.kwargs = kwargs
         self.list_of_callables = list_of_callables
         if self.is_leaf() and list_of_callables not in ([], tuple(), set(), None):
             raise ValueError("Leaf runnable received a non empty list_of_callables")
 
         if list_of_callables in ([], tuple(), set(), None) and not self.is_leaf():
-            raise ValueError("List of callables empty on a non leaf runnable, so nothing can be generated.\
-                              Final callable in list_of_callables must return Stage instances that have is_leaf() == True")
-
-
+            raise ValueError(
+                "List of callables empty on a non leaf runnable, so nothing can be generated.\
+                              Final callable in list_of_callables must return Stage instances that have is_leaf() == True"
+            )
 
     def run(self) -> Generator:
         """Runs the runnable.
         This requires no arguments and returns a generator yielding any amount of tuple, that each have
         a CostModelEvaluation as the first element and a second element that can be anything, meant only for manual
         inspection."""
         raise ImportError("Run function not implemented for runnable")
@@ -35,21 +36,25 @@
         """
         :return: Returns true if the runnable is a leaf runnable, meaning that it does not use (or thus need) any substages
         to be able to yield a result. Final element in list_of_callables must always have is_leaf() == True, except
         for that final element that has an empty list_of_callables
         """
         return False
 
+
 class MainStage:
     """
     Not actually a Stage, as running it does return (not yields!) a list of results instead of a generator
     Can be used as the main entry point
     """
+
     def __init__(self, list_of_callables, **kwargs):
         self.kwargs = kwargs
         self.list_of_callables = list_of_callables
 
     def run(self):
         answers = []
-        for cme, extra_info in self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs).run():
+        for cme, extra_info in self.list_of_callables[0](
+            self.list_of_callables[1:], **self.kwargs
+        ).run():
             answers.append((cme, extra_info))
-        return answers
+        return answers
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/TemporalOrderingConversionStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/TemporalOrderingConversionStage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import logging
 
-import numpy as np
-
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
 from zigzag.classes.opt.temporal.loma.memory_allocator import MemoryAllocator
 from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.workload.layer_node import LayerNode
 
 
 logger = logging.getLogger(__name__)
 
 
 class TemporalOrderingConversionStage(Stage):
-    def __init__(self, list_of_callables, *, accelerator, layer, spatial_mapping, **kwargs):
+    def __init__(
+        self, list_of_callables, *, accelerator, layer, spatial_mapping, **kwargs
+    ):
         """
         Initialize the accelerator and layer attributes.
         :param main_inputs: MainInputs, NOT copied
         """
         super().__init__(list_of_callables, **kwargs)
         self.check_layer(layer)
         self.layer = layer
@@ -36,58 +32,68 @@
         :return: True
         """
         if not layer.core_allocation:
             logger.critical(f"Layer {layer} has no core allocation.")
             raise ValueError()
         if not layer.user_temporal_ordering:
             logger.critical(f"Layer {layer} has no user-defined temporal ordering.")
-            raise ValueError(f"Layer {layer} has no user-defined temporal ordering. Use LomaStage to generate automatically.")
+            raise ValueError(
+                f"Layer {layer} has no user-defined temporal ordering. Use LomaStage to generate automatically."
+            )
 
         return True
 
     def run(self):
         """
         Run this stage by converting the user-defined temporal loop ordering
         to the memory-level based temporal mapping representation.
 
         :param user_spatial_mapping: The user-defined spatial mapping to be converted. If not provided, self.layer.user_spatial_mapping is used.
         """
-        temporal_mapping = self.convert_user_temporal_mapping(self.layer.user_temporal_ordering)
+        temporal_mapping = self.convert_user_temporal_mapping(
+            self.layer.user_temporal_ordering
+        )
         kwargs = self.kwargs.copy()
-        kwargs['temporal_mapping'] = temporal_mapping
-        kwargs['spatial_mapping'] = self.spatial_mapping
-        kwargs['layer'] = self.layer
-        kwargs['accelerator'] = self.accelerator
+        kwargs["temporal_mapping"] = temporal_mapping
+        kwargs["spatial_mapping"] = self.spatial_mapping
+        kwargs["layer"] = self.layer
+        kwargs["accelerator"] = self.accelerator
         substage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
         for cme, extra_info in substage.run():
             yield cme, extra_info
 
     def convert_user_temporal_mapping(self, user_temporal_mapping):
         spatial_mapping = self.spatial_mapping
         layer = self.layer
         layer_dim_sizes = layer.loop_dim_size
         for i, utm in list(enumerate(user_temporal_mapping))[::-1]:
             if utm[0] not in layer_dim_sizes:
-                logger.warning(f"Supplied temporal ordering {utm} for layer {layer} thrown out because loop not present in the layer")
+                logger.warning(
+                    f"Supplied temporal ordering {utm} for layer {layer} thrown out because loop not present in the layer"
+                )
                 del user_temporal_mapping[i]
 
         # I don't think this is actually necessary to check:
         # If a dimension is fully unrolled spatially it doesn't have to be present in temporal ordering.
         # for d in layer_dim_sizes:
         #     if d not in [utm[0] for utm in user_temporal_mapping]:
         #         logger.error(f"Supplied temporal ordering for layer {layer} is missing dimension {d}")
         #         raise ValueError(f"Supplied temporal ordering for layer {layer} is missing dimension {d}")
 
         converted_mapping = []
         for dim, size in user_temporal_mapping:
-            if size == 'all':
+            if size == "all":
                 size = layer_dim_sizes[dim]
                 size_already = 1
-                for dim_already, size_already_sub in converted_mapping + spatial_mapping.spatial_loop_dim_size:
+                for dim_already, size_already_sub in (
+                    converted_mapping + spatial_mapping.spatial_loop_dim_size
+                ):
                     if dim_already == dim:
                         size_already *= size_already_sub
                 size //= size_already
             converted_mapping.append((dim, size))
-        allocator = MemoryAllocator(self.accelerator, layer, spatial_mapping, converted_mapping)
+        allocator = MemoryAllocator(
+            self.accelerator, layer, spatial_mapping, converted_mapping
+        )
 
         temporal_mapping = allocator.run()  # allocate this ordering to the memories
-        return temporal_mapping
+        return temporal_mapping
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/WorkloadStage.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/WorkloadStage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import networkx as nx
 import logging
 
 from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.workload.dnn_workload import DNNWorkload
 from zigzag.classes.workload.dummy_node import DummyNode
 
 
 logger = logging.getLogger(__name__)
 
+
 class WorkloadStage(Stage):
     """
     Class that iterates through the nodes in a given workload graph.
     """
+
     def __init__(self, list_of_callables, *, workload, **kwargs):
         """
         Initialization of self.workload.
         :param main_inputs: MainInputs, NOT copied
         """
         super().__init__(list_of_callables, **kwargs)
         self.workload = workload
 
     def run(self):
         for id, layer in enumerate(nx.topological_sort(self.workload)):
             if type(layer) == DummyNode:
                 continue  # skip the DummyNodes
             kwargs = self.kwargs.copy()
-            kwargs['layer'] = layer
+            kwargs["layer"] = layer
             if layer.name:
                 layer_name = layer.name
             else:
                 layer_name = id
             logger.info(f"Processing layer {layer_name}...")
             sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
             for cme, extra_info in sub_stage.run():
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/stages/__init__.py` & `zigzag-dse-2.3.2/zigzag/classes/stages/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 from .CostModelStage import CostModelStage
 from .DumpStage import DumpStage
 from .PlotTemporalMappingsStage import PlotTemporalMappingsStage
 from .SaveStage import CompleteSaveStage, SimpleSaveStage, PickleSaveStage
 from .GeneralParameterIteratorStage import GeneralParameterIteratorStage
 from .LomaStage import LomaStage
 from .SalsaStage import SalsaStage
-from .MainInputParserStages import AcceleratorParserStage, WorkloadParserStage, WorkloadAndAcceleratorParserStage
+from .MainInputParserStages import AcceleratorParserStage, WorkloadParserStage
 from .ONNXModelParserStage import ONNXModelParserStage
-from .ReduceStages import MinimalEnergyStage, MinimalLatencyStage, MinimalEDPStage, SumStage
-from .RunOptStages import CacheBeforeYieldStage, RemoveExtraInfoStage, MultiProcessingGatherStage, MultiProcessingSpawnStage, SkipIfDumpExistsStage
+from .ReduceStages import (
+    MinimalEnergyStage,
+    MinimalLatencyStage,
+    MinimalEDPStage,
+    SumStage,
+)
+from .RunOptStages import (
+    CacheBeforeYieldStage,
+    RemoveExtraInfoStage,
+    MultiProcessingGatherStage,
+    MultiProcessingSpawnStage,
+    SkipIfDumpExistsStage,
+)
 from .SpatialMappingConversionStage import SpatialMappingConversionStage
 from .SpatialMappingGeneratorStage import SpatialMappingGeneratorStage
 from .Stage import Stage, MainStage
 from .TemporalOrderingConversionStage import TemporalOrderingConversionStage
 from .WorkloadStage import WorkloadStage
 
 """
 Parameter providers: these parameters are provided to substages by the following classes:
- - accelerator: AcceleratorParserStage, WorkloadAndAcceleratorParserStage, DepthFirstStage
- - workload: WorkloadParserStage, WorkloadAndAcceleratorParserStage, DepthFirstStage
+ - accelerator: AcceleratorParserStage, WorkloadAndAcceleratorParserStage
+ - workload: WorkloadParserStage, WorkloadAndAcceleratorParserStage
  - temporal_mapping: LomaStage, TemporalMappingConversionStage
  - spatial_mapping: SpatialMappingGenerationStage, SpatialMappingConversionStage
- - layer: WorkloadStage, DepthFirstStage
+ - layer: WorkloadStage
  - multiprocessing_callback: MultiProcessingGatherStage
  - *:  GeneralParameterIteratorStage: can provide anything
  
 Parameter consumers: these parameters are no longer provided to substages after the following classes
- - accelerator_path: AcceleratorParserStage, WorkloadAndAcceleratorParserStage
- - df_horizontal_caching: DepthFirstStage 
- - df_tilesize_x: DepthFirstStage
- - df_tilesize_y: DepthFirstStage
- - df_vertical_caching: DepthFirstStage
+ - accelerator_path: AcceleratorParserStage
  - dump_filename_pattern: DumpStage
  - plot_filename_pattern: PlotTemporalMappingsStage
  - general_parameter_iterations: GeneralParameterIteratorStage
  - multiprocessing_callback: MultiProcessingSpawnStage
- - workload: DepthFirstStage, WorkloadStage
- - workload_path: WorkloadParserStage, WorkloadAndAcceleratorParserStage
+ - workload: WorkloadStage
+ - workload_path: WorkloadParserStage
  
 Parameters required: these stages require the following parameters:
  - CostModelStage: accelerator, layer, spatial_mapping, temporal_mapping
  - WorkloadStage: workload
- - DepthFirstStage: accelerator, workload, df_tilesize_x, df_tilesize_y, df_horizontal_caching, df_vertical_caching
  - DumpStage: dump_filename_pattern
  - PlotTemporalMappingsStage: plot_filename_pattern
  - GeneralParameterIteratorStage: general_parameter_iterations
  - LomaStage: accelerator, layer, spatial_mapping
  - AcceleratorParserStage: accelerator_path
  - WorkloadParserStage: workload_path
  - WorkloadAndAcceleratorParserStage: workload_path, accelerator_path
  - MultiProcessingSpawnStage: multiprocessing_callback
  - SpatialMappingConversionStage: accelerator, layer
  - SpatialMappingGeneratorStage: accelerator, layer
  - TemporalOrderingConversionStage: accelerator, layer, spatial_mapping
  - SkipIfDumpExistStage: dump_filename_pattern
-"""
+"""
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/workload/dnn_workload.py` & `zigzag-dse-2.3.2/zigzag/classes/workload/dnn_workload.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from zigzag.classes.workload.layer_node import LayerNode
 from typing import Dict, Any
 from networkx import DiGraph
 
 
 class DNNWorkload(DiGraph):
-
     def __init__(self, workload: Dict[Any, Dict], mapping: Dict[Any, Dict], **attr):
         """
         Collect all the algorithmic workload information here.
         :param workload: user-defined workload file (py).
 
         :return (self): Directed Graph with nodes the layers and edges the connections between layers.
         """
@@ -20,37 +19,39 @@
         self.layer_node_list = []
 
         for layer_id, layer in workload.items():
             # TODO Support other type of layers, such as concatenation, max pooling, BN, etc.
             #  What is special about max pooling?
             # elif type(layer_id) == str and layer_id[0:6] == 'concat':
             #     continue
-            if layer['operator_type'] in mapping.keys():
-                for attr_name, attr_va in mapping[layer['operator_type']].items():
+            if layer["operator_type"] in mapping.keys():
+                for attr_name, attr_va in mapping[layer["operator_type"]].items():
                     layer[attr_name] = attr_va
             else:
-                for attr_name, attr_va in mapping['default'].items():
+                for attr_name, attr_va in mapping["default"].items():
                     layer[attr_name] = attr_va
-            '''For each item in the dict generate the LayerNode and add it to the dnn graph G'''
+            """For each item in the dict generate the LayerNode and add it to the dnn graph G"""
             layer_node = LayerNode(layer_id, layer)
-            '''Save this layer_id and LayerNode pair in the layer_id_to_obj dict'''
+            """Save this layer_id and LayerNode pair in the layer_id_to_obj dict"""
             layer_id_to_obj[layer_id] = layer_node
             # self.add_node(layer_id, info=layer_node)
             self.add_node(layer_node)
             self.layer_node_list.append(layer_node)
-            '''Find all of its operand sources and add edges accordingly'''
+            """Find all of its operand sources and add edges accordingly"""
             edges = []
-            for (op, parent_list) in layer.get('operand_source', {}).items():
+            for (op, parent_list) in layer.get("operand_source", {}).items():
                 for parent_id in parent_list:
                     parent_layer = layer_id_to_obj[parent_id]
                     edges.append((parent_layer, layer_node))
                     layer_node.input_operand_source[op] = parent_layer
             self.add_edges_from(edges)
 
     def topological_sort(self):
         return nx.topological_sort(self)
 
     def get_node_with_id(self, id):
         for node in self.nodes:
             if node.id == id:
                 return node
-        raise ValueError("DNNWorkload instance does not have a node with the requested id")
+        raise ValueError(
+            "DNNWorkload instance does not have a node with the requested id"
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/workload/dummy_node.py` & `zigzag-dse-2.3.2/zigzag/classes/workload/dummy_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 class DummyNode:
     """
     A class to represent an ONNX node that is not "accelerateable".
     This node is created to preserve the original ONNX model graph structure,
     but will be skipped by the underlying engines, treating it as a 0 HW cost node.
     """
+
     def __init__(self, id, preds, node_name="", type=None) -> None:
         """Initialize the DummyNode by setting its id, the node's predecessors and optionally giving it a name.
 
         Args:
             id (int): id for this node
             preds (list): list of ids of this node's predecessor nodes
             node_name (str, optional): a name for this node, e.g. the node's name within the onnx model
         """
         self.id = id
-        self.input_operand_source = {'I': preds}
+        self.input_operand_source = {"I": preds}
         self.name = node_name
         self.type = type
-        self.core_allocation = -1  # We assume these nodes are mapped on a core with id -1
+        self.core_allocation = (
+            -1
+        )  # We assume these nodes are mapped on a core with id -1
         self.runtime = 0
         self.start = None
         self.end = None
 
     def __str__(self):
         return f"DummyNode({self.id})"
 
@@ -46,29 +49,27 @@
 
         Args:
             end (int): end time in cycles
         """
         self.end = end
 
     def get_start(self):
-        """Get the start time in cycles of this node.
-        """
+        """Get the start time in cycles of this node."""
         return self.start
-    
+
     def get_end(self):
-        """Get the end time in cycles of this node.
-        """
+        """Get the end time in cycles of this node."""
         return self.end
 
     def get_runtime(self):
         """
         Return the runtime of running this node.
         """
         return self.runtime
 
     def has_end(self) -> bool:
         """Check if this node has already been assigned an end time.
 
         Returns:
             bool: True if this node has been assigned an end time
         """
-        return self.end is not None
+        return self.end is not None
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/workload/layer_node.py` & `zigzag-dse-2.3.2/zigzag/classes/workload/layer_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from math import gcd, prod
 import re
 from collections import defaultdict
 from typing import Dict, List
 from copy import deepcopy
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 from collections import defaultdict
 
-class LayerNode:
 
+class LayerNode:
     def __init__(self, layer_id, layer_attrs, node_name="", type=None):
         """
         To construct each layer node, algorithm equation/dimension/indirect relation are parsed.
         This parser collects information of operand, loop dimension, and loop relevance.
         Equal-to-1 loop dimensions are eliminated.
 
         :param layer_id: The identifier (key) of the layer, as defined in the workload
@@ -50,306 +49,381 @@
         self.id = layer_id
         self.layer_attrs = layer_attrs
         self.name = node_name
         self.type = type
 
         # equation_relations has been replaced by dimension_relations.
         # Check if layer has equation_relations and notify user.
-        if 'equation_relations' in layer_attrs:
-            raise ValueError(f"Please replace equation_relations by dimension_relations for layer {self}.")
-
-        '''Get required attributes from layer_attrs'''
-        equation: str = layer_attrs.get('equation')
-        loop_dim_size: Dict[str, int] = layer_attrs.get('loop_dim_size')
-        pr_loop_dim_size: Dict[str, int] = layer_attrs.get('pr_loop_dim_size', None)
-        operand_precision: Dict[str, int] = layer_attrs.get('operand_precision')
-        dimension_relations: List[str] = layer_attrs.get('dimension_relations', [])
-        user_spatial_mapping: Dict[str, tuple] = layer_attrs.get('spatial_mapping', None)
-        user_temporal_ordering = layer_attrs.get('temporal_ordering', None)
-        core_allocation: int = layer_attrs.get('core_allocation', None)
-        memory_operand_links: Dict[str, str] = layer_attrs.get('memory_operand_links', None)
-        source_storage_level: int = layer_attrs.get('source_storage_level', {})
-        operand_source_dimension_mapping: Dict[Dict[str, str]] = layer_attrs.get('operand_source_dimension_mapping', {})
-        constant_operands: List[str] = layer_attrs.get('constant_operands', [])
-        input_operand_source: Dict[str, list] = layer_attrs.get('operand_source', dict())
+        if "equation_relations" in layer_attrs:
+            raise ValueError(
+                f"Please replace equation_relations by dimension_relations for layer {self}."
+            )
+
+        """Get required attributes from layer_attrs"""
+        equation: str = layer_attrs.get("equation")
+        loop_dim_size: Dict[str, int] = layer_attrs.get("loop_dim_size")
+        pr_loop_dim_size: Dict[str, int] = layer_attrs.get("pr_loop_dim_size", None)
+        operand_precision: Dict[str, int] = layer_attrs.get("operand_precision")
+        dimension_relations: List[str] = layer_attrs.get("dimension_relations", [])
+        user_spatial_mapping: Dict[str, tuple] = layer_attrs.get(
+            "spatial_mapping", None
+        )
+        user_temporal_ordering = layer_attrs.get("temporal_ordering", None)
+        core_allocation: int = layer_attrs.get("core_allocation", None)
+        memory_operand_links: Dict[str, str] = layer_attrs.get(
+            "memory_operand_links", None
+        )
+        source_storage_level: int = layer_attrs.get("source_storage_level", {})
+        operand_source_dimension_mapping: Dict[Dict[str, str]] = layer_attrs.get(
+            "operand_source_dimension_mapping", {}
+        )
+        constant_operands: List[str] = layer_attrs.get("constant_operands", [])
+        input_operand_source: Dict[str, list] = layer_attrs.get(
+            "operand_source", dict()
+        )
         # Save the padding for different tensor dimensions
-        padding: Dict[str, tuple] = layer_attrs.get('padding', {})  # Empty dict signals no padding in any dimension
+        padding: Dict[str, tuple] = layer_attrs.get(
+            "padding", {}
+        )  # Empty dict signals no padding in any dimension
 
         self.equation = equation
-        self.loop_dim_size = dict(item for item in tuple(loop_dim_size.items()))  # if item[1] != 1)
+        self.loop_dim_size = dict(
+            item for item in tuple(loop_dim_size.items())
+        )  # if item[1] != 1)
         self.pr_loop_dim_size = pr_loop_dim_size
         self.operand_precision = operand_precision
         self.dimension_relations = dimension_relations
         self.loop_dim_list = list(loop_dim_size.keys())
         self.user_spatial_mapping = user_spatial_mapping
         self.user_temporal_ordering = user_temporal_ordering
         self.core_allocation = core_allocation
         self.memory_operand_links = memory_operand_links.copy()
         self.source_storage_level = source_storage_level
         self.operand_source_dimension_mapping = operand_source_dimension_mapping
         self.constant_operands = constant_operands
         self.padding = padding
 
-        ''' Step1: extract partially-relevant data dimension and its relation to loop dimensions. '''
+        """ Step1: extract partially-relevant data dimension and its relation to loop dimensions. """
         pr_loop, pr_loop_list, pr_scaling_factors = self.build_pr_funcs()
         self.pr_loop = pr_loop
         self.pr_scaling_factors = pr_scaling_factors
         if not self.pr_loop_dim_size:
-            self.pr_loop_dim_size = {dim: self.calc_pr_dimension_size_total(dim) for dim in pr_loop}
-
-        ''' Step2: extract relevant and irrelevant loop dimensions. '''
-        operand_loop_dim, operand_loop_dim_reform, operand_list, operand_dimensionality_order = \
-            self.extract_r_ir_loop_info(equation, loop_dim_size, pr_loop, pr_loop_list)
+            self.pr_loop_dim_size = {
+                dim: self.calc_pr_dimension_size_total(dim) for dim in pr_loop
+            }
+
+        """ Step2: extract relevant and irrelevant loop dimensions. """
+        (
+            operand_loop_dim,
+            operand_loop_dim_reform,
+            operand_list,
+            operand_dimensionality_order,
+        ) = self.extract_r_ir_loop_info(equation, loop_dim_size, pr_loop, pr_loop_list)
         self.operand_loop_dim = operand_loop_dim
         self.operand_loop_dim_reform = operand_loop_dim_reform
         self.output_operand = operand_list[0]
         self.input_operands = operand_list[1:]
         self.operand_list = operand_list
         self.input_operand_source = input_operand_source
         self.operand_dimensionality_order = operand_dimensionality_order
 
         # Save the variable (non-constant) input operands
-        self.variable_input_operands: list = [op for op in self.input_operands if op not in self.constant_operands]
+        self.variable_input_operands: list = [
+            op for op in self.input_operands if op not in self.constant_operands
+        ]
         # Save the way an operand's tensor should be reshaped for interaction with other nodes.
-        self.operand_tensor_reshape: Dict[str, list] = layer_attrs.get('operand_tensor_reshape',  {op: [] for op in self.operand_list})
+        self.operand_tensor_reshape: Dict[str, list] = layer_attrs.get(
+            "operand_tensor_reshape", {op: [] for op in self.operand_list}
+        )
 
-        ''' Step3: extract layer info, e.g. total operand size, total operand data reuse, total MAC operation, etc. '''
+        """ Step3: extract layer info, e.g. total operand size, total operand data reuse, total MAC operation, etc. """
         self.extract_layer_info()
 
-
     def build_pr_funcs(self):
         # 1 long dimensions are removed in self.loop_dim_size but required in extract_pr_loop_info
         loop_dim_size = defaultdict(lambda: 1)
         loop_dim_size.update(self.loop_dim_size)
         if self.dimension_relations:
-            pr_loop, pr_loop_list, pr_scaling_factors = self.extract_pr_loop_info(self.dimension_relations)
+            pr_loop, pr_loop_list, pr_scaling_factors = self.extract_pr_loop_info(
+                self.dimension_relations
+            )
         else:
             pr_loop, pr_loop_list, pr_scaling_factors = {}, [], {}
 
         return pr_loop, pr_loop_list, pr_scaling_factors
 
     def get_core_allocation(self):
         return self.core_allocation
 
     def __str__(self):
         return f"LayerNode_{self.id}"
 
     def __repr__(self):
         return str(self)
-    
+
     def __jsonrepr__(self):
         """
         JSON representation used for saving this object to a json file.
         """
-        return {"equation": self.equation,
-                "equation_relations": self.dimension_relations,
-                "loop_dimensions": self.loop_dim_size,
-                "operand_precision": self.operand_precision,
-                "core_allocation": self.core_allocation,
-                "user_spatial_mapping": self.user_spatial_mapping,
-                "memory_operand_links": self.memory_operand_links,
-                "source_storage_level": self.source_storage_level}
+        return {
+            "equation": self.equation,
+            "equation_relations": self.dimension_relations,
+            "loop_dimensions": self.loop_dim_size,
+            "operand_precision": self.operand_precision,
+            "core_allocation": self.core_allocation,
+            "user_spatial_mapping": self.user_spatial_mapping,
+            "memory_operand_links": self.memory_operand_links,
+            "source_storage_level": self.source_storage_level,
+        }
 
     def calc_tensor_size(self, layer_op, loop_sizes):
         """
         Calculates the tensor size (nb of elements) for the given operand layer_op with the given loop dimension sizes loop_sizes.
         :param layer_op: str. A String representing the layer operand for which to compute the tensor size.
         :param loop_sizes: dict. A dict with string keys representing the dimension and integer values representing the size.
         """
         return prod(self.calc_tensor_dims(layer_op, loop_sizes).values())
         # Initialize the tensor size as 1
 
     def calc_tensor_dim(self, loop_sizes, dim):
         if dim in loop_sizes:
             return loop_sizes[dim]
         elif dim in self.pr_loop:
-            related_dimension_sizes = [loop_sizes[dimension] for dimension in self.pr_loop[dim]]
+            related_dimension_sizes = [
+                loop_sizes[dimension] for dimension in self.pr_loop[dim]
+            ]
             scaling_factors = list(self.pr_scaling_factors[dim].values())
-            assert len(related_dimension_sizes) == len(scaling_factors) == 2, "Shouldn't happen if partial relevancy checks in extract_pr_loop_info() are done correctly."
-            args = (val for pair in zip(scaling_factors, related_dimension_sizes) for val in pair)
+            assert (
+                len(related_dimension_sizes) == len(scaling_factors) == 2
+            ), "Shouldn't happen if partial relevancy checks in extract_pr_loop_info() are done correctly."
+            args = (
+                val
+                for pair in zip(scaling_factors, related_dimension_sizes)
+                for val in pair
+            )
             pr_dim_size = self.calc_pr_dimension_size(*args)
             # Clip this to the largest possible size for this partially relevant dimension (computed at initialization based on padding)
             pr_dim_size = min(self.pr_loop_dim_size[dim], pr_dim_size)
             return pr_dim_size
         elif dim in self.loop_dim_size:
-            assert self.loop_dim_size[dim] == 1, "This line should only be reached when the dim has a size of 1 in the layer."
+            assert (
+                self.loop_dim_size[dim] == 1
+            ), "This line should only be reached when the dim has a size of 1 in the layer."
             return 1
         else:
-            raise ValueError("Something went wrong in the initialization of the layer, or in the caller function.")
+            raise ValueError(
+                "Something went wrong in the initialization of the layer, or in the caller function."
+            )
 
     def calc_tensor_dims(self, layer_op, loop_sizes):
         out = {}
         op_dimensions = self.operand_loop_dim[layer_op]
-        for dim in op_dimensions['r'] + list(op_dimensions['pr'].keys()):
+        for dim in op_dimensions["r"] + list(op_dimensions["pr"].keys()):
             out[dim] = self.calc_tensor_dim(loop_sizes, dim)
         return out
 
     def calc_pr_dimension_size_total(self, dim):
         """Compute the total pr dimension size of this node, taking padding into account.
 
         Args:
             dim (str): The partially relevant dimension, e.g. 'IX'.
 
         Returns:
             int: The total partially relevant dimension size
         """
-        related_dimension_sizes = [self.loop_dim_size[related_dim] for related_dim in self.pr_loop[dim]]
-        scaling_factors = list(self.pr_scaling_factors[dim].values())  # assumes this dict is ordered
-        assert len(related_dimension_sizes) == len(scaling_factors) == 2, "Shouldn't happen if partial relevancy checks in extract_pr_loop_info() are done correctly."
-        args = (val for pair in zip(scaling_factors, related_dimension_sizes) for val in pair)
+        related_dimension_sizes = [
+            self.loop_dim_size[related_dim] for related_dim in self.pr_loop[dim]
+        ]
+        scaling_factors = list(
+            self.pr_scaling_factors[dim].values()
+        )  # assumes this dict is ordered
+        assert (
+            len(related_dimension_sizes) == len(scaling_factors) == 2
+        ), "Shouldn't happen if partial relevancy checks in extract_pr_loop_info() are done correctly."
+        args = (
+            val
+            for pair in zip(scaling_factors, related_dimension_sizes)
+            for val in pair
+        )
         total_pr_dim_size = self.calc_pr_dimension_size(*args)
         # Partially relevant loop dimensions can also have padding, so get the padding for this pr dimension and subtract
         padding = self.padding.get(dim, (0, 0))  # default = (0, 0)
         total_pr_dim_size_without_padding = int(total_pr_dim_size - sum(padding))
         return total_pr_dim_size_without_padding
 
-
     @staticmethod
     def calc_pr_dimension_size(sa, A, sb, B):
         """
         Calculates the number of unique indices c generated by iterating through the indices
         a in range(0,A,1) and b in range(0,B,1) according to the equation c = sa * a + sb * b.
         sa and sb thus represent the scaling of a, resp. b.
         """
-        return int(A*B - max(0, B - (sa/gcd(sa,sb))) * (A - (sb/gcd(sa,sb))))
-
+        return int(A * B - max(0, B - (sa / gcd(sa, sb))) * (A - (sb / gcd(sa, sb))))
 
     @staticmethod
     def return_lambda(equal_sign_right):
         return eval("lambda n: " + equal_sign_right)
 
     def extract_pr_loop_info(self, equation_relations):
         pr_loop: Dict[str, list] = {}
         pr_loop_list: List[str] = []
         pr_scaling_factors: Dict[str, list] = {}
         padding: Dict[str, int] = {}
         for relation in equation_relations:
-            relation_disassembly = re.findall('[a-zA-Z]+', relation)
-            
-            assert len(relation_disassembly) == 3, f"equation_relation {relation} does not involve a linear relationship between two dimension iterators."
-            
+            relation_disassembly = re.findall("[a-zA-Z]+", relation)
+
+            assert (
+                len(relation_disassembly) == 3
+            ), f"equation_relation {relation} does not involve a linear relationship between two dimension iterators."
+
             key = relation_disassembly[0].upper()
             val = [loop_dim.upper() for loop_dim in relation_disassembly[1:]]
             pr_loop[key] = val
             pr_loop_list.extend([key] + val)
 
             # To extract the scaling factors for the different loop dimension iterators, we need to make sure
             # there is a scaling factor present in the equation. If it is not present, raise an exception.
             scaling_factors = {}
             for val_lower in relation_disassembly[1:]:
-                if relation[relation.index(val_lower)-1] == '*':
-                    if not relation[relation.index(val_lower)-2].isdigit():
-                        raise NotImplementedError(f"Please use a scaling factor for every dimension iterator on the RHS of equation {relation}")
+                if relation[relation.index(val_lower) - 1] == "*":
+                    if not relation[relation.index(val_lower) - 2].isdigit():
+                        raise NotImplementedError(
+                            f"Please use a scaling factor for every dimension iterator on the RHS of equation {relation}"
+                        )
                     else:
-                        scaling_factors[val_lower] = int(re.findall('(\\d+)(?=\\*'+val_lower+')', relation)[0])
+                        scaling_factors[val_lower] = int(
+                            re.findall("(\\d+)(?=\\*" + val_lower + ")", relation)[0]
+                        )
                 else:
                     scaling_factors[val_lower] = 1
-            #scaling_factors = re.findall('[0-9]+', relation)
-            assert len(scaling_factors) == 2, f"Please remove any constants in the equation relation {relation}."
+            # scaling_factors = re.findall('[0-9]+', relation)
+            assert (
+                len(scaling_factors) == 2
+            ), f"Please remove any constants in the equation relation {relation}."
             pr_scaling_factors[key] = scaling_factors
 
         return pr_loop, pr_loop_list, pr_scaling_factors
 
     @staticmethod
     def extract_r_ir_loop_info(equation, loop_dim_size, pr_loop, pr_loop_list):
         operand_loop_dim: Dict[str, Dict] = {}
         operand_list = []
-        equation = equation.replace('*', ' * ')
-        equation = equation.replace('=', ' = ')
-        equation = equation.replace('+', ' + ')
-        equation_disassembly = re.findall('[a-zA-Z,0-9,=,*,+]+', equation)
+        equation = equation.replace("*", " * ")
+        equation = equation.replace("=", " = ")
+        equation = equation.replace("+", " + ")
+        equation_disassembly = re.findall("[a-zA-Z,0-9,=,*,+]+", equation)
         # filter out + that directly precedes an = (+=) or another + (++) to make this work for concat and add
         prev_char = None
         for i, char in enumerate(equation_disassembly):
-            if (char == '=' or char == '+') and prev_char == '+':
-                equation_disassembly.pop(i-1)
+            if (char == "=" or char == "+") and prev_char == "+":
+                equation_disassembly.pop(i - 1)
             prev_char = char
-        split_location = [i for (i, x) in enumerate(equation_disassembly) if x in ['=', '*', '+']] + [
-            len(equation_disassembly)]
+        split_location = [
+            i for (i, x) in enumerate(equation_disassembly) if x in ["=", "*", "+"]
+        ] + [len(equation_disassembly)]
         dimension_list = list(loop_dim_size.keys())
         begin_idx = 0
         operand_dimensionality_order = {}
         for split_loc in split_location:
             operand = equation_disassembly[begin_idx]
             operand_list.append(operand)
             operand_loop_dim[operand] = {}
-            r_loop_list = [loop_dim.upper() for loop_dim in equation_disassembly[begin_idx + 1:split_loc]]
+            r_loop_list = [
+                loop_dim.upper()
+                for loop_dim in equation_disassembly[begin_idx + 1 : split_loc]
+            ]
             ir_loop_list = list(set(dimension_list).difference(r_loop_list))
 
-            pr_loop_remove_flag = any(loop in list(pr_loop.keys()) for loop in r_loop_list)
+            pr_loop_remove_flag = any(
+                loop in list(pr_loop.keys()) for loop in r_loop_list
+            )
             if pr_loop_remove_flag:
-                operand_loop_dim[operand]['r'] = [loop for loop in r_loop_list if
-                                                  loop not in pr_loop_list] #  and loop_dim_size[loop] != 1]
-                operand_loop_dim[operand]['ir'] = [loop for loop in ir_loop_list if
-                                                   loop not in pr_loop_list and loop_dim_size[loop] != 1]
-                operand_loop_dim[operand]['pr'] = pr_loop
+                operand_loop_dim[operand]["r"] = [
+                    loop for loop in r_loop_list if loop not in pr_loop_list
+                ]  #  and loop_dim_size[loop] != 1]
+                operand_loop_dim[operand]["ir"] = [
+                    loop
+                    for loop in ir_loop_list
+                    if loop not in pr_loop_list and loop_dim_size[loop] != 1
+                ]
+                operand_loop_dim[operand]["pr"] = pr_loop
             else:
-                operand_loop_dim[operand]['r'] = [loop for loop in r_loop_list if loop_dim_size[loop] != 1]
-                operand_loop_dim[operand]['ir'] = [loop for loop in ir_loop_list if loop_dim_size[loop] != 1]
-                operand_loop_dim[operand]['pr'] = {}
+                operand_loop_dim[operand]["r"] = [
+                    loop for loop in r_loop_list if loop_dim_size[loop] != 1
+                ]
+                operand_loop_dim[operand]["ir"] = [
+                    loop for loop in ir_loop_list if loop_dim_size[loop] != 1
+                ]
+                operand_loop_dim[operand]["pr"] = {}
             begin_idx = split_loc + 1
 
             # Add the dimensionality order of all relevant (including partially relevant) dimensions of this operand
             operand_dimensionality_order[operand] = r_loop_list
 
-        ''' operand_loop_dim_reform remove the pr loop dict, and put the pr-related data dimension (e.g. IX and IY)
-         to r and ir dict with "_r" and "_ir" suffix. It brings benefits to loop info extraction after pr loop decoupling step. '''
+        """ operand_loop_dim_reform remove the pr loop dict, and put the pr-related data dimension (e.g. IX and IY)
+         to r and ir dict with "_r" and "_ir" suffix. It brings benefits to loop info extraction after pr loop decoupling step. """
         operand_loop_dim_reform = deepcopy(operand_loop_dim)
         for operand, dic in operand_loop_dim.items():
-            del operand_loop_dim_reform[operand]['pr']
-            if dic['pr'] != {}:
-                r_extend_list = [pr_data_dim+'_r' for pr_data_dim in pr_loop.keys()]
-                ir_extend_list = [pr_data_dim+'_ir' for pr_data_dim in pr_loop.keys()]
-                operand_loop_dim_reform[operand]['r'] += r_extend_list
-                operand_loop_dim_reform[operand]['ir'] += ir_extend_list
+            del operand_loop_dim_reform[operand]["pr"]
+            if dic["pr"] != {}:
+                r_extend_list = [pr_data_dim + "_r" for pr_data_dim in pr_loop.keys()]
+                ir_extend_list = [pr_data_dim + "_ir" for pr_data_dim in pr_loop.keys()]
+                operand_loop_dim_reform[operand]["r"] += r_extend_list
+                operand_loop_dim_reform[operand]["ir"] += ir_extend_list
+
+        return (
+            operand_loop_dim,
+            operand_loop_dim_reform,
+            operand_list,
+            operand_dimensionality_order,
+        )
 
-        return operand_loop_dim, operand_loop_dim_reform, operand_list, operand_dimensionality_order
-
-  
     def extract_layer_info(self):
         """
         This function extract basic information for each layer node.
         :return: total_MAC_count, operand_size_elem, operand_size_bit, operand_data_reuse.
         """
 
-        ''' total MAC operation count '''
+        """ total MAC operation count """
         total_MAC_count: int = 1
         for ky in self.loop_dim_size:
             total_MAC_count *= self.loop_dim_size[ky]
         self.total_MAC_count = total_MAC_count
 
-        ''' each operand's size (Unit: # of data element) '''
+        """ each operand's size (Unit: # of data element) """
         operand_size_elem: Dict[str, int] = {}
         for operand, relevancy in self.operand_loop_dim.items():
             operand_size_elem[operand] = 1
-            for r_loop in relevancy['r']:
+            for r_loop in relevancy["r"]:
                 operand_size_elem[operand] *= self.loop_dim_size[r_loop]
-            for pr_loop, pr_loop_collect in relevancy['pr'].items():
-                multiply_factor = self.calc_tensor_dims(operand, self.loop_dim_size)[pr_loop]
+            for pr_loop, pr_loop_collect in relevancy["pr"].items():
+                multiply_factor = self.calc_tensor_dims(operand, self.loop_dim_size)[
+                    pr_loop
+                ]
                 operand_size_elem[operand] *= multiply_factor
         self.operand_size_elem = operand_size_elem
 
-        ''' each operand's size (Unit: bit) '''
+        """ each operand's size (Unit: bit) """
         operand_size_bit: Dict[str, int] = {}
         for operand, size_in_elem in operand_size_elem.items():
             operand_size_bit[operand] = size_in_elem * self.operand_precision[operand]
         self.operand_size_bit = operand_size_bit
 
-        ''' each operand's total data reuse factor, which is total MAC Op/total operand size (in element), 
-        i.e. each data element can be used to support how many MAC operation. '''
+        """ each operand's total data reuse factor, which is total MAC Op/total operand size (in element), 
+        i.e. each data element can be used to support how many MAC operation. """
         operand_data_reuse: Dict[str, float] = {}
         for operand, size_in_elem in operand_size_elem.items():
-            operand_data_reuse[operand] = total_MAC_count/size_in_elem
+            operand_data_reuse[operand] = total_MAC_count / size_in_elem
         self.operand_data_reuse = operand_data_reuse
 
     def get_operand_irrelevant_dimensions(self, layer_op: str):
         """
         Return the irrelevant dimensions of layer operand 'layer_op'.
         """
-        return self.operand_loop_dim[layer_op]['ir']
+        return self.operand_loop_dim[layer_op]["ir"]
 
     def get_layer_operand(self, mem_op: str) -> str:
         """
         Return the layer operand associated with the given memory operand for this layer.
         If there is no such memory operand, an error is raised.
         """
         for layer_operand, memory_operand in self.memory_operand_links.items():
@@ -363,18 +437,25 @@
         If this layer node has no information for the given operand, it returns None.
         """
         if layer_op not in self.source_storage_level:
             return None
         return self.source_storage_level[layer_op]
 
 
-
-
 if __name__ == "__main__":
 
-    equation = 'O[g][b][k][oy][ox]+=W[g][k][c][fy][fx]*I[g][b][c][ix][iy]'
-    dimension_size = {'B': 1, 'K': 32, 'C': 64, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3, 'G': 2}
-    operand_precision = {'O': 24, 'O_final': 24, 'W': 8, 'I': 8}
-    equation_relations = ['ix=ox+fx-1', 'iy=oy+fy-1']
+    equation = "O[g][b][k][oy][ox]+=W[g][k][c][fy][fx]*I[g][b][c][ix][iy]"
+    dimension_size = {
+        "B": 1,
+        "K": 32,
+        "C": 64,
+        "OY": 28,
+        "OX": 28,
+        "FY": 3,
+        "FX": 3,
+        "G": 2,
+    }
+    operand_precision = {"O": 24, "O_final": 24, "W": 8, "I": 8}
+    equation_relations = ["ix=ox+fx-1", "iy=oy+fy-1"]
 
     aa = LayerNode(equation, dimension_size, operand_precision, equation_relations)
-    a=1
+    a = 1
```

### Comparing `zigzag-dse-2.3.1/zigzag/classes/workload/onnx_workload.py` & `zigzag-dse-2.3.2/zigzag/classes/workload/onnx_workload.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from zigzag.classes.workload.layer_node import LayerNode
 from typing import Dict, Any
 from networkx import DiGraph
 
 
 class ONNXWorkload(DiGraph):
-
     def __init__(self, **attr):
         """
         Collect all the algorithmic workload information here.
         :param workload: user-defined workload file (py).
 
         :return (self): Directed Graph with nodes the layers and edges the connections between layers.
         """
@@ -39,11 +38,10 @@
     def topological_sort(self):
         return nx.topological_sort(self)
 
     def get_node_with_id(self, id):
         for node in self.nodes:
             if node.id == id:
                 return node
-        raise ValueError("DNNWorkload instance does not have a node with the requested id")
-
-
-
+        raise ValueError(
+            "DNNWorkload instance does not have a node with the requested id"
+        )
```

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Ascend_like.py` & `zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,132 +6,237 @@
 from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.hardware.architecture.core import Core
 
 
 def memory_hierarchy_dut(multiplier_array):
     """Memory hierarchy variables"""
-    ''' size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) '''
+    """ size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) """
 
-    reg_W1 = MemoryInstance(name="rf_1B", size=8, r_bw=8, w_bw=8, r_cost=0.01, w_cost=0.01, area=0,
-                            r_port=1, w_port=1, rw_port=0, latency=1)
-
-    reg_O1 = MemoryInstance(name="rf_2B", size=16, r_bw=16, w_bw=16, r_cost=0.02, w_cost=0.02, area=0,
-                            r_port=2, w_port=2, rw_port=0, latency=1)
+    reg_W1 = MemoryInstance(
+        name="rf_1B",
+        size=8,
+        r_bw=8,
+        w_bw=8,
+        r_cost=0.01,
+        w_cost=0.01,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+    )
+
+    reg_O4 = MemoryInstance(
+        name="rf_4B",
+        size=32,
+        r_bw=16,
+        w_bw=16,
+        r_cost=0.022,
+        w_cost=0.022,
+        area=0,
+        r_port=2,
+        w_port=2,
+        rw_port=0,
+        latency=1,
+    )
 
     ##################################### on-chip memory hierarchy building blocks #####################################
 
-    sram_64KB_with_8_8K_64_1r_1w_I = \
-        MemoryInstance(name="sram_64KB_I", size=8192 * 8, r_bw=64 * 8, w_bw=64 * 8, r_cost=3.32 * 8, w_cost=3.84 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_64KB_with_8_8K_256_1r_1w_W = \
-        MemoryInstance(name="sram_64KB_W", size=8192 * 8, r_bw=256 * 8, w_bw=256 * 8, r_cost=6.27 * 8, w_cost=13.5 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_256KB_with_8_32KB_256_1r_1w_O = \
-        MemoryInstance(name="sram_256KB_O", size=32768 * 8 * 8, r_bw=256 * 8, w_bw=256 * 8, r_cost=15.4 * 8, w_cost=26.6 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_256KB_with_8_32KB_256_1r_1w_O_staging = \
-        MemoryInstance(name="sram_256KB_O_staging", size=32768 * 8 * 8 + 1, r_bw=256 * 8, w_bw=256 * 8, r_cost=15.4 * 8, w_cost=26.6 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_1M_with_8_128K_bank_128_1r_1w_A = \
-        MemoryInstance(name="sram_1MB_A", size=131072 * 8 * 8, r_bw=512 * 8, w_bw=512 * 8, r_cost=58.2 * 8, w_cost=103.2 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_1M_with_8_128K_bank_128_1r_1w_W = \
-        MemoryInstance(name="sram_1MB_W", size=131072 * 8 * 8, r_bw=512 * 8, w_bw=512 * 8, r_cost=58.2 * 8, w_cost=103.2 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
+    sram_1KB_256_1r_1w_I = MemoryInstance(
+        name="sram_1KB_I",
+        size=1024 * 8,
+        r_bw=256,
+        w_bw=256,
+        r_cost=4.78,
+        w_cost=5.59,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_1KB_256_1r_1w_W = MemoryInstance(
+        name="sram_1KB_W",
+        size=1024 * 8,
+        r_bw=256,
+        w_bw=256,
+        r_cost=4.78,
+        w_cost=5.59,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_1M_with_8_128K_bank_128_1r_1w_A = MemoryInstance(
+        name="sram_1MB_A",
+        size=131072 * 8 * 8,
+        r_bw=128 * 8,
+        w_bw=128 * 8,
+        r_cost=26.01 * 8,
+        w_cost=23.65 * 8,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_1M_with_8_128K_bank_128_1r_1w_W = MemoryInstance(
+        name="sram_1MB_W",
+        size=131072 * 8 * 8,
+        r_bw=128 * 8,
+        w_bw=128 * 8,
+        r_cost=26.01 * 8,
+        w_cost=23.65 * 8,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
 
     #######################################################################################################################
 
-    dram = MemoryInstance(name="dram", size=10000000000, r_bw=64, w_bw=64, r_cost=700, w_cost=750, area=0,
-                          r_port=0, w_port=0, rw_port=1, latency=1)
+    dram = MemoryInstance(
+        name="dram",
+        size=10000000000,
+        r_bw=64,
+        w_bw=64,
+        r_cost=700,
+        w_cost=750,
+        area=0,
+        r_port=0,
+        w_port=0,
+        rw_port=1,
+        latency=1,
+    )
 
     memory_hierarchy_graph = MemoryHierarchy(operational_array=multiplier_array)
 
-    '''
+    """
     fh: from high = wr_in_by_high 
     fl: from low = wr_in_by_low 
     th: to high = rd_out_to_high
     tl: to low = rd_out_to_low
-    '''
+    """
     # we don't have unrolled I-Reg to better support G unrolling
     # memory_hierarchy_graph.add_memory(memory_instance=reg_IW1, operands=('I1',),
     #                                   port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
     #                                   served_dimensions={(0, 0, 0, 0)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_W1, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions={(0, 0, 1, 0), (0, 0, 0, 1)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_O1, operands=('O',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_2', 'th': 'r_port_2'},),
-                                      served_dimensions={(0, 1, 0, 0)})
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_W1,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions={(0, 1, 0), (0, 0, 1)},
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_O4,
+        operands=("O",),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_2", "th": "r_port_2"},
+        ),
+        served_dimensions={(0, 0, 0)},
+    )
 
     ##################################### on-chip highest memory hierarchy initialization #####################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=sram_64KB_with_8_8K_256_1r_1w_W, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-
-    memory_hierarchy_graph.add_memory(memory_instance=sram_64KB_with_8_8K_64_1r_1w_I, operands=('I1',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-
-    memory_hierarchy_graph.add_memory(memory_instance=sram_256KB_with_8_32KB_256_1r_1w_O, operands=('O',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'},),
-                                      served_dimensions='all')
-
-    # memory_hierarchy_graph.add_memory(memory_instance=sram_256KB_with_8_32KB_256_1r_1w_O_staging, operands=('O',),
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1KB_256_1r_1w_I,
+        operands=("I1",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1KB_256_1r_1w_W,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    # memory_hierarchy_graph.add_memory(memory_instance=sram_2KB_with_2_1KB_256_1r_1w, operands=('O',),
     #                                   port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'},),
     #                                   served_dimensions='all')
 
-    memory_hierarchy_graph.add_memory(memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_W, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_A, operands=('I1', 'O'),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_W,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_A,
+        operands=("I1", "O"),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_1", "th": "r_port_1"},
+        ),
+        served_dimensions="all",
+    )
 
     ####################################################################################################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=dram, operands=('I1', 'I2', 'O'),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': 'rw_port_1', 'th': 'rw_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=dram,
+        operands=("I1", "I2", "O"),
+        port_alloc=(
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {
+                "fh": "rw_port_1",
+                "tl": "rw_port_1",
+                "fl": "rw_port_1",
+                "th": "rw_port_1",
+            },
+        ),
+        served_dimensions="all",
+    )
+
+    from zigzag.visualization.graph.memory_hierarchy import (
+        visualize_memory_hierarchy_graph,
+    )
 
-    from zigzag.visualization.graph.memory_hierarchy import visualize_memory_hierarchy_graph
     # visualize_memory_hierarchy_graph(memory_hierarchy_graph)
     return memory_hierarchy_graph
 
 
 def multiplier_array_dut():
-    """ Multiplier array variables """
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.04
     multiplier_area = 1
-    dimensions = {'D1': 16, 'D2': 16, 'D3': 2, 'D4': 2}  # {'D1': ('K', 16), 'D2': ('C', 16), 'D3': ('OX', 2), 'D4': ('OY', 2),}
-
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {
+        "D1": 32,
+        "D2": 8,
+        "D3": 4,
+    }  # {'D1': ('K', 32), 'D2': ('OX', 8), 'D3': ('OY', 4),}
+
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions)
 
     return multiplier_array
 
 
-def cores():
+def cores_dut():
     multiplier_array1 = multiplier_array_dut()
     memory_hierarchy1 = memory_hierarchy_dut(multiplier_array1)
 
     core1 = Core(1, multiplier_array1, memory_hierarchy1)
 
     return {core1}
 
 
-cores = cores()
-global_buffer = None
+cores = cores_dut()
 acc_name = os.path.basename(__file__)[:-3]
-accelerator = Accelerator(acc_name, cores, global_buffer)
-
-a = 1
+accelerator = Accelerator(acc_name, cores)
```

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,100 +6,190 @@
 from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.hardware.architecture.core import Core
 
 
 def memory_hierarchy_dut(multiplier_array):
     """Memory hierarchy variables"""
-    ''' size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) '''
+    """ size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) """
 
-    reg_IW1 = MemoryInstance(name="rf_1B", size=8, r_bw=8, w_bw=8, r_cost=0.01, w_cost=0.01, area=0,
-                             r_port=1, w_port=1, rw_port=0, latency=1)
-
-    reg_O1 = MemoryInstance(name="rf_2B", size=16, r_bw=16, w_bw=16, r_cost=0.02, w_cost=0.02, area=0,
-                            r_port=2, w_port=2, rw_port=0, latency=1)
+    reg_IW1 = MemoryInstance(
+        name="rf_1B",
+        size=8,
+        r_bw=8,
+        w_bw=8,
+        r_cost=0.01,
+        w_cost=0.01,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+    )
+
+    reg_O1 = MemoryInstance(
+        name="rf_2B",
+        size=16,
+        r_bw=16,
+        w_bw=16,
+        r_cost=0.02,
+        w_cost=0.02,
+        area=0,
+        r_port=2,
+        w_port=2,
+        rw_port=0,
+        latency=1,
+    )
 
     ##################################### on-chip memory hierarchy building blocks #####################################
 
-    sram_32KB_512_1r_1w = \
-        MemoryInstance(name="sram_32KB", size=32768 * 8, r_bw=512, w_bw=512, r_cost=22.9, w_cost=52.01, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_2M_with_16_128K_bank_128_1r_1w = \
-        MemoryInstance(name="sram_2MB", size=131072 * 16 * 8, r_bw=128 * 16, w_bw=128 * 16, r_cost=26.01 * 16, w_cost=23.65 * 16, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
+    sram_32KB_512_1r_1w = MemoryInstance(
+        name="sram_32KB",
+        size=32768 * 8,
+        r_bw=512,
+        w_bw=512,
+        r_cost=22.9,
+        w_cost=52.01,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_2M_with_16_128K_bank_128_1r_1w = MemoryInstance(
+        name="sram_2MB",
+        size=131072 * 16 * 8,
+        r_bw=128 * 16,
+        w_bw=128 * 16,
+        r_cost=26.01 * 16,
+        w_cost=23.65 * 16,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
 
     #######################################################################################################################
 
-    dram = MemoryInstance(name="dram", size=10000000000, r_bw=64, w_bw=64, r_cost=700, w_cost=750, area=0,
-                          r_port=0, w_port=0, rw_port=1, latency=1)
+    dram = MemoryInstance(
+        name="dram",
+        size=10000000000,
+        r_bw=64,
+        w_bw=64,
+        r_cost=700,
+        w_cost=750,
+        area=0,
+        r_port=0,
+        w_port=0,
+        rw_port=1,
+        latency=1,
+    )
 
     memory_hierarchy_graph = MemoryHierarchy(operational_array=multiplier_array)
 
-    '''
+    """
     fh: from high = wr_in_by_high 
     fl: from low = wr_in_by_low 
     th: to high = rd_out_to_high
     tl: to low = rd_out_to_low
-    '''
+    """
     # we don't have unrolled I-Reg to better support G unrolling
     # memory_hierarchy_graph.add_memory(memory_instance=reg_IW1, operands=('I1',),
     #                                   port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
     #                                   served_dimensions={(0, 0, 0, 0)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_IW1, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions={(0, 0, 1, 0), (0, 0, 0, 1)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_O1, operands=('O',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_2', 'th': 'r_port_2'},),
-                                      served_dimensions={(0, 1, 0, 0)})
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_IW1,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions={(0, 0, 1, 0), (0, 0, 0, 1)},
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_O1,
+        operands=("O",),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_2", "th": "r_port_2"},
+        ),
+        served_dimensions={(0, 1, 0, 0)},
+    )
 
     ##################################### on-chip highest memory hierarchy initialization #####################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=sram_32KB_512_1r_1w, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=sram_2M_with_16_128K_bank_128_1r_1w, operands=('I1', 'O'),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_32KB_512_1r_1w,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_2M_with_16_128K_bank_128_1r_1w,
+        operands=("I1", "O"),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_1", "th": "r_port_1"},
+        ),
+        served_dimensions="all",
+    )
 
     ####################################################################################################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=dram, operands=('I1', 'I2', 'O'),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': 'rw_port_1', 'th': 'rw_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=dram,
+        operands=("I1", "I2", "O"),
+        port_alloc=(
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {
+                "fh": "rw_port_1",
+                "tl": "rw_port_1",
+                "fl": "rw_port_1",
+                "th": "rw_port_1",
+            },
+        ),
+        served_dimensions="all",
+    )
+
+    from zigzag.visualization.graph.memory_hierarchy import (
+        visualize_memory_hierarchy_graph,
+    )
 
-    from zigzag.visualization.graph.memory_hierarchy import visualize_memory_hierarchy_graph
     # visualize_memory_hierarchy_graph(memory_hierarchy_graph)
     return memory_hierarchy_graph
 
 
 def multiplier_array_dut():
-    """ Multiplier array variables """
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.04
     multiplier_area = 1
-    dimensions = {'D1': 8, 'D2': 8, 'D3': 4, 'D4': 4}  # {'D1': ('K', 8), 'D2': ('C', 8), 'D3': ('OX', 4), 'D4': ('OY', 4),}
-
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {
+        "D1": 8,
+        "D2": 8,
+        "D3": 4,
+        "D4": 4,
+    }  # {'D1': ('K', 8), 'D2': ('C', 8), 'D3': ('OX', 4), 'D4': ('OY', 4),}
+
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions)
 
     return multiplier_array
 
 
-def cores():
+def cores_dut():
     multiplier_array1 = multiplier_array_dut()
     memory_hierarchy1 = memory_hierarchy_dut(multiplier_array1)
 
     core1 = Core(1, multiplier_array1, memory_hierarchy1)
 
     return {core1}
 
 
-cores = cores()
-global_buffer = None
+cores = cores_dut()
 acc_name = os.path.basename(__file__)[:-3]
-accelerator = Accelerator(acc_name, cores, global_buffer)
-
-a = 1
+accelerator = Accelerator(acc_name, cores)
```

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Eyeriss_like.py` & `zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/TPU_like.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,168 @@
+import os
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 from zigzag.classes.hardware.architecture.memory_level import MemoryLevel
 from zigzag.classes.hardware.architecture.operational_unit import Multiplier
 from zigzag.classes.hardware.architecture.operational_array import MultiplierArray
 from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.hardware.architecture.core import Core
 
 
-def memory_hierarchy_latency_test1(multiplier_array):
+def memory_hierarchy_dut(multiplier_array):
     """Memory hierarchy variables"""
-    ''' size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) '''
-    rf1 = MemoryInstance(name="rf_64B", size=512, r_bw=8, w_bw=8, r_cost=1.0, w_cost=1.5, area=0.3, r_port=1, w_port=1, rw_port=0, latency=1)  # rd E per bit 0.125
-    rf2 = MemoryInstance(name="rf_16B", size=128, r_bw=24, w_bw=24, r_cost=1.5, w_cost=2, area=0.95, r_port=1, w_port=1, rw_port=1, latency=1)  # rd E per bit 0.0625
-    # lb1 = MemoryInstance(name="sram_64KB", size=524288, r_bw=128, w_bw=128, r_cost=20, w_cost=25, area=6, r_port=1, w_port=1, rw_port=0, latency=1)  # rd E per bit 0.16
-    lb2 = MemoryInstance(name="sram_8KB", size=65536, r_bw=128, w_bw=128, r_cost=10, w_cost=15, r_port=0, area=3, w_port=0, rw_port=2, latency=1)  # rd E per bit 0.08
-    lb2_64KB = MemoryInstance(name="sram_64KB", size=524288, r_bw=128, w_bw=128, r_cost=20, w_cost=25, area=6, r_port=1, w_port=1, rw_port=0, latency=1)  # rd E per bit 0.08
-    gb = MemoryInstance(name="sram_1M", size=8388608, r_bw=384, w_bw=384, r_cost=100, w_cost=130, area=25, r_port=0, w_port=0, rw_port=2, latency=1)  # rd E per bit 0.26
-    dram = MemoryInstance(name="dram", size=10000000000, r_bw=64, w_bw=64, r_cost=1000, w_cost=1000, area=0, r_port=0, w_port=0, rw_port=1, latency=1) # rd E per bit 16
+    """ size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) """
+
+    reg_W_128B = MemoryInstance(
+        name="rf_128B",
+        size=128 * 8,
+        r_bw=8,
+        w_bw=8,
+        r_cost=0.095,
+        w_cost=0.095,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+    )
+
+    reg_O_2B = MemoryInstance(
+        name="rf_2B",
+        size=16,
+        r_bw=16,
+        w_bw=16,
+        r_cost=0.021,
+        w_cost=0.021,
+        area=0,
+        r_port=2,
+        w_port=2,
+        rw_port=0,
+        latency=1,
+    )
+
+    ##################################### on-chip memory hierarchy building blocks #####################################
+
+    # sram_32KB_512_1r_1w = \
+    #     MemoryInstance(name="sram_32KB", size=32768 * 8, r_bw=512, w_bw=512, r_cost=22.9, w_cost=52.01, area=0,
+    #                    r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
+
+    sram_2M_with_16_128K_bank_128_1r_1w = MemoryInstance(
+        name="sram_2MB",
+        size=131072 * 16 * 8,
+        r_bw=128 * 16,
+        w_bw=128 * 16,
+        r_cost=26.01 * 16,
+        w_cost=23.65 * 16,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    #######################################################################################################################
+
+    dram = MemoryInstance(
+        name="dram",
+        size=10000000000,
+        r_bw=64,
+        w_bw=64,
+        r_cost=700,
+        w_cost=750,
+        area=0,
+        r_port=0,
+        w_port=0,
+        rw_port=1,
+        latency=1,
+    )
 
     memory_hierarchy_graph = MemoryHierarchy(operational_array=multiplier_array)
 
-    '''
+    """
     fh: from high = wr_in_by_high 
     fl: from low = wr_in_by_low 
     th: to high = rd_out_to_high
     tl: to low = rd_out_to_low
-    '''
-    memory_hierarchy_graph.add_memory(memory_instance=rf1, operands=('I1',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions=set())
-    memory_hierarchy_graph.add_memory(memory_instance=rf1, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions=set())
-    memory_hierarchy_graph.add_memory(memory_instance=rf2, operands=('O',),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'rw_port_1'},),
-                                      served_dimensions=set())
-
-    memory_hierarchy_graph.add_memory(memory_instance=lb2, operands=('O',),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_2', 'fl': 'rw_port_2', 'th': 'rw_port_1'},),
-                                      served_dimensions='all', )
-    memory_hierarchy_graph.add_memory(memory_instance=lb2_64KB, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=gb, operands=('I1', 'O'),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_2', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_2', 'fl': 'rw_port_2', 'th': 'rw_port_1'},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=dram, operands=('I1', 'I2', 'O'),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': 'rw_port_1', 'th': 'rw_port_1'},),
-                                      served_dimensions='all')
+    """
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_W_128B,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions={(0, 0)},
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_O_2B,
+        operands=("O",),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_2", "th": "r_port_2"},
+        ),
+        served_dimensions={(0, 1)},
+    )
+
+    ##################################### on-chip highest memory hierarchy initialization #####################################
+
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_2M_with_16_128K_bank_128_1r_1w,
+        operands=("I1", "O"),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_1", "th": "r_port_1"},
+        ),
+        served_dimensions="all",
+    )
+
+    ####################################################################################################################
+
+    memory_hierarchy_graph.add_memory(
+        memory_instance=dram,
+        operands=("I1", "I2", "O"),
+        port_alloc=(
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {
+                "fh": "rw_port_1",
+                "tl": "rw_port_1",
+                "fl": "rw_port_1",
+                "th": "rw_port_1",
+            },
+        ),
+        served_dimensions="all",
+    )
+
+    from zigzag.visualization.graph.memory_hierarchy import (
+        visualize_memory_hierarchy_graph,
+    )
 
-    # from visualization.graph.memory_hierarchy import visualize_memory_hierarchy_graph
-    # visualize_memory_hierarchy_graph(memory_hierarchy_graph)
+    visualize_memory_hierarchy_graph(memory_hierarchy_graph)
     return memory_hierarchy_graph
 
 
-def multiplier_array_latency_test1():
-    """ Multiplier array variables """
+def multiplier_array_dut():
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
-    multiplier_energy = 0.5
-    multiplier_area = 0.1
-    dimensions = {'D1': 14, 'D2': 12}
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    multiplier_energy = 0.04
+    multiplier_area = 1
+    dimensions = {"D1": 32, "D2": 32}  # {'D1': ('K', 32), 'D2': ('C', 32)}
+
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions)
 
     return multiplier_array
 
 
-def cores():
-    multiplier_array1 = multiplier_array_latency_test1()
-    memory_hierarchy1 = memory_hierarchy_latency_test1(multiplier_array1)
+def cores_dut():
+    multiplier_array1 = multiplier_array_dut()
+    memory_hierarchy1 = memory_hierarchy_dut(multiplier_array1)
 
     core1 = Core(1, multiplier_array1, memory_hierarchy1)
 
     return {core1}
 
 
-cores = cores()
-global_buffer = None
-accelerator = Accelerator("Eyeriss-like-simple", cores, global_buffer)
-
+cores = cores_dut()
+acc_name = os.path.basename(__file__)[:-3]
+accelerator = Accelerator(acc_name, cores)
```

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/hardware/Meta_prototype.py` & `zigzag-dse-2.3.2/zigzag/inputs/examples/hardware/Meta_prototype.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,115 +6,235 @@
 from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
 from zigzag.classes.hardware.architecture.accelerator import Accelerator
 from zigzag.classes.hardware.architecture.core import Core
 
 
 def memory_hierarchy_dut(multiplier_array):
     """Memory hierarchy variables"""
-    ''' size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) '''
+    """ size=#bit, bw=(read bw, write bw), cost=(read word energy, write work energy) """
 
-    reg_IW1 = MemoryInstance(name="rf_1B", size=8, r_bw=8, w_bw=8, r_cost=0.01, w_cost=0.01, area=0,
-                             r_port=1, w_port=1, rw_port=0, latency=1)
-
-    reg_O1 = MemoryInstance(name="rf_2B", size=16, r_bw=16, w_bw=16, r_cost=0.02, w_cost=0.02, area=0,
-                            r_port=2, w_port=2, rw_port=0, latency=1)
+    reg_IW1 = MemoryInstance(
+        name="rf_1B",
+        size=8,
+        r_bw=8,
+        w_bw=8,
+        r_cost=0.01,
+        w_cost=0.01,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+    )
+
+    reg_O1 = MemoryInstance(
+        name="rf_2B",
+        size=16,
+        r_bw=16,
+        w_bw=16,
+        r_cost=0.02,
+        w_cost=0.02,
+        area=0,
+        r_port=2,
+        w_port=2,
+        rw_port=0,
+        latency=1,
+    )
 
     ##################################### on-chip memory hierarchy building blocks #####################################
 
-    sram_64KB_with_8_8K_64_1r_1w = \
-        MemoryInstance(name="sram_64KB", size=8192 * 8 * 8, r_bw=64 * 8, w_bw=64 * 8, r_cost=3.32 * 8, w_cost=3.85 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_32KB_with_4_8K_64_1r_1w = \
-        MemoryInstance(name="sram_32KB", size=8192 * 4 * 8, r_bw=64 * 4, w_bw=64 * 4, r_cost=3.32 * 4, w_cost=3.85 * 4, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_1M_with_8_128K_bank_128_1r_1w_A = \
-        MemoryInstance(name="sram_1MB_A", size=131072 * 8 * 8, r_bw=128 * 8, w_bw=128 * 8, r_cost=26.01 * 8, w_cost=23.65 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
-
-    sram_1M_with_8_128K_bank_128_1r_1w_W = \
-        MemoryInstance(name="sram_1MB_W", size=131072 * 8 * 8, r_bw=128 * 8, w_bw=128 * 8, r_cost=26.01 * 8, w_cost=23.65 * 8, area=0,
-                       r_port=1, w_port=1, rw_port=0, latency=1, min_r_granularity=64, min_w_granularity=64)
+    sram_64KB_with_8_8K_64_1r_1w = MemoryInstance(
+        name="sram_64KB",
+        size=8192 * 8 * 8,
+        r_bw=64 * 8,
+        w_bw=64 * 8,
+        r_cost=3.32 * 8,
+        w_cost=3.85 * 8,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_32KB_with_4_8K_64_1r_1w = MemoryInstance(
+        name="sram_32KB",
+        size=8192 * 4 * 8,
+        r_bw=64 * 4,
+        w_bw=64 * 4,
+        r_cost=3.32 * 4,
+        w_cost=3.85 * 4,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_1M_with_8_128K_bank_128_1r_1w_A = MemoryInstance(
+        name="sram_1MB_A",
+        size=131072 * 8 * 8,
+        r_bw=128 * 8,
+        w_bw=128 * 8,
+        r_cost=26.01 * 8,
+        w_cost=23.65 * 8,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
+
+    sram_1M_with_8_128K_bank_128_1r_1w_W = MemoryInstance(
+        name="sram_1MB_W",
+        size=131072 * 8 * 8,
+        r_bw=128 * 8,
+        w_bw=128 * 8,
+        r_cost=26.01 * 8,
+        w_cost=23.65 * 8,
+        area=0,
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=1,
+        min_r_granularity=64,
+        min_w_granularity=64,
+    )
 
     #######################################################################################################################
 
-    dram = MemoryInstance(name="dram", size=10000000000, r_bw=64, w_bw=64, r_cost=700, w_cost=750, area=0,
-                          r_port=0, w_port=0, rw_port=1, latency=1)
+    dram = MemoryInstance(
+        name="dram",
+        size=10000000000,
+        r_bw=64,
+        w_bw=64,
+        r_cost=700,
+        w_cost=750,
+        area=0,
+        r_port=0,
+        w_port=0,
+        rw_port=1,
+        latency=1,
+    )
 
     memory_hierarchy_graph = MemoryHierarchy(operational_array=multiplier_array)
 
-    '''
+    """
     fh: from high = wr_in_by_high 
     fl: from low = wr_in_by_low 
     th: to high = rd_out_to_high
     tl: to low = rd_out_to_low
-    '''
+    """
     # we don't have unrolled I-Reg to better support G unrolling
     # memory_hierarchy_graph.add_memory(memory_instance=reg_IW1, operands=('I1',),
     #                                   port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
     #                                   served_dimensions={(0, 0, 0, 0)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_IW1, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions={(0, 0, 1, 0), (0, 0, 0, 1)})
-    memory_hierarchy_graph.add_memory(memory_instance=reg_O1, operands=('O',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_2', 'th': 'r_port_2'},),
-                                      served_dimensions={(0, 1, 0, 0)})
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_IW1,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions={(0, 0, 1, 0), (0, 0, 0, 1)},
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=reg_O1,
+        operands=("O",),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_2", "th": "r_port_2"},
+        ),
+        served_dimensions={(0, 1, 0, 0)},
+    )
 
     ##################################### on-chip highest memory hierarchy initialization #####################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=sram_64KB_with_8_8K_64_1r_1w, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_W, operands=('I2',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-
-    memory_hierarchy_graph.add_memory(memory_instance=sram_32KB_with_4_8K_64_1r_1w, operands=('I1',),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},),
-                                      served_dimensions='all')
-    memory_hierarchy_graph.add_memory(memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_A, operands=('I1', 'O'),
-                                      port_alloc=({'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'w_port_1', 'tl': 'r_port_1', 'fl': 'w_port_1', 'th': 'r_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_64KB_with_8_8K_64_1r_1w,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_W,
+        operands=("I2",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_32KB_with_4_8K_64_1r_1w,
+        operands=("I1",),
+        port_alloc=({"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},),
+        served_dimensions="all",
+    )
+    memory_hierarchy_graph.add_memory(
+        memory_instance=sram_1M_with_8_128K_bank_128_1r_1w_A,
+        operands=("I1", "O"),
+        port_alloc=(
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": None, "th": None},
+            {"fh": "w_port_1", "tl": "r_port_1", "fl": "w_port_1", "th": "r_port_1"},
+        ),
+        served_dimensions="all",
+    )
 
     ####################################################################################################################
 
-    memory_hierarchy_graph.add_memory(memory_instance=dram, operands=('I1', 'I2', 'O'),
-                                      port_alloc=({'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': None, 'th': None},
-                                                  {'fh': 'rw_port_1', 'tl': 'rw_port_1', 'fl': 'rw_port_1', 'th': 'rw_port_1'},),
-                                      served_dimensions='all')
+    memory_hierarchy_graph.add_memory(
+        memory_instance=dram,
+        operands=("I1", "I2", "O"),
+        port_alloc=(
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {"fh": "rw_port_1", "tl": "rw_port_1", "fl": None, "th": None},
+            {
+                "fh": "rw_port_1",
+                "tl": "rw_port_1",
+                "fl": "rw_port_1",
+                "th": "rw_port_1",
+            },
+        ),
+        served_dimensions="all",
+    )
+
+    from zigzag.visualization.graph.memory_hierarchy import (
+        visualize_memory_hierarchy_graph,
+    )
 
-    from zigzag.visualization.graph.memory_hierarchy import visualize_memory_hierarchy_graph
     # visualize_memory_hierarchy_graph(memory_hierarchy_graph)
     return memory_hierarchy_graph
 
 
 def multiplier_array_dut():
-    """ Multiplier array variables """
+    """Multiplier array variables"""
     multiplier_input_precision = [8, 8]
     multiplier_energy = 0.04
     multiplier_area = 1
-    dimensions = {'D1': 32, 'D2': 2, 'D3': 4, 'D4': 4}  # {'D1': ('K', 32), 'D2': ('C', 2), 'D3': ('OX', 4), 'D4': ('OY', 4),}
-
-    multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+    dimensions = {
+        "D1": 32,
+        "D2": 2,
+        "D3": 4,
+        "D4": 4,
+    }  # {'D1': ('K', 32), 'D2': ('C', 2), 'D3': ('OX', 4), 'D4': ('OY', 4),}
+
+    multiplier = Multiplier(
+        multiplier_input_precision, multiplier_energy, multiplier_area
+    )
     multiplier_array = MultiplierArray(multiplier, dimensions)
 
     return multiplier_array
 
 
-def cores():
+def cores_dut():
     multiplier_array1 = multiplier_array_dut()
     memory_hierarchy1 = memory_hierarchy_dut(multiplier_array1)
 
     core1 = Core(1, multiplier_array1, memory_hierarchy1)
 
     return {core1}
 
 
-cores = cores()
-global_buffer = None
+cores = cores_dut()
 acc_name = os.path.basename(__file__)[:-3]
-accelerator = Accelerator(acc_name, cores, global_buffer)
-
-a = 1
+accelerator = Accelerator(acc_name, cores)
```

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/workload/alexnet.onnx` & `zigzag-dse-2.3.2/zigzag/inputs/examples/workload/alexnet.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/workload/mobilenetv2.onnx` & `zigzag-dse-2.3.2/zigzag/inputs/examples/workload/mobilenetv2.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-2.3.1/zigzag/inputs/examples/workload/resnet18.py` & `zigzag-dse-2.3.2/zigzag/inputs/examples/workload/resnet18.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,332 +1,503 @@
 workload = {
     0: {  # conv1, stride 2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 64, 'C': 3, 'OY': 112, 'OX': 112, 'FY': 7, 'FX': 7},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': []},
-        'constant_operands': ['I', 'W'],
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 64,
+            "C": 3,
+            "OY": 112,
+            "OX": 112,
+            "FY": 7,
+            "FX": 7,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": []},
+        "constant_operands": ["I", "W"],
+    },
     1: {  # max pool, stride 2
-        'operator_type': 'Pooling',
-        'equation': 'O[b][g][oy][ox]+=W[fx][fy]*I[b][g][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'G': 64, 'OY': 56, 'OX': 56, 'FX': 3, 'FY': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'I': 8, 'W': 0},
-        'operand_source': {'W': [], 'I': [0]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Pooling",
+        "equation": "O[b][g][oy][ox]+=W[fx][fy]*I[b][g][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {"B": 1, "G": 64, "OY": 56, "OX": 56, "FX": 3, "FY": 3},
+        "operand_precision": {"O": 16, "O_final": 8, "I": 8, "W": 0},
+        "operand_source": {"W": [], "I": [0]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "G": "K"}},
+    },
     2: {  # conv2_1
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 64, 'C': 64, 'OY': 56, 'OX': 56, 'FY': 3, 'FX': 3, },
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [1]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 64,
+            "C": 64,
+            "OY": 56,
+            "OX": 56,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [1]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     3: {  # conv2_2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 64, 'C': 64, 'OY': 56, 'OX': 56, 'FY': 3, 'FX': 3, },
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [2]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 64,
+            "C": 64,
+            "OY": 56,
+            "OX": 56,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [2]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
+    },
     4: {  # Addition of layer 1 (residual path) and layer 3 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 64, 'OY': 56, 'OX': 56},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [1], 'Y': [3]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 64, "OY": 56, "OX": 56},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [1], "Y": [3]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "K"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     5: {  # conv2_3
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 64, 'C': 64, 'OY': 56, 'OX': 56, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [4]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 64,
+            "C": 64,
+            "OY": 56,
+            "OX": 56,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [4]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     6: {  # conv2_4
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 64, 'C': 64, 'OY': 56, 'OX': 56, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [5]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 64,
+            "C": 64,
+            "OY": 56,
+            "OX": 56,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [5]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     7: {  # Addition of layer 4 (residual connection) and layer 6 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 64, 'OY': 56, 'OX': 56},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [4], 'Y': [6]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'G'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 64, "OY": 56, "OX": 56},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [4], "Y": [6]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "G"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     8: {  # conv3_1, stride 2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 128, 'C': 64, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [7]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 128,
+            "C": 64,
+            "OY": 28,
+            "OX": 28,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [7]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     9: {  # conv3_2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 128, 'C': 128, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [8]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 128,
+            "C": 128,
+            "OY": 28,
+            "OX": 28,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [8]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     10: {  # conv downsample of layer 7
-        'operator_type': 'Conv_downsample',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 128, 'C': 64, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [7]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv_downsample",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 128,
+            "C": 64,
+            "OY": 28,
+            "OX": 28,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [7]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     11: {  # Addition of layer 10 (residual connection) and layer 9 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 128, 'OY': 28, 'OX': 28},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [10], 'Y': [9]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 128, "OY": 28, "OX": 28},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [10], "Y": [9]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "K"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     12: {  # conv3_3
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 128, 'C': 128, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [11]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 128,
+            "C": 128,
+            "OY": 28,
+            "OX": 28,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [11]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     13: {  # conv3_4
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 128, 'C': 128, 'OY': 28, 'OX': 28, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [12]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 128,
+            "C": 128,
+            "OY": 28,
+            "OX": 28,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [12]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     14: {  # Addition of layer 11 (residual connection) and layer 13 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 128, 'OY': 28, 'OX': 28},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [11], 'Y': [13]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'G'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 128, "OY": 28, "OX": 28},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [11], "Y": [13]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "G"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     15: {  # conv4_1, stride 2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 256, 'C': 128, 'OY': 14, 'OX': 14, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [14]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 256,
+            "C": 128,
+            "OY": 14,
+            "OX": 14,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [14]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     16: {  # conv4_2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 256, 'C': 256, 'OY': 14, 'OX': 14, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [15]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 256,
+            "C": 256,
+            "OY": 14,
+            "OX": 14,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [15]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     17: {  # conv downsample of layer 14
-        'operator_type': 'Conv_downsample',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 256, 'C': 128, 'OY': 14, 'OX': 14, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [14]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv_downsample",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 256,
+            "C": 128,
+            "OY": 14,
+            "OX": 14,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [14]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     18: {  # Addition of layer 17 (residual connection) and layer 16 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 256, 'OY': 14, 'OX': 14},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [17], 'Y': [16]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 256, "OY": 14, "OX": 14},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [17], "Y": [16]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "K"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     19: {  # conv4_3
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 256, 'C': 256, 'OY': 14, 'OX': 14, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [18]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 256,
+            "C": 256,
+            "OY": 14,
+            "OX": 14,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [18]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     20: {  # conv4_4
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 256, 'C': 256, 'OY': 14, 'OX': 14, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [19]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 256,
+            "C": 256,
+            "OY": 14,
+            "OX": 14,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [19]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     21: {  # Addition of layer 18 (residual connection) and layer 20 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 256, 'OY': 14, 'OX': 14},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [18], 'Y': [20]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'G'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 256, "OY": 14, "OX": 14},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [18], "Y": [20]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "G"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     22: {  # conv5_1, stride 2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 512, 'C': 256, 'OY': 7, 'OX': 7, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [21]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 512,
+            "C": 256,
+            "OY": 7,
+            "OX": 7,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [21]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     23: {  # conv5_2
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 512, 'C': 512, 'OY': 7, 'OX': 7, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [22]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 512,
+            "C": 512,
+            "OY": 7,
+            "OX": 7,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [22]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     24: {  # conv downsample of layer 21
-        'operator_type': 'Conv_downsample',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=2*ox+1*fx', 'iy=2*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 512, 'C': 256, 'OY': 7, 'OX': 7, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [21]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv_downsample",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=2*ox+1*fx", "iy=2*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 512,
+            "C": 256,
+            "OY": 7,
+            "OX": 7,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [21]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     25: {  # Addition of layer 24 (residual connection) and layer 23 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 512, 'OY': 7, 'OX': 7},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [24], 'Y': [23]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'G'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
-    }
-    ,
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 512, "OY": 7, "OX": 7},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [24], "Y": [23]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "G"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
+    },
     26: {  # conv5_3
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 512, 'C': 512, 'OY': 7, 'OX': 7, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [25]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
-    ,
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 512,
+            "C": 512,
+            "OY": 7,
+            "OX": 7,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [25]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
     27: {  # conv4_4
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 512, 'C': 512, 'OY': 7, 'OX': 7, 'FY': 3, 'FX': 3},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [26]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'K'}},
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 512,
+            "C": 512,
+            "OY": 7,
+            "OX": 7,
+            "FY": 3,
+            "FX": 3,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [26]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "K"}},
     },
     28: {  # Addition of layer 25 (residual connection) and layer 27 (main path)
-        'operator_type': 'Add',
-        'equation': 'O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]',
-        'dimension_relations': [],
-        'loop_dim_size': {'B': 1, 'G': 512, 'OY': 7, 'OX': 7},
-        'operand_precision': {'O': 16, 'O_final': 8, 'X': 8, 'Y': 8},
-        'operand_source': {'X': [25], 'Y': [27]},
-        'constant_operands': [],
-        'operand_source_dimension_mapping': {'X': {'OX': 'OX', 'OY': 'OY', 'G': 'G'}, 'Y': {'OX': 'OX', 'OY': 'OY', 'G': 'K'}},
+        "operator_type": "Add",
+        "equation": "O[b][g][oy][ox]=X[b][g][oy][ox]+Y[b][g][oy][ox]",
+        "dimension_relations": [],
+        "loop_dim_size": {"B": 1, "G": 512, "OY": 7, "OX": 7},
+        "operand_precision": {"O": 16, "O_final": 8, "X": 8, "Y": 8},
+        "operand_source": {"X": [25], "Y": [27]},
+        "constant_operands": [],
+        "operand_source_dimension_mapping": {
+            "X": {"OX": "OX", "OY": "OY", "G": "G"},
+            "Y": {"OX": "OX", "OY": "OY", "G": "K"},
+        },
     },
     29: {  # aver pool
-        'operator_type': 'Pooling',
-        'equation': 'O[b][g][oy][ox]+=W[fx][fy]*I[b][g][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'G': 512, 'OY': 1, 'OX': 1, 'FX': 7, 'FY': 7},
-        'operand_precision': {'O': 16, 'O_final': 8, 'I': 8, 'W': 0},
-        'operand_source': {'W': [], 'I': [28]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'G': 'K'}},
+        "operator_type": "Pooling",
+        "equation": "O[b][g][oy][ox]+=W[fx][fy]*I[b][g][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {"B": 1, "G": 512, "OY": 1, "OX": 1, "FX": 7, "FY": 7},
+        "operand_precision": {"O": 16, "O_final": 8, "I": 8, "W": 0},
+        "operand_source": {"W": [], "I": [28]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "G": "K"}},
     },
     30: {  # fc
-        'operator_type': 'Conv',
-        'equation': 'O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]',
-        'dimension_relations': ['ix=1*ox+1*fx', 'iy=1*oy+1*fy'],
-        'loop_dim_size': {'B': 1, 'K': 1000, 'C': 512, 'OY': 1, 'OX': 1, 'FY': 1, 'FX': 1},
-        'operand_precision': {'O': 16, 'O_final': 8, 'W': 8, 'I': 8},
-        'operand_source': {'W': [], 'I': [29]},
-        'constant_operands': ['W'],
-        'operand_source_dimension_mapping': {'I': {'IX': 'OX', 'IY': 'OY', 'C': 'G'}},
-    }
+        "operator_type": "Conv",
+        "equation": "O[b][k][oy][ox]+=W[k][c][fy][fx]*I[b][c][iy][ix]",
+        "dimension_relations": ["ix=1*ox+1*fx", "iy=1*oy+1*fy"],
+        "loop_dim_size": {
+            "B": 1,
+            "K": 1000,
+            "C": 512,
+            "OY": 1,
+            "OX": 1,
+            "FY": 1,
+            "FX": 1,
+        },
+        "operand_precision": {"O": 16, "O_final": 8, "W": 8, "I": 8},
+        "operand_source": {"W": [], "I": [29]},
+        "constant_operands": ["W"],
+        "operand_source_dimension_mapping": {"I": {"IX": "OX", "IY": "OY", "C": "G"}},
+    },
 }
```

### Comparing `zigzag-dse-2.3.1/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag-dse-2.3.2/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import matplotlib.pyplot as plt
 import networkx as nx
 import matplotlib.pyplot as plt
 
 from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 
+
 def visualize_memory_hierarchy_graph(G: MemoryHierarchy):
     """
     Visualizes a memory hierarchy graph.
     """
 
     generations = list(nx.topological_generations(G))
     max_nodes_gen = max((len(generation) for generation in generations))
@@ -22,20 +23,30 @@
             if len(generation) == max_nodes_gen:
                 x = node_idx
             else:
                 x = (node_idx + 1) * (max_nodes_gen - 1) / (len(generation) + 1)
             pos[node] = (x, y)
             node_list.append(node)
             node_size_list.append(node_size)
-            node_label_dict[node] = f"{node.name}\n{node.operands}\nx{node.unroll_count}"
-
-    nx.draw(G, pos=pos, node_shape='s', nodelist=node_list, node_size=node_size_list, labels=node_label_dict)
+            node_label_dict[
+                node
+            ] = f"{node.name}\n{node.operands}\nx{node.unroll_count}"
+
+    nx.draw(
+        G,
+        pos=pos,
+        node_shape="s",
+        nodelist=node_list,
+        node_size=node_size_list,
+        labels=node_label_dict,
+    )
     plt.title(G.name)
     plt.show()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import pickle
-    with open('../list_of_cmes.pickle', 'rb') as handle:
+
+    with open("../list_of_cmes.pickle", "rb") as handle:
         list_of_cme = pickle.load(handle)
     cme = list_of_cme[0]
-    visualize_memory_hierarchy_graph(cme.accelerator.cores[0].memory_hierarchy)
+    visualize_memory_hierarchy_graph(cme.accelerator.cores[0].memory_hierarchy)
```

### Comparing `zigzag-dse-2.3.1/zigzag/visualization/graph/workload.py` & `zigzag-dse-2.3.2/zigzag/visualization/graph/workload.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,42 @@
 import networkx as nx
 
 
 def visualize_dnn_graph(G):
     pos = {}
     pos_lb = {}
     for i_node, node in enumerate(G.nodes()):
-        pos[node] = (i_node, -2*i_node)
-        pos_lb[node] = (i_node-1.5, -2*i_node-2)
+        pos[node] = (i_node, -2 * i_node)
+        pos_lb[node] = (i_node - 1.5, -2 * i_node - 2)
     plt.figure(figsize=(15, 5))
     rad = 0.8
     ax = plt.gca()
     edges = G.edges()
     for edge in edges:
         source, target = edge
         edge_rad = 0 if pos[target][0] - pos[source][0] == 1 else rad
-        ax.annotate("",
-                    xy=pos[source],
-                    xytext=pos[target],
-                    arrowprops=dict(arrowstyle="-", color="black",
-                                    connectionstyle=f"arc3,rad={edge_rad}",
-                                    alpha=0.7,
-                                    linewidth=5))
-    nx.draw_networkx_nodes(G, pos=pos, node_size=100, node_color='black')
-    nx.draw_networkx_labels(G, pos=pos_lb, font_color='black')
+        ax.annotate(
+            "",
+            xy=pos[source],
+            xytext=pos[target],
+            arrowprops=dict(
+                arrowstyle="-",
+                color="black",
+                connectionstyle=f"arc3,rad={edge_rad}",
+                alpha=0.7,
+                linewidth=5,
+            ),
+        )
+    nx.draw_networkx_nodes(G, pos=pos, node_size=100, node_color="black")
+    nx.draw_networkx_labels(G, pos=pos_lb, font_color="black")
     plt.box(False)
     plt.show()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import zigzag.classes.stages.MainInputParserStages as MainInputParserStages
-    workload = 'zigzag.inputs.examples.workload.resnet18'
-    parsed_workload = MainInputParserStages.parse_workload_from_path_or_from_module(workload)
-    visualize_dnn_graph(parsed_workload)
+
+    workload = "zigzag.inputs.examples.workload.resnet18"
+    parsed_workload = MainInputParserStages.parse_workload_from_path_or_from_module(
+        workload
+    )
+    visualize_dnn_graph(parsed_workload)
```

### Comparing `zigzag-dse-2.3.1/zigzag/visualization/results/plot_cme.py` & `zigzag-dse-2.3.2/zigzag/visualization/results/plot_cme.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,164 +3,262 @@
 from collections import defaultdict
 import matplotlib.pyplot as plt
 from matplotlib.colors import hsv_to_rgb
 import numpy as np
 from zigzag.classes.mapping.combined_mapping import FourWayDataMoving
 from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 
-def bar_plot_cost_model_evaluations_total(cmes: List[CostModelEvaluation], labels, fig_title: str="cost model evaluation comparison", save_path: str="plot.png"):
+# MPL FONT SIZES
+SMALLEST_SIZE = 10
+SMALLER_SIZE = 12
+SMALL_SIZE = 14
+MEDIUM_SIZE = 16
+BIG_SIZE = 18
+BIGGER_SIZE = 20
+plt.rc("font", size=SMALLEST_SIZE)  # controls default text sizes
+plt.rc("axes", titlesize=SMALL_SIZE)  # fontsize of the axes title
+plt.rc("axes", labelsize=BIGGER_SIZE)  # fontsize of the x and y labels
+plt.rc("xtick", labelsize=SMALLER_SIZE)  # fontsize of the tick labels
+plt.rc("ytick", labelsize=SMALLER_SIZE)  # fontsize of the tick labels
+plt.rc("legend", fontsize=SMALL_SIZE)  # legend fontsize
+plt.rc("figure", titlesize=MEDIUM_SIZE)  # fontsize of the figure title
+
+
+def bar_plot_cost_model_evaluations_total(
+    cmes: List[CostModelEvaluation],
+    labels,
+    save_path: str = "plot.png",
+):
     """Plot total energy and latency of each cost model evaluation in a bar chart.
 
     Args:
         cmes (List[CostModelEvaluation]): List of CostModelEvaluations to compare.
         save_path (str): Path to save the plot to.
     """
-    assert len(cmes) == len(labels), "Please match a label for each cost model evaluation."
+    assert len(cmes) == len(
+        labels
+    ), "Please match a label for each cost model evaluation."
     energies = [cme.energy_total for cme in cmes]
     latencies = [cme.latency_total2 for cme in cmes]
 
     x = np.arange(len(labels))  # the label locations
     width = 0.35  # the width of the bars
 
     fig, ax1 = plt.subplots()
     ax2 = ax1.twinx()
 
-    h1 = rects1 = ax1.bar(x - width/2, energies, width, label='Energy (pJ)', color='maroon')
-    h2 = rects2 = ax2.bar(x + width/2, latencies, width, label='Latency (cycle)', color='indigo')
+    colormap = plt.get_cmap("Set1")
+    color_energy = colormap.colors[0]
+    color_latency = colormap.colors[1]
+
+    h1 = rects1 = ax1.bar(
+        x - width / 2, energies, width, label="Energy", color=color_energy
+    )
+    h2 = rects2 = ax2.bar(
+        x + width / 2, latencies, width, label="Latency", color=color_latency
+    )
 
     # Add some text for labels, title and custom x-axis tick labels, etc.
-    ax1.set_ylabel('Energy (pJ)', fontsize=15)
-    ax2.set_ylabel('Latency (cycle)', fontsize=15)
-    ax1.set_title('Scores by group and gender', fontsize=15)
+    ax1.set_ylabel("Energy [pJ]", fontsize=15)
+    ax2.set_ylabel("Latency [cycle]", fontsize=15)
     ax1.set_xticks(x, labels)
-    # hs = h1 + h2
-    # labs = [h.get_label() for h in hs]
-    # ax1.legend(hs, labs, loc='best')
+    handles1, labels1 = ax1.get_legend_handles_labels()
+    handles2, labels2 = ax2.get_legend_handles_labels()
+    ax2.legend(
+        handles1 + handles2,
+        labels1 + labels2,
+        bbox_to_anchor=(0.5, 1.035),
+        loc="lower center",
+        borderaxespad=0,
+        ncol=2,
+    )
+
+    ax1.bar_label(rects1, padding=3, fmt="%.1e")
+    ax2.bar_label(rects2, padding=3, fmt="%.1e")
+    # ax1.figure.texts.append(ax1.texts.pop())
+    # ax2.figure.texts.append(ax2.texts.pop())
 
-    ax1.bar_label(rects1, padding=3, fmt='%.2e')
-    ax2.bar_label(rects2, padding=3, fmt='%.2e')
-
-    ax1.set_title(fig_title)
+    # ax1.set_title(fig_title)
     fig.tight_layout()
     plt.savefig(save_path)
 
 
-
-def bar_plot_cost_model_evaluations_breakdown(cmes: List[CostModelEvaluation], save_path: str):
-    memory_word_access_summed = {d: defaultdict(lambda: defaultdict(lambda: FourWayDataMoving(0, 0, 0, 0))) for d in range(len(cmes))}
+def bar_plot_cost_model_evaluations_breakdown(
+    cmes: List[CostModelEvaluation], save_path: str, xtick_rotation=90
+):
+    memory_word_access_summed = {
+        d: defaultdict(lambda: defaultdict(lambda: FourWayDataMoving(0, 0, 0, 0)))
+        for d in range(len(cmes))
+    }
     mac_costs = defaultdict(lambda: 0)
     memory_instances = {}
-    la_break_down = {d: {'Ideal computation': 0, 'Spatial stall': 0, 'Temporal stall': 0, 'Data loading': 0, 'Data off-loading': 0} for d in range(len(cmes))}
+    la_break_down = {
+        d: {
+            "Ideal computation": 0,
+            "Spatial stall": 0,
+            "Temporal stall": 0,
+            "Data loading": 0,
+            "Data off-loading": 0,
+        }
+        for d in range(len(cmes))
+    }
     la_tot = {d: 0 for d in range(len(cmes))}
 
     for d, cme in enumerate(cmes):
         mh = cme.accelerator.get_core(cme.layer.core_allocation).memory_hierarchy
         mac_costs[d] = cme.MAC_energy
-        la_break_down[d]['Ideal computation'] = cme.ideal_cycle
-        la_break_down[d]['Spatial stall'] = (cme.ideal_temporal_cycle - cme.ideal_cycle)
-        la_break_down[d]['Temporal stall'] = (cme.latency_total0 - cme.ideal_temporal_cycle)
-        la_break_down[d]['Data loading'] = (cme.latency_total1 - cme.latency_total0)
-        la_break_down[d]['Data off-loading'] = (cme.latency_total2 - cme.latency_total1)
+        la_break_down[d]["Ideal computation"] = cme.ideal_cycle
+        la_break_down[d]["Spatial stall"] = cme.ideal_temporal_cycle - cme.ideal_cycle
+        la_break_down[d]["Temporal stall"] = (
+            cme.latency_total0 - cme.ideal_temporal_cycle
+        )
+        la_break_down[d]["Data loading"] = cme.latency_total1 - cme.latency_total0
+        la_break_down[d]["Data off-loading"] = cme.latency_total2 - cme.latency_total1
         la_tot[d] = cme.latency_total2
         for operand in cme.energy_breakdown_further:
             mem_op = cme.layer.memory_operand_links[operand]
             operand_memory_levels = mh.get_memory_levels(mem_op)
             for j in range(len(cme.energy_breakdown_further[operand])):
                 mem = operand_memory_levels[j].name
                 memory_instances[mem] = operand_memory_levels[j]
-                memory_word_access_summed[d][operand][mem] += \
-                    cme.energy_breakdown_further[operand][j]
+                memory_word_access_summed[d][operand][
+                    mem
+                ] += cme.energy_breakdown_further[operand][j]
 
     all_mems = set()
     for v in memory_word_access_summed.values():
         for vv in v.values():
             for vvv in vv.keys():
                 all_mems.add(vvv)
-    all_mems = sorted(list(all_mems), key=lambda m: memory_instances[m].memory_instance.size)
+    all_mems = sorted(
+        list(all_mems), key=lambda m: memory_instances[m].memory_instance.size
+    )
     all_ops = set()
     for v in memory_word_access_summed.values():
         for vv in v.keys():
             all_ops.add(vv)
     all_ops = sorted(list(all_ops))
 
-    ''' plotting start '''
-    ''' Energy part '''
+    """ plotting start """
+    """ Energy part """
 
     fig, (ax1, ax2) = plt.subplots(nrows=2, figsize=(10, 8))
     hues = np.linspace(0, 1, len(all_ops) + 1)[:-1]
-    hatches = ['////', '\\\\\\\\', 'xxxx', '++++']
+    hatches = ["////", "\\\\\\\\", "xxxx", "++++"]
     x = 0
     xticks = {}
     for d, cme in enumerate(cmes):
         total_energy = 0
         startx_of_layer = x
         # mac
-        ax1.bar([x], [mac_costs[d]], width=1, bottom=0, facecolor='k')
+        ax1.bar([x], [mac_costs[d]], width=1, bottom=0, facecolor="k")
         total_energy += mac_costs[d]
         highest_bar = mac_costs[d]
-        xticks[x] = 'MAC'
+        xticks[x] = "MAC"
         x += 1
         # mems
         for mem in all_mems:
             bottom = 0
             for op_i, operand in enumerate(all_ops):
                 for dir_i, dir in enumerate(memory_word_access_summed[d][operand][mem]):
                     height = memory_word_access_summed[d][operand][mem][dir]
-                    ax1.bar([x], [height], width=1, bottom=[bottom],
-                            facecolor=hsv_to_rgb((hues[op_i], 1, 1)), hatch=hatches[dir_i])
+                    ax1.bar(
+                        [x],
+                        [height],
+                        width=1,
+                        bottom=[bottom],
+                        facecolor=hsv_to_rgb((hues[op_i], 1, 1)),
+                        hatch=hatches[dir_i],
+                    )
 
                     bottom += height
             xticks[x] = mem
             total_energy += bottom
             x += 1
             highest_bar = max(bottom, highest_bar)
-        ax1.text(x * 0.5 + startx_of_layer * 0.5, 1.05*highest_bar, "tot:{:,d}".format(int(total_energy)),
-                 horizontalalignment='center', verticalalignment='bottom', weight='bold')
+        x
+        ax1.text(
+            x * 0.5 + startx_of_layer * 0.5,
+            1.05 * highest_bar,
+            "tot:{:,d}".format(int(total_energy)),
+            horizontalalignment="center",
+            verticalalignment="bottom",
+            weight="bold",
+        )
         x += len(all_mems) / 4
 
     for op, h in zip(all_ops, hues):
         ax1.bar(0, 0, width=1, facecolor=hsv_to_rgb((h, 1, 1)), label=op)
 
     for dir_i, dir in enumerate(memory_word_access_summed[d][operand][mem]):
-        ax1.bar([0], [0], width=1, bottom=0, facecolor=(1, 1, 1), hatch=hatches[dir_i], label=dir)
+        ax1.bar(
+            [0],
+            [0],
+            width=1,
+            bottom=0,
+            facecolor=(1, 1, 1),
+            hatch=hatches[dir_i],
+            label=dir,
+        )
 
     ax1.legend(loc="upper left")
-    ax1.set_xticks(list(xticks.keys()), list(xticks.values()), rotation=90)
-    ax1.set_ylim(0, 1.1*ax1.get_ylim()[1])
+    ax1.set_xticks(list(xticks.keys()), list(xticks.values()), rotation=xtick_rotation)
+    ax1.set_ylim(0, 1.1 * ax1.get_ylim()[1])
 
     ax1.set_ylabel("Energy (pJ)", fontsize=15)
 
-    ''' Latency part '''
+    """ Latency part """
     x2 = list(range(len(la_break_down)))
 
     y2 = {ky: [] for ky in la_break_down[0].keys()}
     for _, design_point in la_break_down.items():
         for ky, val in design_point.items():
             y2[ky].append(val)
 
     hues = np.linspace(0, 1, len(y2) + 1)[:-1]
-    
+
     for idx, (ky, va) in enumerate(y2.items()):
         if idx == 0:
-            ax2.bar(np.array(x2), va, width=0.4, color=hsv_to_rgb((hues[idx], 1, 1)), label=ky)
+            ax2.bar(
+                np.array(x2),
+                va,
+                width=0.4,
+                color=hsv_to_rgb((hues[idx], 1, 1)),
+                label=ky,
+            )
             li_pre = va
         else:
-            ax2.bar(np.array(x2), va, width=0.4, color=hsv_to_rgb((hues[idx], 1, 1)), label=ky, bottom=li_pre)
+            ax2.bar(
+                np.array(x2),
+                va,
+                width=0.4,
+                color=hsv_to_rgb((hues[idx], 1, 1)),
+                label=ky,
+                bottom=li_pre,
+            )
             li_pre = [x + y for x, y in zip(li_pre, va)]
 
     for x in x2:
-        ax2.text(x, la_tot[x] * 1.05, "tot:{:,d}".format(int(la_tot[x])),
-                 horizontalalignment='center', verticalalignment='bottom', weight='bold')
+        ax2.text(
+            x,
+            la_tot[x] * 1.05,
+            "tot:{:,d}".format(int(la_tot[x])),
+            horizontalalignment="center",
+            verticalalignment="bottom",
+            weight="bold",
+        )
     ax2.legend()
-    ax2.set_ylim(0, 1.1*ax2.get_ylim()[1])
+    ax2.set_xticks(x2, x2, rotation=xtick_rotation)
+    ax2.set_ylim(0, 1.1 * ax2.get_ylim()[1])
     ax2.set_xlabel("Layers", fontsize=15)
     ax2.set_ylabel("Latency (cycle)", fontsize=15)
 
     fig.tight_layout()
     plt.savefig(save_path)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import pickle
-    with open('../list_of_cmes.pickle', 'rb') as handle:
+
+    with open("../list_of_cmes.pickle", "rb") as handle:
         list_of_cme = pickle.load(handle)
-    bar_plot_cost_model_evaluations_breakdown(list_of_cme, 'plot.png')
+    bar_plot_cost_model_evaluations_breakdown(list_of_cme, "plot.png")
```

### Comparing `zigzag-dse-2.3.1/zigzag/visualization/results/print_mapping.py` & `zigzag-dse-2.3.2/zigzag/visualization/results/print_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from copy import deepcopy
 
 
 def create_printing_block(row, col):
-    return [[' '] * col for _ in range(row)]
+    return [[" "] * col for _ in range(row)]
 
 
 def modify_printing_block(old_block, start_row, start_col, new_str):
     new_block = deepcopy(old_block)
-    new_block[start_row][start_col:start_col + len(new_str)] = new_str
+    new_block[start_row][start_col : start_col + len(new_str)] = new_str
     return new_block
 
 
 def print_printing_block(printing_block):
     print()
     for i in range(len(printing_block)):
-        print(''.join(printing_block[i]))
+        print("".join(printing_block[i]))
 
 
 def print_good_tm_format(tm, mem_name, cme_name, mem_op_to_layer_op):
     op_list = list(tm.keys())
     tm_list = [tp for li in tm[op_list[0]] for tp in li]
 
     # get required interval between operands (e.g., 'W', 'I', 'O'), based on actual mem name length
@@ -29,59 +29,76 @@
                 max_mem_name_len = len(mem_name[operand][lv])
     interval = max_mem_name_len + 10
 
     tot_row = 2 * (len(tm_list) + 1) + 8
     tot_col = int(2 * (len(tm_list) + 1) + 3.75 * interval)
     tot_col_cut = 2 * (len(tm_list) + 1) + interval
     tm_block = create_printing_block(tot_row, tot_col)
-    title = f' Temporal Mapping - {cme_name} '
-    dash = '*' * int((tot_col - len(title)) / 2)
+    title = f" Temporal Mapping - {cme_name} "
+    dash = "*" * int((tot_col - len(title)) / 2)
     tm_block = modify_printing_block(tm_block, 1, 0, dash + title + dash)
     i = 2
     for op in mem_op_to_layer_op.keys():
-        tm_block = modify_printing_block(tm_block, i, 1, f'{op} ({mem_op_to_layer_op[op]}): ' + str(tm[op]))
+        tm_block = modify_printing_block(
+            tm_block, i, 1, f"{op} ({mem_op_to_layer_op[op]}): " + str(tm[op])
+        )
         i += 1
-    tm_block = modify_printing_block(tm_block, 6, 0, '-' * tot_col)
-    tm_block = modify_printing_block(tm_block, 7, 1, 'Temporal Loops')
-    tm_block = modify_printing_block(tm_block, 8, 0, '-' * tot_col)
+    tm_block = modify_printing_block(tm_block, 6, 0, "-" * tot_col)
+    tm_block = modify_printing_block(tm_block, 7, 1, "Temporal Loops")
+    tm_block = modify_printing_block(tm_block, 8, 0, "-" * tot_col)
     finish_row = 2 * len(tm_list) + 7
     for i, li in enumerate(tm_list):
-        tm_block = modify_printing_block(tm_block, finish_row - 2 * i, len(tm_list) - i,
-                                         'for ' + str(li[0]) + ' in ' + '[0:' + str(li[1]) + ')')
-        tm_block = modify_printing_block(tm_block, 2 * (i + 1) + 1 + 7, 0, '-' * tot_col)
+        tm_block = modify_printing_block(
+            tm_block,
+            finish_row - 2 * i,
+            len(tm_list) - i,
+            "for " + str(li[0]) + " in " + "[0:" + str(li[1]) + ")",
+        )
+        tm_block = modify_printing_block(
+            tm_block, 2 * (i + 1) + 1 + 7, 0, "-" * tot_col
+        )
 
     # print mem name to each level
     for idx, operand in enumerate(op_list):
         column_position = tot_col_cut + idx * interval
         tm_block = modify_printing_block(tm_block, 7, column_position, operand)
         i = 0
         for level, lv_li in enumerate(tm[operand]):
             for _ in lv_li:
-                tm_block = modify_printing_block(tm_block, finish_row - 2 * i, column_position,
-                                                 str(mem_name[operand][level]))
+                tm_block = modify_printing_block(
+                    tm_block,
+                    finish_row - 2 * i,
+                    column_position,
+                    str(mem_name[operand][level]),
+                )
                 i += 1
     # tm_block = modify_printing_block(tm_block, finish_row + 2, 1,
     #                                  "(Notes: Temporal Mapping starts from the innermost memory level. MAC level is out of Temporal Mapping's scope.)")
     print_printing_block(tm_block)
 
 
 def print_mapping(cme):
     tm = cme.temporal_mapping.mapping_dic_stationary
     mem_op_to_layer_op = cme.mem_op_to_layer_op
     layer_op_to_mem_op = cme.layer_op_to_mem_op
     mem_name = {}
-    for (mem_op, mems_all_levels) in cme.accelerator.cores[0].mem_hierarchy_dict.items():
+    for (mem_op, mems_all_levels) in cme.accelerator.cores[
+        0
+    ].mem_hierarchy_dict.items():
         layer_op = mem_op_to_layer_op[mem_op]
         mem_name[layer_op] = []
         for mem_a_level in mems_all_levels:
             mem_name[layer_op].append(mem_a_level.name)
-        assert len(tm[layer_op]) == len(mem_name[layer_op]), \
-            f"Temporal mapping level {len(tm[layer_op])} and memory hierarchy level {len(mem_name[layer_op])} of operand {layer_op} do not match."
+        assert len(tm[layer_op]) == len(
+            mem_name[layer_op]
+        ), f"Temporal mapping level {len(tm[layer_op])} and memory hierarchy level {len(mem_name[layer_op])} of operand {layer_op} do not match."
     cme_name = str(cme)
     print_good_tm_format(tm, mem_name, cme_name, layer_op_to_mem_op)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     import pickle
-    with open('../list_of_cmes.pickle', 'rb') as handle:
+
+    with open("../list_of_cmes.pickle", "rb") as handle:
         list_of_cme = pickle.load(handle)
     for cme in list_of_cme:
         print_mapping(cme)
```

### Comparing `zigzag-dse-2.3.1/zigzag_dse.egg-info/PKG-INFO` & `zigzag-dse-2.3.2/zigzag_dse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 2.3.1
+Version: 2.3.2
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, ZigZag-Project
         All rights reserved.
```

### Comparing `zigzag-dse-2.3.1/zigzag_dse.egg-info/SOURCES.txt` & `zigzag-dse-2.3.2/zigzag_dse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 zigzag/classes/cacti/cacti_master/technology.cc
 zigzag/classes/cacti/cacti_master/uca.cc
 zigzag/classes/cacti/cacti_master/uca.h
 zigzag/classes/cacti/cacti_master/version_cacti.h
 zigzag/classes/cacti/cacti_master/wire.cc
 zigzag/classes/cacti/cacti_master/wire.h
 zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-310.pyc
-zigzag/classes/cacti/cacti_master/__pycache__/cacti_config_creator.cpython-38.pyc
 zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
 zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
 zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
 zigzag/classes/cacti/cacti_master/obj_dbg/area.o
 zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
 zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
 zigzag/classes/cacti/cacti_master/obj_dbg/cacti
@@ -147,27 +146,24 @@
 zigzag/classes/hardware/architecture/accelerator.py
 zigzag/classes/hardware/architecture/adder_hierarchy.py
 zigzag/classes/hardware/architecture/core.py
 zigzag/classes/hardware/architecture/dimension.py
 zigzag/classes/hardware/architecture/memory_hierarchy.py
 zigzag/classes/hardware/architecture/memory_instance.py
 zigzag/classes/hardware/architecture/memory_level.py
-zigzag/classes/hardware/architecture/operand_spatial_sharing.py
 zigzag/classes/hardware/architecture/operational_array.py
 zigzag/classes/hardware/architecture/operational_unit.py
-zigzag/classes/hardware/architecture/runtime_mode.py
 zigzag/classes/io/accelerator/parser.py
 zigzag/classes/io/onnx/conv.py
 zigzag/classes/io/onnx/default.py
 zigzag/classes/io/onnx/gemm.py
 zigzag/classes/io/onnx/matmul.py
 zigzag/classes/io/onnx/model.py
 zigzag/classes/io/onnx/parser.py
 zigzag/classes/io/onnx/utils.py
-zigzag/classes/mapping/__init__.py
 zigzag/classes/mapping/combined_mapping.py
 zigzag/classes/mapping/loop.py
 zigzag/classes/mapping/mapping_assist_funcs.py
 zigzag/classes/mapping/memory/data_layout.py
 zigzag/classes/mapping/spatial/spatial_mapping.py
 zigzag/classes/mapping/temporal/temporal_loop.py
 zigzag/classes/mapping/temporal/temporal_mapping.py
@@ -208,20 +204,19 @@
 zigzag/inputs/examples/hardware/Tesla_NPU_like.py
 zigzag/inputs/examples/mapping/alexnet_on_tpu_like.py
 zigzag/inputs/examples/mapping/assend_like.py
 zigzag/inputs/examples/mapping/default.py
 zigzag/inputs/examples/mapping/edge_tpu_like.py
 zigzag/inputs/examples/mapping/meta_prototype_like.py
 zigzag/inputs/examples/mapping/tesla_npu_like.py
-zigzag/inputs/examples/mapping/test.py
 zigzag/inputs/examples/mapping/tpu_like.py
 zigzag/inputs/examples/workload/alexnet.onnx
 zigzag/inputs/examples/workload/mobilenetv2.onnx
+zigzag/inputs/examples/workload/resnet18.onnx
 zigzag/inputs/examples/workload/resnet18.py
-zigzag/inputs/examples/workload/test.py
 zigzag/visualization/graph/memory_hierarchy.py
 zigzag/visualization/graph/workload.py
 zigzag/visualization/results/plot_cme.py
 zigzag/visualization/results/print_mapping.py
 zigzag_dse.egg-info/PKG-INFO
 zigzag_dse.egg-info/SOURCES.txt
 zigzag_dse.egg-info/dependency_links.txt
```

