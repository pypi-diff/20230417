# Comparing `tmp/pdh-0.3.8.tar.gz` & `tmp/pdh-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdh-0.3.8.tar", max compression
+gzip compressed data, was "pdh-0.3.9.tar", max compression
```

## Comparing `pdh-0.3.8.tar` & `pdh-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-02-17 13:51:39.147581 pdh-0.3.8/LICENSE
--rw-r--r--   0        0        0     6464 2023-02-17 13:51:39.147581 pdh-0.3.8/README.md
--rw-r--r--   0        0        0      842 2023-02-17 13:51:39.151581 pdh-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      952 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/__init__.py
--rw-r--r--   0        0        0     2856 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/config.py
--rw-r--r--   0        0        0     4252 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/core.py
--rw-r--r--   0        0        0     3990 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/filters.py
--rw-r--r--   0        0        0    12513 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/main.py
--rw-r--r--   0        0        0     3300 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/output.py
--rw-r--r--   0        0        0     6412 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/pd.py
--rw-r--r--   0        0        0     3300 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/rules.py
--rw-r--r--   0        0        0     3623 2023-02-17 13:51:39.151581 pdh-0.3.8/src/pdh/transformations.py
--rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 pdh-0.3.8/setup.py
--rw-r--r--   0        0        0     7361 1970-01-01 00:00:00.000000 pdh-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-20 11:09:23.897641 pdh-0.3.9/LICENSE
+-rw-r--r--   0        0        0     6464 2023-02-20 11:09:23.897641 pdh-0.3.9/README.md
+-rw-r--r--   0        0        0      842 2023-02-20 11:09:23.897641 pdh-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/__init__.py
+-rw-r--r--   0        0        0     2856 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/config.py
+-rw-r--r--   0        0        0     4252 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/core.py
+-rw-r--r--   0        0        0     3990 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/filters.py
+-rw-r--r--   0        0        0    12513 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/main.py
+-rw-r--r--   0        0        0     3300 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/output.py
+-rw-r--r--   0        0        0     6412 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/pd.py
+-rw-r--r--   0        0        0     3300 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/rules.py
+-rw-r--r--   0        0        0     3766 2023-02-20 11:09:23.897641 pdh-0.3.9/src/pdh/transformations.py
+-rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 pdh-0.3.9/setup.py
+-rw-r--r--   0        0        0     7361 1970-01-01 00:00:00.000000 pdh-0.3.9/PKG-INFO
```

### Comparing `pdh-0.3.8/LICENSE` & `pdh-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/README.md` & `pdh-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/pyproject.toml` & `pdh-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.flake8]
 max-line-length = 172
 ignore = "E203"
 
 
 [tool.poetry]
 name = "pdh"
-version = "0.3.8"
+version = "0.3.9"
 description = "Pagerduty CLI for Humans"
 authors = ["Manuel Bovo <manuel.bovo@gmail.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/mbovo/pdh"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pdh-0.3.8/src/pdh/__init__.py` & `pdh-0.3.9/src/pdh/__init__.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/config.py` & `pdh-0.3.9/src/pdh/config.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/core.py` & `pdh-0.3.9/src/pdh/core.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/filters.py` & `pdh-0.3.9/src/pdh/filters.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/main.py` & `pdh-0.3.9/src/pdh/main.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/output.py` & `pdh-0.3.9/src/pdh/output.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/pd.py` & `pdh-0.3.9/src/pdh/pd.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/rules.py` & `pdh-0.3.9/src/pdh/rules.py`

 * *Files identical despite different names*

### Comparing `pdh-0.3.8/src/pdh/transformations.py` & `pdh-0.3.9/src/pdh/transformations.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         def extract(i: dict) -> str:
             item = i[item_name]
             if change_dict is not None:
                 if i[item_name] in change_dict.keys():
                     item = change_dict[i[item_name]]
             if check:
                 if i[check_field] == check_value:
+                    if item[0] != "[":
+                        item = f"{item}".replace("[", "\\[")  # escape [ and ] to avoid rich formatting
                     return f"[{colors[0]}]{item}[/{colors[0]}]"
                 return f"[{colors[1]}]{item}[/{colors[1]}]"
             else:
                 return f"{item}"
 
         return extract
```

### Comparing `pdh-0.3.8/setup.py` & `pdh-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'rich>=10.10.0,<11.0.0']
 
 entry_points = \
 {'console_scripts': ['pdh = pdh.main:main']}
 
 setup_kwargs = {
     'name': 'pdh',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Pagerduty CLI for Humans',
     'long_description': '# PDH - PagerDuty CLI for humans\n\n![Build Image](https://github.com/mbovo/pdh/actions/workflows/build-image.yml/badge.svg)\n\n`PDH` is a new lightweight CLI for pagerduty interaction: uou can handle your incidents triage without leaving your terminal.\nIt also add some nice tricks to automate the incident triage and easy the on-call burden.\n\nSee [docs](./docs) (TBD)\n\n## Usage\n\nFirst of all you need to configure `pdh` to talk with PagerDuty\'s APIs:\n\n```bash\npdh config\n```\n\nThe wizard will prompt you for 3 settings:\n\n- `apikey` is the API key, you can generate it from the user\'s profile page on pagerduty website\n- `email` the email address of your pagerduty profile\n- `uid` the userID of your account (you can read it from the browser address bar when clicking on "My Profile")\n\nSettings are persisted to `~/.config/pdh.yaml` in clear.\n\n### Listing incidents\n\nAssigned to self:\n\n```bash\npdh inc ls\n```\n\nAny other incident currently outstanding:\n\n```bash\npdh inc ls -e\n```\n\n### Auto ACK incoming incidents\n\nWatch for new incidents every 10s and automatically set them to `Acknowledged`\n\n```bash\npdh inc ls --watch --new --ack --timeout 10\n```\n\n### List all HIGH priority incidents periodically\n\nList incidents asssigned to all users every 5s\n\n```bash\npdh inc ls --high --everything --watch --timeout 5\n```\n\n### Resolve specific incidents\n\n```bash\npdh inc resolve INCID0001 INCID0024 INCID0023\n```\n\n### Resolve all incidents related to `Backups`\n\n```bash\npdh inc ls --resolve --regexp ".*Backup.*"\n```\n\n## Rules\n\n`PDH` support custom scripting applied to your incidents list. These `rules` are in fact any type of executable you can run on your machine.\n\n```bash\npdh inc apply INCID001 -s /path/to/my/script.py -s /path/to/binary\n```\n\nThe `apply` subcommand will call the listed executable/script passing along a json to stdin with the incident informations. The called script can apply any type of checks/sideffects and output another json to stout to answer the call.\n\nEven though rules can be written in any language it\'s very straightforward using python:\n\n### Rules: an example\n\nAn example rule can be written in python with the following lines\n\n```python\n#!/usr/bin/env python3\nfrom pdh import rules, Filter\n\n@rules.rule\ndef main(input):\n    return {i["id"]: i["summary"] for i in input}\n\nif __name__ == "__main__":\n    main()\n```\n\nThis is the simplest rule you can write, reading the input and simply output a new dictionary with the entries. It will output something like:\n\n```bash\n\n pdh inc apply Q1LNI5LNM7RZ2C Q1C5KG41H0SZAM -s ./a.py\n┏━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ script ┃ Q1LNI5LNM7RZ2C                                                     ┃ Q1C5KG41H0SZAM                                                                       ┃\n┡━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ./a.py │  AWS Health Event: us-east-1 EC2 : AWS_EC2_INSTANCE_STOP_SCHEDULED │  AWS Health Event: us-east-1 EC2 : AWS_EC2_INSTANCE_STORE_DRIVE_PERFORMANCE_DEGRADED │\n└────────┴────────────────────────────────────────────────────────────────────┴──────────────────────────────────────────────────────────────────────────────────────┘\n```\n\nThe default output is `table` with one line for each script runned and with one column per each element in the returned object\n\n### Rules: more examples\n\n```python\n#!/usr/bin/env python3\n\n# Needed imports\nfrom pdh import rules, Filter\n\n# This annotation make the main() method parse stdin as json into the parameter called input\n# All returned values are converted to json and printed to stdout\n@rules.rule\ndef main(input):\n\n    # Initialize PagerDuty\'s APIs\n    api = rules.api()\n\n    # From the given input extract only incidents with the word cassandra in title\n    incs = Filter.objects(input, filters=[Filter.regexp("title", ".*EC2.*")])\n\n    # ackwnoledge all previously filtered incidents\n    api.ack(incs)\n\n    # resolve all previously filtered incidents\n    api.resolve(incs)\n\n    # snooze all previously filtered incidents for 1h\n    api.snooze(incs, duration=3600)\n\n    # Chain a given rule, i.e call that rule with the output of this one\n    # chain-loading supports only a single binary, not directories\n    c = rules.chain(incs, "rules/test_chaining.sh")\n\n    # Execute an external program and get the output/err/return code\n    p: rules.ShellResponse = rules.exec(\'kubectl get nodes -o name\')\n    if p.rc > 0:\n      nodes = p.stdout.split("\\n")\n\n    # if you return a dict will be rendered with each item as a column in a table\n    # Othrwise will be converted as string\n    return {i["id"]: i["summary"] for i in incs}\n\n\nif __name__ == "__main__":\n    main()\n\n\n```\n\n## Requirements\n\n- [Taskfile](https://taskfile.dev)\n- Python >=3.9\n- Docker\n\n## Contributing\n\nFirst of all you need to setup the dev environment, using Taskfile:\n\n```bash\ntask setup\n```\n\nThis will create a python virtualenv and install `pre-commit` and `poetry` in your system if you lack them.\n\n\n## License\n\nThis program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.\nSee [](LICENSE) for more details.\n',
     'author': 'Manuel Bovo',
     'author_email': 'manuel.bovo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mbovo/pdh',
```

### Comparing `pdh-0.3.8/PKG-INFO` & `pdh-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdh
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pagerduty CLI for Humans
 Home-page: https://github.com/mbovo/pdh
 License: GPL-3.0-or-later
 Author: Manuel Bovo
 Author-email: manuel.bovo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

