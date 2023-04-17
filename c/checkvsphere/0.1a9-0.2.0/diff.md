# Comparing `tmp/checkvsphere-0.1a9.tar.gz` & `tmp/checkvsphere-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.1a9.tar", last modified: Wed Mar 15 09:39:49 2023, max compression
+gzip compressed data, was "checkvsphere-0.2.0.tar", last modified: Mon Apr 17 12:59:03 2023, max compression
```

## Comparing `checkvsphere-0.1a9.tar` & `checkvsphere-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      264 2023-01-25 12:30:10.233192 checkvsphere-0.1a9/README.md
--rw-r--r--   0        0        0      174 2023-01-17 10:42:21.404433 checkvsphere-0.1a9/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3829 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16298 2022-12-02 09:15:25.388293 checkvsphere-0.1a9/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     5839 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2022-07-18 09:51:10.222733 checkvsphere-0.1a9/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2022-11-11 09:56:50.829790 checkvsphere-0.1a9/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2022-08-01 15:28:58.196194 checkvsphere-0.1a9/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1961 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6717 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     3434 2023-03-14 12:20:28.528461 checkvsphere-0.1a9/checkvsphere/vcmd/hosthealth.py
--rw-r--r--   0        0        0     4553 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0     9815 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4311 2023-03-14 16:23:36.452783 checkvsphere-0.1a9/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7833 2023-03-15 09:27:51.677211 checkvsphere-0.1a9/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2071 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3440 2023-03-14 15:32:45.464185 checkvsphere-0.1a9/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8238 2023-03-13 09:01:04.949489 checkvsphere-0.1a9/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     5050 2023-03-14 15:32:57.011973 checkvsphere-0.1a9/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0      939 2023-03-15 09:39:39.196408 checkvsphere-0.1a9/pyproject.toml
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 checkvsphere-0.1a9/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-04 13:33:00.767834 checkvsphere-0.2.0/README.md
+-rw-r--r--   0        0        0      174 2023-04-04 13:33:00.791833 checkvsphere-0.2.0/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     3882 2023-04-04 13:33:00.807833 checkvsphere-0.2.0/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-04-04 13:33:00.819833 checkvsphere-0.2.0/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16614 2023-04-04 13:33:00.827833 checkvsphere-0.2.0/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     6363 2023-04-06 12:14:26.650417 checkvsphere-0.2.0/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6534 2023-04-05 13:00:59.351204 checkvsphere-0.2.0/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     4520 2023-04-04 13:33:00.863832 checkvsphere-0.2.0/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0    10749 2023-04-04 13:33:00.879832 checkvsphere-0.2.0/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4065 2023-04-04 13:33:00.891832 checkvsphere-0.2.0/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7660 2023-04-04 13:33:00.895832 checkvsphere-0.2.0/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2039 2023-04-04 13:33:00.907831 checkvsphere-0.2.0/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3366 2023-04-04 13:33:00.915831 checkvsphere-0.2.0/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8332 2023-04-05 13:30:02.707750 checkvsphere-0.2.0/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     4958 2023-04-04 13:33:00.939831 checkvsphere-0.2.0/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0     8969 2023-04-06 12:26:23.457744 checkvsphere-0.2.0/checkvsphere/vcmd/vsan.py
+-rw-r--r--   0        0        0      941 2023-04-17 12:58:29.769761 checkvsphere-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 checkvsphere-0.2.0/PKG-INFO
```

### Comparing `checkvsphere-0.1a9/checkvsphere/cli.py` & `checkvsphere-0.2.0/checkvsphere/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     try:
         cmd = sys.argv.pop(1)
     except:
         pass
 
     set_timeout()
 
-    if cmd:
+    if cmd and cmd not in ['-h', 'help', '--help']:
         mod = "".join(c for c in cmd if c.isalnum())
         try:
             runner = importlib.import_module(f"checkvsphere.vcmd.{mod}")
         except ModuleNotFoundError as e:
-            if not e.name.startswith("vcmd."):
+            if not e.name.startswith("checkvsphere.vcmd."):
                 raise e
             print(f"command not found: {cmd}")
             sys.exit(3)
         try:
             sys.argv[0] = f"{sys.argv[0]} {runner.__cmd__}"
         except:
             sys.argv[0] = f"{sys.argv[0]} {cmd}"
```

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/__init__.py` & `checkvsphere-0.2.0/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/cli.py` & `checkvsphere-0.2.0/checkvsphere/tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,20 @@
                                                     'can also be set by env VSPHERE_PASS')
 
         self._standard_args_group.add_argument('-nossl', '--disable-ssl-verification',
                                                required=False,
                                                action='store_true',
                                                help='Disable ssl host certificate verification')
 
+        self._standard_args_group.add_argument('-v', '--verbose',
+                                               required=False,
+                                               default=0,
+                                               action='count',
+                                               help='verbosity')
+
     def get_args(self):
         """
         Supports the command-line arguments needed to form a connection to vSphere.
         """
         args = self._parser.parse_args()
         return args
```

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/helper.py` & `checkvsphere-0.2.0/checkvsphere/tools/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,51 +144,70 @@
     }
 
     CRITICAL_THRESHOLD = {
         'name_or_flags': ['--critical'],
         'options': {'action': 'store', 'help': 'critical threshold'},
     }
 
-    def ALLOWED(help):
+    def ALLOWED(help, name=None):
+        if not name:
+            name = ['--allowed', '--include']
         return {
-            'name_or_flags': ['--allowed'],
+            'name_or_flags': name,
             'options': {
                 'default': [],
                 'help': help,
                 'action': 'append',
             }
         }
-    def BANNED(help):
+    def BANNED(help, name=None):
+        if not name:
+            name = ['--banned', '--exclude']
         return {
-            'name_or_flags': ['--banned'],
+            'name_or_flags': name,
             'options': {
                 'default': [],
                 'help': help,
                 'action': 'append',
             }
         }
 
 
-def isbanned(args, name):
+def isbanned(args, name, attr='banned'):
     '''
     checks name against regexes in args.banned
     '''
-    if args.banned:
-        for pattern in args.banned:
+    banned = getattr(args, attr, None)
+    if banned:
+        for pattern in banned:
             p = re.compile(pattern)
             if p.search(name):
                 return True
 
     return False
 
-def isallowed(args, name):
+def isallowed(args, name, attr='allowed'):
     '''
     checks name against regexes in args.allowed
     '''
-    if args.allowed:
-        for pattern in args.allowed:
+    allowed = getattr(args, attr, None)
+    if allowed:
+        for pattern in allowed:
             p = re.compile(pattern)
             if p.search(name):
                 return True
         return False
 
     return True
+
+def process_retrieve_content(content):
+    """
+    reorganize RetrieveContents shit, so we can use it.
+    """
+    objs = []
+    for o in content:
+        d = {}
+        d['moref'] = o.obj
+        for prop in o.propSet:
+            d[prop.name] = prop.val
+        objs.append(d)
+    return objs
```

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/pchelper.py` & `checkvsphere-0.2.0/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/service_instance.py` & `checkvsphere-0.2.0/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a9/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.2.0/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/about.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/about.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 """
 
 __cmd__ = 'about'
 
 import logging
 from ..tools.helper import find_entity_views
 from pyVmomi import vim
-from pyVim.task import WaitForTask
 from ..tools import cli, service_instance
-from http.client import HTTPConnection
 from .. import CheckVsphereException
 
 
 def run():
     try:
         parser = cli.Parser()
         # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/datastores.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,16 +20,22 @@
 """
 
 __cmd__ = 'datastores'
 
 from pyVmomi import vim, vmodl
 from monplugin import Check, Status, Threshold, Range
 from ..tools import cli, service_instance
-from ..tools.helper import find_entity_views, CheckArgument, isbanned, isallowed
 from .. import CheckVsphereException
+from ..tools.helper import (
+    CheckArgument,
+    find_entity_views,
+    isallowed,
+    isbanned,
+    process_retrieve_content
+)
 
 class Space:
     def __init__(self, capacity, free):
         self.capacity = capacity
         self.free = free
         self.used = capacity - free
         self.usage = 100 * self.used / capacity
@@ -88,31 +94,31 @@
     })
     args = parser.get_args()
 
     si = service_instance.connect(args)
     check = Check(shortname='VSPHERE-VOL', threshold = Threshold(args.warning or None, args.critical or None))
 
     vimtype = None
-    if args.vimname and args.vimtype:
+    if args.vimtype:
         vimtype = getattr(vim, args.vimtype)
 
     datastores = []
 
     if vimtype in [vim.HostSystem, vim.ClusterComputeResource]:
         try:
             vm = find_entity_views(
                 si,
                 vimtype,
                 begin_entity=si.content.rootFolder,
-                sieve={'name': args.vimname},
+                sieve=( {'name': args.vimname} if args.vimname else None ),
                 properties=["name", "datastore"],
             )[0]
             datastores = vm['props']['datastore']
         except IndexError:
-            check.exit(Status.UNKNOWN, f"host {args.vihost} not found")
+            check.exit(Status.UNKNOWN, f"{args.vimtype} {args.vimname} not found")
     else:
         dcs = find_entity_views(
             si,
             vim.Datacenter,
             begin_entity=si.content.rootFolder,
             properties=["datastore"],
         )
@@ -136,15 +142,15 @@
 
     filter_spec = vmodl.query.PropertyCollector.FilterSpec(
         objectSet = objs,
         propSet = [propspec],
     )
 
     result = retrieve( [filter_spec] )
-    stores = fix_content(result)
+    stores = process_retrieve_content(result)
 
 
     for store in stores:
 
         name = store['summary'].name
         datastore_type = store['summary'].type
 
@@ -175,32 +181,18 @@
                     threshold['critical'] = range_in_bytes(Range(args.critical), uom)
                 opts['threshold'] = Threshold(**threshold)
 
                 if s != Status.OK:
                     check.add_message(s, f"{args.metric} on {name} is in state {s.name}: {value :.2f}{uom}")
 
             puom = '%' if metric == 'usage' else 'B'
-            check.add_perfdata(label=f"{name} {metric}", value=space[metric], uom=puom, **opts)
+            check.add_perfmultidata(name, 'datastores',  label=metric, value=space[metric], uom=puom, **opts)
 
     (code, message) = check.check_messages(separator="\n")#, allok=okmessage)
     check.exit(
         code=code,
         message=( message or "everything ok" )
     )
 
 
-def fix_content(content):
-    """
-    reorganize RetrieveContents shit, so we can use it.
-    """
-    objs = []
-    for o in content:
-        d = {}
-        d['moref'] = o.obj
-        for prop in o.propSet:
-            d[prop.name] = prop.val
-        objs.append(d)
-    return objs
-
-
 if __name__ == "__main__":
     run()
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/hosthealth.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/media.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,101 +13,88 @@
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """
---select runtime --subselect health
+checks if there are any vms on a host that have connected cd or floppy drives
+
+This is not good because vms cannot move hosts with mounted cds/floppies
 """
 
-__cmd__ = None # not finished yet 'host-health'
+__cmd__ = 'media'
 
 import logging
 from pyVmomi import vim
-from pyVim.task import WaitForTask
-from http.client import HTTPConnection
+from monplugin import Check, Status
+from .. import CheckVsphereException
 from ..tools import cli, service_instance
-from ..tools.helper import get_obj_by_name, get_metric, CheckArgument
-from ..tools.helper import find_entity_views, get_obj_by_name, get_metric
-from monplugin import Check, Status, Threshold
-
-def health_status(color):
-    return {
-        'red': Status.CRITICAL,
-        'yellow': Status.WARNING,
-        'green': Status.OK
-    }.get(color.lower(), Status.UNKNOWN)
-
+from ..tools.helper import find_entity_views, isbanned, isallowed, CheckArgument
 
 def run():
-    parser = get_argparser()
+    parser = cli.Parser()
+    # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
+    parser.add_optional_arguments(cli.Argument.VIHOST)
+    parser.add_optional_arguments(CheckArgument.ALLOWED('regex match against vm name'))
+    parser.add_optional_arguments(CheckArgument.BANNED('regex match against vm name'))
     args = parser.get_args()
+    si = service_instance.connect(args)
 
-    check = Check(shortname="VSPHERE-HOSTHEALTH")
+    check = Check(shortname='VSPHERE-MEDIA')
 
-    args._si = service_instance.connect(args)
+    if args.vihost:
+        host_view = si.content.viewManager.CreateContainerView(
+            si.content.rootFolder, [vim.HostSystem], True)
+        try:
+            parentView = next(x for x in host_view.view if x.name.lower() == args.vihost.lower())
+        except:
+            raise CheckVsphereException(f"host {args.vihost} not found")
+    else:
+        parentView = si.content.rootFolder
 
+    #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     vms = find_entity_views(
-        args._si,
-        vim.HostSystem,
-        begin_entity=args._si.content.rootFolder,
-        sieve={'name': args.vihost},
-        properties=['runtime', 'overallStatus', 'configIssue', 'summary.config.product.fullName']
-    )
-
-    try:
-        obj = vms[0]['obj'].obj
-        props = vms[0]['props']
-    except IndexError:
-        check.exit(Status.UNKNOWN, f"{args.vimtype} {args.vimname} not found")
-
-    if 'runtime.inMaintenanceMode' in props:
-        status = getattr(Status, args.maintenance_state)
-        if props['runtime.inMaintenanceMode']:
-            check.exit(status, f"{args.vimname} is in maintenance")
-
-def get_perf_values(args, obj, metricId):
-    si = args._si
-
-    perfMgr = si.content.perfManager
-
-    perfQuerySpec = []
-    perfQuerySpec.append(
-        vim.PerformanceManager.QuerySpec(
-            maxSample=1,
-            entity=obj,
-            metricId=[metricId],
-            intervalId=args.interval,
-        )
+        si,
+        vim.VirtualMachine,
+        begin_entity=parentView,
+        properties=['name', 'config.hardware.device', 'config.template']
     )
 
-    perfData = perfMgr.QueryPerf(querySpec=perfQuerySpec)
-    return perfData
+    result = []
 
+    check.add_message(
+        Status.OK,
+        "no connected cdrom/floppy drives found"
+    )
 
-def get_argparser():
-    parser = cli.Parser()
-    parser.add_required_arguments(cli.Argument.VIHOST)
-    parser.add_optional_arguments( {
-        'name_or_flags': ['--maintenance-state'],
-        'options': {
-            'action': 'store',
-            'choices': ['OK', 'WARNING', 'CRITICAL', 'UNKNOWN'],
-            'default': 'UNKNOWN',
-            'help': 'exit with this status if the host is in maintenance, only does something with --vimtype HostSystem'
-        }
-    })
-
-    return parser
+    for vm in vms:
+        match = 0
+        if isbanned(args, vm['props']['name']):
+            continue
+        if not isallowed(args, vm['props']['name']):
+            continue
+
+        if vm['props']['config.template']:
+            # This vm is a template, ignore it
+            continue
+        for device in vm['props']['config.hardware.device']:
+            if \
+                (isinstance(device, vim.vm.device.VirtualCdrom)
+                 or isinstance(device, vim.vm.device.VirtualFloppy)) \
+                    and device.connectable.connected:
+                match += 1
+        if match > 0:
+            check.add_message(
+                Status.CRITICAL,
+                f'{vm["props"]["name"]} has cdrom/floppy drives connected'
+            )
+
+    (code, message) = check.check_messages(separator=' - ')
+    check.exit(
+        code=code,
+        message=message
+    )
 
 
 if __name__ == "__main__":
-    try:
-        run()
-    except SystemExit as e:
-        if e.code > 3 or e.code < 0:
-            print("UNKNOWN EXIT CODE")
-            raise SystemExit(Status.UNKNOWN)
-    except Exception as e:
-        print("UNKNOWN - " + str(e))
-        raise SystemExit(Status.UNKNOWN)
+    run()
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/hostnic.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,24 @@
 Check NICs on the host
 """
 
 __cmd__ = 'host-nic'
 
 import logging
 from pyVmomi import vim
-from pyVim.task import WaitForTask
 from monplugin import Check, Status
-from http.client import HTTPConnection
 from ..tools import cli, service_instance
 from ..tools.helper import find_entity_views, CheckArgument, isbanned
 from .. import CheckVsphereException
 
 
 def run():
     parser = cli.Parser()
     # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
-    parser.add_required_arguments(cli.Argument.VIHOST)
+    parser.add_optional_arguments(cli.Argument.VIHOST)
     parser.add_optional_arguments(CheckArgument.BANNED(
         'regex, check against nic name'
     ))
     parser.add_optional_arguments( {
         'name_or_flags': ['--maintenance-state'],
         'options': {
             'action': 'store',
@@ -74,27 +72,27 @@
 
     #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     try:
         vm = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
-            sieve={'name': args.vihost},
+            sieve=({'name': args.vihost} if args.vihost else None),
             properties=["name", "configManager.networkSystem", "runtime.inMaintenanceMode"]
         )[0]
     except IndexError:
-        check.exit(Status.UNKNOWN, f"host {args.vihost} not found")
+        check.exit(Status.UNKNOWN, f"host {args.vihost or ''} not found")
 
     result = []
 
     if vm['props']['runtime.inMaintenanceMode']:
         status = getattr(Status, args.maintenance_state)
         check.exit(
             status,
-            f"host {args.vihost} is in maintenance"
+            f"host {vm['props']['name']} is in maintenance"
         )
 
     network_system = vm["props"]["configManager.networkSystem"]
     network_info = network_system.networkInfo
 
     if not network_info:
         check.exit(
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/hostruntime.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,27 +18,25 @@
 """
 check various runtime info from a host
 """
 
 __cmd__ = 'host-runtime'
 
 import logging
-from ..tools.helper import find_entity_views
 from pyVmomi import vim
-from pyVim.task import WaitForTask
-from ..tools import cli, service_instance
 from monplugin import Check, Status
-from http.client import HTTPConnection
 from .. import CheckVsphereException
+from ..tools import cli, service_instance
+from ..tools.helper import find_entity_views, isbanned, isallowed, CheckArgument
 
 
 def run():
     parser = cli.Parser()
     # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
-    parser.add_required_arguments(cli.Argument.VIHOST)
+    parser.add_optional_arguments(cli.Argument.VIHOST)
 
     parser.add_required_arguments( {
         'name_or_flags': ['--mode'],
         'options': {
             'action': 'store',
             'choices': [
                 'con',
@@ -59,14 +57,17 @@
             'action': 'store',
             'choices': ['OK', 'WARNING', 'CRITICAL', 'UNKNOWN'],
             'help': 'exit with this status if the host is in maintenance, '
                     'default UNKNOWN, or CRITICAL if --mode maintenance'
         }
     })
 
+    parser.add_optional_arguments(CheckArgument.ALLOWED('regex, name of info item'))
+    parser.add_optional_arguments(CheckArgument.BANNED('regex, name of info item'))
+
     args = parser.get_args()
 
     # default value differs if mode == maintenance
     if not args.maintenance_state:
         args.maintenance_state = 'CRITICAL' if args.mode == 'maintenance' else 'UNKNOWN'
 
     si = service_instance.connect(args)
@@ -75,27 +76,27 @@
 
     #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     try:
         vm = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
-            sieve={'name': args.vihost},
+            sieve=({'name': args.vihost} if args.vihost else None),
             properties=['name', 'runtime', 'overallStatus', 'configIssue', 'summary.config']
         )[0]
     except IndexError:
-        check.exit(Status.UNKNOWN, f"host {args.vihost} not found")
+        check.exit(Status.UNKNOWN, f"host {args.vihost or ''} not found")
 
     result = []
 
     if vm['props']['runtime'].inMaintenanceMode:
         status = getattr(Status, args.maintenance_state)
         check.exit(
             status,
-            f"host {args.vihost} is in maintenance"
+            f"host {vm['props']['name']} is in maintenance"
         )
 
     okmessage = "No errors"
 
     if args.mode == "health":
         okmessage = check_health(check, vm, args, result)
     elif args.mode == "status":
@@ -108,15 +109,19 @@
         okmessage = check_issues(check, vm, args, result)
     elif args.mode == "version":
         version = vm['obj'].obj.summary.config.product.fullName
         check.exit(Status.OK, version)
     elif args.mode == 'maintenance':
         check.exit(Status.OK, "Host is not in maintenance")
 
-    (code, message) = check.check_messages(separator="\n", separator_all='\n', allok=okmessage)
+    opts = {}
+    if not args.verbose:
+        opts['allok'] = okmessage
+
+    (code, message) = check.check_messages(separator="\n", separator_all='\n', **opts)
     check.exit(
         code=code,
         message=( message or  "everything ok" )
     )
 
 def format_issue(issue):
     things = [
@@ -144,14 +149,18 @@
 
     return ", ".join(formattedThings)
 
 
 def check_issues(check, vm, args, result):
     issues = vm['props']['configIssue']
     for issue in issues:
+        if isbanned(args, issue.fullFormattedMessage):
+            continue
+        if not isallowed(args, issue.fullFormattedMessage):
+            continue
         check.add_message(Status.CRITICAL, format_issue(issue))
 
     return "No issues found"
 
 
 def check_con(check, vm, args, result):
     con = vm['props']['runtime'].connectionState
@@ -179,14 +188,18 @@
             "Temperature status unavailable"
         )
 
     numericinfo = systemRuntime.systemHealthInfo.numericSensorInfo
     for info in numericinfo:
         if info.sensorType != "temperature":
             continue
+        if isbanned(args, info.name):
+            continue
+        if not isallowed(args, info.name):
+            continue
         state = health2state(info.healthState.key)
         name = info.name.rstrip(' Temp')
         check.add_perfdata(label=name, value=info.currentReading * (10 ** info.unitModifier))
         check.add_message(state, f"{name} is {info.healthState.key}")
 
     return "All temperature sensors green"
 
@@ -201,14 +214,18 @@
 
     count = {}
 
     # "[$status2text{$fstate}] [Type: $type] [Name: $item_ref->{name}] [Label: $item_ref->{label}] [Summary: $item_ref->{summary}]$multiline";
     if memorystatus:
         for info in memorystatus:
             state = health2state(info.status.key)
+            if isbanned(args, info.name):
+                continue
+            if not isallowed(args, info.name):
+                continue
             if state == Status.UNKNOWN:
                 continue
             check.add_message(state, f"{state.name} [Type: Memory] [Name: { info.name }] [Summary: { info.status.summary }]")
             count.setdefault('memory', 0)
             count['memory'] += 1
 
     if cpustatus:
@@ -223,30 +240,38 @@
                 )
             check.add_message(state, f"{state.name} [Type: CPU] [Name: { info.name }] [Summary: { info.status.summary }]")
             count.setdefault('cpu', 0)
             count['cpu'] += 1
 
     if storagestatus:
         for info in storagestatus:
+            if isbanned(args, info.name):
+                continue
+            if not isallowed(args, info.name):
+                continue
             state = health2state(info.status.key)
             if state == Status.UNKNOWN:
                 continue
 
             check.add_message(state, f"{state.name} [Type: Memory] [Name: { info.name }] [Summary: { info.status.summary }]")
             count.setdefault('storage', 0)
             count['storage'] += 1
 
 
     if numericsensor:
         for info in numericsensor:
             if info.sensorType == "Software Components":
                 # It is said they make no sense
                 continue
+            if isbanned(args, info.name):
+                continue
+            if not isallowed(args, info.name):
+                continue
             if 'unknown' in info.healthState.label and 'Cannot report' in info.healthState.summary:
-                # Filter out sensors which have not valid data. Often a sensor is recognized by vmware
+                # Filter out sensors which have no valid data. Often a sensor is recognized by vmware
                 # but has not the ability to report something senseful. So it can be skipped.
                 continue
 
             state = health2state(info.healthState.key)
             if state == Status.UNKNOWN:
                 continue
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/hostservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,40 @@
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 check services on host
 """
 
-__cmd__ = 'host-services'
+__cmd__ = 'host-service'
 
 import logging
 from pyVmomi import vim, vmodl
-from pyVim.task import WaitForTask
 from monplugin import Check, Status
-from http.client import HTTPConnection
 from ..tools import cli, service_instance
-from ..tools.helper import find_entity_views, CheckArgument, isbanned, isallowed
 from .. import CheckVsphereException
+from ..tools.helper import (
+    CheckArgument,
+    find_entity_views,
+    isallowed,
+    isbanned,
+    process_retrieve_content
+)
 
 def run():
     global args
     parser = cli.Parser()
     parser.add_optional_arguments(CheckArgument.BANNED('regex, name of datastore'))
     parser.add_optional_arguments(CheckArgument.ALLOWED('regex, name of datastore'))
-    parser.add_required_arguments(cli.Argument.VIHOST)
+    parser.add_optional_arguments(cli.Argument.VIHOST)
     parser.add_optional_arguments({
         'name_or_flags': ['--maintenance-state'],
-        'default': 'UNKNOWN',
         'options': {
             'action': 'store',
+            'default': 'UNKNOWN',
             'choices': ['OK', 'WARNING', 'CRITICAL', 'UNKNOWN'],
             'help': 'exit with this status if the host is in maintenance, '
                     'default UNKNOWN, or CRITICAL if --mode maintenance'
         }
     })
     args = parser.get_args()
 
@@ -52,25 +56,25 @@
     check = Check(shortname='VSPHERE-SERVICE')
 
     try:
         host = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
-            sieve={'name': args.vihost},
+            sieve=( {'name': args.vihost} if args.vihost else None ),
             properties=["name", "configManager", "runtime.inMaintenanceMode"],
         )[0]
     except IndexError:
-        check.exit(Status.UNKNOWN, f"host {args.vihost} not found")
+        check.exit(Status.UNKNOWN, f"host {args.vihost or ''} not found")
 
     if host['props']['runtime.inMaintenanceMode']:
         status = getattr(Status, args.maintenance_state)
         check.exit(
             status,
-            f"host {args.vihost} is in maintenance"
+            f"host {host['props']['name']} is in maintenance"
         )
 
     count = {
         'running': 0,
         'not running': 0,
     }
     serviceSystem = service_system(si, host)
@@ -107,25 +111,12 @@
 
     filter_spec = vmodl.query.PropertyCollector.FilterSpec(
         objectSet = objs,
         propSet = [propspec],
     )
 
     result = retrieve( [filter_spec] )
-    service_system = fix_content(result)
+    service_system = process_retrieve_content(result)
     return service_system[0]
 
-def fix_content(content):
-    """
-    reorganize RetrieveContents shit, so we can use it.
-    """
-    objs = []
-    for o in content:
-        d = {}
-        d['moref'] = o.obj
-        for prop in o.propSet:
-            d[prop.name] = prop.val
-        objs.append(d)
-    return objs
-
 if __name__ == "__main__":
     run()
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/hoststorage.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,43 +21,49 @@
 
 __cmd__ = 'host-storage'
 
 import re
 from pyVmomi import vim, vmodl
 from monplugin import Check, Status, Threshold, Range
 from ..tools import cli, service_instance
-from ..tools.helper import find_entity_views, CheckArgument, isbanned, isallowed
 from .. import CheckVsphereException
+from ..tools.helper import (
+    CheckArgument,
+    find_entity_views,
+    isallowed,
+    isbanned,
+    process_retrieve_content
+)
 
 args = None
 
 def run():
     global args
     parser = cli.Parser()
     #parser.add_optional_arguments(CheckArgument.CRITICAL_THRESHOLD)
     #parser.add_optional_arguments(CheckArgument.WARNING_THRESHOLD)
     parser.add_optional_arguments(CheckArgument.BANNED('regex, name of datastore'))
     parser.add_optional_arguments(CheckArgument.ALLOWED('regex, name of datastore'))
-    parser.add_required_arguments(cli.Argument.VIHOST)
+    parser.add_optional_arguments(cli.Argument.VIHOST)
     parser.add_required_arguments( {
         'name_or_flags': ['--mode'],
         'options': {
             'action': 'store',
             'choices': [
                 'adapter',
                 'lun',
             ],
             'help': 'which runtime mode to check'
         }
     })
     parser.add_optional_arguments({
         'name_or_flags': ['--maintenance-state'],
-        'default': 'UNKNOWN',
         'options': {
             'action': 'store',
+            'default': 'UNKNOWN',
             'choices': ['OK', 'WARNING', 'CRITICAL', 'UNKNOWN'],
             'help': 'exit with this status if the host is in maintenance, '
                     'default UNKNOWN, or CRITICAL if --mode maintenance'
         }
     })
     args = parser.get_args()
 
@@ -65,25 +71,25 @@
     check = Check(shortname='VSPHERE-STORAGE')
 
     try:
         host = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
-            sieve={'name': args.vihost},
+            sieve=( {'name': args.vihost} if args.vihost else None ),
             properties=["name", "configManager", "runtime.inMaintenanceMode"],
         )[0]
     except IndexError:
-        check.exit(Status.UNKNOWN, f"host {args.vihost} not found")
+        check.exit(Status.UNKNOWN, f"host {args.vihost or ''} not found")
 
     if host['props']['runtime.inMaintenanceMode']:
         status = getattr(Status, args.maintenance_state)
         check.exit(
             status,
-            f"host {args.vihost} is in maintenance"
+            f"host {host['props']['name']} is in maintenance"
         )
 
     storage = storage_info(si, host)
 
     if args.mode == "adapter":
         check_adapter(check, args, storage)
     elif args.mode == "lun":
@@ -207,27 +213,12 @@
 
     filter_spec = vmodl.query.PropertyCollector.FilterSpec(
         objectSet = objs,
         propSet = [propspec],
     )
 
     result = retrieve( [filter_spec] )
-    storage = fix_content(result)
+    storage = process_retrieve_content(result)
     return storage[0]
 
-
-def fix_content(content):
-    """
-    reorganize RetrieveContents shit, so we can use it.
-    """
-    objs = []
-    for o in content:
-        d = {}
-        d['moref'] = o.obj
-        for prop in o.propSet:
-            d[prop.name] = prop.val
-        objs.append(d)
-    return objs
-
-
 if __name__ == "__main__":
     run()
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/listmetrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 __cmd__ = 'list-metrics'
 
 import logging
 import textwrap
 from pyVmomi import vim
 from ..tools import cli, service_instance
-from pprint import pprint as pp
 
 def run():
     parser = cli.Parser()
     args = parser.get_args()
     si = service_instance.connect(args)
     perfMgr = si.content.perfManager
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/perf.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/perf.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,16 @@
 check performance values from Vsphere
 """
 
 __cmd__ = 'perf'
 
 import logging
 from pyVmomi import vim
-from pyVim.task import WaitForTask
-from http.client import HTTPConnection
 from ..tools import cli, service_instance
-from ..tools.helper import get_obj_by_name, get_metric, CheckArgument
-from ..tools.helper import find_entity_views, get_obj_by_name, get_metric
-from pprint import pprint as pp
+from ..tools.helper import find_entity_views, get_metric, CheckArgument
 from monplugin import Check, Status, Threshold
 
 '''
 [kiloBytes]
 [megaBytes]
 [teraBytes]
 [percent]
@@ -102,36 +98,37 @@
 
     # I hate you so much vmware
     # https://vdc-download.vmware.com/vmwb-repository/dcr-public/bf660c0a-f060-46e8-a94d-4b5e6ffc77ad/208bc706-e281-49b6-a0ce-b402ec19ef82/SDK/vsphere-ws/docs/ReferenceGuide/cpu_counters.html
 
     vms = find_entity_views(
         args._si,
         vimtype,
+        properties=['name'],
         begin_entity=args._si.content.rootFolder,
-        sieve={'name': args.vimname},
+        sieve=( {'name': args.vimname} if args.vimname else None )
     )
 
     try:
         obj = vms[0]['obj'].obj
         props = vms[0]['props']
     except IndexError:
-        check.exit(Status.UNKNOWN, f"{args.vimtype} {args.vimname} not found")
+        check.exit(Status.UNKNOWN, f"{args.vimtype} {args.vimname or ''} not found")
 
     if not metricId:
         raise Exception(
             f"metric not found by {args.perfcounter}:{args.perfinstance}, "
             "maybe --perfinstance='*' helps to examine the available instances"
         )
     if not obj:
         raise Exception(f"vim.{args.vimtype} not found with name {args.vimname}")
 
     if 'runtime.inMaintenanceMode' in props:
         status = getattr(Status, args.maintenance_state)
         if props['runtime.inMaintenanceMode']:
-            check.exit(status, f"{args.vimname} is in maintenance")
+            check.exit(status, f"{args.vimname or props['name']} is in maintenance")
 
     counterInfo = get_counter_info(counter)
 
     try:
         values = get_perf_values(args, obj, metricId)[0]
     except IndexError:
         check.exit(Status.UNKNOWN, f"Cannot find {args.perfcounter} for the queried resources")
@@ -139,33 +136,37 @@
     if not values.value:
         check.exit(code=Status.UNKNOWN, message="No data returned")
 
     if args.perfinstance == '':
         for instance in values.value:
             val = instance.value[0] * counterInfo['factor']
             if instance.id.instance == args.perfinstance:
-                check.add_perfdata(
+                check.add_perfmultidata(
+                    args.perfcounter if instance.id.instance == '' else instance.id.instance,
+                    'perf',
                     label=args.perfcounter,
                     value=val,
                     threshold=check.threshold,
                     uom=counterInfo['perfUnit'],
                 )
                 check.exit(
                     code=check.check_threshold(val),
-                    message=f'Counter {args.perfcounter} on {args.vimtype}:{args.vimname} reported {val} {counterInfo["unit"]}',
+                    message=f'Counter {args.perfcounter} on {args.vimtype}:{args.vimname or props["name"]} reported {val} {counterInfo["unit"]}',
                 )
     else:
         for instance in values.value:
             if instance.id.instance == '':
                 # ignore the aggregate if we query a specific or all instances
                 continue
             if args.perfinstance == '*' or args.perfinstance == instance.id.instance:
                 val = instance.value[0] * counterInfo['factor']
-                check.add_perfdata(
-                    label=f'{args.perfcounter}_{instance.id.instance}',
+                check.add_perfmultidata(
+                    instance.id.instance,
+                    'perf',
+                    label=args.perfcounter,
                     value=val,
                     threshold=check.threshold,
                     uom=counterInfo['perfUnit'],
                 )
                 check.add_message(
                     check.threshold.get_status(val),
                     f"{args.perfcounter}_{instance.id.instance} has value {val} {counterInfo['unit']}",
@@ -205,16 +206,16 @@
             'action': 'store',
             'choices': ['OK', 'WARNING', 'CRITICAL', 'UNKNOWN'],
             'default': 'UNKNOWN',
             'help': 'exit with this status if the host is in maintenance, only does something with --vimtype HostSystem'
         }
     })
 
-    parser.add_required_arguments( CheckArgument.VIMNAME )
     parser.add_required_arguments( CheckArgument.VIMTYPE )
+    parser.add_optional_arguments( CheckArgument.VIMNAME )
 
     parser.add_required_arguments(
         {
             'name_or_flags': ['--perfcounter'],
             'options': {
                 'action': 'store',
                 'help': 'a colon separated string composed of groupInfo.key:nameInfo.key:rollupType',
```

### Comparing `checkvsphere-0.1a9/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.2.0/checkvsphere/vcmd/snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,21 @@
 check age or number of vm snapshots
 """
 
 __cmd__ = 'snapshots'
 
 import logging
 from pyVmomi import vim
-from pyVim.task import WaitForTask
-from http.client import HTTPConnection
 from monplugin import Check, Status, Threshold
 from ..tools import cli, service_instance
 from datetime import datetime, timedelta, timezone
 from ..tools.helper import (
 	CheckArgument,
 	find_entity_views,
 	get_metric,
-	get_obj_by_name,
     isbanned,
     isallowed
 )
 
 check = None
 args = None
```

### Comparing `checkvsphere-0.1a9/pyproject.toml` & `checkvsphere-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.1a9"
+version = "0.2.0"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
-    "monplugin >= 0.4",
+    "monplugin >= 0.5.1",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
 ]
```

### Comparing `checkvsphere-0.1a9/PKG-INFO` & `checkvsphere-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.1a9
+Version: 0.2.0
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Dist: pyvmomi >= 8.0.0.1, < 9
-Requires-Dist: monplugin >= 0.4
+Requires-Dist: monplugin >= 0.5.1
 Project-URL: documentation, https://consol.github.io/check_vsphere
 Project-URL: homepage, https://github.com/consol/check_vsphere
 Project-URL: issues, https://github.com/consol/check_vsphere/issues
 Project-URL: repository, https://github.com/consol/check_vsphere.git
 
 [Documentation](https://consol.github.io/check_vsphere/#/)
```

