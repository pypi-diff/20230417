# Comparing `tmp/dovado-rtl-0.9.8.tar.gz` & `tmp/dovado-rtl-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dovado-rtl-0.9.8.tar", max compression
+gzip compressed data, was "dovado-rtl-0.9.9.tar", max compression
```

## Comparing `dovado-rtl-0.9.8.tar` & `dovado-rtl-0.9.9.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0     1072 2021-12-30 11:05:02.740574 dovado-rtl-0.9.8/LICENSE
--rw-r--r--   0        0        0    13328 2021-12-30 11:05:02.740574 dovado-rtl-0.9.8/README.md
--rw-r--r--   0        0        0     1327 2021-12-30 19:43:31.531379 dovado-rtl-0.9.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.747240 dovado-rtl-0.9.8/src/dovado_rtl/__init__.py
--rw-r--r--   0        0        0     2891 2021-12-30 11:05:02.747240 dovado-rtl-0.9.8/src/dovado_rtl/abstract_classes.py
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.747240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__init__.py
--rw-r--r--   0        0        0     5375 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-36.pyc
--rw-r--r--   0        0        0     5743 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-38.pyc
--rw-r--r--   0        0        0    20538 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    20567 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    12325 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    12295 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    11157 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    10919 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-38.pyc
--rw-r--r--   0        0        0      137 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      220 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      145 2021-12-30 18:10:27.201693 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6296 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-36.pyc
--rw-r--r--   0        0        0     6578 2021-12-30 19:31:01.046066 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-39.pyc
--rw-r--r--   0        0        0    21052 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-36.pyc
--rw-r--r--   0        0        0    20981 2021-12-30 18:10:28.231695 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-39.pyc
--rw-r--r--   0        0        0    12101 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-36.pyc
--rw-r--r--   0        0        0    12065 2021-12-30 18:10:27.715027 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-39.pyc
--rw-r--r--   0        0        0    35614 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlLexer.cpython-38.pyc
--rw-r--r--   0        0        0    93001 2021-12-30 11:05:02.750573 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlListener.cpython-38.pyc
--rw-r--r--   0        0        0   762490 2021-12-30 11:05:02.757240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlParser.cpython-38.pyc
--rw-r--r--   0        0        0    13229 2021-12-30 11:05:02.757240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlTree.cpython-38.pyc
--rw-r--r--   0        0        0    51719 2021-12-30 11:05:02.757240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    13202 2021-12-30 11:05:02.757240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-36.pyc
--rw-r--r--   0        0        0    13293 2021-12-30 18:10:27.425027 dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-39.pyc
--rw-r--r--   0        0        0   118315 2021-12-30 11:05:02.757240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.interp
--rw-r--r--   0        0        0   145460 2021-12-30 11:05:02.760574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.py
--rw-r--r--   0        0        0     8475 2021-12-30 11:05:02.760574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.tokens
--rw-r--r--   0        0        0   314695 2021-12-30 11:05:02.760574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.interp
--rw-r--r--   0        0        0  2587611 2021-12-30 11:05:02.767240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.py
--rw-r--r--   0        0        0     8475 2021-12-30 11:05:02.767240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.tokens
--rw-r--r--   0        0        0   230516 2021-12-30 11:05:02.767240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserListener.py
--rw-r--r--   0        0        0   132602 2021-12-30 11:05:02.767240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserVisitor.py
--rw-r--r--   0        0        0    87082 2021-12-30 11:05:02.767240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-36.pyc
--rw-r--r--   0        0        0    84243 2021-12-30 18:10:28.201695 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-39.pyc
--rw-r--r--   0        0        0  2184428 2021-12-30 11:05:02.773907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-36.pyc
--rw-r--r--   0        0        0  2113885 2021-12-30 18:10:28.115028 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-39.pyc
--rw-r--r--   0        0        0   138587 2021-12-30 11:05:02.777240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-36.pyc
--rw-r--r--   0        0        0   136737 2021-12-30 18:10:28.241695 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-39.pyc
--rw-r--r--   0        0        0   164706 2021-12-30 11:05:02.777240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.interp
--rw-r--r--   0        0        0   201938 2021-12-30 11:05:02.777240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.py
--rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.777240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.tokens
--rw-r--r--   0        0        0   166460 2021-12-30 11:05:02.777240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.interp
--rw-r--r--   0        0        0  1292417 2021-12-30 11:05:02.783907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.py
--rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.783907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.tokens
--rw-r--r--   0        0        0   118219 2021-12-30 11:05:02.783907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserListener.py
--rw-r--r--   0        0        0    68812 2021-12-30 11:05:02.783907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserVisitor.py
--rw-r--r--   0        0        0    16560 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.interp
--rw-r--r--   0        0        0   111864 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.py
--rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.tokens
--rw-r--r--   0        0        0    13241 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserListener.py
--rw-r--r--   0        0        0     7736 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserVisitor.py
--rw-r--r--   0        0        0   118793 2021-12-30 11:05:02.787240 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-36.pyc
--rw-r--r--   0        0        0   115493 2021-12-30 18:10:27.675027 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-39.pyc
--rw-r--r--   0        0        0  1118121 2021-12-30 11:05:02.790574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-36.pyc
--rw-r--r--   0        0        0  1078619 2021-12-30 18:10:27.621694 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-39.pyc
--rw-r--r--   0        0        0    73832 2021-12-30 11:05:02.790574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    72813 2021-12-30 18:10:27.718361 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-39.pyc
--rw-r--r--   0        0        0       23 2021-12-30 11:05:02.790574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/__init__.py
--rw-r--r--   0        0        0      147 2021-12-30 11:05:02.790574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      155 2021-12-30 18:10:27.251693 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34953 2021-12-30 11:05:02.790574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc
--rw-r--r--   0        0        0    34463 2021-12-30 18:10:27.258360 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc
--rw-r--r--   0        0        0   780845 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc
--rw-r--r--   0        0        0   756360 2021-12-30 18:10:27.395027 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc
--rw-r--r--   0        0        0    52120 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    51374 2021-12-30 18:10:27.428360 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-39.pyc
--rw-r--r--   0        0        0   101414 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdl.interp
--rw-r--r--   0        0        0     2009 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdl.tokens
--rw-r--r--   0        0        0    49712 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.interp
--rw-r--r--   0        0        0    61443 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.py
--rw-r--r--   0        0        0     2009 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.tokens
--rw-r--r--   0        0        0    84456 2021-12-30 11:05:02.797241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlListener.py
--rw-r--r--   0        0        0   834953 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlParser.py
--rw-r--r--   0        0        0    49410 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlVisitor.py
--rw-r--r--   0        0        0     8683 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/SystemVerilogLexer.g4
--rw-r--r--   0        0        0    75116 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/SystemVerilogParser.g4
--rw-r--r--   0        0        0    18308 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogLexer.g4
--rw-r--r--   0        0        0    49548 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogParser.g4
--rw-r--r--   0        0        0     3732 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogPreprocessorParser.g4
--rw-r--r--   0        0        0    32924 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/vhdl.g4
--rw-r--r--   0        0        0     4578 2021-12-30 19:27:57.748366 dovado-rtl-0.9.8/src/dovado_rtl/antlr/hdl_representation.py
--rw-r--r--   0        0        0   122049 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.interp
--rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.tokens
--rw-r--r--   0        0        0    77969 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.interp
--rw-r--r--   0        0        0    93629 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.py
--rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.800574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.tokens
--rw-r--r--   0        0        0   169220 2021-12-30 11:05:02.803907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLListener.py
--rw-r--r--   0        0        0  1240332 2021-12-30 11:05:02.807241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLParser.py
--rw-r--r--   0        0        0    97052 2021-12-30 11:05:02.807241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLVisitor.py
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.807241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__init__.py
--rw-r--r--   0        0        0    54911 2021-12-30 11:05:02.807241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-36.pyc
--rw-r--r--   0        0        0    56112 2021-12-30 11:05:02.810574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-38.pyc
--rw-r--r--   0        0        0    53058 2021-12-30 11:05:02.810574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-39.pyc
--rw-r--r--   0        0        0  1209666 2021-12-30 11:05:02.813907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-36.pyc
--rw-r--r--   0        0        0  1173412 2021-12-30 11:05:02.813907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-38.pyc
--rw-r--r--   0        0        0  1172276 2021-12-30 11:05:02.817241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-39.pyc
--rw-r--r--   0        0        0    98397 2021-12-30 11:05:02.817241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    97156 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    97081 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-39.pyc
--rw-r--r--   0        0        0      161 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      244 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      169 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0   152243 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.interp
--rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.tokens
--rw-r--r--   0        0        0    57404 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.interp
--rw-r--r--   0        0        0    66763 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.py
--rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.tokens
--rw-r--r--   0        0        0   112230 2021-12-30 11:05:02.820574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Listener.py
--rw-r--r--   0        0        0  1069709 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Parser.py
--rw-r--r--   0        0        0    64809 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Visitor.py
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__init__.py
--rw-r--r--   0        0        0    39871 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-36.pyc
--rw-r--r--   0        0        0    40592 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-38.pyc
--rw-r--r--   0        0        0    38490 2021-12-30 11:05:02.827241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-39.pyc
--rw-r--r--   0        0        0   887643 2021-12-30 11:05:02.830574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-36.pyc
--rw-r--r--   0        0        0   857612 2021-12-30 11:05:02.830574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-38.pyc
--rw-r--r--   0        0        0   857723 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-39.pyc
--rw-r--r--   0        0        0    66090 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-36.pyc
--rw-r--r--   0        0        0    65257 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-38.pyc
--rw-r--r--   0        0        0    65182 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-39.pyc
--rw-r--r--   0        0        0      159 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      242 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      167 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/__init__.py
--rw-r--r--   0        0        0      147 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      230 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      155 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__init__.py
--rw-r--r--   0        0        0      152 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      235 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      160 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    38096 2021-12-30 11:05:02.833907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc
--rw-r--r--   0        0        0    38237 2021-12-30 11:05:02.837241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-38.pyc
--rw-r--r--   0        0        0    36771 2021-12-30 11:05:02.837241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc
--rw-r--r--   0        0        0   799930 2021-12-30 11:05:02.837241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc
--rw-r--r--   0        0        0   774973 2021-12-30 11:05:02.837241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-38.pyc
--rw-r--r--   0        0        0   774638 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc
--rw-r--r--   0        0        0    54703 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    54026 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    53951 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-39.pyc
--rw-r--r--   0        0        0    52198 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc
--rw-r--r--   0        0        0    51732 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-38.pyc
--rw-r--r--   0        0        0    53014 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.interp
--rw-r--r--   0        0        0    67415 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.py
--rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.tokens
--rw-r--r--   0        0        0   102342 2021-12-30 11:05:02.840574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.interp
--rw-r--r--   0        0        0   853082 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.py
--rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.tokens
--rw-r--r--   0        0        0    86358 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserListener.py
--rw-r--r--   0        0        0    50421 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserVisitor.py
--rw-r--r--   0        0        0   122049 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.interp
--rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.tokens
--rw-r--r--   0        0        0    77969 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.interp
--rw-r--r--   0        0        0    75993 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.java
--rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.843907 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.tokens
--rw-r--r--   0        0        0   799095 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLParser.java
--rw-r--r--   0        0        0   152243 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.interp
--rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.tokens
--rw-r--r--   0        0        0    57404 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.interp
--rw-r--r--   0        0        0    55301 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.java
--rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.847241 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.tokens
--rw-r--r--   0        0        0   690943 2021-12-30 11:05:02.850574 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Parser.java
--rw-r--r--   0        0        0    53014 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.interp
--rw-r--r--   0        0        0    53867 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.java
--rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.tokens
--rw-r--r--   0        0        0   102342 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.interp
--rw-r--r--   0        0        0   575406 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.java
--rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.tokens
--rw-r--r--   0        0        0    53507 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/SysVerilogHDL.g4
--rw-r--r--   0        0        0    47353 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/Verilog2001.g4
--rw-r--r--   0        0        0     6917 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlLexer.g4
--rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlLexer.tokens
--rw-r--r--   0        0        0    25061 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlParser.g4
--rw-r--r--   0        0        0    22803 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/sysverilog_entity_visitor.py
--rw-r--r--   0        0        0    12958 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/verilog2001_entity_visitor.py
--rw-r--r--   0        0        0    14153 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/antlr/vhdl_entity_visitor.py
--rw-r--r--   0        0        0    11297 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/cli_utility.py
--rw-r--r--   0        0        0     3145 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/config.py
--rw-r--r--   0        0        0     1861 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/doc_parsing.py
--rw-r--r--   0        0        0      260 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/enums.py
--rw-r--r--   0        0        0     1449 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/fill_handler.py
--rw-r--r--   0        0        0     1136 2021-12-30 11:05:02.853908 dovado-rtl-0.9.8/src/dovado_rtl/fitness.py
--rw-r--r--   0        0        0    10457 2021-12-30 19:28:46.558644 dovado-rtl-0.9.8/src/dovado_rtl/frame_handling.py
--rw-r--r--   0        0        0     4388 2021-12-30 19:44:58.988687 dovado-rtl-0.9.8/src/dovado_rtl/genetic_algorithm.py
--rw-r--r--   0        0        0    12159 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/main.py
--rw-r--r--   0        0        0     8674 2021-12-30 18:57:37.558543 dovado-rtl-0.9.8/src/dovado_rtl/point_evaluation.py
--rw-r--r--   0        0        0     2910 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/report_parsing.py
--rw-r--r--   0        0        0      511 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/simple_types.py
--rw-r--r--   0        0        0     7953 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/src_parsing.py
--rw-r--r--   0        0        0      883 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/visualize.py
--rw-r--r--   0        0        0     1841 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/src/dovado_rtl/vivado_interaction.py
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/__init__.py
--rw-r--r--   0        0        0     1797 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/full_evalutate_point_frame.tcl
--rw-r--r--   0        0        0     1983 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/implementation.tcl
--rw-r--r--   0        0        0     2938 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/implementation_frame.tcl
--rw-r--r--   0        0        0     1270 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/procs.tcl
--rw-r--r--   0        0        0     1447 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/synthesis.tcl
--rw-r--r--   0        0        0     2440 2021-12-30 11:05:02.857241 dovado-rtl-0.9.8/tcl/synthesis_frame.tcl
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/verilog/__init__.py
--rw-r--r--   0        0        0      788 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/verilog/box.sv
--rw-r--r--   0        0        0      311 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/verilog/box_frame.sv
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/vhdl/__init__.py
--rw-r--r--   0        0        0      657 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/vhdl/box.vhd
--rw-r--r--   0        0        0      447 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/vhdl/box_frame.vhd
--rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/xdc/__init__.py
--rw-r--r--   0        0        0       41 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/xdc/constraint.xdc
--rw-r--r--   0        0        0       42 2021-12-30 11:05:02.860574 dovado-rtl-0.9.8/xdc/constraint_frame.xdc
--rw-r--r--   0        0        0    15412 2021-12-30 19:45:11.976650 dovado-rtl-0.9.8/setup.py
--rw-r--r--   0        0        0    14593 2021-12-30 19:45:11.977216 dovado-rtl-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-12-30 11:05:02.740574 dovado-rtl-0.9.9/LICENSE
+-rw-r--r--   0        0        0    13328 2021-12-30 11:05:02.740574 dovado-rtl-0.9.9/README.md
+-rw-r--r--   0        0        0     1327 2022-01-04 15:39:04.098418 dovado-rtl-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.747240 dovado-rtl-0.9.9/src/dovado_rtl/__init__.py
+-rw-r--r--   0        0        0     2891 2021-12-30 11:05:02.747240 dovado-rtl-0.9.9/src/dovado_rtl/abstract_classes.py
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.747240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__init__.py
+-rw-r--r--   0        0        0     5375 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-36.pyc
+-rw-r--r--   0        0        0     5743 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-38.pyc
+-rw-r--r--   0        0        0    20538 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    20567 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    12325 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    12295 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    11157 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    10919 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0      137 2022-01-04 15:35:04.506785 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      220 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      145 2021-12-30 18:10:27.201693 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6328 2022-01-04 15:35:04.506785 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-36.pyc
+-rw-r--r--   0        0        0     6578 2021-12-30 19:31:01.046066 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-39.pyc
+-rw-r--r--   0        0        0    21052 2022-01-04 15:35:05.550125 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-36.pyc
+-rw-r--r--   0        0        0    20981 2021-12-30 18:10:28.231695 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-39.pyc
+-rw-r--r--   0        0        0    12101 2022-01-04 15:35:05.030122 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-36.pyc
+-rw-r--r--   0        0        0    12065 2021-12-30 18:10:27.715027 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-39.pyc
+-rw-r--r--   0        0        0    35614 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlLexer.cpython-38.pyc
+-rw-r--r--   0        0        0    93001 2021-12-30 11:05:02.750573 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlListener.cpython-38.pyc
+-rw-r--r--   0        0        0   762490 2021-12-30 11:05:02.757240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlParser.cpython-38.pyc
+-rw-r--r--   0        0        0    13229 2021-12-30 11:05:02.757240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlTree.cpython-38.pyc
+-rw-r--r--   0        0        0    51719 2021-12-30 11:05:02.757240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    13202 2022-01-04 15:35:04.733453 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-36.pyc
+-rw-r--r--   0        0        0    13293 2021-12-30 18:10:27.425027 dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-39.pyc
+-rw-r--r--   0        0        0   118315 2021-12-30 11:05:02.757240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.interp
+-rw-r--r--   0        0        0   145460 2021-12-30 11:05:02.760574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.py
+-rw-r--r--   0        0        0     8475 2021-12-30 11:05:02.760574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.tokens
+-rw-r--r--   0        0        0   314695 2021-12-30 11:05:02.760574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.interp
+-rw-r--r--   0        0        0  2587611 2021-12-30 11:05:02.767240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.py
+-rw-r--r--   0        0        0     8475 2021-12-30 11:05:02.767240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.tokens
+-rw-r--r--   0        0        0   230516 2021-12-30 11:05:02.767240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserListener.py
+-rw-r--r--   0        0        0   132602 2021-12-30 11:05:02.767240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserVisitor.py
+-rw-r--r--   0        0        0    87082 2022-01-04 15:35:05.510125 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-36.pyc
+-rw-r--r--   0        0        0    84243 2021-12-30 18:10:28.201695 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-39.pyc
+-rw-r--r--   0        0        0  2184428 2022-01-04 15:35:05.393458 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-36.pyc
+-rw-r--r--   0        0        0  2113885 2021-12-30 18:10:28.115028 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-39.pyc
+-rw-r--r--   0        0        0   138587 2022-01-04 15:35:05.560125 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0   136737 2021-12-30 18:10:28.241695 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-39.pyc
+-rw-r--r--   0        0        0   164706 2021-12-30 11:05:02.777240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.interp
+-rw-r--r--   0        0        0   201938 2021-12-30 11:05:02.777240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.py
+-rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.777240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.tokens
+-rw-r--r--   0        0        0   166460 2021-12-30 11:05:02.777240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.interp
+-rw-r--r--   0        0        0  1292417 2021-12-30 11:05:02.783907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.py
+-rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.783907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.tokens
+-rw-r--r--   0        0        0   118219 2021-12-30 11:05:02.783907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserListener.py
+-rw-r--r--   0        0        0    68812 2021-12-30 11:05:02.783907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserVisitor.py
+-rw-r--r--   0        0        0    16560 2021-12-30 11:05:02.787240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.interp
+-rw-r--r--   0        0        0   111864 2021-12-30 11:05:02.787240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.py
+-rw-r--r--   0        0        0    11068 2021-12-30 11:05:02.787240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.tokens
+-rw-r--r--   0        0        0    13241 2021-12-30 11:05:02.787240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserListener.py
+-rw-r--r--   0        0        0     7736 2021-12-30 11:05:02.787240 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserVisitor.py
+-rw-r--r--   0        0        0   118793 2022-01-04 15:35:04.980121 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-36.pyc
+-rw-r--r--   0        0        0   115493 2021-12-30 18:10:27.675027 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-39.pyc
+-rw-r--r--   0        0        0  1118121 2022-01-04 15:35:04.910121 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-36.pyc
+-rw-r--r--   0        0        0  1078619 2021-12-30 18:10:27.621694 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-39.pyc
+-rw-r--r--   0        0        0    73832 2022-01-04 15:35:05.036789 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    72813 2021-12-30 18:10:27.718361 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-39.pyc
+-rw-r--r--   0        0        0       23 2021-12-30 11:05:02.790574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/__init__.py
+-rw-r--r--   0        0        0      147 2022-01-04 15:35:04.563452 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      155 2021-12-30 18:10:27.251693 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    34953 2022-01-04 15:35:04.570119 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc
+-rw-r--r--   0        0        0    34463 2021-12-30 18:10:27.258360 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc
+-rw-r--r--   0        0        0   780845 2022-01-04 15:35:04.696786 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc
+-rw-r--r--   0        0        0   756360 2021-12-30 18:10:27.395027 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc
+-rw-r--r--   0        0        0    52120 2022-01-04 15:35:04.736786 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    51374 2021-12-30 18:10:27.428360 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-39.pyc
+-rw-r--r--   0        0        0   101414 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdl.interp
+-rw-r--r--   0        0        0     2009 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdl.tokens
+-rw-r--r--   0        0        0    49712 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.interp
+-rw-r--r--   0        0        0    61443 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.py
+-rw-r--r--   0        0        0     2009 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.tokens
+-rw-r--r--   0        0        0    84456 2021-12-30 11:05:02.797241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlListener.py
+-rw-r--r--   0        0        0   834953 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlParser.py
+-rw-r--r--   0        0        0    49410 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlVisitor.py
+-rw-r--r--   0        0        0     8683 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/SystemVerilogLexer.g4
+-rw-r--r--   0        0        0    75116 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/SystemVerilogParser.g4
+-rw-r--r--   0        0        0    18308 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogLexer.g4
+-rw-r--r--   0        0        0    49548 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogParser.g4
+-rw-r--r--   0        0        0     3732 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogPreprocessorParser.g4
+-rw-r--r--   0        0        0    32924 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/vhdl.g4
+-rw-r--r--   0        0        0     4578 2021-12-30 19:27:57.748366 dovado-rtl-0.9.9/src/dovado_rtl/antlr/hdl_representation.py
+-rw-r--r--   0        0        0   122049 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.interp
+-rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.tokens
+-rw-r--r--   0        0        0    77969 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.interp
+-rw-r--r--   0        0        0    93629 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.py
+-rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.800574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.tokens
+-rw-r--r--   0        0        0   169220 2021-12-30 11:05:02.803907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLListener.py
+-rw-r--r--   0        0        0  1240332 2021-12-30 11:05:02.807241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLParser.py
+-rw-r--r--   0        0        0    97052 2021-12-30 11:05:02.807241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLVisitor.py
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.807241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__init__.py
+-rw-r--r--   0        0        0    54911 2021-12-30 11:05:02.807241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-36.pyc
+-rw-r--r--   0        0        0    56112 2021-12-30 11:05:02.810574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-38.pyc
+-rw-r--r--   0        0        0    53058 2021-12-30 11:05:02.810574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-39.pyc
+-rw-r--r--   0        0        0  1209666 2021-12-30 11:05:02.813907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-36.pyc
+-rw-r--r--   0        0        0  1173412 2021-12-30 11:05:02.813907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-38.pyc
+-rw-r--r--   0        0        0  1172276 2021-12-30 11:05:02.817241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-39.pyc
+-rw-r--r--   0        0        0    98397 2021-12-30 11:05:02.817241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    97156 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    97081 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-39.pyc
+-rw-r--r--   0        0        0      161 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      244 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      169 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0   152243 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.interp
+-rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.tokens
+-rw-r--r--   0        0        0    57404 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.interp
+-rw-r--r--   0        0        0    66763 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.py
+-rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.tokens
+-rw-r--r--   0        0        0   112230 2021-12-30 11:05:02.820574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Listener.py
+-rw-r--r--   0        0        0  1069709 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Parser.py
+-rw-r--r--   0        0        0    64809 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Visitor.py
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__init__.py
+-rw-r--r--   0        0        0    39871 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-36.pyc
+-rw-r--r--   0        0        0    40592 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-38.pyc
+-rw-r--r--   0        0        0    38490 2021-12-30 11:05:02.827241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-39.pyc
+-rw-r--r--   0        0        0   887643 2021-12-30 11:05:02.830574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-36.pyc
+-rw-r--r--   0        0        0   857612 2021-12-30 11:05:02.830574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-38.pyc
+-rw-r--r--   0        0        0   857723 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-39.pyc
+-rw-r--r--   0        0        0    66090 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-36.pyc
+-rw-r--r--   0        0        0    65257 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-38.pyc
+-rw-r--r--   0        0        0    65182 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-39.pyc
+-rw-r--r--   0        0        0      159 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      242 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      167 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/__init__.py
+-rw-r--r--   0        0        0      147 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      230 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      155 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__init__.py
+-rw-r--r--   0        0        0      152 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      235 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      160 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    38096 2021-12-30 11:05:02.833907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc
+-rw-r--r--   0        0        0    38237 2021-12-30 11:05:02.837241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-38.pyc
+-rw-r--r--   0        0        0    36771 2021-12-30 11:05:02.837241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc
+-rw-r--r--   0        0        0   799930 2021-12-30 11:05:02.837241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc
+-rw-r--r--   0        0        0   774973 2021-12-30 11:05:02.837241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-38.pyc
+-rw-r--r--   0        0        0   774638 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc
+-rw-r--r--   0        0        0    54703 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    54026 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    53951 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-39.pyc
+-rw-r--r--   0        0        0    52198 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc
+-rw-r--r--   0        0        0    51732 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-38.pyc
+-rw-r--r--   0        0        0    53014 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.interp
+-rw-r--r--   0        0        0    67415 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.py
+-rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.tokens
+-rw-r--r--   0        0        0   102342 2021-12-30 11:05:02.840574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.interp
+-rw-r--r--   0        0        0   853082 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.py
+-rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.tokens
+-rw-r--r--   0        0        0    86358 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserListener.py
+-rw-r--r--   0        0        0    50421 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserVisitor.py
+-rw-r--r--   0        0        0   122049 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.interp
+-rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.tokens
+-rw-r--r--   0        0        0    77969 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.interp
+-rw-r--r--   0        0        0    75993 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.java
+-rw-r--r--   0        0        0     5303 2021-12-30 11:05:02.843907 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.tokens
+-rw-r--r--   0        0        0   799095 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLParser.java
+-rw-r--r--   0        0        0   152243 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.interp
+-rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.tokens
+-rw-r--r--   0        0        0    57404 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.interp
+-rw-r--r--   0        0        0    55301 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.java
+-rw-r--r--   0        0        0     3707 2021-12-30 11:05:02.847241 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.tokens
+-rw-r--r--   0        0        0   690943 2021-12-30 11:05:02.850574 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Parser.java
+-rw-r--r--   0        0        0    53014 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.interp
+-rw-r--r--   0        0        0    53867 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.java
+-rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.tokens
+-rw-r--r--   0        0        0   102342 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.interp
+-rw-r--r--   0        0        0   575406 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.java
+-rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.tokens
+-rw-r--r--   0        0        0    53507 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/SysVerilogHDL.g4
+-rw-r--r--   0        0        0    47353 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/Verilog2001.g4
+-rw-r--r--   0        0        0     6917 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlLexer.g4
+-rw-r--r--   0        0        0     2424 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlLexer.tokens
+-rw-r--r--   0        0        0    25061 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlParser.g4
+-rw-r--r--   0        0        0    22803 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/sysverilog_entity_visitor.py
+-rw-r--r--   0        0        0    12958 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/verilog2001_entity_visitor.py
+-rw-r--r--   0        0        0    14153 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/antlr/vhdl_entity_visitor.py
+-rw-r--r--   0        0        0    11297 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/cli_utility.py
+-rw-r--r--   0        0        0     3145 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/config.py
+-rw-r--r--   0        0        0     1861 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/doc_parsing.py
+-rw-r--r--   0        0        0      260 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/enums.py
+-rw-r--r--   0        0        0     1449 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/fill_handler.py
+-rw-r--r--   0        0        0     1136 2021-12-30 11:05:02.853908 dovado-rtl-0.9.9/src/dovado_rtl/fitness.py
+-rw-r--r--   0        0        0    10457 2021-12-30 19:28:46.558644 dovado-rtl-0.9.9/src/dovado_rtl/frame_handling.py
+-rw-r--r--   0        0        0     4388 2021-12-30 19:44:58.988687 dovado-rtl-0.9.9/src/dovado_rtl/genetic_algorithm.py
+-rw-r--r--   0        0        0    12159 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/main.py
+-rw-r--r--   0        0        0     8531 2022-01-04 14:50:34.063320 dovado-rtl-0.9.9/src/dovado_rtl/point_evaluation.py
+-rw-r--r--   0        0        0     2910 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/report_parsing.py
+-rw-r--r--   0        0        0      511 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/simple_types.py
+-rw-r--r--   0        0        0     7953 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/src_parsing.py
+-rw-r--r--   0        0        0      883 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/visualize.py
+-rw-r--r--   0        0        0     1841 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/src/dovado_rtl/vivado_interaction.py
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/__init__.py
+-rw-r--r--   0        0        0     1797 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/full_evalutate_point_frame.tcl
+-rw-r--r--   0        0        0     1983 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/implementation.tcl
+-rw-r--r--   0        0        0     2938 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/implementation_frame.tcl
+-rw-r--r--   0        0        0     1270 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/procs.tcl
+-rw-r--r--   0        0        0     1447 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/synthesis.tcl
+-rw-r--r--   0        0        0     2440 2021-12-30 11:05:02.857241 dovado-rtl-0.9.9/tcl/synthesis_frame.tcl
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/verilog/__init__.py
+-rw-r--r--   0        0        0      788 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/verilog/box.sv
+-rw-r--r--   0        0        0      311 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/verilog/box_frame.sv
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/vhdl/__init__.py
+-rw-r--r--   0        0        0      657 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/vhdl/box.vhd
+-rw-r--r--   0        0        0      447 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/vhdl/box_frame.vhd
+-rw-r--r--   0        0        0        0 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/xdc/__init__.py
+-rw-r--r--   0        0        0       41 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/xdc/constraint.xdc
+-rw-r--r--   0        0        0       42 2021-12-30 11:05:02.860574 dovado-rtl-0.9.9/xdc/constraint_frame.xdc
+-rw-r--r--   0        0        0    15412 2022-01-04 15:39:14.343492 dovado-rtl-0.9.9/setup.py
+-rw-r--r--   0        0        0    14593 2022-01-04 15:39:14.344133 dovado-rtl-0.9.9/PKG-INFO
```

### Comparing `dovado-rtl-0.9.8/LICENSE` & `dovado-rtl-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/README.md` & `dovado-rtl-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/pyproject.toml` & `dovado-rtl-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dovado-rtl"
-version = "0.9.8"
+version = "0.9.9"
 description = "CLI tool for RTL Design Space Exploration on top of Vivado"
 authors = ["Daniele Paletti <danielepaletti98@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DPaletti/dovado"
 repository = "https://github.com/DPaletti/dovado"
 keywords = [
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/abstract_classes.py` & `dovado-rtl-0.9.9/src/dovado_rtl/abstract_classes.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/HdlRepresentation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/SysVerilogHDLEntityVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/Verilog2001EntityVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/VhdlEntityVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/hdl_representation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 9b1a c661 1359 0000 e300 0000  3......a.Y......
+00000000: 330d 0d0a 5e92 cd61 1359 0000 e300 0000  3...^..a.Y......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 7c00 0000 6400 6401 6c00 6d01 5a01  .s|...d.d.l.m.Z.
 00000030: 6d02 5a02 6d03 5a03 6d04 5a04 6d05 5a05  m.Z.m.Z.m.Z.m.Z.
 00000040: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 0100 6400 6404 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/sysverilog_entity_visitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 13d4 c561 9e32 0000 e300 0000  3......a.2......
+00000000: 330d 0d0a 5e92 cd61 9e32 0000 e300 0000  3...^..a.2......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6800 0000 6400 6401 6c00 6d01 5a01  .sh...d.d.l.m.Z.
 00000030: 6d02 5a02 6d03 5a03 6d04 5a04 6d05 5a05  m.Z.m.Z.m.Z.m.Z.
 00000040: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c0c 6d0d 5a0d 0100 6400 6404 6c0e  d.l.m.Z...d.d.l.
 00000070: 6d0f 5a0f 6d10 5a10 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/verilog2001_entity_visitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlLexer.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlListener.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlListener.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlParser.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlParser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlTree.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlTree.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdlVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdlVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 29d2 c561 4937 0000 e300 0000  3...)..aI7......
+00000000: 330d 0d0a 5e92 cd61 4937 0000 e300 0000  3...^..aI7......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 8400 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 6d02 5a02 6d03 5a03 6d04 5a04 6d05 5a05  m.Z.m.Z.m.Z.m.Z.
 00000040: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d0a 5a0a 0100 6400 6402 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/__pycache__/vhdl_entity_visitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParser.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/SystemVerilogParserVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 74b8 c561 3438 0200 e300 0000  3...t..a48......
+00000000: 330d 0d0a 5e92 cd61 3438 0200 e300 0000  3...^..a48......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogLexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 7bb8 c561 db7b 2700 e300 0000  3...{..a.{'.....
+00000000: 330d 0d0a 5e92 cd61 db7b 2700 e300 0000  3...^..a.{'.....
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 7bb8 c561 fa05 0200 e300 0000  3...{..a........
+00000000: 330d 0d0a 5e92 cd61 fa05 0200 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 4800 0000 6400 6401 6c00 5400 6501  .sH...d.d.l.T.e.
 00000030: 6402 6b09 7226 6403 6501 6b06 7226 6404  d.k.r&d.e.k.r&d.
 00000040: 6405 6c02 6d02 5a02 0100 6e0c 6400 6405  d.l.m.Z...n.d.d.
 00000050: 6c02 6d02 5a02 0100 4700 6406 6407 8400  l.m.Z...G.d.d...
 00000060: 6407 6503 8303 5a04 5b02 6402 5300 2908  d.e...Z.[.d.S.).
 00000070: e900 0000 0029 01da 012a 4eda 012e e901  .....)...*N.....
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/SystemVerilog/__pycache__/SystemVerilogParserVisitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParser.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogParserVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParser.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/VerilogPreprocessorParserVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 0db8 c561 d214 0300 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 d214 0300 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogLexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 13b8 c561 81b8 1300 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 81b8 1300 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 13b8 c561 cc0c 0100 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 cc0c 0100 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 4800 0000 6400 6401 6c00 5400 6501  .sH...d.d.l.T.e.
 00000030: 6402 6b09 7226 6403 6501 6b06 7226 6404  d.k.r&d.e.k.r&d.
 00000040: 6405 6c02 6d02 5a02 0100 6e0c 6400 6405  d.l.m.Z...n.d.d.
 00000050: 6c02 6d02 5a02 0100 4700 6406 6407 8400  l.m.Z...G.d.d...
 00000060: 6407 6503 8303 5a04 5b02 6402 5300 2908  d.e...Z.[.d.S.).
 00000070: e900 0000 0029 01da 012a 4eda 012e e901  .....)...*N.....
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/Verilog2001/__pycache__/VerilogParserVisitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a cab7 c561 03f0 0000 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 03f0 0000 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
@@ -2066,15 +2066,15 @@
 00008110: 0029 024e 7a05 342e 392e 3329 0ada 0573  .).Nz.4.9.3)...s
 00008120: 7570 6572 da08 5f5f 696e 6974 5f5f da0c  uper..__init__..
 00008130: 6368 6563 6b56 6572 7369 6f6e da11 4c65  checkVersion..Le
 00008140: 7865 7241 544e 5369 6d75 6c61 746f 72da  xerATNSimulator.
 00008150: 0361 746e da0e 6465 6369 7369 6f6e 7354  .atn..decisionsT
 00008160: 6f44 4641 da16 5072 6564 6963 7469 6f6e  oDFA..Prediction
 00008170: 436f 6e74 6578 7443 6163 6865 da07 5f69  ContextCache.._i
-00008180: 6e74 6572 70da 085f 6163 7469 6f6e 735a  nterp.._actionsZ
+00008180: 6e74 6572 705a 085f 6163 7469 6f6e 735a  nterpZ._actionsZ
 00008190: 0b5f 7072 6564 6963 6174 6573 2903 da04  ._predicates)...
 000081a0: 7365 6c66 da05 696e 7075 7472 7201 0000  self..inputrr...
 000081b0: 2901 da09 5f5f 636c 6173 735f 5f72 0b00  )...__class__r..
 000081c0: 0000 720c 0000 0072 7401 0000 b403 0000  ..r....rt.......
 000081d0: 730a 0000 0000 010e 010a 0116 0106 017a  s..............z
 000081e0: 1276 6864 6c4c 6578 6572 2e5f 5f69 6e69  .vhdlLexer.__ini
 000081f0: 745f 5f29 b7da 085f 5f6e 616d 655f 5fda  t__)...__name__.
@@ -2139,15 +2139,15 @@
 000085a0: 4e61 6d65 73da 0c6c 6974 6572 616c 4e61  Names..literalNa
 000085b0: 6d65 73da 0d73 796d 626f 6c69 634e 616d  mes..symbolicNam
 000085c0: 6573 da09 7275 6c65 4e61 6d65 73da 0f67  es..ruleNames..g
 000085d0: 7261 6d6d 6172 4669 6c65 4e61 6d65 da03  rammarFileName..
 000085e0: 7379 73da 0673 7464 6f75 7472 0600 0000  sys..stdoutr....
 000085f0: 7274 0100 00da 0d5f 5f63 6c61 7373 6365  rt.....__classce
 00008600: 6c6c 5f5f 720b 0000 0072 0b00 0000 2901  ll__r....r....).
-00008610: 727e 0100 0072 0c00 0000 720e 0000 00c3  r~...r....r.....
+00008610: 727d 0100 0072 0c00 0000 720e 0000 00c3  r}...r....r.....
 00008620: 0200 0073 ce01 0000 0802 0e02 1402 0401  ...s............
 00008630: 0401 0401 0401 0401 0401 0401 0401 0401  ................
 00008640: 0401 0401 0401 0401 0401 0401 0401 0401  ................
 00008650: 0401 0401 0401 0401 0401 0401 0401 0401  ................
 00008660: 0401 0401 0401 0401 0401 0401 0401 0401  ................
 00008670: 0401 0401 0401 0401 0401 0401 0401 0401  ................
 00008680: 0401 0401 0401 0401 0401 0401 0401 0401  ................
@@ -2170,15 +2170,15 @@
 00008790: 1201 2001 1801 1801 1c01 1c01 1801 1801  .. .............
 000087a0: 1c01 0c01 0c01 1001 1801 1401 1c01 1801  ................
 000087b0: 1c01 1801 1402 0e01 0a01 0e01 0a01 0e01  ................
 000087c0: 0c01 0e01 0e01 1401 1c01 1401 1801 1801  ................
 000087d0: 1801 1801 1801 1c01 2401 2c01 2801 0c01  ........$.,.(...
 000087e0: 0c01 1401 1001 1001 1c01 1401 1c01 1801  ................
 000087f0: 1401 0802 0602 720e 0000 0029 0bda 0661  ......r....)...a
-00008800: 6e74 6c72 34da 0269 6f72 0300 0000 728a  ntlr4..ior....r.
+00008800: 6e74 6c72 34da 0269 6f72 0300 0000 7289  ntlr4..ior....r.
 00008810: 0100 00da 0c76 6572 7369 6f6e 5f69 6e66  .....version_inf
 00008820: 6fda 0674 7970 696e 6772 0600 0000 5a09  o..typingr....Z.
 00008830: 7479 7069 6e67 2e69 6f72 0d00 0000 da05  typing.ior......
 00008840: 4c65 7865 7272 0e00 0000 720b 0000 0072  Lexerr....r....r
 00008850: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
 00008860: 3c6d 6f64 756c 653e 0200 0000 7318 0000  <module>....s...
 00008870: 0008 010c 0108 010e 010e 020c 0408 7f00  ................
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a cbb7 c561 89bd 0c00 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 89bd 0c00 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 6000 0000 6400 6401 6c00 5400 6400  .s`...d.d.l.T.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6404 1900 6405 6b04 7238  Z.e.j.d...d.k.r8
 00000050: 6400 6406 6c05 6d06 5a06 0100 6e0c 6400  d.d.l.m.Z...n.d.
 00000060: 6406 6c07 6d06 5a06 0100 6407 6408 8400  d.l.m.Z...d.d...
 00000070: 5a08 4700 6409 640a 8400 640a 6509 8303  Z.G.d.d...d.e...
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a cbb7 c561 02c1 0000 e300 0000  3......a........
+00000000: 330d 0d0a 5e92 cd61 02c1 0000 e300 0000  3...^..a........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 4800 0000 6400 6401 6c00 5400 6501  .sH...d.d.l.T.e.
 00000030: 6402 6b09 7226 6403 6501 6b06 7226 6404  d.k.r&d.e.k.r&d.
 00000040: 6405 6c02 6d02 5a02 0100 6e0c 6400 6405  d.l.m.Z...n.d.d.
 00000050: 6c02 6d02 5a02 0100 4700 6406 6407 8400  l.m.Z...G.d.d...
 00000060: 6407 6503 8303 5a04 5b02 6402 5300 2908  d.e...Z.[.d.S.).
 00000070: e900 0000 0029 01da 012a 4eda 012e e901  .....)...*N.....
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/__pycache__/vhdlVisitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdl.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdl.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdl.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdl.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/generated/vhdl/vhdlVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/generated/vhdl/vhdlVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/SystemVerilogLexer.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/SystemVerilogLexer.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/SystemVerilogParser.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/SystemVerilogParser.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogLexer.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogLexer.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogParser.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogParser.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/VerilogPreprocessorParser.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/VerilogPreprocessorParser.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/grammars/vhdl.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/grammars/vhdl.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/hdl_representation.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/hdl_representation.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDL.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/SysVerilogHDLVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLLexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/SysVerilogHDL/__pycache__/SysVerilogHDLVisitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Lexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Listener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Listener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Parser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Parser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Visitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/Verilog2001Visitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/Verilog2001/__pycache__/Verilog2001Visitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlLexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-39.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlParserVisitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-38.pyc` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/__pycache__/vhdlVisitor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParser.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserListener.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserListener.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserVisitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_generated/vhdl/vhdlParserVisitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDL.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLParser.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/SysVerilogHDLParser.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Lexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Parser.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/Verilog2001Parser.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.interp` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.interp`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.java` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.java`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/.antlr/vhdlParser.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/SysVerilogHDL.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/SysVerilogHDL.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/Verilog2001.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/Verilog2001.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlLexer.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlLexer.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlLexer.tokens` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlLexer.tokens`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/old_grammars/vhdlParser.g4` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/old_grammars/vhdlParser.g4`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/sysverilog_entity_visitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/sysverilog_entity_visitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/verilog2001_entity_visitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/verilog2001_entity_visitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/antlr/vhdl_entity_visitor.py` & `dovado-rtl-0.9.9/src/dovado_rtl/antlr/vhdl_entity_visitor.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/cli_utility.py` & `dovado-rtl-0.9.9/src/dovado_rtl/cli_utility.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/config.py` & `dovado-rtl-0.9.9/src/dovado_rtl/config.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/doc_parsing.py` & `dovado-rtl-0.9.9/src/dovado_rtl/doc_parsing.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/fill_handler.py` & `dovado-rtl-0.9.9/src/dovado_rtl/fill_handler.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/fitness.py` & `dovado-rtl-0.9.9/src/dovado_rtl/fitness.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/frame_handling.py` & `dovado-rtl-0.9.9/src/dovado_rtl/frame_handling.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/genetic_algorithm.py` & `dovado-rtl-0.9.9/src/dovado_rtl/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/main.py` & `dovado-rtl-0.9.9/src/dovado_rtl/main.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/point_evaluation.py` & `dovado-rtl-0.9.9/src/dovado_rtl/point_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,36 +102,32 @@
                                     self.__stop_step.name + "_UTILISATION"
                                 )
                             )
                         ),
                         i.utilisation[0],
                         i.utilisation[1],
                     )
-                    if not i.is_frequency
+                    if i.utilisation
                     else -self.get_max_frequency(
                         report.get_wns(
                             str(self.__config.get_config("WORK_DIR"))
                             + (
                                 str(
                                     self.__config.get_config(
                                         self.__stop_step.name + "_TIMING"
                                     )
                                 )
                             )
                         )
                     )
-                    for i in self.__metrics
                     if not i.custom_metric
+                    else self.compute_custom_metric(i, design_point)
+                    for i in self.__metrics
                 },
             )
-            for i in self.__metrics:
-                if i.custom_metric:
-                    design_value.value[i] = self.compute_custom_metric(
-                        i, design_point
-                    )
         self.__write_csv(design_point, design_value)
         return design_value
 
     def get_max_frequency(self, wns: float) -> float:
 
         return 1000 / (1 / (1 / 1000 * self.__target_clock) - wns)
```

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/report_parsing.py` & `dovado-rtl-0.9.9/src/dovado_rtl/report_parsing.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/src_parsing.py` & `dovado-rtl-0.9.9/src/dovado_rtl/src_parsing.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/visualize.py` & `dovado-rtl-0.9.9/src/dovado_rtl/visualize.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/src/dovado_rtl/vivado_interaction.py` & `dovado-rtl-0.9.9/src/dovado_rtl/vivado_interaction.py`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/full_evalutate_point_frame.tcl` & `dovado-rtl-0.9.9/tcl/full_evalutate_point_frame.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/implementation.tcl` & `dovado-rtl-0.9.9/tcl/implementation.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/implementation_frame.tcl` & `dovado-rtl-0.9.9/tcl/implementation_frame.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/procs.tcl` & `dovado-rtl-0.9.9/tcl/procs.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/synthesis.tcl` & `dovado-rtl-0.9.9/tcl/synthesis.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/tcl/synthesis_frame.tcl` & `dovado-rtl-0.9.9/tcl/synthesis_frame.tcl`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/verilog/box.sv` & `dovado-rtl-0.9.9/verilog/box.sv`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/vhdl/box.vhd` & `dovado-rtl-0.9.9/vhdl/box.vhd`

 * *Files identical despite different names*

### Comparing `dovado-rtl-0.9.8/setup.py` & `dovado-rtl-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 entry_points = \
 {'console_scripts': ['dovado = dovado_rtl.main:main']}
 
 setup_kwargs = {
     'name': 'dovado-rtl',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'CLI tool for RTL Design Space Exploration on top of Vivado',
     'long_description': '\n# Table of Contents\n\n1.  [Installation](#org648fc4e)\n2.  [Usage](#org4d8ab18)\n    1.  [Defining Custom Metrics](#org023397d)\n    2.  [Examples](#orge369aa6)\n        1.  [neorv32 (VHDL)](#orgcb021dc)\n        2.  [corundum (VERILOG)](#org9b66d30)\n        3.  [cv32e40p (SYSTEM-VERILOG)](#orgbda061b)\n3. [Associated Publication](#paper_ref)\nDoVado is a RTL design automation and exploration CLI tool.\n\n\n<a id="org648fc4e"></a>\n\n# Installation\n\nDoVado needs python 3.6 or higher. Install it through pip, on many Linux systems use pip3 to force python 3 installation.\n\n    pip3 install --user --no-cache dovado-rtl\n\n\n<a id="org4d8ab18"></a>\n\n# Usage\n\nDovado has two modes:\n\n-   points: design automation mode in which a file containing parameter values must be given and a file containing all the evaluations is returned for some given metrics,\n-   space: design exploration mode in which parameters and their ranges must be given together with some target metrics and the pareto set of design points with respect to the given metrics is returned.\n\n<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">\n<caption class="t-above"><span class="table-number">Table 1:</span> dovado general parameters</caption>\n\n<colgroup>\n<col  class="org-left" />\n\n<col  class="org-left" />\n\n<col  class="org-left" />\n</colgroup>\n<thead>\n<tr>\n<th scope="col" class="org-left">parameter</th>\n<th scope="col" class="org-left">description</th>\n<th scope="col" class="org-left">mandatory</th>\n</tr>\n</thead>\n\n<tbody>\n<tr>\n<td class="org-left">&#x2013;file-path</td>\n<td class="org-left">path to the target file</td>\n<td class="org-left">yes</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;board</td>\n<td class="org-left">vivado descriptor of a board</td>\n<td class="org-left">yes</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;parameters</td>\n<td class="org-left">parameters to use either for points/space (integers and booleans supported)</td>\n<td class="org-left">yes</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;clock-port</td>\n<td class="org-left">RTL identifier of the clock port</td>\n<td class="org-left">yes</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;implementation</td>\n<td class="org-left">switch to evaluate designs after implementation (default is after synthesis)</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;incremental</td>\n<td class="org-left">switch to use incremental synthesis/implementation</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;directives</td>\n<td class="org-left">list of directives to pass to synthesis, place and route (default is RuntimeOptimized for all three)</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;target-clock</td>\n<td class="org-left">clock (Mhz) to give as a constraint to Vivado (default=1000)</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;metrics</td>\n<td class="org-left">list of metrics to target using their integer identifier (default mode is interactive, you will be asked after first synthesis/implementation)</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#xa0;</td>\n<td class="org-left">&#xa0;</td>\n<td class="org-left">&#xa0;</td>\n</tr>\n</tbody>\n</table>\n\nAfter those parameters specify points/space both these modes take an argument:\n\n-   points argument: specify the path to the csv file containing the design points to be analyzed. The csv file must contain on each line the value for each of the parameters stated through &#x2013;parameters in the same order,\n-   space argument: a list of ranges stated as 1 2 3 4 where this way we would be defining two ranges (1, 2) for the first parameter and (3, 4) for the second parameter\n\nNo further parameters can be passed to points\n\n<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">\n\n\n<colgroup>\n<col  class="org-left" />\n\n<col  class="org-left" />\n\n<col  class="org-left" />\n</colgroup>\n<thead>\n<tr>\n<th scope="col" class="org-left">parameter</th>\n<th scope="col" class="org-left">description</th>\n<th scope="col" class="org-left">mandatory</th>\n</tr>\n</thead>\n\n<tbody>\n<tr>\n<td class="org-left">&#x2013;power-of-2</td>\n<td class="org-left">list of &rsquo;y/n&rsquo; to state whether a parameter must be explored stepping power of 2s</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;param-initial-values</td>\n<td class="org-left">parameter values which are guaranteed to be synthesizable to retrieve metric mapping</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;optimization-runtime</td>\n<td class="org-left">set as a termination condition a timeout as hh:mm:ss</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;read-design-values</td>\n<td class="org-left">read design values from a csv</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;disable-approximate</td>\n<td class="org-left">disable approximation</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;estimation-model</td>\n<td class="org-left">choose Hoeffding Adaptive Tree (default) or Kernel Ridge regressor or Shadow to not use the controller but log anyways</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;controller-model</td>\n<td class="org-left">choose Mab or Distance-based (default) controller</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;disable-controller-mab-weight</td>\n<td class="org-left">disable loss weighting in distance controller</td>\n<td class="org-left">no</td>\n</tr>\n\n\n<tr>\n<td class="org-left">&#x2013;n-controllers</td>\n<td class="org-left">set the number of voting controllers (default is 500, too high for many applications)</td>\n<td class="org-left">no</td>\n</tr>\n</tbody>\n</table>\n\nDirectory structure is vital for the functioning of the tool:\n\n-   VHDL: if a package is used the corresponding folder must be named exactly as the package; if one wants to analyse a module in a project with multiple packages each file belonging to a given package must reside in a subfolder with the same name as the package it belongs to:\n    -   package-name (top folder must have the name of the top package if it exists or any name if it does not exist)\n        -   file-1 (belonging to package-name)\n        -   file-2 (belonging to package-name)\n        -   subpackage1-name\n            -   file-1 (belonging to subpackage-name)\n            -   file-2 (belonging to subpackage-name)\n            -   &#x2026;\n        -   subpackage2-name\n            -   &#x2026;\n        -   &#x2026;\n-   VERILOG/SYSTEM-VERILOG: include directives are not supported all files must be in the same folder, no subfolders allowed;  no import package allowed.\n\nIn order to inspect the tool\'s work you have several files at hand:\n-  `dovado_work/point_evaluation.csv` which has one design evaluation per line, mapped with the points you give dovado; written online during tool\'s execution in points mode\n- `dovado_work/space_exploration.csv` which has all the design points explored together with the design values; written online during tool\'s execution both in points mode and in space mode\n- `dovado_work/design_space.csv` and `dovado_work/objective_space.csv` are written at the end of the design exploration process (space mode) and contain respectively the pareto set of design parameters and the corresponding evaluations\n\n<a id="org023397d"></a>\n\n## Defining Custom Metrics\n\nProcedure:\n\n1.  Create a folder named `custom_metrics` in the same folder where you are running dovado\n    \n        mkdir custom_metrics\n2.  Create the **python** file which will contain your custom metric\n    \n        touch test_metric.py\n3.  Write your metric function, any function you need to carry out the computation and any import for the libraries\n    \n        # here any import works\n        # e.g. import numpy as np\n        import numpy as np\n        \n        \n        def test_metric(**kwargs) -> float:\n            # only one metric per file is admitted\n            # if you want another custom metric create a new file\n            print(kwargs)\n            return float(__helper_function(kwargs["frequency"]))\n        \n        \n        def __helper_function(a):\n            # Care the underscores \'__\' are mandatory for helper functions\n            # This function won\'t show as a metric is here only for helping purposes\n            return a + 1000\n4.  Run dovado without metric selected:\n    \n        dovado --file-path <path to "neorv32/rtl/neorv32/neorv32_top.vhd"> --board xc7k70tfbv676-1 --parameters MEM_INT_IMEM_SIZE --parameters MEM_INT_DMEM_SIZE --clock-port clk_i space 16384 131072 8129 65536 --power-of-2 y --power-of-2 y\n5.  Select your metrics, you will now find your custom metrics after all utilisation metrics provided by your board of choice:\n    ![img](./readme_resources/metrics_selection.png)\n\nGeneral advice:\n\n-   the function must return float (**highly recommended** to annotate the return type)\n-   all helper functions must start with double underscore &ldquo;\\_\\_&rdquo;\n-   relative imports are not supported, use only absolute imports\n-   all subfolders of `custom_metrics` are ignored.\n-   from the \\*\\*kwargs you can access all the other board metrics, the frequency and all the parameters you are using for explorationo by using either &ldquo;frequency&rdquo;,  the name you find above or the parameter name in dovado\'s call e.g:\n    \n        kwargs["frequency"]\n        kwargs["Slice LUTs*"]\n        kwargs["MEM_INT_IMEM_SIZE"]\n\n\n<a id="orge369aa6"></a>\n\n## Examples\n\n\n<a id="orgcb021dc"></a>\n\n### neorv32 (VHDL)\n\n    git clone https://github.com/stnolting/neorv32\n    cd neorv32/rtl\n    mv core neorv32\n\nChanging the name of the core folder, which contains all vhdl files, to the name of the package which is used along the files is mandatory to make dovado get &rsquo;use&rsquo; directives right.\nExploring the parameter space of the top module:\n\n    dovado --file-path <path to "neorv32/rtl/neorv32/neorv32_top.vhd"> --board xc7k70tfbv676-1 --parameters MEM_INT_IMEM_SIZE --parameters MEM_INT_DMEM_SIZE --clock-port clk_i --metrics 0 --metrics 1 --metrics 4 --metrics 9 space 16384 131072 8129 65536 --power-of-2 y --power-of-2 y\n\nAbove we are optimizing two memory parameters (MEM<sub>INT</sub><sub>IMEM</sub><sub>SIZE</sub>, MEM<sub>INT</sub><sub>DMEM</sub><sub>SIZE</sub>) with clk<sub>i</sub> as the clock port with metrics chosen:\n\n-   frequency (0)\n-   LUT occupation (1)\n-   REGISTER occupation (4)\n-   BRAM occupation (9)\n\nRanges are specified after space and we also specify that we want to search only among power of 2&rsquo;s solutions.\n\nHere an example of **exploring boolean parameters**, the trick here is to explore them as normal parameters but use as range [0, 1] obviously they can be mixed up with non-boolean parameters during exploration:\n\n    dovado --file-path <path to "neorv32/rtl/neorv32/neorv32_top.vhd"> --board xc7k70tfbv676-1 --parameters BOOTLOADER_EN --parameters CPU_EXTENSION_RISCV_A --parameters CPU_EXTENSION_RISCV_B --parameters CPU_EXTENSION_RISCV_C --clock-port clk_i --metrics 0 --metrics 1 --metrics 4 --metrics 9 space 0 1 0 1 0 1 0 1 --disable-approximate\n\n\n<a id="org9b66d30"></a>\n\n### corundum (VERILOG)\n\n    git clone https://github.com/corundum/corundum\n    cd corundum/\n\nExploring the parameter space of the top module:\n\n    dovado --file-path <path to "corundum/fpga/common/rtl/cpl_queue_manager.v"> --board xc7k70tfbv676-1 --target-clock 100000 --parameters OP_TABLE_SIZE --parameters QUEUE_INDEX_WIDTH --parameters PIPELINE --clock-port clk --metrics 0 --metrics 1 --metrics 4 --metrics 9 space 8 64 4 11 2 32 --disable-approximate\n\nUsing **approximation** parameters:\n\n    dovado --file-path <path to "corundum/fpga/common/rtl/cpl_queue_manager.v"> --board xc7k70tfbv676-1 --target-clock 100000 --parameters OP_TABLE_SIZE --parameters QUEUE_INDEX_WIDTH --parameters PIPELINE --clock-port clk --metrics 0 --metrics 1 --metrics 4 --metrics 9 space 8 64 4 11 2 32\n\n\n<a id="orgbda061b"></a>\n\n### cv32e40p (SYSTEM-VERILOG)\n\n    git clone https://github.com/openhwgroup/cv32e40p\n    cd rtl\n    mkdir testing\n    cp cv32e40p_fifo.sv testing/\n\nIn this project an include directory is used but dovado does not currently support it thus we create a subfolder, name may be whatever, where to isolate the module we are interested in studying. This workaround is only possible if the module one wants to study works standalone without include directives.\n\n    dovado --file-path <path to "cv32e40p/rtl/testing/cv32e40p_fifo.sv"> --board xc7k70tfbv676-1 --target-clock 100000 --parameters DEPTH --parameters DATA_WIDTH --clock-port clk_i --metrics 0 --metrics 1 --metrics 4 --metrics 9 space 2 4096 2 64 --power-of-2 y --power-of-2 y --disable-approximate\n\n<a id="paper_ref"></a>\n# Associated Publication\n\nIf you find this repository useful, please use the following citation:\n\n```\n@inproceedings{paletti2021dovado,\n  title={Dovado: An Open-Source Design Space Exploration Framework},\n  author={Paletti, Daniele and Conficconi, Davide and Santambrogio, Marco D},\n  booktitle={2021 IEEE International Parallel and Distributed Processing Symposium Workshops (IPDPSW)},\n  pages={128--135},\n  year={2021},\n  organization={IEEE}\n}\n```\n',
     'author': 'Daniele Paletti',
     'author_email': 'danielepaletti98@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DPaletti/dovado',
```

### Comparing `dovado-rtl-0.9.8/PKG-INFO` & `dovado-rtl-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dovado-rtl
-Version: 0.9.8
+Version: 0.9.9
 Summary: CLI tool for RTL Design Space Exploration on top of Vivado
 Home-page: https://github.com/DPaletti/dovado
 License: MIT
 Keywords: Xilinx,Vivado,TCL,VHDL,Verilog,RTL,Design Space,Genetic Algorithm
 Author: Daniele Paletti
 Author-email: danielepaletti98@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dovado-rtl Version: 0.9.8 Summary: CLI tool for RTL
+Metadata-Version: 2.1 Name: dovado-rtl Version: 0.9.9 Summary: CLI tool for RTL
 Design Space Exploration on top of Vivado Home-page: https://github.com/
 DPaletti/dovado License: MIT Keywords:
 Xilinx,Vivado,TCL,VHDL,Verilog,RTL,Design Space,Genetic Algorithm Author:
 Daniele Paletti Author-email: danielepaletti98@gmail.com Requires-Python:
 >=3.6.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

