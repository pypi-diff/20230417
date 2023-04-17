# Comparing `tmp/pyinflux3-cli-0.8.1.tar.gz` & `tmp/pyinflux3-cli-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.8.1.tar", last modified: Fri Apr 14 08:51:55 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.8.2.tar", last modified: Mon Apr 17 16:12:39 2023, max compression
```

## Comparing `pyinflux3-cli-0.8.1.tar` & `pyinflux3-cli-0.8.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:51:55.960038 pyinflux3-cli-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-14 08:51:55.960038 pyinflux3-cli-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 08:51:52.000000 pyinflux3-cli-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:51:55.960038 pyinflux3-cli-0.8.1/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:51:52.000000 pyinflux3-cli-0.8.1/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-14 08:51:52.000000 pyinflux3-cli-0.8.1/influxdb_cli/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:51:55.960038 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 08:51:55.000000 pyinflux3-cli-0.8.1/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-14 08:51:52.000000 pyinflux3-cli-0.8.1/setup-cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:51:55.960038 pyinflux3-cli-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7626 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/setup.cfg
```

### Comparing `pyinflux3-cli-0.8.1/influxdb_cli/influx3.py` & `pyinflux3-cli-0.8.2/influxdb_cli/influx3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-import cmd
+import cmd, ast
 import argparse
 from flightsql import FlightSQLClient
 import json
 from prompt_toolkit import PromptSession
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
@@ -50,14 +50,36 @@
             print("can't write, no active configs")
             return
         if arg == "":
             print("can't write, no line protocol supplied")
             return
         
         self.influxdb_client.write(record=arg)
+    
+    def do_write_csv(self, args):
+        if self._configurations == {}:
+            print("can't write, no active configs")
+            return
+
+        temp = {}
+        attributes = ['file', 'measurement', 'time', 'tags']
+        temp['tags'] = []
+
+        for attribute in attributes:
+            arg_value = getattr(args, attribute)
+            if arg_value is not None:
+                temp[attribute] = arg_value
+        if isinstance(temp['tags'], str):
+            temp['tags'] =  temp['tags'].split(',')
+
+
+        self.influxdb_client.write_csv(csv_file=temp['file'], 
+                                       measurement_name=temp['measurement'], 
+                                       timestamp_column=temp['time'], 
+                                       tag_columns=temp['tags'])
 
     def do_exit(self, arg):
         'Exit the shell: exit'
         print('\nExiting ...')
         return True
 
     def do_EOF(self, arg):
@@ -91,15 +113,15 @@
     
     def config(self, args):
         if args.name in self._configurations:
             config = self._configurations[args.name]
         else:
             config = {}
 
-        attributes = ['namespace', 'host', 'token', 'org']
+        attributes = ['database', 'host', 'token', 'org']
 
         for attribute in attributes:
             arg_value = getattr(args, attribute)
             if arg_value is not None:
                 config[attribute] = arg_value
 
         config['active'] = True
@@ -122,56 +144,64 @@
         self._configurations = json.loads(f.read())
         active_conf = None
         for c in self._configurations.keys():
             if self._configurations[c]["active"]:
                 active_conf = self._configurations[c]
         if active_conf is None:
             print("no active configuration found")
-        self._namespace = active_conf['namespace']
+        self._database = active_conf['database']
 
         self.influxdb_client = InfluxDBClient3(host=f"{active_conf['host']}",
                                                  org=active_conf['org'],
                                                  token=active_conf['token'],
-                                                 namespace=active_conf['namespace']
+                                                 database=active_conf['database']
                                                  )
 
 class StoreRemainingInput(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
-        setattr(namespace, self.dest, ' '.join(values))
+    def __call__(self, parser, database, values, option_string=None):
+        setattr(database, self.dest, ' '.join(values))
 
 def parse_args():
     parser = argparse.ArgumentParser(description= _description_string
                                      )
     subparsers = parser.add_subparsers(dest='command')
 
     sql_parser = subparsers.add_parser('sql', help='execute the given SQL query')
     sql_parser.add_argument('query', metavar='QUERY', nargs='*', action=StoreRemainingInput, help='the SQL query to execute')
 
     write_parser = subparsers.add_parser('write', help='write line protocol to InfluxDB')
     write_parser.add_argument('line_protocol', metavar='LINE PROTOCOL',  nargs='*', action=StoreRemainingInput, help='the data to write')
 
+    write_csv_parser = subparsers.add_parser('write_csv', help='write CSV data to InfluxDB')
+    write_csv_parser.add_argument('--file', help='the CSV file to import', required=True)
+    write_csv_parser.add_argument('--measurement', help='Define the name of the measurement', required=True)
+    write_csv_parser.add_argument('--time', help='Define the name of the time column with the csv file', required=True)
+    write_csv_parser.add_argument('--tags', help='(optional) array of column names which are tags. Format should be: ["tag1", "tag2"]', required=False)
+
     config_parser = subparsers.add_parser("config", help="configure the application")
     config_parser.add_argument("--name", help="Configuration name", required=True)
     config_parser.add_argument("--host", help="Host string")
     config_parser.add_argument("--token", help="Token string")
-    config_parser.add_argument("--namespace", help="Namespace string")
+    config_parser.add_argument("--database", help="Database string")
     config_parser.add_argument("--org", help="Organization string")
 
     config_parser = subparsers.add_parser("help")
 
     return parser.parse_args()
 
 def main():
     args = parse_args()
     app = IOXCLI()
 
     if args.command == 'sql':
         app.do_sql(args.query)
     if args.command == 'write':
         app.do_write(args.line_protocol)
+    if args.command == 'write_csv':
+        app.do_write_csv(args)
     if args.command == 'config':
         app.config(args)
     if args.command == 'help':
         print(_usage_string)
     if args.command is None:
         app.cmdloop()
```

### Comparing `pyinflux3-cli-0.8.1/setup-cli.py` & `pyinflux3-cli-0.8.2/setup-cli.py`

 * *Files identical despite different names*

