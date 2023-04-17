# Comparing `tmp/somenergia_dag_utils-0.1.0.tar.gz` & `tmp/somenergia_dag_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somenergia_dag_utils-0.1.0.tar", max compression
+gzip compressed data, was "somenergia_dag_utils-0.2.0.tar", max compression
```

## Comparing `somenergia_dag_utils-0.1.0.tar` & `somenergia_dag_utils-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0       82 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/README.md
--rw-r--r--   0        0        0      536 2023-04-17 08:14:15.670206 somenergia_dag_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 08:06:05.295744 somenergia_dag_utils-0.1.0/somenergia_dag_utils/__init__.py
--rw-r--r--   0        0        0     3243 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_branch_pull_ssh.py
--rw-r--r--   0        0        0      577 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_check_repo.py
--rw-r--r--   0        0        0      994 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_git_clone_ssh.py
--rw-r--r--   0        0        0     1077 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_image_build.py
--rw-r--r--   0        0        0      526 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_pre_prod_discriminator.py
--rw-r--r--   0        0        0      835 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_remove_image.py
--rw-r--r--   0        0        0     2343 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_update_docker_image.py
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 somenergia_dag_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 08:01:43.930010 somenergia_dag_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0       82 2023-04-17 11:17:53.976992 somenergia_dag_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     1089 2023-04-17 12:12:40.703731 somenergia_dag_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-17 12:04:30.334260 somenergia_dag_utils-0.2.0/somenergia_dag_utils/__init__.py
+-rw-r--r--   0        0        0     3424 2023-04-17 08:22:04.740046 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_branch_pull_ssh.py
+-rw-r--r--   0        0        0      579 2023-04-17 12:05:29.843441 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_check_repo.py
+-rw-r--r--   0        0        0     1015 2023-04-17 08:22:04.744047 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_git_clone_ssh.py
+-rw-r--r--   0        0        0     1037 2023-04-17 08:22:04.748046 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_image_build.py
+-rw-r--r--   0        0        0      528 2023-04-17 08:24:17.638821 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_pre_prod_discriminator.py
+-rw-r--r--   0        0        0      866 2023-04-17 11:38:03.065340 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_remove_image.py
+-rw-r--r--   0        0        0     2432 2023-04-17 08:26:10.817180 somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_update_docker_image.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 somenergia_dag_utils-0.2.0/PKG-INFO
```

### Comparing `somenergia_dag_utils-0.1.0/LICENSE` & `somenergia_dag_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `somenergia_dag_utils-0.1.0/pyproject.toml` & `somenergia_dag_utils-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,49 @@
 [tool.poetry]
 name = "somenergia-dag-utils"
-version = "0.1.0"
+version = "0.2.0"
 description = "utilities to run along with airflow dags used in somenergia"
 authors = ["Equip Dades <dades@somenergia.coop>"]
 readme = "README.md"
 packages = [{include = "somenergia_dag_utils"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-apache-airflow = "^2.5.3"
+apache-airflow = "<2.5.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.261"
 isort = "^5.12.0"
+git-changelog = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+include = '\.pyi?$'
+line-length = 79
+target-version = ['py38']
+# 'extend-exclude' excludes files or directories in addition to the defaults
+extend-exclude = '''
+(
+  /(
+	  \.eggs         # exclude a few common directories in the
+	| \.git          # root of the project
+	| \.hg
+	| \.mypy_cache
+	| \.tox
+	| \.venv
+	| _build
+	| buck-out
+	| build
+	| dist
+  )/
+)
+'''
+
+[tool.poetry_bumpversion.file."somenergia_dag_utils/__init__.py"]
+search = '__version__ = "{current_version}"'
+replace = '__version__ = "{new_version}"'
```

### Comparing `somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_branch_pull_ssh.py` & `somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_branch_pull_ssh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,102 @@
-from airflow.operators.python_operator import BranchPythonOperator
-from airflow import DAG
-import paramiko
 import io
-
 from random import randint
 from time import sleep
 
-class GitPullError(Exception): pass
+import paramiko
+from airflow import DAG
+from airflow.operators.python_operator import BranchPythonOperator
+
+
+class GitPullError(Exception):
+    pass
 
-def pull_repo_ssh(repo_name, repo_server_url, repo_server_key, task_name, dag_id=None):
+
+def pull_repo_ssh(
+    repo_name, repo_server_url, repo_server_key, task_name, dag_id=None
+):
     p = paramiko.SSHClient()
     p.set_missing_host_key_policy(paramiko.AutoAddPolicy())
     keyfile = io.StringIO(repo_server_key)
     mykey = paramiko.RSAKey.from_private_key(keyfile)
     p.connect(repo_server_url, port=2200, username="airflow", pkey=mykey)
 
     # randomly wait to prevent locks
     # TODO should use a dedicated DAG for all alerts
-    sleep(randint(1,10))
+    sleep(randint(1, 10))
 
-    stdin, stdout, stderr = p.exec_command(f"git -C /opt/airflow/repos/{repo_name} fetch")
+    stdin, stdout, stderr = p.exec_command(
+        f"git -C /opt/airflow/repos/{repo_name} fetch"
+    )
     txt_stderr = stderr.readlines()
 
     # TODO might be too fragile
-    if txt_stderr and not (txt_stderr[0].startswith('remote') or txt_stderr[0].startswith('From') or txt_stderr[0].startswith('Warning')):
-        print (f"Stderr of git fetch returned {txt_stderr} and {stdout.readlines()}.")
+    if txt_stderr and not (
+        txt_stderr[0].startswith("remote")
+        or txt_stderr[0].startswith("From")
+        or txt_stderr[0].startswith("Warning")
+    ):
+        print(
+            f"Stderr of git fetch returned {txt_stderr} and {stdout.readlines()}."
+        )
         raise GitPullError(txt_stderr)
     else:
-        print (f"git fetch returned {txt_stderr} and {stdout.readlines()}.")
+        print(f"git fetch returned {txt_stderr} and {stdout.readlines()}.")
 
-    stdin, stdout, stderr = p.exec_command(f"git -C /opt/airflow/repos/{repo_name} diff origin/main -- requirements.txt")
+    stdin, stdout, stderr = p.exec_command(
+        f"git -C /opt/airflow/repos/{repo_name} diff origin/main -- requirements.txt"
+    )
     txt_stdout = stdout.readlines()
     txt_stdout = "".join(txt_stdout)
     requirements_updated = len(txt_stdout) > 0
-    if txt_stderr and not (txt_stderr[0].startswith('remote') or txt_stderr[0].startswith('From')):
-        print (f"Stderr of git diff requirements returned {txt_stderr}. {bool(txt_stderr)}")
+    if txt_stderr and not (
+        txt_stderr[0].startswith("remote") or txt_stderr[0].startswith("From")
+    ):
+        print(
+            f"Stderr of git diff requirements returned {txt_stderr}. {bool(txt_stderr)}"
+        )
         raise GitPullError(txt_stderr)
     if requirements_updated:
-        print (f"Stdout de git diff requirements retornat {txt_stdout} and needs update")
+        print(
+            f"Stdout de git diff requirements retornat {txt_stdout} and needs update"
+        )
     else:
-        print (f"Stdout de git diff requirements no ha retornat cap missatge {txt_stdout}. stdout {stdout.readlines()}")
-    stdin, stdout, stderr = p.exec_command(f"git -C /opt/airflow/repos/{repo_name} pull")
+        print(
+            f"Stdout de git diff requirements no ha retornat cap missatge {txt_stdout}. stdout {stdout.readlines()}"
+        )
+    stdin, stdout, stderr = p.exec_command(
+        f"git -C /opt/airflow/repos/{repo_name} pull"
+    )
     txt_stderr = stderr.readlines()
     txt_stderr = "".join(txt_stderr)
-    print (f"Stderr de git pull ha retornat {txt_stderr}")
+    print(f"Stderr de git pull ha retornat {txt_stderr}")
     # si stderr té més de 0 \n és que hi ha canvis al fer pull
-    #Your configuration specifies to merge with the ref 'refs/heads/main' from the remote, but no such ref was fetched.
-    #Apareix quan fem molts git pull a la vegada
+    # Your configuration specifies to merge with the ref 'refs/heads/main' from the remote, but no such ref was fetched.
+    # Apareix quan fem molts git pull a la vegada
 
     # image removal and build is not working atm
-    print(f'dag id is {dag_id}')
-    if dag_id and dag_id == 'dades_sandbox_dag':
+    print(f"dag id is {dag_id}")
+    if dag_id and dag_id == "dades_sandbox_dag":
         print(f"Requirements updated? {requirements_updated}")
-        return 'update_docker_image' if requirements_updated else task_name
+        return "update_docker_image" if requirements_updated else task_name
     else:
         return task_name
 
-def build_branch_pull_ssh_task(dag: DAG, task_name, repo_name) -> BranchPythonOperator:
+
+def build_branch_pull_ssh_task(
+    dag: DAG, task_name, repo_name
+) -> BranchPythonOperator:
     branch_pull_ssh_task = BranchPythonOperator(
-        task_id='git_pull_task',
+        task_id="git_pull_task",
         python_callable=pull_repo_ssh,
-        op_kwargs={ "repo_name": repo_name,
-                    "repo_server_url": "{{ var.value.repo_server_url }}",
-                    "repo_server_key": "{{ var.value.repo_server_key }}",
-                    "task_name": task_name,
-                    "dag_id": dag.dag_id},
+        op_kwargs={
+            "repo_name": repo_name,
+            "repo_server_url": "{{ var.value.repo_server_url }}",
+            "repo_server_key": "{{ var.value.repo_server_key }}",
+            "task_name": task_name,
+            "dag_id": dag.dag_id,
+        },
         do_xcom_push=False,
-        dag=dag
+        dag=dag,
     )
 
     return branch_pull_ssh_task
```

### Comparing `somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_check_repo.py` & `somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_check_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from airflow.operators.python_operator import BranchPythonOperator
-from airflow import DAG
 import os.path
 
+from airflow import DAG
+from airflow.operators.python_operator import BranchPythonOperator
+
+
 def repo_exists_check(repo_name):
-    if os.path.exists(f'/opt/airflow/repos/{repo_name}/.git'):
-        return 'git_pull_task'
-    return 'git_clone'
+    if os.path.exists(f"/opt/airflow/repos/{repo_name}/.git"):
+        return "git_pull_task"
+    return "git_clone"
+
 
 def build_check_repo_task(dag: DAG, repo_name) -> BranchPythonOperator:
     check_repo_task = BranchPythonOperator(
-        task_id='check_repo_task',
+        task_id="check_repo_task",
         python_callable=repo_exists_check,
-        op_kwargs={ "repo_name": repo_name},
+        op_kwargs={"repo_name": repo_name},
         do_xcom_push=False,
         dag=dag,
     )
 
     return check_repo_task
```

### Comparing `somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_git_clone_ssh.py` & `somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_git_clone_ssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-from airflow.operators.python_operator import PythonOperator
-from airflow import DAG
-import paramiko
 import io
 
+import paramiko
+from airflow import DAG
+from airflow.operators.python_operator import PythonOperator
+
+
 def clone_repo_via_ssh(repo_name, repo_server_url, repo_server_key):
     p = paramiko.SSHClient()
     p.set_missing_host_key_policy(paramiko.AutoAddPolicy())
     keyfile = io.StringIO(repo_server_key)
     mykey = paramiko.RSAKey.from_private_key(keyfile)
     p.connect(repo_server_url, port=2200, username="airflow", pkey=mykey)
-    p.exec_command(f"git clone https://github.com/Som-Energia/{repo_name}.git /opt/airflow/repos/{repo_name}")
+    p.exec_command(
+        f"git clone https://github.com/Som-Energia/{repo_name}.git /opt/airflow/repos/{repo_name}"
+    )
+
 
 def build_git_clone_ssh_task(dag: DAG, repo_name) -> PythonOperator:
     git_clone_ssh_task = PythonOperator(
-        task_id='git_clone_ssh_task',
+        task_id="git_clone_ssh_task",
         python_callable=clone_repo_via_ssh,
-        op_kwargs={ "repo_name": repo_name,
-                    "repo_server_url" : "{{ var.value.repo_server_url }}",
-                    "repo_server_key": "{{ var.value.repo_server_key }}" },
+        op_kwargs={
+            "repo_name": repo_name,
+            "repo_server_url": "{{ var.value.repo_server_url }}",
+            "repo_server_key": "{{ var.value.repo_server_key }}",
+        },
         dag=dag,
     )
 
     return git_clone_ssh_task
```

### Comparing `somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_image_build.py` & `somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_remove_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+import requests
 from airflow import DAG
 from airflow.operators.python import PythonOperator
-import requests
 
-def _process(repo_name, portainer_key, post_url):
-    r = requests.post(
-            url=post_url,
-            headers={
-                'x-api-key' : portainer_key,
-                'Content-Type':'application/json'
-            },
-            params={
-                't':'somenergia-jardiner-carter-requirements:latest',
-                'remote': f'https://github.com/Som-Energia/{repo_name}.git#main',
-                'nocache': 'true'
-            },
-            data='{}',
-            verify=False
+
+def _process(portainer_key, remove_url):
+    r = requests.delete(
+        url=remove_url,
+        headers={
+            "x-api-key": portainer_key,
+            "Content-Type": "application/json",
+        },
+        data="{}",
+        verify=False,
     )
     r.raise_for_status()
 
-def build_image_build_task(dag: DAG, repo_name) -> PythonOperator:
 
-    task_image_build = PythonOperator(
-        task_id='image_build',
+def build_remove_image_task(dag: DAG, repo_name) -> PythonOperator:
+
+    task_remove_image = PythonOperator(
+        task_id="image_remove",
         python_callable=_process,
         op_kwargs={
-            'repo_name': repo_name,
-            'portainer_key': '{{ var.value.portainer_api_key }}',
-            'post_url': '{{ var.value.docker_build_url }}'
+            "portainer_key": "{{ var.value.portainer_api_key }}",
+            "remove_url": "{{ var.value.docker_base_remove_url }}/"
+            + repo_name
+            + "-requirements:latest",
         },
-        trigger_rule='one_success',
-        dag=dag
+        dag=dag,
+        trigger_rule="one_success",
     )
 
-    return task_image_build
+    return task_remove_image
```

### Comparing `somenergia_dag_utils-0.1.0/somenergia_dag_utils/t_update_docker_image.py` & `somenergia_dag_utils-0.2.0/somenergia_dag_utils/t_update_docker_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-from airflow.operators.python_operator import PythonOperator
-from airflow import DAG
-import paramiko
 import io
 
-class UpdateImageError(Exception): pass
+import paramiko
+from airflow import DAG
+from airflow.operators.python_operator import PythonOperator
+
+
+class UpdateImageError(Exception):
+    pass
+
+
+def update_docker_image_from_host_via_ssh(
+    host_server_key, host_server_url, repo_name, moll_url, docker_registry
+):
+    """
+    Update the docker image of the repo in the host server.
 
-def update_docker_image_from_host_via_ssh(host_server_key, host_server_url, repo_name, moll_url, docker_registry):
-    '''
     airflow is running in its container, so we need to connect to the host
     which has the python docker script that works.
     the python script:
     - logins to a docker daemon of a moll
     - tells the moll to build the image given the DockerFile of the repo which is cloned in the host
     - tells the moll to push the image to our private registry
 
     Then, the task will run in a DockerOperator who will download the image from the private registry
     if it doesn't have it. TODO: how will other molls know they have to update it?
-    '''
-    dockerfile = f'/opt/airflow/repos/{repo_name}/'
-    docker_registry_tag = f'{docker_registry}/{repo_name}-requirements:latest'
-    docker_build_push_script = '/opt/airflow/repos/docker-build-push/docker-build-push.py'
+    """
+    dockerfile = f"/opt/airflow/repos/{repo_name}/"
+    docker_registry_tag = f"{docker_registry}/{repo_name}-requirements:latest"
+    docker_build_push_script = (
+        "/opt/airflow/repos/docker-build-push/docker-build-push.py"
+    )
 
     p = paramiko.SSHClient()
     p.set_missing_host_key_policy(paramiko.AutoAddPolicy())
     keyfile = io.StringIO(host_server_key)
     mykey = paramiko.RSAKey.from_private_key(keyfile)
     p.connect(host_server_url, port=2200, username="airflow", pkey=mykey)
     cmd = f"python3 {docker_build_push_script} {moll_url} {dockerfile} {docker_registry_tag}"
@@ -36,21 +46,21 @@
     if txt_stderr:
         raise UpdateImageError(txt_stderr)
     return 0
 
 
 def build_update_image_task(dag: DAG, repo_name) -> PythonOperator:
     update_image_task = PythonOperator(
-        task_id='update_docker_image',
+        task_id="update_docker_image",
         python_callable=update_docker_image_from_host_via_ssh,
         op_kwargs={
             "repo_name": repo_name,
-            "host_server_url" : "{{ var.value.repo_server_url }}",
+            "host_server_url": "{{ var.value.repo_server_url }}",
             "host_server_key": "{{ var.value.repo_server_key }}",
-            "moll_url" : "{{ var.value.generic_moll_url }}",
-            "docker_registry": "{{ conn.somenergia_registry.host }}"
+            "moll_url": "{{ var.value.generic_moll_url }}",
+            "docker_registry": "{{ conn.somenergia_registry.host }}",
         },
-        trigger_rule='one_success',
+        trigger_rule="one_success",
         dag=dag,
     )
 
     return update_image_task
```

### Comparing `somenergia_dag_utils-0.1.0/PKG-INFO` & `somenergia_dag_utils-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: somenergia-dag-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: utilities to run along with airflow dags used in somenergia
 Author: Equip Dades
 Author-email: dades@somenergia.coop
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: apache-airflow (>=2.5.3,<3.0.0)
+Requires-Dist: apache-airflow (<2.5.3)
 Description-Content-Type: text/markdown
 
 # somenergia-dag_utils
 
 Dag tasks to check and update github repositories for CDD
```

