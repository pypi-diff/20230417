# Comparing `tmp/fpop-0.0.5.tar.gz` & `tmp/fpop-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpop-0.0.5.tar", last modified: Wed Mar 15 08:11:11 2023, max compression
+gzip compressed data, was "fpop-0.0.6.tar", last modified: Mon Apr 17 13:05:04 2023, max compression
```

## Comparing `fpop-0.0.5.tar` & `fpop-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 4294967294 4294967294        0 2023-03-15 08:11:11.980011 fpop-0.0.5/
--rw-r--r--   0 4294967294 4294967294     7650 2023-03-15 06:12:17.000000 fpop-0.0.5/LICENSE
--rw-r--r--   0 4294967294 4294967294       16 2023-03-15 06:12:17.000000 fpop-0.0.5/MANIFEST.in
--rw-r--r--   0 4294967294 4294967294      895 2023-03-15 08:11:11.976319 fpop-0.0.5/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      403 2023-03-15 06:12:17.000000 fpop-0.0.5/README.md
-drwxr-xr-x   0 4294967294 4294967294        0 2023-03-15 08:11:11.740308 fpop-0.0.5/fpop/
--rw-r--r--   0 4294967294 4294967294       24 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/__about__.py
--rw-r--r--   0 4294967294 4294967294        0 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/__init__.py
--rw-r--r--   0 4294967294 4294967294     6271 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/prep_fp.py
--rw-r--r--   0 4294967294 4294967294     6496 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/preprun_fp.py
--rw-r--r--   0 4294967294 4294967294     6353 2023-03-15 06:13:05.000000 fpop-0.0.5/fpop/run_fp.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-03-15 08:11:11.817479 fpop-0.0.5/fpop/utils/
--rw-r--r--   0 4294967294 4294967294        0 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/utils/__init__.py
--rw-r--r--   0 4294967294 4294967294      400 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/utils/step_config.py
--rw-r--r--   0 4294967294 4294967294     8925 2023-03-15 06:12:17.000000 fpop-0.0.5/fpop/vasp.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-03-15 08:11:11.797818 fpop-0.0.5/fpop.egg-info/
--rw-r--r--   0 4294967294 4294967294      895 2023-03-15 08:11:11.000000 fpop-0.0.5/fpop.egg-info/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      499 2023-03-15 08:11:11.000000 fpop-0.0.5/fpop.egg-info/SOURCES.txt
--rw-r--r--   0 4294967294 4294967294        1 2023-03-15 08:11:11.000000 fpop-0.0.5/fpop.egg-info/dependency_links.txt
--rw-r--r--   0 4294967294 4294967294       31 2023-03-15 08:11:11.000000 fpop-0.0.5/fpop.egg-info/requires.txt
--rw-r--r--   0 4294967294 4294967294       11 2023-03-15 08:11:11.000000 fpop-0.0.5/fpop.egg-info/top_level.txt
--rw-r--r--   0 4294967294 4294967294       38 2023-03-15 08:11:11.982060 fpop-0.0.5/setup.cfg
--rw-r--r--   0 4294967294 4294967294      847 2023-03-15 08:11:01.000000 fpop-0.0.5/setup.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-03-15 08:11:11.961947 fpop-0.0.5/tests/
--rw-r--r--   0 4294967294 4294967294        0 2023-03-15 06:12:17.000000 fpop-0.0.5/tests/__init__.py
--rw-r--r--   0 4294967294 4294967294      636 2023-03-15 06:12:17.000000 fpop-0.0.5/tests/constants.py
--rw-r--r--   0 4294967294 4294967294      726 2023-03-15 06:12:17.000000 fpop-0.0.5/tests/context.py
--rw-r--r--   0 4294967294 4294967294     1774 2023-03-15 06:12:18.000000 fpop-0.0.5/tests/mocked_ops.py
--rw-r--r--   0 4294967294 4294967294     7994 2023-03-15 06:12:18.000000 fpop-0.0.5/tests/test_prep_run_vasp.py
--rw-r--r--   0 4294967294 4294967294     7956 2023-03-15 06:12:18.000000 fpop-0.0.5/tests/test_prep_vasp.py
--rw-r--r--   0 4294967294 4294967294     6326 2023-03-15 06:12:18.000000 fpop-0.0.5/tests/test_run_vasp.py
--rw-r--r--   0 4294967294 4294967294     2844 2023-03-15 06:12:18.000000 fpop-0.0.5/tests/test_vasp_inputs.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.759537 fpop-0.0.6/
+-rw-r--r--   0 4294967294 4294967294     7650 2023-04-17 12:56:30.000000 fpop-0.0.6/LICENSE
+-rw-r--r--   0 4294967294 4294967294       16 2023-04-17 12:56:30.000000 fpop-0.0.6/MANIFEST.in
+-rw-r--r--   0 4294967294 4294967294      935 2023-04-17 13:05:04.755285 fpop-0.0.6/PKG-INFO
+-rw-r--r--   0 4294967294 4294967294      443 2023-04-17 12:56:30.000000 fpop-0.0.6/README.md
+drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.473580 fpop-0.0.6/fpop/
+-rw-r--r--   0 4294967294 4294967294       24 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/__about__.py
+-rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/__init__.py
+-rw-r--r--   0 4294967294 4294967294    18359 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/abacus.py
+-rw-r--r--   0 4294967294 4294967294     6271 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/prep_fp.py
+-rw-r--r--   0 4294967294 4294967294     6496 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/preprun_fp.py
+-rw-r--r--   0 4294967294 4294967294     6387 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/run_fp.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.568984 fpop-0.0.6/fpop/utils/
+-rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/utils/__init__.py
+-rw-r--r--   0 4294967294 4294967294      407 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/utils/step_config.py
+-rw-r--r--   0 4294967294 4294967294     8936 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/vasp.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.545326 fpop-0.0.6/fpop.egg-info/
+-rw-r--r--   0 4294967294 4294967294      935 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/PKG-INFO
+-rw-r--r--   0 4294967294 4294967294      614 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/SOURCES.txt
+-rw-r--r--   0 4294967294 4294967294        1 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/dependency_links.txt
+-rw-r--r--   0 4294967294 4294967294       31 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/requires.txt
+-rw-r--r--   0 4294967294 4294967294       11 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/top_level.txt
+-rw-r--r--   0 4294967294 4294967294       38 2023-04-17 13:05:04.761684 fpop-0.0.6/setup.cfg
+-rw-r--r--   0 4294967294 4294967294      847 2023-04-17 12:56:30.000000 fpop-0.0.6/setup.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.741001 fpop-0.0.6/tests/
+-rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/__init__.py
+-rw-r--r--   0 4294967294 4294967294     2097 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/constants.py
+-rw-r--r--   0 4294967294 4294967294      716 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/context.py
+-rw-r--r--   0 4294967294 4294967294     2401 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/mocked_ops.py
+-rw-r--r--   0 4294967294 4294967294     8032 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_abacus_inputs.py
+-rw-r--r--   0 4294967294 4294967294     6686 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_abacus.py
+-rw-r--r--   0 4294967294 4294967294     7994 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_run_vasp.py
+-rw-r--r--   0 4294967294 4294967294     7321 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_vasp.py
+-rw-r--r--   0 4294967294 4294967294     5919 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_abacus.py
+-rw-r--r--   0 4294967294 4294967294      943 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_fp.py
+-rw-r--r--   0 4294967294 4294967294     6387 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_vasp.py
+-rw-r--r--   0 4294967294 4294967294     2844 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_vasp_inputs.py
```

### Comparing `fpop-0.0.5/LICENSE` & `fpop-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fpop-0.0.5/PKG-INFO` & `fpop-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fpop
-Version: 0.0.5
+Version: 0.0.6
 Summary: Operators related to first-principles calculation
 Home-page: https://github.com/deepmodeling/fpop
 Author: Chengqian Zhang
 Author-email: 2043899742@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Provides: fpop
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fpop
 `fp` stands for first-principles calculation and `op` stands for operators. The abbreviation `fpop` stands for operators related to first-principles calculation.This project is based on [dflow](https://github.com/deepmodeling/dflow) which is a Python framework for constructing scientific computing workflows (e.g. concurrent learning workflows) employing Argo Workflows as the workflow engine. 
+# Installation
+```
+pip install fpop
+```
```

### Comparing `fpop-0.0.5/fpop/prep_fp.py` & `fpop-0.0.6/fpop/prep_fp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.5/fpop/preprun_fp.py` & `fpop-0.0.6/fpop/preprun_fp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.5/fpop/run_fp.py` & `fpop-0.0.6/fpop/run_fp.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,23 +65,22 @@
     def get_output_sign(cls):
         return OPIOSign(
             {
                 "backward_dir": Artifact(Path),
             }
         )
 
-    @abstractmethod
-    def input_files(self) -> List[str]:
+    def input_files(self, task_path) -> List[str]:
         r'''The mandatory input files to run a FP task.
         Returns
         -------
         files: List[str]
             A list of madatory input files names.
         '''
-        pass
+        return os.listdir(task_path)
 
     @abstractmethod
     def run_task(
         self,
         backward_dir_name,
         log_name,
         backward_list: List[str],
@@ -151,32 +150,32 @@
         run_image_config = ip["run_image_config"]
         backward_dir_name = ip["backward_dir_name"] 
         log_name = ip["log_name"] 
         backward_list = ip["backward_list"]
         optional_input = ip["optional_input"]
         task_name = ip["task_name"]
         task_path = ip["task_path"]
-        input_files = self.input_files()
+        input_files = self.input_files(task_path)
         input_files = [(Path(task_path) / ii).resolve() for ii in input_files]
         work_dir = Path(task_name)
         opt_input_files = []
         if ip["optional_artifact"]:
             for ss,vv in ip["optional_artifact"].items():
                 opt_input_files.append(ss)
         opt_input_files = [(Path(task_path) / ii).resolve() for ii in opt_input_files]
 
         with set_directory(work_dir,mkdir=True):
             # link input files
             for ii in input_files:
-                if not os.path.isfile(ii):
-                    raise FatalError(f"cannot file file {ii}")
+                if not os.path.exists(ii):
+                    raise FatalError(f"cannot file file/directory {ii}")
                 iname = ii.name
                 Path(iname).symlink_to(ii)
             for ii in opt_input_files:
-                if os.path.isfile(ii):
+                if os.path.exists(ii):
                     iname = ii.name
                     Path(iname).symlink_to(ii)
             backward_dir_name = self.run_task(backward_dir_name,log_name,backward_list,run_image_config,optional_input)
 
         return OPIO(
             {
                 "backward_dir": work_dir / backward_dir_name
```

### Comparing `fpop-0.0.5/fpop/vasp.py` & `fpop-0.0.6/fpop/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         if optional_artifact:
             for file_name, file_path in optional_artifact.items():
                 content = file_path.read_text()
                 Path(file_name).write_text(content)
 
 
 class RunVasp(RunFp):
-    def input_files(self) -> List[str]:
+    def input_files(self, task_path) -> List[str]:
         r'''The mandatory input files to run a vasp task.
         Returns
         -------
         files: List[str]
             A list of madatory input files names.
         '''
         return ["POSCAR", "INCAR", "POTCAR", "KPOINTS"]
```

### Comparing `fpop-0.0.5/fpop.egg-info/PKG-INFO` & `fpop-0.0.6/fpop.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fpop
-Version: 0.0.5
+Version: 0.0.6
 Summary: Operators related to first-principles calculation
 Home-page: https://github.com/deepmodeling/fpop
 Author: Chengqian Zhang
 Author-email: 2043899742@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Provides: fpop
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fpop
 `fp` stands for first-principles calculation and `op` stands for operators. The abbreviation `fpop` stands for operators related to first-principles calculation.This project is based on [dflow](https://github.com/deepmodeling/dflow) which is a Python framework for constructing scientific computing workflows (e.g. concurrent learning workflows) employing Argo Workflows as the workflow engine. 
+# Installation
+```
+pip install fpop
+```
```

### Comparing `fpop-0.0.5/setup.py` & `fpop-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fpop",
-    version="0.0.5",
+    version="0.0.6",
     author="Chengqian Zhang",
     author_email="2043899742@qq.com",
     description="Operators related to first-principles calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/fpop",
     packages=setuptools.find_packages(),
```

### Comparing `fpop-0.0.5/tests/context.py` & `fpop-0.0.6/tests/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,11 +11,9 @@
     skip_ut_with_dflow_reason = 'skip because environment variable SKIP_UT_WITH_DFLOW is set to non-zero'
 else:
     skip_ut_with_dflow = False
     skip_ut_with_dflow_reason = ''
 # one needs to set proper values for the following variable.
 default_image = 'dptechnology/dpgen2:latest'
 if os.getenv("DFLOW_DEBUG"):
-    from dflow import (
-        config,
-    )
+    from dflow.config import config
     config["mode"] = "debug"
```

### Comparing `fpop-0.0.5/tests/mocked_ops.py` & `fpop-0.0.6/tests/mocked_ops.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,18 @@
     FatalError,
 )
 
 upload_packages.append(__file__)
 
 import os, json, shutil, re, pickle, glob
 from pathlib import Path
-from typing import Tuple, List
+from typing import Tuple, List, Optional, Dict
 from context import fpop
 from fpop.vasp import RunVasp
+from fpop.run_fp import RunFp
 
 class MockedRunVasp(RunVasp):
     @OP.exec_sign_check
     def execute(
             self,
             ip : OPIO,
     ) -> OPIO:
@@ -59,8 +60,31 @@
         os.chdir(cwd)
 
         return OPIO({
             'backward_dir' : work_dir / backward_dir
         })
 
 
-    
+class TestInputFiles(RunFp):
+    def run_task(
+        self,
+        backward_dir_name,
+        log_name,
+        backward_list: List[str],
+        run_image_config: Optional[Dict]=None,
+        optional_input: Optional[Dict]=None,
+    ):
+        pass
+
+class TestInputFiles2(RunFp):
+    def input_files(self, task_path) -> List[str]:
+        return ["abc","ee"]
+
+    def run_task(
+        self,
+        backward_dir_name,
+        log_name,
+        backward_list: List[str],
+        run_image_config: Optional[Dict]=None,
+        optional_input: Optional[Dict]=None,
+    ):
+        pass
```

### Comparing `fpop-0.0.5/tests/test_prep_run_vasp.py` & `fpop-0.0.6/tests/test_prep_run_vasp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.5/tests/test_prep_vasp.py` & `fpop-0.0.6/tests/test_prep_vasp.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         default_image,
         upload_python_packages,
         skip_ut_with_dflow,
         skip_ut_with_dflow_reason,
         )
 from fpop.vasp import PrepVasp,VaspInputs
 from typing import List
-from constants import POSCAR_1_content,POSCAR_2_content
+from constants import POSCAR_1_content,POSCAR_2_content,dump_conf_from_poscar
 upload_packages.append("../fpop")
 upload_packages.append("./context.py")
 
 def check_vasp_tasks(tcase, ntasks):
     cc = 0
     tdirs = []
     for ii in range (ntasks):
@@ -59,36 +59,14 @@
         tcase.assertTrue(potcar.is_file())
         tcase.assertTrue(kpoints.is_file())
         tcase.assertEqual(incar.read_text(),'here incar')
         tcase.assertEqual(potcar.read_text(),'here potcar')
         cc += 1
     return tdirs
 
-def dump_conf_from_poscar(
-        type, 
-        conf_list
-        ) -> List[str] :
-    for ii in range(len(conf_list)):
-        Path("POSCAR_%d"%ii).write_text(conf_list[ii])
-    if type == "deepmd/npy":
-        confs = []
-        for ii in range(len(conf_list)):
-            ls = dpdata.System("POSCAR_%d"%ii, fmt="vasp/poscar")
-            ls.to_deepmd_npy("data.%03d"%ii)
-            confs.append("data.%03d"%ii)
-            os.remove("POSCAR_%d"%ii)
-        return confs
-    elif type == "vasp/poscar":
-        confs = []
-        for ii in range(len(conf_list)):
-            confs.append("POSCAR_%d")
-        return confs
-    else:
-        return []
-
 class TestPrepVaspDpConf(unittest.TestCase):
     '''
     deepmd/npy format named ["data.000","data.001"].
     no optional_input or optional_artifact.
     '''
     def setUp(self):
         self.ntasks = 2
```

### Comparing `fpop-0.0.5/tests/test_run_vasp.py` & `fpop-0.0.6/tests/test_run_vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import unittest
+import unittest,os
 from dflow.python import OPIO,TransientError
 import shutil
 from pathlib import Path
 from mock import mock, patch, call
 from context import fpop
 from fpop.vasp import RunVasp
 from mocked_ops import MockedRunVasp
 
 class TestRunVasp(unittest.TestCase):
     def setUp(self):
+        self.cwd = os.getcwd()
         self.task_path = Path('task/path')
         self.task_path.mkdir(parents=True, exist_ok=True)
         (self.task_path/'POSCAR').write_text('here poscar')
         (self.task_path/'INCAR').write_text('here incar')
         (self.task_path/'POTCAR').write_text('here potcar')
         (self.task_path/'KPOINTS').write_text('here kpoints')
         (self.task_path/'TEST1').write_text('here test1')
         (self.task_path/'TEST2').write_text('here test2')
         self.task_name = 'task_000'
         Path(self.task_name).mkdir(parents=True, exist_ok=True)
         (Path(self.task_name)/'our_log').write_text('here log')
 
     def tearDown(self):
+        os.chdir(self.cwd)
         if Path('task').is_dir():
             shutil.rmtree('task')
         if Path(self.task_name).is_dir():
             shutil.rmtree(self.task_name)
     
     @patch('fpop.vasp.run_command')
     def test_success(self, mocked_run):
```

### Comparing `fpop-0.0.5/tests/test_vasp_inputs.py` & `fpop-0.0.6/tests/test_vasp_inputs.py`

 * *Files identical despite different names*

