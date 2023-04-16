# Comparing `tmp/asu-0.7.8.tar.gz` & `tmp/asu-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asu-0.7.8.tar", max compression
+gzip compressed data, was "asu-0.7.9.tar", max compression
```

## Comparing `asu-0.7.8.tar` & `asu-0.7.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    18092 2022-07-10 21:02:13.475808 asu-0.7.8/LICENSE
--rw-r--r--   0        0        0     5118 2022-07-10 21:02:13.475808 asu-0.7.8/README.md
--rw-r--r--   0        0        0       22 2022-07-10 21:02:21.892093 asu-0.7.8/asu/__init__.py
--rw-r--r--   0        0        0    10091 2022-07-10 21:02:13.475808 asu-0.7.8/asu/api.py
--rw-r--r--   0        0        0     4592 2022-07-10 21:02:13.475808 asu-0.7.8/asu/asu.py
--rw-r--r--   0        0        0    13293 2022-07-10 21:02:13.475808 asu-0.7.8/asu/build.py
--rw-r--r--   0        0        0     4201 2022-07-10 21:02:13.475808 asu-0.7.8/asu/common.py
--rw-r--r--   0        0        0    13763 2022-07-10 21:02:13.475808 asu-0.7.8/asu/janitor.py
--rw-r--r--   0        0        0     1085 2022-07-10 21:02:13.475808 asu-0.7.8/asu/metrics.py
--rw-r--r--   0        0        0    17625 2022-07-10 21:02:13.475808 asu-0.7.8/asu/openapi.yml
--rw-r--r--   0        0        0    56815 2022-07-10 21:02:13.475808 asu-0.7.8/asu/static/logo.png
--rw-r--r--   0        0        0     6771 2022-07-10 21:02:13.475808 asu-0.7.8/asu/static/style.css
--rw-r--r--   0        0        0     2675 2022-07-10 21:02:13.475808 asu-0.7.8/asu/templates/overview.html
--rw-r--r--   0        0        0      697 2022-07-10 21:02:22.352108 asu-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     6108 2022-07-10 21:02:23.250056 asu-0.7.8/setup.py
--rw-r--r--   0        0        0     6002 2022-07-10 21:02:23.250507 asu-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    18092 2022-07-13 18:38:50.039452 asu-0.7.9/LICENSE
+-rw-r--r--   0        0        0     5118 2022-07-13 18:38:50.039452 asu-0.7.9/README.md
+-rw-r--r--   0        0        0       22 2022-07-13 18:38:58.203447 asu-0.7.9/asu/__init__.py
+-rw-r--r--   0        0        0    10091 2022-07-13 18:38:50.039452 asu-0.7.9/asu/api.py
+-rw-r--r--   0        0        0     4592 2022-07-13 18:38:50.039452 asu-0.7.9/asu/asu.py
+-rw-r--r--   0        0        0    13293 2022-07-13 18:38:50.039452 asu-0.7.9/asu/build.py
+-rw-r--r--   0        0        0     4201 2022-07-13 18:38:50.039452 asu-0.7.9/asu/common.py
+-rw-r--r--   0        0        0    13636 2022-07-13 18:38:50.039452 asu-0.7.9/asu/janitor.py
+-rw-r--r--   0        0        0     1085 2022-07-13 18:38:50.039452 asu-0.7.9/asu/metrics.py
+-rw-r--r--   0        0        0    17625 2022-07-13 18:38:50.039452 asu-0.7.9/asu/openapi.yml
+-rw-r--r--   0        0        0    56815 2022-07-13 18:38:50.039452 asu-0.7.9/asu/static/logo.png
+-rw-r--r--   0        0        0     6771 2022-07-13 18:38:50.039452 asu-0.7.9/asu/static/style.css
+-rw-r--r--   0        0        0     2675 2022-07-13 18:38:50.039452 asu-0.7.9/asu/templates/overview.html
+-rw-r--r--   0        0        0      697 2022-07-13 18:38:58.663450 asu-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6108 2022-07-13 18:38:59.480147 asu-0.7.9/setup.py
+-rw-r--r--   0        0        0     6002 2022-07-13 18:38:59.480618 asu-0.7.9/PKG-INFO
```

### Comparing `asu-0.7.8/LICENSE` & `asu-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/README.md` & `asu-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/api.py` & `asu-0.7.9/asu/api.py`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/asu.py` & `asu-0.7.9/asu/asu.py`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/build.py` & `asu-0.7.9/asu/build.py`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/common.py` & `asu-0.7.9/asu/common.py`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/janitor.py` & `asu-0.7.9/asu/janitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,36 +279,32 @@
         branch(dict): Containing all branch information as defined in BRANCHES
         version(str): Version within branch
         target(str): Target within version
     """
     current_app.logger.info(f"{version}/{target}: Update profiles")
     r = get_redis()
     version_path = branch["path"].format(version=version)
-    req = requests.head(
+
+    profiles_url = (
         current_app.config["UPSTREAM_URL"]
         + f"/{version_path}/targets/{target}/profiles.json"
     )
 
+    req = requests.get(profiles_url)
+
     if req.status_code != 200:
-        current_app.logger.warning(
-            f"{version}/{target}: Could not download profiles.json"
-        )
-        return
+        current_app.logger.warning("Couldn't download %s", profiles_url)
+        return False
 
-    profiles_url = (
-        current_app.config["UPSTREAM_URL"]
-        + f"/{version_path}/targets/{target}/profiles.json"
-    )
+    metadata = req.json()
+    profiles = metadata.pop("profiles", {})
 
     if not is_modified(profiles_url):
         current_app.logger.debug(f"{version}/{target}: Skip profiles update")
-        return
-
-    metadata = requests.get(profiles_url).json()
-    profiles = metadata.pop("profiles", {})
+        return metadata["arch_packages"]
 
     r.hset(f"architecture:{branch['name']}", target, metadata["arch_packages"])
 
     queue = Queue(connection=r)
     registry = FinishedJobRegistry(queue=queue)
     version_code = r.get(f"revision:{version}:{target}")
     if version_code:
@@ -320,15 +316,15 @@
             try:
                 request_hash = request_hash.decode()
                 registry.remove(request_hash, delete_job=True)
                 rmtree(current_app.config["STORE_PATH"] / request_hash)
 
             except NoSuchJobError:
                 current_app.logger.warning("Job was already deleted")
-        r.delete(f"build:{version_code}:{target}")
+        r.delete(f"builds:{version_code}:{target}")
 
     r.set(
         f"revision:{version}:{target}",
         metadata["version_code"],
     )
 
     current_app.logger.info(f"{version}/{target}: Found {len(profiles)} profiles")
```

### Comparing `asu-0.7.8/asu/metrics.py` & `asu-0.7.9/asu/metrics.py`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/openapi.yml` & `asu-0.7.9/asu/openapi.yml`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/static/logo.png` & `asu-0.7.9/asu/static/logo.png`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/static/style.css` & `asu-0.7.9/asu/static/style.css`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/asu/templates/overview.html` & `asu-0.7.9/asu/templates/overview.html`

 * *Files identical despite different names*

### Comparing `asu-0.7.8/pyproject.toml` & `asu-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asu"
-version = "0.7.8"
+version = "0.7.9"
 description = "An image on demand server for OpenWrt based distributions"
 authors = ["Paul Spooren <mail@aparcar.org>"]
 license = "GPL-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `asu-0.7.8/setup.py` & `asu-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'prometheus-client>=0.13.1,<0.14.0',
  'redis>=4.1.1,<5.0.0',
  'requests>=2.27.1,<3.0.0',
  'rq>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'asu',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'An image on demand server for OpenWrt based distributions',
     'long_description': '# Attendedsysupgrade Server for OpenWrt (GSoC 2017)\n\n[![codecov](https://codecov.io/gh/aparcar/asu/branch/master/graph/badge.svg)](https://codecov.io/gh/aparcar/asu)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPi](https://badge.fury.io/py/asu.svg)](https://badge.fury.io/py/asu)\n\nThis project simplifies the sysupgrade process for upgrading the firmware of\ndevices running OpenWrt or distributions based on it. These tools offer an easy\nway to reflash the router with a new firmware version\n(including all packages) without the need to use `opkg`.\n\nIt\'s called Attended SysUpgrade (ASU) because the upgrade process is not started\nautomatically, but is initiated by a user who waits until it\'s done.\n\nASU is based on an API (described below) to request custom firmware images with\nany selection of packages pre-installed. This avoids the need to set up a build\nenvironment, and makes it possible to create a custom firmware image even using\na mobile device.\n\n## Clients of the Sysupgrade Server\n\n### OpenWrt Firmware Selector\n\nSimple web interface using vanilla JavaScript currently developed by @mwarning.\nIt offers a device search based on model names and show links either to\n[official images](https://downloads.openwrt.org/) or requests images via the\n_asu_ API. Please join in the development at\n[GitLab repository](https://gitlab.com/openwrt/web/firmware-selector-openwrt-org)\n\n![ofs](misc/ofs.png)\n\n### LuCI app\n\nThe package\n[`luci-app-attendedsysupgrade`](https://github.com/openwrt/luci/tree/master/applications/luci-app-attendedsysupgrade)\noffers a simple tool under `System > Attended Sysupgrade`. It requests a new\nfirmware image that includes the current set of packages, waits until it\'s built\nand flashes it. If "Keep Configuration" is checked in the GUI, the device\nupgrades to the new firmware without any need to re-enter any configuration or\nre-install any packages.\n\n![luci](misc/luci.png)\n\n### CLI\n\nThe [`auc`](https://github.com/openwrt/packages/tree/master/utils/auc) package\nperforms the same process as the `luci-app-attendedsysupgrade`\nfrom SSH/the command line.\n\n![auc](misc/auc.png)\n\n## Server\n\nThe server listens for image requests and, if valid, automatically generates\nthem. It coordinates several OpenWrt ImageBuilders and caches the resulting\nimages in a Redis database. If an image is cached, the server can provide it\nimmediately without rebuilding.\n\n### Active server\n\n- [sysupgrade.openwrt.org](https://sysupgrade.openwrt.org)\n- [asu.aparcar.org](https://asu.aparcar.org)\n- ~~[chef.libremesh.org](https://chef.libremesh.org)~~ (`CNAME` to\n  asu.aparcar.org)\n\n## Run your own server\n\nRedis is required to store image requests:\n\n    sudo apt install redis-server tar\n\nInstall _asu_:\n\n    pip install asu\n\nCreate a `config.py`.\nYou can use `misc/config.py` as an example.\n\nStart the server via the following commands:\n\n    export FLASK_APP=asu.asu  # set Flask app to asu\n    flask janitor update      # download upstream profiles/packages - this runs forever\n    flask run                 # run development server - this runs forever\n\nStart the worker via the following comand:\n\n    rq worker                 # this runs forever\n\n### Docker\n\nRun the service inside multiple Docker containers. The services include the _\nASU_ server itself, a _janitor_ service which fills the Redis database with\nknown packages and profiles as well as a `rqworker` which actually builds\nimages.\n\nCurrently all services share the same folder and therefore a very "open" access\nis required. Suggestions on how to improve this setup are welcome.\n\n    mkdir ./asu-service/\n    chmod 777 ./asu-service/\n    cp ./misc/config.py ./asu-service/\n    docker-compose up\n\nA webserver should proxy API calls to port 8000 of the `server` service while\nthe `asu/` folder should be file hosted as-is.\n\n### Production\n\nIt is recommended to run _ASU_ via `gunicorn` proxied by `nginx` or\n`caddyserver`. Find a possible server configurations in the `misc/` folder.\n\nThe _ASU_ server will try `$PWD/config.py` and `/etc/asu/config.py` to find a\nconfiguration. Find an example configuration in the `misc/` folder.\n\n    pip install gunicorn\n    gunicorn "asu.asu:create_app()"\n\nIdeally use the tool `squid` to cache package indexes, which are reloaded every\ntime an image is built. Find a basic configuration in at `misc/squid.conf`\nwhich should be copied to `/etc/squid/squid.conf`.\n\nIf you want to use `systemd` find the service files `asu.service` and\n`worker@.service` in the `misc` folder as well.\n\n### Development\n\nAfter cloning this repository, create a Python virtual environment and install\nthe dependencies:\n\n    python3 -m venv .direnv\n    source .direnv/bin/activate\n    pip install -r requirements.txt\n    export FLASK_APP=asu.asu  # set Flask app to asu\n    export FLASK_APP=tests.conftest:mock_app FLASK_DEBUG=1 # run Flask in debug mode with mock data\n    flask run\n\n### API\n\nThe API is documented via _OpenAPI_ and can be viewed interactively on the\nserver:\n\n[https://sysupgrade.openwrt.org/ui/](https://sysupgrade.openwrt.org/ui/)\n',
     'author': 'Paul Spooren',
     'author_email': 'mail@aparcar.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `asu-0.7.8/PKG-INFO` & `asu-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asu
-Version: 0.7.8
+Version: 0.7.9
 Summary: An image on demand server for OpenWrt based distributions
 License: GPL-2.0
 Author: Paul Spooren
 Author-email: mail@aparcar.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
```

