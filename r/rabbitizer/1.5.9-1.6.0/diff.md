# Comparing `tmp/rabbitizer-1.5.9.tar.gz` & `tmp/rabbitizer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.5.9.tar", last modified: Thu Feb 23 01:09:26 2023, max compression
+gzip compressed data, was "rabbitizer-1.6.0.tar", last modified: Mon Apr 17 20:19:35 2023, max compression
```

## Comparing `rabbitizer-1.5.9.tar` & `rabbitizer-1.6.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.546644 rabbitizer-1.5.9/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.550644 rabbitizer-1.5.9/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.550644 rabbitizer-1.5.9/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/Abi_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.550644 rabbitizer-1.5.9/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/AccessType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrCategory_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrId_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrSuffix_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/OperandType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/OperandType_function_declarations.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/Registers_enums.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/Registers_enums.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.550644 rabbitizer-1.5.9/include/instructions/instr_id/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.554644 rabbitizer-1.5.9/include/instructions/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.554644 rabbitizer-1.5.9/include/instructions/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.554644 rabbitizer-1.5.9/include/instructions/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.558644 rabbitizer-1.5.9/include/instructions/operands/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.558644 rabbitizer-1.5.9/include/instructions/registers/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspVector.inc
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-02-23 01:09:26.000000 rabbitizer-1.5.9/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-02-23 01:09:26.000000 rabbitizer-1.5.9/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 01:09:26.000000 rabbitizer-1.5.9/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 01:09:26.000000 rabbitizer-1.5.9/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.546644 rabbitizer-1.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.562644 rabbitizer-1.5.9/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrCategory_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)   108302 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrDescriptor_Descriptors_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    30567 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrId_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:09:26.566644 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RabbitizerRegisterDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/Registers_Names_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-23 01:09:18.000000 rabbitizer-1.5.9/src/instructions/Registers_Names_arrays.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.798258 rabbitizer-1.6.0/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.806258 rabbitizer-1.6.0/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrId_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/Registers_enums.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/Registers_enums.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.806258 rabbitizer-1.6.0/include/instructions/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.810258 rabbitizer-1.6.0/include/instructions/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.814258 rabbitizer-1.6.0/include/instructions/operands/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.822258 rabbitizer-1.6.0/include/instructions/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspVector.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.830258 rabbitizer-1.6.0/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.830258 rabbitizer-1.6.0/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 20:19:35.000000 rabbitizer-1.6.0/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.794258 rabbitizer-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.834258 rabbitizer-1.6.0/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrCategory_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)   108158 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.838258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:35.842258 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RabbitizerRegisterDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-17 20:19:21.000000 rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.template
```

### Comparing `rabbitizer-1.5.9/LICENSE` & `rabbitizer-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/PKG-INFO` & `rabbitizer-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.5.9
+Version: 1.6.0
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.5.9/README.md` & `rabbitizer-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.6.0/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.6.0/include/analysis/RabbitizerRegistersTracker.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.6.0/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/common/RabbitizerConfig.h` & `rabbitizer-1.6.0/include/common/RabbitizerConfig.h`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,19 @@
      * Removing the $0 fixes this issue (but not for handwritten asm)
      *
      * - SN64's assembler expands div to have break if dividing by zero
      * However, the break it generates is different than the one it generates with `break N`
      * So we replace break instrutions for SN64 with the exact word that the assembler generates when expanding div
      */
     bool sn64DivFix;
+    /**
+     * Enables various tweaks to allow building matching with GNU as which
+     * break original compiler behavior and what's specified in the manuals.
+     */
+    bool gnuMode;
 } RabbitizerConfig_ToolchainTweaks;
 
 typedef struct RabbitizerConfig_Misc {
     int opcodeLJust; // The minimal number of characters to left-align the opcode name
     bool unknownInstrComment; // Generate a pseudo-disassembly comment when disassembling non implemented instructions
     bool omit0XOnSmallImm;
     bool upperCaseImm;
```

### Comparing `rabbitizer-1.5.9/include/common/RabbitizerVersion.h` & `rabbitizer-1.6.0/include/common/RabbitizerVersion.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_VERSION_H
 #define RABBITIZER_VERSION_H
 
 #include "Utils.h"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
-#define RAB_VERSION_MINOR 5
-#define RAB_VERSION_PATCH 9
+#define RAB_VERSION_MINOR 6
+#define RAB_VERSION_PATCH 0
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 // Compiled library version
 extern const int RabVersion_Major;
 extern const int RabVersion_Minor;
 extern const int RabVersion_Patch;
```

### Comparing `rabbitizer-1.5.9/include/common/Utils.h` & `rabbitizer-1.6.0/include/common/Utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 #else
 #  define UNREACHABLE
 #endif
 
 
 #define ARRAY_COUNT(arr) (sizeof(arr) / sizeof((arr)[0]))
 
-#define RAB_STRINGIFY(x) #x
+#define RAB_STRINGIFY2(x) #x
+#define RAB_STRINGIFY(x) RAB_STRINGIFY2(x)
 
 #define MASK(v, w) ((v) & ((1 << (w)) - 1))
 
 /*
  * the SHIFT macros take a value, a shift amount, and a width.
  *
  * For the left shift, the lower bits of the value are masked,
```

### Comparing `rabbitizer-1.5.9/include/instructions/InstrId_enum.table.h` & `rabbitizer-1.6.0/include/instructions/InstrId_enum.table.h`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
 RABBITIZER_INSTR_ID_r5900_mula_s,
 RABBITIZER_INSTR_ID_r5900_madd_s,
 RABBITIZER_INSTR_ID_r5900_msub_s,
 RABBITIZER_INSTR_ID_r5900_madda_s,
 RABBITIZER_INSTR_ID_r5900_msuba_s,
 RABBITIZER_INSTR_ID_r5900_max_s,
 RABBITIZER_INSTR_ID_r5900_min_s,
-RABBITIZER_INSTR_ID_r5900_trunc_w_s,
 RABBITIZER_INSTR_ID_r5900_c_lt_s,
 RABBITIZER_INSTR_ID_r5900_c_le_s,
 RABBITIZER_INSTR_ID_r5900_qmfc2,
 RABBITIZER_INSTR_ID_r5900_cfc2,
 RABBITIZER_INSTR_ID_r5900_qmtc2,
 RABBITIZER_INSTR_ID_r5900_ctc2,
 RABBITIZER_INSTR_ID_r5900_bc2f,
```

### Comparing `rabbitizer-1.5.9/include/instructions/InstrId_enum.table.template` & `rabbitizer-1.6.0/include/instructions/InstrId_enum.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/OperandType_enum.table.h` & `rabbitizer-1.6.0/include/instructions/OperandType_enum.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/OperandType_function_declarations.table.h` & `rabbitizer-1.6.0/include/instructions/OperandType_function_declarations.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstrId.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstrSuffix.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstruction.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstructionR5900.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerInstructionRsp.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerOperandType.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerRegister.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.6.0/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/Registers_enums.table.h` & `rabbitizer-1.6.0/include/instructions/Registers_enums.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/Registers_enums.table.template` & `rabbitizer-1.6.0/include/instructions/Registers_enums.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/cpu/cpu_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc`

 * *Files 16% similar despite different names*

```diff
@@ -99,27 +99,14 @@
     .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
     .isFloat=true,
     .modifiesFd=true,
     .readsFs=true,
     .readsFt=true
 ) // floating point MINimum
 
-// Due to the R5900's FPU being non properly complaint the instruction cvt.w.s always behaves as trunc.w.s because is because EE can only do round-to-zero.
-// Assemblers like GAS workaround this issue by decoding cvt.w.s as trunc.w.s, so we mimic that behaviour to allow assembling with GAS.
-// Here's some reading about the binutils rationale:
-// https://sourceware.org/legacy-ml/binutils/2012-11/msg00360.html
-// https://sourceware.org/pipermail/binutils/2013-January/079863.html
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x24, trunc_w_s, trunc.w.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Truncate to Word Fixed-Point
-
 RABBITIZER_DEF_INSTR_ID_ALTNAME(
     r5900, 0x34, c_lt_s, c.lt.s,
     .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
     .isFloat=true,
     .readsFs=true,
     .readsFt=true
 )
```

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_cop2_special2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_mmi_3.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_mmi_3.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/r5900/r5900_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_normal_swc2.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.6.0/include/instructions/instr_id/rsp/rsp_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_r5900.inc` & `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.6.0/include/instructions/operands/RabbitizerOperandType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_Cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprN32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_GprO32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/instructions/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.6.0/include/instructions/registers/RabbitizerRegister_RspVector.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/include/rabbitizer.h` & `rabbitizer-1.6.0/include/rabbitizer.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/pyproject.toml` & `rabbitizer-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.5.9"
+version = "1.6.0"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.5.9/rabbitizer/Config.pyi` & `rabbitizer-1.6.0/rabbitizer/Config.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     pseudos_pseudoBnez: bool = True
     pseudos_pseudoB: bool = True
     pseudos_pseudoMove: bool = True
     pseudos_pseudoNot: bool = True
     pseudos_pseudoNegu: bool = True
     pseudos_pseudoBal: bool = True
 
-    toolchainTweaks_sn64DivFix: bool = False
     toolchainTweaks_treatJAsUnconditionalBranch: bool = False
+    toolchainTweaks_sn64DivFix: bool = False
+    toolchainTweaks_gnuMode: bool = True
 
     misc_opcodeLJust: int = 11
     misc_unknownInstrComment: bool = True
     misc_omit0XOnSmallImm: bool = False
     misc_upperCaseImm: bool = True
 
 config: _RabbitizerConfig
```

### Comparing `rabbitizer-1.5.9/rabbitizer/Enum.pyi` & `rabbitizer-1.6.0/rabbitizer/Enum.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/InstrId.pyi` & `rabbitizer-1.6.0/rabbitizer/InstrId.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/OperandType.pyi` & `rabbitizer-1.6.0/rabbitizer/OperandType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.6.0/rabbitizer/RegGprN32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.6.0/rabbitizer/RegGprO32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.6.0/rabbitizer/RegistersTracker.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.6.0/rabbitizer/enums/enums_utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.6.0/rabbitizer/enums/enums_utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_InstrId.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_enum_OperandType.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_enum_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.6.0/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.6.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer.pyi` & `rabbitizer-1.6.0/rabbitizer/rabbitizer.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_global_config.c`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 DEF_MEMBER_GET_SET_BOOL(pseudos, pseudoMove)
 DEF_MEMBER_GET_SET_BOOL(pseudos, pseudoNot)
 DEF_MEMBER_GET_SET_BOOL(pseudos, pseudoNegu)
 DEF_MEMBER_GET_SET_BOOL(pseudos, pseudoBal)
 
 DEF_MEMBER_GET_SET_BOOL(toolchainTweaks, treatJAsUnconditionalBranch)
 DEF_MEMBER_GET_SET_BOOL(toolchainTweaks, sn64DivFix)
+DEF_MEMBER_GET_SET_BOOL(toolchainTweaks, gnuMode)
 
 DEF_MEMBER_GET_SET_INT(misc, opcodeLJust, false, 0, 0)
 DEF_MEMBER_GET_SET_BOOL(misc, unknownInstrComment)
 DEF_MEMBER_GET_SET_BOOL(misc, omit0XOnSmallImm)
 DEF_MEMBER_GET_SET_BOOL(misc, upperCaseImm)
 
 
@@ -140,14 +141,15 @@
     MEMBER_GET_SET(pseudos, pseudoMove, "", NULL),
     MEMBER_GET_SET(pseudos, pseudoNot, "", NULL),
     MEMBER_GET_SET(pseudos, pseudoNegu, "", NULL),
     MEMBER_GET_SET(pseudos, pseudoBal, "", NULL),
 
     MEMBER_GET_SET(toolchainTweaks, treatJAsUnconditionalBranch, "", NULL),
     MEMBER_GET_SET(toolchainTweaks, sn64DivFix, "", NULL),
+    MEMBER_GET_SET(toolchainTweaks, gnuMode, "", NULL),
 
     MEMBER_GET_SET(misc, opcodeLJust, "", NULL),
     MEMBER_GET_SET(misc, unknownInstrComment, "", NULL),
     MEMBER_GET_SET(misc, omit0XOnSmallImm, "", NULL),
     MEMBER_GET_SET(misc, upperCaseImm, "", NULL),
 
     { 0 },
```

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_module.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_module.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.6.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.6.0/rabbitizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.5.9
+Version: 1.6.0
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.5.9/rabbitizer.egg-info/SOURCES.txt` & `rabbitizer-1.6.0/rabbitizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/setup.py` & `rabbitizer-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.6.0/src/analysis/RabbitizerRegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.6.0/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/common/RabbitizerConfig.c` & `rabbitizer-1.6.0/src/common/RabbitizerConfig.c`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         .pseudoNot = true,
         .pseudoNegu = true,
         .pseudoBal = true,
     },
     .toolchainTweaks = {
         .treatJAsUnconditionalBranch = true,
         .sn64DivFix = false,
+        .gnuMode = true,
     },
     .misc = {
         .opcodeLJust = 7+4,
         .unknownInstrComment = true,
         .omit0XOnSmallImm = false,
         .upperCaseImm = true,
     }
```

### Comparing `rabbitizer-1.5.9/src/common/Utils.c` & `rabbitizer-1.6.0/src/common/Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/InstrDescriptor_Descriptors_array.table.h` & `rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.h`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
 [RABBITIZER_INSTR_ID_r5900_mula_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_madd_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_msub_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_madda_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_msuba_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_max_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_min_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_trunc_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .isFloat=true, .modifiesFd=true, .readsFs=true },
 [RABBITIZER_INSTR_ID_r5900_c_lt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_c_le_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
 [RABBITIZER_INSTR_ID_r5900_qmfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .modifiesRt=true },
 [RABBITIZER_INSTR_ID_r5900_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .modifiesRt=true },
 [RABBITIZER_INSTR_ID_r5900_qmtc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .readsRt=true },
 [RABBITIZER_INSTR_ID_r5900_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .readsRt=true },
 [RABBITIZER_INSTR_ID_r5900_bc2f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true },
```

### Comparing `rabbitizer-1.5.9/src/instructions/InstrDescriptor_Descriptors_array.table.template` & `rabbitizer-1.6.0/src/instructions/InstrDescriptor_Descriptors_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/InstrId_Names_array.table.h` & `rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.h`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
 [RABBITIZER_INSTR_ID_r5900_mula_s] = "mula.s",
 [RABBITIZER_INSTR_ID_r5900_madd_s] = "madd.s",
 [RABBITIZER_INSTR_ID_r5900_msub_s] = "msub.s",
 [RABBITIZER_INSTR_ID_r5900_madda_s] = "madda.s",
 [RABBITIZER_INSTR_ID_r5900_msuba_s] = "msuba.s",
 [RABBITIZER_INSTR_ID_r5900_max_s] = "max.s",
 [RABBITIZER_INSTR_ID_r5900_min_s] = "min.s",
-[RABBITIZER_INSTR_ID_r5900_trunc_w_s] = "trunc.w.s",
 [RABBITIZER_INSTR_ID_r5900_c_lt_s] = "c.lt.s",
 [RABBITIZER_INSTR_ID_r5900_c_le_s] = "c.le.s",
 [RABBITIZER_INSTR_ID_r5900_qmfc2] = "qmfc2",
 [RABBITIZER_INSTR_ID_r5900_cfc2] = "cfc2",
 [RABBITIZER_INSTR_ID_r5900_qmtc2] = "qmtc2",
 [RABBITIZER_INSTR_ID_r5900_ctc2] = "ctc2",
 [RABBITIZER_INSTR_ID_r5900_bc2f] = "bc2f",
```

### Comparing `rabbitizer-1.5.9/src/instructions/InstrId_Names_array.table.template` & `rabbitizer-1.6.0/src/instructions/InstrId_Names_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstrSuffix.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files 17% similar despite different names*

```diff
@@ -91,14 +91,46 @@
 bool RabbitizerInstruction_mustDisasmAsData(const RabbitizerInstruction *self) {
     if (RabbitizerConfig_Cfg.toolchainTweaks.sn64DivFix) {
         if (self->uniqueId == RABBITIZER_INSTR_ID_cpu_break) {
             return true;
         }
     }
 
+    if (RabbitizerConfig_Cfg.toolchainTweaks.gnuMode) {
+        switch (self->uniqueId) {
+            case RABBITIZER_INSTR_ID_cpu_trunc_w_s:
+            case RABBITIZER_INSTR_ID_cpu_cvt_w_s:
+                if (self->category == RABBITIZER_INSTRCAT_R5900) {
+                    /**
+                     * Due to the R5900's FPU being non properly complaint, the instruction cvt.w.s always behaves as
+                     * trunc.w.s because EE can only do round-to-zero.
+                     *
+                     * Assemblers like GAS workaround this issue by decoding cvt.w.s as trunc.w.s, but other assemblers
+                     * just use trunc.w.s and cvt.w.s as-is.
+                     *
+                     * Here's some reading about the binutils rationale:
+                     * - https://sourceware.org/legacy-ml/binutils/2012-11/msg00360.html
+                     * - https://sourceware.org/pipermail/binutils/2013-January/079863.html
+                     *
+                     * Because of this, building with GAS with the -march=r5900 flag produces:
+                     * - trunc.w.s is built as the cvt.w.s instruction.
+                     * - cvt.w.s errors complaining as not being supported by the processor.
+                     *
+                     * To ensure the produced disassembly will still match when built with GAS, we decode this two
+                     * instructions as .word
+                     */
+                    return true;
+                }
+                break;
+
+            default:
+                break;
+        }
+    }
+
     if (!RabbitizerInstruction_isValid(self)) {
         return true;
     }
     return false;
 }
 
 size_t RabbitizerInstruction_getSizeForBuffer(const RabbitizerInstruction *self, size_t immOverrideLength,
```

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files 4% similar despite different names*

```diff
@@ -97,21 +97,23 @@
         }
     }
 
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 
     switch (self->uniqueId) {
         case RABBITIZER_INSTR_ID_cpu_div:
-            if (RabbitizerConfig_Cfg.toolchainTweaks.sn64DivFix && !self->inHandwrittenFunction) {
+            if ((!RabbitizerConfig_Cfg.toolchainTweaks.gnuMode) ||
+                (RabbitizerConfig_Cfg.toolchainTweaks.sn64DivFix && !self->inHandwrittenFunction)) {
                 self->descriptor = &RabbitizerInstrDescriptor_Descriptors[RABBITIZER_INSTR_ID_cpu_sn64_div];
             }
             break;
 
         case RABBITIZER_INSTR_ID_cpu_divu:
-            if (RabbitizerConfig_Cfg.toolchainTweaks.sn64DivFix && !self->inHandwrittenFunction) {
+            if ((!RabbitizerConfig_Cfg.toolchainTweaks.gnuMode) ||
+                (RabbitizerConfig_Cfg.toolchainTweaks.sn64DivFix && !self->inHandwrittenFunction)) {
                 self->descriptor = &RabbitizerInstrDescriptor_Descriptors[RABBITIZER_INSTR_ID_cpu_sn64_divu];
             }
             break;
 
         default:
             break;
     }
```

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files 0% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 #include "common/RabbitizerConfig.h"
 #include "instructions/RabbitizerRegister.h"
 
 size_t RabbitizerOperandType_process_r5900_I(UNUSED const RabbitizerInstruction *self, char *dst,
                                              UNUSED const char *immOverride, UNUSED size_t immOverrideLength) {
     size_t totalSize = 0;
 
-    RABUTILS_BUFFER_CPY(dst, totalSize, "$I");
+    RABUTILS_BUFFER_CPY(dst, totalSize, "I");
 
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_r5900_Q(UNUSED const RabbitizerInstruction *self, char *dst,
                                              UNUSED const char *immOverride, UNUSED size_t immOverrideLength) {
     size_t totalSize = 0;
 
-    RABUTILS_BUFFER_CPY(dst, totalSize, "$Q");
+    RABUTILS_BUFFER_CPY(dst, totalSize, "Q");
 
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_r5900_R(UNUSED const RabbitizerInstruction *self, char *dst,
                                              UNUSED const char *immOverride, UNUSED size_t immOverrideLength) {
     size_t totalSize = 0;
 
-    RABUTILS_BUFFER_CPY(dst, totalSize, "$R");
+    RABUTILS_BUFFER_CPY(dst, totalSize, "R");
 
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_r5900_ACC(UNUSED const RabbitizerInstruction *self, char *dst,
                                                UNUSED const char *immOverride, UNUSED size_t immOverrideLength) {
     size_t totalSize = 0;
 
-    RABUTILS_BUFFER_CPY(dst, totalSize, "$ACC");
+    RABUTILS_BUFFER_CPY(dst, totalSize, "ACC");
 
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_r5900_ACCxyzw(const RabbitizerInstruction *self, char *dst,
                                                    const char *immOverride, size_t immOverrideLength) {
     size_t totalSize = 0;
```

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 /* SPDX-FileCopyrightText: © 2022 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionR5900.h"
+#include "common/RabbitizerConfig.h"
 
 #define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...)    \
     case (caseBits):                                            \
         self->uniqueId = RABBITIZER_INSTR_ID_##prefix##_##name; \
         break;
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
```

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerRegister.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.6.0/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h` & `rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.6.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/Registers_Names_arrays.table.h` & `rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.5.9/src/instructions/Registers_Names_arrays.table.template` & `rabbitizer-1.6.0/src/instructions/Registers_Names_arrays.table.template`

 * *Files identical despite different names*

