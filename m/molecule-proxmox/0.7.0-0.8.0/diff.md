# Comparing `tmp/molecule-proxmox-0.7.0.tar.gz` & `tmp/molecule-proxmox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-proxmox-0.7.0.tar", last modified: Mon Oct 24 17:10:35 2022, max compression
+gzip compressed data, was "molecule-proxmox-0.8.0.tar", last modified: Mon Apr 17 20:12:16 2023, max compression
```

## Comparing `molecule-proxmox-0.7.0.tar` & `molecule-proxmox-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       77 2022-01-31 14:13:36.000000 molecule-proxmox-0.7.0/MANIFEST.in
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     6714 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/PKG-INFO
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     4824 2022-04-04 15:48:43.000000 molecule-proxmox-0.7.0/README.rst
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       38 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/setup.cfg
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     1228 2022-10-24 16:52:04.000000 molecule-proxmox-0.7.0/setup.py
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       22 2022-10-21 19:25:04.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/__init__.py
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/cookiecutter/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)      107 2022-01-31 14:13:36.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/cookiecutter/cookiecutter.json
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)      110 2022-01-31 14:13:36.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     3867 2022-01-31 14:13:36.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/driver.py
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/modules/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)        0 2022-01-31 14:13:36.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/modules/__init__.py
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     6893 2022-04-04 15:43:42.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     2800 2022-07-18 15:24:42.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/create.yml
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     1666 2022-04-04 15:43:42.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/destroy.yml
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)      851 2022-10-21 19:17:43.000000 molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/prepare.yml
-drwxrwxr-x   0 mmeffie   (1000) mmeffie   (1000)        0 2022-10-24 17:10:35.924966 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)     6714 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/PKG-INFO
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)      746 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/SOURCES.txt
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)        1 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/dependency_links.txt
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       61 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/entry_points.txt
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       48 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/requires.txt
--rw-rw-r--   0 mmeffie   (1000) mmeffie   (1000)       17 2022-10-24 17:10:35.000000 molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/top_level.txt
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       77 2022-01-25 16:05:10.000000 molecule-proxmox-0.8.0/MANIFEST.in
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     7645 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     5563 2023-04-17 19:37:13.000000 molecule-proxmox-0.8.0/README.rst
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       38 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/setup.cfg
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1220 2023-04-17 20:04:53.000000 molecule-proxmox-0.8.0/setup.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       22 2023-04-17 20:11:21.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/__init__.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/cookiecutter/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      107 2022-01-25 16:07:10.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/cookiecutter/cookiecutter.json
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      110 2022-01-25 22:32:46.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     3867 2022-01-25 22:36:30.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/driver.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/modules/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        0 2022-01-29 05:50:49.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/modules/__init__.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     6893 2022-05-20 13:00:17.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     4207 2023-04-17 19:56:35.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/create.yml
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1666 2022-05-20 13:00:17.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/destroy.yml
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      851 2023-04-17 19:15:49.000000 molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/prepare.yml
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-04-17 20:12:16.292099 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     7645 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      746 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        1 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       61 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/entry_points.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       40 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/requires.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       17 2023-04-17 20:12:16.000000 molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/top_level.txt
```

### Comparing `molecule-proxmox-0.7.0/PKG-INFO` & `molecule-proxmox-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-proxmox
-Version: 0.7.0
+Version: 0.8.0
 Summary: Proxmox Molecule Plugin :: run molecule tests using proxmox
 Home-page: https://github.com/meffie/molecule-proxmox
 Author: Michael Meffie
 Author-email: mmeffie@sinenomine.net
 License: UNKNOWN
 Description: ***********************
         Molecule Proxmox Plugin
@@ -33,14 +33,15 @@
         -------------------------------------
         
         The molecule instances are created by cloning Proxmox virtual machine
         templates.  You will need to create one or more templates.
         
         Templates have the following requirements.
         
+        * A cloud-init drive if any cloud-init settings are used
         * networking configured
         * Python installed for Ansible
         * qemu-guest-agent installed and enabled in Proxmox
         * ssh server installed
         * user account for Ansible
         * An ssh public key must be added to the ``authorized_keys`` for the Ansible user account.
         * If a non-root user is used for the Ansible user (recommended), that user should be
@@ -112,14 +113,37 @@
                 ssh_user: tester
                 ssh_identity_file: /path/to/id_rsa
                 template_name: debian11
            platforms:
              - name: test01
              - name: test02
         
+        .. code-block:: yaml
+        
+           driver:
+             name: proxmox
+             options:
+                # Secrets file may be encrypted with ansible-vault.
+                proxmox_secrets: /path/to/proxmox_secrets.yml"
+                node: pve01
+                ssh_user: tester
+                ssh_identity_file: /path/to/id_rsa
+                template_name: debian11
+           platforms:
+             - name: test01
+               template_name: debian11
+               # See https://docs.ansible.com/ansible/latest/collections/community/general/proxmox_kvm_module.html
+               # for cloud-init options.
+               ciuser: some_user
+               cipassword: some_password
+               ipconfig:
+                 ipconfig0: 'ip=192.168.0.2/24,gw=192.168.0.1'
+               nameservers:
+                 - 192.169.0.245
+        
         Development
         ===========
         
         To checkout the source code:
         
         .. code-block:: bash
```

### Comparing `molecule-proxmox-0.7.0/README.rst` & `molecule-proxmox-0.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 -------------------------------------
 
 The molecule instances are created by cloning Proxmox virtual machine
 templates.  You will need to create one or more templates.
 
 Templates have the following requirements.
 
+* A cloud-init drive if any cloud-init settings are used
 * networking configured
 * Python installed for Ansible
 * qemu-guest-agent installed and enabled in Proxmox
 * ssh server installed
 * user account for Ansible
 * An ssh public key must be added to the ``authorized_keys`` for the Ansible user account.
 * If a non-root user is used for the Ansible user (recommended), that user should be
@@ -104,14 +105,37 @@
         ssh_user: tester
         ssh_identity_file: /path/to/id_rsa
         template_name: debian11
    platforms:
      - name: test01
      - name: test02
 
+.. code-block:: yaml
+
+   driver:
+     name: proxmox
+     options:
+        # Secrets file may be encrypted with ansible-vault.
+        proxmox_secrets: /path/to/proxmox_secrets.yml"
+        node: pve01
+        ssh_user: tester
+        ssh_identity_file: /path/to/id_rsa
+        template_name: debian11
+   platforms:
+     - name: test01
+       template_name: debian11
+       # See https://docs.ansible.com/ansible/latest/collections/community/general/proxmox_kvm_module.html
+       # for cloud-init options.
+       ciuser: some_user
+       cipassword: some_password
+       ipconfig:
+         ipconfig0: 'ip=192.168.0.2/24,gw=192.168.0.1'
+       nameservers:
+         - 192.169.0.245
+
 Development
 ===========
 
 To checkout the source code:
 
 .. code-block:: bash
```

### Comparing `molecule-proxmox-0.7.0/setup.py` & `molecule-proxmox-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     entry_points={
         'molecule.driver': [
             'proxmox = molecule_proxmox.driver:Proxmox',
         ],
     },
     install_requires=[
         # molecule plugins are not allowed to mention Ansible as a direct dependency
-        'molecule>=3.2.0,<=4.0.1',
+        'molecule==4.0.1',
         'pyyaml',
         'proxmoxer>=1.3.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox/driver.py` & `molecule-proxmox-0.8.0/src/molecule_proxmox/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py` & `molecule-proxmox-0.8.0/src/molecule_proxmox/modules/proxmox_qemu_agent.py`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/create.yml` & `molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/create.yml`

 * *Files 23% similar despite different names*

```diff
@@ -28,14 +28,46 @@
         timeout: "{{ options.timeout | d(omit) }}"
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         loop_var: p
         label: "{{ p.name }}"
       register: proxmox_clone
 
+    - name: "Update molecule instance config(s)"
+      proxmox_kvm:
+        state: present
+        update: true
+        api_host: "{{ api_host | d(options.api_host) | d(omit) }}"
+        api_user: "{{ api_user | d(options.api_user) | d(omit) }}"
+        api_password: "{{ api_password | d(options.api_password) | d(omit) }}"
+        api_token_id: "{{ api_token_id | d(options.api_token_id) | d(omit) }}"
+        api_token_secret: "{{ api_token_secret | d(options.api_token_secret) | d(omit) }}"
+        vmid: "{{ rc.vmid }}"
+        node: "{{ options.node }}"
+        timeout: "{{ options.timeout | d(omit) }}"
+        ciuser: "{{ rc.p.ciuser | d(omit, true) }}"
+        cipassword: "{{ rc.p.cipassword | d(omit, true) }}"
+        citype: "{{ rc.p.citype | d(omit, true) }}"
+        ipconfig: "{{ rc.p.ipconfig | d(omit, true) }}"
+        nameservers: "{{ rc.p.nameservers | d(omit, true) }}"
+        searchdomains: "{{ rc.p.searchdomains | d(omit, true) }}"
+        sshkeys: "{{ rc.p.sshkeys | d(omit, true) }}"
+      when: >
+        rc.p.ciuser is defined or
+        rc.p.cipassword is defined or
+        rc.p.citype is defined or
+        rc.p.ipconfig is defined or
+        rc.p.nameservers is defined or
+        rc.p.searchdomains is defined or
+        rc.p.sshkeys is defined
+      loop: "{{ proxmox_clone.results }}"
+      loop_control:
+        loop_var: rc
+        label: "{{ rc.p.name, rc.vmid }}"
+
     - name: "Start molecule instance(s)."
       proxmox_qemu_agent:
         api_host: "{{ api_host | d(options.api_host) | d(omit) }}"
         api_user: "{{ api_user | d(options.api_user) | d(omit) }}"
         api_password: "{{ api_password | d(options.api_password) | d(omit) }}"
         api_token_id: "{{ api_token_id | d(options.api_token_id) | d(omit) }}"
         api_token_secret: "{{ api_token_secret | d(options.api_token_secret) | d(omit) }}"
```

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/destroy.yml` & `molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox/playbooks/prepare.yml` & `molecule-proxmox-0.8.0/src/molecule_proxmox/playbooks/prepare.yml`

 * *Files identical despite different names*

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/PKG-INFO` & `molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-proxmox
-Version: 0.7.0
+Version: 0.8.0
 Summary: Proxmox Molecule Plugin :: run molecule tests using proxmox
 Home-page: https://github.com/meffie/molecule-proxmox
 Author: Michael Meffie
 Author-email: mmeffie@sinenomine.net
 License: UNKNOWN
 Description: ***********************
         Molecule Proxmox Plugin
@@ -33,14 +33,15 @@
         -------------------------------------
         
         The molecule instances are created by cloning Proxmox virtual machine
         templates.  You will need to create one or more templates.
         
         Templates have the following requirements.
         
+        * A cloud-init drive if any cloud-init settings are used
         * networking configured
         * Python installed for Ansible
         * qemu-guest-agent installed and enabled in Proxmox
         * ssh server installed
         * user account for Ansible
         * An ssh public key must be added to the ``authorized_keys`` for the Ansible user account.
         * If a non-root user is used for the Ansible user (recommended), that user should be
@@ -112,14 +113,37 @@
                 ssh_user: tester
                 ssh_identity_file: /path/to/id_rsa
                 template_name: debian11
            platforms:
              - name: test01
              - name: test02
         
+        .. code-block:: yaml
+        
+           driver:
+             name: proxmox
+             options:
+                # Secrets file may be encrypted with ansible-vault.
+                proxmox_secrets: /path/to/proxmox_secrets.yml"
+                node: pve01
+                ssh_user: tester
+                ssh_identity_file: /path/to/id_rsa
+                template_name: debian11
+           platforms:
+             - name: test01
+               template_name: debian11
+               # See https://docs.ansible.com/ansible/latest/collections/community/general/proxmox_kvm_module.html
+               # for cloud-init options.
+               ciuser: some_user
+               cipassword: some_password
+               ipconfig:
+                 ipconfig0: 'ip=192.168.0.2/24,gw=192.168.0.1'
+               nameservers:
+                 - 192.169.0.245
+        
         Development
         ===========
         
         To checkout the source code:
         
         .. code-block:: bash
```

### Comparing `molecule-proxmox-0.7.0/src/molecule_proxmox.egg-info/SOURCES.txt` & `molecule-proxmox-0.8.0/src/molecule_proxmox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

