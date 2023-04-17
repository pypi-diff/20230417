# Comparing `tmp/uzcloud-billing-0.2.8.tar.gz` & `tmp/uzcloud-billing-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uzcloud-billing-0.2.8.tar", last modified: Fri Oct  7 06:37:41 2022, max compression
+gzip compressed data, was "uzcloud-billing-0.2.9.tar", last modified: Tue Dec 20 10:16:13 2022, max compression
```

## Comparing `uzcloud-billing-0.2.8.tar` & `uzcloud-billing-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.544028 uzcloud-billing-0.2.8/
--rw-rw-rw-   0        0        0      661 2022-07-21 12:56:43.000000 uzcloud-billing-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       35 2022-07-21 12:56:49.000000 uzcloud-billing-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1941 2022-10-07 06:37:41.544028 uzcloud-billing-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2022-07-25 06:44:08.000000 uzcloud-billing-0.2.8/README.rst
--rw-rw-rw-   0        0        0      110 2022-07-21 15:24:56.000000 uzcloud-billing-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0      808 2022-10-07 06:37:41.552042 uzcloud-billing-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      111 2022-07-21 18:25:18.000000 uzcloud-billing-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.495805 uzcloud-billing-0.2.8/uzcloud_billing/
--rw-rw-rw-   0        0        0        0 2022-07-21 14:24:22.000000 uzcloud-billing-0.2.8/uzcloud_billing/__init__.py
--rw-rw-rw-   0        0        0      274 2022-08-22 12:26:12.000000 uzcloud-billing-0.2.8/uzcloud_billing/admin.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.540039 uzcloud-billing-0.2.8/uzcloud_billing/api/
--rw-rw-rw-   0        0        0        0 2022-07-21 10:58:46.000000 uzcloud-billing-0.2.8/uzcloud_billing/api/__init__.py
--rw-rw-rw-   0        0        0      230 2022-07-25 10:02:59.000000 uzcloud-billing-0.2.8/uzcloud_billing/api/permissions.py
--rw-rw-rw-   0        0        0     1130 2022-07-25 06:14:41.000000 uzcloud-billing-0.2.8/uzcloud_billing/api/serializers.py
--rw-rw-rw-   0        0        0     1855 2022-08-22 12:38:09.000000 uzcloud-billing-0.2.8/uzcloud_billing/api/views.py
--rw-rw-rw-   0        0        0      246 2022-07-21 14:29:09.000000 uzcloud-billing-0.2.8/uzcloud_billing/apps.py
--rw-rw-rw-   0        0        0      561 2022-07-22 04:12:24.000000 uzcloud-billing-0.2.8/uzcloud_billing/decorators.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.541067 uzcloud-billing-0.2.8/uzcloud_billing/management/
--rw-rw-rw-   0        0        0        0 2022-07-25 04:30:24.000000 uzcloud-billing-0.2.8/uzcloud_billing/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.544028 uzcloud-billing-0.2.8/uzcloud_billing/management/commands/
--rw-rw-rw-   0        0        0        0 2022-07-25 04:30:24.000000 uzcloud-billing-0.2.8/uzcloud_billing/management/commands/__init__.py
--rw-rw-rw-   0        0        0      977 2022-07-25 07:28:15.000000 uzcloud-billing-0.2.8/uzcloud_billing/management/commands/create_billing_accounts.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.544028 uzcloud-billing-0.2.8/uzcloud_billing/migrations/
--rw-rw-rw-   0        0        0      917 2022-07-21 14:27:48.000000 uzcloud-billing-0.2.8/uzcloud_billing/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      440 2022-07-22 11:15:09.000000 uzcloud-billing-0.2.8/uzcloud_billing/migrations/0002_billingaccount_balance.py
--rw-rw-rw-   0        0        0        0 2022-07-21 14:24:22.000000 uzcloud-billing-0.2.8/uzcloud_billing/migrations/__init__.py
--rw-rw-rw-   0        0        0      597 2022-08-22 12:25:26.000000 uzcloud-billing-0.2.8/uzcloud_billing/models.py
--rw-rw-rw-   0        0        0      402 2022-07-26 12:15:00.000000 uzcloud-billing-0.2.8/uzcloud_billing/receivers.py
--rw-rw-rw-   0        0        0      983 2022-10-07 06:29:41.000000 uzcloud-billing-0.2.8/uzcloud_billing/services.py
--rw-rw-rw-   0        0        0      109 2022-07-26 11:15:14.000000 uzcloud-billing-0.2.8/uzcloud_billing/signals.py
--rw-rw-rw-   0        0        0      261 2022-07-21 13:57:24.000000 uzcloud-billing-0.2.8/uzcloud_billing/urls.py
--rw-rw-rw-   0        0        0     3317 2022-10-07 06:36:50.000000 uzcloud-billing-0.2.8/uzcloud_billing/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-07 06:37:41.527967 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/
--rw-rw-rw-   0        0        0     1941 2022-10-07 06:37:41.000000 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      945 2022-10-07 06:37:41.000000 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-07 06:37:41.000000 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2022-10-07 06:37:41.000000 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-10-07 06:37:41.000000 uzcloud-billing-0.2.8/uzcloud_billing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.202632 uzcloud-billing-0.2.9/
+-rw-rw-rw-   0        0        0      661 2022-07-21 12:56:43.000000 uzcloud-billing-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-07-21 12:56:49.000000 uzcloud-billing-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1941 2022-12-20 10:16:13.202632 uzcloud-billing-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2022-07-25 06:44:08.000000 uzcloud-billing-0.2.9/README.rst
+-rw-rw-rw-   0        0        0      110 2022-07-21 15:24:56.000000 uzcloud-billing-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0      808 2022-12-20 10:16:13.210648 uzcloud-billing-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      111 2022-07-21 18:25:18.000000 uzcloud-billing-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.155802 uzcloud-billing-0.2.9/uzcloud_billing/
+-rw-rw-rw-   0        0        0        0 2022-07-21 14:24:22.000000 uzcloud-billing-0.2.9/uzcloud_billing/__init__.py
+-rw-rw-rw-   0        0        0      463 2022-12-20 10:12:15.000000 uzcloud-billing-0.2.9/uzcloud_billing/admin.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.187415 uzcloud-billing-0.2.9/uzcloud_billing/api/
+-rw-rw-rw-   0        0        0        0 2022-07-21 10:58:46.000000 uzcloud-billing-0.2.9/uzcloud_billing/api/__init__.py
+-rw-rw-rw-   0        0        0      230 2022-07-25 10:02:59.000000 uzcloud-billing-0.2.9/uzcloud_billing/api/permissions.py
+-rw-rw-rw-   0        0        0     1130 2022-07-25 06:14:41.000000 uzcloud-billing-0.2.9/uzcloud_billing/api/serializers.py
+-rw-rw-rw-   0        0        0     1855 2022-08-22 12:38:09.000000 uzcloud-billing-0.2.9/uzcloud_billing/api/views.py
+-rw-rw-rw-   0        0        0      169 2022-12-20 09:49:15.000000 uzcloud-billing-0.2.9/uzcloud_billing/apps.py
+-rw-rw-rw-   0        0        0      561 2022-07-22 04:12:24.000000 uzcloud-billing-0.2.9/uzcloud_billing/decorators.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.195212 uzcloud-billing-0.2.9/uzcloud_billing/management/
+-rw-rw-rw-   0        0        0        0 2022-07-25 04:30:24.000000 uzcloud-billing-0.2.9/uzcloud_billing/management/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.196258 uzcloud-billing-0.2.9/uzcloud_billing/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-07-25 04:30:24.000000 uzcloud-billing-0.2.9/uzcloud_billing/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      977 2022-07-25 07:28:15.000000 uzcloud-billing-0.2.9/uzcloud_billing/management/commands/create_billing_accounts.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.202632 uzcloud-billing-0.2.9/uzcloud_billing/migrations/
+-rw-rw-rw-   0        0        0      917 2022-12-20 09:47:46.000000 uzcloud-billing-0.2.9/uzcloud_billing/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      440 2022-07-22 11:15:09.000000 uzcloud-billing-0.2.9/uzcloud_billing/migrations/0002_billingaccount_balance.py
+-rw-rw-rw-   0        0        0      665 2022-12-20 09:49:48.000000 uzcloud-billing-0.2.9/uzcloud_billing/migrations/0003_billingaccount_account_type_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-07-21 14:24:22.000000 uzcloud-billing-0.2.9/uzcloud_billing/migrations/__init__.py
+-rw-rw-rw-   0        0        0      734 2022-12-20 09:50:19.000000 uzcloud-billing-0.2.9/uzcloud_billing/models.py
+-rw-rw-rw-   0        0        0     1224 2022-12-20 10:05:59.000000 uzcloud-billing-0.2.9/uzcloud_billing/services.py
+-rw-rw-rw-   0        0        0      109 2022-07-26 11:15:14.000000 uzcloud-billing-0.2.9/uzcloud_billing/signals.py
+-rw-rw-rw-   0        0        0      261 2022-07-21 13:57:24.000000 uzcloud-billing-0.2.9/uzcloud_billing/urls.py
+-rw-rw-rw-   0        0        0     3389 2022-12-20 09:48:05.000000 uzcloud-billing-0.2.9/uzcloud_billing/utils.py
+drwxrwxrwx   0        0        0        0 2022-12-20 10:16:13.187415 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/
+-rw-rw-rw-   0        0        0     1941 2022-12-20 10:16:13.000000 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      988 2022-12-20 10:16:13.000000 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-20 10:16:13.000000 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2022-12-20 10:16:13.000000 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-12-20 10:16:13.000000 uzcloud-billing-0.2.9/uzcloud_billing.egg-info/top_level.txt
```

### Comparing `uzcloud-billing-0.2.8/LICENSE` & `uzcloud-billing-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/PKG-INFO` & `uzcloud-billing-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uzcloud-billing
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uzcloud Billing
 Home-page: https://arabboy3332@bitbucket.org/arabboy3332/uzcloud_billing.git
 Author: Arabboy Mamadaliev
 Author-email: mr.arabboy@gmail.com
 License: MIT
 Keywords: uzcloud,billing
 Platform: UNKNOWN
```

### Comparing `uzcloud-billing-0.2.8/README.rst` & `uzcloud-billing-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/setup.cfg` & `uzcloud-billing-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 7a63 6c6f 7564 2d62 696c 6c69   = uzcloud-billi
 00000020: 6e67 0d0a 7665 7273 696f 6e20 3d20 302e  ng..version = 0.
-00000030: 322e 380d 0a61 7574 686f 7220 3d20 4172  2.8..author = Ar
+00000030: 322e 390d 0a61 7574 686f 7220 3d20 4172  2.9..author = Ar
 00000040: 6162 626f 7920 4d61 6d61 6461 6c69 6576  abboy Mamadaliev
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 206d 722e 6172 6162 626f 7940 676d 6169   mr.arabboy@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2055 7a63 6c6f 7564 2042 696c  on = Uzcloud Bil
 00000090: 6c69 6e67 0d0a 6c6f 6e67 5f64 6573 6372  ling..long_descr
 000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
```

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/api/serializers.py` & `uzcloud-billing-0.2.9/uzcloud_billing/api/serializers.py`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/api/views.py` & `uzcloud-billing-0.2.9/uzcloud_billing/api/views.py`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/decorators.py` & `uzcloud-billing-0.2.9/uzcloud_billing/decorators.py`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/management/commands/create_billing_accounts.py` & `uzcloud-billing-0.2.9/uzcloud_billing/management/commands/create_billing_accounts.py`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/migrations/0001_initial.py` & `uzcloud-billing-0.2.9/uzcloud_billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/models.py` & `uzcloud-billing-0.2.9/uzcloud_billing/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from django.db import models
 from django.conf import settings
 
-from uzcloud_billing.utils import generate_account_number
-
 
 class BillingAccount(models.Model):
+    class AccountTypes(models.IntegerChoices):
+        INDIVIDUAL = 1, "Individual"
+        ORGANIZATION = 2, "Organization"
+
     user = models.OneToOneField(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         related_name="billing_account",
     )
-    account_number = models.CharField(
-        max_length=255, default=generate_account_number, unique=True
+    account_number = models.CharField(max_length=255, unique=True)
+    account_type = models.IntegerField(
+        choices=AccountTypes.choices, default=AccountTypes.INDIVIDUAL
     )
-
     balance = models.DecimalField(max_digits=10, decimal_places=2, default=0)
 
     def __str__(self):
         return f"{self.user} - {self.account_number}"
```

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/services.py` & `uzcloud-billing-0.2.9/uzcloud_billing/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import uzcloud_billing.utils as utils
-import uzcloud_billing.models as models
+from uzcloud_billing.models import BillingAccount
 from uzcloud_billing.signals import payment_completed_signal
 
 
+def create_billing_account(*, user, personType=1):
+    return BillingAccount.objects.create(
+        user=user,
+        account_number=utils.generate_account_number(personType=personType),
+        account_type=personType,
+    )
+
+
 def update_account_balance(*, account_number: str, balance: float):
-    billing_account = models.BillingAccount.objects.get(account_number=account_number)
+    billing_account = BillingAccount.objects.get(account_number=account_number)
     billing_account.balance = balance
     billing_account.save()
 
 
 def make_invoice(account_number: str, amount: float, reason: str, data: dict):
     """
     Eaxample Response :
```

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing/utils.py` & `uzcloud-billing-0.2.9/uzcloud_billing/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,28 +40,28 @@
         )
         if response.status_code != 200:
             raise ValueError(response.content)
         self.AUTH_TOKEN = response.json()["access_token"]
         self.DECODED = jwt.decode(self.AUTH_TOKEN, options={"verify_signature": False})
 
     @auth_required
-    def add_account(self):
-        payload = {"personType": 1}
+    def add_account(self, personType: int = 1):
+        payload = {"personType": personType}
         response = requests.post(
             url=self.ADD_ACCOUNT_URL,
             data=json.dumps(payload),
             headers=self.get_headers(),
             **self.REQUEST_CONFIG,
         )
         if response.status_code != 200:
             raise ValueError(response.content)
         return response.json()
 
     @auth_required
-    def get_balance(self, account_number):
+    def get_balance(self, account_number: str):
         response = requests.get(
             url=self.GET_BALANCE_URL,
             params={"accountNumber": account_number},
             headers=self.get_headers(),
             **self.REQUEST_CONFIG,
         )
         if response.status_code != 200:
@@ -96,10 +96,10 @@
             "Content-Type": "application/json",
         }
 
 
 uzcloud_service = UzcloudBilling()
 
 
-def generate_account_number():
-    account = uzcloud_service.add_account()
-    return account["AccountNumber"]
+def generate_account_number(personType=1):
+    account = uzcloud_service.add_account(personType=personType)
+    return account.get("AccountNumber")
```

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing.egg-info/PKG-INFO` & `uzcloud-billing-0.2.9/uzcloud_billing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uzcloud-billing
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uzcloud Billing
 Home-page: https://arabboy3332@bitbucket.org/arabboy3332/uzcloud_billing.git
 Author: Arabboy Mamadaliev
 Author-email: mr.arabboy@gmail.com
 License: MIT
 Keywords: uzcloud,billing
 Platform: UNKNOWN
```

### Comparing `uzcloud-billing-0.2.8/uzcloud_billing.egg-info/SOURCES.txt` & `uzcloud-billing-0.2.9/uzcloud_billing.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.cfg
 setup.py
 uzcloud_billing/__init__.py
 uzcloud_billing/admin.py
 uzcloud_billing/apps.py
 uzcloud_billing/decorators.py
 uzcloud_billing/models.py
-uzcloud_billing/receivers.py
 uzcloud_billing/services.py
 uzcloud_billing/signals.py
 uzcloud_billing/urls.py
 uzcloud_billing/utils.py
 uzcloud_billing.egg-info/PKG-INFO
 uzcloud_billing.egg-info/SOURCES.txt
 uzcloud_billing.egg-info/dependency_links.txt
@@ -24,8 +23,9 @@
 uzcloud_billing/api/serializers.py
 uzcloud_billing/api/views.py
 uzcloud_billing/management/__init__.py
 uzcloud_billing/management/commands/__init__.py
 uzcloud_billing/management/commands/create_billing_accounts.py
 uzcloud_billing/migrations/0001_initial.py
 uzcloud_billing/migrations/0002_billingaccount_balance.py
+uzcloud_billing/migrations/0003_billingaccount_account_type_and_more.py
 uzcloud_billing/migrations/__init__.py
```

