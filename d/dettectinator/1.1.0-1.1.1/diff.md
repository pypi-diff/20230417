# Comparing `tmp/dettectinator-1.1.0.tar.gz` & `tmp/dettectinator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dettectinator-1.1.0.tar", last modified: Thu Dec 22 14:36:55 2022, max compression
+gzip compressed data, was "dettectinator-1.1.1.tar", last modified: Mon Apr 17 10:00:19 2023, max compression
```

## Comparing `dettectinator-1.1.0.tar` & `dettectinator-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-12-22 14:36:55.583354 dettectinator-1.1.0/
--rw-r--r--   0 ruben      (501) staff       (20)    35149 2022-11-02 21:36:33.000000 dettectinator-1.1.0/LICENSE
--rw-r--r--   0 ruben      (501) staff       (20)       11 2022-11-02 21:36:33.000000 dettectinator-1.1.0/MANIFEST.in
--rw-r--r--   0 ruben      (501) staff       (20)     1560 2022-12-22 14:36:55.582870 dettectinator-1.1.0/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)     2364 2022-12-22 14:33:58.000000 dettectinator-1.1.0/README.md
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-12-22 14:36:55.573717 dettectinator-1.1.0/dettectinator/
--rw-r--r--   0 ruben      (501) staff       (20)      107 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)     8958 2022-12-22 14:33:58.000000 dettectinator-1.1.0/dettectinator/cli.py
--rw-r--r--   0 ruben      (501) staff       (20)     3844 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/constants.py
--rw-r--r--   0 ruben      (501) staff       (20)    41297 2022-12-22 14:33:58.000000 dettectinator-1.1.0/dettectinator/dettectinator.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-12-22 14:36:55.578358 dettectinator-1.1.0/dettectinator/plugins/
--rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/plugins/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)    14200 2022-12-22 14:33:58.000000 dettectinator-1.1.0/dettectinator/plugins/datasources_import.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-12-22 14:36:55.582350 dettectinator-1.1.0/dettectinator/plugins/support/
--rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/plugins/support/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)     3481 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/plugins/support/authentication.py
--rw-r--r--   0 ruben      (501) staff       (20)     5333 2022-11-02 21:36:33.000000 dettectinator-1.1.0/dettectinator/plugins/support/msal_patch.py
--rw-r--r--   0 ruben      (501) staff       (20)    32798 2022-12-22 14:33:58.000000 dettectinator-1.1.0/dettectinator/plugins/technique_import.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-12-22 14:36:55.577133 dettectinator-1.1.0/dettectinator.egg-info/
--rw-r--r--   0 ruben      (501) staff       (20)     1560 2022-12-22 14:36:55.000000 dettectinator-1.1.0/dettectinator.egg-info/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      581 2022-12-22 14:36:55.000000 dettectinator-1.1.0/dettectinator.egg-info/SOURCES.txt
--rw-r--r--   0 ruben      (501) staff       (20)        1 2022-12-22 14:36:55.000000 dettectinator-1.1.0/dettectinator.egg-info/dependency_links.txt
--rw-r--r--   0 ruben      (501) staff       (20)      134 2022-12-22 14:36:55.000000 dettectinator-1.1.0/dettectinator.egg-info/requires.txt
--rw-r--r--   0 ruben      (501) staff       (20)       14 2022-12-22 14:36:55.000000 dettectinator-1.1.0/dettectinator.egg-info/top_level.txt
--rw-r--r--   0 ruben      (501) staff       (20)       38 2022-12-22 14:36:55.583452 dettectinator-1.1.0/setup.cfg
--rw-r--r--   0 ruben      (501) staff       (20)     1974 2022-12-22 14:36:33.000000 dettectinator-1.1.0/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.336272 dettectinator-1.1.1/
+-rw-r--r--   0 ruben      (501) staff       (20)    35149 2022-11-02 21:36:33.000000 dettectinator-1.1.1/LICENSE
+-rw-r--r--   0 ruben      (501) staff       (20)       11 2022-11-02 21:36:33.000000 dettectinator-1.1.1/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-04-17 10:00:19.336006 dettectinator-1.1.1/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)     2379 2023-01-25 07:09:52.000000 dettectinator-1.1.1/README.md
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.327377 dettectinator-1.1.1/dettectinator/
+-rw-r--r--   0 ruben      (501) staff       (20)      107 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)     8959 2023-01-25 07:09:52.000000 dettectinator-1.1.1/dettectinator/cli.py
+-rw-r--r--   0 ruben      (501) staff       (20)     3844 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/constants.py
+-rw-r--r--   0 ruben      (501) staff       (20)    41570 2023-04-17 09:54:28.000000 dettectinator-1.1.1/dettectinator/dettectinator.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.333423 dettectinator-1.1.1/dettectinator/plugins/
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)    14192 2023-03-15 09:27:23.000000 dettectinator-1.1.1/dettectinator/plugins/datasources_import.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.335571 dettectinator-1.1.1/dettectinator/plugins/support/
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)     3481 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/authentication.py
+-rw-r--r--   0 ruben      (501) staff       (20)     5333 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/msal_patch.py
+-rw-r--r--   0 ruben      (501) staff       (20)    32798 2023-01-25 07:09:52.000000 dettectinator-1.1.1/dettectinator/plugins/technique_import.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.330592 dettectinator-1.1.1/dettectinator.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      581 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)      134 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/requires.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       14 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       38 2023-04-17 10:00:19.336348 dettectinator-1.1.1/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)     1997 2023-04-17 09:56:17.000000 dettectinator-1.1.1/setup.py
```

### Comparing `dettectinator-1.1.0/LICENSE` & `dettectinator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/PKG-INFO` & `dettectinator-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dettectinator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Dettectinator - The Python library to your DeTT&CT YAML files.
 Home-page: https://github.com/siriussecurity/dettectinator
 Author: Sirius Security
 License: GPL3
 Project-URL: Documentation, https://github.com/siriussecurity/dettectinator/wiki
 Project-URL: Code, https://github.com/siriussecurity/dettectinator
 Project-URL: Issue tracker, https://github.com/siriussecurity/dettectinator/issues
```

### Comparing `dettectinator-1.1.0/README.md` & `dettectinator-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Dettectinator
 Dettectinator - The Python library to your DeTT&amp;CT YAML files.
 
 [DeTT&CT](https://github.com/rabobank-cdc/DeTTECT) is a framework that helps blue teams in using MITRE ATT&CK to score and compare data log source quality, visibility coverage, detection coverage and threat actor behaviours. All administration is done in YAML files which can be editted via the [DeTT&CT Editor](https://rabobank-cdc.github.io/dettect-editor). But what if you want to automate the generation and modification of these YAML files? That's were Dettectinator comes in!
 
 Dettectinator is built to be included in your SOC automation tooling. It can be included as a Python library (`pip install dettectinator`) or it can be used via the command line (`python dettectinator.py -h`).
 
 Dettectinator also provides plugins to read detections and data sources from your SIEM or EDR and create a DeTT&CT YAML for it, so that you can use it to visualize your ATT&CK data source and detection coverage in the ATT&CK  Navigator.
@@ -23,10 +24,10 @@
 For data sources, you can use the following plugins:
 - Defender for Endpoints: tables available in Advanced Hunting (based on OSSEM)
 - Windows Sysmon: event logging based on Sysmon (based on OSSEM and your Sysmon config file)
 - Sentinel Window Security Auditing: event logging (based on OSSEM and EventID's found in your logging)
 - CSV: any csv with ATT&CK data sources and products (file)
 - Excel: any Excel file with ATT&CK data sources and products (file)
 
-It's easy to create your own Dettectinator plugins or edit the ones we've provided to cover additional scenario's.
+It's easy to create your own Dettectinator plugins or edit the ones we've provided to cover additional scenarios.
 
 More information on how to use Dettectinator and how to use and create plugins can be found in the [wiki](https://github.com/siriussecurity/dettectinator/wiki).
```

### Comparing `dettectinator-1.1.0/dettectinator/cli.py` & `dettectinator-1.1.1/dettectinator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             # Get the plugin class if it exists
             if plugin_name in plugins.keys():
                 plugin_class = getattr(plugins[plugin_name], plugin_name)
                 print(f'Plugin "{plugin_name}" has been found.')
             else:
                 print(f'data import plugin "{plugin_name}" does not exist. Valid plugins:')
                 self._print_plugins(plugins)
-                sys.exit()
+                sys.exit(1)
 
             # Add the default command line params
             parser = ArgumentParser(add_help=True, conflict_handler='error', )
             self._set_default_params(parser)
 
             # Add the parameters from the plugin
             plugin_group = parser.add_argument_group(plugin_name)
```

### Comparing `dettectinator-1.1.0/dettectinator/constants.py` & `dettectinator-1.1.1/dettectinator/constants.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/dettectinator/dettectinator.py` & `dettectinator-1.1.1/dettectinator/dettectinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,16 @@
         :param  clean_unused_detections: boolean. When True, all detections in YAML file that don't exist in the given detection_rules list will be removed.
         :param clean_unused_applicable_to: boolean. When True, all detection objects with a applicable_to value that doesn't exist in the given detection_rules list will be removed.
         :return a list with results containing warnings or errors during the update process.
         """
         date_today = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
 
         warnings, results = self._add_rules(detection_rules, date_today)
-        w, r = self._delete_rules(detection_rules, check_unused_detections, clean_unused_detections, location_prefix_unused_detections, check_unused_applicable_to, clean_unused_applicable_to, date_today)
+        w, r = self._delete_rules(detection_rules, check_unused_detections, clean_unused_detections,
+                                  location_prefix_unused_detections, check_unused_applicable_to, clean_unused_applicable_to, date_today)
         warnings += w
         results += r
 
         return warnings, results
 
     def _add_rules(self, detection_rules: dict, date_today: datetime) -> list:
         """
@@ -315,15 +316,16 @@
 
         # Loop through all detection rules:
         for rule_name, rule_data in detection_rules.items():
             # Loop through every technique per rule:
             for technique_id in rule_data['techniques']:
                 attack_technique = self._get_technique_from_attack(technique_id)
                 if attack_technique is None:
-                    warnings.append(f'Technique "{technique_id}" listed in detection rule "{rule_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
+                    warnings.append(
+                        f'Technique "{technique_id}" listed in detection rule "{rule_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
                     continue
 
                 location = rule_name if rule_data['location_prefix'] == '' else rule_data['location_prefix'] + ': ' + rule_name
                 yaml_technique = self._get_technique_from_yaml(technique_id)
                 if yaml_technique is not None:
                     # Check is applicable_to is already there:
                     applicable_to_list = [d['applicable_to'] for d in yaml_technique['detection']]
@@ -338,54 +340,62 @@
                                         rule_exist = True
                                         break
 
                                 # If detection rule is not yet in location field, add detection rule to location field:
                                 if not rule_exist:
                                     d['location'].append(location)
 
+                                    if len(d['score_logbook']) == 1 and d['score_logbook'][0]['date'] is None and d['score_logbook'][0]['score'] == -1:
+                                        d['score_logbook'] = []
+
                                     # Check if score_logbook already has entry for today:
                                     today_found = False
                                     for logbook_entry in d['score_logbook']:
                                         if logbook_entry['date'] == date_today:
                                             logbook_entry['comment'] += f'. Detection rule added: {rule_name}'
                                             today_found = True
                                             break
 
                                     if not today_found:
+                                        score = self._get_latest_score(d)
+                                        score = 1 if score == -1 or score is None else score
                                         d['score_logbook'].append({
                                             'date': date_today,
-                                            'score': self._get_latest_score(d),
+                                            'score': score,
                                             'comment': f'Auto added by Dettectinator. TODO: Check score. Detection rule added: {rule_name}'
                                         })
-                                        results.append(f'Check score for technique {technique_id}. Detection rule(s) added for applicable_to {d["applicable_to"]}.')
+                                        results.append(
+                                            f'Check score for technique {technique_id}. Detection rule(s) added for applicable_to {d["applicable_to"]}.')
 
                                 break
                     else:
                         # applicable_to not present, add new detection object:
                         new_detection = deepcopy(YAML_OBJ_DETECTION)
                         new_detection['applicable_to'] = rule_data['applicable_to']
                         new_detection['location'] = [location]
                         new_detection['score_logbook'][0]['date'] = date_today
                         new_detection['score_logbook'][0]['score'] = 1
-                        new_detection['score_logbook'][0]['comment'] = f'Auto added by Dettectinator. TODO: Check score. applicable_to with detection rule added: {rule_name}'
+                        new_detection['score_logbook'][0][
+                            'comment'] = f'Auto added by Dettectinator. TODO: Check score. applicable_to with detection rule added: {rule_name}'
                         yaml_technique['detection'].append(new_detection)
                         results.append(f'Check score for technique {technique_id}. applicable_to is new: {str(rule_data["applicable_to"])}.')
                 else:
                     # Technique not present in YAML, add:
                     new_technique = deepcopy(YAML_OBJ_TECHNIQUE)
                     new_technique['technique_id'] = technique_id
                     new_technique['technique_name'] = attack_technique['name']
                     new_technique['detection'] = []
                     new_technique['visibility'] = []
                     new_detection = deepcopy(YAML_OBJ_DETECTION)
                     new_detection['applicable_to'] = rule_data['applicable_to']
                     new_detection['location'] = [location]
                     new_detection['score_logbook'][0]['date'] = date_today
                     new_detection['score_logbook'][0]['score'] = 1
-                    new_detection['score_logbook'][0]['comment'] = f'Auto added by Dettectinator. TODO: Check score. Technique with detection rule added: {rule_name}'
+                    new_detection['score_logbook'][0][
+                        'comment'] = f'Auto added by Dettectinator. TODO: Check score. Technique with detection rule added: {rule_name}'
                     new_technique['detection'].append(new_detection)
                     new_visibility = deepcopy(YAML_OBJ_VISIBILITY)
                     new_technique['visibility'].append(new_visibility)
                     self._yaml_content['techniques'].append(new_technique)
                     results.append(f'Check score for technique {technique_id}. Technique is new.')
 
         return warnings, results
@@ -420,15 +430,15 @@
                     locations = deepcopy(detection['location'])
                     for loc in locations:
                         if loc.startswith(location_prefix_unused_detections) and loc not in rules_for_app_to:
                             if check_unused_detections and not clean_unused_detections:
                                 warnings.append('Rule from YAML not found in rules list: ' + loc)
                             elif check_unused_detections and clean_unused_detections:
                                 detection['location'].remove(loc)
-                                score = 0 if len(detection['location']) == 0 else self._get_latest_score(detection)
+                                score = -1 if len(detection['location']) == 0 else self._get_latest_score(detection)
 
                                 # Check if score_logbook already has entry for today:
                                 today_found = False
                                 for logbook_entry in detection['score_logbook']:
                                     if logbook_entry['date'] == date_today:
                                         logbook_entry['score'] = score
                                         logbook_entry['comment'] += f'. Detection rule removed: {loc}'
@@ -440,50 +450,52 @@
                                         'date': date_today,
                                         'score': score,
                                         'comment': f'Auto added by Dettectinator. TODO: Check score. Detection rule removed: {loc}'
                                     })
                                     results.append(f'Check score for technique {yaml_technique["technique_id"]}. Detection rule(s) removed.')
                 else:
                     if check_unused_applicable_to and not clean_unused_applicable_to:
-                        warnings.append(f'YAML applicable_to for technique "{yaml_technique["technique_id"]}" not in rules list: {str(detection["applicable_to"])}.')
+                        warnings.append(
+                            f'YAML applicable_to for technique "{yaml_technique["technique_id"]}" not in rules list: {str(detection["applicable_to"])}.')
                     elif check_unused_applicable_to and clean_unused_applicable_to:
                         to_remove.append(detection)
 
             for item in to_remove:
-                warnings.append(f'YAML applicable_to for technique "{yaml_technique["technique_id"]}" not in rules list, so removed: {str(detection["applicable_to"])}.')
+                warnings.append(
+                    f'YAML applicable_to for technique "{yaml_technique["technique_id"]}" not in rules list, so removed: {str(detection["applicable_to"])}.')
                 yaml_technique['detection'].remove(item)
 
         return warnings, results
 
     def _load_techniques(self) -> None:
         """
         Loads the normalized techniques (including detection and visibility properties) from the techniques YAML file.
         """
         my_techniques = {}
 
         for d in self._yaml_content['techniques']:
             if 'detection' in d:
+                # There is just one detection entry, make it a list:
+                if isinstance(d['detection'], dict):
+                    d['detection'] = [d['detection']]
+
                 # Add detection items:
-                if isinstance(d['detection'], dict):  # There is just one detection entry
-                    d['detection'] = self._set_yaml_dv_comments(d['detection'])
-                    self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'detection', d['detection'])
-                elif isinstance(d['detection'], list):  # There are multiple detection entries
-                    for de in d['detection']:
-                        de = self._set_yaml_dv_comments(de)
-                        self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'detection', de)
+                for de in d['detection']:
+                    de = self._set_yaml_dv_comments(de)
+                    self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'detection', de)
 
             if 'visibility' in d:
+                # There is just one detection entry, make it a list:
+                if isinstance(d['visibility'], dict):
+                    d['visibility'] = [d['visibility']]
+
                 # Add visibility items
-                if isinstance(d['visibility'], dict):  # There is just one visibility entry
-                    d['visibility'] = self._set_yaml_dv_comments(d['visibility'])
-                    self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'visibility', d['visibility'])
-                elif isinstance(d['visibility'], list):  # There are multiple visibility entries
-                    for de in d['visibility']:
-                        de = self._set_yaml_dv_comments(de)
-                        self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'visibility', de)
+                for de in d['visibility']:
+                    de = self._set_yaml_dv_comments(de)
+                    self._add_entry_to_list_in_dictionary(my_techniques, d['technique_id'], 'visibility', de)
 
         self.techniques = my_techniques
 
     def _get_technique(self, technique_id: str) -> object:
         """
         Gets the technique from the normalized YAML techniques.
         """
@@ -614,30 +626,33 @@
             # Loop through all given applicable_to values:
             for data_source_data in data_source_applicable_to:
                 # Health check: is given applicable_to present in systems object. If not: it will be added with platform=all
                 for a in data_source_data['applicable_to']:
                     if a not in self._system_applicable_to_values:
                         self._yaml_content['systems'].append({'applicable_to': a, 'platform': ['all']})
                         self._system_applicable_to_values.append(a)
-                        results.append(f'Applicable_to value "{str(data_source_data["applicable_to"])}" of data source "{data_source_name}" not in systems object of data source YAML file. Added to systems object with platform=all. Please review this new entry.')
+                        results.append(
+                            f'Applicable_to value "{str(data_source_data["applicable_to"])}" of data source "{data_source_name}" not in systems object of data source YAML file. Added to systems object with platform=all. Please review this new entry.')
 
                 # Check if applicable_to is already there:
                 applicable_to_list = [d['applicable_to'] for d in yaml_data_source['data_source']]
                 if data_source_data['applicable_to'] not in applicable_to_list:
                     # applicable_to not present, add new data source object:
                     new_data_source = deepcopy(YAML_OBJ_DATA_SOURCE)
                     new_data_source['applicable_to'] = data_source_data['applicable_to']
                     new_data_source['date_registered'] = date_today
                     new_data_source['date_connected'] = date_today
                     new_data_source['products'] = data_source_data['products']
                     new_data_source['available_for_data_analytics'] = data_source_data['available_for_data_analytics']
                     default_scores, scores_changed = self._set_data_quality(new_data_source, data_source_data)
-                    new_data_source['comment'] = 'Auto added by Dettectinator.' + (' TODO: Check data quality scores, default values used.' if default_scores else '')
+                    new_data_source['comment'] = 'Auto added by Dettectinator.' + \
+                        (' TODO: Check data quality scores, default values used.' if default_scores else '')
                     yaml_data_source['data_source'].append(new_data_source)
-                    results.append(f'Check data quality scores for data source {data_source_name}. applicable_to is new: {str(data_source_data["applicable_to"])}')
+                    results.append(
+                        f'Check data quality scores for data source {data_source_name}. applicable_to is new: {str(data_source_data["applicable_to"])}')
                 else:
                     # applicable_to present, get the object and update:
                     for data_source in yaml_data_source['data_source']:
                         if data_source['applicable_to'] == data_source_data['applicable_to']:
                             changed = False
                             if data_source['products'] != data_source_data['products']:
                                 data_source['products'] = data_source_data['products']
@@ -646,15 +661,16 @@
                                 data_source['available_for_data_analytics'] = data_source_data['available_for_data_analytics']
                                 changed = True
                             default_scores, scores_changed = self._set_data_quality(data_source, data_source_data)
                             if scores_changed:
                                 changed = True
                             if changed:
                                 data_source['comment'] = 'Auto updated by Dettectinator. TODO: Check data quality scores.'
-                                results.append(f'Check data quality scores for data source {data_source_name}. Data source with applicable_to {str(data_source_data["applicable_to"])} is updated.')
+                                results.append(
+                                    f'Check data quality scores for data source {data_source_name}. Data source with applicable_to {str(data_source_data["applicable_to"])} is updated.')
                             break
 
         return warnings, results
 
     def _delete_data_sources(self, data_sources: list, clean_unused_data_sources: bool) -> list:
         """
         Removes data sources from the data source YAML file which are not in the given data_sources list. A comment is added for every change.
@@ -677,15 +693,16 @@
                         applicable_to_ds.append(str(data_source_data['applicable_to']))
 
                 # Make a copy to loop through applicable_to's in YAML (so that original can be mutated):
                 applicable_to_yaml = deepcopy(yaml_data_source['data_source'])
                 for app_to in applicable_to_yaml:
                     if str(app_to['applicable_to']) not in applicable_to_ds:
                         yaml_data_source['data_source'].remove(app_to)
-                        warnings.append(f'YAML applicable_to value "{str(app_to["applicable_to"])}" of data source "{yaml_data_source["data_source_name"]}" not in given data sources list, so removed.')
+                        warnings.append(
+                            f'YAML applicable_to value "{str(app_to["applicable_to"])}" of data source "{yaml_data_source["data_source_name"]}" not in given data sources list, so removed.')
             else:
                 # Data source in YAML but not in data_sources list. So remove.
                 if not clean_unused_data_sources:
                     warnings.append(f'YAML data source "{yaml_data_source["data_source_name"]}" not in given data sources list.')
                 else:
                     to_remove.append(yaml_data_source)
 
@@ -750,9 +767,9 @@
         for data_component in data_components:
             self.data_components[data_component['name'].lower()] = data_component['name']
 
 
 if __name__ == '__main__':
     # Where being run from the command line here, start CLI logic
     cli_mod = importlib.import_module('cli')
-    cli= getattr(cli_mod, 'CommandLine')()
+    cli = getattr(cli_mod, 'CommandLine')()
     cli.start()
```

### Comparing `dettectinator-1.1.0/dettectinator/plugins/datasources_import.py` & `dettectinator-1.1.1/dettectinator/plugins/datasources_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
         for record in ossem_data:
             config_items = sysmon_config.findall(f'.//{record["Audit Category"]}')
 
             # If this is an event type with an onmatch == include attribute without child items this means
             # that nothing is being logged for this event type
             for config_item in config_items:
-                if config_item.attrib['onmatch'] == "include" and len(config_item.getchildren()) == 0:
+                if config_item.attrib['onmatch'] == "include" and len(list(config_item)) == 0:
                     continue
 
             data_source = str(record['Component']).title()
             product = f'{record["EventID"]}: {record["Event Name"]}'
             yield data_source, product, None
 
     def _get_sysmon_config(self) -> Element:
```

### Comparing `dettectinator-1.1.0/dettectinator/plugins/support/authentication.py` & `dettectinator-1.1.1/dettectinator/plugins/support/authentication.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/dettectinator/plugins/support/msal_patch.py` & `dettectinator-1.1.1/dettectinator/plugins/support/msal_patch.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/dettectinator/plugins/technique_import.py` & `dettectinator-1.1.1/dettectinator/plugins/technique_import.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/dettectinator.egg-info/PKG-INFO` & `dettectinator-1.1.1/dettectinator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dettectinator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Dettectinator - The Python library to your DeTT&CT YAML files.
 Home-page: https://github.com/siriussecurity/dettectinator
 Author: Sirius Security
 License: GPL3
 Project-URL: Documentation, https://github.com/siriussecurity/dettectinator/wiki
 Project-URL: Code, https://github.com/siriussecurity/dettectinator
 Project-URL: Issue tracker, https://github.com/siriussecurity/dettectinator/issues
```

### Comparing `dettectinator-1.1.0/dettectinator.egg-info/SOURCES.txt` & `dettectinator-1.1.1/dettectinator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.0/setup.py` & `dettectinator-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 
 Currently de CLI is limited to processing detections through these plugins, the library can also be used for processing data sources.
 
 See the [documentation](https://github.com/siriussecurity/dettectinator) for more information on how to use it."""
 
 setuptools.setup(
     name="dettectinator",
-    version="1.1.0",
+    version="1.1.1",
     author="Sirius Security",
     description="Dettectinator - The Python library to your DeTT&CT YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/siriussecurity/dettectinator",
     project_urls={
         "Documentation": "https://github.com/siriussecurity/dettectinator/wiki",
         "Code": "https://github.com/siriussecurity/dettectinator",
         "Issue tracker": "https://github.com/siriussecurity/dettectinator/issues",
     },
     keywords="mitre attack dettect soc threat hunting",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
-    install_requires=["requests", "ruamel.yaml", "attackcti", "python-dateutil", "msal", "stix2", "openpyxl", "suricataparser", "addonfactory-splunk-conf-parser-lib", "pandas", "anyascii"],
+    install_requires=["requests", "ruamel.yaml", "attackcti", "python-dateutil", "msal", "stix2",
+                      "openpyxl", "suricataparser", "addonfactory-splunk-conf-parser-lib", "pandas", "anyascii"],
     license='GPL3',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Topic :: Security',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9'
     ],
-)
+)
```

