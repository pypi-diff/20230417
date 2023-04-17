# Comparing `tmp/kittycad-0.3.6.tar.gz` & `tmp/kittycad-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.3.6.tar", max compression
+gzip compressed data, was "kittycad-0.3.7.tar", max compression
```

## Comparing `kittycad-0.3.6.tar` & `kittycad-0.3.7.tar`

### file list

```diff
@@ -1,263 +1,263 @@
--rw-r--r--   0        0        0     1065 2023-04-17 17:17:05.112563 kittycad-0.3.6/LICENSE
--rw-r--r--   0        0        0      875 2023-04-17 17:17:05.112563 kittycad-0.3.6/README.md
--rw-r--r--   0        0        0       90 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/__init__.py
--rw-r--r--   0        0        0      105 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3316 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3012 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      185 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     2729 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2434 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     2725 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     4715 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     3388 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4090 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     3785 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     3495 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      338 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-17 17:17:05.176562 kittycad-0.3.6/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2629 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     3428 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      102 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2581 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2104 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      142 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      104 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2409 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      219 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4186 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_2d_vector_conversion.py
--rw-r--r--   0        0        0     3329 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     3974 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1854 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     3559 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     2643 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_execution.py
--rw-r--r--   0        0        0     3574 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3313 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3249 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1158 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      119 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2388 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     2539 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     1954 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0       91 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2305 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2280 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     1939 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     1959 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      109 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      103 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2583 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2316 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2238 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2258 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2333 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2357 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2274 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2342 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2581 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2298 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      142 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/sessions/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/sessions/get_session_for_user.py
--rw-r--r--   0        0        0       87 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3441 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3245 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3533 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3217 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     3567 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3707 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3447 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3379 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3407 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3309 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3243 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3355 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3467 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3391 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3411 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3215 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3327 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3271 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      283 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2386 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2686 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     2804 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2194 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2190 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2199 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2299 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     3257 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     3339 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2414 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     1960 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/client.py
--rw-r--r--   0        0        0     4227 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/client_test.py
--rw-r--r--   0        0        0     7730 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/__init__.py
--rw-r--r--   0        0        0      164 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2261 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      144 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2511 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      221 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      167 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4590 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1638 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      268 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      248 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8246 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2087 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3218 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_token.py
--rw-r--r--   0        0        0     1963 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1396 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5846 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0     2025 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      395 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2131 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1384 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3356 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2663 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/cluster.py
--rw-r--r--   0        0        0      171 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2193 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1574 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/commit.py
--rw-r--r--   0        0        0    14432 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/connection.py
--rw-r--r--   0        0        0     3602 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/country_code.py
--rw-r--r--   0        0        0      224 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     2337 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/currency.py
--rw-r--r--   0        0        0     4342 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/customer.py
--rw-r--r--   0        0        0     4238 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2413 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1499 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1504 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21726 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1735 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3925 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      202 2023-04-17 17:17:05.180563 kittycad-0.3.6/kittycad/models/environment.py
--rw-r--r--   0        0        0     1888 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/error.py
--rw-r--r--   0        0        0     2707 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     5849 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2019 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     6350 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_conversion.py
--rw-r--r--   0        0        0      209 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_export_format.py
--rw-r--r--   0        0        0      161 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file2_d_vector_import_format.py
--rw-r--r--   0        0        0      289 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file3_d_import_format.py
--rw-r--r--   0        0        0     5799 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6220 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5837 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_density.py
--rw-r--r--   0        0        0      315 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0      303 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5822 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5629 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5541 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2276 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/gateway.py
--rw-r--r--   0        0        0      146 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2166 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8343 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2909 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      252 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2777 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1874 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2180 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3190 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2095 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1355 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1894 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5250 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/metadata.py
--rw-r--r--   0        0        0      317 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/method.py
--rw-r--r--   0        0        0     2967 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/new_address.py
--rw-r--r--   0        0        0     1992 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      218 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2449 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1617 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1493 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3874 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2247 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      140 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5526 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     1024 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2588 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1392 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1385 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/pong.py
--rw-r--r--   0        0        0     4159 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     1773 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3573 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1681 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6477 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      285 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      300 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6520 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      334 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      333 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      177 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6490 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      286 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      199 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6537 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      307 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0      626 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      441 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      230 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6464 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      244 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0      639 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6602 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      176 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6481 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      171 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0      345 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0      434 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6419 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6447 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6457 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6386 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      196 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6425 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      263 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6438 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      182 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6490 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      206 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6455 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      209 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6464 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      250 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6373 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      303 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6425 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      311 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6412 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      188 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6399 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0      865 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2533 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5069 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/user.py
--rw-r--r--   0        0        0     1901 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       68 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3346 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       25 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/py.typed
--rw-r--r--   0        0        0      984 2023-04-17 17:17:05.184563 kittycad-0.3.6/kittycad/types.py
--rw-r--r--   0        0        0     1058 2023-04-17 17:17:05.184563 kittycad-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 kittycad-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 21:11:22.955786 kittycad-0.3.7/LICENSE
+-rw-r--r--   0        0        0      875 2023-04-17 21:11:22.955786 kittycad-0.3.7/README.md
+-rw-r--r--   0        0        0       90 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3316 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3012 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      185 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     2729 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2434 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     2725 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     4715 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     3388 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     4090 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     3785 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     3495 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      338 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2257 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2629 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     3428 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      102 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2404 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2581 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2104 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      142 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2409 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      219 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     4186 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_2d_vector_conversion.py
+-rw-r--r--   0        0        0     3329 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     3974 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1854 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     3559 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     2643 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_execution.py
+-rw-r--r--   0        0        0     3574 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     3313 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     3249 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1158 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      119 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2388 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     2539 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     1954 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0       91 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2091 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2305 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2280 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     1939 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     1959 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      109 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2583 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2316 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2238 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2258 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2333 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2357 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2274 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2342 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2581 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2298 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      142 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/sessions/__init__.py
+-rw-r--r--   0        0        0     2398 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/sessions/get_session_for_user.py
+-rw-r--r--   0        0        0       87 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3441 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3245 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3533 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3217 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3467 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     3567 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3243 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3707 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3447 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3379 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3407 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3309 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3243 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3327 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3355 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3467 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3391 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3411 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3215 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3327 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3271 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      283 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2386 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2686 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     2804 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2194 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2190 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2199 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2299 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     3257 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     3339 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2414 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     1960 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/client.py
+-rw-r--r--   0        0        0     4227 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/client_test.py
+-rw-r--r--   0        0        0     7730 2023-04-17 21:11:23.023788 kittycad-0.3.7/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2261 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      144 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2511 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      221 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      167 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4590 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1638 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      268 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      248 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8246 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2087 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3218 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     1963 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1396 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5846 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0     2025 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      395 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2131 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1384 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3356 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2663 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      171 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2193 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1574 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14432 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/connection.py
+-rw-r--r--   0        0        0     3602 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      224 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     2337 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4342 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4238 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2413 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1499 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1504 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21726 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1735 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3925 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      202 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1888 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/error.py
+-rw-r--r--   0        0        0     2707 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     5849 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2019 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     6350 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_conversion.py
+-rw-r--r--   0        0        0      191 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_export_format.py
+-rw-r--r--   0        0        0      161 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file2_d_vector_import_format.py
+-rw-r--r--   0        0        0      261 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file3_d_import_format.py
+-rw-r--r--   0        0        0     5799 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6220 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5837 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_density.py
+-rw-r--r--   0        0        0      269 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0      275 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5822 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5629 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1412 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5541 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2276 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      146 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2166 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8343 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2909 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      252 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2777 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1874 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2180 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3190 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2095 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1355 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1894 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5250 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/metadata.py
+-rw-r--r--   0        0        0      317 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/method.py
+-rw-r--r--   0        0        0     2967 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     1992 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      218 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2449 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1617 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1493 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3874 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2247 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      140 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5526 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     1024 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2588 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1392 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1385 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4159 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     1773 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3573 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1681 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6477 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      285 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      300 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6520 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      334 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      333 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      177 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6490 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      286 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      199 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6537 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      307 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6412 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0      626 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      441 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      230 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6464 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      244 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0      639 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6602 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      176 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6481 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      171 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0      345 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0      434 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6419 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6447 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6457 2023-04-17 21:11:23.027788 kittycad-0.3.7/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6386 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      196 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6425 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      263 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6438 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      182 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6490 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      206 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6455 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      209 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6464 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      250 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6373 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      303 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6425 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      311 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6412 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      188 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6399 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0      865 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2533 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5069 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/user.py
+-rw-r--r--   0        0        0     1901 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       68 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3346 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       25 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/py.typed
+-rw-r--r--   0        0        0      984 2023-04-17 21:11:23.031788 kittycad-0.3.7/kittycad/types.py
+-rw-r--r--   0        0        0     1058 2023-04-17 21:11:23.031788 kittycad-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 kittycad-0.3.7/PKG-INFO
```

### Comparing `kittycad-0.3.6/LICENSE` & `kittycad-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/README.md` & `kittycad-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.3.7/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.3.7/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.3.7/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.3.7/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.3.7/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.3.7/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.3.7/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.3.7/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.3.7/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.3.7/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.3.7/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.3.7/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.3.7/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.3.7/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.3.7/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.3.7/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.3.7/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.3.7/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_2d_vector_conversion.py` & `kittycad-0.3.7/kittycad/api/file/create_file_2d_vector_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.3.7/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_conversion.py` & `kittycad-0.3.7/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.3.7/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_density.py` & `kittycad-0.3.7/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_execution.py` & `kittycad-0.3.7/kittycad/api/file/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_mass.py` & `kittycad-0.3.7/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.3.7/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/create_file_volume.py` & `kittycad-0.3.7/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.3.7/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/hidden/auth_email.py` & `kittycad-0.3.7/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.3.7/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/hidden/logout.py` & `kittycad-0.3.7/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.3.7/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/meta/get_metadata.py` & `kittycad-0.3.7/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.3.7/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/meta/get_schema.py` & `kittycad-0.3.7/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/meta/ping.py` & `kittycad-0.3.7/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.3.7/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/sessions/get_session_for_user.py` & `kittycad-0.3.7/kittycad/api/sessions/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_time_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_voltage_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.3.7/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/delete_user_self.py` & `kittycad-0.3.7/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user.py` & `kittycad-0.3.7/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user_extended.py` & `kittycad-0.3.7/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.3.7/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.3.7/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user_self.py` & `kittycad-0.3.7/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.3.7/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/list_users.py` & `kittycad-0.3.7/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/list_users_extended.py` & `kittycad-0.3.7/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/api/users/update_user_self.py` & `kittycad-0.3.7/kittycad/api/users/update_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/client.py` & `kittycad-0.3.7/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/client_test.py` & `kittycad-0.3.7/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/__init__.py` & `kittycad-0.3.7/kittycad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/ai_plugin_api.py` & `kittycad-0.3.7/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/ai_plugin_auth.py` & `kittycad-0.3.7/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.3.7/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/api_call_query_group.py` & `kittycad-0.3.7/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/api_call_with_price.py` & `kittycad-0.3.7/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.3.7/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/api_token.py` & `kittycad-0.3.7/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/api_token_results_page.py` & `kittycad-0.3.7/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/app_client_info.py` & `kittycad-0.3.7/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/async_api_call.py` & `kittycad-0.3.7/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/async_api_call_results_page.py` & `kittycad-0.3.7/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/billing_info.py` & `kittycad-0.3.7/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/cache_metadata.py` & `kittycad-0.3.7/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/card_details.py` & `kittycad-0.3.7/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/cluster.py` & `kittycad-0.3.7/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/code_output.py` & `kittycad-0.3.7/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/commit.py` & `kittycad-0.3.7/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/connection.py` & `kittycad-0.3.7/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/country_code.py` & `kittycad-0.3.7/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/currency.py` & `kittycad-0.3.7/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/customer.py` & `kittycad-0.3.7/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/customer_balance.py` & `kittycad-0.3.7/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/device_access_token_request_form.py` & `kittycad-0.3.7/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/device_auth_request_form.py` & `kittycad-0.3.7/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/device_auth_verify_params.py` & `kittycad-0.3.7/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/docker_system_info.py` & `kittycad-0.3.7/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/email_authentication_form.py` & `kittycad-0.3.7/kittycad/models/email_authentication_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/engine_metadata.py` & `kittycad-0.3.7/kittycad/models/engine_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/error.py` & `kittycad-0.3.7/kittycad/models/error.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/executor_metadata.py` & `kittycad-0.3.7/kittycad/models/executor_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/extended_user.py` & `kittycad-0.3.7/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/extended_user_results_page.py` & `kittycad-0.3.7/kittycad/models/extended_user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file2_d_vector_conversion.py` & `kittycad-0.3.7/kittycad/models/file2_d_vector_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_center_of_mass.py` & `kittycad-0.3.7/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_conversion.py` & `kittycad-0.3.7/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_density.py` & `kittycad-0.3.7/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_mass.py` & `kittycad-0.3.7/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_surface_area.py` & `kittycad-0.3.7/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_system_metadata.py` & `kittycad-0.3.7/kittycad/models/file_system_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/file_volume.py` & `kittycad-0.3.7/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/gateway.py` & `kittycad-0.3.7/kittycad/models/gateway.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/index_info.py` & `kittycad-0.3.7/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/invoice.py` & `kittycad-0.3.7/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/invoice_line_item.py` & `kittycad-0.3.7/kittycad/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/jetstream.py` & `kittycad-0.3.7/kittycad/models/jetstream.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/jetstream_api_stats.py` & `kittycad-0.3.7/kittycad/models/jetstream_api_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/jetstream_config.py` & `kittycad-0.3.7/kittycad/models/jetstream_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/jetstream_stats.py` & `kittycad-0.3.7/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/leaf_node.py` & `kittycad-0.3.7/kittycad/models/leaf_node.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/mesh.py` & `kittycad-0.3.7/kittycad/models/mesh.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/meta_cluster_info.py` & `kittycad-0.3.7/kittycad/models/meta_cluster_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/metadata.py` & `kittycad-0.3.7/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/new_address.py` & `kittycad-0.3.7/kittycad/models/new_address.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/o_auth2_client_info.py` & `kittycad-0.3.7/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/onboarding.py` & `kittycad-0.3.7/kittycad/models/onboarding.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/output_file.py` & `kittycad-0.3.7/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/payment_intent.py` & `kittycad-0.3.7/kittycad/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/payment_method.py` & `kittycad-0.3.7/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/payment_method_card_checks.py` & `kittycad-0.3.7/kittycad/models/payment_method_card_checks.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/physics_constant.py` & `kittycad-0.3.7/kittycad/models/physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/physics_constant_name.py` & `kittycad-0.3.7/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/plugins_info.py` & `kittycad-0.3.7/kittycad/models/plugins_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/point_e_metadata.py` & `kittycad-0.3.7/kittycad/models/point_e_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/pong.py` & `kittycad-0.3.7/kittycad/models/pong.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/registry_service_config.py` & `kittycad-0.3.7/kittycad/models/registry_service_config.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/runtime.py` & `kittycad-0.3.7/kittycad/models/runtime.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/session.py` & `kittycad-0.3.7/kittycad/models/session.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.3.7/kittycad/models/system_info_default_address_pools.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_acceleration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_angle_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_area_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_charge_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_charge_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_concentration_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_data_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_data_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_density_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_density_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_density_format.py` & `kittycad-0.3.7/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_energy_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_force_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_illuminance_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_length_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_length_format.py` & `kittycad-0.3.7/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_mass_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_metric_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_power_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_radiation_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_radioactivity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_solid_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_time_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_time_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_velocity_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_voltage_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_volume_conversion.py` & `kittycad-0.3.7/kittycad/models/unit_volume_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/unit_volume_format.py` & `kittycad-0.3.7/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/update_user.py` & `kittycad-0.3.7/kittycad/models/update_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/user.py` & `kittycad-0.3.7/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/user_results_page.py` & `kittycad-0.3.7/kittycad/models/user_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/models/verification_token.py` & `kittycad-0.3.7/kittycad/models/verification_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/kittycad/types.py` & `kittycad-0.3.7/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.3.6/pyproject.toml` & `kittycad-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.3.6"
+version = "0.3.7"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
```

### Comparing `kittycad-0.3.6/PKG-INFO` & `kittycad-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.3.6
+Version: 0.3.7
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

