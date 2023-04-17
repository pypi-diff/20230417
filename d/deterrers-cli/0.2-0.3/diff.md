# Comparing `tmp/deterrers-cli-0.2.tar.gz` & `tmp/deterrers-cli-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-cli-0.2.tar", last modified: Thu Apr 13 21:56:09 2023, max compression
+gzip compressed data, was "deterrers-cli-0.3.tar", last modified: Mon Apr 17 13:38:13 2023, max compression
```

## Comparing `deterrers-cli-0.2.tar` & `deterrers-cli-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.573636 deterrers-cli-0.2/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.2/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.2/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:56:09.572636 deterrers-cli-0.2/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     1756 2023-04-13 21:53:30.000000 deterrers-cli-0.2/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.572636 deterrers-cli-0.2/deterrers_cli.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     2026 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       27 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-13 21:56:09.000000 deterrers-cli-0.2/deterrers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-13 21:56:09.572636 deterrers-cli-0.2/deterrerscli/
--rw-r--r--   0 lars      (1000) lars      (1000)     2272 2023-04-13 21:39:15.000000 deterrers-cli-0.2/deterrerscli/__main__.py
--rw-r--r--   0 lars      (1000) lars      (1000)       27 2023-04-13 21:55:40.000000 deterrers-cli-0.2/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-13 21:56:09.573636 deterrers-cli-0.2/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-13 21:56:01.000000 deterrers-cli-0.2/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.3/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.3/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-17 13:38:13.508019 deterrers-cli-0.3/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     1908 2023-04-17 13:28:29.000000 deterrers-cli-0.3/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/deterrers_cli.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/deterrerscli/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2437 2023-04-17 13:23:20.000000 deterrers-cli-0.3/deterrerscli/__main__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-17 13:20:44.000000 deterrers-cli-0.3/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-17 13:38:13.508019 deterrers-cli-0.3/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-17 13:21:20.000000 deterrers-cli-0.3/setup.py
```

### Comparing `deterrers-cli-0.2/LICENSE` & `deterrers-cli-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.2/PKG-INFO` & `deterrers-cli-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.2
+Version: 0.3
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -62,25 +62,27 @@
 ❯ deterrers-cli add --help
 Usage: python -m deterrerscli add [OPTIONS] IPV4
 
   Add IP address to DETERRERS.
 
 Options:
   -a, --admin TEXT  [required]
+  -p, --profile [|HTTP|SSH|HTTP+SSH|Multipurpose]
+  -f, --firewall [|UFW|FirewallD|nftables]
   --help            Show this message and exit.
 ```
 
 ## Example
 
 ```sh
 # Delete IP 192.0.0.1 from DETERRERS
 ❯ deterrers-cli delete 192.0.0.1
 
-# Add IP 192.0.0.1 with group `virtUOS` as admins
-❯ deterrers-cli add --admin virtUOS 192.0.0.1
+# Add IP 192.0.0.1 with group `virtUOS` as admins and firewall profile `Multipurpose`
+❯ deterrers-cli add --admin virtUOS --profile multipurpose 192.0.0.1
 
 # Set firewall profile `SSH`
 ❯ deterrers-cli update --profile ssh 192.0.0.1
 
 # Activate firewall profile
 ❯ deterrers-cli action register 192.0.0.1
 ```
```

### Comparing `deterrers-cli-0.2/README.md` & `deterrers-cli-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -51,25 +51,27 @@
 ❯ deterrers-cli add --help
 Usage: python -m deterrerscli add [OPTIONS] IPV4
 
   Add IP address to DETERRERS.
 
 Options:
   -a, --admin TEXT  [required]
+  -p, --profile [|HTTP|SSH|HTTP+SSH|Multipurpose]
+  -f, --firewall [|UFW|FirewallD|nftables]
   --help            Show this message and exit.
 ```
 
 ## Example
 
 ```sh
 # Delete IP 192.0.0.1 from DETERRERS
 ❯ deterrers-cli delete 192.0.0.1
 
-# Add IP 192.0.0.1 with group `virtUOS` as admins
-❯ deterrers-cli add --admin virtUOS 192.0.0.1
+# Add IP 192.0.0.1 with group `virtUOS` as admins and firewall profile `Multipurpose`
+❯ deterrers-cli add --admin virtUOS --profile multipurpose 192.0.0.1
 
 # Set firewall profile `SSH`
 ❯ deterrers-cli update --profile ssh 192.0.0.1
 
 # Activate firewall profile
 ❯ deterrers-cli action register 192.0.0.1
 ```
```

### Comparing `deterrers-cli-0.2/deterrers_cli.egg-info/PKG-INFO` & `deterrers-cli-0.3/deterrers_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.2
+Version: 0.3
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -62,25 +62,27 @@
 ❯ deterrers-cli add --help
 Usage: python -m deterrerscli add [OPTIONS] IPV4
 
   Add IP address to DETERRERS.
 
 Options:
   -a, --admin TEXT  [required]
+  -p, --profile [|HTTP|SSH|HTTP+SSH|Multipurpose]
+  -f, --firewall [|UFW|FirewallD|nftables]
   --help            Show this message and exit.
 ```
 
 ## Example
 
 ```sh
 # Delete IP 192.0.0.1 from DETERRERS
 ❯ deterrers-cli delete 192.0.0.1
 
-# Add IP 192.0.0.1 with group `virtUOS` as admins
-❯ deterrers-cli add --admin virtUOS 192.0.0.1
+# Add IP 192.0.0.1 with group `virtUOS` as admins and firewall profile `Multipurpose`
+❯ deterrers-cli add --admin virtUOS --profile multipurpose 192.0.0.1
 
 # Set firewall profile `SSH`
 ❯ deterrers-cli update --profile ssh 192.0.0.1
 
 # Activate firewall profile
 ❯ deterrers-cli action register 192.0.0.1
 ```
```

### Comparing `deterrers-cli-0.2/deterrerscli/__main__.py` & `deterrers-cli-0.3/deterrerscli/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,19 +54,21 @@
     '''Delete IP address from DETERRERS.
     '''
     deterrers.delete(ipv4)
 
 
 @cli.command()
 @click.option('--admin', '-a', multiple=True, required=True)
+@click.option('--profile', '-p', default='', type=profiles)
+@click.option('--firewall', '-f', default='', type=host_firewalls)
 @click.argument('ipv4')
-def add(ipv4, admin):
+def add(ipv4, admin, profile, firewall):
     '''Add IP address to DETERRERS.
     '''
-    deterrers.add(ipv4, admin)
+    deterrers.add(ipv4, admin, profile, firewall)
 
 
 @cli.command()
 @click.option('--profile', '-p', default='', type=profiles)
 @click.option('--firewall', '-f', default='', type=host_firewalls)
 @click.argument('ipv4')
 def update(ipv4, profile, firewall):
```

### Comparing `deterrers-cli-0.2/setup.py` & `deterrers-cli-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-cli',
-    version='0.2',
+    version='0.3',
     description='Command line client for DETERRERS',
     url='https://github.com/virtUOS/proteuscmd',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrerscli'],
     license_files=('LICENSE'),
```

