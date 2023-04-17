# Comparing `tmp/waveforms-1.5.83.tar.gz` & `tmp/waveforms-1.5.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveforms-1.5.83.tar", last modified: Wed Apr 12 07:19:08 2023, max compression
+gzip compressed data, was "waveforms-1.5.84.tar", last modified: Mon Apr 17 15:13:02 2023, max compression
```

## Comparing `waveforms-1.5.83.tar` & `waveforms-1.5.84.tar`

### file list

```diff
@@ -1,198 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 07:18:15.000000 waveforms-1.5.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 07:18:15.000000 waveforms-1.5.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 07:19:08.978582 waveforms-1.5.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-12 07:18:15.000000 waveforms-1.5.83/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 07:18:15.000000 waveforms-1.5.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:19:08.978582 waveforms-1.5.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-12 07:18:15.000000 waveforms-1.5.83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/ikcp.c
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/ikcp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/kcp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/prime.c
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/waveform.c
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/waveform.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_lisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_scan_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/math/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fibheap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/math/fit/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/qubit_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/resonator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/prime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/math/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/demodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/_antlr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/_antlr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/prog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/qasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/qasm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/libs/qelib1.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/qlisp/qasm/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/creg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/customunitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/expressionlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/gatebody.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/indexedid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/intnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/nodeexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/primarylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/qreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/unaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasmlexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasmparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/qlisp/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/assembly_left.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/assembly_right.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/library.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/qlisp.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/simulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/clifford/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/seq2mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/rb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/xeb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/scan_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/security/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/security/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/server/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/umsgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/device/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/ipy_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/dhcpd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/kad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/kcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/units/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/plot_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/plot_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/waveform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 15:12:07.000000 waveforms-1.5.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 15:12:07.000000 waveforms-1.5.84/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-17 15:13:02.985558 waveforms-1.5.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-17 15:12:07.000000 waveforms-1.5.84/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-17 15:12:07.000000 waveforms-1.5.84/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:13:02.985558 waveforms-1.5.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-17 15:12:07.000000 waveforms-1.5.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.973558 waveforms-1.5.84/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/ikcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/ikcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/kcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/prime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/waveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-17 15:12:07.000000 waveforms-1.5.84/src/waveform.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.973558 waveforms-1.5.84/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_scan_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-17 15:12:07.000000 waveforms-1.5.84/tests/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.973558 waveforms-1.5.84/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fibheap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/math/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/qubit_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/resonator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/fit/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/prime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/math/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/signal/demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/signal/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/signal/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/math/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/_antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/_antlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.977558 waveforms-1.5.84/waveforms/qlisp/qasm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/libs/qelib1.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/qlisp/qasm/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/binaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/binaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/creg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/customunitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/expressionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/gatebody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/indexedid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/intnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/nodeexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/primarylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/qreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/node/unaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/qasmlexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/qasm/qasmparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/qlisp/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/simulator/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/simulator/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/arch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/assembly_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/assembly_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/qlisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/circuit/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/circuit/simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/quantum/clifford/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/clifford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/clifford/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/clifford/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/clifford/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/clifford/seq2mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/quantum/xeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/scan_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/security/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/server/umsgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.981558 waveforms-1.5.84/waveforms/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/sys/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/device/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/device/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/sys/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/ipy_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/sys/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/net/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/net/dhcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/net/kad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/net/kcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/sys/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/storage/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/sys/storage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.985558 waveforms-1.5.84/waveforms/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/visualization/plot_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/visualization/plot_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-17 15:12:07.000000 waveforms-1.5.84/waveforms/waveform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:13:02.973558 waveforms-1.5.84/waveforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 15:13:02.000000 waveforms-1.5.84/waveforms.egg-info/top_level.txt
```

### Comparing `waveforms-1.5.83/LICENSE` & `waveforms-1.5.84/LICENSE`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/PKG-INFO` & `waveforms-1.5.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.83
+Version: 1.5.84
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.83/README.md` & `waveforms-1.5.84/README.md`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/pyproject.toml` & `waveforms-1.5.84/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/setup.py` & `waveforms-1.5.84/setup.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/ikcp.c` & `waveforms-1.5.84/src/ikcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/ikcp.h` & `waveforms-1.5.84/src/ikcp.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/kcp.c` & `waveforms-1.5.84/src/kcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/prime.c` & `waveforms-1.5.84/src/prime.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/waveform.c` & `waveforms-1.5.84/src/waveform.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/src/waveform.h` & `waveforms-1.5.84/src/waveform.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_compile.py` & `waveforms-1.5.84/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_dicttree.py` & `waveforms-1.5.84/tests/test_dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_lisp.py` & `waveforms-1.5.84/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_msgpack.py` & `waveforms-1.5.84/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_namespace.py` & `waveforms-1.5.84/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_registry.py` & `waveforms-1.5.84/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_scan_iter.py` & `waveforms-1.5.84/tests/test_scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_tomo.py` & `waveforms-1.5.84/tests/test_tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_vm.py` & `waveforms-1.5.84/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/tests/test_waveform.py` & `waveforms-1.5.84/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/__init__.py` & `waveforms-1.5.84/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/autoreload.py` & `waveforms-1.5.84/waveforms/autoreload.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/baseconfig.py` & `waveforms-1.5.84/waveforms/baseconfig.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/cache.py` & `waveforms-1.5.84/waveforms/cache.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/dicttree.py` & `waveforms-1.5.84/waveforms/dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/loader.py` & `waveforms-1.5.84/waveforms/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/bayes.py` & `waveforms-1.5.84/waveforms/math/bayes.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/fibheap.py` & `waveforms-1.5.84/waveforms/math/fibheap.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/fit/__init__.py` & `waveforms-1.5.84/waveforms/math/fit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,9 +6,9 @@
                       gaussian_pdf_2d, get_threshold_info,
                       install_classify_method, mult_gaussian_cdf,
                       mult_gaussian_pdf, readout_distribution,
                       uninstall_classify_method)
 from .simple import (complex_amp_to_real, find_cross_point, fit_circle,
                      fit_cosine, fit_cross_point, fit_pole, goodness_of_fit,
                      inv_poly, lin_fit, poly_fit)
-from .spectrum import (fit_transmon_spectrum, transmon_spectrum,
-                       transmon_spectrum_fast)
+from .spectrum import (fit_transmon_spectrum, get_2d_spectrum_background,
+                       transmon_spectrum, transmon_spectrum_fast)
```

### Comparing `waveforms-1.5.83/waveforms/math/fit/delay.py` & `waveforms-1.5.84/waveforms/math/fit/delay.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/fit/geo.py` & `waveforms-1.5.84/waveforms/math/fit/geo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/fit/qubit_dynamics.py` & `waveforms-1.5.84/waveforms/math/fit/_fit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import functools
 import inspect
 
 import numpy as np
 from scipy.optimize import curve_fit
-from scipy.signal import find_peaks
-
-from waveforms.math.fit.qubit_dynamics import *
 
 
 def fit(func,
         xdata,
         ydata,
         p0=None,
         sigma=None,
@@ -19,15 +15,15 @@
     """
     Fit data to a function.
 
     Args:
         func (function): fitting function
         xdata (np.ndarray): x data
         ydata (np.ndarray): y data
-        p0 (np.ndarray | dict): initial parameters
+        p0 (dict): initial parameters
         sigma (np.ndarray): standard deviation of ydata
         bounds (tuple): lower and upper bounds of parameters
         guess (function): function to guess initial parameters
         static_params (dict): static parameters for fitting
 
     Returns:
         arg_names (list): parameter names
@@ -50,16 +46,19 @@
     def func_wrapper(x, *args):
         params = dict(zip(arg_names, args)) | static_params
         return func(x, **params)
 
     if guess is None and p0 is None:
         raise ValueError('Initial parameters are not specified!')
 
+    if p0 is None:
+        p0 = {}
+
     if guess is not None:
-        p0 = guess(xdata, ydata, static_params)
+        p0 = p0 | guess(xdata, ydata, p0 | static_params)
 
     if isinstance(p0, dict):
         p0 = [p0[arg_name] for arg_name in arg_names]
 
     try:
         popt, pcov = curve_fit(func_wrapper,
                                xdata,
@@ -69,76 +68,7 @@
                                absolute_sigma=True,
                                method='trf',
                                bounds=bounds)
         fitted = func_wrapper(xdata, *popt)
         return arg_names, popt, pcov, fitted
     except:
         raise ValueError('Fitting failed!')
-
-
-def func_rabi(t, A, Tr, freq, phi, B):
-    return A * np.exp(-t / Tr) * np.cos(2 * np.pi * freq * t + phi) + B
-
-
-def guess_rabi(t, y, static_params, freq):
-    if 'B' in static_params:
-        B = static_params['B']
-    else:
-        B = np.median(y)
-
-    if freq is None:
-        freq = np.fft.fftfreq(t.shape[0], t[1] - t[0])[1:(t.shape[0] // 3)]
-        amp = np.abs(np.fft.fft(y))[1:(t.shape[0] // 3)]
-        index, peak_height = find_peaks(amp / np.max(amp),
-                                        height=0.01,
-                                        distance=(t.shape[0] // 3))
-        index = index[np.argsort(peak_height)[-1]]
-        freq = freq[index]
-        spec = np.max(amp) * 2 / len(t)
-    else:
-        spec = 0.0
-
-    A = np.median(np.abs(y - B)) * np.sqrt(2)
-
-    if spec < 0.2 * A:
-        freq = 0.25 / (t[-1] - t[0])
-
-    freq = max(1.0, freq)
-    T = 1 / freq
-    N = len(t[t <= T])
-
-    A0 = np.median(np.abs(y[:N] - B)) * np.sqrt(2)
-    A1 = np.median(np.abs(y[-N:] - B)) * np.sqrt(2)
-    att = -np.log(min(1, A1 / A0))
-    if att < 1e-16:
-        Tr = 1.0
-    elif 2 * T > (t[-1] - t[0]):
-        Tr = (t[-1] - t[0]) / att
-    else:
-        Tr = (t[-1] - t[0] - T) / att
-
-    return {'A': A0, 'B': B, 'Tr': Tr, 'freq': freq, 'phi': np.pi}
-
-
-def fit_rabi(t, y, freq=None, static_params=None):
-    """
-    Fit Rabi oscillation data to a cosine function.
-
-    Args:
-        t (np.ndarray): time array
-        y (np.ndarray): data array
-        Tr (float): Rabi oscillation decay time
-        phi (float): phase
-        freq (float): Rabi frequency
-        static_params (dict): static parameters for fitting
-
-    Returns:
-        popt (np.ndarray): optimized parameters
-        pcov (np.ndarray): covariance matrix
-        fitted (np.ndarray): fitted data
-    """
-
-    return fit(func_rabi,
-               t,
-               y,
-               guess=functools.partial(guess_rabi, freq=freq),
-               static_params=static_params)
```

### Comparing `waveforms-1.5.83/waveforms/math/fit/readout.py` & `waveforms-1.5.84/waveforms/math/fit/readout.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def default_classify(data, params):
     """
     默认的分类方法
     """
     thr = params.get('threshold', 0)
     phi = params.get('phi', 0)
-    return (data * np.exp(-1j * phi)).real > thr
+    return 1 + ((data * np.exp(-1j * phi)).real > thr)
 
 
 def classify_svm(data, params):
     """
     分类方法：SVM
     """
     raise NotImplementedError
@@ -239,20 +239,26 @@
 
 
 def median_complex(c, axis=None):
     return np.median(c.real, axis=axis) + 1j * np.median(c.imag, axis=axis)
 
 
 def fit_readout_distribution(s0, s1):
-    center = 0.5 * (median_complex(s0) + median_complex(s1))
-    s0, s1 = s0 - center, s1 - center
-
-    scale = np.max([np.abs(median_complex(s0)), np.abs(median_complex(s1)), s0.std(), s1.std()])
+    centers = [median_complex(s0), median_complex(s1)]
+    for _ in range(3):
+        m0 = classify_nearest(s0, {'centers': centers}) == 1
+        m1 = classify_nearest(s1, {'centets': centers}) == 2
+        centers = [median_complex(s0[m0]), median_complex(s1[m1])]
 
+    center = np.mean(centers)
+    s0, s1 = s0 - center, s1 - center
+    scale = np.max([np.abs(centers), s0[m0].std(), s1[m1].std()])
     s0, s1 = s0 / scale, s1 / scale
+    centers = [median_complex(s0[m0]), median_complex(s1[m1])]
+    r0, r1 = np.std(s0[m0]), np.std(s1[m1])
 
     def a_b_phi_2_cov(a, b, phi):
         m = np.array([[np.cos(phi) * a, -np.sin(phi) * b],
                       [np.sin(phi) * a, np.cos(phi) * b]])
 
         return m @ m.T
 
@@ -272,30 +278,24 @@
         cr0, cr1, rr0, rr1, ci0, ci1, ri0, ri1, p0, p1, phi0, phi1 = params
 
         c0, c1 = cr0 + 1j * ci0, cr1 + 1j * ci1
 
         cov0 = a_b_phi_2_cov(rr0, ri0, phi0)
         cov1 = a_b_phi_2_cov(rr1, ri1, phi1)
 
-        eps = 1e-20
+        eps = 1e-100
         return (
             -np.log(readout_distribution(s0, p0, c0, c1, cov0, cov1) +
                     eps).sum() -
             np.log(readout_distribution(s1, p1, c0, c1, cov0, cov1) +
                    eps).sum())
 
     res = minimize(loss, [
-        np.median(s0.real),
-        np.median(s1.real),
-        s0.real.std(),
-        s1.real.std(),
-        np.median(s0.imag),
-        np.median(s1.imag),
-        s0.imag.std(),
-        s1.imag.std(), 1, 0, 0, 0
+        centers[0].real, centers[1].real, r0, r1, centers[0].imag,
+        centers[1].imag, r0, r1, 1.0, 0.0, 0, 0
     ],
                    args=(s0, s1),
                    bounds=[(None, None), (None, None), (1e-6, None),
                            (1e-6, None), (None, None), (None, None),
                            (1e-6, None), (1e-6, None), (0, 1), (0, 1),
                            (0, 2 * np.pi), (0, 2 * np.pi)])
```

### Comparing `waveforms-1.5.83/waveforms/math/fit/resonator.py` & `waveforms-1.5.84/waveforms/math/fit/resonator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/fit/simple.py` & `waveforms-1.5.84/waveforms/math/fit/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/graph.py` & `waveforms-1.5.84/waveforms/math/graph.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/prime.py` & `waveforms-1.5.84/waveforms/math/prime.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/signal/demodulate.py` & `waveforms-1.5.84/waveforms/math/signal/demodulate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/signal/distortion.py` & `waveforms-1.5.84/waveforms/math/signal/distortion.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/math/signal/func.py` & `waveforms-1.5.84/waveforms/math/signal/func.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/namespace.py` & `waveforms-1.5.84/waveforms/namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/arch/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/assembly.py` & `waveforms-1.5.84/waveforms/qlisp/assembly.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/base.py` & `waveforms-1.5.84/waveforms/qlisp/base.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/commands.py` & `waveforms-1.5.84/waveforms/qlisp/commands.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/compiler.py` & `waveforms-1.5.84/waveforms/qlisp/compiler.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/config.py` & `waveforms-1.5.84/waveforms/qlisp/config.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/interpreter.py` & `waveforms-1.5.84/waveforms/qlisp/interpreter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/library.py` & `waveforms-1.5.84/waveforms/qlisp/library.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/libs/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/macro.py` & `waveforms-1.5.84/waveforms/qlisp/macro.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/parse.py` & `waveforms-1.5.84/waveforms/qlisp/parse.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/prog.py` & `waveforms-1.5.84/waveforms/qlisp/prog.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/eval.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/eval.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/exceptions.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/libs/qelib1.inc` & `waveforms-1.5.84/waveforms/qlisp/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/barrier.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryop.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryoperator.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/creg.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/customunitary.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/expressionlist.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/external.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/format.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/gate.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/gatebody.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/id.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/idlist.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/if_.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/indexedid.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/intnode.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/measure.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/node.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/nodeexception.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/opaque.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/prefix.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/primarylist.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/program.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/qreg.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/real.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/reset.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/node/unaryoperator.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/qasm.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/qasmlexer.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/qasm/qasmparser.py` & `waveforms-1.5.84/waveforms/qlisp/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/simulator/__init__.py` & `waveforms-1.5.84/waveforms/qlisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/simulator/mat.py` & `waveforms-1.5.84/waveforms/qlisp/simulator/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/simulator/simple.py` & `waveforms-1.5.84/waveforms/qlisp/simulator/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/tokenize.py` & `waveforms-1.5.84/waveforms/qlisp/tokenize.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/qlisp/utils.py` & `waveforms-1.5.84/waveforms/qlisp/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/clifford/clifford.py` & `waveforms-1.5.84/waveforms/quantum/clifford/clifford.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/clifford/db.py` & `waveforms-1.5.84/waveforms/quantum/clifford/db.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/clifford/mat.py` & `waveforms-1.5.84/waveforms/quantum/clifford/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/clifford/seq2mat.py` & `waveforms-1.5.84/waveforms/quantum/clifford/seq2mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/math.py` & `waveforms-1.5.84/waveforms/quantum/math.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/rb.py` & `waveforms-1.5.84/waveforms/quantum/rb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/tomo.py` & `waveforms-1.5.84/waveforms/quantum/tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/quantum/xeb.py` & `waveforms-1.5.84/waveforms/quantum/xeb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/registry.py` & `waveforms-1.5.84/waveforms/registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/scan_iter.py` & `waveforms-1.5.84/waveforms/scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/security/verify.py` & `waveforms-1.5.84/waveforms/security/verify.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/server/__init__.py` & `waveforms-1.5.84/waveforms/server/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/server/__main__.py` & `waveforms-1.5.84/waveforms/server/__main__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/server/umsgpack.py` & `waveforms-1.5.84/waveforms/server/umsgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/device/basedevice.py` & `waveforms-1.5.84/waveforms/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/device/loader.py` & `waveforms-1.5.84/waveforms/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/device/utils.py` & `waveforms-1.5.84/waveforms/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/drivers/FakeInstrument.py` & `waveforms-1.5.84/waveforms/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/ipy_events.py` & `waveforms-1.5.84/waveforms/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/net/dhcp.py` & `waveforms-1.5.84/waveforms/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/net/dhcpd.py` & `waveforms-1.5.84/waveforms/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/net/kad.py` & `waveforms-1.5.84/waveforms/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/net/kcp.py` & `waveforms-1.5.84/waveforms/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/progress.py` & `waveforms-1.5.84/waveforms/sys/progress.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/storage/crud.py` & `waveforms-1.5.84/waveforms/sys/storage/crud.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/sys/storage/models.py` & `waveforms-1.5.84/waveforms/sys/storage/models.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/units/__init__.py` & `waveforms-1.5.84/waveforms/units/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/visualization/__init__.py` & `waveforms-1.5.84/waveforms/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/visualization/plot_layout.py` & `waveforms-1.5.84/waveforms/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/visualization/plot_seq.py` & `waveforms-1.5.84/waveforms/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/waveform.py` & `waveforms-1.5.84/waveforms/waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms/waveform_parser.py` & `waveforms-1.5.84/waveforms/waveform_parser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.83/waveforms.egg-info/PKG-INFO` & `waveforms-1.5.84/waveforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.83
+Version: 1.5.84
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.83/waveforms.egg-info/SOURCES.txt` & `waveforms-1.5.84/waveforms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 waveforms.egg-info/requires.txt
 waveforms.egg-info/top_level.txt
 waveforms/math/__init__.py
 waveforms/math/bayes.py
 waveforms/math/fibheap.py
 waveforms/math/graph.py
 waveforms/math/prime.py
+waveforms/math/transmon.py
 waveforms/math/fit/__init__.py
+waveforms/math/fit/_fit.py
 waveforms/math/fit/delay.py
 waveforms/math/fit/geo.py
 waveforms/math/fit/qubit_dynamics.py
 waveforms/math/fit/readout.py
 waveforms/math/fit/resonator.py
 waveforms/math/fit/simple.py
 waveforms/math/fit/spectrum.py
@@ -139,14 +141,15 @@
 waveforms/quantum/clifford/seq2mat.py
 waveforms/security/__init__.py
 waveforms/security/verify.py
 waveforms/server/__init__.py
 waveforms/server/__main__.py
 waveforms/server/umsgpack.py
 waveforms/sys/__init__.py
+waveforms/sys/chat.py
 waveforms/sys/ipy_events.py
 waveforms/sys/progress.py
 waveforms/sys/device/__init__.py
 waveforms/sys/device/basedevice.py
 waveforms/sys/device/loader.py
 waveforms/sys/device/utils.py
 waveforms/sys/drivers/FakeInstrument.py
```

