# Comparing `tmp/routingblocks-0.1.5.tar.gz` & `tmp/routingblocks-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingblocks-0.1.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "routingblocks-0.1.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `routingblocks-0.1.5.tar` & `routingblocks-0.1.7.tar`

### file list

```diff
@@ -1,287 +1,294 @@
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.clang-format
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.cmake-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.gitignore
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.5/.readthedocs.yaml
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.5/CMakeLists.txt
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.5/README.md
--rw-r--r--   0        0        0     3061 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/Evaluation.h
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/Instance.hpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/Labeling.h
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/LocalSearch.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/Operators.h
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/Solution.h
--rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/binding_helpers.hpp
--rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/large_neighborhood.h
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/include/routingblocks_bindings/utility.h
--rw-r--r--   0        0        0    17898 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/Evaluation.cpp
--rw-r--r--   0        0        0     6255 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/Instance.cpp
--rw-r--r--   0        0        0     6141 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/Labeling.cpp
--rw-r--r--   0        0        0     4063 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/LocalSearch.cpp
--rw-r--r--   0        0        0    10884 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/Operators.cpp
--rw-r--r--   0        0        0    22441 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/Solution.cpp
--rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/bindings.cpp
--rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/large_neighborhood.cpp
--rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/src/utility.cpp
--rwxr-xr-x   0        0        0      192 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubgen.py
--rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_adptw.pyi
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_alns.pyi
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_arc.pyi
--rw-r--r--   0        0        0     1862 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_evaluation.pyi
--rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_frvcp.pyi
--rw-r--r--   0        0        0      928 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_insertion_cache.pyi
--rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_instance.pyi
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_local_search.pyi
--rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_niftw.pyi
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_node.pyi
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_node_location.pyi
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_random.pyi
--rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_removal_cache.pyi
--rw-r--r--   0        0        0     1520 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_route.pyi
--rw-r--r--   0        0        0     2302 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_solution.pyi
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_types.pyi
--rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 routingblocks-0.1.5/bindings/stubs/_vertex.pyi
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/make.bat
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/adptw.rst
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/alns.rst
--rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/auxilliary.rst
--rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/concepts.rst
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/conf.py
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/development.rst
--rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/evaluation.rst
--rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/examples.rst
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/extension.rst
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/frvcp.rst
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/full_api.rst
--rw-r--r--   0        0        0    28352 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/getting_started.rst
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/index.rst
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/instance.rst
--rw-r--r--   0        0        0     2546 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/localsearch.rst
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/niftw.rst
--rw-r--r--   0        0        0      516 2022-11-09 12:37:21.000000 routingblocks-0.1.5/docs/source/solution.rst
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/alns/__init__.py
--rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/alns/__main__.py
--rw-r--r--   0        0        0     4877 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/alns/alns.py
--rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/alns/parsing.py
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/__init__.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/__main__.py
--rw-r--r--   0        0        0    18647 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/alns.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/config.json
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instance/__init__.py
--rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instance/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instance/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instance/parsing.py
--rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c101C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c104C10.txt
--rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c202C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c205C10.txt
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r102C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r103C10.txt
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r201C10.txt
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r203C10.txt
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc102C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc108C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc201C10.txt
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc205C10.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c109_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c201_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c203_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c204_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c205_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c206_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c207_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c208_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r105_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r109_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r110_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r111_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r112_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r208_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r209_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r210_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r211_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc108_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc202_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc208_21.txt
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c103C15.txt
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c106C15.txt
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c202C15.txt
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c208C15.txt
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r102C15.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r105C15.txt
--rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r202C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r209C15.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc103C15.txt
--rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc108C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc202C15.txt
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc204C15.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c101C5.txt
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c103C5.txt
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c206C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c208C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r104C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r105C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r202C5.txt
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r203C5.txt
--rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc105C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc108C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc204C5.txt
--rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc208C5.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/instances/evrptw/README.txt
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/operators/ShawMoveSelector.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/operators/ShawRelatedness.py
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/operators/SpatioTemporalRelatedness.py
--rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/operators/__init__.py
--rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/parameters.py
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/requirements.txt
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/utility/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/evrptw/utility/algorithms.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/ils/__init__.py
--rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/ils/__main__.py
--rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/ils/ils.py
--rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 routingblocks-0.1.5/examples/ils/parsing.py
--rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/CMakeLists.txt
--rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/cmake/CPM.cmake
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/cmake/tools.cmake
--rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/ADPTWEvaluation.h
--rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/FRVCP.h
--rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/Instance.h
--rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/LocalSearch.h
--rw-r--r--   0        0        0     5394 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/NIFTWEvaluation.h
--rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/Solution.h
--rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/adaptive_large_neighborhood.hpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/arc.h
--rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/evaluation.h
--rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/insertion_cache.h
--rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/lns_operators.h
--rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/node.h
--rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/operators/InsertStationOperator.h
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
--rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/operators/RemoveStationOperator.h
--rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/operators/SwapOperator.h
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/operators.h
--rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/removal_cache.h
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/types.h
--rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/adaptive_priority_list.h
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/algorithms.h
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/arc_set.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/heap.h
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/iterator_pair.h
--rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/utility/random.h
--rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/include/routingblocks/vertex.h
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/CMakeLists.txt
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/dynamic_bitset/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/dynamic_bitset/LICENSE.txt
--rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
--rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/small_vector/CMakeLists.txt
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/small_vector/LICENSE.txt
--rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/small_vector/small_vector/small_vector.hpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/xoshiro/CMakeLists.txt
--rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/xoshiro/LICENSE.txt
--rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/lib/xoshiro/xoshiro/xoshiro.h
--rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/ADPTWEvaluation.cpp
--rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/FRVCP.cpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/Instance.cpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/LocalSearch.cpp
--rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/NIFTWEvaluation.cpp
--rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/Solution.cpp
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/adaptive_large_neighborbood.cpp
--rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/lns_operators.cpp
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/node.cpp
--rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/operators/InsertStationOperator.cpp
--rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/src/operators/InterRouteTwoOptOperator.cpp
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/test/CMakeLists.txt
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.5/native/test/src/dummy.cpp
--rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 routingblocks-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/__init__.py
--rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/__init__.py
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/best_insert.py
--rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/cluster_removal.py
--rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/move_selectors.py
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/related_removal.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/route_removal.py
--rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/station_vicinity_removal.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/operators/worst_removal.py
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/utility/__init__.py
--rw-r--r--   0        0        0     2909 2022-11-09 12:37:21.000000 routingblocks-0.1.5/routingblocks/utility/instance_builder.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/reference/insertion_cache.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/reference/removal_cache.py
--rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_frvcp.py
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_local_search.py
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_removal_cache.py
--rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_route_update.py
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/conftest.py
--rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/data/c101C5.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/data/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/data/r101_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/data/r201_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/data/rc101_21.txt
--rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/fixtures/mock_evaluation.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/helpers/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/helpers/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/helpers/parsing.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/__init__.py
--rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_cluster_removal.py
--rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_random_insertion.py
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_random_removal.py
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_related_removal.py
--rw-r--r--   0        0        0     1782 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_station_insertion.py
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_station_removal.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_station_vicinity_removal.py
--rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/operators/test_swap.py
--rw-r--r--   0        0        0     3858 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_evaluation.py
--rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_frvcp.py
--rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_insertion_cache.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_large_neighborhood.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_lns_helpers.py
--rw-r--r--   0        0        0     2644 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_local_search.py
--rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_node.py
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_removal_cache.py
--rw-r--r--   0        0        0    14162 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_route.py
--rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.5/test/tests/test_solution.py
--rw-r--r--   0        0        0     3007 2022-11-09 12:37:21.000000 routingblocks-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.clang-format
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.cmake-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.gitignore
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.7/CMakeLists.txt
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.7/README.md
+-rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Evaluation.h
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Instance.hpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Labeling.h
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/LocalSearch.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Operators.h
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/Solution.h
+-rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/binding_helpers.hpp
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/large_neighborhood.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/specializations/ADPTW.h
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/specializations/NIFTW.h
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/include/routingblocks_bindings/utility.h
+-rw-r--r--   0        0        0    15827 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Evaluation.cpp
+-rw-r--r--   0        0        0     5098 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Instance.cpp
+-rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Labeling.cpp
+-rw-r--r--   0        0        0     4063 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/LocalSearch.cpp
+-rw-r--r--   0        0        0    10884 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Operators.cpp
+-rw-r--r--   0        0        0    22684 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/Solution.cpp
+-rw-r--r--   0        0        0     1345 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/bindings.cpp
+-rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/large_neighborhood.cpp
+-rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/specializations/ADPTW.cpp
+-rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/specializations/NIFTW.cpp
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/src/utility.cpp
+-rw-r--r--   0        0        0     3693 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_adptw.pyi
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_alns.pyi
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_arc.pyi
+-rw-r--r--   0        0        0     8809 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_evaluation.pyi
+-rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_frvcp.pyi
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_insertion_cache.pyi
+-rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_instance.pyi
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_local_search.pyi
+-rw-r--r--   0        0        0     3834 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_niftw.pyi
+-rw-r--r--   0        0        0     4184 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_node.pyi
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_node_location.pyi
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_random.pyi
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_removal_cache.pyi
+-rw-r--r--   0        0        0     8771 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_route.pyi
+-rw-r--r--   0        0        0    10819 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_solution.pyi
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_types.pyi
+-rw-r--r--   0        0        0     1961 2022-11-09 12:37:21.000000 routingblocks-0.1.7/bindings/stubs/_vertex.pyi
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/make.bat
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/adptw.rst
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/alns.rst
+-rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/auxilliary.rst
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/concepts.rst
+-rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/conf.py
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/development.rst
+-rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/evaluation.rst
+-rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/examples.rst
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/extension.rst
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/frvcp.rst
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/full_api.rst
+-rw-r--r--   0        0        0    28336 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      626 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/index.rst
+-rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/instance.rst
+-rw-r--r--   0        0        0     2546 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/localsearch.rst
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/niftw.rst
+-rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/references.bib
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/references.rst
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 routingblocks-0.1.7/docs/source/solution.rst
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/__init__.py
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/__main__.py
+-rw-r--r--   0        0        0     4884 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/alns.py
+-rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/alns/parsing.py
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/__init__.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/__main__.py
+-rw-r--r--   0        0        0    18907 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/alns.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/config.json
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instance/parsing.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c101C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c104C10.txt
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c202C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c205C10.txt
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r102C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r103C10.txt
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r201C10.txt
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r203C10.txt
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc102C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc108C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc201C10.txt
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc205C10.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c109_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c201_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c203_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c204_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c205_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c206_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c207_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c208_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r105_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r109_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r110_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r111_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r112_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r208_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r209_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r210_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r211_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc108_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc202_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc208_21.txt
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c103C15.txt
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c106C15.txt
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c202C15.txt
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c208C15.txt
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r102C15.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r105C15.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r202C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r209C15.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc103C15.txt
+-rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc108C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc202C15.txt
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc204C15.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c101C5.txt
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c103C5.txt
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c206C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c208C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r104C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r105C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r202C5.txt
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r203C5.txt
+-rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc105C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc108C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc204C5.txt
+-rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc208C5.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/instances/evrptw/README.txt
+-rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/ShawMoveSelector.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/ShawRelatedness.py
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/SpatioTemporalRelatedness.py
+-rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/operators/__init__.py
+-rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/parameters.py
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/requirements.txt
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/utility/__init__.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/evrptw/utility/algorithms.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/__init__.py
+-rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/__main__.py
+-rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/ils.py
+-rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 routingblocks-0.1.7/examples/ils/parsing.py
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/cmake/CPM.cmake
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/cmake/tools.cmake
+-rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/ADPTWEvaluation.h
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/FRVCP.h
+-rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/Instance.h
+-rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/LocalSearch.h
+-rw-r--r--   0        0        0    10459 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/NIFTWEvaluation.h
+-rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/Solution.h
+-rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/adaptive_large_neighborhood.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/arc.h
+-rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/evaluation.h
+-rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/insertion_cache.h
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/lns_operators.h
+-rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/node.h
+-rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/InsertStationOperator.h
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
+-rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/RemoveStationOperator.h
+-rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators/SwapOperator.h
+-rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/operators.h
+-rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/removal_cache.h
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/types.h
+-rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/adaptive_priority_list.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/algorithms.h
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/arc_set.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/heap.h
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/iterator_pair.h
+-rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/utility/random.h
+-rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/include/routingblocks/vertex.h
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/LICENSE.txt
+-rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
+-rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/LICENSE.txt
+-rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/small_vector/small_vector/small_vector.hpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/CMakeLists.txt
+-rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/LICENSE.txt
+-rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/lib/xoshiro/xoshiro/xoshiro.h
+-rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/ADPTWEvaluation.cpp
+-rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/FRVCP.cpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/Instance.cpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/LocalSearch.cpp
+-rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/NIFTWEvaluation.cpp
+-rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/Solution.cpp
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/adaptive_large_neighborbood.cpp
+-rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/lns_operators.cpp
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/node.cpp
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/operators/InsertStationOperator.cpp
+-rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/src/operators/InterRouteTwoOptOperator.cpp
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/test/CMakeLists.txt
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.7/native/test/src/dummy.cpp
+-rw-r--r--   0        0        0     1860 2022-11-09 12:37:21.000000 routingblocks-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/adptw/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/niftw/__init__.py
+-rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/__init__.py
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/best_insert.py
+-rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/cluster_removal.py
+-rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/move_selectors.py
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/related_removal.py
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/route_removal.py
+-rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/station_vicinity_removal.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/operators/worst_removal.py
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/utility/__init__.py
+-rw-r--r--   0        0        0     5849 2022-11-09 12:37:21.000000 routingblocks-0.1.7/routingblocks/utility/instance_builder.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/reference/insertion_cache.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/reference/removal_cache.py
+-rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_frvcp.py
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_local_search.py
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_removal_cache.py
+-rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_route_update.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/c101C5.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/r101_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/r201_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/data/rc101_21.txt
+-rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/fixtures/mock_evaluation.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/helpers/parsing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/__init__.py
+-rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_cluster_removal.py
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_random_insertion.py
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_random_removal.py
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_related_removal.py
+-rw-r--r--   0        0        0     1782 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_insertion.py
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_removal.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_station_vicinity_removal.py
+-rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/operators/test_swap.py
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_evaluation.py
+-rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_frvcp.py
+-rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_insertion_cache.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_large_neighborhood.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_lns_helpers.py
+-rw-r--r--   0        0        0     2644 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_local_search.py
+-rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_node.py
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_removal_cache.py
+-rw-r--r--   0        0        0    14114 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_route.py
+-rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.7/test/tests/test_solution.py
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 routingblocks-0.1.7/PKG-INFO
```

### Comparing `routingblocks-0.1.5/.cmake-format` & `routingblocks-0.1.7/.cmake-format`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/.github/workflows/wheels.yml` & `routingblocks-0.1.7/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/.gitignore` & `routingblocks-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/CONTRIBUTING.md` & `routingblocks-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/README.md` & `routingblocks-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/CMakeLists.txt` & `routingblocks-0.1.7/bindings/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -45,26 +45,23 @@
 # Set the compiler standard
 #
 target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_20)
 
 # Create stub file
 file(GLOB stub_files CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/stubs/*.pyi")
 
-function(cat IN_FILE OUT_FILE)
-    file(READ ${IN_FILE} CONTENTS)
-    file(APPEND ${OUT_FILE} "${CONTENTS}")
-endfunction()
-# Prepare a temporary file to "cat" to:
-file(WRITE ${CMAKE_CURRENT_SOURCE_DIR}/_routingblocks.pyi.in "")
+# Generate an empty target file
+file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi "")
 
-# Call the "cat" function for each input file
-foreach (STUB_FILE ${stub_files})
-    cat(${STUB_FILE} _routingblocks.pyi.in)
-endforeach ()
+add_custom_command(
+    OUTPUT ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi
+    COMMAND ${CMAKE_COMMAND} -E echo "Concatenating files..."
+    COMMAND ${CMAKE_COMMAND} -E cat ${stub_files} > "${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi"
+    DEPENDS ${stub_files}
+)
 
-# Copy the temporary file to the final location
-configure_file(${CMAKE_CURRENT_SOURCE_DIR}/_routingblocks.pyi.in ${CMAKE_CURRENT_SOURCE_DIR}/_routingblocks.pyi COPYONLY)
-message(STATUS "Created stub file: ${CMAKE_CURRENT_SOURCE_DIR}/_routingblocks.pyi")
+add_custom_target(stub_file ALL DEPENDS ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi)
+add_dependencies(${PROJECT_NAME} stub_file)
 
 INSTALL(TARGETS routingblocks DESTINATION routingblocks)
 INSTALL(FILES ${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks_bindings/binding_helpers.hpp DESTINATION routingblocks/include/routingblocks/)
-INSTALL(FILES ${CMAKE_CURRENT_SOURCE_DIR}/_routingblocks.pyi DESTINATION routingblocks/)
+INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/_routingblocks.pyi DESTINATION routingblocks/)
```

### Comparing `routingblocks-0.1.5/bindings/include/routingblocks_bindings/binding_helpers.hpp` & `routingblocks-0.1.7/bindings/include/routingblocks_bindings/binding_helpers.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -52,10 +52,24 @@
                                      std::make_shared<data_t>(std::move(user_data)));
     }
 
     template <class data_t> routingblocks::Arc arc_constructor(data_t user_data) {
         return routingblocks::Arc(std::make_shared<data_t>(std::move(user_data)));
     }
 
+    template <class T, class Binding>
+    auto bind_concatenation_evaluation_specialization(Binding& evaluation) {
+        using fwd_label_t = typename T::fwd_label_t;
+        using bwd_label_t = typename T::bwd_label_t;
+        return evaluation.def("propagate_forward", &T::propagate_forward)
+            .def("propagate_backward", &T::propagate_backward)
+            .def("concatenate", &T::concatenate)
+            .def("compute_cost", &T::compute_cost)
+            .def("is_feasible", &T::is_feasible)
+            .def("get_cost_components", &T::get_cost_components)
+            .def("create_forward_label", &T::create_forward_label)
+            .def("create_backward_label", &T::create_backward_label);
+    }
+
 }  // namespace bindings::helpers
 
 #endif
```

### Comparing `routingblocks-0.1.5/bindings/src/Evaluation.cpp` & `routingblocks-0.1.7/bindings/src/Evaluation.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -305,47 +305,13 @@
             .def("compute_cost", &PyEvaluation::py_compute_cost)
             .def("get_cost_components", &PyEvaluation::py_get_cost_components)
             .def("is_feasible", &PyEvaluation::py_is_feasible)
             .def("create_forward_label", &PyEvaluation::py_create_forward_label)
             .def("create_backward_label", &PyEvaluation::py_create_backward_label);
     }
 
-    template <class T, class Binding>
-    auto bind_concatenation_evaluation_specialization(Binding& evaluation) {
-        using fwd_label_t = typename T::fwd_label_t;
-        using bwd_label_t = typename T::bwd_label_t;
-        return evaluation.def("propagate_forward", &T::propagate_forward)
-            .def("propagate_backward", &T::propagate_backward)
-            .def("concatenate", &T::concatenate)
-            .def("compute_cost", &T::compute_cost)
-            .def("is_feasible", &T::is_feasible)
-            .def("get_cost_components", &T::get_cost_components)
-            .def("create_forward_label", &T::create_forward_label)
-            .def("create_backward_label", &T::create_backward_label);
-    }
-
     void bind_evaluation(pybind11::module& m) {
         auto evaluation_interface = bind_evaluation_interface(m);
         bind_py_evaluation(m, evaluation_interface);
-
-        auto adptw_module = m.def_submodule("adptw");
-        bind_concatenation_evaluation_specialization<ADPTWEvaluation>(
-            pybind11::class_<ADPTWEvaluation, std::shared_ptr<ADPTWEvaluation>>(
-                adptw_module, "Evaluation", evaluation_interface)
-                .def(pybind11::init<resource_t, resource_t>()))
-            .def_readwrite("overload_penalty_factor", &ADPTWEvaluation::overload_penalty_factor)
-            .def_readwrite("overcharge_penalty_factor", &ADPTWEvaluation::overcharge_penalty_factor)
-            .def_readwrite("time_shift_penalty_factor",
-                           &ADPTWEvaluation::time_shift_penalty_factor);
-
-        auto niftw_module = m.def_submodule("niftw");
-        bind_concatenation_evaluation_specialization<NIFTWEvaluation>(
-            pybind11::class_<routingblocks::NIFTWEvaluation, std::shared_ptr<NIFTWEvaluation>>(
-                niftw_module, "Evaluation", evaluation_interface)
-                .def(pybind11::init<resource_t, resource_t, resource_t>()))
-            .def_readwrite("overload_penalty_factor", &NIFTWEvaluation::overload_penalty_factor)
-            .def_readwrite("overcharge_penalty_factor", &NIFTWEvaluation::overcharge_penalty_factor)
-            .def_readwrite("time_shift_penalty_factor",
-                           &NIFTWEvaluation::time_shift_penalty_factor);
     }
 
 }  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.5/bindings/src/Instance.cpp` & `routingblocks-0.1.7/bindings/src/Instance.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -35,40 +35,25 @@
                 "classes defined in Python.");
     }
 
     void bind_routingblocks_instance(pybind11::module& m) {
         bind_vertex<pybind11::object>(m, "Vertex");
         bind_arc<pybind11::object>(m, "Arc");
 
-        auto adptw = m.def_submodule("adptw");
-        pybind11::class_<routingblocks::ADPTWVertexData>(adptw, "ADPTWVertexData")
-            .def(pybind11::init<float, float, resource_t, resource_t, resource_t, resource_t>());
-        pybind11::class_<routingblocks::ADPTWArcData>(adptw, "ADPTWArcData")
-            .def(pybind11::init<resource_t, resource_t, resource_t>());
-        adptw.def("create_adptw_vertex", &::bindings::helpers::vertex_constructor<ADPTWVertexData>);
-        adptw.def("create_adptw_arc", &::bindings::helpers::arc_constructor<ADPTWArcData>);
-
-        auto niftw = m.def_submodule("niftw");
-        pybind11::class_<routingblocks::NIFTWVertexData>(niftw, "NIFTWVertexData")
-            .def(pybind11::init<float, float, resource_t, resource_t, resource_t, resource_t>());
-        pybind11::class_<routingblocks::NIFTWArcData>(niftw, "NIFTWArcData")
-            .def(pybind11::init<resource_t, resource_t, resource_t>());
-        niftw.def("create_niftw_vertex", &::bindings::helpers::vertex_constructor<NIFTWVertexData>);
-        niftw.def("create_niftw_arc", &::bindings::helpers::arc_constructor<NIFTWArcData>);
-
         pybind11::class_<routingblocks::Instance>(m, "Instance")
             .def(pybind11::init<std::vector<routingblocks::Vertex>,
                                 std::vector<std::vector<routingblocks::Arc>>>())
             .def(pybind11::init<std::vector<routingblocks::Vertex>,
                                 std::vector<std::vector<routingblocks::Arc>>, int>())
             .def(pybind11::init<routingblocks::Vertex, std::vector<routingblocks::Vertex>,
                                 std::vector<routingblocks::Vertex>,
                                 std::vector<std::vector<routingblocks::Arc>>, int>())
-            .def_property_readonly("fleet_size", &routingblocks::Instance::FleetSize, "The number of "
-                                                                                     "vehicles available.")
+            .def_property_readonly("fleet_size", &routingblocks::Instance::FleetSize,
+                                   "The number of "
+                                   "vehicles available.")
             .def_property_readonly("number_of_customers",
                                    &routingblocks::Instance::NumberOfCustomers)
             .def_property_readonly("number_of_stations", &routingblocks::Instance::NumberOfStations)
             .def_property_readonly("number_of_vertices", &routingblocks::Instance::NumberOfVertices)
             .def_property_readonly("depot", &routingblocks::Instance::Depot, "The depot vertex.")
             .def_property_readonly("stations",
                                    [](const routingblocks::Instance& inst) {
```

### Comparing `routingblocks-0.1.5/bindings/src/Labeling.cpp` & `routingblocks-0.1.7/bindings/src/Labeling.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -90,45 +90,20 @@
                  "Returns true if the label is final, i.e., the path is complete.")
             .def("prepare", &PropagatorClass::prepare, "Prepares the propagator for a new route.")
             .def("create_root_label", &PropagatorClass::create_root_label,
                  "Creates the root label for the propagator.");
     }
 
     void bind_labeling(pybind11::module_& m) {
-        auto adptw = m.def_submodule("adptw");
-        pybind11::class_<FRVCP<ADPTWLabel>>(adptw, "FRVCP")
-            .def(pybind11::init<>([](const Instance& instance, resource_t battery_capacity) {
-                return FRVCP<ADPTWLabel>(
-                    instance, std::make_shared<Propagator<ADPTWLabel>>(instance, battery_capacity));
-            }))
-            .def("optimize", &FRVCP<ADPTWLabel>::optimize, "Solve FRVCP for the specified route.");
-
         auto propagator_interface
             = pybind11::class_<PyPropagator, PyPropagatorTramboline, std::shared_ptr<PyPropagator>>(
                   m, "Propagator")
                   .def(pybind11::init<>());
         bind_propagator<PyPropagator>(propagator_interface);
 
         pybind11::class_<FRVCP<PyPropagator::value_type>>(m, "FRVCP")
             .def(pybind11::init<const Instance&, std::shared_ptr<PyPropagator>>())
             .def("optimize", &FRVCP<PyPropagator::value_type>::optimize,
                  "Solve FRVCP for the specified route.");
-
-        /*auto propagator_interface
-            = bind_propagator<routingblocks::Propagator, PyPropagator>(m, "Propagator")
-                  .def(pybind11::init<>());
-
-        bind_propagator<routingblocks::ADPTWPropagation>(m, "ADPTWPropagation",
-        propagator_interface) .def(pybind11::init<const routingblocks::Instance&>());
-
-        m.def("create_adptw_propagator", [](const routingblocks::Instance& instance) {
-            return std::make_shared<routingblocks::ADPTWPropagation>(instance);
-        });
-
-        pybind11::class_<routingblocks::Label, std::shared_ptr<routingblocks::Label>>(m, "DPLabel",
-                                                                        pybind11::dynamic_attr())
-            .def(pybind11::init<>());
-
-        */
     }
 
 }  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.5/bindings/src/LocalSearch.cpp` & `routingblocks-0.1.7/bindings/src/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/src/Operators.cpp` & `routingblocks-0.1.7/bindings/src/Operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/src/Solution.cpp` & `routingblocks-0.1.7/bindings/src/Solution.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -63,28 +63,29 @@
                 "Backward label at the node", pybind11::return_value_policy::reference_internal)
             .def_property_readonly("__str__", &routingblocks::Node::vertex_strid);
     }
 
     void bind_route(pybind11::module& m) {
         pybind11::class_<routingblocks::Route>(m, "Route")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&>(),
-                 "Creates an empty route.")
+                 pybind11::keep_alive<1, 2>(), "Creates an empty route.")
             .def_property_readonly("cost", &routingblocks::Route::cost, "The cost of the route.")
             .def_property_readonly("cost_components", &routingblocks::Route::cost_components,
                                    "The cost components of the route.")
             .def_property_readonly("feasible", &routingblocks::Route::feasible,
                                    "Whether the route is feasible.")
             .def_property_readonly("empty", &routingblocks::Route::empty,
                                    "Whether the route is empty.")
             .def_property_readonly("modification_timestamp",
                                    &routingblocks::Route::modification_timestamp,
                                    "The route modification_timestamp. May be used for caching.")
             .def("__len__", &routingblocks::Route::size, "The number of vertices in the route.")
             .def("__copy__", [](const Route& r) { return Route(r); })
-            .def("__deepcopy__", [](const Route& r, const pybind11::dict&) { return Route(r); })
+            .def("copy", [](const Route& r) { return Route(r); })
+            .def("__deepcopy__", [](const Route& r, const pybind11::dict*) { return Route(r); })
             .def_property_readonly(
                 "end_depot",
                 [](const Route& r) -> const routingblocks::Node& { return *r.end_depot(); },
                 "The depot at the end of the route.",
                 pybind11::return_value_policy::reference_internal)
             .def_property_readonly(
                 "depot", [](const Route& r) -> const routingblocks::Node& { return *r.begin(); },
@@ -125,20 +126,21 @@
                 [](Route& route, size_t pos, const std::vector<Node>& nodes) {
                     auto ret = route.insert_segment_after(std::next(route.begin(), pos),
                                                           nodes.begin(), nodes.end());
                     return std::distance(route.begin(), ret);
                 },
                 "Inserts the given nodes after the given position.")
             .def("insert_vertices_after",
-                 [](Route& route, pybind11::iterable& vertex_ids_and_locations_list) {
+                 [](Route& route, pybind11::iterable& vertex_ids_and_positions_list) {
                      std::vector<std::pair<VertexID, NodeLocation>> vertex_ids_and_locations;
 
-                     for (const auto& vertex_id_and_location : vertex_ids_and_locations_list) {
-                         vertex_ids_and_locations.push_back(
-                             vertex_id_and_location.cast<std::pair<VertexID, NodeLocation>>());
+                     for (const auto& vertex_id_and_position_iter : vertex_ids_and_positions_list) {
+                         auto [v_id, pos]
+                             = vertex_id_and_position_iter.cast<std::pair<VertexID, int>>();
+                         vertex_ids_and_locations.emplace_back(v_id, NodeLocation(0, pos));
                      }
 
                      route.insert_vertices_after(vertex_ids_and_locations.begin(),
                                                  vertex_ids_and_locations.end());
                  })
             .def("exchange_segments",
                  [](Route& route, size_t begin_pos, size_t end_pos, size_t other_begin_pos,
@@ -205,14 +207,15 @@
                                    "The cost of the solution.")
             .def_property_readonly("cost_components", &routingblocks::Solution::cost_components,
                                    "The cost components of the solution.")
             .def_property_readonly("feasible", &routingblocks::Solution::feasible,
                                    "Whether the solution is "
                                    "feasible.")
             .def("__copy__", [](const Solution& s) { return Solution(s); })
+            .def("copy", [](const Solution& s) { return Solution(s); })
             .def("__deepcopy__",
                  [](const Solution& s, const pybind11::dict&) -> Solution { return Solution(s); })
             .def(
                 "__iter__",
                 [](const Solution& solution) {
                     return pybind11::make_iterator(solution.begin(), solution.end());
                 },
```

### Comparing `routingblocks-0.1.5/bindings/src/bindings.cpp` & `routingblocks-0.1.7/bindings/src/bindings.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 #include <routingblocks_bindings/Operators.h>
 #include <routingblocks_bindings/Solution.h>
 #include <routingblocks_bindings/large_neighborhood.h>
 #include <routingblocks_bindings/utility.h>
 
 #include <routingblocks_bindings/Instance.hpp>
 
+#include "routingblocks_bindings/specializations/ADPTW.h"
+#include "routingblocks_bindings/specializations/NIFTW.h"
+
 using namespace routingblocks::bindings;
 
 #define STRINGIFY(x) #x
 #define PREPROCESSOR_TO_STRING(x) STRINGIFY(x)
 
 #ifndef routingblocks_VERSION
 #    define routingblocks_VERSION "dev"
@@ -39,10 +42,14 @@
     bind_route(m);
     bind_solution(m);
     bind_solution_functions(m);
 
     // Labeling
     bind_labeling(m);
 
-    // routingblocks
+    // ALNS
     bind_large_neighborhood(m);
+
+    // Specializations
+    bind_adptw(m);
+    bind_niftw(m);
 }
```

### Comparing `routingblocks-0.1.5/bindings/src/large_neighborhood.cpp` & `routingblocks-0.1.7/bindings/src/large_neighborhood.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/src/utility.cpp` & `routingblocks-0.1.7/bindings/src/utility.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/stubs/_alns.pyi` & `routingblocks-0.1.7/bindings/stubs/_alns.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/stubs/_frvcp.pyi` & `routingblocks-0.1.7/bindings/stubs/_frvcp.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/stubs/_insertion_cache.pyi` & `routingblocks-0.1.7/bindings/stubs/_insertion_cache.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class InsertionMove:
     vertex_id: VertexID
     after_node: NodeLocation
-    delta_cost: cost_t
+    delta_cost: float
 
-    def __init__(self, vertex_id: VertexID, after_node_location: NodeLocation, delta_cost: cost_t) -> None: ...
+    def __init__(self, vertex_id: VertexID, after_node_location: NodeLocation, delta_cost: float) -> None: ...
 
     def __eq__(self, other: InsertionMove) -> bool: ...
 
 
 class InsertionCache:
     def __init__(self, instance: Instance) -> None: ...
```

### Comparing `routingblocks-0.1.5/bindings/stubs/_local_search.pyi` & `routingblocks-0.1.7/bindings/stubs/_local_search.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/bindings/stubs/_removal_cache.pyi` & `routingblocks-0.1.7/bindings/stubs/_removal_cache.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class RemovalMove:
     vertex_id: VertexID
     node_location: NodeLocation
-    delta_cost: cost_t
+    delta_cost: float
 
-    def __init__(self, vertex_id: VertexID, node_location: NodeLocation, delta_cost: cost_t) -> None: ...
+    def __init__(self, vertex_id: VertexID, node_location: NodeLocation, delta_cost: float) -> None: ...
 
     def __eq__(self, other: RemovalMove) -> bool: ...
 
 
 class RemovalCache:
     def __init__(self, instance: Instance) -> None: ...
```

### Comparing `routingblocks-0.1.5/docs/make.bat` & `routingblocks-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/docs/source/alns.rst` & `routingblocks-0.1.7/docs/source/alns.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/docs/source/auxilliary.rst` & `routingblocks-0.1.7/docs/source/auxilliary.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/docs/source/conf.py` & `routingblocks-0.1.7/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,30 +22,37 @@
 
 extensions = [
     'autoapi.extension',
     'sphinx.ext.autodoc',
     'sphinx.ext.autodoc.typehints',
     'sphinx.ext.autosummary',
     'sphinx.ext.duration',
-    'sphinx.ext.doctest'
+    'sphinx.ext.doctest',
+    'sphinxcontrib.bibtex'
 ]
 
+# AutoAPI
+
 autosummary_generate = True
 autoapi_type = "python"
 autoapi_dirs = [str(routingblocks_import_path)]
 autoapi_options = ["undoc-members", "members", "special-members"]
 
 autoapi_generate_api_docs = False
 autoapi_add_toctree_entry = False
 autoapi_add_objects_to_toctree = False
 
 autoapi_python_class_content = "class"
 autoapi_member_order = "bysource"
+autodoc_member_order = "bysource"
+
+autodoc_typehints = "both"
 
-autodoc_typehints = "description"
+# Bibtex
+bibtex_bibfiles = ['references.bib']
 
 templates_path = ['_templates']
 exclude_patterns = []
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `routingblocks-0.1.5/docs/source/development.rst` & `routingblocks-0.1.7/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/docs/source/getting_started.rst` & `routingblocks-0.1.7/docs/source/getting_started.rst`

 * *Files 6% similar despite different names*

```diff
@@ -32,38 +32,39 @@
     def parse_instance(instance_path: Path):
         str_fields = ['StringID', 'Type']
         with open(instance_path) as instance_stream:
             fields = instance_stream.readline().split()
             # Parse the vertices
             vertices = []
             for line in instance_stream:
-                if len(line) == 0:
+                tokens = line.split()
+                if len(tokens) == 0:
                     break
-                vertex = {key: (x if key in str_fields else float(x)) for key, x in zip(fields, line.split())}
+                # Read columns into a dictionary
+                vertex = {key: (x if key in str_fields else float(x)) for key, x in zip(fields, tokens)}
                 vertices.append(vertex)
             # Parse the parameters
             parameters = {}
             for line in instance_stream:
                 key, *_, value = line.split()
                 # Remove surrounding / characters and parse the value
                 parameters[key] = float(value[1:-1])
 
-        # Create a matrix of arcs
-        arcs = []
+        # Create a mapping from pairs of vertices to arcs
+        arcs = {}
         for i in vertices:
-            next_row = []
             for j in vertices:
                 # Compute distance
                 distance = sqrt((i['x'] - j['x']) ** 2 + (i['y'] - j['y']) ** 2)
                 # Compute travel time (distance / average velocity)
                 travel_time = distance / parameters['v']
                 # Compute consumption (consumption rate * travel time / recharging rate)
                 consumption = parameters['r'] * travel_time / parameters['g']
-                next_row.append(dict(distance=distance, travel_time=travel_time, consumption=consumption))
-            arcs.append(next_row)
+                arcs[i['StringID'], j['StringID']] = dict(distance=distance, travel_time=travel_time,
+                                                          consumption=consumption)
 
         return vertices, arcs, parameters
 
 .. note::
 
     The instance format is described in the `supplemental material <https://data.mendeley.com/datasets/h3mrm5dhxw/1>`_ to `Schneider et. al (2014) <https://pubsonline.informs.org/doi/abs/10.1287/trsc.2013.0490>`_.
 
@@ -73,43 +74,42 @@
 
     def create_instance(serialized_vertices, serialized_arcs) -> rb.Instance:
         instance_builder = rb.utility.InstanceBuilder(create_vertex=rb.adptw.create_adptw_vertex,
                                                       create_arc=rb.adptw.create_adptw_arc)
         # Create and register the vertices
         for vertex in serialized_vertices:
             # Create problem-specific data held by vertices
-            vertex_data = rb.adptw.ADPTWVertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
+            vertex_data = rb.adptw.VertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
                                                    vertex['DueDate'],
                                                    vertex['ServiceTime'])
             # Register the vertex dependinx for x in self._move_selector(related_vertices)g on it's type
             if vertex['Type'] == 'd':
                 instance_builder.set_depot(vertex['StringID'], vertex_data)
             elif vertex['Type'] == 'c':
                 instance_builder.add_customer(vertex['StringID'], vertex_data)
             else:
                 instance_builder.add_station(vertex['StringID'], vertex_data)
 
         # Create and register the arcs
         for (i, j), arc in serialized_arcs.items():
             # Create problem-specific data held by arcs
-            arc_data = rb.adptw.ADPTWArcData(arc['distance'], arc['consumption'], arc['travel_time'])
+            arc_data = rb.adptw.ArcData(arc['distance'], arc['consumption'], arc['travel_time'])
             instance_builder.add_arc(i, j, arc_data)
 
         # Create instance
         return instance_builder.build()
 
 
 .. note::
 
     RoutingBlocks does not store parameters in the Instance object.
 
-We use the InstanceBuilder class, which provides a convenient way to build a RoutingBlocks Instance from a set of vertices and arcs. It takes two functions as arguments: a vertex and an arc factory. These create a vertex or an arc object from the data provided by the user. The InstanceBuilder class then takes care of registering the vertices and arcs in the Instance object.
+We utilize the InstanceBuilder class, offering a convenient way to construct a RoutingBlocks Instance from a set of vertices and arcs. It requires two functions as arguments: a vertex and an arc factory. These functions create a vertex or an arc object based on the data provided by the user. The InstanceBuilder class then handles the registration of vertices and arcs within the Instance object.
 
-
-Having created the instance, we can now implement the ILS algorithm. We start by creating an Evaluation object, which will be responsible for cost calculation and efficient move evaluation. RoutingBlocks already provides a Evaluation class for the EVRP-TW-PR, so we can simply use it:
+Once the instance is created, we can proceed to implement the ILS algorithm. We initiate by creating an Evaluation object, which is responsible for cost calculation and efficient move evaluation. RoutingBlocks already includes an Evaluation class for the EVRP-TW-PR, allowing us to easily use it:
 
 .. note::
 
         It is possible to implement a custom Evaluation class for custom problem settings (See `Custom problem settings <_custom_problem_settings>`_)
 
 .. code-block:: python
 
@@ -123,15 +123,15 @@
     # vehicle capacity, and the charge constraints
     evaluation.overload_penalty_factor = 100.
     evaluation.overcharge_penalty_factor = 100.
     evaluation.time_shift_penalty_factor = 100.
 
 .. note::
 
-    The namespace name ``adptw`` refers to the classification introduced in `Schiffer et al. (2017) <https://www.semanticscholar.org/paper/A-solution-framework-for-the-class-of-vehicle-with-Schiffer-Klein/8eff30dda8ba9faf9aa4d814838fea20d7287203>`_.
+    The module's name ``adptw`` refers to the classification introduced in :cite:t:`vrpis`.
 
 Being done with the setup, we can start implementing the main ILS algorithm.
 We start by creating a random solution:
 
 .. code-block:: python
 
     def create_random_solution(evaluation: rb.Evaluation, instance: rb.Instance):
@@ -147,17 +147,17 @@
                   zip(split_positions, split_positions[1:])]
         # Create RoutingBlocks Route objects
         routes = [rb.create_route(evaluation, instance, route) for route in routes]
         # Create RoutingBlocks Solution object
         return rb.Solution(evaluation, instance, routes)
 
 
-Here, we start by copying all customers into a single list, which is then shuffled and split at random positions to yield a set of routes. We convert these to routingblocks Route objects using the create_route helper function, which takes as arguments the evaluation function, the instance, and a sequence of vertex ids, and creates a Route object, adding start and end depots accordingly. Finally, we create and return a solution from the list of routes.
+Here, we begin by copying all customers into a single list, which is then shuffled and randomly split at various positions to generate a set of routes. We convert these into RoutingBlocks Route objects using the create_route helper function. This function takes the evaluation function, the instance, and a sequence of vertex IDs as arguments and creates a Route object, adding start and end depots as needed. Finally, we create and return a solution using the list of routes.
 
-Next, we create and configure the local search solver:
+Subsequently, we create and configure the local search solver:
 
 .. code-block:: python
 
     local_search = rb.LocalSearch(instance, evaluation, None)
     # Configure the local search to use a best-improvement pivoting rule
     local_search.set_use_best_improvement(True)
     # Create a set of allowed arcs
@@ -168,27 +168,26 @@
         rb.operators.SwapOperator_0_1(instance, arc_set),
         rb.operators.SwapOperator_1_1(instance, arc_set),
         rb.operators.InsertStationOperator(instance),
         rb.operators.RemoveStationOperator(instance),
     ]
 
 
-The local search solver takes three arugments. The instance, the evaluation used, and a second evaluation class that is used to verify moves the first evaluation class deems profitable. This is useful for problems like the EVRP-TW-PR, where exact evaluation is expensive. The default ADPTW Evaluation class implements approximate move evaluation. We could either pass a exact evaluation class here, or we could pass None, which will cause the local search to verify moves by applying them to a copy of the solution, evaluation the cost based on forward labels. This is what we do here.
-
-We also create a set of operators that will be used later when calling the local search. The implementations provided by RoutingBlocks take a set of allowed arcs as an argument. Only arcs within this set will be considered by the operator. By default, all arcs are allowed.
+The local search solver accepts three arguments: the instance, the evaluation used, and a second evaluation object that verifies moves deemed profitable by the first evaluation class. This is beneficial for problems like EVRP-TW-PR, where exact evaluation is costly. By default, the ADPTW Evaluation class implements approximate move evaluation. We can either pass an exact evaluation class here, or we can pass None, which prompts the local search to validate moves by applying them to a solution copy and evaluating the cost based on forward labels. This is what we do here.
 
+Additionally, we create a set of operators to be used later when invoking the local search. The implementations provided by RoutingBlocks require a set of allowed arcs as an argument. The operator will only consider arcs within this set. By default, all arcs are allowed.
 Executing the local search procedure is as simple as calling
 
 .. code-block:: python
 
     local_search.optimize(solution, operators)
 
-Note that this will modify the solution object in-place.
+Be aware that this process will modify the solution object in-place.
 
-The final procedure to implement is the perturbation function. This function perturbs the local minimum found by the local search to escape local optima. We implement a simple perturbation function that exchanges a random number of segments between randomly selected routes in the solution:
+The last procedure to implement is the perturbation function. This function disturbs the local minimum identified by the local search in order to escape local optima. We implement a straightforward perturbation function that swaps a random number of segments between randomly chosen routes within the solution:
 
 .. code-block:: python
 
     def perturb(solution: rb.Solution, max_exchanges: int) -> rb.Solution:
         assert sum(1 for r in solution if not r.empty) > 1, "Cannot perturb a solution with only one route."
         # Create a new solution by copying the current solution
         new_solution = copy.copy(solution)
@@ -282,17 +281,17 @@
 
 The full source code can be found in the main `github repository <https://github.com/tumBAIS/RoutingBlocks/tree/develop/examples/ils>`_ .
 
 Extending the algorithm to an ALNS
 ------------------------------------
 .. _alns_extension:
 
-A simple ILS algorithm is often not sufficient to compete on problem settings such as the EVRP-TW-PR. Here, state of the art algorithm base on `ALNS <https://en.wikipedia.org/wiki/Adaptive_large_neighborhood_search>`_. ALNS utilizes a set of destroy and repair operators to perturb the current solution. The destroy operators remove a part of the solution, while the repair operators try to repair the solution by inserting the removed customers into the solution again. Selecting the operators is done probabilistically, with the probability of selecting an operator being proportional to the operator's performance, which is estimated based the number of times a operator improved the solution.
+A simple ILS algorithm often falls short in competitive problem settings such as the EVRP-TW-PR. In these cases, state-of-the-art algorithms rely on ALNS. ALNS employs a set of destroy and repair operators to perturb the current solution. Destroy operators remove a portion of the solution, while repair operators attempt to fix the solution by reinserting the removed customers. Operator selection is done probabilistically, with the probability of selecting an operator being proportional to its performance, which is estimated based on the number of times an operator has improved the solution.
 
-RoutingBlocks provides a ALNS solver and several destroy and repair operators out of the box. Implementing ALNS is thus straightforward:
+RoutingBlocks offers an ALNS solver and several destroy and repair operators out of the box, making the implementation of ALNS fairly straightforward:
 
 .. code-block:: python
 
     def alns(instance: rb.Instance, vehicle_storage_capacity: float, vehicle_battery_capacity_time: float,
              number_of_iterations: int = 100, min_vertex_removal_factor: float = 0.2,
              max_vertex_removal_factor: float = 0.4):
         evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
@@ -332,23 +331,25 @@
                                                                     rb.operators.blink_selector_factory(
                                                                         blink_probability=0.1, randgen=randgen)))
         alns.add_destroy_operator(rb.operators.RandomRemovalOperator(randgen))
         alns.add_destroy_operator(rb.operators.WorstRemovalOperator(instance,
                                                                     rb.operators.blink_selector_factory(
                                                                         blink_probability=0.1, randgen=randgen)))
 
-We start from the boilerplate code developed for the ILS and only add a few lines to create and configure the ALNS solver. This class is responsible for operator selection and weight adaption. It takes as arguments a random engine and a smoothing factor. The smoothing factor determines the weight of historic performance when selecting an operator. Next, we create and register destroy and repair operators with the ALNS solver. RoutingBlocks provides a `set of standard operators <alns_operators>`_ out of the box. Here, we use RandomInsertion, BestInsertion, RandomRemoval, and WorstRemoval. We configure BestInsertion and WorstRemoval to select insertion/removal spots using a blink selection criterion.
 
-We can now utilize the ALNS solver to perturb the current solution in the main loop:
+We begin with the boilerplate code established for the ILS and add just a few lines to create and configure the ALNS solver. This class is responsible for operator selection and weight adaptation. It takes a random engine and a smoothing factor as arguments. The smoothing factor determines the weight of historical performance when selecting an operator. Next, we create and register destroy and repair operators with the ALNS solver. RoutingBlocks provides a `set of standard operators <alns_operators>`_ out of the box. In this case, we use RandomInsertion, BestInsertion, RandomRemoval, and WorstRemoval. We configure BestInsertion and WorstRemoval to select insertion/removal spots using a blink selection criterion.
+
+We can now employ the ALNS solver to perturb the current solution within the main loop:
+
 
 .. code-block:: python
 
         # Generate a random starting solution
         best_solution = create_random_solution(evaluation, instance)
-        for i in range(number_of_iterations):
+        for i in range(1, number_of_iterations+1):
             current_solution = copy.copy(best_solution)
             # Perturb the current solution
             number_of_vertices_to_remove = int(random.uniform(min_vertex_removal_factor, max_vertex_removal_factor) * sum(
                 len(route) - 2 for route in current_solution))
             picked_operators = alns.generate(evaluation, current_solution, number_of_vertices_to_remove)
 
             # Search the neighborhood of the current solution. This modifies the solution in-place.
@@ -367,18 +368,19 @@
 
             # Calculate new operator weights based on the last period
             if i % 20 == 0:
                 alns.adapt_operator_weights()
 
         return best_solution
 
-We utilize three fundamental methods of the ALNS solver:
-1. alns.generate, which selects and applies a destroy and a repair operator to the current solution, modifying it in-place. The method returns a tuple of the selected operators.
-2. alns.collect_score, which collects scores for the passed operators. The method takes as arguments the selected operators and a score.
-3. alns.adapt_operator_weights, which adapts the weights of the operators based on the scores collected in the last period.
+We employ three essential methods of the ALNS solver:
+
+1. alns.generate: This method selects and applies a destroy and a repair operator to the current solution, modifying it in-place. It returns a tuple of the chosen operators.
+2. alns.collect_score: This method gathers scores for the provided operators. It requires the selected operators and a score as arguments.
+3. alns.adapt_operator_weights: This method adjusts the weights of the operators based on the scores collected during the last period.
 
 For more details on the ALNS solver, see the `documentation <alns>`_. The full code of the ALNS algorithm is available `here <alns_code>`_. A more sophisticated ALNS-based algorithm can be found in the `main repository <https://github.com/tumBAIS/RoutingBlocks/tree/main/examples/evrptw>`_.
 
 Implementing custom operators
 ------------------------------------
 
 The RoutingBlocks library provides a set of standard operators out of the box. However, it is also possible to implement custom local search, destroy, and repair operators. We'll implement a simple RouteRemoval destroy operator as an example:
```

### Comparing `routingblocks-0.1.5/docs/source/index.rst` & `routingblocks-0.1.7/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     :maxdepth: 1
     :caption: Further Reading
 
     extension
     examples
     development
     full_api
+    references
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
-* :ref:`search`
+* :ref:`search`
```

### Comparing `routingblocks-0.1.5/docs/source/localsearch.rst` & `routingblocks-0.1.7/docs/source/localsearch.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/README.md` & `routingblocks-0.1.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/alns/__main__.py` & `routingblocks-0.1.7/examples/alns/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/alns/alns.py` & `routingblocks-0.1.7/examples/alns/alns.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     alns.add_destroy_operator(rb.operators.RandomRemovalOperator(randgen))
     alns.add_destroy_operator(rb.operators.WorstRemovalOperator(instance,
                                                                 rb.operators.blink_selector_factory(
                                                                     blink_probability=0.1, randgen=randgen)))
 
     # Generate a random starting solution
     best_solution = create_random_solution(evaluation, instance)
-    for i in range(number_of_iterations):
+    for i in range(1, number_of_iterations + 1):
         current_solution = copy.copy(best_solution)
         # Perturb the current solution
         number_of_vertices_to_remove = int(random.uniform(min_vertex_removal_factor, max_vertex_removal_factor) * sum(
             len(route) - 2 for route in current_solution))
         picked_operators = alns.generate(evaluation, current_solution, number_of_vertices_to_remove)
 
         # Search the neighborhood of the current solution. This modifies the solution in-place.
```

### Comparing `routingblocks-0.1.5/examples/alns/parsing.py` & `routingblocks-0.1.7/examples/alns/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,26 +42,26 @@
 
 def create_instance(serialized_vertices, serialized_arcs) -> rb.Instance:
     instance_builder = rb.utility.InstanceBuilder(create_vertex=rb.adptw.create_adptw_vertex,
                                                   create_arc=rb.adptw.create_adptw_arc)
     # Create and register the vertices
     for vertex in serialized_vertices:
         # Create problem-specific data held by vertices
-        vertex_data = rb.adptw.ADPTWVertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
-                                               vertex['DueDate'],
-                                               vertex['ServiceTime'])
+        vertex_data = rb.adptw.VertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
+                                          vertex['DueDate'],
+                                          vertex['ServiceTime'])
         # Register the vertex depending on it's type
         if vertex['Type'] == 'd':
             instance_builder.set_depot(vertex['StringID'], vertex_data)
         elif vertex['Type'] == 'c':
             instance_builder.add_customer(vertex['StringID'], vertex_data)
         else:
             instance_builder.add_station(vertex['StringID'], vertex_data)
 
     # Create and register the arcs
     for (i, j), arc in serialized_arcs.items():
         # Create problem-specific data held by arcs
-        arc_data = rb.adptw.ADPTWArcData(arc['distance'], arc['consumption'], arc['travel_time'])
+        arc_data = rb.adptw.ArcData(arc['distance'], arc['consumption'], arc['travel_time'])
         instance_builder.add_arc(i, j, arc_data)
 
     # Create instance
     return instance_builder.build()
```

### Comparing `routingblocks-0.1.5/examples/evrptw/__main__.py` & `routingblocks-0.1.7/examples/evrptw/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/alns.py` & `routingblocks-0.1.7/examples/evrptw/alns.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def register(self, solution: routingblocks.Solution):
         self._last_penalites.append(self._get_cost_components(solution))
         if len(self._last_penalites) > self._window_length:
             self._last_penalites.pop(0)
 
 
 class ALNS:
-    def __init__(self, evaluation: routingblocks.Evaluation, py_instance: ADPTWInstance,
+    def __init__(self, evaluation: routingblocks.adptw.Evaluation, py_instance: ADPTWInstance,
                  cpp_instance: routingblocks.Instance,
                  params: ALNSParams, seed: int):
         self._evaluation = evaluation
         self._py_instance = py_instance
         self._cpp_instance = cpp_instance
         self._params = params
         # Initialize random engines
@@ -174,27 +174,27 @@
         return self._best_solution.cost if self._best_solution else sys.float_info.max
 
     @property
     def _best_feasible_obj(self):
         return self._best_feasible_solution.cost if self._best_feasible_solution else sys.float_info.max
 
     def _make_feasible(self, solution: routingblocks.Solution):
-        penalty_factors = self._evaluation.penalty_factors
-        self._evaluation.penalty_factors = [penalty_factors[0], penalty_factors[1] * 100.,
-                                            penalty_factors[2] * 100.,
-                                            penalty_factors[3] * 100.]
+        penalty_factors = [self._evaluation.overload_penalty_factor, self._evaluation.overcharge_penalty_factor,
+                           self._evaluation.time_shift_penalty_factor]
+        self._update_penalty_factors(*(x * 100.0 for x in penalty_factors))
         self._local_search.optimize(solution, self._operators)
-        self._evaluation.penalty_factors = penalty_factors
+        self._update_penalty_factors(*penalty_factors)
 
     def _remove_vehicle(self, solution: routingblocks.Solution):
         # Reset penalty
-        current_penalties = self._evaluation.penalty_factors
-        for i in range(1, len(current_penalties)):
-            current_penalties[i] = max(current_penalties[i], self._params.initial_penalties[i - 1] * 100)
-        self._evaluation.penalty_factors = current_penalties
+        penalty_factors = [self._evaluation.overload_penalty_factor, self._evaluation.overcharge_penalty_factor,
+                           self._evaluation.time_shift_penalty_factor]
+        for i in range(len(penalty_factors)):
+            penalty_factors[i] = max(penalty_factors[i], self._params.initial_penalties[i - 1] * 100)
+        self._update_penalty_factors(*penalty_factors)
         self._boosted_penalties = True
 
         # Remove route
         fewest_customer_route = min(solution, key=lambda r: len(r))
         customers = [x.vertex_id for x in fewest_customer_route if x.vertex.is_customer]
 
         solution.remove_route(fewest_customer_route)
@@ -231,15 +231,15 @@
                     self._last_vehicle_decrease_iter = self._iters
                     self._reached_vehicle_lb = False
                 self._best_feasible_solution = copy.deepcopy(solution)
                 if len(self._best_feasible_solution) > len(self._best_solution):
                     self._best_solution = copy.deepcopy(solution)
                 if self._boosted_penalties:
                     self._boosted_penalties = False
-                    self._evaluation.penalty_factors = self._saved_penalties
+                    self._update_penalty_factors(*self._saved_penalties)
                 print(
                     f"[{self.elapsed:.2f}s, {self._iters}, {self._iters_since_improvement}]: Found new best feasible solution: {solution_cost} ({self._best_feasible_obj}, {len(solution)})")
                 score = self._params.new_best_feasible_score
         return score
 
     @property
     def elapsed(self):
@@ -329,26 +329,28 @@
                 # Trigger the vehicle minimization procedure
             if not self._reached_vehicle_lb:
                 if (self._iters - self._last_vehicle_decrease_iter > self._params.vehicle_decrease_period_length) \
                         and (self._best_feasible_solution is not None):
                     self._last_vehicle_decrease_iter = self._ls_iters
                     self._reached_vehicle_lb = True
                     if not self._boosted_penalties:
-                        self._saved_penalties = list(self._evaluation.penalty_factors)
+                        self._saved_penalties = [self._evaluation.overload_penalty_factor,
+                                                 self._evaluation.overcharge_penalty_factor,
+                                                 self._evaluation.time_shift_penalty_factor]
                     if len(self._best_feasible_solution) > self._vehicle_lb:
                         while len(self._current_solution) > len(self._best_feasible_solution) - 1:
                             self._remove_vehicle(self._current_solution)
                     self._best_solution = self._current_solution
                     print(f"Decreased max number of vehicles to {len(self._best_feasible_solution) - 1}")
             else:
                 if len(self._best_feasible_solution) > len(
                         self._current_solution) and (
                         self._ls_iters - self._last_vehicle_decrease_iter) > self._params.vehicle_decreased_search_period_length:
                     self._current_solution = copy.deepcopy(self._best_feasible_solution)
-                    self._evaluation.penalty_factors = self._saved_penalties
+                    self._update_penalty_factors(*self._saved_penalties)
                     self._boosted_penalties = False
                     self._best_solution = copy.deepcopy(self._best_feasible_solution)
                     print(f"Increased max number of vehicles to {len(self._current_solution)}")
 
         if self._best_feasible_solution is not None:
             return self._best_feasible_solution
         else:
```

### Comparing `routingblocks-0.1.5/examples/evrptw/config.json` & `routingblocks-0.1.7/examples/evrptw/config.json`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instance/interface.py` & `routingblocks-0.1.7/examples/evrptw/instance/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,22 @@
         vertex_id, vertex.vertex_id, vertex.is_station, vertex.is_depot, data_factory(vertex))
 
 
 def create_cpp_arc(arc: Arc, data_factory: Callable[[Arc], Any]) -> evrptw.Arc:
     return evrptw.adptw.create_adptw_arc(data_factory(arc))
 
 
-def adptw_vertex_data_factory(vertex: Vertex) -> evrptw.adptw.ADPTWVertexData:
-    return evrptw.adptw.ADPTWVertexData(vertex.x_coord, vertex.y_coord, vertex.demand, vertex.ready_time,
-                                        vertex.due_time,
-                                        vertex.service_time)
+def adptw_vertex_data_factory(vertex: Vertex) -> evrptw.adptw.VertexData:
+    return evrptw.adptw.VertexData(vertex.x_coord, vertex.y_coord, vertex.demand, vertex.ready_time,
+                                   vertex.due_time,
+                                   vertex.service_time)
 
 
-def adptw_arc_data_factory(arc: Arc) -> evrptw.adptw.ADPTWArcData:
-    return evrptw.adptw.ADPTWArcData(arc.distance, arc.consumption, arc.travel_time)
+def adptw_arc_data_factory(arc: Arc) -> evrptw.adptw.ArcData:
+    return evrptw.adptw.ArcData(arc.distance, arc.consumption, arc.travel_time)
 
 
 def create_cpp_instance(instance: Instance) -> evrptw.Instance:
     vertex_data_factory = adptw_vertex_data_factory
     arc_data_factory = adptw_arc_data_factory
 
     # Convert vertices
```

### Comparing `routingblocks-0.1.5/examples/evrptw/instance/models.py` & `routingblocks-0.1.7/examples/evrptw/instance/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instance/parsing.py` & `routingblocks-0.1.7/examples/evrptw/instance/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c101C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c101C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c104C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c104C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c202C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c202C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/c205C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/c205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r102C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r103C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r103C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r201C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/r203C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/r203C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc102C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc108C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc108C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc201C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/10/rc205C10.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/10/rc205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c101_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c102_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c103_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c104_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c105_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c106_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c107_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c108_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c109_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c201_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c202_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c203_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c204_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c205_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c206_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c207_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/c208_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/c208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r101_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r102_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r103_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r104_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r105_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r106_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r107_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r108_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r109_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r110_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r110_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r111_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r111_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r112_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r112_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r201_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r202_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r203_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r204_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r205_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r206_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r207_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r208_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r209_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r209_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r210_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r210_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/r211_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/r211_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc101_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc102_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc103_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc104_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc105_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc106_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc107_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc108_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc201_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc202_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc203_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc204_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc205_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc206_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc207_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/100/rc208_21.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/100/rc208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c103C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c106C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c106C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c202C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/c208C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/c208C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r102C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r102C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r105C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r105C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r202C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/r209C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/r209C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc103C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc108C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc108C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc202C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/15/rc204C15.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/15/rc204C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c101C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c103C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c103C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c206C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c206C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/c208C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/c208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r104C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r104C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r105C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r202C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r202C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/r203C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/r203C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc105C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc108C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc108C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc204C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc204C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/5/rc208C5.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/5/rc208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/instances/evrptw/README.txt` & `routingblocks-0.1.7/examples/evrptw/instances/evrptw/README.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/operators/ShawMoveSelector.py` & `routingblocks-0.1.7/examples/evrptw/operators/ShawMoveSelector.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/operators/ShawRelatedness.py` & `routingblocks-0.1.7/examples/evrptw/operators/ShawRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/operators/SpatioTemporalRelatedness.py` & `routingblocks-0.1.7/examples/evrptw/operators/SpatioTemporalRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/operators/__init__.py` & `routingblocks-0.1.7/examples/evrptw/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/evrptw/parameters.py` & `routingblocks-0.1.7/examples/evrptw/parameters.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/ils/__main__.py` & `routingblocks-0.1.7/examples/ils/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/ils/ils.py` & `routingblocks-0.1.7/examples/ils/ils.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/examples/ils/parsing.py` & `routingblocks-0.1.7/examples/ils/parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         fields = instance_stream.readline().split()
         # Parse the vertices
         vertices = []
         for line in instance_stream:
             tokens = line.split()
             if len(tokens) == 0:
                 break
+            # Read columns into a dictionary
             vertex = {key: (x if key in str_fields else float(x)) for key, x in zip(fields, tokens)}
             vertices.append(vertex)
         # Parse the parameters
         parameters = {}
         for line in instance_stream:
             key, *_, value = line.split()
             # Remove surrounding / characters and parse the value
@@ -42,26 +43,26 @@
 
 def create_instance(serialized_vertices, serialized_arcs) -> rb.Instance:
     instance_builder = rb.utility.InstanceBuilder(create_vertex=rb.adptw.create_adptw_vertex,
                                                   create_arc=rb.adptw.create_adptw_arc)
     # Create and register the vertices
     for vertex in serialized_vertices:
         # Create problem-specific data held by vertices
-        vertex_data = rb.adptw.ADPTWVertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
-                                               vertex['DueDate'],
-                                               vertex['ServiceTime'])
+        vertex_data = rb.adptw.VertexData(vertex['x'], vertex['y'], vertex['demand'], vertex['ReadyTime'],
+                                          vertex['DueDate'],
+                                          vertex['ServiceTime'])
         # Register the vertex depending on it's type
         if vertex['Type'] == 'd':
             instance_builder.set_depot(vertex['StringID'], vertex_data)
         elif vertex['Type'] == 'c':
             instance_builder.add_customer(vertex['StringID'], vertex_data)
         else:
             instance_builder.add_station(vertex['StringID'], vertex_data)
 
     # Create and register the arcs
     for (i, j), arc in serialized_arcs.items():
         # Create problem-specific data held by arcs
-        arc_data = rb.adptw.ADPTWArcData(arc['distance'], arc['consumption'], arc['travel_time'])
+        arc_data = rb.adptw.ArcData(arc['distance'], arc['consumption'], arc['travel_time'])
         instance_builder.add_arc(i, j, arc_data)
 
     # Create instance
     return instance_builder.build()
```

### Comparing `routingblocks-0.1.5/native/CMakeLists.txt` & `routingblocks-0.1.7/native/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/cmake/CPM.cmake` & `routingblocks-0.1.7/native/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/cmake/tools.cmake` & `routingblocks-0.1.7/native/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/ADPTWEvaluation.h` & `routingblocks-0.1.7/native/include/routingblocks/ADPTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/FRVCP.h` & `routingblocks-0.1.7/native/include/routingblocks/FRVCP.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/Instance.h` & `routingblocks-0.1.7/native/include/routingblocks/Instance.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/LocalSearch.h` & `routingblocks-0.1.7/native/include/routingblocks/LocalSearch.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/Solution.h` & `routingblocks-0.1.7/native/include/routingblocks/Solution.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/adaptive_large_neighborhood.hpp` & `routingblocks-0.1.7/native/include/routingblocks/adaptive_large_neighborhood.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/arc.h` & `routingblocks-0.1.7/native/include/routingblocks/arc.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/evaluation.h` & `routingblocks-0.1.7/native/include/routingblocks/evaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/insertion_cache.h` & `routingblocks-0.1.7/native/include/routingblocks/insertion_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/lns_operators.h` & `routingblocks-0.1.7/native/include/routingblocks/lns_operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/node.h` & `routingblocks-0.1.7/native/include/routingblocks/node.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/operators/InsertStationOperator.h` & `routingblocks-0.1.7/native/include/routingblocks/operators/InsertStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/operators/InterRouteTwoOptOperator.h` & `routingblocks-0.1.7/native/include/routingblocks/operators/InterRouteTwoOptOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/operators/RemoveStationOperator.h` & `routingblocks-0.1.7/native/include/routingblocks/operators/RemoveStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/operators/SwapOperator.h` & `routingblocks-0.1.7/native/include/routingblocks/operators/SwapOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/operators.h` & `routingblocks-0.1.7/native/include/routingblocks/operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/removal_cache.h` & `routingblocks-0.1.7/native/include/routingblocks/removal_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/adaptive_priority_list.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/adaptive_priority_list.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/algorithms.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/algorithms.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/arc_set.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/arc_set.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/heap.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/heap.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/iterator_pair.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/iterator_pair.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/utility/random.h` & `routingblocks-0.1.7/native/include/routingblocks/utility/random.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/include/routingblocks/vertex.h` & `routingblocks-0.1.7/native/include/routingblocks/vertex.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/dynamic_bitset/LICENSE.txt` & `routingblocks-0.1.7/native/lib/dynamic_bitset/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp` & `routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h` & `routingblocks-0.1.7/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/small_vector/LICENSE.txt` & `routingblocks-0.1.7/native/lib/small_vector/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/small_vector/small_vector/small_vector.hpp` & `routingblocks-0.1.7/native/lib/small_vector/small_vector/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/xoshiro/LICENSE.txt` & `routingblocks-0.1.7/native/lib/xoshiro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/lib/xoshiro/xoshiro/xoshiro.h` & `routingblocks-0.1.7/native/lib/xoshiro/xoshiro/xoshiro.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/ADPTWEvaluation.cpp` & `routingblocks-0.1.7/native/src/ADPTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/Instance.cpp` & `routingblocks-0.1.7/native/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/LocalSearch.cpp` & `routingblocks-0.1.7/native/src/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/NIFTWEvaluation.cpp` & `routingblocks-0.1.7/native/src/NIFTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/Solution.cpp` & `routingblocks-0.1.7/native/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/lns_operators.cpp` & `routingblocks-0.1.7/native/src/lns_operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/node.cpp` & `routingblocks-0.1.7/native/src/node.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/operators/InsertStationOperator.cpp` & `routingblocks-0.1.7/native/src/operators/InsertStationOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/src/operators/InterRouteTwoOptOperator.cpp` & `routingblocks-0.1.7/native/src/operators/InterRouteTwoOptOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/native/test/CMakeLists.txt` & `routingblocks-0.1.7/native/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/pyproject.toml` & `routingblocks-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["scikit-build-core>=0.2.1", "pybind11", "mypy"]
+requires = ["scikit-build-core>=0.2.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "RoutingBlocks"
-version = "0.1.5"
+version = "0.1.7"
 description = "A package for the implementation of vehicle routing problems with intermediate stops"
 readme = "README.md"
 authors = [
     { name = "Patrick Sean Klein", email = "patrick.sean.klein@tum.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
@@ -21,23 +21,35 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-benchmark", "pytest-randomly", "pydantic"]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints", "sphinx-autoapi"]
+examples = ["click", "pydantic"]
 
 
 [tool.scikit-build]
 wheel.expand-macos-universal-tags = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "test/tests/",
 ]
 
 [tool.cibuildwheel]
-test-command = 'python -m pytest {project}/test/tests -m "not benchmark" --randomly-dont-reorganize'
-test-extras = ["test"]
+test-command = [
+    'python -m pytest {project}/test/tests -m "not benchmark" --randomly-dont-reorganize',
+    'cd {project}/examples && python -m ils -n 10 evrptw/instances/evrptw/100/c101_21.txt',
+    'cd {project}/examples && python -m alns -n 10 evrptw/instances/evrptw/100/c101_21.txt',
+    'cd {project}/examples && python -m evrptw --time-limit 120 --config-path evrptw/config.json evrptw/instances/evrptw/100/c101_21.txt',
+]
+test-extras = ["test", "examples"]
 test-skip = ["*universal2:arm64"]
 build = ["cp*-manylinux_x86_64", "cp*-win32", "cp*-win_amd64", "cp*-macosx_*"]
 build-verbosity = 3
+
+[[tool.cibuildwheel.overrides]]
+select = '*-win*'
+test-command = [
+    'python -m pytest {project}/test/tests -m "not benchmark" --randomly-dont-reorganize'
+]
```

### Comparing `routingblocks-0.1.5/routingblocks/operators/__init__.py` & `routingblocks-0.1.7/routingblocks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/best_insert.py` & `routingblocks-0.1.7/routingblocks/operators/best_insert.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/cluster_removal.py` & `routingblocks-0.1.7/routingblocks/operators/cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/move_selectors.py` & `routingblocks-0.1.7/routingblocks/operators/move_selectors.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/related_removal.py` & `routingblocks-0.1.7/routingblocks/operators/related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/route_removal.py` & `routingblocks-0.1.7/routingblocks/operators/route_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/station_vicinity_removal.py` & `routingblocks-0.1.7/routingblocks/operators/station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/operators/worst_removal.py` & `routingblocks-0.1.7/routingblocks/operators/worst_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/routingblocks/utility/instance_builder.py` & `routingblocks-0.1.7/test/tests/helpers/interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,52 @@
-from typing import Callable, TypeVar
+from __future__ import annotations
+from .models import Vertex, Instance, Arc
+from .parsing import parse_instance
+from pathlib import Path
+from typing import Callable, Any
 
-from .. import Instance, Vertex, Arc
+try:
+    import routingblocks as evrptw
+except ModuleNotFoundError:
+    pass
 
-T = TypeVar('T')
-VertexID = int
-vertex_factory = Callable[[VertexID, str, bool, bool, T], Vertex]
-arc_factory = Callable[[T], Arc]
-
-
-class InstanceBuilder:
-    def __init__(self, create_vertex: vertex_factory = Vertex, create_arc: arc_factory = Arc):
-        self._depot = None
-        self._customers = {}
-        self._stations = {}
-
-        self._create_vertex = create_vertex
-        self._create_arc = create_arc
-
-        self.fleet_size = 0
-
-        self._arcs = {}
-
-    def _add_vertex(self, str_id: str, is_depot: bool, is_station: bool, vertex_data):
-        assert is_depot + is_station < 2, "Vertex cannot be both depot and station"
-        if is_depot:
-            if self._depot is not None:
-                raise ValueError(f"Instance already has a depot")
-            self._depot = (str_id, False, True, vertex_data)
-        elif is_station:
-            self._stations[str_id] = (str_id, True, False, vertex_data)
-        else:
-            self._customers[str_id] = (str_id, False, False, vertex_data)
-
-    def set_depot(self, str_id: str, vertex_data):
-        self._add_vertex(str_id, True, False, vertex_data)
-
-    def add_customer(self, str_id: str, vertex_data):
-        self._add_vertex(str_id, False, False, vertex_data)
-
-    def add_station(self, str_id: str, vertex_data):
-        self._add_vertex(str_id, False, True, vertex_data)
-
-    def add_arc(self, i: str, j: str, arc_data):
-        self._arcs[i, j] = arc_data
-
-    @property
-    def number_of_vertices(self):
-        return (self._depot is not None) + len(self._customers) + len(self._stations)
-
-    def reset(self):
-        self._depot = None
-        self._customers.clear()
-        self._stations.clear()
-        self._arcs.clear()
-
-    def build(self) -> Instance:
-        if self._depot is None:
-            raise ValueError(f"Instance requires depot")
-        if len(self._customers) == 0:
-            raise ValueError("Instance requires at least one customer")
-        if len(self._arcs) != self.number_of_vertices * self.number_of_vertices:
-            raise ValueError("Instance requires arcs between all vertices")
-
-        vertices = [self._create_vertex(i, *vertex_data) for i, vertex_data in
-                    enumerate((self._depot, *self._customers.values(),
-                               *self._stations.values()))]
-
-        arc_matrix = []
-        for i, origin in enumerate(vertices):
-            arc_matrix.append([])
-            for j, destination in enumerate(vertices):
-                arc_data = self._arcs.get((origin.str_id, destination.str_id))
-                if arc_data is None:
-                    raise ValueError(f"Instance requires arc between {origin.str_id} and {destination.str_id}")
-                arc_matrix[i].append(self._create_arc(arc_data))
 
-        return Instance(vertices, arc_matrix, self.fleet_size)
+def create_cpp_vertex(vertex: Vertex, vertex_id: int, data_factory: Callable[[Vertex], Any]) -> evrptw.Vertex:
+    return evrptw.adptw.create_adptw_vertex(
+        vertex_id, vertex.vertex_id, vertex.is_station, vertex.is_depot, data_factory(vertex))
+
+
+def create_cpp_arc(arc: Arc, data_factory: Callable[[Arc], Any]) -> evrptw.Arc:
+    return evrptw.adptw.create_adptw_arc(data_factory(arc))
+
+
+def adptw_vertex_data_factory(vertex: Vertex) -> evrptw.adptw.VertexData:
+    return evrptw.adptw.VertexData(vertex.x_coord, vertex.y_coord, vertex.demand, vertex.ready_time,
+                                   vertex.due_date,
+                                   vertex.service_time)
+
+
+def adptw_arc_data_factory(arc: Arc) -> evrptw.adptw.ArcData:
+    return evrptw.adptw.ArcData(arc.distance, arc.consumption, arc.travel_time)
+
+
+def create_cpp_instance(instance: Instance) -> evrptw.Instance:
+    vertex_data_factory = adptw_vertex_data_factory
+    arc_data_factory = adptw_arc_data_factory
+
+    # Convert vertices
+    sorted_vertices = [instance.depot, *sorted(instance.customers, key=lambda v: v.vertex_id),
+                       *sorted(instance.stations, key=lambda v: v.vertex_id)]
+    cpp_vertices = [create_cpp_vertex(v, i, data_factory=vertex_data_factory) for i, v in enumerate(sorted_vertices)]
+    id_map = {cpp_v.vertex_id: v for v, cpp_v in zip(sorted_vertices, cpp_vertices)}
+
+    cpp_arcs = [
+        [create_cpp_arc(instance.arcs[id_map[i.vertex_id].vertex_id, id_map[j.vertex_id].vertex_id],
+                        data_factory=arc_data_factory)
+         for j in cpp_vertices] for i in cpp_vertices]
+
+    return evrptw.Instance(cpp_vertices, cpp_arcs, instance.parameters.fleet_size)
+
+
+def parse_evrptw_instance(filename: Path) -> evrptw.Instance:
+    # Create cpp instance
+    return parse_instance(filename)
```

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/reference/insertion_cache.py` & `routingblocks-0.1.7/test/tests/benchmarks/reference/insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/reference/removal_cache.py` & `routingblocks-0.1.7/test/tests/benchmarks/reference/removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_frvcp.py` & `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_local_search.py` & `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_removal_cache.py` & `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/benchmarks/test_benchmark_route_update.py` & `routingblocks-0.1.7/test/tests/benchmarks/test_benchmark_route_update.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/__init__.py` & `routingblocks-0.1.7/test/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/data/c101C5.txt` & `routingblocks-0.1.7/test/tests/fixtures/data/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/data/c101_21.txt` & `routingblocks-0.1.7/test/tests/fixtures/data/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/data/r101_21.txt` & `routingblocks-0.1.7/test/tests/fixtures/data/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/data/r201_21.txt` & `routingblocks-0.1.7/test/tests/fixtures/data/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/data/rc101_21.txt` & `routingblocks-0.1.7/test/tests/fixtures/data/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/fixtures/mock_evaluation.py` & `routingblocks-0.1.7/test/tests/fixtures/mock_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/helpers/models.py` & `routingblocks-0.1.7/test/tests/helpers/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/helpers/parsing.py` & `routingblocks-0.1.7/test/tests/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_cluster_removal.py` & `routingblocks-0.1.7/test/tests/operators/test_cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_random_insertion.py` & `routingblocks-0.1.7/test/tests/operators/test_random_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_random_removal.py` & `routingblocks-0.1.7/test/tests/operators/test_random_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_related_removal.py` & `routingblocks-0.1.7/test/tests/operators/test_related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_station_insertion.py` & `routingblocks-0.1.7/test/tests/operators/test_station_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_station_vicinity_removal.py` & `routingblocks-0.1.7/test/tests/operators/test_station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/operators/test_swap.py` & `routingblocks-0.1.7/test/tests/operators/test_swap.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_frvcp.py` & `routingblocks-0.1.7/test/tests/test_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_insertion_cache.py` & `routingblocks-0.1.7/test/tests/test_insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_large_neighborhood.py` & `routingblocks-0.1.7/test/tests/test_large_neighborhood.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_lns_helpers.py` & `routingblocks-0.1.7/test/tests/test_lns_helpers.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_local_search.py` & `routingblocks-0.1.7/test/tests/test_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_node.py` & `routingblocks-0.1.7/test/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_removal_cache.py` & `routingblocks-0.1.7/test/tests/test_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/test/tests/test_route.py` & `routingblocks-0.1.7/test/tests/test_route.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 def test_route_insert_vertices(mock_evaluation, sorted_locations: bool, adptw_instance: evrptw.Instance):
     instance: evrptw.Instance = adptw_instance
     customers = list(instance.customers)
     route = evrptw.create_route(mock_evaluation, instance,
                                 [customers[0].vertex_id, customers[1].vertex_id, customers[2].vertex_id])
     # [0, 1, 2, 3, 0]
     to_insert = [customers[3].vertex_id, customers[4].vertex_id]
-    insertion_positions = [evrptw.NodeLocation(0, 0), evrptw.NodeLocation(0, 1)]
+    insertion_positions = [0, 1]
     if sorted_locations:
         insertion_positions.reverse()
         to_insert.reverse()
 
     expected_route = evrptw.create_route(mock_evaluation, instance,
                                          [customers[3].vertex_id, customers[0].vertex_id, customers[4].vertex_id,
                                           customers[1].vertex_id,
```

### Comparing `routingblocks-0.1.5/test/tests/test_solution.py` & `routingblocks-0.1.7/test/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.5/PKG-INFO` & `routingblocks-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: routingblocks
-Version: 0.1.5
+Version: 0.1.7
 Summary: A package for the implementation of vehicle routing problems with intermediate stops
 Author-Email: Patrick Sean Klein <patrick.sean.klein@tum.de>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: examples
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-randomly; extra == "test"
 Requires-Dist: pydantic; extra == "test"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
+Requires-Dist: click; extra == "examples"
+Requires-Dist: pydantic; extra == "examples"
 Description-Content-Type: text/markdown
 
 # RoutingBlocks
 
 `RoutingBlocks` is an open-source Python package for the implementation of algorithms for Vehicle Routing Problems with
 Intermediate Stops.
```

