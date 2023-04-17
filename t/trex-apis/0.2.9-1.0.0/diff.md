# Comparing `tmp/trex-apis-0.2.9.tar.gz` & `tmp/trex-apis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-0.2.9.tar", last modified: Fri Mar  3 04:50:47 2023, max compression
+gzip compressed data, was "trex-apis-1.0.0.tar", last modified: Mon Apr 17 03:30:13 2023, max compression
```

## Comparing `trex-apis-0.2.9.tar` & `trex-apis-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.898113 trex-apis-0.2.9/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-03-03 04:50:47.898234 trex-apis-0.2.9/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-0.2.9/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-03-03 04:50:47.898656 trex-apis-0.2.9/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-03-03 04:45:38.000000 trex-apis-0.2.9/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.881320 trex-apis-0.2.9/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1110 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.882144 trex-apis-0.2.9/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-0.2.9/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      728 2023-01-03 04:03:16.000000 trex-apis-0.2.9/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.892379 trex-apis-0.2.9/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-0.2.9/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7390 2023-01-25 07:12:41.000000 trex-apis-0.2.9/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-0.2.9/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31457 2023-02-26 09:27:48.000000 trex-apis-0.2.9/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-0.2.9/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8300 2023-01-13 04:35:13.000000 trex-apis-0.2.9/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10939 2023-02-24 02:08:38.000000 trex-apis-0.2.9/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-0.2.9/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-0.2.9/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27309 2023-02-22 08:31:07.000000 trex-apis-0.2.9/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36302 2023-01-30 04:44:34.000000 trex-apis-0.2.9/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-0.2.9/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14802 2023-02-27 02:58:10.000000 trex-apis-0.2.9/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.893265 trex-apis-0.2.9/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-0.2.9/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4454 2023-01-18 15:02:20.000000 trex-apis-0.2.9/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.895073 trex-apis-0.2.9/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-0.2.9/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-0.2.9/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7220 2023-02-20 04:25:05.000000 trex-apis-0.2.9/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-0.2.9/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.895877 trex-apis-0.2.9/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-0.2.9/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-0.2.9/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.897144 trex-apis-0.2.9/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-0.2.9/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-0.2.9/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    61210 2023-03-03 04:45:00.000000 trex-apis-0.2.9/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.528474 trex-apis-1.0.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-17 03:30:13.528585 trex-apis-1.0.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-17 03:30:13.529000 trex-apis-1.0.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-04-17 03:27:06.000000 trex-apis-1.0.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.517962 trex-apis-1.0.0/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1164 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.518481 trex-apis-1.0.0/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.0/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      728 2023-01-03 04:03:16.000000 trex-apis-1.0.0/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.525039 trex-apis-1.0.0/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.0/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7466 2023-03-08 14:11:16.000000 trex-apis-1.0.0/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.0/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35717 2023-04-12 10:19:52.000000 trex-apis-1.0.0/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.0/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.0/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.0/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10939 2023-03-21 01:50:25.000000 trex-apis-1.0.0/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.0/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.0/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27328 2023-04-12 09:15:21.000000 trex-apis-1.0.0/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.0/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.0/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.0/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.525512 trex-apis-1.0.0/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.0/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4555 2023-03-21 09:28:04.000000 trex-apis-1.0.0/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.526841 trex-apis-1.0.0/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.0/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.0/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7220 2023-02-20 04:25:05.000000 trex-apis-1.0.0/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.0/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.527208 trex-apis-1.0.0/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.0/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.0/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.528196 trex-apis-1.0.0/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.0/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.0/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    74352 2023-04-12 06:10:24.000000 trex-apis-1.0.0/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-0.2.9/setup.py` & `trex-apis-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='0.2.9',
+     version='1.0.0',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-0.2.9/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.0/trex_apis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 trex_apis.egg-info/top_level.txt
 trexapi/__init__.py
 trexapi/conf.py
 trexapi/controllers/__init__.py
 trexapi/controllers/api_routes.py
 trexapi/controllers/app_api_routes.py
 trexapi/controllers/customer_api_routes.py
+trexapi/controllers/customer_membership_api_routes.py
 trexapi/controllers/customer_reward_api_routes.py
 trexapi/controllers/loyalty_api_routes.py
 trexapi/controllers/outlet_api_routes.py
 trexapi/controllers/payment_api_routes.py
 trexapi/controllers/pos_api_routes.py
 trexapi/controllers/reward_api_routes.py
 trexapi/controllers/user_api_routes.py
```

### Comparing `trex-apis-0.2.9/trexapi/conf.py` & `trex-apis-1.0.0/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/api_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
                     if api_key == merchant_acct.api_key:
                         merchant_user               = MerchantUser.get_by_username(username)
                         (expiry_datetime, token)    = self.generate_token(acct_id, username)
                         #session['auth_username']    = username
                         #session['acct_id']          = acct_id
                         
                         logger.debug('token=%s', token)
+                        logger.debug('expiry_datetime=%s', expiry_datetime)
                         logger.debug('auth_username=%s', username)
             
                         output_json =  {
                                         'auth_token'        : token,
                                         'expires_in'        : int(api_conf.API_TOKEN_EXPIRY_LENGTH_IN_MINUTE) * 60,
                                         #'expiry_datetime'   : expiry_datetime.strftime('%d-%m-%Y %h:%M:$S'),
                                         'granted_outlet'    : merchant_user.granted_outlet_details_list,
```

### Comparing `trex-apis-0.2.9/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/customer_api_routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from flask.json import jsonify
 from datetime import datetime
 from trexapi.decorators.api_decorators import auth_token_required,\
     outlet_key_required
 from trexlib.utils.string_util import is_not_empty
-from trexmodel.models.datastore.customer_models import Customer
+from trexmodel.models.datastore.customer_models import Customer,\
+    CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from trexmodel.models.datastore.merchant_models import Outlet,\
     MerchantAcct, MerchantUser
 from trexapi.forms.customer_api_forms import CustomerDetailsNewForm, CustomerDetailsUpdateForm,\
     CustomerSearchForm
@@ -28,14 +29,18 @@
 from trexapi.controllers.user_api_routes import user_details_dict
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexapi.utils.reward_transaction_helper import revert_redemption,\
     revert_transaction
+from trexanalytics.bigquery_upstream_data_config import create_merchant_registered_customer_upstream_for_merchant,\
+    create_registered_customer_upstream_for_system
+from trexmodel.models.datastore.membership_models import MerchantMembership,\
+    MerchantTierMembership
 
 logger = logging.getLogger('api')
 
 
 customer_api_bp = Blueprint('customer_api_base_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
@@ -149,14 +154,18 @@
                                                             email                   = customer_data_in_json.get('email'), 
                                                             gender                  = customer_data_in_json.get('gender'),
                                                             birth_date              = birth_date,
                                                             mobile_phone            = mobile_phone, 
                                                             merchant_reference_code = customer_data_in_json.get('merchant_reference_code'), 
                                                             password                = customer_data_in_json.get('password'),
                                                             )
+                            
+                            create_merchant_registered_customer_upstream_for_merchant(created_customer)
+                            create_registered_customer_upstream_for_system(created_customer)
+                            
                         logger.debug('created_customer=%s', created_customer)
                     else:
                         logger.warn('Invalid granted outlet key')
                 else:
                     logger.warn('Invalid granted outlet key')
             
                 if customer_is_exist:
@@ -460,14 +469,78 @@
                 customer_list.append(customer_details_dict)
     
         #return create_rest_message(status_code=StatusCode.OK, customer_list=customer_list)
         return jsonify(customer_list)
     else:
         return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
 
+@customer_api_bp.route('/reference-code/<reference_code>/list-membership', methods=['GET'])
+@auth_token_required
+def list_customer_membership(reference_code):
+    if is_not_empty(reference_code):
+        acct_id   = request.headers.get('x-acct-id')
+        db_client = create_db_client(caller_info="list_customer_membership")
+        customer_membership_final_list = []
+        
+        logger.debug('reference_code=%s', reference_code)
+        
+        with db_client.context():
+            merchant_acct = MerchantAcct.fetch(acct_id)
+            customer = Customer.get_by_reference_code(reference_code, merchant_acct)
+            customer_memberhips_list        = CustomerMembership.list_active_by_customer(customer)
+            customer_tier_memberhips_list   = CustomerTierMembership.list_active_by_customer(customer)
+            
+            logger.debug('customer=%s', customer)
+            
+            logger.debug('customer_memberhips_list=%s', customer_memberhips_list)
+            
+            if is_not_empty(customer_memberhips_list):
+                merchant_memberships_list = MerchantMembership.list_by_merchant_acct(merchant_acct)
+                
+                for cm in customer_memberhips_list:
+                    for mm in merchant_memberships_list:
+                        if mm.key_in_str == cm.merchant_membership_key:
+                            customer_membership_data = {
+                                                            'key'           : cm.key_in_str,
+                                                            'label'         : mm.label,
+                                                            'entitled_date' : cm.entitled_date.strftime('%d-%m-%Y'),
+                                                            'expiry_date'   : cm.expiry_date.strftime('%d-%m-%Y'),
+                                                            'is_tier'       : False,
+                                                            }
+                            
+                            if cm.renewed_date is not None:
+                                customer_membership_data['renewed_date'] = cm.renewed_date.strftime('%d-%m-%Y'),
+                            
+                            customer_membership_final_list.append(customer_membership_data)
+                            break
+                        
+            if is_not_empty(customer_tier_memberhips_list):
+                merchant_tier_memberships_list = MerchantTierMembership.list_by_merchant_acct(merchant_acct)
+                
+                for cm in customer_tier_memberhips_list:
+                    for mm in merchant_tier_memberships_list:
+                        if mm.key_in_str == cm.merchant_tier_membership_key:
+                            customer_membership_data = {
+                                                            'key'           : cm.key_in_str,
+                                                            'label'         : mm.label,
+                                                            'entitled_date' : cm.entitled_date.strftime('%d-%m-%Y'),
+                                                            'expiry_date'   : cm.expiry_date.strftime('%d-%m-%Y'),
+                                                            'is_tier'       : True,
+                                                            }
+                            
+                            customer_membership_final_list.append(customer_membership_data)
+                            break            
+        
+    
+        return jsonify(customer_membership_final_list)
+    else:
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+                
+
+
 @customer_api_bp.route('/reference-code/<reference_code>/transaction/limit/<limit>', methods=['GET'])
 @auth_token_required
 def list_customer_transaction(reference_code, limit):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
```

### Comparing `trex-apis-0.2.9/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/reward_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             logger.debug('reward transaction data is valid')
             
             sales_amount        = float(reward_transaction_form.sales_amount.data)
             tax_amount          = reward_transaction_form.tax_amount.data
             invoice_id          = reward_transaction_form.invoice_id.data
             remarks             = reward_transaction_form.remarks.data
             invoice_details     = transaction_data_in_json.get('invoice_details')
+            
             transact_datetime   = None
             
             
             if tax_amount is None:
                 tax_amount = .0
             else:
                 tax_amount = float(tax_amount)
@@ -137,14 +138,16 @@
             
             if check_transaction_by_invoice_id:
                 return create_rest_message("The invoice id have been taken", status_code=StatusCode.BAD_REQUEST)
             else:
                 transact_datetime_in_gmt    = reward_transaction_form.transact_datetime.data
                 merchant_username           = get_logged_in_api_username()
                 
+                logger.debug('transact_datetime_in_gmt=%s', transact_datetime_in_gmt)
+                
                 if merchant_username:
                     try:
                         with db_client.context():
                             transact_outlet         = Outlet.fetch(request.headers.get('x-outlet-key'))
                             merchant_acct           = transact_outlet.merchant_acct_entity
                             customer                = Customer.get_by_reference_code(reference_code, merchant_acct)
                             
@@ -346,16 +349,15 @@
                 merchant_acct           = topup_outlet.merchant_acct_entity
                 customer_acct           = Customer.get_by_reference_code(reference_code, merchant_acct)
                 prepaid_program         = PrepaidSettings.fetch(prepaid_program_key)
                 topup_by_merchant_user  = MerchantUser.get_by_username(merchant_username)
                 
                 if customer_acct and prepaid_program:
                     
-                    (customer_transaction, prepaid_summary) = create_topup_prepaid_transaction(customer_acct, 
-                                                                                                prepaid_program, 
+                    (customer_transaction, prepaid_summary) = create_topup_prepaid_transaction(customer_acct, prepaid_program, 
                                                                                                 topup_amount=topup_amount, 
                                                                                                 topup_outlet=topup_outlet, 
                                                                                                 topup_by=topup_by_merchant_user, 
                                                                                                 invoice_id=invoice_id, 
                                                                                                 remarks = remarks,
                                                                                                 system_remarks = 'Topup Prepaid',
                                                                                                 )
```

### Comparing `trex-apis-0.2.9/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/user_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,22 +140,25 @@
             user_acct = User.get_by_email(email)
         
         if user_acct:
             logger.debug('auth_user: found user account by email=%s', email)    
             logger.debug('auth_user: found user account by password=%s', password)
             if user_acct.is_valid_password(password):
                 (expiry_datetime, token)    = generate_user_auth_token(user_acct.user_id, user_acct.reference_code)
+                
+                response_data = {
+                                    'auth_token'              : token,
+                                    }
+                    
+                response_data.update(user_details_dict(user_acct))
+                
+                logger.debug('auth_user debug: response_data=%s', response_data)
+                
                 return create_rest_message(status_code=StatusCode.OK, 
-                                           auth_token                           = token,
-                                           reference_code                       = user_acct.reference_code, 
-                                           name                                 = user_acct.name, 
-                                           is_email_verified                    = user_acct.is_email_verified, 
-                                           is_mobile_phone_verified             = user_acct.is_mobile_phone_verified,
-                                           email_vc_expiry_datetime             = str(user_acct.email_vc_expiry_datetime),
-                                           mobile_phone_vc_expiry_datetime      = str(user_acct.mobile_phone_vc_expiry_datetime),
+                                           **response_data
                                            
                                            )
             
             else:
                 logger.warn('auth_user: user password is invalid')
                 return create_rest_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
             
@@ -236,31 +239,32 @@
             return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_mobile_phone_account: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
 
 @user_api_bp.route('/register-as-customer', methods=['POST'])
+@user_auth_token_required
 def register_user_as_customer():
     user_data_in_json           = request.get_json()
     reference_code              = user_data_in_json.get('reference_code')
     merchant_reference_code     = user_data_in_json.get('merchant_reference_code')
+    outlet_key                  = user_data_in_json.get('outlet_key')
     
     logger.debug('register_user_as_customer: user_data_in_json=%s', user_data_in_json)
     
     try:
         if is_not_empty(reference_code):
             logger.debug('customer registration input is valid')
             db_client = create_db_client(caller_info="register_user_as_customer")
             
             created_customer        = None
             existing_user_acct      = None
             is_email_used           = False
             is_mobile_phone_used    = False
-            outlet_key              = request.headers.get('x-outlet-key')
             merchant_act_key        = None
             
             merchant_acct           = None
             
             with db_client.context():
                 existing_user_acct  = User.get_by_reference_code(reference_code)
                 if existing_user_acct:
@@ -353,21 +357,21 @@
     
     email_vc_expiry_datetime            = None
     mobile_phone_vc_expiry_datetime     = None
     
     email_verified_datetime             = None
     mobile_phone_verified_datetime      = None
     
-    if is_email_verified == False:
+    if is_email_verified == False and is_not_empty(user_acct.email_vc_expiry_datetime):
         #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
         email_vc_expiry_datetime = str(user_acct.email_vc_expiry_datetime)
     else:
         email_verified_datetime = str(user_acct.email_verified_datetime)
             
-    if is_mobile_phone_verified == False:
+    if is_mobile_phone_verified == False and is_not_empty(user_acct.mobile_phone_vc_expiry_datetime):
         #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
         mobile_phone_vc_expiry_datetime = str(user_acct.mobile_phone_vc_expiry_datetime)
     else:
         mobile_phone_verified_datetime = str(user_acct.mobile_phone_verified_datetime)
         
     birth_date_str = None
     if is_not_empty(user_acct.birth_date):
@@ -409,20 +413,21 @@
             db_client = create_db_client(caller_info="register_user_as_customer")
             
             customer                = None
             outlet_key              = request.headers.get('x-outlet-key')
             merchant_acct           = None
             existing_user_acct      = None
             
+            logger.debug('outlet_key=%s', outlet_key)
+            
             with db_client.context():
                 outlet          = Outlet.fetch(outlet_key)
                     
-                if merchant_acct and outlet:
-                        
-                    logger.debug('merchant_acct.key_in_str=%s', merchant_acct.key_in_str)
+                if outlet:
+                    merchant_acct = outlet.merchant_acct_entity    
                     logger.debug('outlet.merchant_acct_key=%s', outlet.merchant_acct_key)
                     
                     
                     customer = Customer.get_by_reference_code(reference_code, merchant_acct)
                     existing_user_acct = User.get_by_reference_code(reference_code)
                      
                 else:
```

### Comparing `trex-apis-0.2.9/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.0/trexapi/controllers/voucher_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_redemption_upstream_for_merchant
 from trexmodel import program_conf
 from trexapi import conf
 from trexmodel.models.datastore.user_models import User
 from flask.json import jsonify
+from trexmodel.models.datastore.model_decorators import model_transactional
 
 logger = logging.getLogger('api')
 
 
 voucher_api_bp = Blueprint('voucher_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
@@ -157,26 +158,33 @@
                 return create_rest_message("Voucher ({redeem_codes_list}) is not valid".format(redeem_codes_list=",".join(found_not_valid_redeem_code_list)), 
                                            status_code=StatusCode.BAD_REQUEST)            
             
             elif already_redeemed_list:
                 return create_rest_message("Voucher ({redeem_codes_list}) have been redeemed before,  thus it is not allow to redeem again".format(redeem_codes_list=",".join(already_redeemed_list)), 
                                            status_code=StatusCode.BAD_REQUEST)
             else:
-                if to_redeem_voucher_keys_list:
-                    with db_client.context():
-                        if to_redeem_voucher_keys_list:
-                            
-                            customer_redemption = CustomerRedemption.create(customer, program_conf.REWARD_FORMAT_VOUCHER , redeemed_by_outlet,
+                
+                @model_transactional(desc='redeem_voucher')
+                def __start_transaction_for_redeem_voucher():
+                    
+                    customer_redemption = CustomerRedemption.create(customer, program_conf.REWARD_FORMAT_VOUCHER , redeemed_by_outlet,
                                       redeemed_amount               = 1,            
                                       redeemed_voucher_keys_list    = to_redeem_voucher_keys_list, 
                                       redeemed_by                   = redeemed_by, 
                                       redeemed_datetime             = redeemed_datetime,
                                       invoice_id                    = invoice_id,
                                       remarks                       = remarks,
                                       )
+                    return customer_redemption
+                
+                if to_redeem_voucher_keys_list:
+                    with db_client.context():
+                        if to_redeem_voucher_keys_list:
+                            
+                            customer_redemption = __start_transaction_for_redeem_voucher()
                             
                             logger.debug('customer_redemption=%s', customer_redemption)
                             
             
                         if customer_redemption:
                             create_merchant_customer_redemption_upstream_for_merchant(customer_redemption, streamed_datetime=redeemed_datetime)
```

### Comparing `trex-apis-0.2.9/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.0/trexapi/decorators/api_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from flask import request, session, abort
 from trexlib.utils.string_util import is_not_empty
 from trexlib.utils.crypto_util import decrypt_json
 import logging
 from datetime import datetime
 
 logger = logging.getLogger('decorator')
-
+#logger = logging.getLogger('debug')
 
 def auth_token_required(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
         auth_token  = request.headers.get('x-auth-token')
         acct_id     = request.headers.get('x-acct-id')
             
         logger.debug('acct_id=%s', acct_id)
         logger.debug('auth_token=%s', auth_token)
         
         if is_not_empty(auth_token):
             try:
                 auth_details_json = decrypt_json(auth_token)
             except:
+                logger.error('Authenticated token is not valid')
                 return ("Authenticated token is not valid", 401)
             
             logger.debug('auth_details_json=%s', auth_details_json)
             
             if auth_details_json:
                 expiry_datetime     = auth_details_json.get('expiry_datetime')
                 acct_id_from_token  = auth_details_json.get('acct_id')
```

### Comparing `trex-apis-0.2.9/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.0/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.0/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.0/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.0/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/utils/api_helpers.py` & `trex-apis-1.0.0/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.9/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.0/trexapi/utils/reward_transaction_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 from trexlib.utils.google.cloud_tasks_util import create_task
 from trexadmin import conf
 from trexlib.conf import CHECK_CUSTOMER_ENTITLE_REWARD_TASK_URL, SYSTEM_TASK_SERVICE_CREDENTIAL_PATH, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL  
 import logging
 from trexadmin.libs.app.reward_program.reward_program_factory import RewardProgramFactory
 from trexadmin.controllers.system.system_routes import get_currency_config
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
-    CustomerStampReward, CustomerEntitledVoucher, VoucherRewardDetailsForUpstreamData
+    CustomerStampReward, CustomerEntitledVoucher, VoucherRewardDetailsForUpstreamData,\
+    CustomerEntitledTierRewardSummary
 from datetime import datetime
 from trexmodel import program_conf
 from trexmodel.models.datastore.customer_model_helpers import update_customer_entiteld_voucher_summary_after_reverted_voucher,\
     update_reward_summary_with_new_reward,\
     update_prepaid_summary_with_new_prepaid,\
     update_customer_entiteld_voucher_summary_with_customer_new_voucher,\
-    update_prepaid_summary_with_reverted_prepaid
+    update_prepaid_summary_with_reverted_prepaid,\
+    update_reward_summary_with_reverted_reward
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_reverted_upstream_for_merchant,\
     create_merchant_customer_transaction_upstream_for_merchant,\
     create_merchant_customer_redemption_upstream_for_merchant,\
     create_merchant_customer_prepaid_upstream_for_merchant,\
     create_merchant_customer_prepaid_reverted_upstream_for_merchant,\
     create_merchant_customer_redemption_reverted_upstream_for_merchant
 from trexmodel.models.datastore.membership_models import MerchantTierMembership
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 from trexadmin.libs.app.reward_program.reward_program_base import EntitledVoucherSummary
-from trexmodel.models.datastore.customer_models import Customer
+from trexmodel.models.datastore.customer_models import Customer,\
+    CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
+from trexlib.utils.string_util import is_not_empty
+from trexlib.utils.log_util import get_tracelog
 
 logger = logging.getLogger('debug')
 #logger = logging.getLogger('debug')
 
 
 def create_sales_transaction(customer, transact_outlet=None, sales_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
                             transact_by=None, transact_datetime=None, invoice_details=None):
@@ -70,26 +75,27 @@
         if trigger_check_reward_success:
             create_merchant_customer_transaction_upstream_for_merchant(customer_transaction, streamed_datetime=transact_datetime)
         
         return customer_transaction
         
     return __start_transaction_for_customer_transaction()
 
-def create_non_sales_system_transaction(customer, transact_datetime=None, remarks=None):
+def create_non_sales_system_transaction(customer, transact_datetime=None, remarks=None, system_remarks=None):
     
     logger.debug('---create_sales_transaction---')
     
     #@model_transactional(desc='create_non_sales_system_transaction')
     def __start_transaction_for_customer_transaction():
         customer_transaction = CustomerTransaction.create_system_transaction(
                                        customer, 
                                        transact_datetime    = transact_datetime,
                                        allow_to_revert      = False,
                                        is_sales_transaction = False,
                                        remarks              = remarks,
+                                       system_remarks       = system_remarks,
                                        )
             
         return customer_transaction
         
     return __start_transaction_for_customer_transaction()
     
 def trigger_spending_reward_for_transaction(transaction_details):
@@ -120,23 +126,17 @@
                         service_email   = SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
                         )
         
         return True
     else:
         
         customer_acct       = transaction_details.transact_customer_acct
-        merchant_acct       = transaction_details.transact_merchant_acct
+        #merchant_acct       = transaction_details.transact_merchant_acct
         check_reward_status = check_spending_reward_for_transaction(customer_acct, transaction_details)
         
-        if check_reward_status:
-            
-            update_customer_kpi_summary_and_transact_summary(customer_acct, transaction_details)
-            check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details)
-            #check_tier_reward_for_transaction(customer_acct, transaction_details)
-            
         return check_reward_status
 
 def update_customer_kpi_summary_and_transact_summary(customer_acct, transaction_details):
     
     logger.debug('---update_customer_kpi_summary_and_transact_summary---')
     
     kpi_summary = customer_acct.kpi_summary
@@ -230,147 +230,181 @@
     
     logger.debug('update_customer_kpi_summary_from_transaction_list debug: customer_acct.kpi_summary after updated=%s', customer_acct.kpi_summary)
     
 
 def check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details):
     
     logger.debug('---check_for_tier_membership_upgrade_downgrade---')
-    
-    merchant_tier_membership_list   = MerchantTierMembership.list_by_merchant_acct(merchant_acct)
-    existing_tier_membership_key    = customer_acct.tier_membership_key
-    existing_tier_membership        = None
-    membership_to_assign            = None
-    
-    customer_kpi_summary            = customer_acct.kpi_summary
-    
-    total_transact_amount           = customer_kpi_summary['total_transact_amount']
-    total_accumulated_point         = customer_kpi_summary['total_accumulated_point']
-    total_accumulated_stamp         = customer_kpi_summary['total_accumulated_stamp'] 
-    total_accumulated_prepaid       = customer_kpi_summary['total_accumulated_prepaid']
-    
-    logger.debug('check_for_tier_membership_upgrade_downgrade: total_transact_amount=%s', total_transact_amount)
-    logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_point=%s', total_accumulated_point)
-    logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_stamp=%s', total_accumulated_stamp)
-    logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_prepaid=%s', total_accumulated_prepaid)
-    
-    existing_membership_qualification_details       = {}
-    highest_entitle_qualification_details           = {}
-    no_membership_or_membership_is_auto_assigned    = False
-    
-    if existing_tier_membership_key:
-        existing_tier_membership        = MerchantTierMembership.fetch(existing_tier_membership_key)
-        
-        if existing_tier_membership:
-            if existing_tier_membership.archived==True:
-                existing_tier_membership = None
-                no_membership_or_membership_is_auto_assigned = True
-            else:
-                if existing_tier_membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_AUTO_ASSIGN:
-                    no_membership_or_membership_is_auto_assigned = True
+    if merchant_acct.is_tier_membership_configured:
+        merchant_tier_membership_list   = MerchantTierMembership.list_by_merchant_acct(merchant_acct)
+        existing_tier_membership_key    = customer_acct.tier_membership_key
+        existing_tier_membership        = None
+        membership_to_assign            = None
+        
+        customer_kpi_summary            = customer_acct.kpi_summary
+        
+        total_transact_amount           = customer_kpi_summary['total_transact_amount']
+        total_accumulated_point         = customer_kpi_summary['total_accumulated_point']
+        total_accumulated_stamp         = customer_kpi_summary['total_accumulated_stamp'] 
+        total_accumulated_prepaid       = customer_kpi_summary['total_accumulated_prepaid']
+        
+        logger.debug('check_for_tier_membership_upgrade_downgrade: total_transact_amount=%s', total_transact_amount)
+        logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_point=%s', total_accumulated_point)
+        logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_stamp=%s', total_accumulated_stamp)
+        logger.debug('check_for_tier_membership_upgrade_downgrade: total_accumulated_prepaid=%s', total_accumulated_prepaid)
+        
+        existing_membership_qualification_details                   = {}
+        highest_entitle_qualification_details                       = {}
+        no_membership_or_existing_membership_is_auto_assigned       = False
+        
+        if existing_tier_membership_key:
+            existing_tier_membership        = MerchantTierMembership.fetch(existing_tier_membership_key)
+            
+            if existing_tier_membership:
+                if existing_tier_membership.archived==True:
+                    existing_tier_membership = None
+                    no_membership_or_existing_membership_is_auto_assigned = True
                 else:
-                    existing_membership_qualification_details[existing_tier_membership.entitle_qualification_type] = existing_tier_membership.entitle_qualification_value
-    else:
-        no_membership_or_membership_is_auto_assigned = True
-            
-    for membership in merchant_tier_membership_list:
-        
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_AUTO_ASSIGN:
-            if existing_tier_membership is None:
-                membership_to_assign = membership
-                
-                logger.debug('Found auto assign tier membership')
+                    if existing_tier_membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_AUTO_ASSIGN:
+                        no_membership_or_existing_membership_is_auto_assigned = True
+                    else:
+                        existing_membership_qualification_details[existing_tier_membership.entitle_qualification_type] = existing_tier_membership.entitle_qualification_value
+        else:
+            no_membership_or_existing_membership_is_auto_assigned = True
                 
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_EXCEED_SPENDING_AMOUNT:
-            if transaction_details.transact_amount >= membership.entitle_qualification_value:
-                highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
-                if membership.entitle_qualification_value > highest_entitle_qualification_value:
+        for membership in merchant_tier_membership_list:
+            logger.debug('checking tier membership %s, entitle_qualification_type=%s', membership.label, membership.entitle_qualification_type)
+            
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_AUTO_ASSIGN:
+                if membership_to_assign is None:
                     membership_to_assign = membership
-                    highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
                     
-                    logger.debug('Found %s tier membership to assign', membership.label)
-            
+                    logger.debug('Found auto assign tier membership')
+                    
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_EXCEED_SPENDING_AMOUNT:
+                logger.debug('checking tier membership is based on spending amount')
+                if transaction_details.transact_amount >= membership.entitle_qualification_value:
+                    highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
+                    if membership.entitle_qualification_value > highest_entitle_qualification_value:
+                        membership_to_assign = membership
+                        highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                        
+                        logger.debug('Found %s tier membership to assign', membership.label)
                 
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_SPENDING_AMOUNT:
-            if total_transact_amount >= membership.entitle_qualification_value:
-                highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
-                if membership.entitle_qualification_value > highest_entitle_qualification_value:
-                    membership_to_assign = membership
-                    highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
                     
-                    logger.debug('Found %s tier membership to assign', membership.label)
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_SPENDING_AMOUNT:
+                logger.debug('checking tier membership is based on accumulated spending amount, where amount is %s', membership.entitle_qualification_value)
+                if total_transact_amount >= membership.entitle_qualification_value:
+                    highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
+                    if membership.entitle_qualification_value > highest_entitle_qualification_value:
+                        membership_to_assign = membership
+                        highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                        
+                        logger.debug('Found %s tier membership to assign', membership.label)
+                        
                     
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_POINT_AMOUNT:
+                logger.debug('checking tier membership is based on accumulated point amount, where amount is %s', membership.entitle_qualification_value)
+                if total_accumulated_point >= membership.entitle_qualification_value:
+                    highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
+                    if membership.entitle_qualification_value > highest_entitle_qualification_value:
+                        membership_to_assign = membership
+                        highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                        
+                        logger.debug('Found %s tier membership to assign', membership.label)
                 
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_POINT_AMOUNT:
-            if total_accumulated_point >= membership.entitle_qualification_value:
-                highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
-                if membership.entitle_qualification_value > highest_entitle_qualification_value:
-                    membership_to_assign = membership
-                    highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                                        
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_STAMP_AMOUNT:
+                logger.debug('checking tier membership is based on accumulated stamp amount, where amount is %s', membership.entitle_qualification_value)
+                if total_accumulated_stamp >= membership.entitle_qualification_value:
+                    highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
+                    if membership.entitle_qualification_value > highest_entitle_qualification_value:
+                        membership_to_assign = membership
+                        highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                        
+                        logger.debug('Found %s tier membership to assign', membership.label)
+                        
                     
-                    logger.debug('Found %s tier membership to assign', membership.label)
+            if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_PREPAID_AMOUNT:
+                logger.debug('checking tier membership is based on accumulated prepaid amount, where amount is %s', membership.entitle_qualification_value)
+                if total_accumulated_prepaid >= membership.entitle_qualification_value:
+                    highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
+                    if membership.entitle_qualification_value > highest_entitle_qualification_value:
+                        membership_to_assign = membership
+                        highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+                        
+                        logger.debug('Found %s tier membership to assign', membership.label)
+                        
+        
+        if membership_to_assign:
+            logger.debug('membership_to_assign=%s, ', membership_to_assign.label)
             
-                                    
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_STAMP_AMOUNT:
-            if total_accumulated_stamp >= membership.entitle_qualification_value:
-                highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
-                if membership.entitle_qualification_value > highest_entitle_qualification_value:
-                    membership_to_assign = membership
-                    highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
+            
+            is_membership_change = membership_to_assign.key_in_str!=existing_tier_membership_key
+            
+            logger.debug('is_membership_change=%s', is_membership_change)
+            
+            if existing_tier_membership:
+                logger.debug('existing_tier_membership=%s', existing_tier_membership.label)
+                
+                if is_membership_change:
+                    logger.debug('check_for_tier_membership_upgrade_downgrade: found upgrading tier membership to assign')
                     
-                    logger.debug('Found %s tier membership to assign', membership.label)
+                    CustomerTierMembership.change(customer_acct,
+                                              membership_to_assign, 
+                                              transaction_details,
+                                              entitled_datetime=transaction_details.transact_datetime,
+                                              )
                     
-                
-        if membership.entitle_qualification_type == program_conf.MEMBERSHIP_ENTITLE_QUALIFICATION_TYPE_ACCUMULATED_PREPAID_AMOUNT:
-            if total_accumulated_prepaid >= membership.entitle_qualification_value:
-                highest_entitle_qualification_value =  highest_entitle_qualification_details.get(membership.entitle_qualification_type) or 0
-                if membership.entitle_qualification_value > highest_entitle_qualification_value:
-                    membership_to_assign = membership
-                    highest_entitle_qualification_details[membership.entitle_qualification_type] = membership.entitle_qualification_value
                     
-                    logger.debug('Found %s tier membership to assign', membership.label)
                     
-    
-    if membership_to_assign:
-        
-        new_tier_membership_key = membership_to_assign.create_ndb_key()
-        
-        if existing_tier_membership:
-            if existing_tier_membership_key!=new_tier_membership_key:
-                logger.debug('check_for_tier_membership_upgrade_downgrade: found upgrading tier membership to assign')
-                customer_acct.previous_tier_membership  = customer_acct.tier_membership
-                customer_acct.tier_membership           = new_tier_membership_key
-                customer_acct.put()
-                
-                if existing_membership_qualification_details.get(membership_to_assign.entitle_qualification_type):
-                    if no_membership_or_membership_is_auto_assigned:
+                    logger.debug('existing_membership_qualification_details=%s', existing_membership_qualification_details)
+                    logger.debug('no_membership_or_existing_membership_is_auto_assigned=%s', no_membership_or_existing_membership_is_auto_assigned)
+                    
+                    check_reward_for_new_membership(customer_acct, transaction_details, membership_to_assign)
+                    
+                    '''
+                    #if existing_membership_qualification_details.get(membership_to_assign.entitle_qualification_type):
+                    if no_membership_or_existing_membership_is_auto_assigned:
+                        logger.debug('going to check reward for new tier membership')
                         check_reward_for_new_membership(customer_acct, transaction_details, membership_to_assign)
                     else:
                         if highest_entitle_qualification_details.get(membership_to_assign.entitle_qualification_type) > existing_membership_qualification_details.get(membership_to_assign.entitle_qualification_type):
-                            logger.debug('Membership upgrade')
+                            logger.debug('Membership is upgrading')
                             check_reward_for_new_membership(customer_acct, transaction_details, membership_to_assign)
                         else:
-                            logger.debug('Membership downgrade')
-                
+                            logger.debug('Membership is downgrading')
+                    '''
+                    
+                    
+                else:
+                    logger.debug('check_for_tier_membership_upgrade_downgrade: remain as existing tier membership')
             else:
-                logger.debug('check_for_tier_membership_upgrade_downgrade: remain as existing tier membership')
+                logger.debug('check_for_tier_membership_upgrade_downgrade: found new tier membership to assign')
+                CustomerTierMembership.create(customer_acct, 
+                                              membership_to_assign, 
+                                              transaction_details,
+                                              entitled_datetime=transaction_details.transact_datetime,
+                                              
+                                              )
+                #customer_acct.tier_membership = new_tier_membership_key
+                
+                check_reward_for_new_membership(customer_acct, transaction_details, membership_to_assign)
+                
+                #customer_acct.put()
         else:
-            logger.debug('check_for_tier_membership_upgrade_downgrade: found new tier membership to assign')
-            customer_acct.tier_membership = new_tier_membership_key
-            
-            check_reward_for_new_membership(customer_acct, transaction_details, membership_to_assign)
-            
-            customer_acct.put()
+            if existing_tier_membership:
+                #should be downgrade and remove membership
+                customer_acct.tier_membership           = None
+                customer_acct.put()
+                logger.debug('check_for_tier_membership_upgrade_downgrade: not tier membership to upgrade, thus remain as existing tier membership')
+            else:
+                logger.debug('check_for_tier_membership_upgrade_downgrade: not yet entitle any tier membership')
     else:
-        if existing_tier_membership:
-            #should be downgrade and remove membership
-            customer_acct.tier_membership           = None
-            customer_acct.put()
-            logger.debug('check_for_tier_membership_upgrade_downgrade: not tier membership to upgrade, thus remain as existing tier membership')
-        else:
-            logger.debug('check_for_tier_membership_upgrade_downgrade: not yet entitle any tier membership')
+        logger.debug('no tier membership is configured thus ignore')
 
 def check_reward_for_new_membership(customer_acct, transaction_details, new_membership):
     
     logger.debug('---check_reward_for_new_membership---')
     
     merchant_acct                           = transaction_details.transact_merchant_acct
     merchant_program_configuration_list     = merchant_acct.published_program_configuration.get('programs')
@@ -390,14 +424,15 @@
         if  program_reward_base== program_conf.REWARD_BASE_ON_GIVEAWAY:
             
             program_giveaway_method = program_configuration.get('giveaway_method')
             
             logger.debug('check_reward_for_new_membership: program_giveaway_method=%s', program_giveaway_method)
             
             if  program_giveaway_method== program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM:
+                logger.debug('found giveaway method is system')
                 giveaaway_system_settings = program_configuration.get('program_settings').get('giveaway_system_settings')
                 
                 logger.debug('check_reward_for_new_membership: giveaaway_system_settings=%s', giveaaway_system_settings)
                 
                 if giveaaway_system_settings is not None and giveaaway_system_settings.get('giveaway_system_condition') == program_conf.GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP:
                     logger.debug('giveaway tier memberships=%s', giveaaway_system_settings.get('giveaway_tier_memberships'))
                     if giveaaway_system_settings.get('giveaway_tier_memberships'):
@@ -405,15 +440,15 @@
                             membership_program_configuration_list.append(program_configuration)
     
     logger.debug('membership_program_configuration_list=%s', membership_program_configuration_list)
     
     if membership_program_configuration_list:
         currency_code   = merchant_acct.currency_code
         currency_config = get_currency_config(currency_code)
-        return RewardProgramFactory().get_giveaway_based_reward(customer_acct, transaction_details, 
+        return RewardProgramFactory().get_giveaway_reward(customer_acct, transaction_details, 
                                                                             program_configuration_list  = membership_program_configuration_list, 
                                                                             currency                    = currency_config
                                                                             )
     
     
 def check_tier_reward_for_transaction(customer_acct, transaction_details, program_configuration_list=None):
     
@@ -441,35 +476,61 @@
                                                             program_configuration_list=program_configuration_list, 
                                                             currency=currency_config)
     
     
     if give_reward_status:
         #check if the giveaway reward format match tier reward program setting
         check_tier_reward_for_transaction(customer_acct, transaction_details)
-    
+        update_customer_kpi_summary_and_transact_summary(customer_acct, transaction_details)
+        check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details)
+        
     return give_reward_status
     
 def check_giveaway_reward_for_transaction(customer_acct, transaction_details, program_configuration_list=None, reward_set=1):
-    merchant_acct   = transaction_details.transact_merchant_acct
-    currency_code   = merchant_acct.currency_code
+    merchant_acct                   = transaction_details.transact_merchant_acct
+    program_configuration_list      = merchant_acct.program_configuration_list if program_configuration_list is None else program_configuration_list
+    currency_code                   = merchant_acct.currency_code
     
-    currency_config = get_currency_config(currency_code)
+    currency_config                 = get_currency_config(currency_code)
     
     give_reward_status =  RewardProgramFactory().get_giveaway_reward(customer_acct, 
                                                             transaction_details, 
                                                             program_configuration_list=program_configuration_list, 
                                                             currency=currency_config, 
                                                             reward_set=reward_set)
     
     if give_reward_status:
         #check if the giveaway reward format match tier reward program setting
         check_tier_reward_for_transaction(customer_acct, transaction_details)
+        update_customer_kpi_summary_and_transact_summary(customer_acct, transaction_details)
+        check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details)
     
     return give_reward_status
 
+def check_giveaway_reward_for_membership_purchase_transaction(customer_acct, transaction_details, program_configuration_list=None, reward_set=1):
+    logger.debug('---check_giveaway_reward_for_membership_purchase_transaction---')
+    merchant_acct                   = transaction_details.transact_merchant_acct
+    program_configuration_list      = merchant_acct.program_configuration_list if program_configuration_list is None else program_configuration_list
+    
+    currency_code   = merchant_acct.currency_code
+    
+    currency_config = get_currency_config(currency_code)
+    
+    give_reward_status =  RewardProgramFactory().get_purchase_membership_giveaway_reward(customer_acct, 
+                                                            transaction_details, 
+                                                            program_configuration_list=program_configuration_list, 
+                                                            currency=currency_config, 
+                                                            reward_set=reward_set)
+    
+    '''
+    if give_reward_status:
+        #check if the giveaway reward format match tier reward program setting
+        check_tier_reward_for_transaction(customer_acct, transaction_details)
+    '''
+    return give_reward_status
 
 def redeem_reward_transaction(customer, redeem_outlet=None, reward_format=None, reward_amount=.0, invoice_id=None, remarks=None, 
                             redeemed_by=None, redeemed_datetime=None, transaction_id=None,
                             redeemed_voucher_keys_list=None
                             ):
     logger.debug('---redeem_reward_transaction---')
     
@@ -527,220 +588,315 @@
     
     for prepaid in  prepaid_reward_list:
         prepaid = prepaid.to_prepaid_summary()
         prepaid_summary = update_prepaid_summary_with_new_prepaid(prepaid_summary, prepaid)
     
     customer.prepaid_summary = prepaid_summary
     customer.put()
+    
+def update_customer_memberships_list(customer):
+    customer_memberships_list     = CustomerMembership.list_all_by_customer(customer)
+    memberships_list              = []
+    
+    
+    for customer_membership in  customer_memberships_list:
+        if customer_membership.is_valid():
+            memberships_list.append(customer_membership.merchant_membership_key)
+        
+        
+    customer.memberships_list    = memberships_list
+    
+    customer.put()    
 
-def revert_transaction(transaction_details, reverted_by, reverted_datetime=None):
+def revert_transaction(transaction_details, reverted_by, reverted_datetime=None, create_upstream=True):
     merchant_acct                       = transaction_details.transact_merchant_acct
     transaction_id                      = transaction_details.transaction_id
     customer_acct                       = transaction_details.transact_customer_acct
-    is_stamp_entitled_in_transaction    = False
-    is_point_entitled_in_transaction    = False
-    is_voucher_entitled_in_transaction  = False
-    is_prepaid_entitled_in_transaction  = False
         
-    if transaction_details.entitled_reward_summary is not None:
+    if transaction_details.is_membership_purchase:
+        #remove membership
+        purchased_customer_membership   = transaction_details.purchased_customer_membership_entity
+        try:
+            merchant_membership_key         = purchased_customer_membership.merchant_membership_key 
+            purchased_customer_membership.delete()
+        except:
+            logger.error('Failed due to %s', get_tracelog())
+        
+        
+        if is_not_empty(customer_acct.memberships_list):
+            customer_acct.memberships_list.remove(merchant_membership_key)
+        
+        customer_acct.put()
+        
+        return True
+        
+    elif transaction_details.is_membership_renew:
+        #revert renewal
+        renewed_customer_membership = transaction_details.purchased_customer_membership_entity
+        renewed_customer_membership.revert_renewal()    
+        customer_acct.put()
+        
+        return True
+    else:    
+    
         is_stamp_entitled_in_transaction    = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_STAMP) is not None
         is_point_entitled_in_transaction    = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_POINT) is not None
         is_voucher_entitled_in_transaction  = transaction_details.entitled_voucher_summary is not None
-    
-    
-    if transaction_details.entitled_prepaid_summary is not None:
-        is_prepaid_entitled_in_transaction  = True
-    
-    
-    reverting_point_details_list        = CustomerPointReward.list_by_transaction_id(transaction_id) if is_point_entitled_in_transaction else []
-    reverting_stamp_details_list        = CustomerStampReward.list_by_transaction_id(transaction_id) if is_stamp_entitled_in_transaction else []
-    reverting_vouchers_list             = CustomerEntitledVoucher.list_by_transaction_id(transaction_id) if is_voucher_entitled_in_transaction else []
-    reverting_prepaid_list              = CustomerPrepaidReward.list_by_transaction_id(transaction_id) if is_prepaid_entitled_in_transaction else []
-    
-    is_transaction_reward_used          = False
-    customer_prepaid_summary            = customer_acct.prepaid_summary or {}
-    entitled_voucher_summary            = customer_acct.entitled_voucher_summary or {}
-    
-    
-    if reverted_datetime is None:
-        reverted_datetime = datetime.utcnow()
-    
-    logger.debug('revert_transaction: transaction_id=%s', transaction_id)
-    logger.debug('revert_transaction: reverted_datetime=%s', reverted_datetime)
-    logger.debug('revert_transaction: reverting_point_details_list count=%s', len(reverting_point_details_list))
-    logger.debug('revert_transaction: reverting_stamp_details_list count=%s', len(reverting_stamp_details_list))
-    logger.debug('revert_transaction: reverting_vouchers_list count=%s', len(reverting_vouchers_list))
-    logger.debug('revert_transaction: reverting_prepaid_list count=%s', len(reverting_prepaid_list))
-    
-    for p in reverting_point_details_list:
-        if p.is_used:
-            is_transaction_reward_used = True
-            break
-    
-    if is_transaction_reward_used is False:
-        for p in reverting_stamp_details_list:
-            if p.is_used:
-                is_transaction_reward_used = True
-                break
-            
-    if is_transaction_reward_used is False:
-        for p in reverting_vouchers_list:
-            if p.is_used:
-                is_transaction_reward_used = True
-                break
-            
-    if is_transaction_reward_used is False:
-        for p in reverting_prepaid_list:
-            if p.is_used:
-                is_transaction_reward_used = True
-                break        
-    
-    logger.debug('revert: is_transaction_reward_used=%s', is_transaction_reward_used)
-    
-    if is_transaction_reward_used is False:
+        is_prepaid_entitled_in_transaction  = transaction_details.entitled_prepaid_summary is not None
         
-        logger.debug('Going to revert transaction')
         
-        reverted_by_key                                = reverted_by.create_ndb_key()
-        transaction_details.is_revert                  = True
-        transaction_details.reverted_datetime          = reverted_datetime
-        transaction_details.reverted_by                = reverted_by_key
-        transaction_details.reverted_by_username       = reverted_by.username
-        transaction_details.put()
+        logger.debug('transaction_details.entitled_reward_summary=%s', transaction_details.entitled_reward_summary)
+        logger.debug('transaction_details.entitled_prepaid_summary=%s', transaction_details.entitled_prepaid_summary)
         
-        for p in reverting_point_details_list:
-            if p.is_valid:
-                p.status                        = program_conf.REWARD_STATUS_REVERTED
-                p.reverted_datetime             = reverted_datetime
-                p.reverted_by                   = reverted_by_key
-                p.reverted_by_username          = reverted_by.username
-                p.put()
-                
-                create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
-                
-            
-        for p in reverting_stamp_details_list:
-            if p.is_valid:
-                p.status                        = program_conf.REWARD_STATUS_REVERTED
-                p.reverted_datetime             = reverted_datetime
-                p.reverted_by                   = reverted_by_key
-                p.reverted_by_username          = reverted_by.username
-                p.put()
-                
-                create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
-            
-        for p in reverting_vouchers_list:
-            if p.is_valid:
-                p.status                        = program_conf.REWARD_STATUS_REVERTED
-                p.reverted_datetime             = reverted_datetime
-                p.reverted_by                   = reverted_by_key
-                p.reverted_by_username          = reverted_by.username
-                p.put()
-                
-                entitled_voucher_summary = update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, p)
-                
-                voucher_key         = p.entitled_voucher_key
-                expiry_date         = p.expiry_date
-                rewarded_datetime   = p.rewarded_datetime
-                
-                voucher_reward_brief = VoucherRewardDetailsForUpstreamData(voucher_key, 1, expiry_date, rewarded_datetime)
-                create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, voucher_reward_brief, reverted_datetime)
-        
-        for p in reverting_prepaid_list:
-            if p.is_valid:
-                p.status                        = program_conf.REWARD_STATUS_REVERTED
-                p.reverted_datetime             = reverted_datetime
-                p.reverted_by                   = reverted_by_key
-                p.reverted_by_username          = reverted_by.username
-                p.put()
-                
-                customer_prepaid_summary = update_prepaid_summary_with_reverted_prepaid(customer_prepaid_summary, p.to_prepaid_summary())
-                create_merchant_customer_prepaid_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
-        
-        
-        
-        if is_stamp_entitled_in_transaction or is_point_entitled_in_transaction:
-            update_customer_reward_summary(customer_acct)
-        
-        if is_prepaid_entitled_in_transaction:
-            #update_customer_prepaid_summary(customer_acct)
-            customer_acct.prepaid_summary           = customer_prepaid_summary
-        
-        if is_voucher_entitled_in_transaction:
-            customer_acct.entitled_voucher_summary  = entitled_voucher_summary
-        
-        total_transact_amount       = .0
-        total_accumulated_point     = .0
-        total_accumulated_stamp     = 0
-        total_accumulated_topup     = .0
-        total_accumulated_prepaid   = .0
-        
-        
-        if customer_acct.kpi_summary:
-            total_transact_amount           = customer_acct.kpi_summary.get('total_transact_amount') or .0
-            total_accumulated_point         = customer_acct.kpi_summary.get('total_accumulated_point') or .0
-            total_accumulated_stamp         = customer_acct.kpi_summary.get('total_accumulated_stamp') or 0
-            total_accumulated_topup         = customer_acct.kpi_summary.get('total_accumulated_topup') or .0
-            total_accumulated_prepaid       = customer_acct.kpi_summary.get('total_accumulated_prepaid') or .0
         
-        else:
-            customer_acct.kpi_summary = {}
+        reverting_point_details_list        = CustomerPointReward.list_by_transaction_id(transaction_id) if is_point_entitled_in_transaction else []
+        reverting_stamp_details_list        = CustomerStampReward.list_by_transaction_id(transaction_id) if is_stamp_entitled_in_transaction else []
+        reverting_vouchers_list             = CustomerEntitledVoucher.list_by_transaction_id(transaction_id) if is_voucher_entitled_in_transaction else []
+        reverting_prepaid_list              = CustomerPrepaidReward.list_by_transaction_id(transaction_id) if is_prepaid_entitled_in_transaction else []
         
-        transaction_entitled_point      = .0
-        transaction_entitled_stamp      = 0
-        transaction_topup_prepaid       = .0
-        transaction_entitled_prepaid    = .0
+        is_transaction_reward_used          = False
+        customer_reward_summary             = customer_acct.reward_summary or {}
+        customer_prepaid_summary            = customer_acct.prepaid_summary or {}
+        entitled_voucher_summary            = customer_acct.entitled_voucher_summary or {}
         
-        if is_point_entitled_in_transaction:
-            transaction_entitled_point = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_POINT).get('amount')
-            
-        if is_stamp_entitled_in_transaction:
-            transaction_entitled_stamp = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_STAMP).get('amount')
+        
+        if reverted_datetime is None:
+            reverted_datetime = datetime.utcnow()
+        
+        logger.debug('revert_transaction: transaction_id=%s', transaction_id)
+        logger.debug('revert_transaction: reverted_datetime=%s', reverted_datetime)
+        logger.debug('revert_transaction: reverting_point_details_list count=%s', len(reverting_point_details_list))
+        logger.debug('revert_transaction: reverting_stamp_details_list count=%s', len(reverting_stamp_details_list))
+        logger.debug('revert_transaction: reverting_vouchers_list count=%s', len(reverting_vouchers_list))
+        logger.debug('revert_transaction: reverting_prepaid_list count=%s', len(reverting_prepaid_list))
+        
+        for p in reverting_point_details_list:
+            if p.is_used:
+                is_transaction_reward_used = True
+                break
+        
+        if is_transaction_reward_used is False:
+            for p in reverting_stamp_details_list:
+                if p.is_used:
+                    is_transaction_reward_used = True
+                    break
+                
+        if is_transaction_reward_used is False:
+            for p in reverting_vouchers_list:
+                if p.is_used:
+                    is_transaction_reward_used = True
+                    break
+                
+        if is_transaction_reward_used is False:
+            for p in reverting_prepaid_list:
+                if p.is_used:
+                    is_transaction_reward_used = True
+                    break        
+        
+        logger.debug('revert: is_transaction_reward_used=%s', is_transaction_reward_used)
+        
+        if is_transaction_reward_used is False:
+            
+            logger.debug('Going to revert transaction')
+            
+            reverted_by_key                                = reverted_by.create_ndb_key()
+            transaction_details.is_revert                  = True
+            transaction_details.reverted_datetime          = reverted_datetime
+            transaction_details.reverted_by                = reverted_by_key
+            transaction_details.reverted_by_username       = reverted_by.username
+            transaction_details.put()
+            
+            for p in reverting_point_details_list:
+                if p.is_valid:
+                    p.status                        = program_conf.REWARD_STATUS_REVERTED
+                    p.reverted_datetime             = reverted_datetime
+                    p.reverted_by                   = reverted_by_key
+                    p.reverted_by_username          = reverted_by.username
+                    p.put()
+                    
+                    customer_reward_summary = update_reward_summary_with_reverted_reward(customer_reward_summary, p.to_reward_summary())
+                    if create_upstream:
+                        create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
+                    
+                
+            for p in reverting_stamp_details_list:
+                if p.is_valid:
+                    p.status                        = program_conf.REWARD_STATUS_REVERTED
+                    p.reverted_datetime             = reverted_datetime
+                    p.reverted_by                   = reverted_by_key
+                    p.reverted_by_username          = reverted_by.username
+                    p.put()
+                    
+                    customer_reward_summary = update_reward_summary_with_reverted_reward(customer_reward_summary, p.to_reward_summary())
+                    if create_upstream:
+                        create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
+                
+            for p in reverting_vouchers_list:
+                if p.is_valid:
+                    p.status                        = program_conf.REWARD_STATUS_REVERTED
+                    p.reverted_datetime             = reverted_datetime
+                    p.reverted_by                   = reverted_by_key
+                    p.reverted_by_username          = reverted_by.username
+                    p.put()
+                    
+                    entitled_voucher_summary = update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, p)
+                    
+                    voucher_key         = p.entitled_voucher_key
+                    expiry_date         = p.expiry_date
+                    rewarded_datetime   = p.rewarded_datetime
+                    
+                    voucher_reward_brief = VoucherRewardDetailsForUpstreamData(voucher_key, 1, expiry_date, rewarded_datetime)
+                    if create_upstream:
+                        create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, voucher_reward_brief, reverted_datetime)
+            
+            for p in reverting_prepaid_list:
+                if p.is_valid:
+                    p.status                        = program_conf.REWARD_STATUS_REVERTED
+                    p.reverted_datetime             = reverted_datetime
+                    p.reverted_by                   = reverted_by_key
+                    p.reverted_by_username          = reverted_by.username
+                    p.put()
+                    
+                    customer_prepaid_summary = update_prepaid_summary_with_reverted_prepaid(customer_prepaid_summary, p.to_prepaid_summary())
+                    if create_upstream:
+                        #create_merchant_customer_prepaid_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
+                        create_merchant_customer_reward_reverted_upstream_for_merchant(transaction_details, p, reverted_datetime)
+            
+            
+            
+            if is_stamp_entitled_in_transaction or is_point_entitled_in_transaction:
+                #update_customer_reward_summary(customer_acct)
+                customer_acct.reward_summary           = customer_reward_summary
+            
+            if is_prepaid_entitled_in_transaction:
+                #update_customer_prepaid_summary(customer_acct)
+                customer_acct.prepaid_summary           = customer_prepaid_summary
+            
+            if is_voucher_entitled_in_transaction:
+                customer_acct.entitled_voucher_summary  = entitled_voucher_summary
+            
+            total_transact_amount       = .0
+            total_accumulated_point     = .0
+            total_accumulated_stamp     = 0
+            total_accumulated_topup     = .0
+            total_accumulated_prepaid   = .0
+            
+            
+            if customer_acct.kpi_summary:
+                total_transact_amount           = customer_acct.kpi_summary.get('total_transact_amount') or .0
+                total_accumulated_point         = customer_acct.kpi_summary.get('total_accumulated_point') or .0
+                total_accumulated_stamp         = customer_acct.kpi_summary.get('total_accumulated_stamp') or 0
+                total_accumulated_topup         = customer_acct.kpi_summary.get('total_accumulated_topup') or .0
+                total_accumulated_prepaid       = customer_acct.kpi_summary.get('total_accumulated_prepaid') or .0
             
-        if is_prepaid_entitled_in_transaction:
-            transaction_topup_prepaid = transaction_details.entitled_prepaid_summary.get('amount')
+            else:
+                customer_acct.kpi_summary = {}
             
-        customer_acct.last_transact_datetime    = customer_acct.previous_transact_datetime
-        total_transact_amount                   -= transaction_details.transact_amount
-        total_accumulated_point                 -= transaction_entitled_point
-        total_accumulated_stamp                 -= transaction_entitled_stamp
-        total_accumulated_topup                 -= transaction_topup_prepaid
-        total_accumulated_prepaid               -= transaction_entitled_prepaid
-        
-        if total_transact_amount<0:
-            total_transact_amount = .0
+            transaction_entitled_point      = .0
+            transaction_entitled_stamp      = 0
+            transaction_topup_prepaid       = .0
+            transaction_entitled_prepaid    = .0
+            
+            logger.debug('is_point_entitled_in_transaction=%s', is_point_entitled_in_transaction)
+            logger.debug('is_stamp_entitled_in_transaction=%s', is_stamp_entitled_in_transaction)
+            logger.debug('is_prepaid_entitled_in_transaction=%s', is_prepaid_entitled_in_transaction)
+            
+            if is_point_entitled_in_transaction:
+                logger.debug('transaction_details entitled point summary=%s', transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_POINT))
+                transaction_entitled_point = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_POINT).get('amount') or 0
+                
+            if is_stamp_entitled_in_transaction:
+                logger.debug('transaction_details entitled stamp summary=%s', transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_STAMP))
+                transaction_entitled_stamp = transaction_details.entitled_reward_summary.get(program_conf.REWARD_FORMAT_STAMP).get('amount') or 0
+                
+            if is_prepaid_entitled_in_transaction:
+                logger.debug('transaction_details entitled prepaid summary=%s', transaction_details.entitled_prepaid_summary)
+                transaction_topup_prepaid = transaction_details.entitled_prepaid_summary.get('amount') or .0
+                
+            customer_acct.last_transact_datetime    = customer_acct.previous_transact_datetime
+            total_transact_amount                   -= transaction_details.transact_amount
+            total_accumulated_point                 -= transaction_entitled_point
+            total_accumulated_stamp                 -= transaction_entitled_stamp
+            total_accumulated_topup                 -= transaction_topup_prepaid
+            total_accumulated_prepaid               -= transaction_entitled_prepaid
+            
+            if total_transact_amount<0:
+                total_transact_amount = .0
+                
+            if total_accumulated_point<0:
+                total_accumulated_point = .0
+                
+            if total_accumulated_stamp<0:
+                total_accumulated_stamp = 0        
+                
+            if total_accumulated_topup<0:
+                total_accumulated_topup = .0
+                
+            if total_accumulated_prepaid<0:
+                total_accumulated_prepaid = .0        
+                
+            customer_acct.kpi_summary['total_transact_amount']          = total_transact_amount
+            customer_acct.kpi_summary['total_accumulated_point']        = total_accumulated_point
+            customer_acct.kpi_summary['total_accumulated_stamp']        = total_accumulated_stamp
+            customer_acct.kpi_summary['total_accumulated_topup']        = total_accumulated_topup
+            customer_acct.kpi_summary['total_accumulated_prepaid']      = total_accumulated_prepaid
             
-        if total_accumulated_point<0:
-            total_accumulated_point = .0
             
-        if total_accumulated_stamp<0:
-            total_accumulated_stamp = 0        
+            customer_acct.put()
+             
+            check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details) 
             
-        if total_accumulated_topup<0:
-            total_accumulated_topup = .0
+            __revert_tier_reward(customer_acct, transaction_details)
             
-        if total_accumulated_prepaid<0:
-            total_accumulated_prepaid = .0        
             
-        customer_acct.kpi_summary['total_transact_amount']          = total_transact_amount
-        customer_acct.kpi_summary['total_accumulated_point']        = total_accumulated_point
-        customer_acct.kpi_summary['total_accumulated_stamp']        = total_accumulated_stamp
-        customer_acct.kpi_summary['total_accumulated_topup']        = total_accumulated_topup
-        customer_acct.kpi_summary['total_accumulated_prepaid']      = total_accumulated_prepaid
-        
-        customer_acct.put()
-         
-        check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details) 
+            return True
         
-        return True
+        else:
+            raise Exception('Transaction reward have been used')
     
+
+def __revert_tier_reward(customer, transaction_details):
+    customer_tier_reward_summary_list    = CustomerEntitledTierRewardSummary.list_tier_reward_summary_by_customer(customer)
+    transaction_id = transaction_details.transaction_id
+    
+    logger.debug('__revert_tier_reward debug: transation id to revert tier reward = %s', transaction_id)
+    
+    if is_not_empty(customer_tier_reward_summary_list):
+        for customer_tier_reward_summary in customer_tier_reward_summary_list:
+            tier_summary = customer_tier_reward_summary.tier_summary
+            is_tier_summary_reverted = False
+            logger.debug('tier_summary before =%s', tier_summary)
+            
+            for tier in tier_summary.get('tiers'):
+                unlock_value = tier.get('unlock_value')
+                
+                #for unlock_source in tier.get('unlock_source_details'):
+                unlock_sources_list = []
+                for index, unlock_source in enumerate(tier.get('unlock_source_details')):    
+                    if unlock_source.get('transaction_id') == transaction_id:
+                        logger.debug('__revert_tier_reward debug: Found unlock source based on transaction id, tier no=%d, unlock amount=%d', index, unlock_source.get('amount'))
+                        unlock_value -= unlock_source.get('amount')
+                        
+                        tier['unlock_status']   = False
+                        tier['unlock_value']    = unlock_value
+                        
+                        is_tier_summary_reverted = True
+                    else:
+                        unlock_sources_list.append(unlock_source)
+                
+                tier['unlock_source_details'] = unlock_sources_list    
+                
+            logger.debug('tier_summary after =%s', tier_summary)
+            
+            if is_tier_summary_reverted:
+                customer_tier_reward_summary.put() 
     else:
-        raise Exception('Transaction reward have been used')
-    
-    
+        logger.debug('__revert_tier_reward debug: not found any tier reward cycle for customer')
+        
+        
 def create_topup_prepaid_transaction(customer, prepaid_program, topup_outlet=None, topup_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
                             topup_by=None):
     
     logger.debug('---create_topup_prepaid_transaction---')
     
     transact_datetime   = datetime.now()
     prepaid_summary     = {}
@@ -784,14 +940,15 @@
             
             customer.prepaid_summary = prepaid_summary
             customer.put()
             
             update_customer_kpi_summary_and_transact_summary(customer, customer_transaction)
             
             create_merchant_customer_prepaid_upstream_for_merchant(customer_transaction, prepaid_topup_reward, streamed_datetime=transact_datetime)
+            create_merchant_customer_transaction_upstream_for_merchant(customer_transaction, streamed_datetime=transact_datetime)
         
         return (customer_transaction, prepaid_summary)
         
     return __start_transaction_for_customer_transaction()  
 
 
 def update_customer_all_entitled_reward_summary(customer):
@@ -925,26 +1082,63 @@
         
         logger.debug('------> going to check for program_key=%s for %s', program_key, customer.name)
         
         is_entitled_before = Customer.check_birthday_reward_have_entitled_before(customer, this_year, program_key)
         logger.debug('------> Customer(%s) entitled before (%s) =%s %s', customer.name, program_desc)
         
         if is_entitled_before == False:
-            transaction_details = create_non_sales_system_transaction(customer, transact_datetime=transact_datetime, remarks=remarks)   
+            transaction_details = create_non_sales_system_transaction(customer, transact_datetime=transact_datetime, remarks=remarks)
+            
+            logger.debug('transaction_details=%s', transaction_details)
+               
             currency_config = get_currency_config(currency_code)
             RewardProgramFactory().get_giveaway_based_reward(customer, transaction_details, 
                                                                                 program_configuration_list  = [program_configuration], 
                                                                                 currency                    = currency_config
                                                                                 )
             Customer.update_customer_entitled_birthday_reward_summary(customer, program_key)
         else:
             logger.info('Customer(%s) have entitled birthday reward (%s) on year %d', customer.name, program_desc, this_year)
     except:
         logger.error('Failed to process for customer=%s', customer.name)
         
+@model_transactional(desc="giveaway_membership_reward_to_customer")                
+def giveaway_membership_reward_to_customer(customer, program_configuration, transact_datetime, merchant_acct ):
+    
+    try:
+        this_year               = transact_datetime.year
+        program_key             = program_configuration.get('program_key')
+        program_label           = program_configuration.get('label')
+        remarks                 = program_configuration.get('remarks')
+        program_desc            = program_configuration.get('desc')
+        currency_code           = merchant_acct.currency_code
+        
+        logger.debug('------> going to check for program_key=%s for %s', program_key, customer.name)
+        
+        is_entitled_before = Customer.check_membership_year_reward_have_entitled_before(customer, this_year, program_key)
+        logger.debug('------> Customer(%s) entitled %s', customer.name, program_desc)
+        
+        if is_entitled_before == False:
+            system_remarks = 'Giveaway reward from %s' % program_label
+            transaction_details = create_non_sales_system_transaction(customer, remarks=remarks, system_remarks=system_remarks)
+            
+            logger.debug('transaction_details=%s', transaction_details)
+               
+            currency_config = get_currency_config(currency_code)
+            RewardProgramFactory().get_giveaway_reward(customer, transaction_details, 
+                                                                                program_configuration_list  = [program_configuration], 
+                                                                                currency                    = currency_config
+                                                                                )
+            Customer.update_customer_entitled_membership_reward_summary(customer, program_key)
+        else:
+            logger.info('Customer(%s) have entitled membership reward (%s) on year %d', customer.name, program_desc, this_year)
+    except:
+        logger.error('Failed to process for customer=%s, due to %s', customer.name, get_tracelog())  
+        raise      
+        
 
 def revert_redemption(redemption_details, reverted_by, reverted_datetime=None):
     
     if reverted_datetime is None:
         reverted_datetime = datetime.utcnow()
     
     redeem_transaction_id       = redemption_details.transaction_id
@@ -1132,12 +1326,12 @@
                 customer.prepaid_summary['amount'] += redeemed_amount
         
         customer.put()
         
     redemption_details.revert(reverted_by, reverted_datetime=reverted_datetime)
     
     
-    create_merchant_customer_redemption_reverted_upstream_for_merchant(redemption_details, reverted_datetime)
+    create_merchant_customer_redemption_reverted_upstream_for_merchant(redemption_details)
```

