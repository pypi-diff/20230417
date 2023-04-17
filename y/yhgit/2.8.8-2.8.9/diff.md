# Comparing `tmp/yhgit-2.8.8.tar.gz` & `tmp/yhgit-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yhgit-2.8.8.tar", last modified: Thu Mar 23 02:14:10 2023, max compression
+gzip compressed data, was "yhgit-2.8.9.tar", last modified: Thu Mar 23 06:19:27 2023, max compression
```

## Comparing `yhgit-2.8.8.tar` & `yhgit-2.8.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 02:14:10.448428 yhgit-2.8.8/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.8.8/LICENSE.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 02:14:10.448616 yhgit-2.8.8/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.8.8/README.md
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-03-23 02:14:10.449423 yhgit-2.8.8/setup.cfg
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     2086 2023-03-23 02:13:58.000000 yhgit-2.8.8/setup.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 02:14:10.444052 yhgit-2.8.8/yhgit/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.8.8/yhgit/__init__.py
--rw-r--r--   0 fanguohuijack   (501) staff       (20)    60275 2023-03-23 02:13:52.000000 yhgit-2.8.8/yhgit/yhgit.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 02:14:10.447492 yhgit-2.8.8/yhgit.egg-info/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/SOURCES.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/dependency_links.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/entry_points.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/requires.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-03-23 02:14:10.000000 yhgit-2.8.8/yhgit.egg-info/top_level.txt
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.387082 yhgit-2.8.9/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.8.9/LICENSE.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 06:19:27.387199 yhgit-2.8.9/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.8.9/README.md
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-03-23 06:19:27.387581 yhgit-2.8.9/setup.cfg
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     2086 2023-03-23 06:18:49.000000 yhgit-2.8.9/setup.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.383940 yhgit-2.8.9/yhgit/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.8.9/yhgit/__init__.py
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)    60363 2023-03-23 06:05:47.000000 yhgit-2.8.9/yhgit/yhgit.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.386874 yhgit-2.8.9/yhgit.egg-info/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/SOURCES.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/dependency_links.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/entry_points.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/requires.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/top_level.txt
```

### Comparing `yhgit-2.8.8/LICENSE.txt` & `yhgit-2.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yhgit-2.8.8/PKG-INFO` & `yhgit-2.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.8.8
+Version: 2.8.9
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

### Comparing `yhgit-2.8.8/README.md` & `yhgit-2.8.9/README.md`

 * *Files identical despite different names*

### Comparing `yhgit-2.8.8/setup.py` & `yhgit-2.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     packages=find_packages(),
     entry_points={
           'console_scripts': [
               'yhgit = yhgit.yhgit:main'
           ]
     },
     python_requires='>=3.7',
-    version='2.8.8',  # Start with a small number and increase it with every change you make
+    version='2.8.9',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='yh branch git manager util',  # Give a short description about your library
     author='yonghuifan21',  # Type in your name
     author_email='jackfan1@yonghui.com',  # Type in your E-Mail
     url='http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git',
     download_url='https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz',  # I explain this later on
     keywords=['yhgit', 'git', 'yh'],  # Keywords that define your package best
```

### Comparing `yhgit-2.8.8/yhgit/yhgit.py` & `yhgit-2.8.9/yhgit/yhgit.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,29 +60,31 @@
     module = ''
     pod = ''
     result = 0
     pod = ''
     branch = ''
     msg = ''
     tag = ''
+    git = ''
 
-    def __init__(self, module, pod, res, branch, msg='', tag=''):
+    def __init__(self, module, pod, res, branch, msg='', tag='', git=''):
         """
         :param module: 模块名字
         :param pod: pod名字
         :param res: 结果 0 表示失败 1 表示成功 -1 表示其他异常
         :param branch: 分支
         :param msg: 错误信息
         """
         self.module = module
         self.result = res
         self.pod = pod
         self.msg = msg
         self.branch = branch
         self.tag = tag
+        self.git = git
 
 
 # 读取yaml文件数据
 def yaml_data(yaml_path):
     """
     :param yaml_path: ymal路径
     :return: 返回yaml数据
@@ -437,24 +439,24 @@
         for mo_re in branch_result:
             if a.module and mo_re.module and a.module == mo_re.module and mo_re.result == 1:
                 module_dict = {"module": mo_re.module, "pod": a.pod, "git": a.git, "branch": n_branch,
                                "configurations": a.configurations,
                                "inhibit_warnings": a.inhibit_warnings}
                 dependenceList[index] = module_dict
         index += 1
-    # print("convert=======" + str(dependenceList))
+    print("convert=======" + str(dependenceList))
     except_list = [
-        module for module in branch_result if module.module not in [
-            pod.module for pod in conver_deplist]]
+        module for module in branch_result if ((module.result == 1) and (module.module not in [
+            pod.module for pod in conver_deplist]))]
     if len(except_list) > 0:
         for mo_re in except_list:
             module_dict = {
                 "module": mo_re.module,
-                "pod": a.pod,
-                "git": a.git,
+                "pod": mo_re.pod,
+                "git": mo_re.git,
                 "branch": n_branch
             }
             dependenceList.append(module_dict)
 
     # print("except_list=======" + str(dependenceList))
     if not (before_branch and len(before_branch) > 0):
         before_branch = n_branch
@@ -1097,15 +1099,15 @@
             open(yamlPath, 'w').close()
             after_convert = []
             module_dict = {"module": newfile_name, "pod": newfile_name, "git": git, "branch": n_branch}
             after_convert.append(module_dict)
             podmodule_data = {"version": "1.0.0", "branch": str(n_branch), "dependencies": after_convert}
             save_dict_to_yaml(podmodule_data, yamlPath)
 
-        branch_res = [ModuleStatusModel(newfile_name, newfile_name, res, n_branch, error)]
+        branch_res = [ModuleStatusModel(newfile_name, newfile_name, res, n_branch, error, git=git)]
         update_module_files(yamlPath, localyamlPath, branch_res, n_branch, modules_name)
         succ_list = []
         fail_list = []
         for merg_Model in branch_res:
             if merg_Model.result == 1:
                 succ_list.append(merg_Model)
             else:
```

### Comparing `yhgit-2.8.8/yhgit.egg-info/PKG-INFO` & `yhgit-2.8.9/yhgit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.8.8
+Version: 2.8.9
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

