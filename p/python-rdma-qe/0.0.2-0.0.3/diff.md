# Comparing `tmp/python_rdma_qe-0.0.2.tar.gz` & `tmp/python_rdma_qe-0.0.3.tar.gz`

## Comparing `python_rdma_qe-0.0.2.tar` & `python_rdma_qe-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe_test.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdmaqe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/common/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/common/cli.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/common/fmf_tools.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/common/tc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/general.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/opa.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/roce.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/sriov/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/sriov/abc_sriov.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/rdma/sriov/sriov.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/.fmf/version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/functional.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/init_mem.txt
--rw-r--r--   0        0        0    23939 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/init_top.txt
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/rdmaqe/tests/sriov/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/README.md
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     4101 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe_test.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdmaqe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/cli.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/file_libs.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/fmf_tools.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/common/tc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/general.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/opa.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/roce.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/abc_sriov.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/sriov.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/.fmf/version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/functional.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_mem.txt
+-rw-r--r--   0        0        0    23939 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_top.txt
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/rdmaqe/tests/sriov/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    35079 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/LICENSE
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/README.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 python_rdma_qe-0.0.3/PKG-INFO
```

### Comparing `python_rdma_qe-0.0.2/rdmaqe_test.py` & `python_rdma_qe-0.0.3/rdmaqe_test.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/requirements-stable.txt` & `python_rdma_qe-0.0.3/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/common/cli.py` & `python_rdma_qe-0.0.3/rdmaqe/common/cli.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/common/fmf_tools.py` & `python_rdma_qe-0.0.3/rdmaqe/common/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/common/tc.py` & `python_rdma_qe-0.0.3/rdmaqe/common/tc.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/rdma/general.py` & `python_rdma_qe-0.0.3/rdmaqe/rdma/general.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/rdma/opa.py` & `python_rdma_qe-0.0.3/rdmaqe/rdma/opa.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/rdma/roce.py` & `python_rdma_qe-0.0.3/rdmaqe/rdma/roce.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/rdma/sriov/abc_sriov.py` & `python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/abc_sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/rdma/sriov/sriov.py` & `python_rdma_qe-0.0.3/rdmaqe/rdma/sriov/sriov.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/functional.py` & `python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/functional.py`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/rdmaqe/tests/opa-fm/init_top.txt` & `python_rdma_qe-0.0.3/rdmaqe/tests/opa-fm/init_top.txt`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/LICENSE` & `python_rdma_qe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/pyproject.toml` & `python_rdma_qe-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rdma_qe-0.0.2/PKG-INFO` & `python_rdma_qe-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rdma-qe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Redhat Kernel RDMA QE Python libs and tests
 Project-URL: Documentation, https://gitlab.com/rh-rdma-qe/python-rdma-qe#README.md
 Project-URL: Issues, https://gitlab.com/rh-rdma-qe/python-rdma-qe/issues
 Project-URL: Source, https://gitlab.com/rh-rdma-qe/python-rdma-qe
 Author-email: Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
```

