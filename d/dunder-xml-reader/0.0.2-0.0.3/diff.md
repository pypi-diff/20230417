# Comparing `tmp/dunder_xml_reader-0.0.2.tar.gz` & `tmp/dunder_xml_reader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunder_xml_reader-0.0.2.tar", last modified: Mon Aug 15 20:54:11 2022, max compression
+gzip compressed data, was "dunder_xml_reader-0.0.3.tar", last modified: Mon Apr 17 20:17:15 2023, max compression
```

## Comparing `dunder_xml_reader-0.0.2.tar` & `dunder_xml_reader-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:54:11.273389 dunder_xml_reader-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    51352 2022-08-15 20:54:11.273389 dunder_xml_reader-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10941 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:54:11.269389 dunder_xml_reader-0.0.2/dunder_xml_reader/
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/dunder_xml_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/dunder_xml_reader/safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/dunder_xml_reader/xml_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/dunder_xml_reader/xml_node_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:54:11.269389 dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    51352 2022-08-15 20:54:11.000000 dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-15 20:54:11.000000 dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 20:54:11.000000 dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-15 20:54:11.000000 dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-15 20:54:11.273389 dunder_xml_reader-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:54:11.273389 dunder_xml_reader-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/test/test_safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4964 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/test/test_xml_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     7974 2022-08-15 20:53:27.000000 dunder_xml_reader-0.0.2/test/test_xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/dunder_xml_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_xml_node_list.py
```

### Comparing `dunder_xml_reader-0.0.2/LICENSE` & `dunder_xml_reader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.2/PKG-INFO` & `dunder_xml_reader-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunder_xml_reader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -903,14 +903,55 @@
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
     >>> cxml = parse_xml(raw_xml_text)
     >>> print(cxml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
+### XML with namespaces ###
+
+The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
+this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+for example:
+
+    <?xml version="1.0" encoding="UTF-8"?>
+    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
+      <soapenv:Body>
+        <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
+          <ClaimResponse>
+            <status>S</status>
+            <errorDetail/>
+            <claimNumber>LC0000001742</claimNumber>
+          </ClaimResponse>
+        </ReceiveClaimResponse>
+      </soapenv:Body>
+    </soapenv:Envelope>
+
+Using the `namespaces` argument to `parse_xml()`, you can have the attributes prefixed with
+an alias:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/': 'soap',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job': 'claim'
+    ... }
+    >>> soap.soap_Body.claim_ReceiveClaimResponse.claim_ClaimResponse.claim_status.text()
+    S
+    >>>
+
+If you don't want any prefixes and you just want to strip out the namespace references you
+can either pass a `set` of namespace strings to `parse_xml()`:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job'
+    ... }
+    >>> soap.Body.ReceiveClaimResponse.ClaimResponse.status.text()
+    S
+    >>>
+
 ## Bonus: SafeReference ##
 
 SafeReference is a wrapper that you can wrap a xmlNode instance in (or any other Python object
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
```

### Comparing `dunder_xml_reader-0.0.2/README.md` & `dunder_xml_reader-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -227,14 +227,55 @@
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
     >>> cxml = parse_xml(raw_xml_text)
     >>> print(cxml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
+### XML with namespaces ###
+
+The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
+this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+for example:
+
+    <?xml version="1.0" encoding="UTF-8"?>
+    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
+      <soapenv:Body>
+        <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
+          <ClaimResponse>
+            <status>S</status>
+            <errorDetail/>
+            <claimNumber>LC0000001742</claimNumber>
+          </ClaimResponse>
+        </ReceiveClaimResponse>
+      </soapenv:Body>
+    </soapenv:Envelope>
+
+Using the `namespaces` argument to `parse_xml()`, you can have the attributes prefixed with
+an alias:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/': 'soap',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job': 'claim'
+    ... }
+    >>> soap.soap_Body.claim_ReceiveClaimResponse.claim_ClaimResponse.claim_status.text()
+    S
+    >>>
+
+If you don't want any prefixes and you just want to strip out the namespace references you
+can either pass a `set` of namespace strings to `parse_xml()`:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job'
+    ... }
+    >>> soap.Body.ReceiveClaimResponse.ClaimResponse.status.text()
+    S
+    >>>
+
 ## Bonus: SafeReference ##
 
 SafeReference is a wrapper that you can wrap a xmlNode instance in (or any other Python object
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
```

### Comparing `dunder_xml_reader-0.0.2/dunder_xml_reader/__init__.py` & `dunder_xml_reader-0.0.3/dunder_xml_reader/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,25 @@
 """
 import xml.etree.ElementTree
 
 from dunder_xml_reader.xml_node import XmlNode
 from dunder_xml_reader.safe_reference import SafeReference
 
 
-def parse_xml(raw_text: str) -> XmlNode:
+def parse_xml(raw_text: str, namespaces=None) -> XmlNode:
     """
     Parse raw_text as XML and return a XmlNode instance of the root.
     :param raw_text: string holding valid XML
+    :param namespaces: dict of namespaces
     :return: XmlNode instance pointing to root of XML
     """
     node = xml.etree.ElementTree.fromstring(raw_text)
-    return XmlNode(node=node, parent_node=None, raw_text=raw_text)
+    
+    return XmlNode(node=node, parent_node=None, raw_text=raw_text, \
+                   namespaces=namespaces)
 
 
 def safe_reference(object, default='') -> SafeReference:
     """
     Wrap object graph in a SafeReference instance.
     :param object: The object to wrap
     :param default: What should be returned instead of throwing Exception
```

### Comparing `dunder_xml_reader-0.0.2/dunder_xml_reader/safe_reference.py` & `dunder_xml_reader-0.0.3/dunder_xml_reader/safe_reference.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.2/dunder_xml_reader/xml_node.py` & `dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,34 @@
     Using Python's built-in ElementTree package can be involved, especially when you
     are simply trying to just read data out of a CXML order for mapping.  The purpose
     of this class is to simply quick extraction of data out of a CXML order.  It is
     a dynamic class that exposes child-nodes as Python class attributes.  See the
     GitHub repo's README.md for examples on how to use.
     """
 
-    def __init__(self, node, parent_node=None, raw_text: str = None):
+    def __init__(self, node, parent_node=None, raw_text: str = None, namespaces=None):
         """
         Constructor.
         :param node: A Python ElementTree (root) node to wrap
         :param parent_node: If this is not the root, this the parent ElementTree node
         :param raw_text:  Raw XML text string if you want to keep a copy
         """
         self.raw_text = raw_text
         self.node = node
+        self.namespaces = namespaces if namespaces is not None else {}
         self.case_insensitive_props = dict((k.lower(), k) for k in self.node.attrib)
         self.parent_node = parent_node
 
     def text(self) -> str:
         """Get the node's text (the string between the XML tags)."""
         return '' if self.node.text is None else self.node.text
 
     def tag(self) -> str:
         """Get the XML element tag from the node."""
-        return self.node.tag
+        return self._fixtag(self.node.tag)
 
     def get(self, item: str, default: str = None) -> str:
         """Get the given property from the node."""
         case_sensitive_item = self.case_insensitive_props.get(item.lower(), item)
         return self.node.attrib.get(case_sensitive_item, default)
 
     def __getitem__(self, item: Union[int, str]):
@@ -48,22 +49,40 @@
             return self.node.attrib[case_sensitive_item]
 
     def __contains__(self, item: str):
         case_sensitive_item = self.case_insensitive_props.get(item.lower(), item)
         return case_sensitive_item in self.node.attrib
 
     def __getattr__(self, attribute: str):
-        nodes = [n for n in self.node if n.tag.lower() == attribute.lower()]
+        nodes = [n for n in self.node if self._fixtag(n.tag).lower() == attribute.lower()]
         if len(nodes) == 1:
-            return XmlNode(node=nodes[0], parent_node=self.node)
+            return XmlNode(node=nodes[0], parent_node=self.node, namespaces=self.namespaces)
         if len(nodes) > 1:
-            return XmlNodeList([XmlNode(node=n, parent_node=self.node) for n in nodes])
+            return XmlNodeList([XmlNode(node=n, parent_node=self.node,
+                                        namespaces=self.namespaces) for n in nodes])
         raise AttributeError(f"'{self.node.tag}' object has no attribute '{attribute}'")
 
     def __len__(self):
         return 1
 
     def __repr__(self):
         return f"XmlNode: {self.tag()}"
 
     def __dir__(self):
-        return [n.tag for n in self.node]
+        return [self._fixtag(n.tag) for n in self.node]
+
+    def _fixtag(self, tag):
+        for ns_tag in self.namespaces:
+            full_tag = f"{{{ns_tag}}}"
+            if tag.startswith(full_tag):
+                prefix = self._ns_prefix(ns_tag)
+                return tag.replace(full_tag, prefix)
+        return tag
+
+    def _ns_prefix(self, ns):
+        if isinstance(self.namespaces, set):
+            return ''
+        else:
+            if self.namespaces[ns]:
+                return f"{self.namespaces[ns]}_"
+            else:
+                return ''
```

### Comparing `dunder_xml_reader-0.0.2/dunder_xml_reader/xml_node_list.py` & `dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node_list.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.2/dunder_xml_reader.egg-info/PKG-INFO` & `dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunder-xml-reader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -903,14 +903,55 @@
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
     >>> cxml = parse_xml(raw_xml_text)
     >>> print(cxml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
+### XML with namespaces ###
+
+The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
+this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+for example:
+
+    <?xml version="1.0" encoding="UTF-8"?>
+    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
+      <soapenv:Body>
+        <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
+          <ClaimResponse>
+            <status>S</status>
+            <errorDetail/>
+            <claimNumber>LC0000001742</claimNumber>
+          </ClaimResponse>
+        </ReceiveClaimResponse>
+      </soapenv:Body>
+    </soapenv:Envelope>
+
+Using the `namespaces` argument to `parse_xml()`, you can have the attributes prefixed with
+an alias:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/': 'soap',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job': 'claim'
+    ... }
+    >>> soap.soap_Body.claim_ReceiveClaimResponse.claim_ClaimResponse.claim_status.text()
+    S
+    >>>
+
+If you don't want any prefixes and you just want to strip out the namespace references you
+can either pass a `set` of namespace strings to `parse_xml()`:
+
+    >>> soap = parse_xml(raw_soap_text, namespaces={
+    ...   'http://schemas.xmlsoap.org/soap/envelope/',
+    ...   'http://insurance.com/webservices/ReceiveClaim.job'
+    ... }
+    >>> soap.Body.ReceiveClaimResponse.ClaimResponse.status.text()
+    S
+    >>>
+
 ## Bonus: SafeReference ##
 
 SafeReference is a wrapper that you can wrap a xmlNode instance in (or any other Python object
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
```

### Comparing `dunder_xml_reader-0.0.2/pyproject.toml` & `dunder_xml_reader-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dunder_xml_reader"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Steve Brettschneider", email="steve@bluehousefamily.com" },
 ]
 description = "Pythonic XML parsing/reading"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dunder_xml_reader-0.0.2/test/test_safe_reference.py` & `dunder_xml_reader-0.0.3/test/test_safe_reference.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.2/test/test_xml_node.py` & `dunder_xml_reader-0.0.3/test/test_xml_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -248,7 +248,59 @@
     # When
     result = conf_header.Notes.text()
 
     # Then
     assert result == ''
 
 
+def test_with_namespaces(sample_soap_text):
+    # Given
+    raw_text = sample_soap_text
+
+    # When
+    result = parse_xml(raw_text, namespaces={
+        'http://schemas.xmlsoap.org/soap/envelope/': 'soap',
+        'http://insurance.com/webservices/ReceiveClaim.job': 'claim'
+    })
+
+    # Then
+    assert result.raw_text is raw_text
+    assert result.tag() == 'soap_Envelope'
+    assert dir(result.soap_Body) == ['claim_ReceiveClaimResponse']
+    assert hasattr(result.soap_Body, 'claim_ReceiveClaimResponse')
+    assert result.soap_Body.claim_ReceiveClaimResponse.claim_ClaimResponse.claim_status.text() == 'S'
+
+
+def test_with_blanked_namespaces(sample_soap_text):
+    # Given
+    raw_text = sample_soap_text
+
+    # When
+    result = parse_xml(raw_text, namespaces={
+        'http://schemas.xmlsoap.org/soap/envelope/',
+        'http://insurance.com/webservices/ReceiveClaim.job'
+    })
+
+    # Then
+    assert result.raw_text is raw_text
+    assert result.tag() == 'Envelope'
+    assert dir(result.Body) == ['ReceiveClaimResponse']
+    assert hasattr(result.Body, 'ReceiveClaimResponse')
+    assert result.Body.ReceiveClaimResponse.ClaimResponse.status.text() == 'S'
+
+
+def test_with_some_blanked_namespaces(sample_soap_text):
+    # Given
+    raw_text = sample_soap_text
+
+    # When
+    result = parse_xml(raw_text, namespaces={
+        'http://schemas.xmlsoap.org/soap/envelope/': 'soap',
+        'http://insurance.com/webservices/ReceiveClaim.job': None
+    })
+
+    # Then
+    assert result.raw_text is raw_text
+    assert result.tag() == 'soap_Envelope'
+    assert dir(result.soap_Body) == ['ReceiveClaimResponse']
+    assert hasattr(result.soap_Body, 'ReceiveClaimResponse')
+    assert result.soap_Body.ReceiveClaimResponse.ClaimResponse.status.text() == 'S'
```

### Comparing `dunder_xml_reader-0.0.2/test/test_xml_node_list.py` & `dunder_xml_reader-0.0.3/test/test_xml_node_list.py`

 * *Files identical despite different names*

