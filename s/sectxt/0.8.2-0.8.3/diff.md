# Comparing `tmp/sectxt-0.8.2.tar.gz` & `tmp/sectxt-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectxt-0.8.2.tar", last modified: Fri Apr 14 08:14:18 2023, max compression
+gzip compressed data, was "sectxt-0.8.3.tar", last modified: Mon Apr 17 09:00:15 2023, max compression
```

## Comparing `sectxt-0.8.2.tar` & `sectxt-0.8.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.023958 sectxt-0.8.2/
--rw-rw-rw-   0        0        0    13827 2023-04-14 07:57:53.000000 sectxt-0.8.2/LICENCE
--rw-rw-rw-   0        0        0    10927 2023-04-14 08:14:18.024885 sectxt-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     9876 2023-04-14 07:57:53.000000 sectxt-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 08:14:17.985293 sectxt-0.8.2/sectxt/
--rw-rw-rw-   0        0        0    17312 2023-04-14 07:57:53.000000 sectxt-0.8.2/sectxt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.020958 sectxt-0.8.2/sectxt.egg-info/
--rw-rw-rw-   0        0        0    10927 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 08:14:17.000000 sectxt-0.8.2/sectxt.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1021 2023-04-14 08:14:18.027878 sectxt-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-04-14 07:57:53.000000 sectxt-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:14:18.021956 sectxt-0.8.2/test/
--rw-rw-rw-   0        0        0     9029 2023-04-14 07:57:53.000000 sectxt-0.8.2/test/test_sectxt.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.918703 sectxt-0.8.3/
+-rw-rw-rw-   0        0        0    13827 2023-04-17 08:37:08.000000 sectxt-0.8.3/LICENCE
+-rw-rw-rw-   0        0        0    10776 2023-04-17 09:00:15.920744 sectxt-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9725 2023-04-17 08:37:08.000000 sectxt-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.885722 sectxt-0.8.3/sectxt/
+-rw-rw-rw-   0        0        0    17133 2023-04-17 08:37:08.000000 sectxt-0.8.3/sectxt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.915734 sectxt-0.8.3/sectxt.egg-info/
+-rw-rw-rw-   0        0        0    10776 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1021 2023-04-17 09:00:15.928702 sectxt-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-04-17 08:37:08.000000 sectxt-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.916700 sectxt-0.8.3/test/
+-rw-rw-rw-   0        0        0     8679 2023-04-17 08:37:08.000000 sectxt-0.8.3/test/test_sectxt.py
```

### Comparing `sectxt-0.8.2/LICENCE` & `sectxt-0.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `sectxt-0.8.2/PKG-INFO` & `sectxt-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.2
+Version: 0.8.3
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -94,33 +94,33 @@
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
 | "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
-| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+| "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
 
 
 ### Possible recommendations
 
-| code                       | message                                                                                |
-|----------------------------|----------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
-| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
+| code                       | message                                                                                        |
+|----------------------------|------------------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."         |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                     |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
+| "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
-| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
+
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.2/README.md` & `sectxt-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,33 @@
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
 | "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
-| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+| "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
 
 
 ### Possible recommendations
 
-| code                       | message                                                                                |
-|----------------------------|----------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
-| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
+| code                       | message                                                                                        |
+|----------------------------|------------------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."         |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                     |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
+| "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
-| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
+
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.2/sectxt/__init__.py` & `sectxt-0.8.3/sectxt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 import dateutil.parser
 import requests
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 s = requests.Session()
 
 
 class ErrorDict(TypedDict):
     code: str
     message: str
@@ -285,29 +285,24 @@
             self._add_error(
                 "no_line_separators",
                 "Every line must end with either a carriage "
                 "return and line feed characters or just a line "
                 "feed character",
             )
 
-        if "csaf" not in self._values:
-            self._add_recommendation(
-                "no_csaf", "'CSAF' field should appear at least once"
-            )
-        else:
+        if "csaf" in self._values:
             if not all(
                 v.endswith("provider-metadata.json") for v in self._values["csaf"]
             ):
                 self._add_error(
                     "no_csaf_file",
-                    "All CSAF field in the security.txt must point "
-                    "to a provider-metadata.json file",
+                    "All CSAF fields must point to a provider-metadata.json file.",
                 )
             if len(self._values["csaf"]) > 1:
-                self._add_notification(
+                self._add_recommendation(
                     "multiple_csaf_fields",
                     "It is allowed to have more than one csaf field, "
                     "however this should be removed if possible.",
                 )
 
         if "contact" not in self._values:
             self._add_error("no_contact", "'Contact' field must appear at least once.")
```

### Comparing `sectxt-0.8.2/sectxt.egg-info/PKG-INFO` & `sectxt-0.8.3/sectxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.2
+Version: 0.8.3
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -94,33 +94,33 @@
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
 | "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
-| "no_csaf_file"        | "All CSAF field in the security.txt must point to a provider-metadata.json file"                                                                                       |
+| "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
 
 
 ### Possible recommendations
 
-| code                       | message                                                                                |
-|----------------------------|----------------------------------------------------------------------------------------|
-| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."         |
-| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address." |
-| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                             |
-| "no_canonical"             | "'Canonical' field should be present in a signed file."                                |
-| "no_csaf"                  | "'CSAF' field should appear at least once"                                             |
+| code                       | message                                                                                        |
+|----------------------------|------------------------------------------------------------------------------------------------|
+| "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
+| "no_encryption"            | "'Encryption' field should be present when 'Contact' field contains an email address."         |
+| "not_signed"<sup>[1]</sup> | "security.txt should be digitally signed."                                                     |
+| "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
+| "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
-| "multiple_csaf_fields"        | "It is allowed to have more than one CSAF field, however this should be removed if possible."                                                                               |
+
 
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.2/setup.cfg` & `sectxt-0.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sectxt-0.8.2/test/test_sectxt.py` & `sectxt-0.8.3/test/test_sectxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,24 +179,14 @@
         )
         p = Parser(single_line_security_txt)
         self.assertFalse(p.is_valid())
         self.assertEqual(
             len([1 for r in p._errors if r["code"] == "no_line_separators"]), 1
         )
 
-    def test_csaf_optional(self):
-        content = _signed_example.replace(
-            "CSAF: https://example.com/.well-known/csaf/provider-metadata.json", ""
-        )
-        p = Parser(content)
-        self.assertTrue(p.is_valid())
-        self.assertEqual(
-            len([1 for r in p._recommendations if r["code"] == "no_csaf"]), 1
-        )
-
     def test_csaf_https_uri(self):
         content = _signed_example.replace(
             "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
             "CSAF: http://example.com/.well-known/csaf/provider-metadata.json",
         )
         p = Parser(content)
         self.assertFalse(p.is_valid())
@@ -216,15 +206,15 @@
             "# CSAF link",
             "# CSAF link\n"
             "CSAF: https://example2.com/.well-known/csaf/provider-metadata.json",
         )
         p = Parser(content)
         self.assertTrue(p.is_valid())
         self.assertEqual(
-            len([1 for r in p._notifications if r["code"] == "multiple_csaf_fields"]), 1
+            len([1 for r in p._recommendations if r["code"] == "multiple_csaf_fields"]), 1
         )
 
 
 def test_not_correct_path(requests_mock: Mocker):
     with Mocker() as m:
         m.get(
             "https://example.com/.well-known/security.txt",
```

