# Comparing `tmp/pydbbackups-0.0.4.tar.gz` & `tmp/pydbbackups-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbbackups-0.0.4.tar", max compression
+gzip compressed data, was "pydbbackups-0.1.0.tar", max compression
```

## Comparing `pydbbackups-0.0.4.tar` & `pydbbackups-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-04-10 18:04:15.039262 pydbbackups-0.0.4/LICENSE
--rw-r--r--   0        0        0      762 2023-04-11 15:50:15.989646 pydbbackups-0.0.4/README.md
--rw-r--r--   0        0        0      394 2023-04-11 16:03:17.287223 pydbbackups-0.0.4/pydbbackups/__init__.py
--rw-r--r--   0        0        0       85 2023-03-26 16:35:39.235013 pydbbackups-0.0.4/pydbbackups/backups/__init__.py
--rw-r--r--   0        0        0     1443 2023-04-11 14:59:10.375930 pydbbackups-0.0.4/pydbbackups/backups/base.py
--rw-r--r--   0        0        0      776 2023-04-04 15:17:50.157968 pydbbackups-0.0.4/pydbbackups/backups/mongodb.py
--rw-r--r--   0        0        0     1201 2023-04-10 14:23:53.741447 pydbbackups-0.0.4/pydbbackups/backups/postgres.py
--rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.0.4/pydbbackups/cli/__init__.py
--rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.0.4/pydbbackups/cli/config.py
--rw-r--r--   0        0        0     1854 2023-04-11 16:10:46.105655 pydbbackups-0.0.4/pydbbackups/cli/main.py
--rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.0.4/pydbbackups/cli/models/__init__.py
--rw-r--r--   0        0        0      325 2023-04-09 16:07:03.941354 pydbbackups-0.0.4/pydbbackups/cli/models/backup_data.py
--rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.0.4/pydbbackups/cli/services/__init__.py
--rw-r--r--   0        0        0     1715 2023-04-11 15:52:37.888137 pydbbackups-0.0.4/pydbbackups/cli/services/backups.py
--rw-r--r--   0        0        0     1453 2023-04-10 16:49:51.999547 pydbbackups-0.0.4/pydbbackups/cli/utils/__init__.py
--rw-r--r--   0        0        0      526 2023-04-09 16:37:14.487168 pydbbackups-0.0.4/pydbbackups/errors.py
--rw-r--r--   0        0        0      654 2023-04-11 16:10:38.665692 pydbbackups-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 pydbbackups-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-10 18:04:15.039262 pydbbackups-0.1.0/LICENSE
+-rw-r--r--   0        0        0      688 2023-04-17 13:30:02.519868 pydbbackups-0.1.0/README.md
+-rw-r--r--   0        0        0      342 2023-04-17 13:28:48.086818 pydbbackups-0.1.0/pydbbackups/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-13 23:17:43.410842 pydbbackups-0.1.0/pydbbackups/backups/__init__.py
+-rw-r--r--   0        0        0     1251 2023-04-15 14:03:21.910715 pydbbackups-0.1.0/pydbbackups/backups/base.py
+-rw-r--r--   0        0        0     1953 2023-04-17 13:23:46.359484 pydbbackups-0.1.0/pydbbackups/backups/mongodb.py
+-rw-r--r--   0        0        0     2701 2023-04-16 22:35:52.710687 pydbbackups-0.1.0/pydbbackups/backups/postgres.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.1.0/pydbbackups/cli/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.1.0/pydbbackups/cli/config.py
+-rw-r--r--   0        0        0     3861 2023-04-17 13:31:05.492808 pydbbackups-0.1.0/pydbbackups/cli/main.py
+-rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.1.0/pydbbackups/cli/models/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-16 16:49:12.978652 pydbbackups-0.1.0/pydbbackups/cli/models/backup_data.py
+-rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.1.0/pydbbackups/cli/services/__init__.py
+-rw-r--r--   0        0        0     2731 2023-04-16 22:47:27.036091 pydbbackups-0.1.0/pydbbackups/cli/services/backups.py
+-rw-r--r--   0        0        0     2790 2023-04-17 13:21:57.866782 pydbbackups-0.1.0/pydbbackups/cli/utils/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-13 14:07:01.165007 pydbbackups-0.1.0/pydbbackups/errors.py
+-rw-r--r--   0        0        0      655 2023-04-17 13:30:29.724269 pydbbackups-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 pydbbackups-0.1.0/PKG-INFO
```

### Comparing `pydbbackups-0.0.4/LICENSE` & `pydbbackups-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.4/pydbbackups/backups/base.py` & `pydbbackups-0.1.0/pydbbackups/backups/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 from dataclasses import dataclass
 from typing import Optional, Sequence, Tuple
 from io import BytesIO
 from pathlib import Path
 from pydbbackups.errors import MethodNotImplemented, CommandNotFound
-import subprocess
+from shutil import which
 
 
 @dataclass
 class Backup:
     host: str
     username: str
     database: str
 
     uri: Optional[str] = None
     password: Optional[str] = None
     port: Optional[int] = None
 
-    compress: Optional[bool] = False
-
     CMDS_TO_CHECK: Optional[Sequence[Tuple[str, Optional[str]] | str]] = None
 
     @classmethod
     def exist_cmds(cls):
         if not cls.CMDS_TO_CHECK:
             print(
                 f"Warning : The {cls.__name__} class doesn't have commands to check")
             return
 
         for cmd in cls.CMDS_TO_CHECK:
-            args = []
+            # args = []
             if isinstance(cmd, tuple):
                 command = cmd[0]
-                if len(cmd) > 1:
-                    args = cmd[1]
+                # if len(cmd) > 1:
+                #     args = cmd[1]
             else:
                 command = cmd
 
-            try:
-                subprocess.Popen([
-                    command,
-                    *args
-                ], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            except FileNotFoundError:
+            if not which(command):
                 raise CommandNotFound(command)
 
-    def dump(self) -> BytesIO:
+    def dump(self, **kwargs) -> BytesIO:
         raise MethodNotImplemented('Dump')
 
     def restore(self, file_path: Path) -> BytesIO:
         raise MethodNotImplemented('Restore')
 
     def __post_init__(self):
         self.exist_cmds()
```

### Comparing `pydbbackups-0.0.4/pydbbackups/cli/main.py` & `pydbbackups-0.1.0/pydbbackups/cli/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import click
 import getpass
+import inquirer
+import time
 
 from rich.table import Table
 from rich.console import Console
 from pydbbackups.cli.config import build_config
 from pydbbackups.cli.services import BackupsService
 
 
 @click.group(invoke_without_command=True, no_args_is_help=True)
-@click.version_option('0.0.4', prog_name='dbbackups')
+@click.version_option('0.1.0', prog_name='dbbackups')
 def app():
     """ Awesome APP """
 
 
 @app.command(name='list')
 def get_backups():
     table = Table()
 
+    table.add_column('ID')
     table.add_column('Nombre')
     table.add_column('Base de datos')
     table.add_column('Fecha')
 
-    for bfile, bdata in BackupsService.list_backups():
-        table.add_row(bfile.name, bdata.database_name, bfile.date)
+    for _, bdata in BackupsService.list_backups():
+        table.add_row(
+            f"{bdata.id}",
+            f"{bdata.name}.{bdata.ext}",
+            bdata.database_name,
+            bdata.created_at.strftime('%d/%m/%y %H:%M:%S')
+        )
 
     console = Console()
     console.print(table)
 
 
 @app.command(name='dump')
 @click.option('--name', required=True)
 @click.option('--database-type', required=True, type=click.Choice(['postgres', 'mongodb']))
 @click.option('--host', required=True)
 @click.option('--database', required=True)
 @click.option('--username', default=None)
 @click.option('--password', default=None)
 @click.option('--without-password', default=False)
 @click.option('--port', default=None)
-@click.option('--compress', default=None)
-def make_backup(name: str, database_type, host, database, username, password, without_password, port, compress):
+@click.option('--compress', default=None, is_flag=True)
+@click.option('--format', default=None)
+@click.option('--file', required=False, default=None)
+def make_backup(name: str, database_type, host, database, username, password, without_password, port, compress, **kwargs):
     name = name.replace('-', '_')
 
     if without_password is False and password is None:
         password = getpass.getpass('Password: ')
 
     if without_password is True:
         password = None
@@ -50,19 +60,72 @@
     service = BackupsService.build(
         database_type,
         host=host,
         database=database,
         username=username,
         password=password,
         port=port,
-        compress=compress)
+    )
 
     console = Console()
     with console.status("[bold green]Dumping database ..."):
-        service.dump(name)
+        service.dump(name, compress=compress, **kwargs)
+        time.sleep(1)
+    console.print("[bold green] Backup created !")
+
+
+@app.command(name='restore')
+@click.option('--database-type', required=True, type=click.Choice(['postgres', 'mongodb']))
+@click.option('--host', required=True)
+@click.option('--port', default=None)
+@click.option('--database', required=True)
+@click.option('--username', required=True)
+@click.option('--password', default=None)
+@click.option('--without-password', default=False)
+def restore_backup(database_type, host, port, database, username, password, without_password):
+    if without_password is False and password is None:
+        password = getpass.getpass('Password: ')
+
+    if without_password is True:
+        password = None
+
+    service = BackupsService.build(
+        database_type,
+        host=host,
+        port=port,
+        database=database,
+        username=username,
+        password=password
+    )
+    console = Console()
+
+    backups = [v for v in BackupsService.list_backups()]
+    backups.sort(key=lambda v: v[1].id)
+    backups = [
+        f"{d.id} - {d.name}.{d.ext} - {d.database_name}" for _, d in backups]
+
+    questions = [
+        inquirer.List(
+            name='backup',
+            message='Select the backup to restore',
+            choices=backups
+        )
+    ]
+    answers = inquirer.prompt(questions)
+
+    if not answers:
+        raise ValueError('We need than you selected a backup to restore')
+
+    backup_id = int(answers['backup'].split(' - ')[0])
+    finded_backup = BackupsService.get_backup(backup_id)
+
+    with console.status("[bold green]Restoring backup ..."):
+        service.restore(finded_backup.backup)
+        time.sleep(1)
+    console.print("[bold green]Backup restored !")
 
 
 def main():
     build_config()
     app()
```

### Comparing `pydbbackups-0.0.4/pydbbackups/cli/services/backups.py` & `pydbbackups-0.1.0/pydbbackups/cli/services/backups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-from pydbbackups.cli.utils import get_backup_class, save_backup_file, get_backups_data, get_backups_files, DTEncoder
+from pydbbackups.cli.utils import get_backup_class, save_backup_file, get_backups_data, get_backups_files, DTEncoder, mongo_ext_formatter, postgres_ext_formatter
 from pydbbackups.cli.config import BACKUPS_DATA_DIR
 from pydbbackups.cli.models import BackupData, BackupFile
 
 from pydbbackups import Backup
 from datetime import datetime
 from dataclasses import asdict
 import json
+from pathlib import Path
+
+
+def backup_ext_formatter(db_type: str, name: str, **kwargs) -> str:
+    databases = {
+        "postgres": postgres_ext_formatter,
+        "mongodb": mongo_ext_formatter
+    }
+
+    formatter = databases.get(db_type, None)
+
+    if not formatter:
+        return name
+
+    return formatter(name, **kwargs)
 
 
 class BackupsService:
     backup_cls: Backup
     db_type: str
 
     def __init__(self, backup_cls: Backup = None) -> None:
@@ -25,36 +40,57 @@
 
     @staticmethod
     def list_backups():
         data = get_backups_data()
         backups = get_backups_files()
 
         for bfile in backups:
-            bdata = next((obj for obj in data if obj.name == bfile.name), None)
+            # Get the first object
+            bdata = next((obj for obj in data if obj.id == bfile.id), None)
             if not bdata:
                 continue
 
             yield bfile, bdata
 
-    def dump(self, name: str):
-        output = self.backup_cls.dump()
-        if not output:
-            return
+    @staticmethod
+    def get_backup(backup_id: int):
+        data = get_backups_data()
+        for v in data:
+            if v.id == backup_id:
+                return v
+
+    def dump(self, name: str, **kwargs):
+        output = self.backup_cls.dump(**kwargs)
+        content = output.read()
 
+        data = get_backups_data()
+        created_id = len(data)
         created_at = datetime.now()
-        meta = save_backup_file(BackupFile(
-            name, created_at, ""), output.read().decode('utf-8'))
-        print(meta.file, 'Created !')
 
-        data = get_backups_data()
+        name = backup_ext_formatter(
+            self.db_type, name, **kwargs)
+
+        if len(name.split('.')) > 1:
+            [name, ext] = name.split('.')
+
+        if not output or len(content) == 0:
+            print('Warning: This backup will not be saved')
+            return
+        else:
+            meta = save_backup_file(BackupFile(
+                id=created_id, name=name, ext=ext, file=Path()), content)
+            print(meta.file, 'Created !')
+
         data.append(BackupData(**{
             "id": len(data),
-            "name": name,
+            "name": meta.name,
+            "ext": meta.ext,
             "database_name": self.db_type,
+            "backup": meta.file,
             "created_at": created_at
         }))
 
         serialized_data = [asdict(v) for v in data]
         BACKUPS_DATA_DIR.write_text(json.dumps(serialized_data, cls=DTEncoder))
 
-    def restore(self):
-        self.backup_cls.restore()
+    def restore(self, backup: Path):
+        self.backup_cls.restore(backup)
```

### Comparing `pydbbackups-0.0.4/pydbbackups/errors.py` & `pydbbackups-0.1.0/pydbbackups/errors.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.4/PKG-INFO` & `pydbbackups-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pydbbackups
-Version: 0.0.4
+Version: 0.1.0
 Summary: DB backups handler
 Home-page: https://github.com/jbuendia1y/pydbbackups
 License: MIT
 Keywords: backups,databases,handler,library,cli
 Author: jbuendia1y
 Author-email: jgamer669@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pymongo (>=4.3.3,<5.0.0)
+Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Project-URL: Repository, https://github.com/jbuendia1y/pydbbackups
 Description-Content-Type: text/markdown
 
 # PyDBBackups
 
 A backup handler
@@ -35,34 +35,31 @@
     --name backup-example \
     --database-type postgres \
     --host localhost \
     --database test \
     --username postgres \
     --port 5432
 
-# backup-example___2023-04-10 11:42:59.090131 Created !
+# 0__backup-example.sql Created !
 ```
 
 ## Code example
 
 ```python
 from pydbbackups import Postgres
 
 cls = Postgres(
-    name="MyDB",
-    compress=False,
     database="test",
     host="localhost",
     port=5432,
     username="postgres",
     password="postgres"
 )
 
 # In some cases dump method, return None
-# Like MongoDB
 
 output = cls.dump()  # Return BytesIO
 print(output.read().decode('utf-8'))
 
 ```
 
 <p align="center">@jbuendia1y &#60;jbuendia1y@gmail.com&#62;</p>
```

