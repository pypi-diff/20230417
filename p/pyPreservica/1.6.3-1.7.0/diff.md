# Comparing `tmp/pyPreservica-1.6.3.tar.gz` & `tmp/pyPreservica-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-1.6.3.tar", last modified: Thu Feb  2 16:50:13 2023, max compression
+gzip compressed data, was "pyPreservica-1.7.0.tar", last modified: Mon Apr 17 14:19:21 2023, max compression
```

## Comparing `pyPreservica-1.6.3.tar` & `pyPreservica-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 16:50:13.609622 pyPreservica-1.6.3/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-02-02 16:50:13.609622 pyPreservica-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-02 16:50:13.562752 pyPreservica-1.6.3/pyPreservica/
--rw-rw-rw-   0        0        0      970 2023-02-02 16:49:42.000000 pyPreservica-1.6.3/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37463 2022-07-13 14:33:42.000000 pyPreservica-1.6.3/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    31812 2023-02-02 14:13:30.000000 pyPreservica-1.6.3/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16084 2021-11-19 09:54:40.000000 pyPreservica-1.6.3/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105213 2022-12-02 14:18:15.000000 pyPreservica-1.6.3/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6230 2022-10-13 10:30:26.000000 pyPreservica-1.6.3/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.6.3/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.6.3/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23299 2021-11-15 13:21:31.000000 pyPreservica-1.6.3/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92022 2023-02-02 16:03:44.000000 pyPreservica-1.6.3/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0    17717 2022-05-26 15:15:21.000000 pyPreservica-1.6.3/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-02-02 16:50:13.594000 pyPreservica-1.6.3/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-02-02 16:50:12.000000 pyPreservica-1.6.3/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-02-02 16:50:12.000000 pyPreservica-1.6.3/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 16:50:12.000000 pyPreservica-1.6.3/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-02-02 16:50:12.000000 pyPreservica-1.6.3/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-02 16:50:12.000000 pyPreservica-1.6.3/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-02 16:50:13.609622 pyPreservica-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1661 2023-02-02 16:49:42.000000 pyPreservica-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.805726 pyPreservica-1.7.0/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-04-17 14:19:21.790105 pyPreservica-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.751688 pyPreservica-1.7.0/pyPreservica/
+-rw-rw-rw-   0        0        0      970 2023-02-02 16:53:09.000000 pyPreservica-1.7.0/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37713 2023-03-01 16:08:31.000000 pyPreservica-1.7.0/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    31931 2023-03-01 16:00:56.000000 pyPreservica-1.7.0/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.0/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.0/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6260 2023-03-01 16:11:00.000000 pyPreservica-1.7.0/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.0/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.0/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.0/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92270 2023-03-21 17:44:59.000000 pyPreservica-1.7.0/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.0/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.790105 pyPreservica-1.7.0/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:19:21.805726 pyPreservica-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-02-02 16:53:09.000000 pyPreservica-1.7.0/setup.py
```

### Comparing `pyPreservica-1.6.3/LICENSE.txt` & `pyPreservica-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.6.3/PKG-INFO` & `pyPreservica-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.6.3/README.md` & `pyPreservica-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.6.3/pyPreservica/__init__.py` & `pyPreservica-1.7.0/pyPreservica/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 from .adminAPI import AdminAPI
 from .monitorAPI import MonitorAPI, MonitorCategory, MonitorStatus, MessageStatus
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "1.6.3"
+__version__ = "1.7.0"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-1.6.3/pyPreservica/adminAPI.py` & `pyPreservica-1.7.0/pyPreservica/adminAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """
         if (self.major_version < 7) and (self.minor_version < 5):
             raise RuntimeError(
                 "delete_system_role API call is only available with a Preservica v6.5.0 system or higher")
 
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.delete(f'https://{self.server}/api/admin/security/roles/{role_name}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/roles/{role_name}', headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_system_role(role_name)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -58,15 +58,15 @@
         """
         if (self.major_version < 7) and (self.minor_version < 4):
             raise RuntimeError(
                 "delete_security_tag API call is only available with a Preservica v6.4.0 system or higher")
 
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.delete(f'https://{self.server}/api/admin/security/tags/{tag_name}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/tags/{tag_name}', headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_security_tag(tag_name)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -88,15 +88,15 @@
 
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         xml_tag = xml.etree.ElementTree.Element('Role', {"xmlns": self.admin_ns})
         xml_tag.text = str(role_name).strip()
         xml_request = xml.etree.ElementTree.tostring(xml_tag, encoding='utf-8')
-        request = self.session.post(f'https://{self.server}/api/admin/security/roles', data=xml_request,
+        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/security/roles', data=xml_request,
                                     headers=headers)
         if request.status_code == requests.codes.created:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             return entity_response.text
         elif request.status_code == requests.codes.unauthorized:
@@ -124,15 +124,15 @@
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         xml_tag = xml.etree.ElementTree.Element('Tag', {"xmlns": self.admin_ns})
         xml_tag.text = str(tag_name).strip()
         xml_request = xml.etree.ElementTree.tostring(xml_tag, encoding='utf-8')
 
-        request = self.session.post(f'https://{self.server}/api/admin/security/tags', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/security/tags', data=xml_request, headers=headers)
         if request.status_code == requests.codes.created:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             return entity_response.text
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
@@ -152,15 +152,15 @@
         self.__check_if_user_has_manager_role()
 
         if (self.major_version < 7) and (self.minor_version < 5):
             raise RuntimeError(
                 "system_roles API call is only available with a Preservica v6.5.0 system or higher")
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/admin/security/roles', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/admin/security/roles', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             roles = entity_response.findall(f'.//{{{self.admin_ns}}}Role')
             security_roles = []
             for role in roles:
@@ -179,15 +179,15 @@
 
         :return: list of security tags
         :rtype: list
 
         """
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/admin/security/tags', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/admin/security/tags', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             tags = entity_response.findall(f'.//{{{self.admin_ns}}}Tag')
             security_tags = []
             for tag in tags:
@@ -207,15 +207,15 @@
         :param username: email address of the preservica user
         :type username: str
 
         """
         self.__check_if_user_has_manager_role()
         self.disable_user(username)
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.delete(f'https://{self.server}/api/admin/users/{username}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/users/{username}', headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_user(username)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -249,15 +249,15 @@
             xml.etree.ElementTree.SubElement(xml_object, "externallyAuthenticated").text = "true"
             xml.etree.ElementTree.SubElement(xml_object, "userName").text = username
         xml_roles = xml.etree.ElementTree.SubElement(xml_object, "Roles")
         for role in roles:
             xml.etree.ElementTree.SubElement(xml_roles, "Role").text = role
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'https://{self.server}/api/admin/users', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/users', data=xml_request, headers=headers)
         if request.status_code == requests.codes.created:
             return self.user_details(username)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_user(username, full_name, roles)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -274,24 +274,24 @@
          :type new_display_name: str
 
          :return: dictionary of user attributes
          :rtype: dict
          """
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f"https://{self.server}/api/admin/users/{username}", headers=headers)
+        request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users/{username}", headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             fullname = entity_response.find(f'.//{{{self.admin_ns}}}FullName')
             fullname.text = new_display_name
             xml_request = xml.etree.ElementTree.tostring(entity_response, encoding='utf-8')
             logger.debug(xml_request)
-            update_request = self.session.put(f'https://{self.server}/api/admin/users/{username}', data=xml_request,
+            update_request = self.session.put(f'{self.protocol}://{self.server}/api/admin/users/{username}', data=xml_request,
                                               headers=headers)
             if update_request.status_code == requests.codes.ok:
                 return self.user_details(username)
             elif update_request.status_code == requests.codes.unauthorized:
                 self.token = self.__token__()
                 return self.change_user_display_name(username, new_display_name)
             else:
@@ -313,15 +313,15 @@
 
         :return: dictionary of user attributes
         :rtype: dict
         """
 
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f"https://{self.server}/api/admin/users/{username}", headers=headers)
+        request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users/{username}", headers=headers)
         return_dict = {}
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             username = entity_response.find(f'.//{{{self.admin_ns}}}UserName')
             return_dict['UserName'] = username.text
@@ -346,15 +346,15 @@
         else:
             logger.error(request.content.decode('utf-8'))
             raise RuntimeError(request.status_code, "user_details failed")
 
     def __account_status_(self, username: str, status: str, name: str):
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain;charset=UTF-8'}
         data = {"userEnabledStatus": status}
-        request = self.session.put(f"https://{self.server}/api/admin/users/{username}/enabled", headers=headers,
+        request = self.session.put(f"{self.protocol}://{self.server}/api/admin/users/{username}/enabled", headers=headers,
                                    data=data)
         if request.status_code == requests.codes.ok:
             return request.content.decode("utf-8")
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.__account_status_(username, status, name)
         else:
@@ -406,15 +406,15 @@
 
         :return list of usernames:
         :rtype: list
         """
 
         self.__check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f"https://{self.server}/api/admin/users", headers=headers)
+        request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users", headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             users = entity_response.findall(f'.//{{{self.admin_ns}}}User')
             system_users = []
             for user in users:
@@ -454,15 +454,15 @@
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"https://{self.server}/api/admin/schemas", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/schemas", headers=headers, params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_schema(name, description, originalName, xml_data)
         else:
@@ -503,15 +503,15 @@
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"https://{self.server}/api/admin/documents", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/documents", headers=headers, params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_document(name, xml_data, document_type)
         else:
@@ -532,15 +532,15 @@
 
         self.__check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for document in self.xml_documents():
             if document['SchemaUri'] == uri.strip():
-                request = self.session.delete(f"https://{self.server}/api/admin/documents/{document['ApiId']}",
+                request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}",
                                               headers=headers)
                 if request.status_code == requests.codes.no_content:
                     return
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.delete_xml_document(uri)
                 else:
@@ -561,15 +561,15 @@
 
         self.__check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for schema in self.xml_schemas():
             if schema['SchemaUri'] == uri.strip():
-                request = self.session.delete(f"https://{self.server}/api/admin/schemas/{schema['ApiId']}",
+                request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/schemas/{schema['ApiId']}",
                                               headers=headers)
                 if request.status_code == requests.codes.no_content:
                     return
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.delete_xml_schema(uri)
                 else:
@@ -587,15 +587,15 @@
         :rtype: str
 
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for schema in self.xml_schemas():
             if schema['SchemaUri'] == uri.strip():
-                request = self.session.get(f"https://{self.server}/api/admin/schemas/{schema['ApiId']}/content",
+                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/schemas/{schema['ApiId']}/content",
                                            headers=headers)
                 if request.status_code == requests.codes.ok:
                     xml_response = str(request.content.decode('utf-8'))
                     return xml_response
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_schema(uri)
@@ -613,15 +613,15 @@
         :return: The XML document as a string
         :rtype: str
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         for document in self.xml_documents():
             if document['SchemaUri'] == uri.strip():
-                request = self.session.get(f"https://{self.server}/api/admin/documents/{document['ApiId']}/content",
+                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}/content",
                                            headers=headers)
                 if request.status_code == requests.codes.ok:
                     xml_response = str(request.content.decode('utf-8'))
                     return xml_response
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_document(uri)
@@ -634,15 +634,15 @@
         fetch the list of XML documents stored in Preservica
 
         :return: List of XML documents stored in Preservica
         :rtype: list
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/admin/documents', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/admin/documents', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             documents = entity_response.findall(f'.//{{{self.admin_ns}}}Document')
             results = list()
             for document in documents:
@@ -670,15 +670,15 @@
 
         :return: List of XML schema's stored in Preservica
         :rtype: list
 
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
-        request = self.session.get(f'https://{self.server}/api/admin/schemas', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/admin/schemas', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             schemas = entity_response.findall(f'.//{{{self.admin_ns}}}Schema')
             results = []
             for schema in schemas:
@@ -705,15 +705,15 @@
         fetch the list of xml transforms stored in Preservica
 
         :return: List of XML transforms stored in Preservica
         :rtype: list
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/admin/transforms', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/admin/transforms', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             transforms = entity_response.findall(f'.//{{{self.admin_ns}}}Transform')
             results = []
             for transform in transforms:
@@ -758,15 +758,15 @@
         :return: The XML transform as a string
         :rtype: str
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         for transform in self.xml_transforms():
             if (transform['FromSchemaUri'] == input_uri.strip()) and (transform['ToSchemaUri'] == output_uri.strip()):
-                request = self.session.get(f"https://{self.server}/api/admin/transforms/{transform['ApiId']}/content",
+                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}/content",
                                            headers=headers)
                 if request.status_code == requests.codes.ok:
                     return str(request.content.decode('utf-8'))
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_transform(input_uri, output_uri)
                 else:
@@ -790,15 +790,15 @@
 
         self.__check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for transform in self.xml_transforms():
             if (transform['FromSchemaUri'] == input_uri.strip()) and (transform['ToSchemaUri'] == output_uri.strip()):
-                request = self.session.delete(f"https://{self.server}/api/admin/transforms/{transform['ApiId']}",
+                request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}",
                                               headers=headers)
                 if request.status_code == requests.codes.no_content:
                     return
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.delete_xml_transform(input_uri, output_uri)
                 else:
@@ -841,15 +841,15 @@
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"https://{self.server}/api/admin/transforms", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/transforms", headers=headers, params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
 
         if request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_transform(name, input_uri, output_uri, purpose, originalName, xml_data)
```

### Comparing `pyPreservica-1.6.3/pyPreservica/common.py` & `pyPreservica-1.7.0/pyPreservica/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -611,15 +611,15 @@
 
     def __find_user_roles_(self) -> list:
         """
         Get a list of roles for the user
         :return list of roles:
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f"https://{self.server}/api/user/details", headers=headers)
+        request = self.session.get(f"{self.protocol}://{self.server}/api/user/details", headers=headers)
         if request.status_code == requests.codes.ok:
             roles = json.loads(str(request.content.decode('utf-8')))['roles']
             return roles
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.__find_user_roles_()
 
@@ -632,15 +632,15 @@
          """
 
         if (self.major_version < 7) and (self.minor_version < 4) and (self.patch_version < 1):
             raise RuntimeError("security_tags API call is only available with a Preservica v6.3.1 system or higher")
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
-        request = self.session.get(f'https://{self.server}/api/security/tags', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/security/tags', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             security_tags = {}
             tags = entity_response.findall(f'.//{{{self.sec_ns}}}Tag')
             for tag in tags:
@@ -703,15 +703,15 @@
                 self.admin_ns = f"{NS_ADMIN}/v{self.major_version}.{self.minor_version}"
 
     def __version_number__(self):
         """
         Determine the version number of the server
         """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/versiondetails/version', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/versiondetails/version', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_ = str(request.content.decode('utf-8'))
             version = xml_[xml_.find("<CurrentVersion>") + len("<CurrentVersion>"):xml_.find("</CurrentVersion>")]
             version_numbers = version.split(".")
             self.major_version = int(version_numbers[0])
             self.minor_version = int(version_numbers[1])
             self.patch_version = int(version_numbers[2])
@@ -737,15 +737,15 @@
         config['credentials'] = {'username': self.username, 'password': self.password, 'tenant': self.tenant,
                                  'server': self.server}
         with open('credentials.properties', 'wt', encoding="utf-8") as configfile:
             config.write(configfile)
 
     def manager_token(self, username: str, password: str):
         data = {'username': username, 'password': password, 'tenant': self.tenant}
-        response = self.session.post(f'https://{self.server}/api/accesstoken/login', data=data)
+        response = self.session.post(f'{self.protocol}://{self.server}/api/accesstoken/login', data=data)
         if response.status_code == requests.codes.ok:
             return response.json()['token']
         else:
             msg = "Could not generate valid manager approval password"
             logger.error(msg)
             logger.error(response.status_code)
             logger.error(str(response.content))
@@ -754,15 +754,15 @@
     def __token__(self):
         logger.debug("Token Expired Requesting New Token")
         if self.shared_secret is False:
             if self.tenant is None:
                 data = {'username': self.username, 'password': self.password, 'includeUserDetails': 'true'}
             else:
                 data = {'username': self.username, 'password': self.password, 'tenant': self.tenant}
-            response = self.session.post(f'https://{self.server}/api/accesstoken/login', data=data)
+            response = self.session.post(f'{self.protocol}://{self.server}/api/accesstoken/login', data=data)
             if response.status_code == requests.codes.ok:
                 if self.tenant is None:
                     self.tenant = response.json()['tenant']
                 return response.json()['token']
             else:
                 msg = "Failed to create a password based authentication token. Check your credentials are correct"
                 logger.error(msg)
@@ -772,29 +772,30 @@
         if self.shared_secret is True:
             endpoint = "api/accesstoken/acquire-external"
             timestamp = int(time.time())
             to_hash = f"preservica-external-auth{timestamp}{self.username}{self.password}"
             sha1 = hashlib.sha1()
             sha1.update(to_hash.encode(encoding='utf-8'))
             data = {"username": self.username, "tenant": self.tenant, "timestamp": timestamp, "hash": sha1.hexdigest()}
-            response = self.session.post(f'https://{self.server}/{endpoint}', data=data)
+            response = self.session.post(f'{self.protocol}://{self.server}/{endpoint}', data=data)
             if response.status_code == requests.codes.ok:
                 return response.json()['token']
             else:
                 msg = "Failed to create a shared secret authentication token. Check your credentials are correct"
                 logger.error(msg)
                 raise RuntimeError(response.status_code, msg)
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False):
+                 use_shared_secret: bool = False, protocol: str = "https"):
 
         config = configparser.ConfigParser(interpolation=configparser.Interpolation())
         config.read('credentials.properties', encoding='utf-8')
         self.session = requests.Session()
         self.shared_secret = bool(use_shared_secret)
+        self.protocol = protocol
 
         if not username:
             username = os.environ.get('PRESERVICA_USERNAME')
             if username is None:
                 try:
                     username = config['credentials']['username']
                 except KeyError:
```

### Comparing `pyPreservica-1.6.3/pyPreservica/contentAPI.py` & `pyPreservica-1.7.0/pyPreservica/contentAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
 
 class ContentAPI(AuthenticatedAPI):
 
-    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False):
-        super().__init__(username, password, tenant, server, use_shared_secret)
+    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
         self.callback = None
 
     class SearchResult:
         def __init__(self, metadata, refs, hits, results_list, next_start):
             self.metadata = metadata
             self.refs = refs
             self.hits = int(hits)
@@ -51,15 +51,15 @@
         :return: Dictionary of object attributes
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/json'}
         if type(entity_type) == EntityType:
             params = {'id': f'sdb:{entity_type.value}|{reference}'}
         else:
             params = {'id': f'sdb:{entity_type}|{reference}'}
-        request = self.session.get(f'https://{self.server}/api/content/object-details', params=params, headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/content/object-details', params=params, headers=headers)
         if request.status_code == requests.codes.ok:
             return request.json()["value"]
         elif request.status_code == requests.codes.not_found:
             logger.error(f"The requested reference is not found in the repository: {reference}")
             raise RuntimeError(reference, "The requested reference is not found in the repository")
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
@@ -67,15 +67,15 @@
         else:
             logger.error(f"object_details failed with error code: {request.status_code}")
             raise RuntimeError(request.status_code, f"object_details failed with error code: {request.status_code}")
 
     def download(self, reference, filename):
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/octet-stream'}
         params = {'id': f'sdb:IO|{reference}'}
-        with self.session.get(f'https://{self.server}/api/content/download', params=params, headers=headers,
+        with self.session.get(f'{self.protocol}://{self.server}/api/content/download', params=params, headers=headers,
                               stream=True) as req:
             if req.status_code == requests.codes.ok:
                 with open(filename, 'wb') as file:
                     for chunk in req.iter_content(chunk_size=CHUNK_SIZE):
                         file.write(chunk)
                         file.flush()
                 file.close()
@@ -89,15 +89,15 @@
             else:
                 logger.error(f"download failed with error code: {req.status_code}")
                 raise RuntimeError(req.status_code, f"download failed with error code: {req.status_code}")
 
     def thumbnail(self, entity_type, reference, filename, size=Thumbnail.LARGE):
         headers = {HEADER_TOKEN: self.token, 'accept': 'image/png'}
         params = {'id': f'sdb:{entity_type}|{reference}', 'size': f'{size.value}'}
-        with self.session.get(f'https://{self.server}/api/content/thumbnail', params=params, headers=headers,
+        with self.session.get(f'{self.protocol}://{self.server}/api/content/thumbnail', params=params, headers=headers,
                               stream=True) as req:
             if req.status_code == requests.codes.ok:
                 with open(filename, 'wb') as file:
                     for chunk in req.iter_content(chunk_size=CHUNK_SIZE):
                         file.write(chunk)
                         file.flush()
                 return filename
@@ -110,15 +110,15 @@
                 raise RuntimeError(reference, "The requested reference is not found in the repository")
             else:
                 logger.error(f"thumbnail failed with error code: {req.status_code}")
                 raise RuntimeError(req.status_code, f"thumbnail failed with error code: {req.status_code}")
 
     def indexed_fields(self):
         headers = {HEADER_TOKEN: self.token}
-        results = self.session.get(f'https://{self.server}/api/content/indexed-fields', headers=headers)
+        results = self.session.get(f'{self.protocol}://{self.server}/api/content/indexed-fields', headers=headers)
         if results.status_code == requests.codes.ok:
             fields = {}
             for ob in results.json()["value"]:
                 field = f'{ob["shortName"]}.{ob["index"]}'
                 fields[field] = ob["uri"]
             return fields
         elif results.status_code == requests.codes.unauthorized:
@@ -158,15 +158,15 @@
         headers = {'Content-Type': 'application/x-www-form-urlencoded', HEADER_TOKEN: self.token}
         query_term = ('{ "q":  "%s" }' % query)
         if list_indexes is None or len(list_indexes) == 0:
             metadata_fields = "xip.title,xip.description,xip.document_type,xip.parent_ref,xip.security_descriptor"
         else:
             metadata_fields = ','.join(list_indexes)
         payload = {'start': start_from, 'max': str(page_size), 'metadata': metadata_fields, 'q': query_term}
-        results = self.session.post(f'https://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
         results_list = []
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             metadata = json_doc['value']['metadata']
             refs = list(json_doc['value']['objectIds'])
             refs = list(map(lambda x: content_api_identifier_to_type(x), refs))
             hits = int(json_doc['value']['totalHits'])
@@ -244,15 +244,15 @@
                 field_list.append('{' f' "name": "{key}", "values": ["{value}"] ' + '}')
 
         filter_terms = ','.join(field_list)
 
         query_term = ('{ "q":  "%s",  "fields":  [ %s ] }' % (query, filter_terms))
 
         payload = {'start': start_from, 'max': str(10), 'metadata': list(filter_values.keys()), 'q': query_term}
-        results = self.session.post(f'https://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             return int(json_doc['value']['totalHits'])
         elif results.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.search_index_filter_hits(query, filter_values)
         else:
@@ -273,15 +273,15 @@
 
         filter_terms = ','.join(field_list)
 
         query_term = ('{ "q":  "%s",  "fields":  [ %s ] }' % (query, filter_terms))
 
         payload = {'start': start_from, 'max': str(page_size), 'metadata': list(filter_values.keys()), 'q': query_term}
         logger.debug(payload)
-        results = self.session.post(f'https://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
         results_list = []
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             metadata = json_doc['value']['metadata']
             refs = list(json_doc['value']['objectIds'])
             refs = list(map(lambda x: content_api_identifier_to_type(x), refs))
             hits = int(json_doc['value']['totalHits'])
```

### Comparing `pyPreservica-1.6.3/pyPreservica/entityAPI.py` & `pyPreservica-1.7.0/pyPreservica/entityAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
             The EntityAPI allows users to interact with the Preservica repository
 
 
     """
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False):
-        super().__init__(username, password, tenant, server, use_shared_secret)
+                 use_shared_secret: bool = False,  protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
         xml.etree.ElementTree.register_namespace("oai_dc", "http://www.openarchives.org/OAI/2.0/oai_dc/")
         xml.etree.ElementTree.register_namespace("ead", "urn:isbn:1-931666-22-9")
 
     def user_security_tags(self, with_permissions: bool = False) -> dict:
         """
              Return  security tags available for the  current user
 
@@ -98,15 +98,15 @@
         :type pid: str
 
         :return: The downloaded zip file name
         :rtype: str
 
         """
         headers = {HEADER_TOKEN: self.__token__(), 'Content-Type': 'application/xml;charset=UTF-8'}
-        download = self.session.get(f'https://{self.server}/api/entity/actions/exports/{pid}/content',
+        download = self.session.get(f'{self.protocol}://{self.server}/api/entity/actions/exports/{pid}/content',
                                     stream=True, headers=headers)
         if download.status_code == requests.codes.ok:
             with open(f'{pid}.zip', 'wb') as file:
                 for chunk in download.iter_content(chunk_size=CHUNK_SIZE):
                     file.write(chunk)
                 file.flush()
             logger.debug(f"Downloaded open package into {pid}.zip")
@@ -174,15 +174,15 @@
         xml.etree.ElementTree.SubElement(xml_object, "IncludeMetadata").text = include_metadata
         xml.etree.ElementTree.SubElement(xml_object, "IncludedGenerations").text = include_generation
         xml.etree.ElementTree.SubElement(xml_object, "IncludeParentHierarchy").text = include_parent.lower()
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
 
         logger.debug(xml_request)
 
-        request = self.session.post(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/exports',
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/exports',
                                     headers=headers, data=xml_request)
 
         if request.status_code == requests.codes.accepted:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.__export_opex_start__(entity, IncludeContent=include_content,
@@ -252,15 +252,15 @@
            Returns the filename of the new file
 
            :param entity: The entity containing the file
            :param filename: The filename to write the bytes to
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/octet-stream'}
         params = {'id': f'sdb:{entity.entity_type.value}|{entity.reference}'}
-        with self.session.get(f'https://{self.server}/api/content/download', params=params, headers=headers,
+        with self.session.get(f'{self.protocol}://{self.server}/api/content/download', params=params, headers=headers,
                               stream=True) as request:
             if request.status_code == requests.codes.ok:
                 with open(filename, 'wb') as file:
                     for chunk in request.iter_content(chunk_size=CHUNK_SIZE):
                         file.write(chunk)
                     file.flush()
                 return filename
@@ -278,15 +278,15 @@
             Does the entity have a thumbnail image attached
             Returns false if the entity has no thumbnail
 
             :param entity: The entity
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/octet-stream'}
         params = {'id': f'sdb:{entity.entity_type.value}|{entity.reference}', 'size': f'{Thumbnail.SMALL.value}'}
-        with self.session.get(f'https://{self.server}/api/content/thumbnail', params=params,
+        with self.session.get(f'{self.protocol}://{self.server}/api/content/thumbnail', params=params,
                               headers=headers) as request:
             if request.status_code == requests.codes.ok:
                 return True
             if request.status_code == requests.codes.not_found:
                 return False
             elif request.status_code == requests.codes.unauthorized:
                 self.token = self.__token__()
@@ -305,15 +305,15 @@
 
             :param entity: The entity containing the file
             :param filename: The filename to write the bytes to
             :param size: The size of the thumbnail
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/octet-stream'}
         params = {'id': f'sdb:{entity.entity_type.value}|{entity.reference}', 'size': f'{size.value}'}
-        with self.session.get(f'https://{self.server}/api/content/thumbnail', params=params,
+        with self.session.get(f'{self.protocol}://{self.server}/api/content/thumbnail', params=params,
                               headers=headers, stream=True) as request:
             if request.status_code == requests.codes.ok:
                 with open(filename, 'wb') as file:
                     for chunk in request.iter_content(chunk_size=CHUNK_SIZE):
                         file.write(chunk)
                     file.flush()
                 return filename
@@ -339,15 +339,15 @@
              :param identifier_value: The value of the identifier to delete.
           """
 
         if (self.major_version < 7) and (self.minor_version < 1):
             raise RuntimeError("delete_identifiers API call is not available when connected to a v6.0 System")
 
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             identifier_list = entity_response.findall(f'.//{{{self.xip_ns}}}Identifier')
             for identifier_element in identifier_list:
                 _ref = _type = _value = _aipid = None
@@ -358,15 +358,15 @@
                         _type = identifier.text
                     if identifier.tag.endswith("Value") and identifier_value is not None:
                         _value = identifier.text
                     if identifier.tag.endswith("ApiId"):
                         _aipid = identifier.text
                 if _ref == entity.reference and _type == identifier_type and _value == identifier_value:
                     del_req = self.session.delete(
-                        f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers/{_aipid}',
+                        f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers/{_aipid}',
                         headers=headers)
                     if del_req.status_code == requests.codes.unauthorized:
                         self.token = self.__token__()
                         return self.delete_identifiers(entity, identifier_type, identifier_value)
                     if del_req.status_code == requests.codes.no_content:
                         pass
                     else:
@@ -385,15 +385,15 @@
 
              Returns the set of external identifiers on the entity
 
              :param entity: The entity
              :type  entity: Entity
           """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             identifier_list = entity_response.findall(f'.//{{{self.xip_ns}}}Identifier')
             result = set()
@@ -422,15 +422,15 @@
              Returns the set of entities which have the external identifier
 
              :param identifier_type: The identifier type
              :param identifier_value: The identifier value
           """
         headers = {HEADER_TOKEN: self.token}
         payload = {'type': identifier_type, 'value': identifier_value}
-        request = self.session.get(f'https://{self.server}/api/entity/entities/by-identifier', params=payload,
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/entities/by-identifier', params=payload,
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             entity_list = entity_response.findall(f'.//{{{self.entity_ns}}}Entity')
             result = set()
@@ -473,15 +473,15 @@
         xml_object = xml.etree.ElementTree.Element('Identifier', {"xmlns": self.xip_ns})
         xml.etree.ElementTree.SubElement(xml_object, "Type").text = identifier_type
         xml.etree.ElementTree.SubElement(xml_object, "Value").text = identifier_value
         xml.etree.ElementTree.SubElement(xml_object, "Entity").text = entity.reference
         end_point = f"/{entity.path}/{entity.reference}/identifiers"
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'https://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             identifier_response = xml.etree.ElementTree.fromstring(xml_string)
             aip_id = identifier_response.find(f'.//{{{self.xip_ns}}}ApiId')
             if hasattr(aip_id, 'text'):
                 return aip_id.text
             else:
@@ -528,15 +528,15 @@
 
             :param relationship:
             :return:
         """
         headers = {HEADER_TOKEN: self.token}
         entity = self.entity(relationship.entity_type, relationship.this_ref)
         end_point = f"{entity.path}/{entity.reference}/links/{relationship.api_id}"
-        request = self.session.delete(f'https://{self.server}/api/entity/{end_point}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/entity/{end_point}', headers=headers)
         if request.status_code == requests.codes.no_content:
             print(relationship)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.__delete_relationship(relationship)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url, "delete_relationships",
@@ -585,15 +585,15 @@
         """
 
         headers = {HEADER_TOKEN: self.token}
         end_point = f"{entity.path}/{entity.reference}/links"
 
         if next_page is None:
             params = {'start': '0', 'max': str(maximum)}
-            request = self.session.get(f'https://{self.server}/api/entity/{end_point}', headers=headers, params=params)
+            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{end_point}', headers=headers, params=params)
         else:
             request = self.session.get(next_page, headers=headers)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -656,15 +656,15 @@
         xml.etree.ElementTree.SubElement(xml_object, "Type").text = relationship_type
         xml.etree.ElementTree.SubElement(xml_object, "FromEntity").text = from_entity.reference
         xml.etree.ElementTree.SubElement(xml_object, "ToEntity").text = to_entity.reference
 
         end_point = f"/{from_entity.path}/{from_entity.reference}/links"
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'https://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             logger.debug(xml_string)
             link_response = xml.etree.ElementTree.fromstring(xml_string)
             relation = link_response.find(f'.//{{{self.xip_ns}}}Link')
             relation_type = relation.find(f'.//{{{self.xip_ns}}}Type')
             return relation_type.text
@@ -771,15 +771,15 @@
             tree = xml.etree.ElementTree.parse(data)
             content.append(tree.getroot())
         else:
             raise RuntimeError("Unknown data type")
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         end_point = f"/{entity.path}/{entity.reference}/metadata"
         logger.debug(xml_request)
-        request = self.session.post(f'https://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
         if request.status_code == requests.codes.ok:
             return self.entity(entity_type=entity.entity_type, reference=entity.reference)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_metadata(entity, schema, data)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url, "add_metadata",
@@ -809,15 +809,15 @@
             xml.etree.ElementTree.SubElement(xml_object, "CustomType").text = entity.custom_type
 
         if entity.parent is not None:
             xml.etree.ElementTree.SubElement(xml_object, "Parent").text = entity.parent
 
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.put(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}',
                                    data=xml_request, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             response = self.entity_from_string(xml_response)
             if isinstance(entity, Asset):
                 asset = Asset(response['reference'], response['title'], response['description'],
                               response['security_tag'],
@@ -865,30 +865,30 @@
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         if isinstance(entity, Asset) and dest_folder is None:
             raise RuntimeError(entity.reference, "Only folders can be moved to the root of the repository")
         if dest_folder is not None:
             data = dest_folder.reference
         else:
             data = "@root@"
-        request = self.session.put(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
                                    data=data, headers=headers)
         if request.status_code == requests.codes.accepted:
             return request.content.decode()
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.move_async(entity, dest_folder)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url, "move_async",
                                       request.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
     def get_async_progress(self, pid: str) -> str:
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
-        request = self.session.get(f"https://{self.server}/api/entity/progress/{pid}", headers=headers)
+        request = self.session.get(f"{self.protocol}://{self.server}/api/entity/progress/{pid}", headers=headers)
         if request.status_code == requests.codes.ok:
             entity_response = xml.etree.ElementTree.fromstring(request.content.decode("utf-8"))
             status = entity_response.find(".//{http://status.preservica.com}Status")
             if hasattr(status, 'text'):
                 return status.text
             else:
                 return "UNKNOWN"
@@ -915,15 +915,15 @@
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         if isinstance(entity, Asset) and dest_folder is None:
             raise RuntimeError(entity.reference, "Only folders can be moved to the root of the repository")
         if dest_folder is not None:
             data = dest_folder.reference
         else:
             data = "@root@"
-        request = self.session.put(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
                                    data=data, headers=headers)
         if request.status_code == requests.codes.accepted:
             sleep_sec = 1
             while True:
                 status = self.get_async_progress(request.content.decode("utf-8"))
                 if status != "ACTIVE":
                     return self.entity(entity.entity_type, entity.reference)
@@ -972,15 +972,15 @@
         xml.etree.ElementTree.SubElement(structural_object, "Description").text = description
         xml.etree.ElementTree.SubElement(structural_object, "SecurityTag").text = security_tag
         if parent is not None:
             xml.etree.ElementTree.SubElement(structural_object, "Parent").text = parent
 
         xml_request = xml.etree.ElementTree.tostring(structural_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'https://{self.server}/api/entity/structural-objects', data=xml_request,
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/structural-objects', data=xml_request,
                                     headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity = self.entity_from_string(xml_response)
             return Folder(entity['reference'], entity['title'], entity['description'],
                           entity['security_tag'],
                           entity['parent'],
@@ -1052,15 +1052,15 @@
 
          :param entity:       The entity to change
          :param new_tag:      The new security tag
          """
         self.token = self.__token__()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         end_point = f"/{entity.path}/{entity.reference}/security-descriptor"
-        request = self.session.put(f'https://{self.server}/api/entity{end_point}?includeDescendants=false',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity{end_point}?includeDescendants=false',
                                    data=new_tag, headers=headers)
         if request.status_code == requests.codes.accepted:
             sleep_sec = 1
             while True:
                 status = self.get_async_progress(request.content.decode("utf-8"))
                 if status != "ACTIVE":
                     return self.entity(entity.entity_type, entity.reference)
@@ -1083,15 +1083,15 @@
           Returns a process ID asynchronous (without blocking)
 
           :param entity:       The entity to change
           :param new_tag:      The new security tag
           """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         end_point = f"/{entity.path}/{entity.reference}/security-descriptor"
-        request = self.session.put(f'https://{self.server}/api/entity{end_point}?includeDescendants=false',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity{end_point}?includeDescendants=false',
                                    data=new_tag, headers=headers)
         if request.status_code == requests.codes.accepted:
             return request.content.decode("utf-8")
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.security_tag_async(entity, new_tag)
         else:
@@ -1165,15 +1165,15 @@
         xml.etree.ElementTree.SubElement(io_object, "SecurityTag").text = str(security_tag)
         xml.etree.ElementTree.SubElement(io_object, "Parent").text = parent.reference
         rep_object = xml.etree.ElementTree.SubElement(xip_object, "Representation")
         xml.etree.ElementTree.SubElement(rep_object, "Type").text = "Physical"
 
         xml_request = xml.etree.ElementTree.tostring(xip_object, encoding='utf-8')
 
-        request = self.session.post(f'https://{self.server}/api/entity/{IO_PATH}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/{IO_PATH}', data=xml_request, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             entity = self.entity_from_string(xml_string)
             return Asset(entity['reference'], entity['title'], entity['description'],
                          entity['security_tag'], entity['parent'],
                          entity['metadata'])
         elif request.status_code == requests.codes.unauthorized:
@@ -1190,15 +1190,15 @@
          Retrieve an Asset by its reference
 
          Returns Asset
 
          :param reference:            The unique identifier of the entity
          """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/{IO_PATH}/{reference}', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{IO_PATH}/{reference}', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity = self.entity_from_string(xml_response)
             asset = Asset(entity['reference'], entity['title'], entity['description'],
                           entity['security_tag'], entity['parent'],
                           entity['metadata'])
             if 'CustomType' in entity:
@@ -1222,15 +1222,15 @@
          Retrieve a Folder by its reference
 
          Returns Folder
 
          :param reference:            The unique identifier of the entity
          """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/{SO_PATH}/{reference}', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{SO_PATH}/{reference}', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity = self.entity_from_string(xml_response)
             folder = Folder(entity['reference'], entity['title'], entity['description'],
                             entity['security_tag'], entity['parent'],
                             entity['metadata'])
             if 'CustomType' in entity:
@@ -1254,15 +1254,15 @@
          Retrieve an ContentObject by its reference
 
          Returns ContentObject
 
          :param reference:            The unique identifier of the entity
          """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'https://{self.server}/api/entity/{CO_PATH}/{reference}', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{CO_PATH}/{reference}', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity = self.entity_from_string(xml_response)
             content_object = ContentObject(entity['reference'], entity['title'], entity['description'],
                                            entity['security_tag'], entity['parent'],
                                            entity['metadata'])
             if 'CustomType' in entity:
@@ -1498,15 +1498,15 @@
                 headers["Fixity-SHA-512"] = fixity_value
 
         headers["Filename"] = os.path.basename(file_name)
         headers['Content-Length'] = str(os.path.getsize(file_name))
 
         with open(file_name, 'rb') as f:
             request = self.session.post(
-                f'https://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations',
+                f'{self.protocol}://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations',
                 params=params, data=f, headers=headers)
 
         if request.status_code == requests.codes.ok:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             return self.replace_generation_async(content_object=content_object, file_name=file_name,
                                                  fixity_algorithm=fixity_algorithm, fixity_value=fixity_value)
@@ -1522,15 +1522,15 @@
 
         Returns list
 
         :param content_object:
         """
         headers = {HEADER_TOKEN: self.token}
         request = self.session.get(
-            f'https://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations', headers=headers)
+            f'{self.protocol}://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             generations = entity_response.findall(f'.//{{{self.entity_ns}}}Generation')
             result = []
             for g in generations:
                 if hasattr(g, 'text'):
@@ -1576,15 +1576,15 @@
 
         :param asset:   The asset
         :returns set[Representation]
         """
         headers = {HEADER_TOKEN: self.token}
         if not isinstance(asset, Asset):
             return None
-        request = self.session.get(f'https://{self.server}/api/entity/{asset.path}/{asset.reference}/representations',
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{asset.path}/{asset.reference}/representations',
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             representations = entity_response.findall(f'.//{{{self.entity_ns}}}Representation')
             result = set()
             for r in representations:
@@ -1611,15 +1611,15 @@
             raise RuntimeError("Thumbnail API is only available when connected to a v6.2 System")
 
         if isinstance(entity, ContentObject):
             raise RuntimeError("Thumbnails cannot be added to Content Objects")
 
         headers = {HEADER_TOKEN: self.token}
 
-        request = self.session.delete(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
                                       headers=headers)
         if request.status_code == requests.codes.no_content:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.remove_thumbnail(entity)
         else:
@@ -1641,15 +1641,15 @@
 
         if isinstance(entity, ContentObject):
             raise RuntimeError("Thumbnails cannot be added to Content Objects")
 
         headers = {HEADER_TOKEN: self.token}  # , 'Content-Type': 'application/octet-stream'}
 
         with open(image_file, 'rb') as fd:
-            request = self.session.put(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
+            request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
                                        data=fd, headers=headers)
 
         if request.status_code == requests.codes.no_content:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_thumbnail(entity, image_file)
@@ -1666,15 +1666,15 @@
         if self.major_version < 7 and self.minor_version < 1:
             logger.error("Entity events is only available when connected to a v6.1 System")
             raise RuntimeError("Entity events is only available when connected to a v6.1 System")
 
         headers = {HEADER_TOKEN: self.token}
         params = {'start': str(0), 'max': str(maximum)}
 
-        request = self.session.get(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
                                    params=params, headers=headers)
 
         if request.status_code == requests.codes.ok:
             pass
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._event_actions(entity, maximum=maximum)
@@ -1710,21 +1710,21 @@
 
     def children(self, folder: Folder = None, maximum: int = 100, next_page: str = None) -> PagedSet:
         headers = {HEADER_TOKEN: self.token}
         data = {'start': str(0), 'max': str(maximum)}
         folder_reference = folder
         if next_page is None:
             if folder_reference is None:
-                request = self.session.get(f'https://{self.server}/api/entity/root/children', params=data,
+                request = self.session.get(f'{self.protocol}://{self.server}/api/entity/root/children', params=data,
                                            headers=headers)
             else:
                 if hasattr(folder, "reference"):
                     folder_reference = folder.reference
                 request = self.session.get(
-                    f'https://{self.server}/api/entity/structural-objects/{folder_reference}/children',
+                    f'{self.protocol}://{self.server}/api/entity/structural-objects/{folder_reference}/children',
                     params=data, headers=headers)
         else:
             request = self.session.get(next_page, headers=headers)
         logger.debug(request.url)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
@@ -1780,15 +1780,15 @@
             paged_set = self._all_events_page(next_page=paged_set.next_page)
             for entity in paged_set.results:
                 yield entity
 
     def _entity_from_event_page(self, event_id: str, maximum: int = 25, next_page: str = None):
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         if next_page is None:
-            url = f'https://{self.server}/api/entity/events/{event_id}/event-actions'
+            url = f'{self.protocol}://{self.server}/api/entity/events/{event_id}/event-actions'
             response = requests.get(url, params={'start': 0, 'max': maximum}, headers=headers)
         else:
             response = requests.get(next_page, headers=headers)
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._entity_from_event_page(event_id, maximum, next_page)
         if response.status_code == 200:
@@ -1831,15 +1831,15 @@
             params["types"] = kwargs.get("type")
         if "from_date" in kwargs:
             params["from"] = kwargs.get("from_date")
         if "to_date" in kwargs:
             params["to"] = kwargs.get("to_date")
 
         if next_page is None:
-            request = self.session.get(f'https://{self.server}/api/entity/events', params=params, headers=headers)
+            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/events', params=params, headers=headers)
         else:
             request = self.session.get(next_page, headers=headers)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -1894,15 +1894,15 @@
             logger.error("Entity events is only available when connected to a v6.1 System")
             raise RuntimeError("Entity events is only available when connected to a v6.1 System")
 
         headers = {HEADER_TOKEN: self.token}
         params = {'start': str(0), 'max': str(maximum)}
         if next_page is None:
             request = self.session.get(
-                f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
+                f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
                 params=params, headers=headers)
         else:
             request = self.session.get(next_page, headers=headers)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
@@ -1985,15 +1985,15 @@
 
     def _updated_entities_page(self, previous_days: int = 1, maximum: int = 50, next_page: str = None) -> PagedSet:
         headers = {HEADER_TOKEN: self.token}
         x = datetime.utcnow() - timedelta(days=previous_days)
         today = x.replace(tzinfo=timezone.utc).isoformat()
         if next_page is None:
             params = {'date': today, 'start': '0', 'max': str(maximum)}
-            request = self.session.get(f'https://{self.server}/api/entity/entities/updated-since',
+            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/entities/updated-since',
                                        headers=headers, params=params)
         else:
             request = self.session.get(next_page, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -2081,20 +2081,20 @@
         xml_object = xml.etree.ElementTree.Element('DeletionAction',
                                                    {"xmlns:xip": self.xip_ns, "xmlns": self.entity_ns})
         submission_el = xml.etree.ElementTree.SubElement(xml_object, "Submission")
         comment_el = xml.etree.ElementTree.SubElement(submission_el, "Comment")
         comment_el.text = operator_comment
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.delete(f'https://{self.server}/api/entity/{entity.path}/{entity.reference}',
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}',
                                       data=xml_request, headers=headers)
         logger.debug(request.content.decode("utf-8"))
         if request.status_code == requests.codes.accepted:
             progress = request.content.decode("utf-8")
-            req = self.session.get(f"https://{self.server}/api/entity/progress/{progress}", headers=headers)
+            req = self.session.get(f"{self.protocol}://{self.server}/api/entity/progress/{progress}", headers=headers)
             while True:
                 if req.status_code == requests.codes.ok:
                     entity_response = xml.etree.ElementTree.fromstring(req.content.decode("utf-8"))
                     status = entity_response.find(".//{http://status.preservica.com}Status")
                     if hasattr(status, 'text'):
                         if status.text == "PENDING":
                             headers = {HEADER_TOKEN: self.manager_token(manager_username, manager_password),
@@ -2102,23 +2102,23 @@
                             xml_object = xml.etree.ElementTree.Element('DeletionAction ', {"xmlns:xip": self.xip_ns,
                                                                                            "xmlns": self.entity_ns})
                             approval_el = xml.etree.ElementTree.SubElement(xml_object, "Approval")
                             xml.etree.ElementTree.SubElement(approval_el, "Approved").text = "true"
                             xml.etree.ElementTree.SubElement(approval_el, "Comment").text = supervisor_comment
                             xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
                             logger.debug(xml_request)
-                            approve = self.session.put(f"https://{self.server}/api/entity/actions/deletions/{progress}",
+                            approve = self.session.put(f"{self.protocol}://{self.server}/api/entity/actions/deletions/{progress}",
                                                        data=xml_request, headers=headers)
                             if approve.status_code == requests.codes.accepted:
                                 return entity.reference
                             else:
                                 logger.error(approve.content.decode('utf-8'))
                                 raise RuntimeError(approve.status_code, "delete_asset failed during approval")
                         sleep(2.0)
-                req = self.session.get(f"https://{self.server}/api/entity/progress/{progress}", headers=headers)
+                req = self.session.get(f"{self.protocol}://{self.server}/api/entity/progress/{progress}", headers=headers)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._delete_entity(entity, operator_comment, supervisor_comment)
         if request.status_code == requests.codes.unprocessable:
             logger.error(request.content.decode('utf-8'))
             raise RuntimeError(request.status_code, "no active workflow context for full deletion exists in the system")
         if request.status_code == requests.codes.forbidden:
```

### Comparing `pyPreservica-1.6.3/pyPreservica/monitorAPI.py` & `pyPreservica-1.7.0/pyPreservica/monitorAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def _messages_page_(self, monitor_id, maximum: int = 50, next_page: str = None, status: MessageStatus = None) -> PagedSet:
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/json;charset=UTF-8'}
 
         if next_page is None:
             params = {'monitor': monitor_id, 'start': int(0), 'max': maximum}
             if status:
                 params['status'] = status.value
-            request = self.session.get(f'https://{self.server}/api/processmonitor/messages', headers=headers,
+            request = self.session.get(f'{self.protocol}://{self.server}/api/processmonitor/messages', headers=headers,
                                        params=params)
         else:
             params = {'monitor': monitor_id}
             if status:
                 params['status'] = status.value
             request = self.session.get(next_page, headers=headers, params=params)
         if request.status_code == requests.codes.ok:
@@ -108,15 +108,15 @@
         Get the historical record of progress for a single monitor
 
         :param monitor_id:  The Process ID
         :type monitor_id:   str
         :return: List of timeseries information
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/json;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/processmonitor/monitors/{monitor_id}/timeseries',
+        request = self.session.get(f'{self.protocol}://{self.server}/api/processmonitor/monitors/{monitor_id}/timeseries',
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             response = json.loads(str(request.content.decode('utf-8')))
             return response['value']['timeseries']
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.timeseries(monitor_id)
@@ -136,15 +136,15 @@
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/json;charset=UTF-8'}
         params = {}
         if status:
             params['status'] = status.value
         if category:
             params['category'] = category.value
-        request = self.session.get(f'https://{self.server}/api/processmonitor/monitors', headers=headers, params=params)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/processmonitor/monitors', headers=headers, params=params)
         if request.status_code == requests.codes.ok:
             monitors = json.loads(str(request.content.decode('utf-8')))
             for monitor in monitors['value']['monitors']:
                 monitor['MonitorId'] = monitor.pop('mappedId')
                 yield monitor
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
```

### Comparing `pyPreservica-1.6.3/pyPreservica/opex.py` & `pyPreservica-1.7.0/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.6.3/pyPreservica/parAPI.py` & `pyPreservica-1.7.0/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.6.3/pyPreservica/retentionAPI.py` & `pyPreservica-1.7.0/pyPreservica/retentionAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
     def __repr__(self):
         return self.__str__()
 
 
 class RetentionAPI(AuthenticatedAPI):
 
-    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False):
-        super().__init__(username, password, tenant, server, use_shared_secret)
+    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
         if self.major_version < 7 and self.minor_version < 2:
             raise RuntimeError("Retention API is only available when connected to a v6.2 System")
 
     def policy(self, reference: str) -> RetentionPolicy:
         """
          Return a retention policy by reference
 
@@ -71,15 +71,15 @@
         :type reference: str
 
         :return: The retention policy
         :rtype: RetentionPolicy
 
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.get(f'https://{self.server}/api/entity/retention-policies/{reference}', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/retention-policies/{reference}', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             ref = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}Ref').text
             assert ref == reference
             name = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}Name').text
@@ -92,16 +92,19 @@
                 f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}StartDateField').text
             rp.start_date_field = start_date_field
             period = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}Period').text
             rp.period = period
             period_unit = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}PeriodUnit').text
             rp.period_unit = period_unit
             expiry_action = entity_response.find(
-                f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}ExpiryAction').text
-            rp.expiry_action = expiry_action
+                f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}ExpiryAction')
+            if expiry_action is not None:
+                rp.expiry_action = expiry_action.text
+            else:
+                rp.expiry_action = None
             restriction = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}Restriction')
             if restriction is not None:
                 rp.restriction = restriction.text
             else:
                 rp.restriction = None
             assignable = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy/{{{self.rm_ns}}}Assignable')
             rp.assignable = strtobool(assignable.text)
@@ -124,15 +127,15 @@
         :type status: bool
 
 
         :return:
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain;charset=UTF-8'}
         data = str(status)
-        request = self.session.put(f'https://{self.server}/api/entity/retention-policies/{reference}/assignable',
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/retention-policies/{reference}/assignable',
                                    headers=headers, data=data)
         if request.status_code == requests.codes.ok:
             pass
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.assignable_policy(reference, status)
         else:
@@ -220,15 +223,15 @@
         xml.etree.ElementTree.SubElement(retention_policy, "ExpiryAction").text = expiry_action
         xml.etree.ElementTree.SubElement(retention_policy, "ExpiryActionParameters").text = expiry_action_parameters
         xml.etree.ElementTree.SubElement(retention_policy, "Restriction").text = restriction
         xml.etree.ElementTree.SubElement(retention_policy, "Assignable").text = str(assignable)
 
         xml_request = xml.etree.ElementTree.tostring(retention_policy, encoding='utf-8')
 
-        request = self.session.put(f'https://{self.server}/api/entity/retention-policies/{reference}', data=xml_request,
+        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/retention-policies/{reference}', data=xml_request,
                                    headers=headers)
         if request.status_code == requests.codes.ok:
             return self.policy(reference)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.update_policy(reference, **kwargs)
         else:
@@ -315,15 +318,15 @@
         xml.etree.ElementTree.SubElement(retention_policy, "ExpiryAction").text = expiry_action
         xml.etree.ElementTree.SubElement(retention_policy, "ExpiryActionParameters").text = expiry_action_parameters
         xml.etree.ElementTree.SubElement(retention_policy, "Restriction").text = restriction
         xml.etree.ElementTree.SubElement(retention_policy, "Assignable").text = str(assignable)
 
         xml_request = xml.etree.ElementTree.tostring(retention_policy, encoding='utf-8')
 
-        request = self.session.post(f'https://{self.server}/api/entity/retention-policies', data=xml_request,
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/retention-policies', data=xml_request,
                                     headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             retention_policy = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy')
             ref = retention_policy.find(f'.//{{{self.rm_ns}}}Ref').text
             return self.policy(ref)
@@ -340,15 +343,15 @@
         Delete a retention policy
 
         :param reference: The policy reference
         :type reference: str
 
         """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.delete(f'https://{self.server}/api/entity/retention-policies/{reference}',
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/entity/retention-policies/{reference}',
                                       headers=headers)
         if request.status_code == requests.codes.no_content:
             pass
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_policy(reference)
         else:
@@ -364,15 +367,15 @@
 
         :return: The retention policy
         :rtype: RetentionPolicy
 
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         data = {'start': str(0), 'max': "250"}
-        request = self.session.get(f'https://{self.server}/api/entity/retention-policies', data=data, headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/retention-policies', data=data, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             for assignment in entity_response.findall(f'.//{{{self.entity_ns}}}RetentionPolicy'):
                 ref = assignment.attrib['ref']
                 policy_name = assignment.attrib['name']
@@ -392,15 +395,15 @@
 
         :return: Set of retention policies
         :rtype: Set[RetentionPolicy]
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         data = {'start': str(0), 'max': "250"}
-        request = self.session.get(f'https://{self.server}/api/entity/retention-policies', data=data, headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/retention-policies', data=data, headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             logger.debug(xml_response)
             result = set()
             total_results = int(entity_response.find(
                 f'.//{{{self.entity_ns}}}TotalResults').text)
@@ -436,15 +439,15 @@
             raise RuntimeError("Retention policies can only be assigned to Assets")
 
         assignment = xml.etree.ElementTree.Element('RetentionAssignment', {"xmlns": self.rm_ns})
         xml.etree.ElementTree.SubElement(assignment, "RetentionPolicy").text = policy.reference
         xml_request = xml.etree.ElementTree.tostring(assignment, encoding='utf-8').decode('utf-8')
         logger.debug(xml_request)
         request = self.session.post(
-            f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/retention-assignments',
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/retention-assignments',
             headers=headers, data=xml_request)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             api_id = entity_response.find(f'.//{{{self.rm_ns}}}ApiId').text
             policy_ref = entity_response.find(f'.//{{{self.rm_ns}}}RetentionPolicy').text
@@ -473,15 +476,15 @@
         :rtype: str
 
         """
 
         headers = {HEADER_TOKEN: self.token}
 
         request = self.session.delete(
-            f'https://{self.server}/api/entity/information-objects/{retention_assignment.entity_reference}/retention'
+            f'{self.protocol}://{self.server}/api/entity/information-objects/{retention_assignment.entity_reference}/retention'
             f'-assignments/{retention_assignment.api_id}', headers=headers)
         if request.status_code == requests.codes.no_content:
             return retention_assignment.entity_reference
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.remove_assignments(retention_assignment)
         else:
@@ -496,15 +499,15 @@
 
           :return: Set of policy assignments
           :rtype: Set[RetentionAssignment]
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(
-            f'https://{self.server}/api/entity/{entity.path}/{entity.reference}/retention-assignments',
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/retention-assignments',
             headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             result = set()
             for assignment in entity_response.findall(f'.//{{{self.rm_ns}}}RetentionAssignment'):
                 entity_ref = assignment.find(f'.//{{{self.rm_ns}}}Entity').text
```

### Comparing `pyPreservica-1.6.3/pyPreservica/uploadAPI.py` & `pyPreservica-1.7.0/pyPreservica/uploadAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import base64
 import csv
 import shutil
 import tempfile
 import uuid
 import xml
 from datetime import datetime
 from time import sleep
@@ -1185,15 +1184,14 @@
                                                tenant=self.tenant)
         if hasattr(folder, "reference"):
             folder = entity_client.folder(folder.reference)
         else:
             folder = entity_client.folder(folder)
         try:
             import tweepy
-            from tweepy import TweepError
         except ImportError:
             logger.error("Package tweepy is required for twitter harvesting. pip install --upgrade tweepy")
             raise RuntimeError("Package tweepy is required for twitter harvesting. pip install --upgrade tweepy")
         config = configparser.ConfigParser()
         config.read('credentials.properties')
         if twitter_consumer_key is None:
             twitter_consumer_key = os.environ.get('TWITTER_CONSUMER_KEY')
@@ -1371,15 +1369,14 @@
                                                tenant=self.tenant)
         if hasattr(folder, "reference"):
             folder = entity_client.folder(folder.reference)
         else:
             folder = entity_client.folder(folder)
         try:
             import tweepy
-            # from tweepy import TweepError
         except ImportError:
             logger.error("Package tweepy is required for twitter harvesting. pip install --upgrade tweepy")
             raise RuntimeError("Package tweepy is required for twitter harvesting. pip install --upgrade tweepy")
         config = configparser.ConfigParser()
         config.read('credentials.properties')
         if twitter_consumer_key is None:
             twitter_consumer_key = os.environ.get('TWITTER_CONSUMER_KEY')
@@ -1723,22 +1720,23 @@
     def upload_zip_package_to_Azure(self, path_to_zip_package, container_name, folder=None, delete_after_upload=False,
                                     show_progress=False):
 
         """
          Uploads a zip file package to an Azure container connected to a Preservica Cloud System
 
          :param str path_to_zip_package: Path to the package
-         :param str container_name: container connected to an ingest workflow
+         :param str container_name: container connected to the ingest workflow
          :param Folder folder: The folder to ingest the package into
          :param bool delete_after_upload: Delete the local copy of the package after the upload has completed
 
         """
 
         if (self.major_version < 7) and (self.minor_version < 5):
-            raise RuntimeError("This call [upload_zip_package_to_Azure] is only available against v6.5 systems and above")
+            raise RuntimeError(
+                "This call [upload_zip_package_to_Azure] is only available against v6.5 systems and above")
 
         from azure.storage.blob import ContainerClient
 
         if (self.major_version > 5) and (self.minor_version > 4):
             locations = self.upload_locations()
             for location in locations:
                 if location['containerName'] == container_name:
@@ -1746,32 +1744,35 @@
                     account_key = credentials['key']
                     session_token = credentials['sessionToken']
 
                     sas_url = f"https://{account_key}.blob.core.windows.net/{container_name}"
                     container = ContainerClient.from_container_url(container_url=sas_url, credential=session_token)
 
                     upload_key = str(uuid.uuid4())
-                    metadata = {'key': upload_key, 'name': upload_key + ".zip", 'bucket': container_name, 'status': 'ready'}
+                    metadata = {'key': upload_key, 'name': upload_key + ".zip", 'bucket': container_name,
+                                'status': 'ready'}
 
                     if hasattr(folder, "reference"):
                         metadata['collectionreference'] = folder.reference
                     elif isinstance(folder, str):
                         metadata['collectionreference'] = folder
 
                     properties = None
 
                     len_bytes = Path(path_to_zip_package).stat().st_size
 
                     if show_progress:
                         with tqdm.wrapattr(open(path_to_zip_package, 'rb'), "read", total=len_bytes) as data:
-                            blob_client = container.upload_blob(name=upload_key, data=data, metadata=metadata, length=len_bytes)
+                            blob_client = container.upload_blob(name=upload_key, data=data, metadata=metadata,
+                                                                length=len_bytes)
                             properties = blob_client.get_blob_properties()
                     else:
                         with open(path_to_zip_package, "rb") as data:
-                            blob_client = container.upload_blob(name=upload_key, data=data, metadata=metadata, length=len_bytes)
+                            blob_client = container.upload_blob(name=upload_key, data=data, metadata=metadata,
+                                                                length=len_bytes)
                             properties = blob_client.get_blob_properties()
 
                     if delete_after_upload:
                         os.remove(path_to_zip_package)
 
                     return properties
 
@@ -1798,37 +1799,38 @@
                 if location['containerName'] == bucket_name:
                     credentials = self.upload_credentials(location['apiId'])
                     access_key = credentials['key']
                     secret_key = credentials['secret']
                     session_token = credentials['sessionToken']
                     endpoint = credentials['endpoint']
 
-            session = boto3.Session(aws_access_key_id=access_key, aws_secret_access_key=secret_key,
-                                    aws_session_token=session_token)
-            s3 = session.resource(service_name="s3")
+                    session = boto3.Session(aws_access_key_id=access_key, aws_secret_access_key=secret_key,
+                                            aws_session_token=session_token)
+                    s3 = session.resource(service_name="s3")
 
-            upload_key = str(uuid.uuid4())
-            s3_object = s3.Object(bucket_name, upload_key)
-            metadata = {'key': upload_key, 'name': upload_key + ".zip", 'bucket': bucket_name, 'status': 'ready'}
+                    upload_key = str(uuid.uuid4())
+                    s3_object = s3.Object(bucket_name, upload_key)
+                    metadata = {'key': upload_key, 'name': upload_key + ".zip", 'bucket': bucket_name,
+                                'status': 'ready'}
 
-            if hasattr(folder, "reference"):
-                metadata['collectionreference'] = folder.reference
-            elif isinstance(folder, str):
-                metadata['collectionreference'] = folder
+                    if hasattr(folder, "reference"):
+                        metadata['collectionreference'] = folder.reference
+                    elif isinstance(folder, str):
+                        metadata['collectionreference'] = folder
 
-            metadata['size'] = str(Path(path_to_zip_package).stat().st_size)
-            metadata['createdby'] = self.username
+                    metadata['size'] = str(Path(path_to_zip_package).stat().st_size)
+                    metadata['createdby'] = self.username
 
-            metadata_map = {'Metadata': metadata}
+                    metadata_map = {'Metadata': metadata}
 
-            s3_object.upload_file(path_to_zip_package, Callback=callback, ExtraArgs=metadata_map,
-                                  Config=transfer_config)
+                    s3_object.upload_file(path_to_zip_package, Callback=callback, ExtraArgs=metadata_map,
+                                          Config=transfer_config)
 
-            if delete_after_upload:
-                os.remove(path_to_zip_package)
+                    if delete_after_upload:
+                        os.remove(path_to_zip_package)
 
     def upload_zip_package(self, path_to_zip_package, folder=None, callback=None, delete_after_upload=False):
         """
         Uploads a zip file package directly to Preservica and starts an ingest workflow
 
         :param str path_to_zip_package: Path to the package
         :param Folder folder: The folder to ingest the package into
```

### Comparing `pyPreservica-1.6.3/pyPreservica/workflowAPI.py` & `pyPreservica-1.7.0/pyPreservica/workflowAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
     """
 
     workflow_states = ['Aborted', 'Active', 'Completed', 'Finished_Mixed_Outcome', 'Pending', 'Suspended', 'Unknown',
                        'Failed']
     workflow_types = ['Ingest', 'Access', 'Transformation', 'DataManagement']
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False):
-        super().__init__(username, password, tenant, server, use_shared_secret)
+                 use_shared_secret: bool = False, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
         self.base_url = "sdb/rest/workflow"
 
     def get_workflow_contexts_by_type(self, workflow_type: str):
         """
         Return a list of Workflow Contexts which have the same Workflow type
 
         :param workflow_type: The Workflow type  Ingest, Access, Transformation or DataManagement
@@ -114,15 +114,15 @@
         :rtype: list
 
         """
 
         headers = {HEADER_TOKEN: self.token}
         params = {"type": workflow_type}
         workflow_contexts = []
-        request = self.session.get(f'https://{self.server}/{self.base_url}/contexts', headers=headers, params=params)
+        request = self.session.get(f'{self.protocol}://{self.server}/{self.base_url}/contexts', headers=headers, params=params)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             contexts = entity_response.findall(f".//{{{NS_WORKFLOW}}}WorkflowContext")
             for context in contexts:
                 wrkfl_id = context.find(f".//{{{NS_WORKFLOW}}}Id").text
                 name = context.find(f".//{{{NS_WORKFLOW}}}Name").text
@@ -147,15 +147,15 @@
         :rtype: list
 
         """
 
         headers = {HEADER_TOKEN: self.token}
         params = {"workflowDefinitionId": definition}
         workflow_contexts = []
-        request = self.session.get(f'https://{self.server}/{self.base_url}/contexts', headers=headers, params=params)
+        request = self.session.get(f'{self.protocol}://{self.server}/{self.base_url}/contexts', headers=headers, params=params)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             contexts = entity_response.findall(f".//{{{NS_WORKFLOW}}}WorkflowContext")
             for context in contexts:
                 wrkfl_id = context.find(f".//{{{NS_WORKFLOW}}}Id").text
                 name = context.find(f".//{{{NS_WORKFLOW}}}Name").text
@@ -198,15 +198,15 @@
             parameter = xml.etree.ElementTree.SubElement(request_payload, "Parameter")
             xml.etree.ElementTree.SubElement(parameter, "Key").text = key
             xml.etree.ElementTree.SubElement(parameter, "Value").text = value
 
         xml.etree.ElementTree.SubElement(request_payload, "CorrelationId").text = correlation_id
 
         xml_request = xml.etree.ElementTree.tostring(request_payload, encoding='utf-8')
-        request = self.session.post(f'https://{self.server}/{self.base_url}/instances', headers=headers,
+        request = self.session.post(f'{self.protocol}://{self.server}/{self.base_url}/instances', headers=headers,
                                     data=xml_request)
         if request.status_code == requests.codes.created:
             return correlation_id
         if request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.start_workflow_instance(workflow_context, **kwargs)
         else:
@@ -226,15 +226,15 @@
             converted_list = [str(int(e)) for e in instance_ids]
             param_string = ",".join(converted_list)
         else:
             param_string = str(int(instance_ids))
 
         headers = {HEADER_TOKEN: self.token}
         params = {"workflowInstanceIds": param_string}
-        request = self.session.post(f'https://{self.server}/{self.base_url}/instances/terminate',
+        request = self.session.post(f'{self.protocol}://{self.server}/{self.base_url}/instances/terminate',
                                     headers=headers, params=params)
         if request.status_code == requests.codes.accepted:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.terminate_workflow_instance(instance_ids)
         else:
@@ -251,15 +251,15 @@
         :return: workflow_instance
         :rtype: WorkflowInstance
 
         """
 
         headers = {HEADER_TOKEN: self.token}
         params = {"includeErrors": "true"}
-        request = self.session.get(f'https://{self.server}/{self.base_url}/instances/{str(instance_id)}',
+        request = self.session.get(f'{self.protocol}://{self.server}/{self.base_url}/instances/{str(instance_id)}',
                                    headers=headers, params=params)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             w_id = int(entity_response.find(f".//{{{NS_WORKFLOW}}}Id").text)
             assert instance_id == w_id
@@ -355,15 +355,15 @@
         if "to" in kwargs:
             to_date = kwargs.get("to")
             params["to"] = to_date
 
         params["start"] = int(start_value)
         params["max"] = int(maximum)
 
-        request = self.session.get(f'https://{self.server}/{self.base_url}/instances', headers=headers, params=params)
+        request = self.session.get(f'{self.protocol}://{self.server}/{self.base_url}/instances', headers=headers, params=params)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             total_count = int(entity_response.find(f".//{{{NS_WORKFLOW}}}TotalCount").text)
             count = int(entity_response.find(f".//{{{NS_WORKFLOW}}}Count").text)
             workflow_instance = entity_response.findall(f".//{{{NS_WORKFLOW}}}WorkflowInstance")
```

### Comparing `pyPreservica-1.6.3/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-1.7.0/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.6.3/setup.py` & `pyPreservica-1.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="1.6.3",
+    version="1.7.0",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
@@ -37,14 +37,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: System :: Archiving",
     ],
     keywords='Preservica API Preservation',
-    install_requires=["requests", "certifi", "boto3", "botocore", "s3transfer", "cryptography", "azure-storage-blob", "tqdm"],
+    install_requires=["requests", "certifi", "boto3", "botocore", "s3transfer", "azure-storage-blob", "tqdm"],
     project_urls={
         'Documentation': 'https://pypreservica.readthedocs.io',
         'Source': 'https://github.com/carj/pyPreservica',
         'Discussion Forum': 'https://groups.google.com/g/pypreservica',
     }
 )
```

