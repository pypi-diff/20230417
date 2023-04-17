# Comparing `tmp/sshclick-0.4.4.tar.gz` & `tmp/sshclick-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshclick-0.4.4.tar", max compression
+gzip compressed data, was "sshclick-0.5.0.tar", max compression
```

## Comparing `sshclick-0.4.4.tar` & `sshclick-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
--rw-r--r--   0        0        0     1068 2022-05-26 10:44:55.000000 sshclick-0.4.4/LICENSE
--rw-r--r--   0        0        0    13665 2022-08-08 14:36:37.567084 sshclick-0.4.4/README.md
--rw-r--r--   0        0        0      914 2022-08-08 14:36:37.567084 sshclick-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/__init__.py
--rw-r--r--   0        0        0      575 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/cmd_group.py
--rw-r--r--   0        0        0      602 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/cmd_host.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/__init__.py
--rw-r--r--   0        0        0     1121 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/group_create.py
--rw-r--r--   0        0        0      830 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/group_delete.py
--rw-r--r--   0        0        0      802 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/group_list.py
--rw-r--r--   0        0        0     1579 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/group_set.py
--rw-r--r--   0        0        0     2050 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/group/group_show.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/__init__.py
--rw-r--r--   0        0        0     2875 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_create.py
--rw-r--r--   0        0        0      931 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_delete.py
--rw-r--r--   0        0        0     4753 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_list.py
--rw-r--r--   0        0        0     4879 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_set.py
--rw-r--r--   0        0        0     3296 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_show.py
--rw-r--r--   0        0        0     1270 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/cmds/host/host_test.py
--rw-r--r--   0        0        0      292 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/globals.py
--rw-r--r--   0        0        0     1037 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/main.py
--rw-r--r--   0        0        0      231 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/__init__.py
--rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/__init__.py
--rw-r--r--   0        0        0     1890 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/card.py
--rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/json.py
--rw-r--r--   0        0        0     1928 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/panels.py
--rw-r--r--   0        0        0     1866 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/simple.py
--rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/table.py
--rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/host_styles/table2.py
--rw-r--r--   0        0        0    12144 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/ssh_config.py
--rw-r--r--   0        0        0      355 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/ssh_group.py
--rw-r--r--   0        0        0     1371 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/ssh_host.py
--rw-r--r--   0        0        0     4082 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/sshextras.py
--rw-r--r--   0        0        0     1813 2022-08-08 14:36:37.567084 sshclick-0.4.4/sshclick/sshc/sshutils.py
--rw-r--r--   0        0        0    14913 2022-08-08 14:43:18.311148 sshclick-0.4.4/setup.py
--rw-r--r--   0        0        0    14523 2022-08-08 14:43:18.311983 sshclick-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-17 16:09:18.391084 sshclick-0.5.0/LICENSE
+-rw-r--r--   0        0        0    14399 2023-04-17 16:08:59.411089 sshclick-0.5.0/README.md
+-rw-r--r--   0        0        0     1037 2023-04-17 13:22:02.913713 sshclick-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-10 13:49:51.835727 sshclick-0.5.0/sshclick/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-17 12:52:26.614177 sshclick-0.5.0/sshclick/cmds/cmd_config.py
+-rw-r--r--   0        0        0      646 2022-08-10 20:50:38.844620 sshclick-0.5.0/sshclick/cmds/cmd_group.py
+-rw-r--r--   0        0        0      732 2023-04-14 15:17:18.853394 sshclick-0.5.0/sshclick/cmds/cmd_host.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:48:49.004234 sshclick-0.5.0/sshclick/cmds/config/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-17 12:59:37.314064 sshclick-0.5.0/sshclick/cmds/config/config_del.py
+-rw-r--r--   0        0        0     1354 2023-04-17 12:59:34.824065 sshclick-0.5.0/sshclick/cmds/config/config_set.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/group/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-14 13:48:55.874783 sshclick-0.5.0/sshclick/cmds/group/group_create.py
+-rw-r--r--   0        0        0     2217 2023-04-14 13:45:08.024842 sshclick-0.5.0/sshclick/cmds/group/group_delete.py
+-rw-r--r--   0        0        0     1068 2022-09-11 17:04:13.785725 sshclick-0.5.0/sshclick/cmds/group/group_list.py
+-rw-r--r--   0        0        0     1196 2023-04-14 14:12:19.544415 sshclick-0.5.0/sshclick/cmds/group/group_rename.py
+-rw-r--r--   0        0        0     2421 2023-04-14 13:49:04.844781 sshclick-0.5.0/sshclick/cmds/group/group_set.py
+-rw-r--r--   0        0        0     2387 2023-04-17 09:36:07.926863 sshclick-0.5.0/sshclick/cmds/group/group_show.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/cmds/host/__init__.py
+-rw-r--r--   0        0        0     3970 2023-04-14 14:07:21.804493 sshclick-0.5.0/sshclick/cmds/host/host_create.py
+-rw-r--r--   0        0        0     2458 2023-04-14 14:08:54.144468 sshclick-0.5.0/sshclick/cmds/host/host_delete.py
+-rw-r--r--   0        0        0     1715 2023-04-17 09:39:36.716809 sshclick-0.5.0/sshclick/cmds/host/host_install_key.py
+-rw-r--r--   0        0        0     4494 2023-04-17 10:02:52.786444 sshclick-0.5.0/sshclick/cmds/host/host_list.py
+-rw-r--r--   0        0        0     1162 2023-04-14 14:12:44.404409 sshclick-0.5.0/sshclick/cmds/host/host_rename.py
+-rw-r--r--   0        0        0     6579 2023-04-14 14:19:27.594303 sshclick-0.5.0/sshclick/cmds/host/host_set.py
+-rw-r--r--   0        0        0     3005 2023-04-17 12:43:47.674312 sshclick-0.5.0/sshclick/cmds/host/host_show.py
+-rw-r--r--   0        0        0     1581 2023-04-14 13:45:33.234835 sshclick-0.5.0/sshclick/cmds/host/host_test.py
+-rw-r--r--   0        0        0      107 2023-04-17 12:21:37.064660 sshclick-0.5.0/sshclick/globals.py
+-rw-r--r--   0        0        0     1891 2023-04-17 13:24:55.183668 sshclick-0.5.0/sshclick/main.py
+-rw-r--r--   0        0        0      411 2023-04-17 12:19:51.954689 sshclick-0.5.0/sshclick/sshc/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/__init__.py
+-rw-r--r--   0        0        0     2312 2022-09-11 16:36:02.105733 sshclick-0.5.0/sshclick/sshc/host_styles/card.py
+-rw-r--r--   0        0        0      363 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/json.py
+-rw-r--r--   0        0        0     2484 2023-04-17 09:57:40.316526 sshclick-0.5.0/sshclick/sshc/host_styles/panels.py
+-rw-r--r--   0        0        0     2262 2022-09-11 16:56:01.465727 sshclick-0.5.0/sshclick/sshc/host_styles/simple.py
+-rw-r--r--   0        0        0     1429 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/table.py
+-rw-r--r--   0        0        0     1780 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/host_styles/table2.py
+-rw-r--r--   0        0        0    16226 2023-04-17 12:19:45.224691 sshclick-0.5.0/sshclick/sshc/ssh_config.py
+-rw-r--r--   0        0        0      434 2023-04-17 08:39:08.357758 sshclick-0.5.0/sshclick/sshc/ssh_group.py
+-rw-r--r--   0        0        0     1447 2023-04-17 12:19:06.094701 sshclick-0.5.0/sshclick/sshc/ssh_host.py
+-rw-r--r--   0        0        0     4555 2023-04-17 12:20:45.644673 sshclick-0.5.0/sshclick/sshc/ssh_parameters.py
+-rw-r--r--   0        0        0     4082 2022-08-08 14:36:37.567084 sshclick-0.5.0/sshclick/sshc/sshextras.py
+-rw-r--r--   0        0        0     4842 2023-04-17 12:22:18.274649 sshclick-0.5.0/sshclick/sshc/sshutils.py
+-rw-r--r--   0        0        0    15497 1970-01-01 00:00:00.000000 sshclick-0.5.0/PKG-INFO
```

### Comparing `sshclick-0.4.4/LICENSE` & `sshclick-0.5.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Karlo Tisaj
+Copyright (c) 2023 Karlo Tisaj
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sshclick-0.4.4/README.md` & `sshclick-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SSH Click Config manager (sshclick)
 
-Check this page on [GitHub](https://github.com/karlot/sshclick)
+![splash_gif](tapes/splash.gif)
 
 ## Links
 
 - [Intro](https://github.com/karlot/sshclick#intro)
 - [Why?](https://github.com/karlot/sshclick#why)
 - [What does it do](https://github.com/karlot/sshclick#what-does-it-do)
   - [Installation procedure](https://github.com/karlot/sshclick#installation-procedure)
@@ -141,15 +141,15 @@
 #@desc: <GROUP-DESCRIPTION> [OPTIONAL, SINGLE]
 #@info: <GROUP-INFO-LINES>  [OPTIONAL,MULTIPLE]
 #-------------------------------------------------------------------------------
 Host ...    <-- this hosts definitions are part of the defined group
     param1 value1
     param2 value2
 
-#@host: <HOST-INFO-LINES>  [OPTIONAL,MULTIPLE] <-- Adds info to following host
+#@host: <HOST-INFO-LINES>   [OPTIONAL,MULTIPLE] <-- Adds info to following host
 Host ...
 
 <ANOTHER GROUP HEADER>
 ```
 
 If there are no groups defined, then all hosts are considered to be part of "default" group. SSHClick can be used to move hosts between groups and handle keeping SSH config "tidy" and with consistent format.
 
@@ -159,86 +159,89 @@
 SSHClick is deploying `sshc` cli tool that allows interacting with your SSH Config file and perform various organization,listing, displaying and modification of SSH Group/Host configuration parameters.  
 `sshc` comes with pre-built lots of help options so each level of commands provide `--help` options to provide you info what commands and options are available at which command level.  
 
 For example to check version, type: `sshc --version`  
 _Sample output:_
 ```console
 $ sshc --version
-SSHClick (sshc) - Version: 0.4.1
+SSHClick (sshc) - Version: 0.5.0
 ```
 
 If you run `sshc` command alone, or adding `-h` or `--help` option, it will show help what else must be added to the command...  
 _Example:_
 ```console
 $ sshc --help
 Usage: sshc [OPTIONS] COMMAND [ARGS]...
 
-  SSHClick - SSH Config manager
+  SSHClick - SSH Config manager. version 0.5.0
 
-  Note: As this is early alpha, backup your SSH config files before this
+  NOTE: As this is early alpha, backup your SSH config files before this
   software, as you might accidentally lose some configuration
 
 Options:
-  --sshconfig PATH  Config file, default is ~/.ssh/config
-  --stdout          Send changed SSH config to STDOUT instead to original file
-  --version         Show current version
+  --sshconfig TEXT  Config file (default: ~/.ssh/config)
+  --stdout          Send changed SSH config to STDOUT instead to original
+                    file, can be enabled with setting ENV variable (export
+                    SSHC_STDOUT=1)
+  --version         Show the version and exit.
   -h, --help        Show this message and exit.
 
 Commands:
-  group  Manage groups
-  host   Manage hosts
+  config  Modify SSHClick configuration trough SSH Config
+  group   Command group for managing groups
+  groups  Lists all groups
+  host    Command group for managing hosts
+  hosts   List configured hosts
 ```
 
-Main sub-commands are for separate control of:  
-- Groups (via `sshc group` command)
-  - Allows operation of groups inside SSH config
-- Hosts (via `sshc host` command)
-  - Allows operation of hosts inside SSH config
 
 ### `group` commands and options
 
 To manage "groups" type `sshc group --help` to see options.  
 _example:_
 ```console
 $ sshc group --help
 Usage: sshc group [OPTIONS] COMMAND [ARGS]...
 
-  Manage groups
+  Command group for managing groups
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
   create  Create new group
   delete  Delete group
   list    Lists all groups
+  rename  Rename existing group
   set     Change group parameters
   show    Shows group details
 ```
 
 ### `host` commands and options
 
 To manage "groups" type `sshc host --help` to see options.  
 _example:_
 ```console
 $ sshc host --help
 Usage: sshc host [OPTIONS] COMMAND [ARGS]...
 
-  Manage hosts
+  Command group for managing hosts
 
 Options:
   -h, --help  Show this message and exit.
 
 Commands:
-  create  Create new host configuration
-  delete  Delete host from configuration
-  list    List hosts
-  set     Changes/sets host configuration parameters
-  show    Display info for host
-  test    Test SSH host connection
+  create   Create new host
+  delete   Delete host(s)
+  install  Install SSH key to hosts (experimental)
+  list     List configured hosts
+  rename   Rename existing host
+  set      Set/Change host configuration
+  show     Show current host configuration
+  test     Test SSH host connection  (experimental)
 ```
 
 ### Output styling and user ENV variables
 
 `sshc host show` can display host output is several formats, you can specify it with `sshc host show <host> --style <style>`  
 Available styles are:
 
@@ -286,55 +289,63 @@
 
 
 #-------------------------------------------------------------------------------
 #@group: jumphost
 #@desc: Edge-server / SSH bastion
 #@info: Used for jump-proxy from intnet to internal lab servers
 #-------------------------------------------------------------------------------
+#@host: This host can be used as proxyjump to reach LAB servers
 Host jumper1
     hostname 123.123.123.123
     user master
     port 1234
 
 
 #-------------------------------------------------------------------------------
 #@group: lab-servers
 #@desc: Testing/Support servers
 #@info: Some [red]important[/] detail here!
 #@info: We can have color markups in descriptions and info lines
 #-------------------------------------------------------------------------------
+#@host: This server is [red]not[/] reachable directly, only via [green]jumper1[/]
 Host lab-serv1
     hostname 10.10.0.1
     user admin
 
+#@host: This server is [red]not[/] reachable directly, only via [green]jumper1[/]
 Host lab-serv2
-    hostname 10.16.141
-
-Host lab-*
-    user user123
-    proxyjump jumper1
+    hostname 10.10.0.2
 
+#@host: This server is [red]not[/] reachable directly, only via [green]lab-serv1[/]
+#@host: SSHClick can represent how end-to-end tunels will be established
 Host server-behind-lab
     hostname 10.30.0.1
     user testuser
     port 1234
     proxyjump lab-serv1
+    localforward 7630 127.0.0.1:7630
 
-```
+#@host: This pattern applies to all hosts starting with 'lab-'
+#@host: setting 'user' and 'proxyjump' property
+Host lab-*
+    user user123
+    proxyjump jumper1
 
+```
+<!-- 
 ### Demo showing some `sshc group` operations:
 [![asciicast](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89.svg)](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89)
 
 
 ### Demo showing some `sshc host` operations:
 [![asciicast](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA.svg)](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA)
 
 
 ### Demo displaying "end-to-end" tunnel visualization in graph
-[![asciicast](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE.svg)](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE)
+[![asciicast](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE.svg)](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE) -->
 
 
 ## Author
 
 Karlo Tisaj  
 email: karlot@gmail.com  
 github: https://github.com/karlot
```

### Comparing `sshclick-0.4.4/pyproject.toml` & `sshclick-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# !!! Remember to update version here and in the code !!! 
+# (ಠ_ಠ)  -- I wish poetry could just read version from the package
+
 [tool.poetry]
 name = "sshclick"
 homepage = "https://github.com/karlot/sshclick"
-version = "0.4.4"
+version = "0.5.0"
 description = "SSH Config manager"
 authors = ["Karlo Tisaj <karlot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -17,21 +20,21 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-click = "^8.1.3"
-prettytable = "^3.2.0"
-rich = "^12.5.1"
+click = "^8.1"
+prettytable = "^3.7"
+rich = "^13.3"
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.3"
 
 
 [tool.poetry.scripts]
 sshc = "sshclick.main:cli"
 
 
 [build-system]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sshclick-0.4.4/sshclick/cmds/cmd_group.py` & `sshclick-0.5.0/sshclick/cmds/cmd_group.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import click
 
 #------------------------------------------------------------------------------
 # GROUP Commands
 #------------------------------------------------------------------------------
-@click.group(name="group")
+@click.group(name="group", help="Command group for managing groups")
 def ssh_group():
-    """
-    Manage groups
-    """
+    pass
 
 #// Linking other sub-commands
-from .group import group_create, group_delete, group_list, group_set, group_show
+from .group import group_create, group_delete, group_list, group_set, group_show, group_rename
 ssh_group.add_command(group_create.cmd)
 ssh_group.add_command(group_delete.cmd)
 ssh_group.add_command(group_list.cmd)
 ssh_group.add_command(group_set.cmd)
 ssh_group.add_command(group_show.cmd)
+ssh_group.add_command(group_rename.cmd)
```

### Comparing `sshclick-0.4.4/sshclick/cmds/group/group_create.py` & `sshclick-0.5.0/sshclick/cmds/group/group_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import click
 from sshclick.sshc import SSH_Config, SSH_Group
 
 #------------------------------------------------------------------------------
 # COMMAND: group create
 #------------------------------------------------------------------------------
-@click.command(name="create", help="Create new group")
-@click.option("-d", "--desc", default=None, type=str, help="Short description of group")
-@click.option("-i", "--info", default=[], multiple=True, type=str, help="Info line, can be set multiple times")
+SHORT_HELP = "Create new group"
+LONG_HELP  = """
+Create new group
+
+Group is used as visual and searchable separation between hosts.
+It is achieved trough readable comments with special comment keyword
+defining start of the group "#@group: <group-name>", every host defined
+after this keyword is considered as part of this group.
+"""
+
+# Parameters help:
+DESC_HELP  = "Short description of group"
+INFO_HELP  = "Info line, can be set multiple times"
+#------------------------------------------------------------------------------
+
+@click.command(name="create", short_help=SHORT_HELP, help=LONG_HELP)
+@click.option("-d", "--desc", default="", help=DESC_HELP)
+@click.option("-i", "--info", multiple=True, help=INFO_HELP)
 @click.argument("name")
 @click.pass_context
 def cmd(ctx, name, desc, info):
     config: SSH_Config = ctx.obj
 
     # Check if already group exists
-    found_group = config.find_group_by_name(name, throw_on_fail=False)
-    if found_group:
+    if not config.check_group_by_name(name):
         print(f"Cannot create new group '{name}', as group already exists with this name")
         ctx.exit(1)
 
-    new_group = SSH_Group(name, desc=desc, info=info)
+    new_group = SSH_Group(name, desc=desc, info=list(info))
 
     # Add new group to config and show newly created group
     config.groups.append(new_group)
-    
     config.generate_ssh_config().write_out()
+
     if not config.stdout:
         print(f"Created group: {name}")
-
```

### Comparing `sshclick-0.4.4/sshclick/cmds/group/group_list.py` & `sshclick-0.5.0/sshclick/cmds/group/group_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,29 @@
 from rich.console import Console
 from rich.table import Table
 from rich import box
 
 #------------------------------------------------------------------------------
 # COMMAND: group list
 #------------------------------------------------------------------------------
-@click.command(name="list", help="Lists all groups")
+SHORT_HELP = "Lists all groups"
+LONG_HELP  = SHORT_HELP
+
+# Parameters help:
+#------------------------------------------------------------------------------
+
+@click.command(name="list", short_help=SHORT_HELP, help=LONG_HELP)
 @click.pass_context
 def cmd(ctx):
     config: SSH_Config = ctx.obj
 
     table = Table(box=box.SQUARE, style="grey35")
     table.add_column("Name", style="white")
-    table.add_column("Num.Hosts", justify="right", style="bright_yellow")
-    table.add_column("Desc", style="gray50")
+    table.add_column("#Hosts", justify="right", style="bright_yellow")
+    table.add_column("#Patterns", justify="right", style="bright_cyan")
+    table.add_column("Desc", style="grey50")
 
     for group in config.groups:
-        table.add_row(group.name, str(len(group.hosts)), group.desc)
+        table.add_row(group.name, str(len(group.hosts)), str(len(group.patterns)), group.desc)
 
     console = Console()
     console.print(table)
```

### Comparing `sshclick-0.4.4/sshclick/cmds/group/group_set.py` & `sshclick-0.5.0/sshclick/cmds/group/group_delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 import click
-from sshclick.sshc import SSH_Config, complete_ssh_group_names
-
-#TODO: Check click.edit for multiline edit option (info, or even params?)
+from sshclick.sshc import SSH_Config
+from sshclick.sshc import complete_ssh_group_names, expand_names
 
 #------------------------------------------------------------------------------
-# COMMAND: group-set
+# COMMAND: group delete
+#------------------------------------------------------------------------------
+SHORT_HELP = "Delete group"
+LONG_HELP  = """
+Delete group
+
+Command accepts single or multiple groups names to delete.
+If autocompletion is enabled, command will also offer current configured groups for TAB completion.
+Alternatively when group "NAME" is specified with "r:" prefix, then value is used as regex match
+to find all group names that match given pattern, and will expand target group list accordingly.
+
+Regex matches and direct or autocompleted names can be mixed.
+Group deletion will be prompted for confirmation.
+"""
+
+# Parameters help:
+YES_HELP   = "Skip confirmation and assume 'yes'. Be careful!"
 #------------------------------------------------------------------------------
-@click.command(name="set", help="Change group parameters")
-@click.option("-r", "--rename", default=None, help="Rename group")
-@click.option("-d", "--desc", default=None, help="Set description")
-@click.option("-i", "--info", default=None, multiple=True, help="Set info, can be set multiple times")
-@click.argument("name", shell_complete=complete_ssh_group_names)
+
+@click.command(name="delete", short_help=SHORT_HELP, help=LONG_HELP)
+@click.option("--yes", is_flag=True, help=YES_HELP)
+@click.argument("names", nargs=-1, required=True, shell_complete=complete_ssh_group_names)
 @click.pass_context
-def cmd(ctx, name, rename, desc, info):
+def cmd(ctx, names, yes):
     config: SSH_Config = ctx.obj
 
-    # Nothing was provided
-    if not rename and not desc and not info:
-        print("Calling set on group without specifying any option is not valid!")
-        print("Run 'sshc group set -h' for help.")
-        ctx.exit(1)
-
-    # Find group by name
-    found_group = config.find_group_by_name(name, throw_on_fail=False)
-    if not found_group:
-        print(f"Cannot modify group '{name}', it is not defined in configuration!")
-        ctx.exit(1)
-
-    if rename:
-        found_group.name = rename
-    
-    if desc:
-        found_group.desc = desc
-
-    if info:
-        if len(info[0]) > 0:
-            found_group.info = info
-        else:
-            found_group.info = []
-
-    config.generate_ssh_config().write_out()
-    if not config.stdout:
-        print(f"Modified group: {name}")
+    selected_group_list = expand_names(names, config.get_all_group_names())
+    selected_group_list.sort()
+
+    # Deleting requires confirmation
+    if not yes:
+        print(f"Following groups will be deleted: [{','.join(selected_group_list)}]")
+        if not click.confirm('Are you sure?'):
+            ctx.exit(1)
+
+    # When deleting multiple groups, iterate over all of them
+    config_updated = False
+    for name in selected_group_list:
+
+        # Find group by name
+        if not config.check_group_by_name(name):
+            print(f"Cannot delete group '{name}', it is not defined in configuration!")
+            continue
+
+        config.groups.remove(config.get_group_by_name(name))
+        config_updated = True
+
+        if not config.stdout:
+            print(f"Deleted group: {name}")
+
+    # ReWrite config only when config was actually changed
+    if config_updated:
+        config.generate_ssh_config().write_out()
```

### Comparing `sshclick-0.4.4/sshclick/cmds/group/group_show.py` & `sshclick-0.5.0/sshclick/cmds/group/group_show.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 import click
-from sshclick.sshc import SSH_Config, complete_ssh_group_names
+from typing import List
+
+from sshclick.sshc import SSH_Config
+from sshclick.sshc import complete_ssh_group_names
 
 from rich.table import Table
 from rich.panel import Panel
 from rich import box
 from rich.console import Console
 
 #------------------------------------------------------------------------------
 # COMMAND: group show
 #------------------------------------------------------------------------------
-@click.command(name="show", help="Shows group details")
+SHORT_HELP = "Shows group details"
+LONG_HELP  = """
+Display/Shows details from a group
+
+Currently WIP - command will allow some styles in outputs...
+"""
+
+# Parameters help:
+#------------------------------------------------------------------------------
+
+@click.command(name="show", short_help=SHORT_HELP, help=LONG_HELP)
 @click.argument("name", shell_complete=complete_ssh_group_names)
 @click.pass_context
 def cmd(ctx, name):
     config: SSH_Config = ctx.obj
 
-    found_group = config.find_group_by_name(name, throw_on_fail=False)
-    if not found_group:
+    if not config.check_group_by_name(name):
         print(f"Cannot show group '{name}', it is not defined in configuration!")
         ctx.exit(1)
 
-    host_list = []
+    found_group = config.get_group_by_name(name)
+    host_list: List[str] = []
+
     for host in found_group.hosts:
         if "hostname" in host.params:
             h_name = host.params["hostname"]
             h_port = (":" + host.params["port"]) if "port" in host.params else ""
             host_list.append(f"{host.name} ({h_name}{h_port})")
         else:
             host_list.append(host.name)
 
-    pattern_list = []
+    pattern_list: List[str] = []
     for host in found_group.patterns:
         # hack to search via case insensitive info
         if "hostname" in host.params:
             h_name = host.params["hostname"]
             pattern_list.append(f"{host.name} ({h_name})")
         else:
             pattern_list.append(host.name)
```

### Comparing `sshclick-0.4.4/sshclick/cmds/host/host_delete.py` & `sshclick-0.5.0/sshclick/cmds/group/group_rename.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import click
-from sshclick.sshc import SSH_Config, complete_ssh_host_names
+from sshclick.sshc import SSH_Config
+from sshclick.sshc import complete_ssh_group_names
 
 #------------------------------------------------------------------------------
-# COMMAND: host delete
+# COMMAND: group rename
 #------------------------------------------------------------------------------
-@click.command(name="delete", help="Delete host from configuration")
-@click.argument("name", shell_complete=complete_ssh_host_names)
+SHORT_HELP = "Rename existing group"
+LONG_HELP  = "Rename existing group in configuration"
+
+#------------------------------------------------------------------------------
+
+@click.command(name="rename", short_help=SHORT_HELP, help=LONG_HELP)
+@click.argument("name", shell_complete=complete_ssh_group_names)
+@click.argument("new_name")
 @click.pass_context
-def cmd(ctx, name):
+def cmd(ctx, name, new_name):
     config: SSH_Config = ctx.obj
 
-    found_host, found_group = config.find_host_by_name(name, throw_on_fail=False)
-    if not found_host:
-        print(f"Cannot delete host '{name}' as it is not defined in configuration!")
+    if not config.check_group_by_name(name):
+        print(f"Cannot rename group '{name}', as it is not defined in configuration!")
+        ctx.exit(1)
+    if config.check_group_by_name(new_name):
+        print(f"Cannot rename group '{name}' to '{new_name}' as new name is already used!")
         ctx.exit(1)
-    
-    if found_host.type == "normal":
-        found_group.hosts.remove(found_host)
-    else:
-        found_group.patterns.remove(found_host)
 
+    config.get_group_by_name(name).name = new_name
     config.generate_ssh_config().write_out()
+    
     if not config.stdout:
-        print(f"Deleted host: {name}")
+        print(f"Renamed group: {name} -> {new_name}")
```

### Comparing `sshclick-0.4.4/sshclick/cmds/host/host_list.py` & `sshclick-0.5.0/sshclick/cmds/host/host_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 import click
-import re
-import copy
-from sshclick.sshc import SSH_Config, SSH_Group, SSH_Host
+from typing import List
+from sshclick.sshc import SSH_Config, SSH_Host
 
 from rich.console import Console
 from rich.table import Table
 from rich import box
-
 console = Console()
 
 #------------------------------------------------------------------------------
 # COMMAND: host-list
 #------------------------------------------------------------------------------
-@click.command(name="list", help="List hosts")
-@click.option("-g", "--group",  "group_filter", default=None,  help="Filter for group that host belongs to (regex)")
-@click.option("-n", "--name",   "name_filter",  default=None,  help="Filter for host name (regex)")
-@click.option("-v", "--verbose", is_flag=True,  default=False, help="Show verbose info (all parameters)")
+SHORT_HELP = "List configured hosts"
+LONG_HELP  = """
+List hosts from current configuration
+
+Command allows displaying hosts with various properties, and filtering output list for easier searching.
+SSHC will display also usually not visible "INHERITANCE" of parameters trough "PATTERNS", and from
+which pattern parameter for given host would be applied (inherited).
+
+Normal output will try to show only most important information about listed hosts, while if requested,
+VERBOSE option will try to show ALL defined/inherited parameters for all listed hosts.
+Alternatively for details on only single host, use "sshc host show" command.
+
+Host list can be limited with filters, to only show specific hosts that match NAME regex or GROUP regex.
+When both NAME and GROUP regex are defined, output must satisfy both filters.
+"""
+
+# Parameters help:
+GROUP_HELP   = "Filter for host groups (regex)"
+NAME_HELP    = "Filter for host names (regex)"
+VERBOSE_HELP = "Show verbose info (all parameters)"
+#------------------------------------------------------------------------------
+
+@click.command(name="list", short_help=SHORT_HELP, help=LONG_HELP)
+@click.option("-g", "--group",  "group_filter", help=GROUP_HELP)
+@click.option("-n", "--name",   "name_filter",  help=NAME_HELP)
+@click.option("-v", "--verbose", is_flag=True,  help=VERBOSE_HELP)
 @click.pass_context
 def cmd(ctx, group_filter, name_filter, verbose):
     config: SSH_Config = ctx.obj
 
     # Filter out groups and hosts if filters are defined via CLI
-    filtered_groups: list[SSH_Group] = []
-    for group in config.groups:
-        # If group filter is defined, check if current group matches the name to progress
-        if group_filter:
-            group_match = re.search(group_filter, group.name)
-            if not group_match:
-                continue
-        
-        # When group is not skipped, check if name filter is used, and filter out groups
-        if name_filter:
-            # Make a new copy of group, so we dont mess original config
-            group_copy = copy.copy(group)
-            group_copy.hosts = []
-            group_copy.patterns = []
-            include_group = False
-
-            for host in group.hosts + group.patterns:
-                match = re.search(name_filter, host.name)
-                if match:
-                    include_group = True
-                    if host.type == "normal":
-                        group_copy.hosts.append(host)
-                    else:
-                        group_copy.patterns.append(host)
-            if include_group:
-                filtered_groups.append(group_copy)
-        else:
-            filtered_groups.append(group)
+    filtered_groups = config.filter_config(group_filter, name_filter)
 
     if not filtered_groups:
         print("No host is matching any given filter!")
         ctx.exit(1)
     
     # This lists define host properties and which parameters will be displayed
     host_props = ["name", "group", "type"]
     params     = ["hostname", "user"]
 
     # If output is verbose, we need to find all parameters, and add them to params list
     if verbose:
-        flat_config: list[SSH_Host] = []
+        flat_config: List[SSH_Host] = []
         for group in filtered_groups:
             for h in group.hosts + group.patterns:
                 flat_config.append(h)
         for host in flat_config:
             for i_params in host.params:
                 if (not i_params in params):
                     params.append(i_params)
@@ -72,30 +65,27 @@
     header = host_props + ([f"param:{p}" for p in params])
     table = Table(*header, box=box.SQUARE, style="gray35")
 
     # Start adding rows    
     for group in filtered_groups:
         # Iterate trough hosts and patters
         for host in group.hosts + group.patterns:
-            inherited: list[tuple[str, dict]] = []
-            if host.type == "normal":
-                inherited = config.find_inherited_params(host.name)
             host_params = []
             # Go trough list of all params we know are available across current host list
             for table_param in params:
                 if table_param in host.params:
                     # Handle direct params, and handle if its a list or string
                     if isinstance(host.params[table_param], list):
                         host_params.append("\n".join(host.params[table_param]))
                     else:
                         host_params.append(host.params[table_param])
                 else:
                     # Handle inherited params (only valid for "normal" hosts)
-                    if inherited:
-                        for pattern, i_params in inherited:
+                    if host.inherited_params:
+                        for pattern, i_params in host.inherited_params:
                             if table_param in i_params:
                                 if isinstance(i_params[table_param], list):
                                     table_param = "\n".join([f"{val}  ({pattern})" for val in i_params[table_param]])
                                     host_params.append(table_param)
                                 else:
                                     host_params.append(f"[yellow]{i_params[table_param]}  ({pattern})[/]")
                             else:
```

### Comparing `sshclick-0.4.4/sshclick/cmds/host/host_test.py` & `sshclick-0.5.0/sshclick/cmds/host/host_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import click
 import subprocess
 from sshclick.sshc import SSH_Config, complete_ssh_host_names
 
 #------------------------------------------------------------------------------
-# COMMAND: host connect
+# COMMAND: host test
 #------------------------------------------------------------------------------
-@click.command(name="test", help="Test SSH host connection")
-@click.option("--timeout", default=3, help="Timeout for SSH connection")
+SHORT_HELP = "Test SSH host connection  (experimental)"
+LONG_HELP  = """
+Test SSH host connectivity end-to-end
+
+NOTE: This command is experimental and might change or be removed in future
+"""
+
+# Parameters help:
+TIME_HELP  = "Timeout for SSH connection"
+#------------------------------------------------------------------------------
+
+@click.command(name="test", short_help=SHORT_HELP, help=LONG_HELP)
+@click.option("--timeout", default=3, help=TIME_HELP)
 @click.argument("name", shell_complete=complete_ssh_host_names)
 @click.pass_context
-def cmd(ctx, name, timeout):
+def cmd(ctx: click.core.Context, name: str, timeout: int):
     config: SSH_Config = ctx.obj
 
-    found_host, _ = config.find_host_by_name(name, throw_on_fail=False)
+    found_host, _ = config.get_host_by_name(name)
     if not found_host:
         print(f"Cannot test host '{name}' as it is not defined in configuration!")
         ctx.exit(1)
 
     hostname = found_host.params["hostname"]
 
     #// SSH Command method via subprocess
     #------------------------------------------------
     ssh_command = f"ssh -q -o StrictHostKeyChecking=no -o ConnectTimeout={timeout} {name} 'exit 0'"
     response = subprocess.run(ssh_command, shell=True)
     
-    print(f"Connection with SSH Host name: {name} ({hostname}) ", end="")
+    print(f"Connection to: {name} ({hostname}) ", end="")
     if response.returncode == 0:
         print("successful!")
         ctx.exit()
     else:
         print("failed!")
         ctx.exit(1)
```

### Comparing `sshclick-0.4.4/sshclick/sshc/host_styles/card.py` & `sshclick-0.5.0/sshclick/sshc/host_styles/card.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 from rich import box
 
 #------------------------------------------------------------------------------
 # Render host data in panel with single-card look
 #------------------------------------------------------------------------------
 def render(host: SSH_Host):
     out_type = host.type if host.type == "normal" else f"[cyan]{host.type}[/]"
-    out_info = "\n".join(host.info) if host.info else "- No info defined - "
 
+    #// Add Host data information
+    #// -----------------------------------------------------------------------
     layout_table = Table("", box=box.ROUNDED, style="grey35" ,show_edge=True, show_header=False)
     layout_table.add_row(f"[bright_white]Name [/]:  {host.name}")
     layout_table.add_row(f"[bright_white]Group[/]:  {host.group}")
     layout_table.add_row(f"[bright_white]Type [/]:  {out_type}")
 
+    #// Add Host info panel (if host info exist)
+    #// -----------------------------------------------------------------------
     if host.info:
         layout_table.add_row("")
+        out_info = "\n".join(host.info)
         layout_table.add_row(f"[gray50]{out_info}[/]")
 
     layout_table.add_row("")
 
+    #// Prepare table with params and append it to the layout table
+    #// -----------------------------------------------------------------------
     param_table = Table(box=box.SIMPLE, style="grey35", show_header=True, show_edge=False, pad_edge=False)
     param_table.add_column("Param")
     param_table.add_column("Value")
     param_table.add_column("Inherited-from")
 
     # Add rows for SSH Config parameters
     for key, value in host.params.items():
@@ -36,10 +42,11 @@
     for pattern, pattern_params in host.inherited_params:
         for param, value in pattern_params.items():
             if not param in host.params:
                 output_value = value if not isinstance(value, list) else "\n".join(value)
                 param_table.add_row(param, output_value, pattern, style="yellow")
 
     layout_table.add_row(param_table)
-    wrapper_panel = Panel(layout_table, box=box.SIMPLE, padding=(0,0))
 
-    return wrapper_panel
+    #// Render output
+    #// -----------------------------------------------------------------------
+    return Panel(layout_table, box=box.SIMPLE, padding=(0,0))
```

### Comparing `sshclick-0.4.4/sshclick/sshc/host_styles/panels.py` & `sshclick-0.5.0/sshclick/sshc/host_styles/simple.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from textwrap import dedent
 from ..ssh_host import SSH_Host
 
 from rich.table import Table
 from rich.panel import Panel
 from rich.console import Group
 from rich import box
 
 #------------------------------------------------------------------------------
-# Render host data in panels with separate sections
+# Render host data in panel without borders and minimal decorations
 #------------------------------------------------------------------------------
 def render(host: SSH_Host):
     out_type = host.type if host.type == "normal" else f"[cyan]{host.type}[/]"
-    out_info = "\n".join(host.info) if host.info else "- No info defined - "
 
-    panel_data = f"""\
-    [bright_white]Name [/]:  {host.name}
-    [bright_white]Group[/]:  {host.group}
-    [bright_white]Type [/]:  {out_type}\
-    """
-    host_panel = Panel(dedent(panel_data), border_style="grey35", title="Host", title_align="left")
-    info_panel = Panel(out_info,           border_style="grey35", style="gray50", title="Info", title_align="left")
-
-    param_table = Table(box=box.ROUNDED, style="grey35", show_header=True, show_edge=True, expand=True)
+    #// Add Host data information
+    #// -----------------------------------------------------------------------
+    panel_data = [
+        f"[bright_white]Name [/]:  {host.name}",
+        f"[bright_white]Group[/]:  {host.group}",
+        f"[bright_white]Type [/]:  {out_type}",
+    ]
+    
+    #// Add Host info data (if host info exist)
+    #// -----------------------------------------------------------------------
+    if host.info:
+        out_info = "\n".join(host.info)
+        panel_data = panel_data + [
+            f"",
+            f"[gray50]{out_info}[/]",
+        ]
+    host_panel = Panel("\n".join(panel_data), box=box.SIMPLE, border_style="grey35", padding=(0,0))
+
+    #// Prepare table with params
+    #// -----------------------------------------------------------------------
+    param_table = Table(box=box.SIMPLE, style="grey35", show_header=True, show_edge=False, pad_edge=True)
     param_table.add_column("Param")
     param_table.add_column("Value")
     param_table.add_column("Inherited-from")
 
     # Add rows for SSH Config parameters
     for key, value in host.params.items():
         output_value = value if not isinstance(value, list) else "\n".join(value)
@@ -34,10 +44,12 @@
     # Add rows for inherited SSH Config parameters
     for pattern, pattern_params in host.inherited_params:
         for param, value in pattern_params.items():
             if not param in host.params:
                 output_value = value if not isinstance(value, list) else "\n".join(value)
                 param_table.add_row(param, output_value, pattern, style="yellow")
 
-    panel_group = Group(host_panel, info_panel, param_table) if host.info else Group(host_panel, param_table)
-
-    return Panel.fit(panel_group, box=box.SIMPLE, padding=(0,0))
+    param_table.add_row("")
+    
+    #// Render output
+    #// -----------------------------------------------------------------------
+    return Group(host_panel, param_table)
```

### Comparing `sshclick-0.4.4/sshclick/sshc/host_styles/simple.py` & `sshclick-0.5.0/sshclick/sshc/host_styles/table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 from ..ssh_host import SSH_Host
 
 from rich.table import Table
-from rich.panel import Panel
-from rich.console import Group
 from rich import box
 
 #------------------------------------------------------------------------------
-# Render host data in panel without borders and minimal decorations
+# Render host data in single flat 3-column table
 #------------------------------------------------------------------------------
 def render(host: SSH_Host):
     out_type = host.type if host.type == "normal" else f"[cyan]{host.type}[/]"
     out_info = "\n".join(host.info) if host.info else "- No info defined - "
 
-    panel_data = [
-        f"[bright_white]Name [/]:  {host.name}",
-        f"[bright_white]Group[/]:  {host.group}",
-        f"[bright_white]Type [/]:  {out_type}",
-    ]
-    if host.info:
-        panel_data = panel_data + [
-            f"",
-            f"[gray50]{out_info}[/]",
-        ]
-    host_panel = Panel("\n".join(panel_data), box=box.SIMPLE, border_style="grey35", padding=(0,0))
-
-    param_table = Table(box=box.SIMPLE, style="grey35", show_header=True, show_edge=False, pad_edge=True)
-    param_table.add_column("Param")
-    param_table.add_column("Value")
-    param_table.add_column("Inherited-from")
-
+    table = Table(box=box.SQUARE, style="grey39")
+    table.add_column("Parameter")
+    table.add_column("Value")
+    table.add_column("Inherited-from")
+    
+    table.add_row("Name",  host.name)
+    table.add_row("Group", host.group)
+    table.add_row("Type",  out_type)
+    table.add_row("Info",  out_info, style="grey50")
+    
     # Add rows for SSH Config parameters
     for key, value in host.params.items():
         output_value = value if not isinstance(value, list) else "\n".join(value)
-        param_table.add_row(key, output_value)
+        table.add_row(f"Param:{key}", output_value)
 
     # Add rows for inherited SSH Config parameters
     for pattern, pattern_params in host.inherited_params:
         for param, value in pattern_params.items():
             if not param in host.params:
                 output_value = value if not isinstance(value, list) else "\n".join(value)
-                param_table.add_row(param, output_value, pattern, style="yellow")
-
-    param_table.add_row("")
-    panel_group = Group(host_panel, param_table)
+                table.add_row(f"param:{param}", output_value, pattern, style="yellow")
     
-    return panel_group
+    return table
+
```

### Comparing `sshclick-0.4.4/sshclick/sshc/host_styles/table2.py` & `sshclick-0.5.0/sshclick/sshc/host_styles/table2.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.4.4/sshclick/sshc/ssh_config.py` & `sshclick-0.5.0/sshclick/sshc/ssh_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import re
-import fnmatch
-
-from ..globals import *
-from .ssh_host import SSH_Host
-from .ssh_group import SSH_Group
+import re, fnmatch, copy
+from typing import List, Optional, Tuple
 
 import logging
 logging.basicConfig(level=logging.INFO)
 
+from .ssh_host import SSH_Host
+from .ssh_group import SSH_Group
+from .ssh_parameters import PARAMS_WITH_ALLOWED_MULTIPLE_VALUES
+
 class SSH_Config:
     """
     SSH Configuration class
 
     Main class for handling SSH configuration, reading from file, parsing and
     generating and writing contents back to SSH configuration file
     """
+    DEFAULT_GROUP_NAME: str = "default"
 
-    def __init__(self, file: str, config_lines: list = [], stdout: bool = DEFAULT_STDOUT):
+    def __init__(self, file: str, config_lines: List[str] = [], stdout: bool = False):
         self.ssh_config_file: str = file
-        self.ssh_config_lines: list = config_lines
+        self.ssh_config_lines: List[str] = config_lines
 
         # configuration representation (array of SSH groups?)
-        self.groups: list = [SSH_Group(name=DEFAULT_GROUP_NAME, desc="Default group")]
+        self.groups: List[SSH_Group] = [SSH_Group(name=self.DEFAULT_GROUP_NAME, desc="Default group")]
 
         # options
         self.stdout: bool = stdout
+        self.opts: dict = {}
 
         # parsing "cache" info
         self.current_grindex: int = 0
-        self.current_group: str = DEFAULT_GROUP_NAME
-        self.current_host: SSH_Host = None
+        self.current_group: str = self.DEFAULT_GROUP_NAME
+        self.current_host: Optional[SSH_Host] = None
         self.current_host_info: list = []
 
 
     def read(self):
         """
         Read content of SSH config file
         """
@@ -51,37 +53,48 @@
                 self.groups[self.current_grindex].hosts.append(self.current_host)
             else:
                 self.groups[self.current_grindex].patterns.append(self.current_host)
             # Reset "cache" since we flushed host info
             self.current_host = None
 
 
+    # TODO: Add ability to separate host parameters with optional "=" sign
     def parse(self):
         """
         Parse config lines one by one and generate configuration structure
         """
         # Parse each line of the configuration, line by line
         for config_line_index, line in enumerate(self.ssh_config_lines):
             line = line.strip()     # remove start and end whitespace
 
             # Skip empty lines, go to next...
             if not line:
                 continue
             
-            # Process special metadata for grouping: "#@group", "#@desc", "#@info"
-            if line.startswith("#@"):
-                match = re.search(r"^#@(\w+):\s*(.+)$", line)
+            # Reworked parsing method... special "meta" keys not needed, regex now parses words
+            # so its much more "freely" in reading from config file writing is still in legacy style
+            # in future, output config write styles could be changed... 
+            if line.startswith("#"):
+                match = re.search(r"^#[\s@]*(group|desc|info|host|config)[\s:]+(.+)$", line)
 
                 # In case special comment is unreadable
                 if not match:
-                    logging.warning(f"META: Unmatched metadata line {line} on SSH-config line number {config_line_index}")
+                    logging.debug(f"DROP COMMENT: '{line}'")
                     continue
                 
                 metadata, value = match.groups()
-                if metadata == "group":
+
+                if metadata == "config":
+                    # Config options are configured as key=value within config line...
+                    logging.debug(f"META: Config line found '{value}' Caching for next host definition...'")
+                    conf_key, conf_val = value.split("=")
+                    self.opts[conf_key] = conf_val
+                    continue
+
+                elif metadata == "group":
                     # New group found... flush any previous data and create new baseline
                     self._config_flush_host()
 
                     logging.debug(f"META: Starting new group: {value}")
                     self.groups.append(SSH_Group(name=value))
 
                     self.current_grindex = len(self.groups) - 1
@@ -101,22 +114,17 @@
 
                 elif metadata == "host":
                     logging.debug(f"META: Host comment found '{value}' Caching for next host definition...'")
                     self.current_host_info.append(value)
                     continue
 
                 else:
-                    logging.warning(f"META: Unhandled metadata metadata '{metadata}' on SSH-config line number {config_line_index}")
+                    logging.warning(f"META: Unhandled metadata '{metadata}' on SSH-config line number: {config_line_index}")
                     continue
 
-            # Ignore rest of commented lines
-            if line.startswith("#"):
-                logging.debug(f"DROP COMMENT: '{line}'")
-                continue
-
             # Here we expect only normal ssh config lines "Host" is usually the keyword that begins definition
             # if we find any other keyword before first host keyword is defined, configuration is wrong probably
             match = re.search(r"^(\w+)\s+(.+)$", line)
             if not match:
                 logging.warning(f"KEYWORD: Incorrect configuration line '{line}' on SSH-config line number {config_line_index}")
                 continue
 
@@ -151,52 +159,69 @@
                             self.current_host.params[keyword].append(value)
                     else:
                         self.current_host.params[keyword] = value
                         continue
         
         # Last entries must be flushed manually as there are no new "hosts" to trigger storing parsed data into config struct
         self._config_flush_host()
+
+        # Second stage, check any inheritances and fill them
+        # start = time.time()
+        for group in self.groups:
+            for host in group.hosts:
+                inherited_params: List[Tuple[str, dict]] = []
+                if host.type == "normal":
+                    inherited_params = self.find_inherited_params(host.name)
+                    host.inherited_params = inherited_params
+        # end = time.time() - start
+        # print(f"Inheritance check elapsed: {end:0.3f}s")
         return self
 
 
     def generate_ssh_config(self):
         """
         SSH config generation function
 
         Function takes config data structure, and target file information.
         Then generates SSH config compatible file with all data, compatible with
         internal object model.
         """
         SSHCONFIG_INDENT = "    "
+        SSHCONFIG_META_PREFIX = "@"
+        SSHCONFIG_META_SEPARATOR = ": "
 
         # First we lines before we flush them into file
-        lines = ["#<<<<< SSH Config file managed by sshclick >>>>>\n"]
+        lines: List[str] = ["#<<<<< SSH Config file managed by sshclick >>>>>\n"]
+
+        # Dump any saved configuration
+        for option in self.opts:
+            lines.append(f"#{SSHCONFIG_META_PREFIX}config{SSHCONFIG_META_SEPARATOR}{option}={self.opts[option]}\n")
 
         for group in self.groups:
             # Ship default group as it does not have to be specified
-            render_header = False if group.name == DEFAULT_GROUP_NAME else True
+            render_header = False if group.name == self.DEFAULT_GROUP_NAME else True
             
             if render_header:
                 # Add extra blank line when outputting new group header
                 lines.append("\n")
                 # Start header line for the group with known metadata
                 lines.append(f"#{'-'*79}\n")        # add horizontal decoration line
-                lines.append(f"#@group: {group.name}\n")
+                lines.append(f"#{SSHCONFIG_META_PREFIX}group{SSHCONFIG_META_SEPARATOR}{group.name}\n")
                 if group.desc:
-                    lines.append(f"#@desc: {group.desc}\n")
+                    lines.append(f"#{SSHCONFIG_META_PREFIX}desc{SSHCONFIG_META_SEPARATOR}{group.desc}\n")
                 for info in group.info:
-                    lines.append(f"#@info: {info}\n")
+                    lines.append(f"#{SSHCONFIG_META_PREFIX}info{SSHCONFIG_META_SEPARATOR}{info}\n")
                 lines.append(f"#{'-'*79}\n")        # add horizontal decoration line
 
             # Append hosts and patterns items from group
             for host in group.hosts + group.patterns:
                 # If there is host-info assigned to host, add it before adding "host" definition
                 for host_info in host.info:
-                    lines.append(f"#@host: {host_info}\n")
-                
+                    lines.append(f"#{SSHCONFIG_META_PREFIX}host{SSHCONFIG_META_SEPARATOR}{host_info}\n")
+
                 # Add "host" line definition
                 lines.append(f"Host {host.name}\n")
 
                 # Add all assigned host params
                 for token, value in host.params.items():
                     if type(value) is str:
                         lines.append(f"{SSHCONFIG_INDENT}{token} {value}\n")
@@ -208,93 +233,153 @@
                 
                 # Add newline after host definition
                 lines.append("\n")
             
         # Store output lines
         self.ssh_config_lines = lines
         return self
-        
 
-    def write_out(self):
+
+    def write_out(self) -> None:
         """
         Write generated SSH config to target file
         """
         if self.stdout:
             print("".join(self.ssh_config_lines))
         else:
             with open(self.ssh_config_file, "w") as out:
                 out.writelines(self.ssh_config_lines)
-        
 
-    def find_group_by_name(self, name: str, throw_on_fail: bool = True):
+
+    def check_group_by_name(self, name: str) -> bool:
+        """
+        Check if specific group name is present in configuration
+        """
+        for group in self.groups:
+            if group.name == name:
+                return True
+        return False
+
+
+    def get_group_by_name(self, name: str) -> SSH_Group:
         """
         Find group in configuration that matches the name (strict match, one only!)
         On success returns matched group, on fail depending on 'throw_on_fail' flag
         function will either return 'None' or will throw exception
         """
         for group in self.groups:
             if group.name == name:
                 return group
-        if not throw_on_fail:
-            return None
         raise Exception(f"Requested group '{name}' not found in the SSH configuration")
 
 
-    def find_host_by_name(self, name: str, throw_on_fail: bool = True):
+    def check_host_by_name(self, name: str) -> bool:
+        """
+        Check if specific host name is present in configuration
+        """
+        for group in self.groups:
+            all_hosts = group.hosts + group.patterns
+            for host in all_hosts:
+                if host.name == name:
+                    return True
+        return False
+
+
+    def get_host_by_name(self, name: str) -> Tuple[SSH_Host, SSH_Group]:
         """
         Find host in configuration that matches the name (strict match, one only!)
         On success returns host and his assigned group, on fail depending on 'throw_on_fail' flag
         function will either return ('None','None') or will throw exception
         """
-        found_host = None
-        found_group = None
-        
         for group in self.groups:
             all_hosts = group.hosts + group.patterns
             for host in all_hosts:
                 if host.name == name:
-                    found_host = host
-                    found_group = group
-        
-        if not found_host and throw_on_fail:
-            raise Exception(f"Requested host '{name}' not found in the SSH configuration")
-
-        return found_host, found_group
+                    return host, group
+        raise Exception(f"Requested host '{name}' not found in the SSH configuration")
 
 
-    def get_all_host_names(self) -> list:
+    def get_all_host_names(self) -> List[str]:
         """
         Return all host names from current configuration
         Useful for auto-completion, or for quick checking if name already exists
         """
-        all_hosts: list = []
+        all_hosts: List[str] = []
         for group in self.groups:
-            for host in group.hosts:
+            for host in group.hosts + group.patterns:
                 all_hosts.append(host.name)
         return all_hosts
 
 
-    def get_all_group_names(self) -> list:
+    def get_all_group_names(self) -> List[str]:
         """
         Return all group names from current configuration
         Useful for auto-completion, or for quick checking if name already exists
         """
-        all_groups: list = []
+        all_groups: List[str] = []
         for group in self.groups:
             all_groups.append(group.name)
         return all_groups
 
 
-    def find_inherited_params(self, host_name: str) -> list:
+    def find_inherited_params(self, host_name: str) -> List[Tuple[str,dict]]:
         """
-        Returns array of 2-item tuples, where first item is name of pattern from
+        Given a host name, finds and returns list of 2-item tuples, where first item is name of pattern from
         which params are inherited, and second item is parameters dictionary from the pattern
         """
-        inherited: list = []
+        inherited: List[Tuple[str,dict]] = []
         for group in self.groups:
             for pattern in group.patterns:
                 # Check if any one of pattern (from all groups) will match host name
                 if fnmatch.fnmatch(host_name, pattern.name):
                     inherited.append((pattern.name, pattern.params))
-
+        
         return inherited
 
+
+    def filter_config(self, group_filter: str, name_filter: str) -> List[SSH_Group]:
+        """
+        Function takes optional group and name regex, and if they are not None or empty,
+        function creates a new list of SSH groups and their SSH hosts, but with all
+        non-matching items removed.
+        """
+        filtered_groups: List[SSH_Group] = []
+        for group in self.groups:
+            # If group filter is defined, check if current group matches the name to progress
+            if group_filter:
+                group_match = re.search(group_filter, group.name)
+                if not group_match:
+                    continue
+            
+            # When group is not skipped, check if name filter is used, and filter out groups
+            if name_filter:
+                # Make a new copy of group, so we dont mess original config
+                group_copy = copy.copy(group)
+                group_copy.hosts = []
+                group_copy.patterns = []
+                include_group = False
+
+                for host in group.hosts + group.patterns:
+                    match = re.search(name_filter, host.name)
+                    if match:
+                        include_group = True
+                        if host.type == "normal":
+                            group_copy.hosts.append(host)
+                        else:
+                            group_copy.patterns.append(host)
+                if include_group:
+                    filtered_groups.append(group_copy)
+            else:
+                filtered_groups.append(group)
+        return filtered_groups
+
+
+    def move_host_to_group(self, found_host: SSH_Host, found_group: SSH_Group, target_group: SSH_Group) -> None:
+        """
+        Function that moves host from one group to other group
+        """
+        if found_host.type == "normal":
+            target_group.hosts.append(found_host)
+            found_group.hosts.remove(found_host)
+        else:
+            target_group.patterns.append(found_host)
+            found_group.patterns.remove(found_host)
```

### Comparing `sshclick-0.4.4/sshclick/sshc/ssh_host.py` & `sshclick-0.5.0/sshclick/sshc/ssh_host.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
+from ..globals import DEFAULT_HOST_STYLE
+from typing import List
 from dataclasses import dataclass, field
 import importlib
 
 from rich.console import Console
 console = Console()
 
 DEBUG_STYLES = False
 
 @dataclass
 class SSH_Host:
     """ Class for SSH host config structure """
     name: str
     group: str
     type: str = "normal"
-    info: list = field(default_factory=list)
+    info: List[str] = field(default_factory=list)
     params: dict = field(default_factory=dict)
 
     inherited_params: list = field(default_factory=list)
-    print_style: str = "panels"
+    print_style: str = DEFAULT_HOST_STYLE
 
 
     # Method for interaction with printing the object via Rich library
     # Each supported style should be located in defined folder (by default under "host_styles")
     # Each module must have "render" function, and return "rich renderable" object
     def __rich__(self):
         try:
-            # If current host "print_style" for is set to "panels", we will try
+            # If current host "print_style" is set to "panels", we will try
             # to import module from "./host_styles/panels.py"
             style = importlib.import_module(f'sshclick.sshc.host_styles.{self.print_style}')
             return style.render(self)
         except ModuleNotFoundError:
             return f"SSH_Host style [bright_red]'{self.print_style}'[/] is not implemented!"
         except Exception:
             if DEBUG_STYLES:
```

### Comparing `sshclick-0.4.4/sshclick/sshc/sshextras.py` & `sshclick-0.5.0/sshclick/sshc/sshextras.py`

 * *Files identical despite different names*

### Comparing `sshclick-0.4.4/setup.py` & `sshclick-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,388 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sshclick
+Version: 0.5.0
+Summary: SSH Config manager
+Home-page: https://github.com/karlot/sshclick
+License: MIT
+Author: Karlo Tisaj
+Author-email: karlot@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: prettytable (>=3.7,<4.0)
+Requires-Dist: rich (>=13.3,<14.0)
+Description-Content-Type: text/markdown
+
+# SSH Click Config manager (sshclick)
+
+![splash_gif](tapes/splash.gif)
+
+## Links
+
+- [Intro](https://github.com/karlot/sshclick#intro)
+- [Why?](https://github.com/karlot/sshclick#why)
+- [What does it do](https://github.com/karlot/sshclick#what-does-it-do)
+  - [Installation procedure](https://github.com/karlot/sshclick#installation-procedure)
+  - [Upgrade procedure](https://github.com/karlot/sshclick#upgrade-procedure)
+  - [Uninstall procedure](https://github.com/karlot/sshclick#uninstall-procedure)
+- [SSH Config structure](https://github.com/karlot/sshclick#ssh-config-structure-and-important-note-about-comments)
+  - [Comment blocks and metadata](https://github.com/karlot/sshclick#comment-blocks-and-metadata-in-ssh-config)
+- [Example usage and features](https://github.com/karlot/sshclick#example-usage-and-features)
+  - [Group commands and options](https://github.com/karlot/sshclick#group-commands-and-options)
+  - [Host commands and options](https://github.com/karlot/sshclick#host-commands-and-options)
+  - [Output styling and user ENV variables](https://github.com/karlot/sshclick#output-styling-and-user-env-variables)
+- [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)
+  - [sshc group operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-group-operations)
+  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations)
+- [Author](https://github.com/karlot/sshclick#author)
+- [License](https://github.com/karlot/sshclick#license)
+
+
+## Intro
+Terminal based assisted management of your SSH config files.  
+Built out of boredom with managing messy and huge ssh_config files.  
+
+EARLY VERSION, backup your SSH config files before using!  
+SSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config!  
+
+**Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**
+
+## Why?
+
+What am I trying to solve with this tool?
+* I need something that works fast and great in terminal, and does not require complex setup.
+* Managing some other configuration files that renders to SSH config is extra step that I don't like.
+* SSH config is already feature-full with all options SSH client support, why inventing extra layer?
+* SSH config is the only config I need to backup.
+* I need quick way to search, group and visualize all hosts inside SSH configuration (especially since it can grow huge)
+
+
+## What does it do?
+
+SSHClick (sshc) is just a tool designed to work with existing SSH configuration files on your Linux/Windows/WSL terminal environment.  
+It basically parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.
+Trough additional "magic" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.
+
+
+### Installation procedure
+
+Should be straight forward...  
+
+1. **Check preconditions:**
+    - Currently only tested on Linux (Debian 10,11, Ubuntu 20.04,22.04), but should work on other systems as well
+    - Minimum python3.7 (tested up to 3.11 beta) & pip installed
+        - it is preferable to not use system python version, to install "custom" user python on linux, you can try using pyenv (https://github.com/pyenv/pyenv
+    - git installed
+
+2. **Install package:**
+    - from PyPI using pip
+        ```
+        pip install sshclick
+        ```
+
+    - (OR) from source using pip
+        ```sh
+        git clone https://github.com/karlot/sshclick
+        cd sshclick
+        pip install .
+        ```
+
+3. Use it as you like, `sshc` command should be available to access SSHClick application, see below chapter for basic [usage](https://github.com/karlot/sshclick#example-usage-and-features)
+
+4. Install shell autocompletion (_TAB-TAB auto-completes on commands, options, groups and hosts_)
+    * __Bash__ - Add this line to end of your `~/.profile` file:
+      ```sh
+      eval "$(_SSHC_COMPLETE=bash_source sshc)"
+      ```
+    * __Zsh__ - Add this line to end of your `~/.zshrc` file:
+      ```sh
+      eval "$(_SSHC_COMPLETE=zsh_source sshc)"
+      ```
+
+
+### Upgrade procedure
+
+* Upgrade from new PyPI release:  
+  ```sh
+  pip install --upgrade sshclick
+  ```
+
+* Upgrade from source:
+  Assuming installation is already done, and previous version is cloned in some local folder
+
+  ```sh
+  cd sshclick     # cd into existing previously cloned repo folder
+  git pull
+  pip install --upgrade .
+  ```
+
+
+### Uninstall procedure
+Simply run:
+```
+pip uninstall sshclick
+```
+
+In case you have installed from cloned source code, you can delete locally cloned repo.
+```sh
+rm -r sshclick
+```
+
+---
+
+## SSH Config structure, and important note about comments
+
+SSHClick when editing and writing to SSH config file must use specific style, and is internally using comments to "organize" configuration itself. This means comments outside of what sshclick is handling are unsupported and will be lost when SSHClick modifies a file.)
+
+
+### Comment blocks and metadata in SSH Config
+
+SSHClick uses comments to add extra information which it can use to add concept of grouping and extra information to hosts. Special "metadata" lines start with `#@` followed by some of meta-tags like `group`, `desc`, `info`. This are all considered group metadata tags, as they apply on the group level. Note that line separations above and below "group header" are added only for visual aid, they are ignored at parsing, but are included when modifying/generating SSH config file.  
+
+This "headers" can be added manually also in SSH config, or sshclick can add them and move hosts under specific group, using `sshc` cli tool
+
+Normally start of the "GROUP HEADER" inside SSH Config would look like below.  
+- `#@group:` is KEY metadata tag, that during "parsing" defines that all hosts configured below this "tag" belong to this group
+- `#@desc:` is optional tag that adds "description" to defined group, and will display in usual group display commands
+- `#@info:` is optional tag that can appear multiple times, adding extra information lines tied to the group.
+
+Additionally each "host" definition can have optional meta info:
+- `#@host:` is optional tag that can appear multiple times, that can hold some information about the host, this meta info when defined applies to next "host" definition that will appear. If this key is added after "host" keyword, it will be applied to next host, for that reason, keep this host meta info above the actual host definition.
+
+Following is sample how group header is rendered by SSHClick:
+```
+#-------------------------------------------------------------------------------
+#@group: <GROUP-NAME>       [MANDATORY]   <-- This line starts new group
+#@desc: <GROUP-DESCRIPTION> [OPTIONAL, SINGLE]
+#@info: <GROUP-INFO-LINES>  [OPTIONAL,MULTIPLE]
+#-------------------------------------------------------------------------------
+Host ...    <-- this hosts definitions are part of the defined group
+    param1 value1
+    param2 value2
+
+#@host: <HOST-INFO-LINES>   [OPTIONAL,MULTIPLE] <-- Adds info to following host
+Host ...
+
+<ANOTHER GROUP HEADER>
+```
+
+If there are no groups defined, then all hosts are considered to be part of "default" group. SSHClick can be used to move hosts between groups and handle keeping SSH config "tidy" and with consistent format.
+
+
+## Example usage and features
+
+SSHClick is deploying `sshc` cli tool that allows interacting with your SSH Config file and perform various organization,listing, displaying and modification of SSH Group/Host configuration parameters.  
+`sshc` comes with pre-built lots of help options so each level of commands provide `--help` options to provide you info what commands and options are available at which command level.  
+
+For example to check version, type: `sshc --version`  
+_Sample output:_
+```console
+$ sshc --version
+SSHClick (sshc) - Version: 0.5.0
+```
+
+If you run `sshc` command alone, or adding `-h` or `--help` option, it will show help what else must be added to the command...  
+_Example:_
+```console
+$ sshc --help
+Usage: sshc [OPTIONS] COMMAND [ARGS]...
+
+  SSHClick - SSH Config manager. version 0.5.0
+
+  NOTE: As this is early alpha, backup your SSH config files before this
+  software, as you might accidentally lose some configuration
+
+Options:
+  --sshconfig TEXT  Config file (default: ~/.ssh/config)
+  --stdout          Send changed SSH config to STDOUT instead to original
+                    file, can be enabled with setting ENV variable (export
+                    SSHC_STDOUT=1)
+  --version         Show the version and exit.
+  -h, --help        Show this message and exit.
+
+Commands:
+  config  Modify SSHClick configuration trough SSH Config
+  group   Command group for managing groups
+  groups  Lists all groups
+  host    Command group for managing hosts
+  hosts   List configured hosts
+```
+
+
+### `group` commands and options
+
+To manage "groups" type `sshc group --help` to see options.  
+_example:_
+```console
+$ sshc group --help
+Usage: sshc group [OPTIONS] COMMAND [ARGS]...
+
+  Command group for managing groups
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  create  Create new group
+  delete  Delete group
+  list    Lists all groups
+  rename  Rename existing group
+  set     Change group parameters
+  show    Shows group details
+```
+
+### `host` commands and options
+
+To manage "groups" type `sshc host --help` to see options.  
+_example:_
+```console
+$ sshc host --help
+Usage: sshc host [OPTIONS] COMMAND [ARGS]...
+
+  Command group for managing hosts
+
+Options:
+  -h, --help  Show this message and exit.
+
+Commands:
+  create   Create new host
+  delete   Delete host(s)
+  install  Install SSH key to hosts (experimental)
+  list     List configured hosts
+  rename   Rename existing host
+  set      Set/Change host configuration
+  show     Show current host configuration
+  test     Test SSH host connection  (experimental)
+```
+
+### Output styling and user ENV variables
+
+`sshc host show` can display host output is several formats, you can specify it with `sshc host show <host> --style <style>`  
+Available styles are:
+
+| Style              | Description                                       |
+|--------------------|---------------------------------------------------|
+| `panels` (default) | Display data in several panels                    |
+| `card`             | Add data to single "card"                         |
+| `simple`           | Simple output with minimal decorations            |
+| `table`            | Flat table with 3 columns                         |
+| `table2`           | Nested table with separated host SSH params       |
+| `json`             | JSON output, useful for binding with other tools |
+
+If you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.
+
+In case user do not line "fancy" colors in output, you can set ENV variable to disable all color outputs with `export NO_COLOR=1`. If you want it permanently you can add it to startup "rc" files as well.
+
+
+> NOTE! When sending output into non-terminal such as to file, SSHClick will recognize that and will remove all ANSI Escape characters (colors and stuff...) so that output is captured in clear way.
+
+
+## Recorded demos
+
+Following demos will use this config sample file as input (located in ~/.ssh/config):
+
+```
+#<<<<< SSH Config file managed by sshclick >>>>>
+
+#-------------------------------------------------------------------------------
+#@group: network
+#@desc: Network devices in my lab
+#@info: user='admin' password='password'
+#@info: Not really, but for demo its ok :)
+#-------------------------------------------------------------------------------
+Host net-switch1
+    hostname 10.1.1.1
+
+Host net-switch2
+    hostname 10.1.1.2
+
+Host net-switch3
+    hostname 10.1.1.3
+
+Host net-*
+    user admin
+
+
+#-------------------------------------------------------------------------------
+#@group: jumphost
+#@desc: Edge-server / SSH bastion
+#@info: Used for jump-proxy from intnet to internal lab servers
+#-------------------------------------------------------------------------------
+#@host: This host can be used as proxyjump to reach LAB servers
+Host jumper1
+    hostname 123.123.123.123
+    user master
+    port 1234
+
+
+#-------------------------------------------------------------------------------
+#@group: lab-servers
+#@desc: Testing/Support servers
+#@info: Some [red]important[/] detail here!
+#@info: We can have color markups in descriptions and info lines
+#-------------------------------------------------------------------------------
+#@host: This server is [red]not[/] reachable directly, only via [green]jumper1[/]
+Host lab-serv1
+    hostname 10.10.0.1
+    user admin
+
+#@host: This server is [red]not[/] reachable directly, only via [green]jumper1[/]
+Host lab-serv2
+    hostname 10.10.0.2
+
+#@host: This server is [red]not[/] reachable directly, only via [green]lab-serv1[/]
+#@host: SSHClick can represent how end-to-end tunels will be established
+Host server-behind-lab
+    hostname 10.30.0.1
+    user testuser
+    port 1234
+    proxyjump lab-serv1
+    localforward 7630 127.0.0.1:7630
+
+#@host: This pattern applies to all hosts starting with 'lab-'
+#@host: setting 'user' and 'proxyjump' property
+Host lab-*
+    user user123
+    proxyjump jumper1
+
+```
+<!-- 
+### Demo showing some `sshc group` operations:
+[![asciicast](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89.svg)](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89)
+
+
+### Demo showing some `sshc host` operations:
+[![asciicast](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA.svg)](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA)
+
+
+### Demo displaying "end-to-end" tunnel visualization in graph
+[![asciicast](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE.svg)](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE) -->
+
+
+## Author
+
+Karlo Tisaj  
+email: karlot@gmail.com  
+github: https://github.com/karlot
+
+
+## License
+
+[MIT License](LICENSE)
 
-packages = \
-['sshclick',
- 'sshclick.cmds',
- 'sshclick.cmds.group',
- 'sshclick.cmds.host',
- 'sshclick.sshc',
- 'sshclick.sshc.host_styles']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0', 'prettytable>=3.2.0,<4.0.0', 'rich>=12.5.1,<13.0.0']
-
-entry_points = \
-{'console_scripts': ['sshc = sshclick.main:cli']}
-
-setup_kwargs = {
-    'name': 'sshclick',
-    'version': '0.4.4',
-    'description': 'SSH Config manager',
-    'long_description': '# SSH Click Config manager (sshclick)\n\nCheck this page on [GitHub](https://github.com/karlot/sshclick)\n\n## Links\n\n- [Intro](https://github.com/karlot/sshclick#intro)\n- [Why?](https://github.com/karlot/sshclick#why)\n- [What does it do](https://github.com/karlot/sshclick#what-does-it-do)\n  - [Installation procedure](https://github.com/karlot/sshclick#installation-procedure)\n  - [Upgrade procedure](https://github.com/karlot/sshclick#upgrade-procedure)\n  - [Uninstall procedure](https://github.com/karlot/sshclick#uninstall-procedure)\n- [SSH Config structure](https://github.com/karlot/sshclick#ssh-config-structure-and-important-note-about-comments)\n  - [Comment blocks and metadata](https://github.com/karlot/sshclick#comment-blocks-and-metadata-in-ssh-config)\n- [Example usage and features](https://github.com/karlot/sshclick#example-usage-and-features)\n  - [Group commands and options](https://github.com/karlot/sshclick#group-commands-and-options)\n  - [Host commands and options](https://github.com/karlot/sshclick#host-commands-and-options)\n  - [Output styling and user ENV variables](https://github.com/karlot/sshclick#output-styling-and-user-env-variables)\n- [Recorded demos](https://github.com/karlot/sshclick#recorded-demos)\n  - [sshc group operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-group-operations)\n  - [sshc host operations](https://github.com/karlot/sshclick#demo-showing-some-sshc-host-operations)\n- [Author](https://github.com/karlot/sshclick#author)\n- [License](https://github.com/karlot/sshclick#license)\n\n\n## Intro\nTerminal based assisted management of your SSH config files.  \nBuilt out of boredom with managing messy and huge ssh_config files.  \n\nEARLY VERSION, backup your SSH config files before using!  \nSSHClick can be used with "show" and "list" commands for hosts, without modifying your SSH Config!  \n\n**Only commands that modify configuration will edit and rewrite/restructure your SSH Config file. In that case, any added comment or infos that are not in form that SSHClick understand will be discarded, and configuration will be re-formatted to match SSHClick style. See below details to understand how SSH Click would keep your config organized**\n\n## Why?\n\nWhat am I trying to solve with this tool?\n* I need something that works fast and great in terminal, and does not require complex setup.\n* Managing some other configuration files that renders to SSH config is extra step that I don\'t like.\n* SSH config is already feature-full with all options SSH client support, why inventing extra layer?\n* SSH config is the only config I need to backup.\n* I need quick way to search, group and visualize all hosts inside SSH configuration (especially since it can grow huge)\n\n\n## What does it do?\n\nSSHClick (sshc) is just a tool designed to work with existing SSH configuration files on your Linux/Windows/WSL terminal environment.  \nIt basically parses your SSH config, and can provide easy commands to list, filter, modify or view specific Host entries.\nTrough additional "magic" comments it can add abstractions such as "groups" and various information that is both readable in the configuration file, and can be parsed and printed while using the tool.\n\n\n### Installation procedure\n\nShould be straight forward...  \n\n1. **Check preconditions:**\n    - Currently only tested on Linux (Debian 10,11, Ubuntu 20.04,22.04), but should work on other systems as well\n    - Minimum python3.7 (tested up to 3.11 beta) & pip installed\n        - it is preferable to not use system python version, to install "custom" user python on linux, you can try using pyenv (https://github.com/pyenv/pyenv\n    - git installed\n\n2. **Install package:**\n    - from PyPI using pip\n        ```\n        pip install sshclick\n        ```\n\n    - (OR) from source using pip\n        ```sh\n        git clone https://github.com/karlot/sshclick\n        cd sshclick\n        pip install .\n        ```\n\n3. Use it as you like, `sshc` command should be available to access SSHClick application, see below chapter for basic [usage](https://github.com/karlot/sshclick#example-usage-and-features)\n\n4. Install shell autocompletion (_TAB-TAB auto-completes on commands, options, groups and hosts_)\n    * __Bash__ - Add this line to end of your `~/.profile` file:\n      ```sh\n      eval "$(_SSHC_COMPLETE=bash_source sshc)"\n      ```\n    * __Zsh__ - Add this line to end of your `~/.zshrc` file:\n      ```sh\n      eval "$(_SSHC_COMPLETE=zsh_source sshc)"\n      ```\n\n\n### Upgrade procedure\n\n* Upgrade from new PyPI release:  \n  ```sh\n  pip install --upgrade sshclick\n  ```\n\n* Upgrade from source:\n  Assuming installation is already done, and previous version is cloned in some local folder\n\n  ```sh\n  cd sshclick     # cd into existing previously cloned repo folder\n  git pull\n  pip install --upgrade .\n  ```\n\n\n### Uninstall procedure\nSimply run:\n```\npip uninstall sshclick\n```\n\nIn case you have installed from cloned source code, you can delete locally cloned repo.\n```sh\nrm -r sshclick\n```\n\n---\n\n## SSH Config structure, and important note about comments\n\nSSHClick when editing and writing to SSH config file must use specific style, and is internally using comments to "organize" configuration itself. This means comments outside of what sshclick is handling are unsupported and will be lost when SSHClick modifies a file.)\n\n\n### Comment blocks and metadata in SSH Config\n\nSSHClick uses comments to add extra information which it can use to add concept of grouping and extra information to hosts. Special "metadata" lines start with `#@` followed by some of meta-tags like `group`, `desc`, `info`. This are all considered group metadata tags, as they apply on the group level. Note that line separations above and below "group header" are added only for visual aid, they are ignored at parsing, but are included when modifying/generating SSH config file.  \n\nThis "headers" can be added manually also in SSH config, or sshclick can add them and move hosts under specific group, using `sshc` cli tool\n\nNormally start of the "GROUP HEADER" inside SSH Config would look like below.  \n- `#@group:` is KEY metadata tag, that during "parsing" defines that all hosts configured below this "tag" belong to this group\n- `#@desc:` is optional tag that adds "description" to defined group, and will display in usual group display commands\n- `#@info:` is optional tag that can appear multiple times, adding extra information lines tied to the group.\n\nAdditionally each "host" definition can have optional meta info:\n- `#@host:` is optional tag that can appear multiple times, that can hold some information about the host, this meta info when defined applies to next "host" definition that will appear. If this key is added after "host" keyword, it will be applied to next host, for that reason, keep this host meta info above the actual host definition.\n\nFollowing is sample how group header is rendered by SSHClick:\n```\n#-------------------------------------------------------------------------------\n#@group: <GROUP-NAME>       [MANDATORY]   <-- This line starts new group\n#@desc: <GROUP-DESCRIPTION> [OPTIONAL, SINGLE]\n#@info: <GROUP-INFO-LINES>  [OPTIONAL,MULTIPLE]\n#-------------------------------------------------------------------------------\nHost ...    <-- this hosts definitions are part of the defined group\n    param1 value1\n    param2 value2\n\n#@host: <HOST-INFO-LINES>  [OPTIONAL,MULTIPLE] <-- Adds info to following host\nHost ...\n\n<ANOTHER GROUP HEADER>\n```\n\nIf there are no groups defined, then all hosts are considered to be part of "default" group. SSHClick can be used to move hosts between groups and handle keeping SSH config "tidy" and with consistent format.\n\n\n## Example usage and features\n\nSSHClick is deploying `sshc` cli tool that allows interacting with your SSH Config file and perform various organization,listing, displaying and modification of SSH Group/Host configuration parameters.  \n`sshc` comes with pre-built lots of help options so each level of commands provide `--help` options to provide you info what commands and options are available at which command level.  \n\nFor example to check version, type: `sshc --version`  \n_Sample output:_\n```console\n$ sshc --version\nSSHClick (sshc) - Version: 0.4.1\n```\n\nIf you run `sshc` command alone, or adding `-h` or `--help` option, it will show help what else must be added to the command...  \n_Example:_\n```console\n$ sshc --help\nUsage: sshc [OPTIONS] COMMAND [ARGS]...\n\n  SSHClick - SSH Config manager\n\n  Note: As this is early alpha, backup your SSH config files before this\n  software, as you might accidentally lose some configuration\n\nOptions:\n  --sshconfig PATH  Config file, default is ~/.ssh/config\n  --stdout          Send changed SSH config to STDOUT instead to original file\n  --version         Show current version\n  -h, --help        Show this message and exit.\n\nCommands:\n  group  Manage groups\n  host   Manage hosts\n```\n\nMain sub-commands are for separate control of:  \n- Groups (via `sshc group` command)\n  - Allows operation of groups inside SSH config\n- Hosts (via `sshc host` command)\n  - Allows operation of hosts inside SSH config\n\n### `group` commands and options\n\nTo manage "groups" type `sshc group --help` to see options.  \n_example:_\n```console\n$ sshc group --help\nUsage: sshc group [OPTIONS] COMMAND [ARGS]...\n\n  Manage groups\n\nOptions:\n  -h, --help  Show this message and exit.\n\nCommands:\n  create  Create new group\n  delete  Delete group\n  list    Lists all groups\n  set     Change group parameters\n  show    Shows group details\n```\n\n### `host` commands and options\n\nTo manage "groups" type `sshc host --help` to see options.  \n_example:_\n```console\n$ sshc host --help\nUsage: sshc host [OPTIONS] COMMAND [ARGS]...\n\n  Manage hosts\n\nOptions:\n  -h, --help  Show this message and exit.\n\nCommands:\n  create  Create new host configuration\n  delete  Delete host from configuration\n  list    List hosts\n  set     Changes/sets host configuration parameters\n  show    Display info for host\n  test    Test SSH host connection\n```\n\n### Output styling and user ENV variables\n\n`sshc host show` can display host output is several formats, you can specify it with `sshc host show <host> --style <style>`  \nAvailable styles are:\n\n| Style              | Description                                       |\n|--------------------|---------------------------------------------------|\n| `panels` (default) | Display data in several panels                    |\n| `card`             | Add data to single "card"                         |\n| `simple`           | Simple output with minimal decorations            |\n| `table`            | Flat table with 3 columns                         |\n| `table2`           | Nested table with separated host SSH params       |\n| `json`             | JSON output, useful for binding with other tools |\n\nIf you want to have some style statically set for your shell, you can export ENV variable with `export SSHC_HOST_STYLE=table`, and add it to `.profile` or `.bashrc` or `.zshrc`, so its set when shell session is starting, to set "default" style to that one.\n\nIn case user do not line "fancy" colors in output, you can set ENV variable to disable all color outputs with `export NO_COLOR=1`. If you want it permanently you can add it to startup "rc" files as well.\n\n\n> NOTE! When sending output into non-terminal such as to file, SSHClick will recognize that and will remove all ANSI Escape characters (colors and stuff...) so that output is captured in clear way.\n\n\n## Recorded demos\n\nFollowing demos will use this config sample file as input (located in ~/.ssh/config):\n\n```\n#<<<<< SSH Config file managed by sshclick >>>>>\n\n#-------------------------------------------------------------------------------\n#@group: network\n#@desc: Network devices in my lab\n#@info: user=\'admin\' password=\'password\'\n#@info: Not really, but for demo its ok :)\n#-------------------------------------------------------------------------------\nHost net-switch1\n    hostname 10.1.1.1\n\nHost net-switch2\n    hostname 10.1.1.2\n\nHost net-switch3\n    hostname 10.1.1.3\n\nHost net-*\n    user admin\n\n\n#-------------------------------------------------------------------------------\n#@group: jumphost\n#@desc: Edge-server / SSH bastion\n#@info: Used for jump-proxy from intnet to internal lab servers\n#-------------------------------------------------------------------------------\nHost jumper1\n    hostname 123.123.123.123\n    user master\n    port 1234\n\n\n#-------------------------------------------------------------------------------\n#@group: lab-servers\n#@desc: Testing/Support servers\n#@info: Some [red]important[/] detail here!\n#@info: We can have color markups in descriptions and info lines\n#-------------------------------------------------------------------------------\nHost lab-serv1\n    hostname 10.10.0.1\n    user admin\n\nHost lab-serv2\n    hostname 10.16.141\n\nHost lab-*\n    user user123\n    proxyjump jumper1\n\nHost server-behind-lab\n    hostname 10.30.0.1\n    user testuser\n    port 1234\n    proxyjump lab-serv1\n\n```\n\n### Demo showing some `sshc group` operations:\n[![asciicast](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89.svg)](https://asciinema.org/a/BQoVXv2HSeIvTyATeKUBGfr89)\n\n\n### Demo showing some `sshc host` operations:\n[![asciicast](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA.svg)](https://asciinema.org/a/wzLefl49CRErBoFwC6ir96FFA)\n\n\n### Demo displaying "end-to-end" tunnel visualization in graph\n[![asciicast](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE.svg)](https://asciinema.org/a/I4O2bfDiRAN7xEGdTB1S9rChE)\n\n\n## Author\n\nKarlo Tisaj  \nemail: karlot@gmail.com  \ngithub: https://github.com/karlot\n\n\n## License\n\n[MIT License](LICENSE)\n\n\n',
-    'author': 'Karlo Tisaj',
-    'author_email': 'karlot@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/karlot/sshclick',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

