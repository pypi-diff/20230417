# Comparing `tmp/kiln_connect-1.0.0.dev3.tar.gz` & `tmp/kiln_connect-1.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiln_connect-1.0.0.dev3.tar", max compression
+gzip compressed data, was "kiln_connect-1.0.0.dev4.tar", max compression
```

## Comparing `kiln_connect-1.0.0.dev3.tar` & `kiln_connect-1.0.0.dev4.tar`

### file list

```diff
@@ -1,212 +1,244 @@
--rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/docs/README.md
--rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev3/kiln_cli/__init__.py
--rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_cli/accounts.py
--rw-r--r--   0        0        0     6670 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_cli/eth.py
--rw-r--r--   0        0        0      388 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_cli/main.py
--rwxr-xr-x   0        0        0     6101 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_cli/sol.py
--rw-r--r--   0        0        0     6844 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_cli/xtz.py
--rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev3/kiln_connect/__init__.py
--rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev3/kiln_connect/accounts.py
--rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/errors.py
--rw-r--r--   0        0        0     4144 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/eth.py
--rw-r--r--   0        0        0     5285 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/integrations.py
--rw-r--r--   0        0        0     3271 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/kiln_connect.py
--rw-r--r--   0        0        0    10203 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/__init__.py
--rw-r--r--   0        0        0      333 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    32819 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/accounts_api.py
--rw-r--r--   0        0        0    79532 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/eth_api.py
--rw-r--r--   0        0        0    96157 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/sol_api.py
--rw-r--r--   0        0        0    59673 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/xtz_api.py
--rw-r--r--   0        0        0    30218 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api_client.py
--rw-r--r--   0        0        0    17494 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/configuration.py
--rw-r--r--   0        0        0     5713 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/exceptions.py
--rw-r--r--   0        0        0     9362 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/__init__.py
--rw-r--r--   0        0        0     3006 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account.py
--rw-r--r--   0        0        0     2782 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_payload.py
--rw-r--r--   0        0        0     4028 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio.py
--rw-r--r--   0        0        0     4878 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     3019 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     3016 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     3245 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/core_stake.py
--rw-r--r--   0        0        0     2666 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
--rw-r--r--   0        0        0     3090 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2910 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_kiln_stats.py
--rw-r--r--   0        0        0     2971 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     3028 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_network_stats.py
--rw-r--r--   0        0        0     3485 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     4582 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_deposit.py
--rw-r--r--   0        0        0     3820 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
--rw-r--r--   0        0        0     3522 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     4456 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     3376 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_payload.py
--rw-r--r--   0        0        0     3042 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     3846 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_reward.py
--rw-r--r--   0        0        0     2662 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_signed_tx.py
--rw-r--r--   0        0        0     7278 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_stake.py
--rw-r--r--   0        0        0     4514 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status.py
--rw-r--r--   0        0        0     5288 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status_receipt.py
--rw-r--r--   0        0        0     3681 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     2972 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
--rw-r--r--   0        0        0     3064 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_accounts200_response.py
--rw-r--r--   0        0        0     2929 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2962 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_operations200_response.py
--rw-r--r--   0        0        0     6360 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3087 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3076 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     3187 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
--rw-r--r--   0        0        0     5115 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     3187 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     5085 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2879 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_account201_response.py
--rw-r--r--   0        0        0     2966 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2959 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_keys201_response.py
--rw-r--r--   0        0        0     5501 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2932 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2958 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2940 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2914 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2902 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2966 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2932 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     2534 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_broadcast_tx.py
--rw-r--r--   0        0        0     2607 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2816 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     3015 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     2965 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_network_stats.py
--rw-r--r--   0        0        0     3299 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
--rw-r--r--   0        0        0     3074 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2765 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2579 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_prepared_tx.py
--rw-r--r--   0        0        0     3082 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_reward_by_day.py
--rw-r--r--   0        0        0     3246 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
--rw-r--r--   0        0        0     3070 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     5320 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake.py
--rw-r--r--   0        0        0     2685 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake_tx.py
--rw-r--r--   0        0        0     3095 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2996 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2694 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/soltx_status.py
--rw-r--r--   0        0        0     2666 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2984 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2664 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     3294 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_cycle_reward.py
--rw-r--r--   0        0        0     3130 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_daily_reward.py
--rw-r--r--   0        0        0     3522 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_network_stats.py
--rw-r--r--   0        0        0     2832 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2662 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_signed_tx.py
--rw-r--r--   0        0        0     5809 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_stake.py
--rw-r--r--   0        0        0     2871 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtztx_status.py
--rw-r--r--   0        0        0     3193 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtztx_status_receipt.py
--rw-r--r--   0        0        0    13289 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/rest.py
--rw-r--r--   0        0        0        0 2023-04-03 07:07:01.546136 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account.py
--rw-r--r--   0        0        0     2283 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_payload.py
--rw-r--r--   0        0        0     3364 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio.py
--rw-r--r--   0        0        0     3074 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     2552 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     2552 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     2053 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_accounts_api.py
--rw-r--r--   0        0        0     2719 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_core_stake.py
--rw-r--r--   0        0        0     2949 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_api.py
--rw-r--r--   0        0        0     2414 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2252 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
--rw-r--r--   0        0        0     2620 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2337 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
--rw-r--r--   0        0        0     2310 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     2273 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_network_stats.py
--rw-r--r--   0        0        0     2735 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     3049 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
--rw-r--r--   0        0        0     2791 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
--rw-r--r--   0        0        0     2875 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     3182 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     2587 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
--rw-r--r--   0        0        0     2809 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     2432 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_reward.py
--rw-r--r--   0        0        0     2201 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_signed_tx.py
--rw-r--r--   0        0        0     3015 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_stake.py
--rw-r--r--   0        0        0     4064 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
--rw-r--r--   0        0        0     3737 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status.py
--rw-r--r--   0        0        0     3576 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py
--rw-r--r--   0        0        0     2650 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     3709 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
--rw-r--r--   0        0        0     2595 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_accounts200_response.py
--rw-r--r--   0        0        0     2615 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2553 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
--rw-r--r--   0        0        0     3451 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2803 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3444 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
--rw-r--r--   0        0        0     4114 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2550 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     2327 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
--rw-r--r--   0        0        0     2865 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3155 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2480 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2650 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     2327 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     2779 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3071 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2877 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2535 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_account201_response.py
--rw-r--r--   0        0        0     2514 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2259 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
--rw-r--r--   0        0        0     2899 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2489 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     4344 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2444 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2431 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2447 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2746 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2499 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2489 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2581 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     3350 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_api.py
--rw-r--r--   0        0        0     2192 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
--rw-r--r--   0        0        0     2290 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2599 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     2750 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     2394 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_network_stats.py
--rw-r--r--   0        0        0     2967 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
--rw-r--r--   0        0        0     2458 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2439 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2206 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
--rw-r--r--   0        0        0     2471 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
--rw-r--r--   0        0        0     2538 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
--rw-r--r--   0        0        0     2773 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     3183 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake.py
--rw-r--r--   0        0        0     2253 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake_tx.py
--rw-r--r--   0        0        0     2739 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2630 2023-04-04 13:04:32.724122 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2199 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_soltx_status.py
--rw-r--r--   0        0        0     2541 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_api.py
--rw-r--r--   0        0        0     2414 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2237 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2646 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2388 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     2426 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
--rw-r--r--   0        0        0     2374 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
--rw-r--r--   0        0        0     2362 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_network_stats.py
--rw-r--r--   0        0        0     2601 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2201 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
--rw-r--r--   0        0        0     2666 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_stake.py
--rw-r--r--   0        0        0     2333 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
--rw-r--r--   0        0        0     2580 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtztx_status.py
--rw-r--r--   0        0        0     2502 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py
--rw-r--r--   0        0        0      642 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/sol.py
--rw-r--r--   0        0        0      238 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/utils.py
--rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev3/kiln_connect/xtz.py
--rw-r--r--   0        0        0     1012 2023-04-04 13:04:56.237284 kiln_connect-1.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     6609 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev4/docs/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev4/kiln_cli/__init__.py
+-rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev4/kiln_cli/accounts.py
+-rw-r--r--   0        0        0     2520 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_cli/atom.py
+-rw-r--r--   0        0        0     6670 2023-04-06 15:53:36.351598 kiln_connect-1.0.0.dev4/kiln_cli/eth.py
+-rw-r--r--   0        0        0      410 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_cli/main.py
+-rwxr-xr-x   0        0        0    10741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_cli/sol.py
+-rw-r--r--   0        0        0     6844 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev4/kiln_cli/xtz.py
+-rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev4/kiln_connect/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev4/kiln_connect/accounts.py
+-rw-r--r--   0        0        0      656 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/atom.py
+-rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev4/kiln_connect/errors.py
+-rw-r--r--   0        0        0     4144 2023-04-14 03:37:21.881892 kiln_connect-1.0.0.dev4/kiln_connect/eth.py
+-rw-r--r--   0        0        0     5301 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/integrations.py
+-rw-r--r--   0        0        0     3666 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/kiln_connect.py
+-rw-r--r--   0        0        0    11600 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    32819 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/accounts_api.py
+-rw-r--r--   0        0        0    21212 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/atom_api.py
+-rw-r--r--   0        0        0    79556 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/eth_api.py
+-rw-r--r--   0        0        0   104060 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/sol_api.py
+-rw-r--r--   0        0        0    59673 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/xtz_api.py
+-rw-r--r--   0        0        0    30218 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api_client.py
+-rw-r--r--   0        0        0    17494 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/configuration.py
+-rw-r--r--   0        0        0     5713 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/exceptions.py
+-rw-r--r--   0        0        0    10698 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0     3006 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account.py
+-rw-r--r--   0        0        0     2782 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_payload.py
+-rw-r--r--   0        0        0     4028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio.py
+-rw-r--r--   0        0        0     4878 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     3019 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     3016 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     3478 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/atom_reward.py
+-rw-r--r--   0        0        0     4849 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/atom_stake.py
+-rw-r--r--   0        0        0     3245 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/core_stake.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     3090 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2910 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_kiln_stats.py
+-rw-r--r--   0        0        0     2971 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     3028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_network_stats.py
+-rw-r--r--   0        0        0     3485 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     4582 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_deposit.py
+-rw-r--r--   0        0        0     3820 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     4456 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     3376 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_payload.py
+-rw-r--r--   0        0        0     3042 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     3846 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_reward.py
+-rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_signed_tx.py
+-rw-r--r--   0        0        0     7278 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_stake.py
+-rw-r--r--   0        0        0     4514 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_unsigned_tx.py
+-rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status.py
+-rw-r--r--   0        0        0     5288 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status_receipt.py
+-rw-r--r--   0        0        0     3681 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py
+-rw-r--r--   0        0        0     2972 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     3064 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_accounts200_response.py
+-rw-r--r--   0        0        0     3098 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3087 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     2929 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_operations200_response.py
+-rw-r--r--   0        0        0     7941 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3087 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_operations200_response.py
+-rw-r--r--   0        0        0    13955 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     5115 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     5085 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2879 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_account201_response.py
+-rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2959 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_keys201_response.py
+-rw-r--r--   0        0        0     5501 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2958 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2940 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2914 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2902 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_stakes201_response.py
+-rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     2572 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_broadcast_tx.py
+-rw-r--r--   0        0        0     2607 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2816 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     3025 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_network_stats.py
+-rw-r--r--   0        0        0     4048 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_create_account.py
+-rw-r--r--   0        0        0     4104 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     3866 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_deactivate.py
+-rw-r--r--   0        0        0     4037 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_delegate.py
+-rw-r--r--   0        0        0     4064 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_merge.py
+-rw-r--r--   0        0        0     4244 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_redelegate.py
+-rw-r--r--   0        0        0     4313 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_split.py
+-rw-r--r--   0        0        0     4218 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_operation_withdraw.py
+-rw-r--r--   0        0        0     3299 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     3072 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2765 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2617 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_prepared_tx.py
+-rw-r--r--   0        0        0     3142 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_reward_by_day.py
+-rw-r--r--   0        0        0     3317 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     3070 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     5250 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake.py
+-rw-r--r--   0        0        0     2734 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake_tx.py
+-rw-r--r--   0        0        0     3095 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2996 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     2705 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/soltx_status.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2984 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2664 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     3294 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_cycle_reward.py
+-rw-r--r--   0        0        0     3130 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_daily_reward.py
+-rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_network_stats.py
+-rw-r--r--   0        0        0     2832 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_signed_tx.py
+-rw-r--r--   0        0        0     5809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_stake.py
+-rw-r--r--   0        0        0     2871 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtztx_status.py
+-rw-r--r--   0        0        0     3193 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtztx_status_receipt.py
+-rw-r--r--   0        0        0    13289 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/rest.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/__init__.py
+-rw-r--r--   0        0        0     2257 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account.py
+-rw-r--r--   0        0        0     2283 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_payload.py
+-rw-r--r--   0        0        0     3364 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio.py
+-rw-r--r--   0        0        0     3074 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     2053 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_accounts_api.py
+-rw-r--r--   0        0        0     1632 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_atom_api.py
+-rw-r--r--   0        0        0     2284 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_atom_reward.py
+-rw-r--r--   0        0        0     2624 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_atom_stake.py
+-rw-r--r--   0        0        0     2719 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_core_stake.py
+-rw-r--r--   0        0        0     2949 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_api.py
+-rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2252 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     2620 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2337 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
+-rw-r--r--   0        0        0     2310 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     2273 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_network_stats.py
+-rw-r--r--   0        0        0     2735 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     3049 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
+-rw-r--r--   0        0        0     2791 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     2875 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     3182 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     2587 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
+-rw-r--r--   0        0        0     2809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2432 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_reward.py
+-rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_signed_tx.py
+-rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_stake.py
+-rw-r--r--   0        0        0     4064 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
+-rw-r--r--   0        0        0     3737 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status.py
+-rw-r--r--   0        0        0     3576 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py
+-rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py
+-rw-r--r--   0        0        0     3709 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     2595 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_accounts200_response.py
+-rw-r--r--   0        0        0     2625 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3007 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     2615 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2553 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
+-rw-r--r--   0        0        0     3451 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2803 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     4114 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     2550 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py
+-rw-r--r--   0        0        0     3163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     2706 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3141 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     2480 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     2779 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3071 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     2877 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2535 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_account201_response.py
+-rw-r--r--   0        0        0     2514 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2259 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
+-rw-r--r--   0        0        0     2899 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     4344 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2431 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2447 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2746 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py
+-rw-r--r--   0        0        0     2499 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2581 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     3493 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_api.py
+-rw-r--r--   0        0        0     2162 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
+-rw-r--r--   0        0        0     2290 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2599 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     2750 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     2270 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_network_stats.py
+-rw-r--r--   0        0        0     2792 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_create_account.py
+-rw-r--r--   0        0        0     2873 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     2687 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py
+-rw-r--r--   0        0        0     2741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_delegate.py
+-rw-r--r--   0        0        0     2644 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_merge.py
+-rw-r--r--   0        0        0     2786 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py
+-rw-r--r--   0        0        0     2740 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_split.py
+-rw-r--r--   0        0        0     2788 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py
+-rw-r--r--   0        0        0     2953 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     2451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2439 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
+-rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
+-rw-r--r--   0        0        0     2379 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     2773 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     2728 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake.py
+-rw-r--r--   0        0        0     2169 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake_tx.py
+-rw-r--r--   0        0        0     2739 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2630 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_soltx_status.py
+-rw-r--r--   0        0        0     2541 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_api.py
+-rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2237 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2646 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2388 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     2426 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
+-rw-r--r--   0        0        0     2374 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
+-rw-r--r--   0        0        0     2362 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_network_stats.py
+-rw-r--r--   0        0        0     2601 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_stake.py
+-rw-r--r--   0        0        0     2333 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     2580 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtztx_status.py
+-rw-r--r--   0        0        0     2502 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py
+-rw-r--r--   0        0        0     6471 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/sol.py
+-rw-r--r--   0        0        0      451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev4/kiln_connect/utils.py
+-rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev4/kiln_connect/xtz.py
+-rw-r--r--   0        0        0     1012 2023-04-17 03:18:02.028563 kiln_connect-1.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     6609 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev4/PKG-INFO
```

### Comparing `kiln_connect-1.0.0.dev3/docs/README.md` & `kiln_connect-1.0.0.dev4/docs/README.md`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_cli/accounts.py` & `kiln_connect-1.0.0.dev4/kiln_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_cli/eth.py` & `kiln_connect-1.0.0.dev4/kiln_cli/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_cli/sol.py` & `kiln_connect-1.0.0.dev4/kiln_cli/xtz.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,178 +1,201 @@
-"""Solana commands.
+"""Tezos commands.
 
 This file contains multiple CLI commands showcasing how to use the
-KilnConnect SDK to interact with the Solana blockchain.
+KilnConnect SDK to interact with the Tezos blockchain.
 
 Code here is voluntarily kept simple: it could be refactored with some
 levels of abstraction to avoid repetitions, but would imply readers to
 understand things unrelated to what their primary goal is: use the
 SDK. So let's keep it stupid simple so the integration work is
 simpler.
 """
 import logging
 from enum import Enum
 
-import re
 import click
+import re
 import typer
 
 from rich.console import Console
 from rich.table import Table
 from typing import Tuple
 
 import kiln_connect
 
-sol_cli = typer.Typer(
-    name='sol', help='Staking utilities for Solana', no_args_is_help=True)
+xtz_cli = typer.Typer(
+    name='xtz', help='Staking utilities for Tezos', no_args_is_help=True)
 
 console = Console()
 error_console = Console(stderr=True)
 
 
 class RewardsFormat(str, Enum):
     daily = "daily"
-    epoch = "epoch"
-
-
-class AccountFormat(str, Enum):
-    wallet = "wallet"
-    stake_account = "stake-account"
+    cycle = "cycle"
 
 
-def pretty_lamport_to_sol(lamport: str) -> str:
-    """Quick helper to pretty print LAMPORT to SOL.
-    """
-    if not lamport:
-        return 'n/a'
-    sol = str(round(int(lamport) / 1_000_000_000, 3))
-    return f"{sol} SOL"
-
+def sort_identifiers(identifiers: list[str]) -> Tuple[list[str], list[str]]:
+    """Sorts XTZ filtering identifiers in corresponding buckets.
 
-def sort_identifiers(identifiers: list[str], account_format: AccountFormat) -> Tuple[list[str], list[str]]:
-    """Sorts SOL filtering identifiers in corresponding buckets.
+    The Kiln XTZ API supports filtering by:
 
-    The Kiln SOL API supports filtering by:
-
-    - Solana wallet address
+    - Tezos wallet address
     - Kiln Account ID (UUID)
 
     This functions returns the identifiers sorted in their corresponding bucket.
     """
 
     accounts = []
     wallets = []
-    stake_accounts = []
 
     for identifier in identifiers:
+        identifier = identifier[2:] if '0x' in identifier else identifier
+
         # Kiln Account UUIDs
         if re.match('^[0-9a-f]{8}-[0-9a-f]{4}-[0-5][0-9a-f]{3}-[089ab][0-9a-f]{3}-[0-9a-f]{12}$', identifier):
             accounts.append(identifier)
             continue
 
-        # Wallet addresses or Stake accounts
-        if re.match('^[1-9A-HJ-NP-Za-km-z]{32,44}$', identifier):
-            if account_format == AccountFormat.stake_account:
-                stake_accounts.append(identifier)
-            else:
-                wallets.append(identifier)
+        # Wallet addresses start with tz or KT1
+        if re.match('^(tz|KT1)[a-zA-Z0-9]*$', identifier):
+            wallets.append(identifier)
             continue
 
         raise click.UsageError(
-            "Unknown identifier (should be a SOL stake account address, a SOL wallet address or a Kiln account UUID)")
+            "Unknown identifier (should be a BLS validator address, an ETH wallet address or a Kiln account UUID)")
 
     # This is a current limit of the Kiln API, we only support one
     # filter type at a time. This removes confusion when a staked is
     # matched by multiple filters.
-    if accounts and (wallets or stake_accounts):
+    if accounts and wallets:
         raise click.UsageError(
             "Identifiers should be of the same type"
         )
 
-    return accounts or None, wallets or None, stake_accounts or None
+    return accounts or None, wallets or None
+
+
+def pretty_mutez_to_tez(mutez: str) -> str:
+    """Quick helper to pretty print MUTEZ to TEZ.
+    """
+    if not mutez:
+        return 'n/a'
+    tez = str(round(int(mutez) / 1e6, 6))
+    return f"{tez}XTZ"
 
 
-@sol_cli.command("network-stats")
-def sol_network_stats():
-    """Show the Solana network stats.
+@xtz_cli.command("network-stats")
+def xtz_network_stats():
+    """Show Tezos Network Stats.
     """
     with kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env()) as kc:
-        stats = kc.sol.get_sol_network_stats()
+        ns = kc.xtz.get_xtz_network_stats()
 
-        table = Table('Network Gross APY %', 'Nb validators',
-                      'Supply Percentage Stake')
+        table = Table('Network Gross APY %', 'Nb Validator', 'Supply Percentage Stake', 'Updated At')
         table.add_row(
-            str(round(stats.data.network_gross_apy, 3)),
-            str(stats.data.nb_validators),
-            str(round(stats.data.supply_staked_percent, 3)),
+            str(round(ns.data.network_gross_apy, 3)),
+            str(ns.data.nb_validators),
+            str(round(ns.data.supply_staked_percent, 3)),
+            str(ns.data.updated_at)
         )
 
         console.print(table)
 
 
-@sol_cli.command("stakes")
-def sol_stakes(
-        identifiers: list[str],
-        account_format: AccountFormat = typer.Option(AccountFormat.wallet, '--account-format')):
-    """Show the stakes for the specified Solana wallet addresses or Kiln Account IDs.
+@xtz_cli.command("stakes")
+def xtz_stakes(identifiers: list[str]):
+    """List Tezos Stake status.
     """
     with kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env()) as kc:
-        accounts, wallets, stake_accounts = sort_identifiers(
-            identifiers, account_format)
+        accounts, wallets = sort_identifiers(identifiers)
 
-        stakes = kc.sol.get_sol_stakes(
-            wallets=wallets, accounts=accounts, stake_accounts=stake_accounts)
+        stakes = kc.xtz.get_xtz_stakes(accounts=accounts, wallets=wallets)
 
-        table = Table('Stake(s)', 'Status', 'Balance', 'Rewards')
+        table = Table('Stake(s)', 'Baker', 'Status', 'Delegated at Block', 'Delegated Cycle', 'Activated Cycle',
+                      'Balance', 'Rewards')
         for stake in stakes.data:
             table.add_row(
-                stake.stake_account,
+                stake.stake_address,
+                stake.baker_address,
                 stake.state,
-                str(pretty_lamport_to_sol(stake.balance)),
-                str(pretty_lamport_to_sol(stake.rewards)),
-            )
+                str(stake.delegated_block),
+                str(stake.delegated_cycle),
+                str(stake.activated_cycle),
+                pretty_mutez_to_tez(stake.balance),
+                pretty_mutez_to_tez(stake.rewards))
 
         console.print(table)
 
 
-@sol_cli.command("rewards")
-def sol_rewards(
+@xtz_cli.command("rewards")
+def xtz_rewards(
         identifiers: list[str],
-        account_format: AccountFormat = typer.Option(
-            AccountFormat.wallet, '--account-format'),
         response_format: RewardsFormat = typer.Option(RewardsFormat.daily, '--format')):
-    """Show the rewards for the specified Solana wallet addresses or Kiln Account IDs.
+    """View Tezos rewards.
     """
     with kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env()) as kc:
-        accounts, wallets, stake_accounts = sort_identifiers(
-            identifiers, account_format)
+        accounts, wallets = sort_identifiers(identifiers)
 
-        rewards = kc.sol.get_sol_rewards(
-            wallets=wallets, accounts=accounts, stake_accounts=stake_accounts, format=response_format.value)
+        rewards = kc.xtz.get_xtz_rewards(accounts=accounts, wallets=wallets, format=response_format.value)
 
         if response_format == RewardsFormat.daily:
             table = Table('Date', 'Active Balance', 'Rewards', 'Gross APY')
             for reward in rewards.data:
                 table.add_row(
                     str(reward.actual_instance.var_date),
-                    pretty_lamport_to_sol(
-                        reward.actual_instance.active_balance),
-                    pretty_lamport_to_sol(reward.actual_instance.rewards),
-                    str(round(reward.actual_instance.net_apy, 3))
+                    pretty_mutez_to_tez(reward.actual_instance.active_balance),
+                    pretty_mutez_to_tez(reward.actual_instance.rewards),
+                    str(round(reward.actual_instance.gross_apy, 3))
                 )
             console.print(table)
-        elif response_format == RewardsFormat.epoch:
-            table = Table('Epoch', 'Active Balance', 'Rewards', 'Gross APY')
+        elif response_format == RewardsFormat.cycle:
+            table = Table('Cycle', 'Cycle Begins At', 'Active Balance', 'Rewards', 'Gross APY')
             for reward in rewards.data:
                 table.add_row(
-                    str(reward.actual_instance.epoch),
-                    pretty_lamport_to_sol(
-                        reward.actual_instance.active_balance),
-                    pretty_lamport_to_sol(reward.actual_instance.rewards),
-                    str(round(reward.actual_instance.net_apy, 3)))
-                console.print(table)
+                    str(reward.actual_instance.cycle),
+                    str(reward.actual_instance.cycle_begins_at),
+                    pretty_mutez_to_tez(reward.actual_instance.active_balance),
+                    pretty_mutez_to_tez(reward.actual_instance.rewards),
+                    str(round(reward.actual_instance.gross_apy, 3)))
+            console.print(table)
+
+
+@xtz_cli.command("stake")
+def xtz_stake_via_fireblocks(account_id: str, wallet: str, baker: str):
+    """
+    Stake XTZ via Fireblocks
+    :param account_id:
+    :param wallet:
+    :param baker:
+    :return:
+    """
+    with kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env()) as kc:
+        with console.status("[bold green]Staking in progress...") as status:
+            data = kc.xtz.stake("fireblocks", account_id, wallet, baker)
+            console.print("==============")
+            console.print("[bold]Successfully staked[/bold]")
+            console.print(f"[bold]TX Hash[/bold]: {data.tx_hash}")
+            status.stop()
+
+
+@xtz_cli.command("unstake")
+def xtz_unstake_via_fireblocks(account_id: str, wallet: str):
+    """
+    Unstake XTZ via Fireblocks
+    :param account_id:
+    :param wallet:
+    :return:
+    """
+    with kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env()) as kc:
+        with console.status("[bold green]Unstaking in progress...") as status:
+            data = kc.xtz.unstake("fireblocks", account_id, wallet)
+            console.print("==============")
+            console.print("[bold]Successfully unstaked[/bold]")
+            console.print(f"[bold]TX Hash[/bold]: {data.tx_hash}")
+            status.stop()
 
 
-@sol_cli.command("test")
-def sol_test():
+@xtz_cli.command("test")
+def xtz_test():
     kiln_connect.KilnConnect(kiln_connect.KilnConfig.from_env())
     logging.debug("test")
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/accounts.py` & `kiln_connect-1.0.0.dev4/kiln_connect/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/errors.py` & `kiln_connect-1.0.0.dev4/kiln_connect/errors.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/eth.py` & `kiln_connect-1.0.0.dev4/kiln_connect/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/integrations.py` & `kiln_connect-1.0.0.dev4/kiln_connect/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     provider: str
     parameters: dict
 
 
 class Asset(str, Enum):
     eth = "eth"
     xtz = "xtz"
+    sol = "sol"
 
 
 class FireblocksIntegration:
     """Handles the Fireblocks integration.
     """
 
     def __init__(self, config: IntegrationConfig):
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/kiln_connect.py` & `kiln_connect-1.0.0.dev4/kiln_connect/kiln_connect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 
 from dataclasses import dataclass
 
 from kiln_connect.openapi_client import ApiClient, Configuration
 
+from .atom import ATOM
 from .eth import ETH
 from .sol import SOL
 from .xtz import XTZ
 from .accounts import Accounts
 from .errors import (
     KilnInvalidEnvError,
     KilnError  # noqa: F401
@@ -27,26 +28,35 @@
     @staticmethod
     def from_env():
         """Init the Config looking at what we find in the env.
         """
         integration_configs = []
 
         env = os.getenv("KILN_ENV")
-        if env not in ["devnet", "testnet"]:
+        if env not in ["devnet", "testnet", "mainnet"]:
             raise KilnInvalidEnvError
 
         # Fireblocks integration
         fireblocks_api_token = os.getenv("FIREBLOCKS_API_KEY")
         if fireblocks_api_token:
             assets = {}
-            if env == "devnet" or env == "testnet":
-                assets = {
-                    Asset.eth: "ETH_TEST3",
-                    Asset.xtz: "XTZ_TEST"
-                }
+
+            match env:
+                case "devnet" | "testnet":
+                    assets = {
+                        Asset.eth: "ETH_TEST3",
+                        Asset.xtz: "XTZ_TEST",
+                        Asset.sol: "SOL_TEST"
+                    }
+                case "mainnet":
+                    assets = {
+                        Asset.eth: "ETH",
+                        Asset.xtz: "XTZ",
+                        Asset.sol: "SOL"
+                    }
 
             fireblocks_raw_key_path = os.getenv("FIREBLOCKS_RAW_KEY_PATH")
             fireblocks_vault_account_id = os.getenv(
                 "FIREBLOCKS_VAULT_ACCOUNT_ID")
             integration_configs.append(IntegrationConfig(
                 name="fireblocks",
                 provider="fireblocks",
@@ -66,15 +76,16 @@
             os.makedirs(os.path.dirname(log_dir), exist_ok=True)
             logging.basicConfig(
                 format=format,
                 filename=log_dir,
                 level=logging.DEBUG,
                 encoding="utf-8")
         else:
-            logging.basicConfig(format=format, level=logging.DEBUG, encoding="utf-8")
+            logging.basicConfig(
+                format=format, level=logging.DEBUG, encoding="utf-8")
 
         return KilnConfig(
             kiln_base_url=os.getenv("KILN_API_URL"),
             kiln_api_token=os.getenv("KILN_API_TOKEN"),
             integrations=integration_configs,
         )
 
@@ -94,14 +105,15 @@
         )
 
         self._integrations = Integrations(config.integrations)
 
         self.xtz = XTZ(self._api, self._integrations)
         self.eth = ETH(self._api, self._integrations)
         self.sol = SOL(self._api, self._integrations)
+        self.atom = ATOM(self._api, self._integrations)
         self.accounts = Accounts(self._api, self._integrations)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/__init__.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 
 from __future__ import absolute_import
 
 __version__ = "1.0.0"
 
 # import apis into sdk package
 from kiln_connect.openapi_client.api.accounts_api import AccountsApi
+from kiln_connect.openapi_client.api.atom_api import AtomApi
 from kiln_connect.openapi_client.api.eth_api import EthApi
 from kiln_connect.openapi_client.api.sol_api import SolApi
 from kiln_connect.openapi_client.api.xtz_api import XtzApi
 
 # import ApiClient
 from kiln_connect.openapi_client.api_client import ApiClient
 from kiln_connect.openapi_client.configuration import Configuration
 from kiln_connect.openapi_client.exceptions import OpenApiException
 from kiln_connect.openapi_client.exceptions import ApiTypeError
 from kiln_connect.openapi_client.exceptions import ApiValueError
 from kiln_connect.openapi_client.exceptions import ApiKeyError
 from kiln_connect.openapi_client.exceptions import ApiAttributeError
 from kiln_connect.openapi_client.exceptions import ApiException
 # import models into sdk package
+from kiln_connect.openapi_client.models.atom_reward import ATOMReward
+from kiln_connect.openapi_client.models.atom_stake import ATOMStake
 from kiln_connect.openapi_client.models.account import Account
 from kiln_connect.openapi_client.models.account_payload import AccountPayload
 from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards
 from kiln_connect.openapi_client.models.core_stake import CoreStake
@@ -58,22 +61,26 @@
 from kiln_connect.openapi_client.models.eth_stake import ETHStake
 from kiln_connect.openapi_client.models.ethtx_status import ETHTxStatus
 from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt
 from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner
 from kiln_connect.openapi_client.models.eth_unsigned_tx import ETHUnsignedTx
 from kiln_connect.openapi_client.models.get_account_portfolio200_response import GetAccountPortfolio200Response
 from kiln_connect.openapi_client.models.get_accounts200_response import GetAccounts200Response
+from kiln_connect.openapi_client.models.get_atom_rewards200_response import GetAtomRewards200Response
+from kiln_connect.openapi_client.models.get_atom_stakes200_response import GetAtomStakes200Response
 from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
 from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response_data_inner import GetEthOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
 from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
 from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
+from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
+from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
@@ -93,14 +100,22 @@
 from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response
 from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response
 from kiln_connect.openapi_client.models.sol_broadcast_tx import SOLBroadcastTx
 from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload
 from kiln_connect.openapi_client.models.sol_deactivate_stake_tx_payload import SOLDeactivateStakeTxPayload
 from kiln_connect.openapi_client.models.sol_merge_stakes_tx_payload import SOLMergeStakesTxPayload
 from kiln_connect.openapi_client.models.sol_network_stats import SOLNetworkStats
+from kiln_connect.openapi_client.models.sol_operation_create_account import SOLOperationCreateAccount
+from kiln_connect.openapi_client.models.sol_operation_create_account_with_seed import SOLOperationCreateAccountWithSeed
+from kiln_connect.openapi_client.models.sol_operation_deactivate import SOLOperationDeactivate
+from kiln_connect.openapi_client.models.sol_operation_delegate import SOLOperationDelegate
+from kiln_connect.openapi_client.models.sol_operation_merge import SOLOperationMerge
+from kiln_connect.openapi_client.models.sol_operation_redelegate import SOLOperationRedelegate
+from kiln_connect.openapi_client.models.sol_operation_split import SOLOperationSplit
+from kiln_connect.openapi_client.models.sol_operation_withdraw import SOLOperationWithdraw
 from kiln_connect.openapi_client.models.sol_post_stakes_payload import SOLPostStakesPayload
 from kiln_connect.openapi_client.models.sol_post_stakes_payload_stakes_inner import SOLPostStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.sol_prepare_tx_payload import SOLPrepareTxPayload
 from kiln_connect.openapi_client.models.sol_prepared_tx import SOLPreparedTx
 from kiln_connect.openapi_client.models.sol_reward_by_day import SOLRewardByDay
 from kiln_connect.openapi_client.models.sol_reward_by_epoch import SOLRewardByEpoch
 from kiln_connect.openapi_client.models.sol_split_stake_tx_payload import SOLSplitStakeTxPayload
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/accounts_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/eth_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/eth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_reports(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> str:  # noqa: E501
+    def get_eth_reports(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> bytearray:  # noqa: E501
         """Excel Reports  # noqa: E501
 
         Generates an Excel report sheet for your stakes and rewards  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_reports(validators, wallets, accounts, async_req=True)
@@ -523,15 +523,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: bytearray
         """
         kwargs['_return_http_data_only'] = True
         return self.get_eth_reports_with_http_info(validators, wallets, accounts, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_eth_reports_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
         """Excel Reports  # noqa: E501
@@ -566,15 +566,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'validators',
             'wallets',
@@ -633,15 +633,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/octet-stream'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "bytearray",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
             '/v1/eth/reports', 'GET',
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/sol_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/sol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from datetime import date
 
 from pydantic import Field, StrictStr, conlist
 
 from typing import Optional
 
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
+from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.post_sol_broadcast_tx201_response import PostSolBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_sol_prepare_tx201_response import PostSolPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_stake_tx201_response import PostSolStakeTx201Response
 from kiln_connect.openapi_client.models.post_sol_stakes201_response import PostSolStakes201Response
@@ -195,15 +196,178 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_sol_reports(self, stake_accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of stake addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, **kwargs) -> str:  # noqa: E501
+    def get_sol_operations(self, stake_accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of stake addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetSolOperations200Response:  # noqa: E501
+        """Operations  # noqa: E501
+
+        Get the operations of Solana stakes  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_sol_operations(stake_accounts, wallets, accounts, async_req=True)
+        >>> result = thread.get()
+
+        :param stake_accounts: Comma-separated list of stake addresses
+        :type stake_accounts: List[str]
+        :param wallets: Comma-separated list of wallets addresses
+        :type wallets: List[str]
+        :param accounts: Comma-separated list of Kiln accounts identifiers
+        :type accounts: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GetSolOperations200Response
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_sol_operations_with_http_info(stake_accounts, wallets, accounts, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_sol_operations_with_http_info(self, stake_accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of stake addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+        """Operations  # noqa: E501
+
+        Get the operations of Solana stakes  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_sol_operations_with_http_info(stake_accounts, wallets, accounts, async_req=True)
+        >>> result = thread.get()
+
+        :param stake_accounts: Comma-separated list of stake addresses
+        :type stake_accounts: List[str]
+        :param wallets: Comma-separated list of wallets addresses
+        :type wallets: List[str]
+        :param accounts: Comma-separated list of Kiln accounts identifiers
+        :type accounts: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GetSolOperations200Response, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'stake_accounts',
+            'wallets',
+            'accounts'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_sol_operations" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('stake_accounts') is not None:  # noqa: E501
+            _query_params.append(('stake_accounts', _params['stake_accounts']))
+            _collection_formats['stake_accounts'] = 'csv'
+        if _params.get('wallets') is not None:  # noqa: E501
+            _query_params.append(('wallets', _params['wallets']))
+            _collection_formats['wallets'] = 'csv'
+        if _params.get('accounts') is not None:  # noqa: E501
+            _query_params.append(('accounts', _params['accounts']))
+            _collection_formats['accounts'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json; charset=utf-8'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['bearerAuth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GetSolOperations200Response",
+            '400': None,
+            '401': None,
+            '500': None,
+        }
+
+        return self.api_client.call_api(
+            '/v1/sol/operations', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def get_sol_reports(self, stake_accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of stake addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, **kwargs) -> bytearray:  # noqa: E501
         """Reports  # noqa: E501
 
         Get reports on Solana staking  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_sol_reports(stake_accounts, wallets, accounts, format, async_req=True)
@@ -226,15 +390,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: str
+        :rtype: bytearray
         """
         kwargs['_return_http_data_only'] = True
         return self.get_sol_reports_with_http_info(stake_accounts, wallets, accounts, format, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_sol_reports_with_http_info(self, stake_accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of stake addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, **kwargs):  # noqa: E501
         """Reports  # noqa: E501
@@ -271,15 +435,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'stake_accounts',
             'wallets',
@@ -341,15 +505,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/octet-stream'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "bytearray",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
             '/v1/sol/reports', 'GET',
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api/xtz_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api/xtz_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/api_client.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/configuration.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/exceptions.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/__init__.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
+from kiln_connect.openapi_client.models.atom_reward import ATOMReward
+from kiln_connect.openapi_client.models.atom_stake import ATOMStake
 from kiln_connect.openapi_client.models.account import Account
 from kiln_connect.openapi_client.models.account_payload import AccountPayload
 from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance
 from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards
 from kiln_connect.openapi_client.models.core_stake import CoreStake
@@ -40,22 +42,26 @@
 from kiln_connect.openapi_client.models.eth_stake import ETHStake
 from kiln_connect.openapi_client.models.ethtx_status import ETHTxStatus
 from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt
 from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner
 from kiln_connect.openapi_client.models.eth_unsigned_tx import ETHUnsignedTx
 from kiln_connect.openapi_client.models.get_account_portfolio200_response import GetAccountPortfolio200Response
 from kiln_connect.openapi_client.models.get_accounts200_response import GetAccounts200Response
+from kiln_connect.openapi_client.models.get_atom_rewards200_response import GetAtomRewards200Response
+from kiln_connect.openapi_client.models.get_atom_stakes200_response import GetAtomStakes200Response
 from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
 from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response_data_inner import GetEthOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
 from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
 from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
+from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
+from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
@@ -75,14 +81,22 @@
 from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response
 from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response
 from kiln_connect.openapi_client.models.sol_broadcast_tx import SOLBroadcastTx
 from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload
 from kiln_connect.openapi_client.models.sol_deactivate_stake_tx_payload import SOLDeactivateStakeTxPayload
 from kiln_connect.openapi_client.models.sol_merge_stakes_tx_payload import SOLMergeStakesTxPayload
 from kiln_connect.openapi_client.models.sol_network_stats import SOLNetworkStats
+from kiln_connect.openapi_client.models.sol_operation_create_account import SOLOperationCreateAccount
+from kiln_connect.openapi_client.models.sol_operation_create_account_with_seed import SOLOperationCreateAccountWithSeed
+from kiln_connect.openapi_client.models.sol_operation_deactivate import SOLOperationDeactivate
+from kiln_connect.openapi_client.models.sol_operation_delegate import SOLOperationDelegate
+from kiln_connect.openapi_client.models.sol_operation_merge import SOLOperationMerge
+from kiln_connect.openapi_client.models.sol_operation_redelegate import SOLOperationRedelegate
+from kiln_connect.openapi_client.models.sol_operation_split import SOLOperationSplit
+from kiln_connect.openapi_client.models.sol_operation_withdraw import SOLOperationWithdraw
 from kiln_connect.openapi_client.models.sol_post_stakes_payload import SOLPostStakesPayload
 from kiln_connect.openapi_client.models.sol_post_stakes_payload_stakes_inner import SOLPostStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.sol_prepare_tx_payload import SOLPrepareTxPayload
 from kiln_connect.openapi_client.models.sol_prepared_tx import SOLPreparedTx
 from kiln_connect.openapi_client.models.sol_reward_by_day import SOLRewardByDay
 from kiln_connect.openapi_client.models.sol_reward_by_epoch import SOLRewardByEpoch
 from kiln_connect.openapi_client.models.sol_split_stake_tx_payload import SOLSplitStakeTxPayload
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/core_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_kiln_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_deposit.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_deposit.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_operation_execution_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_signed_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_account_portfolio200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_accounts200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py`

 * *Files 27% similar despite different names*

```diff
@@ -85,14 +85,49 @@
     @classmethod
     def from_json(cls, json_str: str) -> GetEthOperations200ResponseDataInner:
         """Returns the object represented by the json string"""
         instance = cls()
         error_messages = []
         match = 0
 
+        # use oneOf discriminator to lookup the data type
+        _data_type = json.loads(json_str).get("type")
+        if not _data_type:
+            raise ValueError("Failed to lookup data type from the field `type` in the input.")
+
+        # check if data type is `ETHOperationConsensusWithdrawal`
+        if _data_type == "ETHOperationConsensusWithdrawal":
+            instance.actual_instance = ETHOperationConsensusWithdrawal.from_json(json_str)
+            return instance
+
+        # check if data type is `ETHOperationDeposit`
+        if _data_type == "ETHOperationDeposit":
+            instance.actual_instance = ETHOperationDeposit.from_json(json_str)
+            return instance
+
+        # check if data type is `ETHOperationExecutionReward`
+        if _data_type == "ETHOperationExecutionReward":
+            instance.actual_instance = ETHOperationExecutionReward.from_json(json_str)
+            return instance
+
+        # check if data type is `ETHOperationConsensusWithdrawal`
+        if _data_type == "consensus_withdrawal":
+            instance.actual_instance = ETHOperationConsensusWithdrawal.from_json(json_str)
+            return instance
+
+        # check if data type is `ETHOperationDeposit`
+        if _data_type == "deposit":
+            instance.actual_instance = ETHOperationDeposit.from_json(json_str)
+            return instance
+
+        # check if data type is `ETHOperationExecutionReward`
+        if _data_type == "execution_reward":
+            instance.actual_instance = ETHOperationExecutionReward.from_json(json_str)
+            return instance
+
         # deserialize data into ETHOperationDeposit
         try:
             instance.actual_instance = ETHOperationDeposit.from_json(json_str)
             match += 1
         except ValidationError as e:
             error_messages.append(str(e))
         # deserialize data into ETHOperationConsensusWithdrawal
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_account201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_sol_stakes201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_broadcast_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, StrictStr
 
 class SOLBroadcastTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    tx_hash: StrictStr = ...
+    tx_hash: Optional[StrictStr] = None
     __properties = ["tx_hash"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_network_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field
 
 class SOLNetworkStats(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    network_gross_apy: float = Field(..., description="Gross annual percentage yield")
-    supply_staked_percent: float = Field(..., description="Supply of Solana currently staked")
-    nb_validators: float = Field(..., description="Number of active stakes")
+    network_gross_apy: Optional[float] = Field(None, description="Gross annual percentage yield")
+    supply_staked_percent: Optional[float] = Field(None, description="Supply of Solana currently staked")
+    nb_validators: Optional[float] = Field(None, description="Number of active stakes")
     __properties = ["network_gross_apy", "supply_staked_percent", "nb_validators"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_post_stakes_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class SOLPostStakesPayloadStakesInner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    stake_account: Optional[StrictStr] = Field(None, alias="stakeAccount", description="Public key of the stake account")
+    stake_account: Optional[StrictStr] = Field(None, alias="stakeAccount", description="Stake account to be delegated")
     balance: Optional[float] = Field(None, description="Balance to delegate in SOL")
     __properties = ["stakeAccount", "balance"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_prepared_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_prepared_tx.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, StrictStr
 
 class SOLPreparedTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    signed_tx_serialized: StrictStr = ...
+    signed_tx_serialized: Optional[StrictStr] = None
     __properties = ["signed_tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_reward_by_day.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_reward_by_day.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class SOLRewardByDay(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     var_date: date = Field(..., alias="date", description="Day for this reward entry")
-    rewards: StrictStr = Field(..., description="Accumulated rewards in Lamport during the day")
-    active_balance: StrictStr = Field(..., description="Active balance in Lamport after rewards computing")
-    net_apy: float = Field(..., description="Net annual percentage yield")
+    rewards: Optional[StrictStr] = Field(None, description="Accumulated rewards in Lamport during the day")
+    active_balance: Optional[StrictStr] = Field(None, description="Active balance in Lamport after rewards computing")
+    net_apy: Optional[float] = Field(None, description="Net annual percentage yield")
     __properties = ["date", "rewards", "active_balance", "net_apy"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_reward_by_epoch.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class SOLRewardByEpoch(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     epoch: StrictInt = Field(..., description="Epoch for this reward entry")
-    epoch_ts: datetime = Field(..., description="Epoch timestamp for this reward entry")
-    rewards: StrictStr = Field(..., description="Accumulated rewards in Lamport during the day")
-    active_balance: StrictStr = Field(..., description="Active balance in Lamport after rewards computing")
-    net_apy: float = Field(..., description="Net annual percentage yield")
+    epoch_ts: Optional[datetime] = Field(None, description="Epoch timestamp for this reward entry")
+    rewards: Optional[StrictStr] = Field(None, description="Accumulated rewards in Lamport during the day")
+    active_balance: Optional[StrictStr] = Field(None, description="Active balance in Lamport after rewards computing")
+    net_apy: Optional[float] = Field(None, description="Net annual percentage yield")
     __properties = ["epoch", "epoch_ts", "rewards", "active_balance", "net_apy"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
 class SOLStake(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    stake_account: Optional[StrictStr] = Field(..., description="Public key of the stake account")
-    vote_account: StrictStr = Field(..., description="Public key of the validator")
-    withdraw_pubkey: Optional[StrictStr] = Field(..., description="Withdraw pubkey")
-    state: StrictStr = Field(..., description="State of the Solan stake")
+    stake_account: Optional[StrictStr] = Field(None, description="Delegated stake account")
+    vote_account: Optional[StrictStr] = Field(None, description="Vote account to which this stake was re-delegated.")
+    withdraw_pubkey: Optional[StrictStr] = Field(None, description="Withdraw pubkey")
+    state: Optional[StrictStr] = Field(None, description="Stake state")
     activated_at: Optional[datetime] = Field(None, description="Date at which this stake was activated")
     activated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was activated")
     deactivated_at: Optional[datetime] = Field(None, description="Date at which this stake was deactivated")
     deactivated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was deactivated")
     delegated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was delegated")
-    balance: StrictStr = Field(..., description="Current balance in Lamport")
-    rewards: StrictStr = Field(..., description="Sum of rewards rewards in Lamport earned by this stake")
-    net_apy: float = Field(..., description="net annual percentage yield")
-    updated_at: datetime = Field(..., description="Last date this data was updated")
+    balance: Optional[StrictStr] = Field(None, description="Current balance in Lamport")
+    rewards: Optional[StrictStr] = Field(None, description="Sum of rewards rewards in Lamport earned by this stake")
+    net_apy: Optional[float] = Field(None, description="Net annual percentage yield")
+    updated_at: Optional[datetime] = Field(None, description="Last date this data was updated")
     __properties = ["stake_account", "vote_account", "withdraw_pubkey", "state", "activated_at", "activated_epoch", "deactivated_at", "deactivated_epoch", "delegated_epoch", "balance", "rewards", "net_apy", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -61,18 +61,14 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if stake_account (nullable) is None
-        if self.stake_account is None:
-            _dict['stake_account'] = None
-
         # set to None if withdraw_pubkey (nullable) is None
         if self.withdraw_pubkey is None:
             _dict['withdraw_pubkey'] = None
 
         # set to None if deactivated_at (nullable) is None
         if self.deactivated_at is None:
             _dict['deactivated_at'] = None
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, StrictStr
 
 class SOLStakeTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    unsigned_tx_hash: StrictStr = ...
-    unsigned_tx_serialized: StrictStr = ...
+    unsigned_tx_hash: Optional[StrictStr] = None
+    unsigned_tx_serialized: Optional[StrictStr] = None
     __properties = ["unsigned_tx_hash", "unsigned_tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/soltx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/soltx_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class SOLTxStatus(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    status: StrictStr = Field(..., description="Transaction status")
+    status: Optional[StrictStr] = Field(None, description="Transaction status")
     receipt: Optional[Dict[str, Any]] = None
     __properties = ["status", "receipt"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_daily_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_daily_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_signed_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtz_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtztx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtztx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/models/xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/models/xtztx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/rest.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_accounts_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_core_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_kiln_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_deposit.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_deposit.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_reward.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `ETHReward`
         """
         model = kiln_connect.openapi_client.models.eth_reward.ETHReward()  # noqa: E501
         if include_optional :
             return ETHReward(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023', 
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
                 consensus_rewards = '2988504000000000', 
                 execution_rewards = '0', 
                 rewards = '2988504000000000', 
                 stake_balance = '64000000000000000000', 
                 gross_apy = 3.407, 
                 cl_apy = 3.407, 
                 el_apy = 0.0
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_signed_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_accounts200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # uncomment below to create an instance of `GetEthRewards200Response`
         """
         model = kiln_connect.openapi_client.models.get_eth_rewards200_response.GetEthRewards200Response()  # noqa: E501
         if include_optional :
             return GetEthRewards200Response(
                 data = [
                     kiln_connect.openapi_client.models.eth_reward.ETHReward(
-                        date = 'Sun Jan 15 00:00:00 GMT 2023', 
+                        date = 'Sun Jan 15 00:00:00 UTC 2023', 
                         consensus_rewards = '2988504000000000', 
                         execution_rewards = '0', 
                         rewards = '2988504000000000', 
                         stake_balance = '64000000000000000000', 
                         gross_apy = 3.407, 
                         cl_apy = 3.407, 
                         el_apy = 0.0, )
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,24 +40,20 @@
         if include_optional :
             return GetSolRewards200ResponseDataInner(
                 epoch = 120, 
                 epoch_ts = '2023-01-14T01:13:59Z', 
                 rewards = '1000', 
                 active_balance = '1000', 
                 net_apy = 3.407, 
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023'
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023'
             )
         else :
             return GetSolRewards200ResponseDataInner(
                 epoch = 120,
-                epoch_ts = '2023-01-14T01:13:59Z',
-                rewards = '1000',
-                active_balance = '1000',
-                net_apy = 3.407,
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023',
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
         )
         """
 
     def testGetSolRewards200ResponseDataInner(self):
         """Test GetSolRewards200ResponseDataInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         # uncomment below to create an instance of `GetSolStakes200Response`
         """
         model = kiln_connect.openapi_client.models.get_sol_stakes200_response.GetSolStakes200Response()  # noqa: E501
         if include_optional :
             return GetSolStakes200Response(
                 data = [
                     kiln_connect.openapi_client.models.sol_stake.SOLStake(
-                        stake_account = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye', 
-                        vote_account = 'EHrKMrVsNNqBjYuKbuzf5rJZcu89dg5cwdRduMdSE557', 
-                        withdraw_pubkey = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye', 
+                        stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
+                        vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
+                        withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
                         state = 'active', 
                         activated_at = '2023-01-14T01:13:59Z', 
                         activated_epoch = 150, 
                         deactivated_at = '2023-01-14T01:13:59Z', 
                         deactivated_epoch = 150, 
                         delegated_epoch = 150, 
                         balance = '1000000000',
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,24 +35,24 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `GetXtzRewards200ResponseDataInner`
         """
         model = kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner.GetXtzRewards200ResponseDataInner()  # noqa: E501
         if include_optional :
             return GetXtzRewards200ResponseDataInner(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023', 
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
                 rewards = '27098488', 
                 active_balance = '34329999165', 
                 gross_apy = 36.053, 
                 cycle = 271, 
                 cycle_begins_at = '2022-09-01T08:44Z'
             )
         else :
             return GetXtzRewards200ResponseDataInner(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023',
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
                 cycle = 271,
                 cycle_begins_at = '2022-09-01T08:44Z',
         )
         """
 
     def testGetXtzRewards200ResponseDataInner(self):
         """Test GetXtzRewards200ResponseDataInner"""
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_account201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,21 @@
     def test_get_sol_network_stats(self):
         """Test case for get_sol_network_stats
 
         Network Stats  # noqa: E501
         """
         pass
 
+    def test_get_sol_operations(self):
+        """Test case for get_sol_operations
+
+        Operations  # noqa: E501
+        """
+        pass
+
     def test_get_sol_reports(self):
         """Test case for get_sol_reports
 
         Reports  # noqa: E501
         """
         pass
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         model = kiln_connect.openapi_client.models.sol_broadcast_tx.SOLBroadcastTx()  # noqa: E501
         if include_optional :
             return SOLBroadcastTx(
                 tx_hash = ''
             )
         else :
             return SOLBroadcastTx(
-                tx_hash = '',
         )
         """
 
     def testSOLBroadcastTx(self):
         """Test SOLBroadcastTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_network_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,14 @@
             return SOLNetworkStats(
                 network_gross_apy = 4.5, 
                 supply_staked_percent = 12.4, 
                 nb_validators = 402
             )
         else :
             return SOLNetworkStats(
-                network_gross_apy = 4.5,
-                supply_staked_percent = 12.4,
-                nb_validators = 402,
         )
         """
 
     def testSOLNetworkStats(self):
         """Test SOLNetworkStats"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,24 +37,24 @@
         # uncomment below to create an instance of `SOLPostStakesPayload`
         """
         model = kiln_connect.openapi_client.models.sol_post_stakes_payload.SOLPostStakesPayload()  # noqa: E501
         if include_optional :
             return SOLPostStakesPayload(
                 stakes = [
                     kiln_connect.openapi_client.models.sol_post_stakes_payload_stakes_inner.SOLPostStakesPayload_stakes_inner(
-                        stake_account = '8nPu8b7ty2Ni99QoSpZudCBoWXk6dFKbaPcBfSwYR81T', 
+                        stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
                         balance = 1000000, )
                     ], 
                 account_id = '92f5bfd4-ea38-4824-84f7-686eddff5539'
             )
         else :
             return SOLPostStakesPayload(
                 stakes = [
                     kiln_connect.openapi_client.models.sol_post_stakes_payload_stakes_inner.SOLPostStakesPayload_stakes_inner(
-                        stake_account = '8nPu8b7ty2Ni99QoSpZudCBoWXk6dFKbaPcBfSwYR81T', 
+                        stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
                         balance = 1000000, )
                     ],
                 account_id = '92f5bfd4-ea38-4824-84f7-686eddff5539',
         )
         """
 
     def testSOLPostStakesPayload(self):
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SOLPostStakesPayloadStakesInner`
         """
         model = kiln_connect.openapi_client.models.sol_post_stakes_payload_stakes_inner.SOLPostStakesPayloadStakesInner()  # noqa: E501
         if include_optional :
             return SOLPostStakesPayloadStakesInner(
-                stake_account = '8nPu8b7ty2Ni99QoSpZudCBoWXk6dFKbaPcBfSwYR81T', 
+                stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
                 balance = 1000000
             )
         else :
             return SOLPostStakesPayloadStakesInner(
         )
         """
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_prepared_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_prepared_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         model = kiln_connect.openapi_client.models.sol_prepared_tx.SOLPreparedTx()  # noqa: E501
         if include_optional :
             return SOLPreparedTx(
                 signed_tx_serialized = ''
             )
         else :
             return SOLPreparedTx(
-                signed_tx_serialized = '',
         )
         """
 
     def testSOLPreparedTx(self):
         """Test SOLPreparedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_reward_by_day.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_reward_by_day.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,25 +35,22 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SOLRewardByDay`
         """
         model = kiln_connect.openapi_client.models.sol_reward_by_day.SOLRewardByDay()  # noqa: E501
         if include_optional :
             return SOLRewardByDay(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023', 
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
                 rewards = '1000', 
                 active_balance = '1000', 
                 net_apy = 3.407
             )
         else :
             return SOLRewardByDay(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023',
-                rewards = '1000',
-                active_balance = '1000',
-                net_apy = 3.407,
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
         )
         """
 
     def testSOLRewardByDay(self):
         """Test SOLRewardByDay"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,14 @@
                 rewards = '1000', 
                 active_balance = '1000', 
                 net_apy = 3.407
             )
         else :
             return SOLRewardByEpoch(
                 epoch = 120,
-                epoch_ts = '2023-01-14T01:13:59Z',
-                rewards = '1000',
-                active_balance = '1000',
-                net_apy = 3.407,
         )
         """
 
     def testSOLRewardByEpoch(self):
         """Test SOLRewardByEpoch"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,38 +35,30 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SOLStake`
         """
         model = kiln_connect.openapi_client.models.sol_stake.SOLStake()  # noqa: E501
         if include_optional :
             return SOLStake(
-                stake_account = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye', 
-                vote_account = 'EHrKMrVsNNqBjYuKbuzf5rJZcu89dg5cwdRduMdSE557', 
-                withdraw_pubkey = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye', 
+                stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
+                vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
+                withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
                 state = 'active', 
                 activated_at = '2023-01-14T01:13:59Z', 
                 activated_epoch = 150, 
                 deactivated_at = '2023-01-14T01:13:59Z', 
                 deactivated_epoch = 150, 
                 delegated_epoch = 150, 
                 balance = '1000000000', 
                 rewards = '1000000000', 
                 net_apy = 3.407, 
                 updated_at = '2023-01-14T01:13:59Z'
             )
         else :
             return SOLStake(
-                stake_account = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye',
-                vote_account = 'EHrKMrVsNNqBjYuKbuzf5rJZcu89dg5cwdRduMdSE557',
-                withdraw_pubkey = '5i5tXdoQ4hWKPqys7MLwq2H9L4PYDYPR5RN3ueheMQye',
-                state = 'active',
-                balance = '1000000000',
-                rewards = '1000000000',
-                net_apy = 3.407,
-                updated_at = '2023-01-14T01:13:59Z',
         )
         """
 
     def testSOLStake(self):
         """Test SOLStake"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake_tx.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,14 @@
         if include_optional :
             return SOLStakeTx(
                 unsigned_tx_hash = '', 
                 unsigned_tx_serialized = ''
             )
         else :
             return SOLStakeTx(
-                unsigned_tx_hash = '',
-                unsigned_tx_serialized = '',
         )
         """
 
     def testSOLStakeTx(self):
         """Test SOLStakeTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_soltx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_soltx_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         if include_optional :
             return SOLTxStatus(
                 status = 'success', 
                 receipt = None
             )
         else :
             return SOLTxStatus(
-                status = 'success',
         )
         """
 
     def testSOLTxStatus(self):
         """Test SOLTxStatus"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_api.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_daily_reward.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_daily_reward.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `XTZDailyReward`
         """
         model = kiln_connect.openapi_client.models.xtz_daily_reward.XTZDailyReward()  # noqa: E501
         if include_optional :
             return XTZDailyReward(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023', 
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
                 rewards = '27098488', 
                 active_balance = '420000000000', 
                 gross_apy = 3.42
             )
         else :
             return XTZDailyReward(
-                var_date = 'Sun Jan 15 00:00:00 GMT 2023',
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
         )
         """
 
     def testXTZDailyReward(self):
         """Test XTZDailyReward"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_network_stats.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_signed_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_stake.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtztx_status.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtztx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev4/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/kiln_connect/xtz.py` & `kiln_connect-1.0.0.dev4/kiln_connect/xtz.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev3/pyproject.toml` & `kiln_connect-1.0.0.dev4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiln-connect"
-version = "1.0.0-dev3"
+version = "1.0.0-dev4"
 description = ""
 authors = ["s. rannou <mxs@sbrk.org>"]
 maintainers = ["s. rannou <mxs@sbrk.org>"]
 readme = "docs/README.md"
 homepage = "https://kiln.fi/"
 repository = "https://github.com/kilnfi/sdk-py"
 keywords = ["staking", "blockchain"]
```

### Comparing `kiln_connect-1.0.0.dev3/PKG-INFO` & `kiln_connect-1.0.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiln-connect
-Version: 1.0.0.dev3
+Version: 1.0.0.dev4
 Summary: 
 Home-page: https://kiln.fi/
 Keywords: staking,blockchain
 Author: s. rannou
 Author-email: mxs@sbrk.org
 Maintainer: s. rannou
 Maintainer-email: mxs@sbrk.org
```

