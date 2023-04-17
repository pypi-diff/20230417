# Comparing `tmp/idem-azure-0.3.2.tar.gz` & `tmp/idem-azure-0.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-azure-0.3.2.tar", last modified: Tue Apr 11 13:23:00 2023, max compression
+gzip compressed data, was "idem-azure-0.3.2.1.tar", last modified: Mon Apr 17 14:46:29 2023, max compression
```

## Comparing `idem-azure-0.3.2.tar` & `idem-azure-0.3.2.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-04-11 13:22:45.000000 idem-azure-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7784 2023-04-11 13:23:00.002657 idem-azure-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6904 2023-04-11 13:22:45.000000 idem-azure-0.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/azure/
--rw-r--r--   0 root         (0) root         (0)     1994 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/azure/login.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/azure/mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/metadata/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/backup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/backup/virtual_networks/
--rw-r--r--   0 root         (0) root         (0)    10446 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/nat_gateways.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/routes.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     3940 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/compute/
--rw-r--r--   0 root         (0) root         (0)     4226 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/network/
--rw-r--r--   0 root         (0) root         (0)     3877 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     4221 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     3946 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/virtual_networks.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3193 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3948 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)     4116 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     4191 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/pop_create/azure/
--rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/api_reference.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/api_spec.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/init.py
--rw-r--r--   0 root         (0) root         (0)     5085 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/resource.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/rest.py
--rw-r--r--   0 root         (0) root         (0)    11179 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/reconcile/pending/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)    10160 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)    12622 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16304 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    19615 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)    11659 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/network/
--rw-r--r--   0 root         (0) root         (0)    15838 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)    14921 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    15532 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    15488 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    16001 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    13954 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)    12656 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    17142 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    15676 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    14926 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/policy/
--rw-r--r--   0 root         (0) root         (0)    12283 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)    11624 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    29668 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/states/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     8445 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)    11477 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     2377 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     7362 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16498 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    31418 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     4329 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/network/
--rw-r--r--   0 root         (0) root         (0)     6983 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     7073 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    14334 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     8907 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    13498 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3795 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_assignment.py
--rw-r--r--   0 root         (0) root         (0)     6870 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_definition.py
--rw-r--r--   0 root         (0) root         (0)     5513 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3308 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    52455 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     3956 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/subscription/subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/validators/
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/validators/http.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7784 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4368 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 13:23:00.002657 idem-azure-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2792 2023-04-11 13:22:45.000000 idem-azure-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6904 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/acct/azure/
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/acct/azure/login.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/acct/azure/mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/acct/metadata/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/backup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/nat_gateways.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/routes.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/network/virtual_networks.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/exec/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/exec/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/pop_create/azure/
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/api_reference.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/api_spec.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/init.py
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/rest.py
+-rw-r--r--   0 root         (0) root         (0)    11179 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/pop_create/azure/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/reconcile/pending/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.464121 idem-azure-0.3.2.1/idem_azure/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)    10160 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16304 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    19615 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)    11659 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/network/
+-rw-r--r--   0 root         (0) root         (0)    15838 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    14921 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    15532 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    15488 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    16001 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    13954 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    17142 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    15676 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)    11624 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    29668 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/states/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     8445 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)    11477 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/states/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     7362 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16498 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    31418 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     4329 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     6983 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    14334 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    13498 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/policy/policy_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     6870 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/policy/policy_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    52455 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/subscription/subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/azure/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.472122 idem-azure-0.3.2.1/idem_azure/tool/validators/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/idem_azure/tool/validators/http.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-17 14:46:28.000000 idem-azure-0.3.2.1/idem_azure/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:46:29.468121 idem-azure-0.3.2.1/idem_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-04-17 14:46:29.000000 idem-azure-0.3.2.1/idem_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-17 14:46:29.000000 idem-azure-0.3.2.1/idem_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:46:29.000000 idem-azure-0.3.2.1/idem_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-17 14:46:29.000000 idem-azure-0.3.2.1/idem_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 14:46:29.000000 idem-azure-0.3.2.1/idem_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-17 14:46:29.476122 idem-azure-0.3.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-04-17 14:46:15.000000 idem-azure-0.3.2.1/setup.py
```

### Comparing `idem-azure-0.3.2/LICENSE` & `idem-azure-0.3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/PKG-INFO` & `idem-azure-0.3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.2
+Version: 0.3.2.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.2/README.rst` & `idem-azure-0.3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/acct/azure/login.py` & `idem-azure-0.3.2.1/idem_azure/acct/azure/login.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/acct/azure/mock.py` & `idem-azure-0.3.2.1/idem_azure/acct/azure/mock.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/backup/virtual_networks/nat_gateways.py` & `idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/backup/virtual_networks/public_ip_addresses.py` & `idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/backup/virtual_networks/routes.py` & `idem-azure-0.3.2.1/idem_azure/backup/virtual_networks/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/conf.py` & `idem-azure-0.3.2.1/idem_azure/conf.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_assignments.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_definitions.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/compute/virtual_machines.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/compute/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/management_groups/management_groups.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/firewall.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/firewall_policies.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/network_interfaces.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/network_security_groups.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/route_tables.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/routes.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/security_rules.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/subnets.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/network/virtual_networks.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/permission.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/permission.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_assignments.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/policy/policy_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_definitions.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/subscription/attach_subscriptions.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/exec/azure/subscription/subscriptions.py` & `idem-azure-0.3.2.1/idem_azure/exec/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/api_reference.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/api_reference.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/api_spec.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/api_spec.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/init.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/init.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/plugin.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/resource.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/resource.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/rest.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/rest.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/pop_create/azure/template.py` & `idem-azure-0.3.2.1/idem_azure/pop_create/azure/template.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/reconcile/pending/azure.py` & `idem-azure-0.3.2.1/idem_azure/reconcile/pending/azure.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/authorization/role_assignments.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/authorization/role_definitions.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/compute/virtual_machines.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/compute/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/management_groups/management_groups.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/firewall.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/firewall_policies.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/network_interfaces.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/network_security_groups.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/route_tables.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/routes.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/security_rules.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/subnets.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/network/virtual_networks.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/policy/policy_assignments.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/policy/policy_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/policy/policy_definitions.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/storage_resource_provider/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/subscription/attach_subscriptions.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/states/azure/subscription/subscriptions.py` & `idem-azure-0.3.2.1/idem_azure/states/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_assignments.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_definitions.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/compute/virtual_machines.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/compute/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/container.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/container.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/management_groups/management_groups.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/firewall.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/firewall_policies.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/network_interfaces.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/network_security_groups.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/route_tables.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/routes.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/security_rules.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/subnets.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/network/virtual_networks.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_assignment.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/policy/policy_assignment.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_definition.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/request.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/request.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/subscription/subscriptions.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/test_state_utils.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/azure/uri.py` & `idem-azure-0.3.2.1/idem_azure/tool/azure/uri.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure/tool/validators/http.py` & `idem-azure-0.3.2.1/idem_azure/tool/validators/http.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/idem_azure.egg-info/PKG-INFO` & `idem-azure-0.3.2.1/idem_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.2
+Version: 0.3.2.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.2/idem_azure.egg-info/SOURCES.txt` & `idem-azure-0.3.2.1/idem_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.2/setup.py` & `idem-azure-0.3.2.1/setup.py`

 * *Files identical despite different names*

