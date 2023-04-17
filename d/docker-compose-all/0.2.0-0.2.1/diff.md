# Comparing `tmp/docker-compose-all-0.2.0.tar.gz` & `tmp/docker-compose-all-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-compose-all-0.2.0.tar", last modified: Sun Mar 26 14:31:36 2023, max compression
+gzip compressed data, was "docker-compose-all-0.2.1.tar", last modified: Mon Apr 17 14:05:42 2023, max compression
```

## Comparing `docker-compose-all-0.2.0.tar` & `docker-compose-all-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2023-03-26 14:31:36.640948 docker-compose-all-0.2.0/
--rw-r--r--   0 shen       (501) staff       (20)    35149 2019-07-29 17:50:11.000000 docker-compose-all-0.2.0/LICENSE
--rw-r--r--   0 shen       (501) staff       (20)       29 2020-10-10 00:17:28.000000 docker-compose-all-0.2.0/MANIFEST.in
--rw-r--r--   0 shen       (501) staff       (20)      824 2023-03-26 14:31:36.640603 docker-compose-all-0.2.0/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      143 2023-03-26 14:28:18.000000 docker-compose-all-0.2.0/Readme.PyPI.md
--rw-r--r--   0 shen       (501) staff       (20)     1858 2023-03-26 14:29:24.000000 docker-compose-all-0.2.0/Readme.md
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2023-03-26 14:31:36.640086 docker-compose-all-0.2.0/docker_compose_all.egg-info/
--rw-r--r--   0 shen       (501) staff       (20)      824 2023-03-26 14:31:36.000000 docker-compose-all-0.2.0/docker_compose_all.egg-info/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      288 2023-03-26 14:31:36.000000 docker-compose-all-0.2.0/docker_compose_all.egg-info/SOURCES.txt
--rw-r--r--   0 shen       (501) staff       (20)        1 2023-03-26 14:31:36.000000 docker-compose-all-0.2.0/docker_compose_all.egg-info/dependency_links.txt
--rw-r--r--   0 shen       (501) staff       (20)       64 2023-03-26 14:31:36.000000 docker-compose-all-0.2.0/docker_compose_all.egg-info/entry_points.txt
--rw-r--r--   0 shen       (501) staff       (20)       19 2023-03-26 14:31:36.000000 docker-compose-all-0.2.0/docker_compose_all.egg-info/top_level.txt
--rwxr-xr-x   0 shen       (501) staff       (20)    11236 2023-03-26 14:28:37.000000 docker-compose-all-0.2.0/docker_compose_all.py
--rw-r--r--   0 shen       (501) staff       (20)       38 2023-03-26 14:31:36.641049 docker-compose-all-0.2.0/setup.cfg
--rwxr-xr-x   0 shen       (501) staff       (20)     1193 2023-03-26 09:38:51.000000 docker-compose-all-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      824 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/docker_compose_all.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      824 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    11610 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/docker_compose_all.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1123 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/setup.py
```

### Comparing `docker-compose-all-0.2.0/LICENSE` & `docker-compose-all-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-compose-all-0.2.0/PKG-INFO` & `docker-compose-all-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-compose-all
-Version: 0.2.0
+Version: 0.2.1
 Summary: A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 Home-page: https://github.com/Phuker/docker-compose-all
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
```

### Comparing `docker-compose-all-0.2.0/Readme.md` & `docker-compose-all-0.2.1/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 python3 -m pip install -U docker-compose-all
 ```
 
 ## Usage
 
 ```console
 # docker-compose-all --help
-usage: docker_compose_all.py [-h] [--restart | --stop | --down | --build | --up | --ps | --top] [--dokill] [--normi] [--nopull] [--doclean] [-v] DIR
+usage: docker-compose-all [-h] [--restart | --stop | --down | --build | --up | --ps | --top] [--dokill] [--normi] [--nopull] [--doclean] [-V] [-v] [dir_path]
 
-docker-compose-all version 0.2.0
+docker-compose-all version 0.2.1
 A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 https://github.com/Phuker/docker-compose-all
 
 positional arguments:
-  DIR            A directory which contains Docker Compose projects
+  dir_path       A directory which contains Docker Compose projects, default: '.'
 
-options:
+optional arguments:
   -h, --help     show this help message and exit
   --restart      Completely rebuild and rerun all. Including the following steps: stop, down, build, up, ps.
   --stop         Stop all containers
   --down         Make all down. Stop and remove containers, networks, images
   --build        Rebuild all
   --up           Make all up
   --ps           Each ps
   --top          List all process
+  -V, --version  Show version and exit
   -v, --verbose  Increase verbosity level (use -vv or more for greater effect)
 
 docker-compose options:
   --dokill       Run "docker-compose kill" instead of "docker-compose stop"
   --normi        Do NOT remove Docker images when running "docker-compose down"
   --nopull       Do NOT pull images when running "docker-compose build"
   --doclean      Clean up before exit, if no error. Remove ALL unused networks, images and build cache. WARN: This may cause data loss.
```

### Comparing `docker-compose-all-0.2.0/docker_compose_all.egg-info/PKG-INFO` & `docker-compose-all-0.2.1/docker_compose_all.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-compose-all
-Version: 0.2.0
+Version: 0.2.1
 Summary: A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 Home-page: https://github.com/Phuker/docker-compose-all
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
```

### Comparing `docker-compose-all-0.2.0/docker_compose_all.py` & `docker-compose-all-0.2.1/docker_compose_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 import atexit
 import time
 import subprocess
 import shlex
 from datetime import timedelta
 
 
+__version__ = '0.2.1'
+logger = logging.getLogger(__name__)
+shell_args = None
+
+VERSION_STR_SHORT = f'docker-compose-all version {__version__}'
+VERSION_STR_LONG = f'docker-compose-all version {__version__}\n{__doc__.strip()}'
+
 # https://docs.docker.com/compose/compose-file/03-compose-file/
 DOCKER_COMPOSE_FILENAME_SET = {
     'compose.yaml',
     'compose.yml',
     'docker-compose.yaml',
     'docker-compose.yml',
 }
@@ -37,18 +44,14 @@
 COMMAND_CLEAN_BUILDER = ('Remove build cache', ['docker', 'builder', 'prune', '-f'])
 COMMANDS_CLEAN = [
     COMMAND_CLEAN_NETWORKS,
     COMMAND_CLEAN_IMAGES,
     COMMAND_CLEAN_BUILDER,
 ]
 
-__version__ = '0.2.0'
-logger = logging.getLogger(__name__)
-shell_args = None
-
 
 def _assert(expr, msg=''):
     if not expr:
         raise AssertionError(msg)
 
 
 def _init_logging():
@@ -74,48 +77,56 @@
     logging.addLevelName(logging.INFO, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.INFO)))
     logging.addLevelName(logging.DEBUG, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.DEBUG)))
 
 
 def _parse_args():
     global shell_args
 
+    default_docker_files_dir = '.'
+
     parser = argparse.ArgumentParser(
-        description=f'docker-compose-all version {__version__}\n{__doc__.strip()}',
+        description=VERSION_STR_LONG,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         add_help=True
     )
 
     group = parser.add_mutually_exclusive_group(required=False)
-    group.add_argument('--restart',  action="store_true", help="Completely rebuild and rerun all. Including the following steps: stop, down, build, up, ps.")
-    group.add_argument('--stop', action="store_true", help="Stop all containers")
-    group.add_argument('--down', action="store_true", help="Make all down. Stop and remove containers, networks, images")
-    group.add_argument('--build', action="store_true", help="Rebuild all")
-    group.add_argument('--up', action="store_true", help="Make all up")
-    group.add_argument('--ps', action="store_true", help="Each ps")
-    group.add_argument('--top', action="store_true", help="List all process")
+    group.add_argument('--restart', action='store_true', help='Completely rebuild and rerun all. Including the following steps: stop, down, build, up, ps.')
+    group.add_argument('--stop', action='store_true', help='Stop all containers')
+    group.add_argument('--down', action='store_true', help='Make all down. Stop and remove containers, networks, images')
+    group.add_argument('--build', action='store_true', help='Rebuild all')
+    group.add_argument('--up', action='store_true', help='Make all up')
+    group.add_argument('--ps', action='store_true', help='Each ps')
+    group.add_argument('--top', action='store_true', help='List all process')
 
     dc_opt_group = parser.add_argument_group('docker-compose options')
     dc_opt_group.add_argument('--dokill', action='store_true', help='Run "docker-compose kill" instead of "docker-compose stop"')
     dc_opt_group.add_argument('--normi', action='store_true', help='Do NOT remove Docker images when running "docker-compose down"')
     dc_opt_group.add_argument('--nopull', action='store_true', help='Do NOT pull images when running "docker-compose build"')
     dc_opt_group.add_argument('--doclean', action='store_true', help='Clean up before exit, if no error. Remove ALL unused networks, images and build cache. WARN: This may cause data loss.')
 
-    parser.add_argument('docker_files_dir', metavar="DIR", help="A directory which contains Docker Compose projects")
+    parser.add_argument('docker_files_dir', metavar='dir_path', nargs='?', default=default_docker_files_dir, help=f'A directory which contains Docker Compose projects, default: {default_docker_files_dir!r}')
+
+    parser.add_argument('-V', '--version', action='store_true', help='Show version and exit')
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase verbosity level (use -vv or more for greater effect)')
 
     shell_args = parser.parse_args()
 
     if shell_args.verbose >= 1:
         logging.root.setLevel(logging.DEBUG)
     
     shell_args.docker_files_dir = os.path.abspath(os.path.expanduser(shell_args.docker_files_dir))
     _assert(os.path.isdir(shell_args.docker_files_dir), f'Dir not found: {shell_args.docker_files_dir!r}')
 
     logger.debug('Command line arguments: %r', shell_args)
 
+    if shell_args.version:
+        print(VERSION_STR_LONG)
+        sys.exit(0)
+
 
 def colored(s, foreground, background=None, **kwargs):
     if kwargs.get('repr', False):
         s = repr(s)
     else:
         s = str(s)
     
@@ -270,15 +281,15 @@
         atexit.register(lambda: logger.info('Exiting'))
     else:
         atexit.register(lambda: logger.info('Exiting\n'))
 
     _start_time_stamp = time.time()
     atexit.register(lambda: logger.info('Time elapsed: %s', timedelta(seconds=int(time.time() - _start_time_stamp))))
 
-    logger.info(colored('docker-compose-all version %s', 'default', bold=True), __version__)
+    logger.info(colored(VERSION_STR_SHORT, 'default', bold=True))
 
     update_docker_compose_commands()
 
     # Run as root, after argparse (could show help)
     if not os.getuid() == 0:
         logger.critical('Need root privilege')
         sys.exit(1)
```

### Comparing `docker-compose-all-0.2.0/setup.py` & `docker-compose-all-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 from setuptools import setup
 
-import docker_compose_all
 
 with open('Readme.PyPI.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='docker-compose-all',
-    version=docker_compose_all.__version__,
     description='A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     author='Phuker',
     author_email='Phuker@users.noreply.github.com',
     url='https://github.com/Phuker/docker-compose-all',
     license='GNU General Public License v3.0',
     packages=[],
     py_modules = ['docker_compose_all'],
     install_requires=[],
```

