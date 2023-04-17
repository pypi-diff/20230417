# Comparing `tmp/kittycad-0.3.5.tar.gz` & `tmp/kittycad-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.3.5.tar", max compression
+gzip compressed data, was "kittycad-0.3.6.tar", max compression
```

## Comparing `kittycad-0.3.5.tar` & `kittycad-0.3.6.tar`

### file list

```diff
@@ -1,267 +1,263 @@
--rw-r--r--   0        0        0     1065 2023-04-06 22:38:56.203191 kittycad-0.3.5/LICENSE
--rw-r--r--   0        0        0      875 2023-04-06 22:38:56.203191 kittycad-0.3.5/README.md
--rw-r--r--   0        0        0       90 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/__init__.py
--rw-r--r--   0        0        0      105 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     2840 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     2536 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      185 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     2729 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2434 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     2725 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     5024 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     3388 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4090 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     3785 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     3495 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      338 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2629 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2411 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     3428 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      102 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2581 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2104 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      142 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      104 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2409 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      219 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4186 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_2d_vector_conversion.py
--rw-r--r--   0        0        0     4024 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_3d_conversion.py
--rw-r--r--   0        0        0     3329 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     3974 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1854 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     3559 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     2643 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_execution.py
--rw-r--r--   0        0        0     3574 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3313 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3249 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     5036 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/get_file_conversion.py
--rw-r--r--   0        0        0     4877 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/get_file_conversion_for_user.py
--rw-r--r--   0        0        0     1158 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      119 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2388 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     2539 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     1954 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0       91 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2305 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     1939 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     1959 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      109 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      103 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2583 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2316 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2238 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2258 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2333 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2357 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2274 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2342 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2581 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2298 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      142 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/sessions/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/sessions/get_session_for_user.py
--rw-r--r--   0        0        0       87 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3441 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3245 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3533 2023-04-06 22:38:56.267193 kittycad-0.3.5/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3217 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     3567 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3707 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3447 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3379 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3407 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3309 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3355 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3391 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      283 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2386 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2686 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     2804 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2194 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2190 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2199 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2299 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     3257 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     3339 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2414 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     1960 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/client.py
--rw-r--r--   0        0        0     4227 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/client_test.py
--rw-r--r--   0        0        0     7833 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/__init__.py
--rw-r--r--   0        0        0      164 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2261 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      144 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2511 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      221 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      167 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4590 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1638 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      268 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      248 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8246 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2087 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3218 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_token.py
--rw-r--r--   0        0        0     1963 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1396 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5846 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0     2025 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      439 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2131 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1384 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3356 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2663 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/cluster.py
--rw-r--r--   0        0        0      171 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2193 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1574 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/commit.py
--rw-r--r--   0        0        0    14432 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/connection.py
--rw-r--r--   0        0        0     3602 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/country_code.py
--rw-r--r--   0        0        0      224 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     2337 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/currency.py
--rw-r--r--   0        0        0     4342 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/customer.py
--rw-r--r--   0        0        0     4238 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2413 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1499 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1504 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21726 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1735 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3925 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      202 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/environment.py
--rw-r--r--   0        0        0     1888 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/error.py
--rw-r--r--   0        0        0     2707 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     5849 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2019 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     6350 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file2_d_vector_conversion.py
--rw-r--r--   0        0        0      209 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file2_d_vector_export_format.py
--rw-r--r--   0        0        0      161 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file2_d_vector_import_format.py
--rw-r--r--   0        0        0     6255 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file3_d_conversion.py
--rw-r--r--   0        0        0      267 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file3_d_export_format.py
--rw-r--r--   0        0        0      289 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file3_d_import_format.py
--rw-r--r--   0        0        0     5799 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6220 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5837 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_density.py
--rw-r--r--   0        0        0      315 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0      303 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5822 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5629 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1412 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5541 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2276 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/gateway.py
--rw-r--r--   0        0        0      146 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2166 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8343 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2909 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      252 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2777 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1874 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2180 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3190 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2095 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1355 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1894 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5250 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/metadata.py
--rw-r--r--   0        0        0      317 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/method.py
--rw-r--r--   0        0        0     2967 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/new_address.py
--rw-r--r--   0        0        0     1992 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      218 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2449 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1617 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1493 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3874 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2247 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      140 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5526 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     1024 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2588 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1392 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1385 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/pong.py
--rw-r--r--   0        0        0     4159 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     1773 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3573 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1681 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6477 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      285 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6386 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      300 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6520 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      334 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6373 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      333 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6399 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      177 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6490 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      286 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6373 2023-04-06 22:38:56.271193 kittycad-0.3.5/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      199 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6537 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      307 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6412 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0      626 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6399 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      441 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6386 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      230 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6464 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      244 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6399 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0      639 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6602 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      176 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6481 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      171 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6373 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0      345 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0      434 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6419 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6447 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6457 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6386 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      196 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6425 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      263 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6438 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      182 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6490 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      206 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6455 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      209 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6464 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      250 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6373 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      303 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6425 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      311 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6412 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      188 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6399 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0      865 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2533 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5069 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/user.py
--rw-r--r--   0        0        0     1901 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       68 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3346 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       25 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/py.typed
--rw-r--r--   0        0        0      984 2023-04-06 22:38:56.275194 kittycad-0.3.5/kittycad/types.py
--rw-r--r--   0        0        0     1058 2023-04-06 22:38:56.275194 kittycad-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 kittycad-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 17:17:05.112563 kittycad-0.3.6/LICENSE
+-rw-r--r--   0        0        0      875 2023-04-17 17:17:05.112563 kittycad-0.3.6/README.md
+-rw-r--r--   0        0        0       90 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3316 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3012 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      185 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     2729 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2434 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     2725 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     4715 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     3388 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     4090 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     3785 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     3495 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      338 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2257 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2629 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     3428 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      102 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2404 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2581 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2104 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      142 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2409 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      219 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     4186 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_2d_vector_conversion.py
+-rw-r--r--   0        0        0     3329 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     3974 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1854 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     3559 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     2643 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_execution.py
+-rw-r--r--   0        0        0     3574 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3313 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3249 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1158 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      119 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2388 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     2539 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     1954 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0       91 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2091 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2305 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2280 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     1939 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     1959 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      109 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2583 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2316 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2238 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2258 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2333 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2357 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2274 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2342 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2581 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2298 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      142 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/sessions/__init__.py
+-rw-r--r--   0        0        0     2398 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/sessions/get_session_for_user.py
+-rw-r--r--   0        0        0       87 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3441 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3245 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3533 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3217 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3467 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     3567 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3243 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3707 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3447 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3379 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3407 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3309 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3243 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3327 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3355 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3467 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3391 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3327 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      283 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2386 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2686 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     2804 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2194 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2190 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2199 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     3257 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     3339 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2414 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     1960 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/client.py
+-rw-r--r--   0        0        0     4227 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/client_test.py
+-rw-r--r--   0        0        0     7730 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2261 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      144 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2511 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      221 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      167 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4590 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1638 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      268 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      248 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8246 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2087 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3218 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     1963 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1396 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5846 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0     2025 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      395 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2131 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1384 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3356 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2663 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      171 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2193 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1574 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14432 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/connection.py
+-rw-r--r--   0        0        0     3602 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      224 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     2337 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4342 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4238 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2413 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1499 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1504 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21726 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1735 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3925 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      202 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1888 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/error.py
+-rw-r--r--   0        0        0     2707 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     5849 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2019 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     6350 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_conversion.py
+-rw-r--r--   0        0        0      209 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_export_format.py
+-rw-r--r--   0        0        0      161 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_import_format.py
+-rw-r--r--   0        0        0      289 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file3_d_import_format.py
+-rw-r--r--   0        0        0     5799 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6220 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5837 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_density.py
+-rw-r--r--   0        0        0      315 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0      303 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5822 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5629 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5541 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2276 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      146 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2166 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8343 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2909 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      252 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2777 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1874 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2180 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3190 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2095 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1355 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1894 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5250 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/metadata.py
+-rw-r--r--   0        0        0      317 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/method.py
+-rw-r--r--   0        0        0     2967 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     1992 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      218 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2449 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1617 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1493 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3874 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2247 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      140 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5526 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     1024 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2588 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1392 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1385 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4159 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     1773 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3573 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1681 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6477 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      285 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      300 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6520 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      334 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      333 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      177 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6490 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      286 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      199 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6537 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      307 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0      626 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      441 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      230 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6464 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      244 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0      639 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6602 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      176 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6481 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      171 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0      345 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0      434 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6419 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6447 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6457 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      196 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6425 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      263 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6438 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      182 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6490 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      206 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6455 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      209 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6464 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      250 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      303 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6425 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      311 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      188 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0      865 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2533 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5069 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/user.py
+-rw-r--r--   0        0        0     1901 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       68 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3346 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       25 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/py.typed
+-rw-r--r--   0        0        0      984 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/types.py
+-rw-r--r--   0        0        0     1058 2023-04-17 17:17:05.184563 kittycad-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 kittycad-0.3.6/PKG-INFO
```

### Comparing `kittycad-0.3.5/LICENSE` & `kittycad-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/README.md` & `kittycad-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.3.6/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,129 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.mesh import Mesh
+from ...models.unit_energy_conversion import UnitEnergyConversion
 from ...models.error import Error
-from ...models.image_type import ImageType
-from ...models.file_export_format import FileExportFormat
+from ...models.unit_energy_format import UnitEnergyFormat
+from ...models.unit_energy_format import UnitEnergyFormat
 from ...types import Response
 
 def _get_kwargs(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
+	output_format: UnitEnergyFormat,
+	src_format: UnitEnergyFormat,
+	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/ai/image-to-3d/{input_format}/{output_format}".format(client.base_url, input_format=input_format, output_format=output_format)
+	url = "{}/unit/conversion/energy/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
-		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Mesh, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = Mesh.from_dict(response.json())
+		response_200 = UnitEnergyConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Mesh, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitEnergyConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
+	output_format: UnitEnergyFormat,
+	src_format: UnitEnergyFormat,
+	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Union[Any, UnitEnergyConversion, Error]]:
 	kwargs = _get_kwargs(
-		input_format=input_format,
 		output_format=output_format,
-		body=body,
+		src_format=src_format,
+		value=value,
 		client=client,
 	)
 
-	response = httpx.post(
+	response = httpx.get(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
+	output_format: UnitEnergyFormat,
+	src_format: UnitEnergyFormat,
+	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
+	""" Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
-		input_format=input_format,
 		output_format=output_format,
-		body=body,
+		src_format=src_format,
+		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
+	output_format: UnitEnergyFormat,
+	src_format: UnitEnergyFormat,
+	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, Mesh, Error]]:
+) -> Response[Union[Any, UnitEnergyConversion, Error]]:
 	kwargs = _get_kwargs(
-		input_format=input_format,
 		output_format=output_format,
-		body=body,
+		src_format=src_format,
+		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	input_format: ImageType,
-	output_format: FileExportFormat,
-	body: bytes,
+	output_format: UnitEnergyFormat,
+	src_format: UnitEnergyFormat,
+	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, Mesh, Error]]:
+) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
+	""" Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
-		input_format=input_format,
 		output_format=output_format,
-		body=body,
+		src_format=src_format,
+		value=value,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.3.6/kittycad/api/ai/create_image_to_3d.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
 from ...models.mesh import Mesh
 from ...models.error import Error
+from ...models.image_type import ImageType
 from ...models.file_export_format import FileExportFormat
 from ...types import Response
 
 def _get_kwargs(
+	input_format: ImageType,
 	output_format: FileExportFormat,
-	prompt: str,
+	body: bytes,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/ai/text-to-3d/{output_format}?prompt={prompt}".format(client.base_url, output_format=output_format, prompt=prompt)
+	url = "{}/ai/image-to-3d/{input_format}/{output_format}".format(client.base_url, input_format=input_format, output_format=output_format)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
+		"content": body,
 	}
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Mesh, Error]]:
 	if response.status_code == 200:
 		response_200 = Mesh.from_dict(response.json())
 		return response_200
@@ -46,72 +49,82 @@
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
+	input_format: ImageType,
 	output_format: FileExportFormat,
-	prompt: str,
+	body: bytes,
 	*,
 	client: Client,
 ) -> Response[Union[Any, Mesh, Error]]:
 	kwargs = _get_kwargs(
+		input_format=input_format,
 		output_format=output_format,
-		prompt=prompt,
+		body=body,
 		client=client,
 	)
 
 	response = httpx.post(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
+	input_format: ImageType,
 	output_format: FileExportFormat,
-	prompt: str,
+	body: bytes,
 	*,
 	client: Client,
 ) -> Optional[Union[Any, Mesh, Error]]:
+	""" This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better. """
 
 	return sync_detailed(
+		input_format=input_format,
 		output_format=output_format,
-		prompt=prompt,
+		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
+	input_format: ImageType,
 	output_format: FileExportFormat,
-	prompt: str,
+	body: bytes,
 	*,
 	client: Client,
 ) -> Response[Union[Any, Mesh, Error]]:
 	kwargs = _get_kwargs(
+		input_format=input_format,
 		output_format=output_format,
-		prompt=prompt,
+		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.post(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
+	input_format: ImageType,
 	output_format: FileExportFormat,
-	prompt: str,
+	body: bytes,
 	*,
 	client: Client,
 ) -> Optional[Union[Any, Mesh, Error]]:
+	""" This is an alpha endpoint. It will change in the future. The current output is honestly pretty bad. So if you find this endpoint, you get what you pay for, which currently is nothing. But in the future will be made a lot better. """
 
 	return (
 		await asyncio_detailed(
+		input_format=input_format,
 		output_format=output_format,
-		prompt=prompt,
+		body=body,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.3.6/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.3.6/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.3.6/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.3.6/kittycad/api/api_calls/get_async_operation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
 from ...models.file_conversion import FileConversion
 from ...models.file2_d_vector_conversion import File2DVectorConversion
-from ...models.file3_d_conversion import File3DConversion
 from ...models.file_center_of_mass import FileCenterOfMass
 from ...models.file_mass import FileMass
 from ...models.file_volume import FileVolume
 from ...models.file_density import FileDensity
 from ...models.file_surface_area import FileSurfaceArea
 from ...models.error import Error
 from ...types import Response
@@ -28,15 +27,15 @@
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	if response.status_code == 200:
 		data = response.json()
 		try:
 			if not isinstance(data, dict):
 				raise TypeError()
 			option = FileConversion.from_dict(data)
 			return option
@@ -48,21 +47,14 @@
 			option = File2DVectorConversion.from_dict(data)
 			return option
 		except:
 			pass
 		try:
 			if not isinstance(data, dict):
 				raise TypeError()
-			option = File3DConversion.from_dict(data)
-			return option
-		except:
-			pass
-		try:
-			if not isinstance(data, dict):
-				raise TypeError()
 			option = FileCenterOfMass.from_dict(data)
 			return option
 		except:
 			pass
 		try:
 			if not isinstance(data, dict):
 				raise TypeError()
@@ -96,28 +88,28 @@
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
 	id: str,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+) -> Response[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	kwargs = _get_kwargs(
 		id=id,
 		client=client,
 	)
 
 	response = httpx.get(
 		verify=client.verify_ssl,
@@ -127,15 +119,15 @@
 	return _build_response(response=response)
 
 
 def sync(
 	id: str,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+) -> Optional[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	""" Get the status and output of an async operation.
 This endpoint requires authentication by any KittyCAD user. It returns details of the requested async operation for the user.
 If the user is not authenticated to view the specified async operation, then it is not returned.
 Only KittyCAD employees with the proper access can view async operations for other users. """
 
 	return sync_detailed(
 		id=id,
@@ -143,15 +135,15 @@
 	).parsed
 
 
 async def asyncio_detailed(
 	id: str,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+) -> Response[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	kwargs = _get_kwargs(
 		id=id,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
@@ -159,15 +151,15 @@
 	return _build_response(response=response)
 
 
 async def asyncio(
 	id: str,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileConversion, File2DVectorConversion, File3DConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
+) -> Optional[Union[Any, FileConversion, File2DVectorConversion, FileCenterOfMass, FileMass, FileVolume, FileDensity, FileSurfaceArea, Error]]:
 	""" Get the status and output of an async operation.
 This endpoint requires authentication by any KittyCAD user. It returns details of the requested async operation for the user.
 If the user is not authenticated to view the specified async operation, then it is not returned.
 Only KittyCAD employees with the proper access can view async operations for other users. """
 
 	return (
 		await asyncio_detailed(
```

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.3.6/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.3.6/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.3.6/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.3.6/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.3.6/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.3.6/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.3.6/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.3.6/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.3.6/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.3.6/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.3.6/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.3.6/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_2d_vector_conversion.py` & `kittycad-0.3.6/kittycad/api/file/create_file_2d_vector_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_3d_conversion.py` & `kittycad-0.3.6/kittycad/api/file/create_file_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.file3_d_conversion import File3DConversion
+from ...models.file_conversion import FileConversion
 from ...models.error import Error
-from ...models.file3_d_export_format import File3DExportFormat
-from ...models.file3_d_import_format import File3DImportFormat
+from ...models.file_export_format import FileExportFormat
+from ...models.file_import_format import FileImportFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: File3DExportFormat,
-	src_format: File3DImportFormat,
+	output_format: FileExportFormat,
+	src_format: FileImportFormat,
 	body: bytes,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/3d/conversion/{src_format}/{output_format}".format(client.base_url, output_format=output_format, src_format=src_format)
+	url = "{}/file/conversion/{src_format}/{output_format}".format(client.base_url, output_format=output_format, src_format=src_format)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, File3DConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileConversion, Error]]:
 	if response.status_code == 201:
-		response_201 = File3DConversion.from_dict(response.json())
+		response_201 = FileConversion.from_dict(response.json())
 		return response_201
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, File3DConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: File3DExportFormat,
-	src_format: File3DImportFormat,
+	output_format: FileExportFormat,
+	src_format: FileImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, File3DConversion, Error]]:
+) -> Response[Union[Any, FileConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
@@ -71,60 +71,60 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: File3DExportFormat,
-	src_format: File3DImportFormat,
+	output_format: FileExportFormat,
+	src_format: FileImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, File3DConversion, Error]]:
-	""" Convert a 3D file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[Any, FileConversion, Error]]:
+	""" Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
 If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: File3DExportFormat,
-	src_format: File3DImportFormat,
+	output_format: FileExportFormat,
+	src_format: FileImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, File3DConversion, Error]]:
+) -> Response[Union[Any, FileConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.post(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: File3DExportFormat,
-	src_format: File3DImportFormat,
+	output_format: FileExportFormat,
+	src_format: FileImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, File3DConversion, Error]]:
-	""" Convert a 3D file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[Any, FileConversion, Error]]:
+	""" Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
 If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
```

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.3.6/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_conversion.py` & `kittycad-0.3.6/kittycad/api/file/create_file_mass.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,134 +1,131 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.file_conversion import FileConversion
+from ...models.file_mass import FileMass
 from ...models.error import Error
-from ...models.file_export_format import FileExportFormat
-from ...models.file_import_format import FileImportFormat
+from ...models.file3_d_import_format import File3DImportFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: FileExportFormat,
-	src_format: FileImportFormat,
+	material_density: float,
+	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/conversion/{src_format}/{output_format}".format(client.base_url, output_format=output_format, src_format=src_format)
+	url = "{}/file/mass?material_density={material_density}&src_format={src_format}".format(client.base_url, material_density=material_density, src_format=src_format)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileMass, Error]]:
 	if response.status_code == 201:
-		response_201 = FileConversion.from_dict(response.json())
+		response_201 = FileMass.from_dict(response.json())
 		return response_201
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileMass, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: FileExportFormat,
-	src_format: FileImportFormat,
+	material_density: float,
+	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileConversion, Error]]:
+) -> Response[Union[Any, FileMass, Error]]:
 	kwargs = _get_kwargs(
-		output_format=output_format,
+		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
 	response = httpx.post(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: FileExportFormat,
-	src_format: FileImportFormat,
+	material_density: float,
+	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileConversion, Error]]:
-	""" Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
-If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
+) -> Optional[Union[Any, FileMass, Error]]:
+	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return sync_detailed(
-		output_format=output_format,
+		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: FileExportFormat,
-	src_format: FileImportFormat,
+	material_density: float,
+	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileConversion, Error]]:
+) -> Response[Union[Any, FileMass, Error]]:
 	kwargs = _get_kwargs(
-		output_format=output_format,
+		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.post(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: FileExportFormat,
-	src_format: FileImportFormat,
+	material_density: float,
+	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileConversion, Error]]:
-	""" Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
-If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
+) -> Optional[Union[Any, FileMass, Error]]:
+	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return (
 		await asyncio_detailed(
-		output_format=output_format,
+		material_density=material_density,
 		src_format=src_format,
 		body=body,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.3.6/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_density.py` & `kittycad-0.3.6/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_execution.py` & `kittycad-0.3.6/kittycad/api/file/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_mass.py` & `kittycad-0.3.6/kittycad/api/file/create_file_volume.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,122 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.file_mass import FileMass
+from ...models.file_volume import FileVolume
 from ...models.error import Error
 from ...models.file3_d_import_format import File3DImportFormat
 from ...types import Response
 
 def _get_kwargs(
-	material_density: float,
 	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/mass?material_density={material_density}&src_format={src_format}".format(client.base_url, material_density=material_density, src_format=src_format)
+	url = "{}/file/volume?src_format={src_format}".format(client.base_url, src_format=src_format)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileMass, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileVolume, Error]]:
 	if response.status_code == 201:
-		response_201 = FileMass.from_dict(response.json())
+		response_201 = FileVolume.from_dict(response.json())
 		return response_201
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileMass, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileVolume, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	material_density: float,
 	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
+) -> Response[Union[Any, FileVolume, Error]]:
 	kwargs = _get_kwargs(
-		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
 	response = httpx.post(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	material_density: float,
 	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
-	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[Any, FileVolume, Error]]:
+	""" Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return sync_detailed(
-		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	material_density: float,
 	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileMass, Error]]:
+) -> Response[Union[Any, FileVolume, Error]]:
 	kwargs = _get_kwargs(
-		material_density=material_density,
 		src_format=src_format,
 		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.post(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	material_density: float,
 	src_format: File3DImportFormat,
 	body: bytes,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileMass, Error]]:
-	""" Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[Any, FileVolume, Error]]:
+	""" Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
 If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
 
 	return (
 		await asyncio_detailed(
-		material_density=material_density,
 		src_format=src_format,
 		body=body,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.3.6/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/file/create_file_volume.py` & `kittycad-0.3.6/kittycad/api/users/get_user_extended.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,113 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.file_volume import FileVolume
+from ...models.extended_user import ExtendedUser
 from ...models.error import Error
-from ...models.file3_d_import_format import File3DImportFormat
 from ...types import Response
 
 def _get_kwargs(
-	src_format: File3DImportFormat,
-	body: bytes,
+	id: str,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/file/volume?src_format={src_format}".format(client.base_url, src_format=src_format)
+	url = "{}/users-extended/{id}".format(client.base_url, id=id)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
-		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, FileVolume, Error]]:
-	if response.status_code == 201:
-		response_201 = FileVolume.from_dict(response.json())
-		return response_201
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ExtendedUser, Error]]:
+	if response.status_code == 200:
+		response_200 = ExtendedUser.from_dict(response.json())
+		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, FileVolume, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, ExtendedUser, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	src_format: File3DImportFormat,
-	body: bytes,
+	id: str,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileVolume, Error]]:
+) -> Response[Union[Any, ExtendedUser, Error]]:
 	kwargs = _get_kwargs(
-		src_format=src_format,
-		body=body,
+		id=id,
 		client=client,
 	)
 
-	response = httpx.post(
+	response = httpx.get(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	src_format: File3DImportFormat,
-	body: bytes,
+	id: str,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileVolume, Error]]:
-	""" Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+	""" To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
+To get information about any KittyCAD user, you must be a KittyCAD employee. """
 
 	return sync_detailed(
-		src_format=src_format,
-		body=body,
+		id=id,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	src_format: File3DImportFormat,
-	body: bytes,
+	id: str,
 	*,
 	client: Client,
-) -> Response[Union[Any, FileVolume, Error]]:
+) -> Response[Union[Any, ExtendedUser, Error]]:
 	kwargs = _get_kwargs(
-		src_format=src_format,
-		body=body,
+		id=id,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.post(**kwargs)
+		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	src_format: File3DImportFormat,
-	body: bytes,
+	id: str,
 	*,
 	client: Client,
-) -> Optional[Union[Any, FileVolume, Error]]:
-	""" Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint. """
+) -> Optional[Union[Any, ExtendedUser, Error]]:
+	""" To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
+Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
+To get information about any KittyCAD user, you must be a KittyCAD employee. """
 
 	return (
 		await asyncio_detailed(
-		src_format=src_format,
-		body=body,
+		id=id,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.3.6/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/hidden/auth_email.py` & `kittycad-0.3.6/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.3.6/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/hidden/logout.py` & `kittycad-0.3.6/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.3.6/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/meta/get_metadata.py` & `kittycad-0.3.6/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/meta/get_schema.py` & `kittycad-0.3.6/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/meta/ping.py` & `kittycad-0.3.6/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.3.6/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/sessions/get_session_for_user.py` & `kittycad-0.3.6/kittycad/api/sessions/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_energy_conversion import UnitEnergyConversion
+from ...models.unit_metric_power_cubed_conversion import UnitMetricPowerCubedConversion
 from ...models.error import Error
-from ...models.unit_energy_format import UnitEnergyFormat
-from ...models.unit_energy_format import UnitEnergyFormat
+from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_metric_power import UnitMetricPower
 from ...types import Response
 
 def _get_kwargs(
-	output_format: UnitEnergyFormat,
-	src_format: UnitEnergyFormat,
+	output_format: UnitMetricPower,
+	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/energy/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/metric/cubed/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitEnergyConversion.from_dict(response.json())
+		response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: UnitEnergyFormat,
-	src_format: UnitEnergyFormat,
+	output_format: UnitMetricPower,
+	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -70,58 +70,58 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitEnergyFormat,
-	src_format: UnitEnergyFormat,
+	output_format: UnitMetricPower,
+	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
-	""" Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitEnergyFormat,
-	src_format: UnitEnergyFormat,
+	output_format: UnitMetricPower,
+	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitEnergyConversion, Error]]:
+) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitEnergyFormat,
-	src_format: UnitEnergyFormat,
+	output_format: UnitMetricPower,
+	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitEnergyConversion, Error]]:
-	""" Convert a energy unit value to another energy unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_metric_power_cubed_conversion import UnitMetricPowerCubedConversion
+from ...models.unit_metric_power_conversion import UnitMetricPowerConversion
 from ...models.error import Error
 from ...models.unit_metric_power import UnitMetricPower
 from ...models.unit_metric_power import UnitMetricPower
 from ...types import Response
 
 def _get_kwargs(
 	output_format: UnitMetricPower,
 	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/metric/cubed/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/metric/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitMetricPowerCubedConversion.from_dict(response.json())
+		response_200 = UnitMetricPowerConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
 	output_format: UnitMetricPower,
 	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -75,16 +75,16 @@
 
 def sync(
 	output_format: UnitMetricPower,
 	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
@@ -92,15 +92,15 @@
 
 async def asyncio_detailed(
 	output_format: UnitMetricPower,
 	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitMetricPowerCubedConversion, Error]]:
+) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -112,16 +112,16 @@
 
 async def asyncio(
 	output_format: UnitMetricPower,
 	src_format: UnitMetricPower,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerCubedConversion, Error]]:
-	""" Convert a metric cubed unit value to another metric cubed unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_metric_power_conversion import UnitMetricPowerConversion
+from ...models.unit_power_conversion import UnitPowerConversion
 from ...models.error import Error
-from ...models.unit_metric_power import UnitMetricPower
-from ...models.unit_metric_power import UnitMetricPower
+from ...models.unit_power_format import UnitPowerFormat
+from ...models.unit_power_format import UnitPowerFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
+	output_format: UnitPowerFormat,
+	src_format: UnitPowerFormat,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/metric/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPowerConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitMetricPowerConversion.from_dict(response.json())
+		response_200 = UnitPowerConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPowerConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
+	output_format: UnitPowerFormat,
+	src_format: UnitPowerFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Response[Union[Any, UnitPowerConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -70,58 +70,58 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
+	output_format: UnitPowerFormat,
+	src_format: UnitPowerFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
-	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
+	output_format: UnitPowerFormat,
+	src_format: UnitPowerFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitMetricPowerConversion, Error]]:
+) -> Response[Union[Any, UnitPowerConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitMetricPower,
-	src_format: UnitMetricPower,
+	output_format: UnitPowerFormat,
+	src_format: UnitPowerFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitMetricPowerConversion, Error]]:
-	""" Convert a metric unit value to another metric unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_power_conversion import UnitPowerConversion
+from ...models.unit_pressure_conversion import UnitPressureConversion
 from ...models.error import Error
-from ...models.unit_power_format import UnitPowerFormat
-from ...models.unit_power_format import UnitPowerFormat
+from ...models.unit_pressure_format import UnitPressureFormat
+from ...models.unit_pressure_format import UnitPressureFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
+	output_format: UnitPressureFormat,
+	src_format: UnitPressureFormat,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/power/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/pressure/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPowerConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPressureConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitPowerConversion.from_dict(response.json())
+		response_200 = UnitPressureConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPowerConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPressureConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
+	output_format: UnitPressureFormat,
+	src_format: UnitPressureFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitPowerConversion, Error]]:
+) -> Response[Union[Any, UnitPressureConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -70,58 +70,58 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
+	output_format: UnitPressureFormat,
+	src_format: UnitPressureFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitPowerConversion, Error]]:
-	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
+	output_format: UnitPressureFormat,
+	src_format: UnitPressureFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitPowerConversion, Error]]:
+) -> Response[Union[Any, UnitPressureConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitPowerFormat,
-	src_format: UnitPowerFormat,
+	output_format: UnitPressureFormat,
+	src_format: UnitPressureFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitPowerConversion, Error]]:
-	""" Convert a power unit value to another power unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_pressure_conversion import UnitPressureConversion
+from ...models.unit_voltage_conversion import UnitVoltageConversion
 from ...models.error import Error
-from ...models.unit_pressure_format import UnitPressureFormat
-from ...models.unit_pressure_format import UnitPressureFormat
+from ...models.unit_voltage_format import UnitVoltageFormat
+from ...models.unit_voltage_format import UnitVoltageFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
+	output_format: UnitVoltageFormat,
+	src_format: UnitVoltageFormat,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/pressure/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/voltage/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitPressureConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitPressureConversion.from_dict(response.json())
+		response_200 = UnitVoltageConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitPressureConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitVoltageConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
+	output_format: UnitVoltageFormat,
+	src_format: UnitVoltageFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
+) -> Response[Union[Any, UnitVoltageConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -70,58 +70,58 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
+	output_format: UnitVoltageFormat,
+	src_format: UnitVoltageFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
-	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+	""" Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
+	output_format: UnitVoltageFormat,
+	src_format: UnitVoltageFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitPressureConversion, Error]]:
+) -> Response[Union[Any, UnitVoltageConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitPressureFormat,
-	src_format: UnitPressureFormat,
+	output_format: UnitVoltageFormat,
+	src_format: UnitVoltageFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitPressureConversion, Error]]:
-	""" Convert a pressure unit value to another pressure unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+	""" Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_time_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/unit/get_voltage_unit_conversion.py` & `kittycad-0.3.6/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.unit_voltage_conversion import UnitVoltageConversion
+from ...models.unit_volume_conversion import UnitVolumeConversion
 from ...models.error import Error
-from ...models.unit_voltage_format import UnitVoltageFormat
-from ...models.unit_voltage_format import UnitVoltageFormat
+from ...models.unit_volume_format import UnitVolumeFormat
+from ...models.unit_volume_format import UnitVolumeFormat
 from ...types import Response
 
 def _get_kwargs(
-	output_format: UnitVoltageFormat,
-	src_format: UnitVoltageFormat,
+	output_format: UnitVolumeFormat,
+	src_format: UnitVolumeFormat,
 	value: float,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/unit/conversion/voltage/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
+	url = "{}/unit/conversion/volume/{src_format}/{output_format}?value={value}".format(client.base_url, output_format=output_format, src_format=src_format, value=value)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
 	if response.status_code == 200:
-		response_200 = UnitVoltageConversion.from_dict(response.json())
+		response_200 = UnitVolumeConversion.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, UnitVolumeConversion, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	output_format: UnitVoltageFormat,
-	src_format: UnitVoltageFormat,
+	output_format: UnitVolumeFormat,
+	src_format: UnitVolumeFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+) -> Response[Union[Any, UnitVolumeConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
@@ -70,58 +70,58 @@
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	output_format: UnitVoltageFormat,
-	src_format: UnitVoltageFormat,
+	output_format: UnitVolumeFormat,
+	src_format: UnitVolumeFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
-	""" Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
+	""" Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions. """
 
 	return sync_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	output_format: UnitVoltageFormat,
-	src_format: UnitVoltageFormat,
+	output_format: UnitVolumeFormat,
+	src_format: UnitVolumeFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Response[Union[Any, UnitVoltageConversion, Error]]:
+) -> Response[Union[Any, UnitVolumeConversion, Error]]:
 	kwargs = _get_kwargs(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
 		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	output_format: UnitVoltageFormat,
-	src_format: UnitVoltageFormat,
+	output_format: UnitVolumeFormat,
+	src_format: UnitVolumeFormat,
 	value: float,
 	*,
 	client: Client,
-) -> Optional[Union[Any, UnitVoltageConversion, Error]]:
-	""" Convert a voltage unit value to another voltage unit value. This is a nice endpoint to use for helper functions. """
+) -> Optional[Union[Any, UnitVolumeConversion, Error]]:
+	""" Convert a volume unit value to another volume unit value. This is a nice endpoint to use for helper functions. """
 
 	return (
 		await asyncio_detailed(
 		output_format=output_format,
 		src_format=src_format,
 		value=value,
 			client=client,
```

### Comparing `kittycad-0.3.5/kittycad/api/users/delete_user_self.py` & `kittycad-0.3.6/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user.py` & `kittycad-0.3.6/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user_extended.py` & `kittycad-0.3.6/kittycad/api/users/update_user_self.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,111 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.extended_user import ExtendedUser
+from ...models.user import User
 from ...models.error import Error
+from ...models.update_user import UpdateUser
 from ...types import Response
 
 def _get_kwargs(
-	id: str,
+	body: UpdateUser,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/users-extended/{id}".format(client.base_url, id=id)
+	url = "{}/user".format(client.base_url)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
+		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ExtendedUser, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
 	if response.status_code == 200:
-		response_200 = ExtendedUser.from_dict(response.json())
+		response_200 = User.from_dict(response.json())
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ExtendedUser, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	id: str,
+	body: UpdateUser,
 	*,
 	client: Client,
-) -> Response[Union[Any, ExtendedUser, Error]]:
+) -> Response[Union[Any, User, Error]]:
 	kwargs = _get_kwargs(
-		id=id,
+		body=body,
 		client=client,
 	)
 
-	response = httpx.get(
+	response = httpx.put(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	id: str,
+	body: UpdateUser,
 	*,
 	client: Client,
-) -> Optional[Union[Any, ExtendedUser, Error]]:
-	""" To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
-Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
-To get information about any KittyCAD user, you must be a KittyCAD employee. """
+) -> Optional[Union[Any, User, Error]]:
+	""" This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user. """
 
 	return sync_detailed(
-		id=id,
+		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	id: str,
+	body: UpdateUser,
 	*,
 	client: Client,
-) -> Response[Union[Any, ExtendedUser, Error]]:
+) -> Response[Union[Any, User, Error]]:
 	kwargs = _get_kwargs(
-		id=id,
+		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.get(**kwargs)
+		response = await _client.put(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	id: str,
+	body: UpdateUser,
 	*,
 	client: Client,
-) -> Optional[Union[Any, ExtendedUser, Error]]:
-	""" To get information about yourself, use `/users-extended/me` as the endpoint. By doing so you will get the user information for the authenticated user.
-Alternatively, to get information about the authenticated user, use `/user/extended` endpoint.
-To get information about any KittyCAD user, you must be a KittyCAD employee. """
+) -> Optional[Union[Any, User, Error]]:
+	""" This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user. """
 
 	return (
 		await asyncio_detailed(
-		id=id,
+		body=body,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.3.6/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.3.6/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user_self.py` & `kittycad-0.3.6/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.3.6/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/list_users.py` & `kittycad-0.3.6/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/list_users_extended.py` & `kittycad-0.3.6/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/api/users/update_user_self.py` & `kittycad-0.3.6/kittycad/api/meta/get_openai_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,100 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import Client
-from ...models.user import User
+from ...models.dict import dict
 from ...models.error import Error
-from ...models.update_user import UpdateUser
 from ...types import Response
 
 def _get_kwargs(
-	body: UpdateUser,
 	*,
 	client: Client,
 ) -> Dict[str, Any]:
-	url = "{}/user".format(client.base_url)
+	url = "{}/openai/openapi.json".format(client.base_url)
 
 	headers: Dict[str, Any] = client.get_headers()
 	cookies: Dict[str, Any] = client.get_cookies()
 
 	return {
 		"url": url,
 		"headers": headers,
 		"cookies": cookies,
 		"timeout": client.get_timeout(),
-		"content": body,
 	}
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, User, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, dict, Error]]:
 	if response.status_code == 200:
-		response_200 = User.from_dict(response.json())
+		response_200 = response.json()
 		return response_200
 	if response.status_code == 400:
 		response_4XX = Error.from_dict(response.json())
 		return response_4XX
 	if response.status_code == 500:
 		response_5XX = Error.from_dict(response.json())
 		return response_5XX
 	return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, User, Error]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, dict, Error]]:
 	return Response(
 		status_code=response.status_code,
 		content=response.content,
 		headers=response.headers,
 		parsed=_parse_response(response=response),
 	)
 
 
 def sync_detailed(
-	body: UpdateUser,
 	*,
 	client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Union[Any, dict, Error]]:
 	kwargs = _get_kwargs(
-		body=body,
 		client=client,
 	)
 
-	response = httpx.put(
+	response = httpx.get(
 		verify=client.verify_ssl,
 		**kwargs,
 	)
 
 	return _build_response(response=response)
 
 
 def sync(
-	body: UpdateUser,
 	*,
 	client: Client,
-) -> Optional[Union[Any, User, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user. """
+) -> Optional[Union[Any, dict, Error]]:
+	""" This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars. """
 
 	return sync_detailed(
-		body=body,
 		client=client,
 	).parsed
 
 
 async def asyncio_detailed(
-	body: UpdateUser,
 	*,
 	client: Client,
-) -> Response[Union[Any, User, Error]]:
+) -> Response[Union[Any, dict, Error]]:
 	kwargs = _get_kwargs(
-		body=body,
 		client=client,
 	)
 
 	async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-		response = await _client.put(**kwargs)
+		response = await _client.get(**kwargs)
 
 	return _build_response(response=response)
 
 
 async def asyncio(
-	body: UpdateUser,
 	*,
 	client: Client,
-) -> Optional[Union[Any, User, Error]]:
-	""" This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user. """
+) -> Optional[Union[Any, dict, Error]]:
+	""" This is the same as the OpenAPI schema, BUT it has some modifications to make it compatible with OpenAI. For example, descriptions must be < 300 chars. """
 
 	return (
 		await asyncio_detailed(
-		body=body,
 			client=client,
 		)
 	).parsed
```

### Comparing `kittycad-0.3.5/kittycad/client.py` & `kittycad-0.3.6/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/client_test.py` & `kittycad-0.3.6/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/__init__.py` & `kittycad-0.3.6/kittycad/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,14 @@
 from .error import Error
 from .executor_metadata import ExecutorMetadata
 from .extended_user import ExtendedUser
 from .extended_user_results_page import ExtendedUserResultsPage
 from .file2_d_vector_conversion import File2DVectorConversion
 from .file2_d_vector_export_format import File2DVectorExportFormat
 from .file2_d_vector_import_format import File2DVectorImportFormat
-from .file3_d_conversion import File3DConversion
-from .file3_d_export_format import File3DExportFormat
 from .file3_d_import_format import File3DImportFormat
 from .file_center_of_mass import FileCenterOfMass
 from .file_conversion import FileConversion
 from .file_density import FileDensity
 from .file_export_format import FileExportFormat
 from .file_import_format import FileImportFormat
 from .file_mass import FileMass
```

### Comparing `kittycad-0.3.5/kittycad/models/ai_plugin_api.py` & `kittycad-0.3.6/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/ai_plugin_auth.py` & `kittycad-0.3.6/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.3.6/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/api_call_query_group.py` & `kittycad-0.3.6/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/api_call_with_price.py` & `kittycad-0.3.6/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.3.6/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/api_token.py` & `kittycad-0.3.6/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/api_token_results_page.py` & `kittycad-0.3.6/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/app_client_info.py` & `kittycad-0.3.6/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/async_api_call.py` & `kittycad-0.3.6/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/async_api_call_results_page.py` & `kittycad-0.3.6/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/billing_info.py` & `kittycad-0.3.6/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/cache_metadata.py` & `kittycad-0.3.6/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/card_details.py` & `kittycad-0.3.6/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/cluster.py` & `kittycad-0.3.6/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/code_output.py` & `kittycad-0.3.6/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/commit.py` & `kittycad-0.3.6/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/connection.py` & `kittycad-0.3.6/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/country_code.py` & `kittycad-0.3.6/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/currency.py` & `kittycad-0.3.6/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/customer.py` & `kittycad-0.3.6/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/customer_balance.py` & `kittycad-0.3.6/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/device_access_token_request_form.py` & `kittycad-0.3.6/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/device_auth_request_form.py` & `kittycad-0.3.6/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/device_auth_verify_params.py` & `kittycad-0.3.6/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/docker_system_info.py` & `kittycad-0.3.6/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/email_authentication_form.py` & `kittycad-0.3.6/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/engine_metadata.py` & `kittycad-0.3.6/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/error.py` & `kittycad-0.3.6/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/executor_metadata.py` & `kittycad-0.3.6/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/extended_user.py` & `kittycad-0.3.6/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/extended_user_results_page.py` & `kittycad-0.3.6/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file2_d_vector_conversion.py` & `kittycad-0.3.6/kittycad/models/file2_d_vector_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file3_d_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_power_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
-from ..models.file3_d_export_format import File3DExportFormat
-from ..models.file3_d_import_format import File3DImportFormat
+from ..models.unit_power_format import UnitPowerFormat
 from ..models.api_call_status import ApiCallStatus
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="File3DConversion")
+T = TypeVar("T", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class File3DConversion:
+class UnitPowerConversion:
     """ """
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    output: Union[Unset, str] = UNSET
-    output_format: Union[Unset, File3DExportFormat] = UNSET
-    src_format: Union[Unset, File3DImportFormat] = UNSET
+    input: Union[Unset, float] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_format: Union[Unset, UnitPowerFormat] = UNSET
+    src_format: Union[Unset, UnitPowerFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -35,14 +35,15 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        input = self.input
         output = self.output
         output_format: Union[Unset, str] = UNSET
         if not isinstance(self.output_format, Unset):
             output_format = self.output_format.value
         src_format: Union[Unset, str] = UNSET
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format.value
@@ -64,14 +65,16 @@
             field_dict['completed_at'] = completed_at
         if created_at is not UNSET:
             field_dict['created_at'] = created_at
         if error is not UNSET:
             field_dict['error'] = error
         if id is not UNSET:
             field_dict['id'] = id
+        if input is not UNSET:
+            field_dict['input'] = input
         if output is not UNSET:
             field_dict['output'] = output
         if output_format is not UNSET:
             field_dict['output_format'] = output_format
         if src_format is not UNSET:
             field_dict['src_format'] = src_format
         if started_at is not UNSET:
@@ -102,29 +105,31 @@
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
         id = d.pop("id", UNSET)
 
+        input = d.pop("input", UNSET)
+
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, File3DExportFormat]
+        output_format: Union[Unset, UnitPowerFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = File3DExportFormat(_output_format)
+            output_format = UnitPowerFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, File3DImportFormat]
+        src_format: Union[Unset, UnitPowerFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = File3DImportFormat(_src_format)
+            src_format = UnitPowerFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -141,30 +146,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file3_d_conversion = cls(
+        unit_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
+            input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file3_d_conversion.additional_properties = d
-        return file3_d_conversion
+        unit_power_conversion.additional_properties = d
+        return unit_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.5/kittycad/models/file_center_of_mass.py` & `kittycad-0.3.6/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_conversion.py` & `kittycad-0.3.6/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_density.py` & `kittycad-0.3.6/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_mass.py` & `kittycad-0.3.6/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_surface_area.py` & `kittycad-0.3.6/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_system_metadata.py` & `kittycad-0.3.6/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/file_volume.py` & `kittycad-0.3.6/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/gateway.py` & `kittycad-0.3.6/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/index_info.py` & `kittycad-0.3.6/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/invoice.py` & `kittycad-0.3.6/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/invoice_line_item.py` & `kittycad-0.3.6/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/jetstream.py` & `kittycad-0.3.6/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/jetstream_api_stats.py` & `kittycad-0.3.6/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/jetstream_config.py` & `kittycad-0.3.6/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/jetstream_stats.py` & `kittycad-0.3.6/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/leaf_node.py` & `kittycad-0.3.6/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/mesh.py` & `kittycad-0.3.6/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/meta_cluster_info.py` & `kittycad-0.3.6/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/metadata.py` & `kittycad-0.3.6/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/new_address.py` & `kittycad-0.3.6/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/o_auth2_client_info.py` & `kittycad-0.3.6/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/onboarding.py` & `kittycad-0.3.6/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/output_file.py` & `kittycad-0.3.6/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/payment_intent.py` & `kittycad-0.3.6/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/payment_method.py` & `kittycad-0.3.6/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/payment_method_card_checks.py` & `kittycad-0.3.6/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/physics_constant.py` & `kittycad-0.3.6/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/physics_constant_name.py` & `kittycad-0.3.6/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/plugins_info.py` & `kittycad-0.3.6/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/point_e_metadata.py` & `kittycad-0.3.6/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/pong.py` & `kittycad-0.3.6/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/registry_service_config.py` & `kittycad-0.3.6/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/runtime.py` & `kittycad-0.3.6/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/session.py` & `kittycad-0.3.6/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.3.6/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_acceleration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_angle_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_area_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_charge_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_charge_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_concentration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_data_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_data_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_density_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_density_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_density_format.py` & `kittycad-0.3.6/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_energy_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_force_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_illuminance_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_length_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_length_format.py` & `kittycad-0.3.6/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_mass_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_metric_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_power_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_volume_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
-from ..models.unit_power_format import UnitPowerFormat
+from ..models.unit_volume_format import UnitVolumeFormat
 from ..models.api_call_status import ApiCallStatus
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitPowerConversion")
+T = TypeVar("T", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPowerConversion:
+class UnitVolumeConversion:
     """ """
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitPowerFormat] = UNSET
-    src_format: Union[Unset, UnitPowerFormat] = UNSET
+    output_format: Union[Unset, UnitVolumeFormat] = UNSET
+    src_format: Union[Unset, UnitVolumeFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -110,26 +110,26 @@
         id = d.pop("id", UNSET)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitPowerFormat]
+        output_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitPowerFormat(_output_format)
+            output_format = UnitVolumeFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitPowerFormat]
+        src_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitPowerFormat(_src_format)
+            src_format = UnitVolumeFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -146,31 +146,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_power_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_power_conversion.additional_properties = d
-        return unit_power_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.3.5/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_radiation_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_radioactivity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_solid_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_time_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_time_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.3.6/kittycad/models/unit_voltage_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/unit_volume_format.py` & `kittycad-0.3.6/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/update_user.py` & `kittycad-0.3.6/kittycad/models/update_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/user.py` & `kittycad-0.3.6/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/user_results_page.py` & `kittycad-0.3.6/kittycad/models/user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/models/verification_token.py` & `kittycad-0.3.6/kittycad/models/verification_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/kittycad/types.py` & `kittycad-0.3.6/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.5/pyproject.toml` & `kittycad-0.3.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.3.5"
+version = "0.3.6"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
 ]
 include = ["CHANGELOG.md", "kittycad/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-httpx = ">=0.15.4,<0.24.0"
-attrs = ">=20.1.0,<23.0.0"
+httpx = ">=0.15.4,<0.25.0"
+attrs = ">=20.1.0,<24.0.0"
 python-dateutil = "^2.8.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.1"
 flake8 = "^5.0.4"
 pytest = "^7.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
```

### Comparing `kittycad-0.3.5/PKG-INFO` & `kittycad-0.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.3.5
+Version: 0.3.6
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=20.1.0,<23.0.0)
-Requires-Dist: httpx (>=0.15.4,<0.24.0)
+Requires-Dist: attrs (>=20.1.0,<24.0.0)
+Requires-Dist: httpx (>=0.15.4,<0.25.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![image](https://user-images.githubusercontent.com/19377312/165883233-3bdbc9fb-ddf9-4173-8cf2-d1b70ab7127d.png)
 
 # kittycad.py
```

