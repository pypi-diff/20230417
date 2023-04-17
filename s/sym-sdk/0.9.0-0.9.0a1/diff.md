# Comparing `tmp/sym-sdk-0.9.0.tar.gz` & `tmp/sym-sdk-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym-sdk-0.9.0.tar", max compression
+gzip compressed data, was "sym-sdk-0.9.0a1.tar", max compression
```

## Comparing `sym-sdk-0.9.0.tar` & `sym-sdk-0.9.0a1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     1660 2022-04-28 14:38:47.028565 sym-sdk-0.9.0/DESCRIPTION.rst
--rw-r--r--   0        0        0      150 2022-04-28 14:38:47.028565 sym-sdk-0.9.0/LICENSE
--rw-r--r--   0        0        0     1734 2022-04-28 14:39:52.753270 sym-sdk-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      874 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/__init__.py
--rw-r--r--   0        0        0      162 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/annotations/__init__.py
--rw-r--r--   0        0        0      611 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/annotations/_handlers.py
--rw-r--r--   0        0        0     2887 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/errors.py
--rw-r--r--   0        0        0     4235 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/event.py
--rw-r--r--   0        0        0      481 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      565 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/access_strategy.py
--rw-r--r--   0        0        0      890 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/aws.py
--rw-r--r--   0        0        0     1680 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/identity.py
--rw-r--r--   0        0        0      470 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/slack.py
--rw-r--r--   0        0        0     1428 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/exceptions/sym_exception.py
--rw-r--r--   0        0        0     2352 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/flow.py
--rw-r--r--   0        0        0      103 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/__init__.py
--rw-r--r--   0        0        0      850 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/aws_lambda.py
--rw-r--r--   0        0        0     2347 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/github.py
--rw-r--r--   0        0        0     1765 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/okta.py
--rw-r--r--   0        0        0     2709 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/pagerduty.py
--rw-r--r--   0        0        0     2480 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/slack.py
--rw-r--r--   0        0        0     1197 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/integrations/store.py
--rw-r--r--   0        0        0      231 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/models.py
--rw-r--r--   0        0        0    11566 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/resource.py
--rw-r--r--   0        0        0      222 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/strategies/__init__.py
--rw-r--r--   0        0        0     9930 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/strategies/access_strategy.py
--rw-r--r--   0        0        0     1595 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/strategies/integration.py
--rw-r--r--   0        0        0      920 2022-04-28 14:38:47.032565 sym-sdk-0.9.0/sym/sdk/target.py
--rw-r--r--   0        0        0      331 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/templates/__init__.py
--rw-r--r--   0        0        0     7081 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/templates/approval.py
--rw-r--r--   0        0        0     1272 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/templates/step.py
--rw-r--r--   0        0        0     1418 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/templates/template.py
--rw-r--r--   0        0        0        0 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/annotations/__init__.py
--rw-r--r--   0        0        0      290 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/annotations/test_reducer.py
--rw-r--r--   0        0        0        0 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/integrations/__init__.py
--rw-r--r--   0        0        0     1130 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/integrations/test_pagerduty_interface.py
--rw-r--r--   0        0        0        0 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/static/__init__.py
--rw-r--r--   0        0        0     3072 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/static/approvers_test_code.py
--rw-r--r--   0        0        0      376 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/test_flow.py
--rw-r--r--   0        0        0     3588 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/test_resource.py
--rw-r--r--   0        0        0      255 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/test_target.py
--rw-r--r--   0        0        0      379 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/tests/test_templates.py
--rw-r--r--   0        0        0     3251 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/user.py
--rw-r--r--   0        0        0      124 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/utils/__init__.py
--rw-r--r--   0        0        0     1124 2022-04-28 14:38:47.036565 sym-sdk-0.9.0/sym/sdk/utils/user.py
--rw-r--r--   0        0        0       22 2022-04-28 14:39:52.813271 sym-sdk-0.9.0/sym/sdk/version.py
--rw-r--r--   0        0        0     2674 2022-04-28 14:39:53.543323 sym-sdk-0.9.0/setup.py
--rw-r--r--   0        0        0     2376 2022-04-28 14:39:53.543733 sym-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1660 2022-04-19 21:18:13.515767 sym-sdk-0.9.0a1/DESCRIPTION.rst
+-rw-r--r--   0        0        0      150 2022-04-19 21:18:13.515767 sym-sdk-0.9.0a1/LICENSE
+-rw-r--r--   0        0        0     1742 2022-04-19 21:19:28.792075 sym-sdk-0.9.0a1/pyproject.toml
+-rw-r--r--   0        0        0      874 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/__init__.py
+-rw-r--r--   0        0        0      162 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/annotations/__init__.py
+-rw-r--r--   0        0        0      611 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/annotations/_handlers.py
+-rw-r--r--   0        0        0     2887 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/errors.py
+-rw-r--r--   0        0        0     4235 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/event.py
+-rw-r--r--   0        0        0      481 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      565 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/access_strategy.py
+-rw-r--r--   0        0        0      890 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/aws.py
+-rw-r--r--   0        0        0     1680 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/identity.py
+-rw-r--r--   0        0        0      470 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/slack.py
+-rw-r--r--   0        0        0     1428 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/exceptions/sym_exception.py
+-rw-r--r--   0        0        0     2352 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/flow.py
+-rw-r--r--   0        0        0      103 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/__init__.py
+-rw-r--r--   0        0        0      850 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/aws_lambda.py
+-rw-r--r--   0        0        0     2336 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/github.py
+-rw-r--r--   0        0        0     1696 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/http.py
+-rw-r--r--   0        0        0     1765 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/okta.py
+-rw-r--r--   0        0        0     2709 2022-04-19 21:18:13.519767 sym-sdk-0.9.0a1/sym/sdk/integrations/pagerduty.py
+-rw-r--r--   0        0        0     2480 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/integrations/slack.py
+-rw-r--r--   0        0        0     1197 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/integrations/store.py
+-rw-r--r--   0        0        0      231 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/models.py
+-rw-r--r--   0        0        0    11143 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/resource.py
+-rw-r--r--   0        0        0     1726 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/secret.py
+-rw-r--r--   0        0        0      222 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/strategies/__init__.py
+-rw-r--r--   0        0        0     9975 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/strategies/access_strategy.py
+-rw-r--r--   0        0        0     1587 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/strategies/integration.py
+-rw-r--r--   0        0        0      920 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/target.py
+-rw-r--r--   0        0        0      331 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/templates/__init__.py
+-rw-r--r--   0        0        0     7081 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/templates/approval.py
+-rw-r--r--   0        0        0     1272 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/templates/step.py
+-rw-r--r--   0        0        0     1418 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/templates/template.py
+-rw-r--r--   0        0        0        0 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/annotations/__init__.py
+-rw-r--r--   0        0        0      290 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/annotations/test_reducer.py
+-rw-r--r--   0        0        0        0 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/integrations/__init__.py
+-rw-r--r--   0        0        0     1130 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/integrations/test_pagerduty_interface.py
+-rw-r--r--   0        0        0        0 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/static/__init__.py
+-rw-r--r--   0        0        0     3072 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/static/approvers_test_code.py
+-rw-r--r--   0        0        0      376 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/test_flow.py
+-rw-r--r--   0        0        0     2550 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/test_resource.py
+-rw-r--r--   0        0        0      255 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/test_target.py
+-rw-r--r--   0        0        0      379 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/tests/test_templates.py
+-rw-r--r--   0        0        0     3252 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/user.py
+-rw-r--r--   0        0        0      124 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1124 2022-04-19 21:18:13.523767 sym-sdk-0.9.0a1/sym/sdk/utils/user.py
+-rw-r--r--   0        0        0       30 2022-04-19 21:19:28.868077 sym-sdk-0.9.0a1/sym/sdk/version.py
+-rw-r--r--   0        0        0     2676 2022-04-19 21:19:29.571845 sym-sdk-0.9.0a1/setup.py
+-rw-r--r--   0        0        0     2378 2022-04-19 21:19:29.572196 sym-sdk-0.9.0a1/PKG-INFO
```

### Comparing `sym-sdk-0.9.0/DESCRIPTION.rst` & `sym-sdk-0.9.0a1/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/pyproject.toml` & `sym-sdk-0.9.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-sdk"
-version = "0.9.0"
+version = "0.9.0-alpha.1"
 description = "Sym's Python SDK"
 authors = ["Sym Engineering <pypi@symops.io>"]
 license = "Proprietary"
 readme = "DESCRIPTION.rst"
 homepage = "https://sdk.docs.symops.com/"
 repository = "https://github.com/symopsio/sym-sdk"
 classifiers=[
```

### Comparing `sym-sdk-0.9.0/sym/sdk/__init__.py` & `sym-sdk-0.9.0a1/sym/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/annotations/_handlers.py` & `sym-sdk-0.9.0a1/sym/sdk/annotations/_handlers.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/errors.py` & `sym-sdk-0.9.0a1/sym/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/event.py` & `sym-sdk-0.9.0a1/sym/sdk/event.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/exceptions/access_strategy.py` & `sym-sdk-0.9.0a1/sym/sdk/exceptions/access_strategy.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/exceptions/aws.py` & `sym-sdk-0.9.0a1/sym/sdk/exceptions/aws.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/exceptions/identity.py` & `sym-sdk-0.9.0a1/sym/sdk/exceptions/identity.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/exceptions/sym_exception.py` & `sym-sdk-0.9.0a1/sym/sdk/exceptions/sym_exception.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/flow.py` & `sym-sdk-0.9.0a1/sym/sdk/flow.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/aws_lambda.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/github.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,10 +44,10 @@
 
     Args:
         repo_name: The name, not including organization, of the repository to get the collaborators
             of
         roles: A set of one or more roles on which to filter collaborators.
 
     Returns:
-        A list of :class:`Users <sym.sdk.user.User>` corresponding to collaborators with the specified role(s)
+        A list of :class:`~sym.sdk.User`s corresponding to collaborators with the specified role(s)
         of the specified repository.
     """
```

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/okta.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/okta.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/pagerduty.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/pagerduty.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/slack.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/slack.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/integrations/store.py` & `sym-sdk-0.9.0a1/sym/sdk/integrations/store.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/resource.py` & `sym-sdk-0.9.0a1/sym/sdk/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,15 @@
     def __str__(self) -> str:
         return json.dumps(self.dict(), indent=2)
 
     def __repr__(self) -> str:
         return str(self)
 
     def dict(self):
+        """Represent this resource as a dictionary."""
         return {
             k: v.dict() if isinstance(v, SymBaseResource) else v
             for k in dir(self)
             if not k.startswith("_")
             and isinstance((v := getattr(self, k)), (SymBaseResource, str, int, dict, list))
         }
 
@@ -316,23 +317,14 @@
     Read more about `Sym Resources <https://docs.symops.com/docs/sym-concepts>`_.
     """
 
     def __init__(self, srn: Union[SRN, str]):
         self._srn = SRN.parse(str(srn))
 
     def __getattr__(self, name: str):
-        """__getattr__ is called as a last resort if there are no attributes on the
-        instance that match the name.
-
-        This override allows attributes of the SRN to be called as attributes directly\
-        on the resource without needing to define them.
-        """
-        if name in {"srn", "_srn"}:
-            # Raise if we've failed to find SRN, otherwise we'll infinitely recurse.
-            raise AttributeError(f"no attribute '{name}'")
         return getattr(self.srn, name)
 
     def __eq__(self, other):
         if not isinstance(other, SymResource):
             return False
         return self.srn == other.srn
 
@@ -347,11 +339,9 @@
         """A :class:`~sym.sdk.resource.SRN` object that represents the unique identifier
         for this resource.
         """
         return self._srn
 
     @property
     def name(self) -> str:
-        """An alias for this resource's slug, represented by its
-        :class:`~sym.sdk.resource.SRN`.
-        """
+        """An alias for this resource's slug, derived from its :class:`~sym.sdk.resource.SRN`."""
         return self.srn.slug
```

### Comparing `sym-sdk-0.9.0/sym/sdk/strategies/access_strategy.py` & `sym-sdk-0.9.0a1/sym/sdk/strategies/access_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from abc import ABC, abstractmethod
-from typing import Optional, final
+from typing import TYPE_CHECKING, Optional, final
 
 from sym.sdk.event import Event
 from sym.sdk.exceptions.identity import IdentityNotFound
 from sym.sdk.user import User
 from sym.sdk.utils import persist_user_identity
 
-from .integration import Integration
+if TYPE_CHECKING:
+    from sym.sdk.strategies import Integration
 
 
 class AccessStrategy(ABC):
     """A standardized interface that allows Implementers to define custom Strategies, enabling Sym
     to perform escalations and de-escalations against almost any Internet-accessible service."""
 
     @final
-    def __init__(self, integration: Integration):
+    def __init__(self, integration: "Integration"):
         self.integration = integration
 
     @final
     def get_requester_identity(self, event: Event) -> str:
         """Retrieves the external identity of the user who initiated the request represented by the
         ``event`` parameter; first from stored user information, then by calling
         :func:`~sym.sdk.strategies.access_strategy.AccessStrategy.fetch_remote_identity` as needed.
```

### Comparing `sym-sdk-0.9.0/sym/sdk/strategies/integration.py` & `sym-sdk-0.9.0a1/sym/sdk/strategies/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict
 
-from sym.sdk.resource import SymBaseResource
+from sym.sdk.resource import SymResource
 
 
-class Integration(ABC, SymBaseResource):
+class Integration(ABC, SymResource):
     """Represents an Integration (service-specific config and state) in the Sym SDK.
 
     For the purposes of the SDK, Integrations can be thought of as the "state" of a Strategy. Or, to
     put it another way, if a Strategy tells Sym how to interact with an external service to perform
     escalations, the Integration is the service-specific state Sym maintains, including the identity
     mappings of Sym users to the external service."""
```

### Comparing `sym-sdk-0.9.0/sym/sdk/target.py` & `sym-sdk-0.9.0a1/sym/sdk/target.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/templates/approval.py` & `sym-sdk-0.9.0a1/sym/sdk/templates/approval.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/templates/step.py` & `sym-sdk-0.9.0a1/sym/sdk/templates/step.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/templates/template.py` & `sym-sdk-0.9.0a1/sym/sdk/templates/template.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/tests/integrations/test_pagerduty_interface.py` & `sym-sdk-0.9.0a1/sym/sdk/tests/integrations/test_pagerduty_interface.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/tests/static/approvers_test_code.py` & `sym-sdk-0.9.0a1/sym/sdk/tests/static/approvers_test_code.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/sym/sdk/tests/test_resource.py` & `sym-sdk-0.9.0a1/sym/sdk/tests/test_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import pytest
 
 from sym.sdk.resource import (
     SRN,
     InvalidSlugError,
     InvalidSRNError,
     MultipleErrors,
-    SymResource,
     TrailingSeparatorError,
 )
 
 
-class MockSymResource(SymResource):
-    """This is a test class for SymResource behavior."""
-
-
 class TestResource:
     def test_sym_resource_fails_on_malformed_srn(self):
         self._test_bad("foo", InvalidSRNError)
         self._test_bad("foo:bar", InvalidSRNError)
         self._test_bad("foo:bar:baz", InvalidSRNError)
         self._test_bad("foo:bar:baz:boz", InvalidSRNError)
         self._test_bad("foo:bar:baz:lates:", TrailingSeparatorError, match="trailing separator.")
@@ -65,30 +60,7 @@
 
         srn_str = str(srn)
         srn2 = SRN.parse(srn_str)
 
         assert srn == srn2
         assert str(srn) == str(srn2)
         assert text == srn_str
-
-    def test_sym_resource_srn_getattr_fallback(self):
-        srn = SRN.parse("test:mock:slug:latest:12345")
-        resource = MockSymResource(srn=srn)
-
-        assert resource.srn == srn
-        assert resource.name == srn.slug
-        assert resource.organization == srn.organization
-        assert resource.identifier == srn.identifier
-
-    def test_sym_resource_srn_getattr_errors(self):
-        srn = SRN.parse("test:mock:slug:latest:12345")
-        resource = MockSymResource(srn=srn)
-
-        # Ensure a normal missing attribute errors properly.
-        with pytest.raises(AttributeError, match="no attribute 'nope'"):
-            resource.nope
-
-        # Delete the attributes so the __getattr__ override should fall back,
-        # but we want to ensure it doesn't infinitely recurse.
-        delattr(resource, "_srn")
-        with pytest.raises(AttributeError, match="no attribute 'srn"):
-            resource.srn
```

### Comparing `sym-sdk-0.9.0/sym/sdk/user.py` & `sym-sdk-0.9.0a1/sym/sdk/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     @property
     @abstractmethod
     def identities(self) -> Dict[str, List[UserIdentity]]:
         """Retrieves the set of identities associated with this
         :class:`~sym.sdk.user.User`, grouped by service type.
 
-        A mapping of service types to lists of :class:`~sym.sdk.user.UserIdentity`.
+        A mapping of service types to lists of :class:`~sym.sdk.user.UserIdentity`s.
         """
 
     @abstractmethod
     def identity(
         self,
         service_type: str,
         service_id: Optional[str] = None,
```

### Comparing `sym-sdk-0.9.0/sym/sdk/utils/user.py` & `sym-sdk-0.9.0a1/sym/sdk/utils/user.py`

 * *Files identical despite different names*

### Comparing `sym-sdk-0.9.0/setup.py` & `sym-sdk-0.9.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'pydantic>=1.7.3,<2.0.0',
  'requests>=2.25.1,<3.0.0',
  'structlog==21.5.0',
  'virtualenv>=20.4.7,<21.0.0']
 
 setup_kwargs = {
     'name': 'sym-sdk',
-    'version': '0.9.0',
+    'version': '0.9.0a1',
     'description': "Sym's Python SDK",
     'long_description': 'Sym Python SDK\n================\n\n`Sym <https://symops.com/>`_ is the security workflow platform made for engineers, by engineers.\n\nWe solve the intent-to-execution gap between policies and workflows by providing fast-moving engineering teams with the just-right primitives to roll out best-practice controls.\n\nThis is the Python SDK for Sym.\nFor guides and other help, check out our `main docs site <https://docs.symops.com/>`_.\n\nThe SDK docs are broken into several core modules, which are described below.\nClick on one to see the classes and functions available in your `Handlers <https://docs.symops.com/docs/handlers>`_.\n\nThe Sym SDK is used to customize workflow templates that are exposed by our `Terraform provider <https://docs.symops.com/docs/terraform-provider>`_. Here\'s an example using the ``sym:approve`` Template!\n\n.. code-block:: python\n\n   from sym.sdk.annotations import reducer\n   from sym.sdk.integrations import pagerduty, okta, slack\n\n   @reducer\n   def get_approvers(evt):\n      # The import here uses credentials defined in an Integration in Terraform\n      if pagerduty.is_on_call(evt.user, schedule="id_of_eng_on_call"):\n         # This is a self-approval in a DM\n         return slack.user(evt.user)\n\n      if evt.payload.fields["urgency"] == "Emergency":\n         # This is a self-approval in a channel\n         return slack.channel("#break-glass", allow_self=True)\n\n      on_call_mgrs = okta.group("OnCallManagers").members()\n      # This would cause each on-call manager to be DMed\n      return slack.group([slack.user(x) for x in on_call_mgrs])\n\nIf you\'re interested in using Sym, please `reach out <https://symops.com/sales>`_!\n',
     'author': 'Sym Engineering',
     'author_email': 'pypi@symops.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://sdk.docs.symops.com/',
```

### Comparing `sym-sdk-0.9.0/PKG-INFO` & `sym-sdk-0.9.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-sdk
-Version: 0.9.0
+Version: 0.9.0a1
 Summary: Sym's Python SDK
 Home-page: https://sdk.docs.symops.com/
 License: Proprietary
 Author: Sym Engineering
 Author-email: pypi@symops.io
 Requires-Python: >=3.8.6,<4.0.0
 Classifier: License :: Other/Proprietary License
```

