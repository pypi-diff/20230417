# Comparing `tmp/bimdata-api-client-9.8.1.tar.gz` & `tmp/bimdata-api-client-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimdata-api-client-9.8.1.tar", last modified: Tue Dec 20 14:24:37 2022, max compression
+gzip compressed data, was "bimdata-api-client-9.9.0.tar", last modified: Thu Jan  5 14:09:01 2023, max compression
```

## Comparing `bimdata-api-client-9.8.1.tar` & `bimdata-api-client-9.9.0.tar`

### file list

```diff
@@ -1,534 +1,532 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.722050 bimdata-api-client-9.8.1/
--rw-r--r--   0 runner    (1000) runner    (1000)   121260 2022-12-20 14:24:37.722050 bimdata-api-client-9.8.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)   120961 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.678050 bimdata-api-client-9.8.1/bimdata_api_client/
--rw-r--r--   0 runner    (1000) runner    (1000)      931 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.682050 bimdata-api-client-9.8.1/bimdata_api_client/api/
--rw-r--r--   0 runner    (1000) runner    (1000)      218 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   290191 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/bcf_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)   195944 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/checker_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)   603258 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)  1000398 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/ifc_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)   926406 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/model_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24783 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/sso_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32630 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api/webhook_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37802 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/api_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.682050 bimdata-api-client-9.8.1/bimdata_api_client/apis/
--rw-r--r--   0 runner    (1000) runner    (1000)      795 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/apis/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18045 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/configuration.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5221 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.702050 bimdata-api-client-9.8.1/bimdata_api_client/model/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11661 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/bcf_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11363 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/bcf_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12146 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/building.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11230 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/building_model_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12620 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/check_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/check_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13295 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/check_project_access.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12359 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/checker_result.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12057 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/checker_result_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12068 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/classification.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11925 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11780 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/clipping_plane.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11901 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/clipping_plane_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14175 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/cloud.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12218 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11920 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_invitation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11811 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11649 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11723 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/coloring.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11823 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/coloring_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13203 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/comment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13156 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11995 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/component.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12016 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12197 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/components_parent.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12347 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/components_parent_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11386 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/create_building_by_name_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11386 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/create_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11340 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/create_multi_page_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12706 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/detailed_extensions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11506 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/direction.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11527 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/direction_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16433 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/document.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11756 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/document_with_element_list.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13528 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/element.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11688 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/element_classification_relation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11778 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/element_classification_relation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11747 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/element_property_set_relation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13188 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13348 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/extensions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11710 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/feature.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11760 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/feature_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15011 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11905 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_group_permission.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11976 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_group_permission_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11471 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13121 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_user_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14657 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_without_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12167 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/folder_without_children_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17626 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/full_topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17846 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/full_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12100 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12385 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/group_folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11634 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11619 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_access_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11452 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13426 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_checker.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11503 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_checker_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_export_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12336 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_merge_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11657 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_optimize_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11900 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/import_group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14730 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/label.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11699 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/label_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12225 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/layer.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12006 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/layer_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11921 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/layer_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12140 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11674 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/line.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11766 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/line_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15959 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11555 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11287 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_image_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14634 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12268 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/material.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11792 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/material_list_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11467 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/material_list_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11786 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/material_option.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11577 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/material_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19942 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11669 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11690 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_errors_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13013 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_files.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12938 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_property.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14233 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12689 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/model_with_positioning_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12389 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11608 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/organization_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12666 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/orthogonal_camera.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12808 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/orthogonal_camera_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11344 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_bcf_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11936 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_check_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12078 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_checker_result_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11946 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11792 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_cloud_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13177 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14315 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_document_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13169 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12148 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_folder_without_children_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17789 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_full_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11532 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_group_folder_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11615 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11473 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ifc_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11524 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ifc_checker_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11672 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_label_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12085 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14254 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12262 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_positioning_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11977 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_priority_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11687 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_processor_handler_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11831 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_project_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12066 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12841 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11944 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12142 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13016 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_rule_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12295 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_rule_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12528 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ruleset_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11859 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11672 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_stage_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11283 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_storey_building_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12370 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11605 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_tag_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16973 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12010 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_status_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11714 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_type_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14548 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11339 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_user_cloud_update_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11500 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_user_project_update_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16460 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_viewpoint_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11601 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11922 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11318 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_validation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11764 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_web_hook_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12759 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_zone_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11871 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/patched_zone_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12899 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/perspective_camera.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13062 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/perspective_camera_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11906 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/pin.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11977 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/pin_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11494 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/point.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11515 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/point_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12220 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/positioning_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12107 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/priority.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12022 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/priority_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11990 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/processor_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13337 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12002 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_access_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11864 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11650 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_folder_tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12272 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12216 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_invitation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12085 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11693 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11518 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_size.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13171 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/project_with_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12934 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/property_definition.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12820 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/property_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12001 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12696 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/property_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12121 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11693 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/public_organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11626 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/public_organization_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11863 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_classification.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11720 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12298 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_definition.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12155 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12856 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12999 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14233 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_elements.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14633 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_elements_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11826 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_layer.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11712 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12270 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12389 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11696 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_components.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11553 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_components_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12560 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11682 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_options.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11539 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_options_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12156 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11670 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12294 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12230 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11910 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_system.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11992 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13528 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_unit.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13475 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/raw_unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18313 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/recursive_folder_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12214 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13138 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/rule_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12995 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/rule_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12237 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/rule_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12410 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ruleset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12428 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/ruleset_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12090 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/self_bcf_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14462 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/self_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11479 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/simple_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14548 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/size.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11664 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/snapshot.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11732 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/snapshot_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12611 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/space.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11880 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/stage.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11699 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/stage_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12138 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/storey.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11304 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/storey_building_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11224 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/storey_model_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12529 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/system.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12415 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11709 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/tag.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11238 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/tag_id_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11624 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/tag_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16924 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17030 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12164 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12079 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic_status_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11856 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11771 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/topic_type_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14426 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/unit.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14394 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13312 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/user.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14096 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/user_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12786 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/user_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11350 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/user_project_id_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11755 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/view_setup_hints.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11776 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/view_setup_hints_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15762 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/viewpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16439 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/viewpoint_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14169 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12453 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa_comment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11580 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11901 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12861 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa_validation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11385 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visa_validation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12177 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visibility.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12298 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/visibility_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11883 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/web_hook.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11827 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/web_hook_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12419 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/write_folder_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13130 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/zone.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12671 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/zone_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12623 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/zone_space.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11892 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model/zone_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    82239 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/model_utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.702050 bimdata-api-client-9.8.1/bimdata_api_client/models/
--rw-r--r--   0 runner    (1000) runner    (1000)    18330 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/bimdata_api_client/models/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14349 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/bimdata_api_client/rest.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.678050 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)   121260 2022-12-20 14:24:37.000000 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)    20337 2022-12-20 14:24:37.000000 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-12-20 14:24:37.000000 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       86 2022-12-20 14:24:37.000000 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       24 2022-12-20 14:24:37.000000 bimdata-api-client-9.8.1/bimdata_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      248 2022-12-20 14:24:37.722050 bimdata-api-client-9.8.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1235 2022-12-20 14:24:35.000000 bimdata-api-client-9.8.1/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-12-20 14:24:37.722050 bimdata-api-client-9.8.1/test/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8819 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_bcf_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_bcf_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_bcf_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1033 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_building.py
--rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_building_model_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_check_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1049 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_check_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_check_project_access.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5440 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_checker_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_checker_result.py
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_checker_result_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      920 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_classification.py
--rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1082 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_clipping_plane.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_clipping_plane_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1230 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_cloud.py
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_cloud_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_cloud_invitation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_cloud_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_cloud_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17421 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_collaboration_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_coloring.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1049 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_coloring_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      871 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_comment.py
--rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      885 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1211 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_components_parent.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1348 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_components_parent_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1015 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_create_building_by_name_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_create_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1015 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_create_multi_page_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1383 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_detailed_extensions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      885 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_direction.py
--rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_direction_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1090 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_document.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1074 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_document_with_element_list.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1331 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1027 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_element_classification_relation.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1077 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_element_classification_relation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1057 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_element_property_set_relation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1326 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      892 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_extensions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      871 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_feature.py
--rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_feature_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1228 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1047 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_group_permission.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1126 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_group_permission_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_user_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1185 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_without_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_folder_without_children_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_full_topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1170 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_full_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      958 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1118 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_group_folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_access_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31332 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_ifc_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1243 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_checker.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_checker_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_export_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      929 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_merge_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ifc_optimize_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_import_group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      892 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_label.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_label_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_layer.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_layer_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_layer_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      926 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_line.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1005 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_line_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1256 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_marketplace_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_marketplace_app_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1007 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_marketplace_app_image_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_marketplace_app_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      979 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_material.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1172 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_material_list_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1138 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_material_list_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_material_option.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1058 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_material_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1017 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26269 2022-12-20 14:24:19.000000 bimdata-api-client-9.8.1/test/test_model_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_errors_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_files.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1043 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_property.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_model_with_positioning_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)      906 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)      956 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_organization_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1103 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_orthogonal_camera.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1211 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_orthogonal_camera_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_bcf_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1099 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_check_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_checker_result_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1020 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_cloud_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_document_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1376 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1071 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_folder_without_children_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1220 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_full_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_group_folder_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_group_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_ifc_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_ifc_checker_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_label_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_model_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1028 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_positioning_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_priority_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1035 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_processor_handler_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_project_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1150 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_property_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1136 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1117 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_rule_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1189 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_rule_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1185 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_ruleset_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_stage_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_storey_building_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_tag_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_topic_status_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      986 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_topic_type_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1051 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1029 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_user_cloud_update_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1043 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_user_project_update_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1892 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_viewpoint_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_visa_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_visa_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_visa_validation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_web_hook_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1156 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_zone_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      986 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_patched_zone_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1110 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_perspective_camera.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1218 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_perspective_camera_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      919 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_pin.py
--rw-r--r--   0 runner    (1000) runner    (1000)      998 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_pin_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_point.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_point_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_positioning_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)      878 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_priority.py
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_priority_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_processor_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      947 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_access_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_access_token_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1040 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_folder_tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)      942 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)      992 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_invitation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_size.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_project_with_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_property_definition.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1100 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_property_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1086 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1009 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_property_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      949 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_public_organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)      999 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_public_organization_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      942 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_classification.py
--rw-r--r--   0 runner    (1000) runner    (1000)      992 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_classification_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_definition.py
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_definition_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_element_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1730 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_elements.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2012 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_elements_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      879 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_layer.py
--rw-r--r--   0 runner    (1000) runner    (1000)      929 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_layer_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1319 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_list.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_list_components.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_list_components_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1456 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_list_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_options.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_options_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_material_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_property.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_property_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1023 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_property_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1102 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_property_set_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_system.py
--rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      872 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_unit.py
--rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_raw_unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1355 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_recursive_folder_children.py
--rw-r--r--   0 runner    (1000) runner    (1000)      959 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_rule_component.py
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_rule_component_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1038 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_rule_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ruleset.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_ruleset_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      901 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_self_bcf_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1177 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_self_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_simple_element.py
--rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_size.py
--rw-r--r--   0 runner    (1000) runner    (1000)      878 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_snapshot.py
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_snapshot_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_space.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_space_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1445 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_sso_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_stage.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_stage_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1019 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_storey.py
--rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_storey_building_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      979 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_storey_model_plan_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      864 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_system.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_system_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      843 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_tag.py
--rw-r--r--   0 runner    (1000) runner    (1000)      908 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_tag_id_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_tag_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic_status_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_topic_type_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_unit.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_unit_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_user.py
--rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_user_invitation.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_user_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_user_project_id_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_view_setup_hints.py
--rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_view_setup_hints_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1589 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_viewpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1842 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_viewpoint_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1165 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1001 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa_comment.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa_comment_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa_validation.py
--rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visa_validation_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1098 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visibility.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1206 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_visibility_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      872 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_web_hook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_web_hook_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1619 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_webhook_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_write_folder_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      926 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_zone.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1005 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_zone_request.py
--rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_zone_space.py
--rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.8.1/test/test_zone_space_request.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:01.025819 bimdata-api-client-9.9.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)   121212 2023-01-05 14:09:01.025819 bimdata-api-client-9.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)   120913 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:00.989818 bimdata-api-client-9.9.0/bimdata_api_client/
+-rw-r--r--   0 runner    (1000) runner    (1000)      931 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:00.993819 bimdata-api-client-9.9.0/bimdata_api_client/api/
+-rw-r--r--   0 runner    (1000) runner    (1000)      218 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   290191 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/bcf_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   195944 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/checker_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   603258 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  1000398 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/ifc_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   926406 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/model_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24783 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/sso_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32630 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api/webhook_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37802 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:00.993819 bimdata-api-client-9.9.0/bimdata_api_client/apis/
+-rw-r--r--   0 runner    (1000) runner    (1000)      795 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18045 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/configuration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5221 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:01.009819 bimdata-api-client-9.9.0/bimdata_api_client/model/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11661 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/bcf_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11363 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/bcf_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12146 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/building.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11230 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/building_model_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12620 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/check_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/check_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13295 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/check_project_access.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12359 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/checker_result.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12057 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/checker_result_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12068 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/classification.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11925 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11780 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/clipping_plane.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11901 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/clipping_plane_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14206 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/cloud.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12218 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11920 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_invitation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11811 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11649 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11723 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/coloring.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11823 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/coloring_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13203 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/comment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13156 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11995 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12016 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12197 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/components_parent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12347 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/components_parent_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11386 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/create_building_by_name_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11386 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/create_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11340 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/create_multi_page_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12706 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/detailed_extensions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11506 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/direction.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11527 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/direction_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16433 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/document.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11756 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/document_with_element_list.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13528 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11688 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/element_classification_relation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11778 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/element_classification_relation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11747 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/element_property_set_relation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13188 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13348 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/extensions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11710 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/feature.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11760 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/feature_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15011 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11905 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_group_permission.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11976 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_group_permission_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11471 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13121 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_user_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14657 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_without_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12167 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/folder_without_children_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17626 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/full_topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17846 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/full_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12100 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12385 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/group_folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11634 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11619 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_access_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11452 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13426 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_checker.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11503 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_checker_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_export_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12336 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_merge_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11657 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_optimize_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11900 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/import_group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14730 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/label.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11699 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/label_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12225 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/layer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12006 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/layer_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11921 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/layer_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12140 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11674 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/line.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11766 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/line_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11555 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12840 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_light.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11871 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_light_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12268 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/material.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11792 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/material_list_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11467 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/material_list_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11786 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/material_option.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11577 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/material_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19942 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11669 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11690 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_errors_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13013 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12938 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_property.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14233 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12689 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/model_with_positioning_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12389 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11608 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/organization_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12666 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/orthogonal_camera.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12808 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/orthogonal_camera_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11344 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_bcf_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11936 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_check_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12078 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_checker_result_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11946 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11792 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_cloud_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13177 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14315 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_document_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13169 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12148 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_folder_without_children_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17789 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_full_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11532 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_group_folder_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11615 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11473 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ifc_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11524 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ifc_checker_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11672 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_label_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12085 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14254 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12262 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_positioning_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11977 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_priority_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11687 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_processor_handler_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11831 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_project_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12066 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12841 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11944 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12142 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13016 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_rule_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12295 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_rule_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12528 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ruleset_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11859 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11672 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_stage_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11283 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_storey_building_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12370 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11605 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_tag_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16973 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12010 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_status_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11714 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_type_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14548 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11339 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_user_cloud_update_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11500 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_user_project_update_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16460 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_viewpoint_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11601 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11922 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11318 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_validation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11764 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_web_hook_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12759 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_zone_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11871 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/patched_zone_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12899 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/perspective_camera.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13062 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/perspective_camera_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11906 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/pin.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11977 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/pin_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11494 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/point.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11515 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/point_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12220 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/positioning_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12107 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/priority.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12022 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/priority_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11990 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/processor_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13337 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12002 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_access_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11864 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11650 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_folder_tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12272 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12216 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_invitation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12085 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11693 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11518 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_size.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13171 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/project_with_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12934 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/property_definition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12820 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/property_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12001 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12696 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/property_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12121 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11693 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/public_organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11626 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/public_organization_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11863 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_classification.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11720 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12298 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_definition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12155 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12856 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12999 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14233 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_elements.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14633 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_elements_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11826 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_layer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11712 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12270 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12389 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11696 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_components.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11553 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_components_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12560 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11682 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_options.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11539 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_options_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12156 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11670 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12294 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12230 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11910 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_system.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11992 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13528 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_unit.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13475 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/raw_unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18201 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/recursive_folder_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12214 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13138 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/rule_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12995 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/rule_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12237 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/rule_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12410 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ruleset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12428 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/ruleset_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12090 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/self_bcf_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14462 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/self_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11479 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/simple_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14548 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/size.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11664 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/snapshot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11732 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/snapshot_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12611 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/space.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11880 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11784 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/stage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11699 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/stage_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12138 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/storey.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11304 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/storey_building_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11224 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/storey_model_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12529 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/system.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12415 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11709 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/tag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11238 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/tag_id_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11624 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/tag_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16924 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17030 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12164 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12079 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic_status_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11856 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11771 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/topic_type_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14426 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/unit.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14394 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13312 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14096 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/user_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12786 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/user_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11350 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/user_project_id_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11755 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/view_setup_hints.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11776 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/view_setup_hints_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15762 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/viewpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16439 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/viewpoint_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14169 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12453 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa_comment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11580 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11901 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12861 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa_validation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11385 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visa_validation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12177 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visibility.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12298 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/visibility_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11883 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/web_hook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11827 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/web_hook_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12419 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/write_folder_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13130 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/zone.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12671 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/zone_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12623 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/zone_space.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11892 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model/zone_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    82239 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/model_utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:01.009819 bimdata-api-client-9.9.0/bimdata_api_client/models/
+-rw-r--r--   0 runner    (1000) runner    (1000)    18258 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/bimdata_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14349 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/bimdata_api_client/rest.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:00.989818 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)   121212 2023-01-05 14:09:00.000000 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)    20260 2023-01-05 14:09:00.000000 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-01-05 14:09:00.000000 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       86 2023-01-05 14:09:00.000000 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       24 2023-01-05 14:09:00.000000 bimdata-api-client-9.9.0/bimdata_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      248 2023-01-05 14:09:01.025819 bimdata-api-client-9.9.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1235 2023-01-05 14:08:58.000000 bimdata-api-client-9.9.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-01-05 14:09:01.025819 bimdata-api-client-9.9.0/test/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8819 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_bcf_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_bcf_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_bcf_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1033 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_building.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_building_model_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_check_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1049 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_check_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_check_project_access.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5440 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_checker_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_checker_result.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_checker_result_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      920 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_classification.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1082 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_clipping_plane.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_clipping_plane_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1251 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/test/test_cloud.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_cloud_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_cloud_invitation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_cloud_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_cloud_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17421 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_collaboration_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      970 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_coloring.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1049 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_coloring_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      871 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_comment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      885 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1211 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_components_parent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1348 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_components_parent_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1015 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_create_building_by_name_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_create_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1015 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_create_multi_page_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1383 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_detailed_extensions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      885 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_direction.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_direction_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1090 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_document.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1074 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_document_with_element_list.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1331 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1027 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_element_classification_relation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1077 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_element_classification_relation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1057 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_element_property_set_relation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1326 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      892 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_extensions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      871 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_feature.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_feature_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1228 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1047 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_group_permission.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1126 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_group_permission_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_user_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1185 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_without_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_folder_without_children_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_full_topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1170 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_full_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      958 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1118 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_group_folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_access_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31332 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_ifc_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1243 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_checker.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_checker_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_export_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      929 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_merge_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ifc_optimize_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_import_group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      892 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_label.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_label_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_layer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_layer_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_layer_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      926 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_line.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1005 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_line_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_marketplace_app_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1220 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/test/test_marketplace_app_light.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1007 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/test/test_marketplace_app_light_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      979 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_material.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1172 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_material_list_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1138 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_material_list_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_material_option.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1058 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_material_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1017 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26269 2022-12-20 14:24:19.000000 bimdata-api-client-9.9.0/test/test_model_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_errors_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1043 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_property.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_model_with_positioning_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      906 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      956 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_organization_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1103 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_orthogonal_camera.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1211 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_orthogonal_camera_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_bcf_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1099 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_check_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_checker_result_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1020 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_cloud_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_document_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1376 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1071 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_folder_without_children_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1220 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_full_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_group_folder_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_group_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_ifc_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_ifc_checker_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_label_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_model_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1028 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_positioning_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      978 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_priority_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1035 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_processor_handler_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_project_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1150 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_property_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1136 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1117 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_rule_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1189 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_rule_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1185 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_ruleset_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_stage_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_storey_building_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_tag_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_topic_status_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      986 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_topic_type_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1051 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1029 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_user_cloud_update_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1043 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_user_project_update_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1892 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_viewpoint_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_visa_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_visa_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_visa_validation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_web_hook_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1156 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_zone_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      986 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_patched_zone_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1110 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_perspective_camera.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1218 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_perspective_camera_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      919 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_pin.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      998 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_pin_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_point.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_point_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_positioning_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      878 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_priority.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_priority_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      935 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_processor_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      947 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_access_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_access_token_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1040 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_folder_tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      942 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      992 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_invitation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      921 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_size.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_project_with_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1021 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_property_definition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1100 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_property_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1086 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1009 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_property_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      949 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_public_organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      999 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_public_organization_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      942 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_classification.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      992 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_classification_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_definition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_definition_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_element_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1730 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_elements.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2012 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_elements_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      879 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_layer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      929 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_layer_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1319 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_list.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_list_components.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_list_components_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1456 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_list_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_options.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_options_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_material_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_property.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_property_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1023 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_property_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1102 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_property_set_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_system.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      872 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_unit.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_raw_unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1125 2023-01-05 14:08:43.000000 bimdata-api-client-9.9.0/test/test_recursive_folder_children.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      959 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_rule_component.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_rule_component_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1038 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_rule_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      943 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ruleset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_ruleset_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      901 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_self_bcf_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1177 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_self_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_simple_element.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_size.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      878 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_snapshot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      928 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_snapshot_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_space.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_space_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1445 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_sso_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_stage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_stage_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1019 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_storey.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_storey_building_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      979 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_storey_model_plan_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      864 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_system.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_system_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      843 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_tag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      908 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_tag_id_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      893 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_tag_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      907 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic_status_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_topic_type_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_unit.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_unit_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      850 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_user.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      993 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_user_invitation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_user_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_user_project_id_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_view_setup_hints.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      972 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_view_setup_hints_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1589 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_viewpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1842 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_viewpoint_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1165 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1001 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa_comment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa_comment_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      900 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1022 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa_validation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      971 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visa_validation_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1098 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visibility.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1206 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_visibility_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      872 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_web_hook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      922 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_web_hook_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1619 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      950 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_write_folder_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      926 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_zone.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1005 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_zone_request.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      886 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_zone_space.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      936 2022-11-30 09:50:11.000000 bimdata-api-client-9.9.0/test/test_zone_space_request.py
```

### Comparing `bimdata-api-client-9.8.1/PKG-INFO` & `bimdata-api-client-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimdata-api-client
-Version: 9.8.1
+Version: 9.9.0
 Summary: BIMData API
 Home-page: https://github.com/bimdata/python-api-client
 Author: BIMData.io
 Author-email: contact@bimdata.io
 License: UNKNOWN
 Keywords: Swagger,BIMData API
 Platform: UNKNOWN
@@ -741,18 +741,17 @@
  - [LabelRequest](docs/LabelRequest.md)
  - [Layer](docs/Layer.md)
  - [LayerElement](docs/LayerElement.md)
  - [LayerElementRequest](docs/LayerElementRequest.md)
  - [LayerRequest](docs/LayerRequest.md)
  - [Line](docs/Line.md)
  - [LineRequest](docs/LineRequest.md)
- - [MarketplaceApp](docs/MarketplaceApp.md)
  - [MarketplaceAppImage](docs/MarketplaceAppImage.md)
- - [MarketplaceAppImageRequest](docs/MarketplaceAppImageRequest.md)
- - [MarketplaceAppRequest](docs/MarketplaceAppRequest.md)
+ - [MarketplaceAppLight](docs/MarketplaceAppLight.md)
+ - [MarketplaceAppLightRequest](docs/MarketplaceAppLightRequest.md)
  - [Material](docs/Material.md)
  - [MaterialListComponent](docs/MaterialListComponent.md)
  - [MaterialListComponentRequest](docs/MaterialListComponentRequest.md)
  - [MaterialOption](docs/MaterialOption.md)
  - [MaterialRequest](docs/MaterialRequest.md)
  - [Model](docs/Model.md)
  - [ModelErrors](docs/ModelErrors.md)
```

### Comparing `bimdata-api-client-9.8.1/README.md` & `bimdata-api-client-9.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6937,625 +6937,622 @@
 0001b180: 2e6d 6429 0a20 2d20 5b4c 6179 6572 5265  .md). - [LayerRe
 0001b190: 7175 6573 745d 2864 6f63 732f 4c61 7965  quest](docs/Laye
 0001b1a0: 7252 6571 7565 7374 2e6d 6429 0a20 2d20  rRequest.md). - 
 0001b1b0: 5b4c 696e 655d 2864 6f63 732f 4c69 6e65  [Line](docs/Line
 0001b1c0: 2e6d 6429 0a20 2d20 5b4c 696e 6552 6571  .md). - [LineReq
 0001b1d0: 7565 7374 5d28 646f 6373 2f4c 696e 6552  uest](docs/LineR
 0001b1e0: 6571 7565 7374 2e6d 6429 0a20 2d20 5b4d  equest.md). - [M
-0001b1f0: 6172 6b65 7470 6c61 6365 4170 705d 2864  arketplaceApp](d
-0001b200: 6f63 732f 4d61 726b 6574 706c 6163 6541  ocs/MarketplaceA
-0001b210: 7070 2e6d 6429 0a20 2d20 5b4d 6172 6b65  pp.md). - [Marke
-0001b220: 7470 6c61 6365 4170 7049 6d61 6765 5d28  tplaceAppImage](
-0001b230: 646f 6373 2f4d 6172 6b65 7470 6c61 6365  docs/Marketplace
-0001b240: 4170 7049 6d61 6765 2e6d 6429 0a20 2d20  AppImage.md). - 
-0001b250: 5b4d 6172 6b65 7470 6c61 6365 4170 7049  [MarketplaceAppI
-0001b260: 6d61 6765 5265 7175 6573 745d 2864 6f63  mageRequest](doc
-0001b270: 732f 4d61 726b 6574 706c 6163 6541 7070  s/MarketplaceApp
-0001b280: 496d 6167 6552 6571 7565 7374 2e6d 6429  ImageRequest.md)
-0001b290: 0a20 2d20 5b4d 6172 6b65 7470 6c61 6365  . - [Marketplace
-0001b2a0: 4170 7052 6571 7565 7374 5d28 646f 6373  AppRequest](docs
-0001b2b0: 2f4d 6172 6b65 7470 6c61 6365 4170 7052  /MarketplaceAppR
-0001b2c0: 6571 7565 7374 2e6d 6429 0a20 2d20 5b4d  equest.md). - [M
-0001b2d0: 6174 6572 6961 6c5d 2864 6f63 732f 4d61  aterial](docs/Ma
-0001b2e0: 7465 7269 616c 2e6d 6429 0a20 2d20 5b4d  terial.md). - [M
-0001b2f0: 6174 6572 6961 6c4c 6973 7443 6f6d 706f  aterialListCompo
-0001b300: 6e65 6e74 5d28 646f 6373 2f4d 6174 6572  nent](docs/Mater
-0001b310: 6961 6c4c 6973 7443 6f6d 706f 6e65 6e74  ialListComponent
-0001b320: 2e6d 6429 0a20 2d20 5b4d 6174 6572 6961  .md). - [Materia
-0001b330: 6c4c 6973 7443 6f6d 706f 6e65 6e74 5265  lListComponentRe
-0001b340: 7175 6573 745d 2864 6f63 732f 4d61 7465  quest](docs/Mate
-0001b350: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
-0001b360: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
-0001b370: 5b4d 6174 6572 6961 6c4f 7074 696f 6e5d  [MaterialOption]
-0001b380: 2864 6f63 732f 4d61 7465 7269 616c 4f70  (docs/MaterialOp
-0001b390: 7469 6f6e 2e6d 6429 0a20 2d20 5b4d 6174  tion.md). - [Mat
-0001b3a0: 6572 6961 6c52 6571 7565 7374 5d28 646f  erialRequest](do
-0001b3b0: 6373 2f4d 6174 6572 6961 6c52 6571 7565  cs/MaterialReque
-0001b3c0: 7374 2e6d 6429 0a20 2d20 5b4d 6f64 656c  st.md). - [Model
-0001b3d0: 5d28 646f 6373 2f4d 6f64 656c 2e6d 6429  ](docs/Model.md)
-0001b3e0: 0a20 2d20 5b4d 6f64 656c 4572 726f 7273  . - [ModelErrors
-0001b3f0: 5d28 646f 6373 2f4d 6f64 656c 4572 726f  ](docs/ModelErro
-0001b400: 7273 2e6d 6429 0a20 2d20 5b4d 6f64 656c  rs.md). - [Model
-0001b410: 4572 726f 7273 5265 7175 6573 745d 2864  ErrorsRequest](d
-0001b420: 6f63 732f 4d6f 6465 6c45 7272 6f72 7352  ocs/ModelErrorsR
-0001b430: 6571 7565 7374 2e6d 6429 0a20 2d20 5b4d  equest.md). - [M
-0001b440: 6f64 656c 4669 6c65 735d 2864 6f63 732f  odelFiles](docs/
-0001b450: 4d6f 6465 6c46 696c 6573 2e6d 6429 0a20  ModelFiles.md). 
-0001b460: 2d20 5b4d 6f64 656c 5072 6f70 6572 7479  - [ModelProperty
-0001b470: 5d28 646f 6373 2f4d 6f64 656c 5072 6f70  ](docs/ModelProp
-0001b480: 6572 7479 2e6d 6429 0a20 2d20 5b4d 6f64  erty.md). - [Mod
-0001b490: 656c 5265 7175 6573 745d 2864 6f63 732f  elRequest](docs/
-0001b4a0: 4d6f 6465 6c52 6571 7565 7374 2e6d 6429  ModelRequest.md)
-0001b4b0: 0a20 2d20 5b4d 6f64 656c 5769 7468 506f  . - [ModelWithPo
-0001b4c0: 7369 7469 6f6e 696e 6750 6c61 6e5d 2864  sitioningPlan](d
-0001b4d0: 6f63 732f 4d6f 6465 6c57 6974 6850 6f73  ocs/ModelWithPos
-0001b4e0: 6974 696f 6e69 6e67 506c 616e 2e6d 6429  itioningPlan.md)
-0001b4f0: 0a20 2d20 5b4f 7267 616e 697a 6174 696f  . - [Organizatio
-0001b500: 6e5d 2864 6f63 732f 4f72 6761 6e69 7a61  n](docs/Organiza
-0001b510: 7469 6f6e 2e6d 6429 0a20 2d20 5b4f 7267  tion.md). - [Org
-0001b520: 616e 697a 6174 696f 6e52 6571 7565 7374  anizationRequest
-0001b530: 5d28 646f 6373 2f4f 7267 616e 697a 6174  ](docs/Organizat
-0001b540: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
+0001b1f0: 6172 6b65 7470 6c61 6365 4170 7049 6d61  arketplaceAppIma
+0001b200: 6765 5d28 646f 6373 2f4d 6172 6b65 7470  ge](docs/Marketp
+0001b210: 6c61 6365 4170 7049 6d61 6765 2e6d 6429  laceAppImage.md)
+0001b220: 0a20 2d20 5b4d 6172 6b65 7470 6c61 6365  . - [Marketplace
+0001b230: 4170 704c 6967 6874 5d28 646f 6373 2f4d  AppLight](docs/M
+0001b240: 6172 6b65 7470 6c61 6365 4170 704c 6967  arketplaceAppLig
+0001b250: 6874 2e6d 6429 0a20 2d20 5b4d 6172 6b65  ht.md). - [Marke
+0001b260: 7470 6c61 6365 4170 704c 6967 6874 5265  tplaceAppLightRe
+0001b270: 7175 6573 745d 2864 6f63 732f 4d61 726b  quest](docs/Mark
+0001b280: 6574 706c 6163 6541 7070 4c69 6768 7452  etplaceAppLightR
+0001b290: 6571 7565 7374 2e6d 6429 0a20 2d20 5b4d  equest.md). - [M
+0001b2a0: 6174 6572 6961 6c5d 2864 6f63 732f 4d61  aterial](docs/Ma
+0001b2b0: 7465 7269 616c 2e6d 6429 0a20 2d20 5b4d  terial.md). - [M
+0001b2c0: 6174 6572 6961 6c4c 6973 7443 6f6d 706f  aterialListCompo
+0001b2d0: 6e65 6e74 5d28 646f 6373 2f4d 6174 6572  nent](docs/Mater
+0001b2e0: 6961 6c4c 6973 7443 6f6d 706f 6e65 6e74  ialListComponent
+0001b2f0: 2e6d 6429 0a20 2d20 5b4d 6174 6572 6961  .md). - [Materia
+0001b300: 6c4c 6973 7443 6f6d 706f 6e65 6e74 5265  lListComponentRe
+0001b310: 7175 6573 745d 2864 6f63 732f 4d61 7465  quest](docs/Mate
+0001b320: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
+0001b330: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
+0001b340: 5b4d 6174 6572 6961 6c4f 7074 696f 6e5d  [MaterialOption]
+0001b350: 2864 6f63 732f 4d61 7465 7269 616c 4f70  (docs/MaterialOp
+0001b360: 7469 6f6e 2e6d 6429 0a20 2d20 5b4d 6174  tion.md). - [Mat
+0001b370: 6572 6961 6c52 6571 7565 7374 5d28 646f  erialRequest](do
+0001b380: 6373 2f4d 6174 6572 6961 6c52 6571 7565  cs/MaterialReque
+0001b390: 7374 2e6d 6429 0a20 2d20 5b4d 6f64 656c  st.md). - [Model
+0001b3a0: 5d28 646f 6373 2f4d 6f64 656c 2e6d 6429  ](docs/Model.md)
+0001b3b0: 0a20 2d20 5b4d 6f64 656c 4572 726f 7273  . - [ModelErrors
+0001b3c0: 5d28 646f 6373 2f4d 6f64 656c 4572 726f  ](docs/ModelErro
+0001b3d0: 7273 2e6d 6429 0a20 2d20 5b4d 6f64 656c  rs.md). - [Model
+0001b3e0: 4572 726f 7273 5265 7175 6573 745d 2864  ErrorsRequest](d
+0001b3f0: 6f63 732f 4d6f 6465 6c45 7272 6f72 7352  ocs/ModelErrorsR
+0001b400: 6571 7565 7374 2e6d 6429 0a20 2d20 5b4d  equest.md). - [M
+0001b410: 6f64 656c 4669 6c65 735d 2864 6f63 732f  odelFiles](docs/
+0001b420: 4d6f 6465 6c46 696c 6573 2e6d 6429 0a20  ModelFiles.md). 
+0001b430: 2d20 5b4d 6f64 656c 5072 6f70 6572 7479  - [ModelProperty
+0001b440: 5d28 646f 6373 2f4d 6f64 656c 5072 6f70  ](docs/ModelProp
+0001b450: 6572 7479 2e6d 6429 0a20 2d20 5b4d 6f64  erty.md). - [Mod
+0001b460: 656c 5265 7175 6573 745d 2864 6f63 732f  elRequest](docs/
+0001b470: 4d6f 6465 6c52 6571 7565 7374 2e6d 6429  ModelRequest.md)
+0001b480: 0a20 2d20 5b4d 6f64 656c 5769 7468 506f  . - [ModelWithPo
+0001b490: 7369 7469 6f6e 696e 6750 6c61 6e5d 2864  sitioningPlan](d
+0001b4a0: 6f63 732f 4d6f 6465 6c57 6974 6850 6f73  ocs/ModelWithPos
+0001b4b0: 6974 696f 6e69 6e67 506c 616e 2e6d 6429  itioningPlan.md)
+0001b4c0: 0a20 2d20 5b4f 7267 616e 697a 6174 696f  . - [Organizatio
+0001b4d0: 6e5d 2864 6f63 732f 4f72 6761 6e69 7a61  n](docs/Organiza
+0001b4e0: 7469 6f6e 2e6d 6429 0a20 2d20 5b4f 7267  tion.md). - [Org
+0001b4f0: 616e 697a 6174 696f 6e52 6571 7565 7374  anizationRequest
+0001b500: 5d28 646f 6373 2f4f 7267 616e 697a 6174  ](docs/Organizat
+0001b510: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
+0001b520: 2d20 5b4f 7274 686f 676f 6e61 6c43 616d  - [OrthogonalCam
+0001b530: 6572 615d 2864 6f63 732f 4f72 7468 6f67  era](docs/Orthog
+0001b540: 6f6e 616c 4361 6d65 7261 2e6d 6429 0a20  onalCamera.md). 
 0001b550: 2d20 5b4f 7274 686f 676f 6e61 6c43 616d  - [OrthogonalCam
-0001b560: 6572 615d 2864 6f63 732f 4f72 7468 6f67  era](docs/Orthog
-0001b570: 6f6e 616c 4361 6d65 7261 2e6d 6429 0a20  onalCamera.md). 
-0001b580: 2d20 5b4f 7274 686f 676f 6e61 6c43 616d  - [OrthogonalCam
-0001b590: 6572 6152 6571 7565 7374 5d28 646f 6373  eraRequest](docs
-0001b5a0: 2f4f 7274 686f 676f 6e61 6c43 616d 6572  /OrthogonalCamer
-0001b5b0: 6152 6571 7565 7374 2e6d 6429 0a20 2d20  aRequest.md). - 
-0001b5c0: 5b50 6174 6368 6564 4263 6650 726f 6a65  [PatchedBcfProje
-0001b5d0: 6374 5265 7175 6573 745d 2864 6f63 732f  ctRequest](docs/
-0001b5e0: 5061 7463 6865 6442 6366 5072 6f6a 6563  PatchedBcfProjec
-0001b5f0: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
-0001b600: 5b50 6174 6368 6564 4368 6563 6b50 6c61  [PatchedCheckPla
-0001b610: 6e52 6571 7565 7374 5d28 646f 6373 2f50  nRequest](docs/P
-0001b620: 6174 6368 6564 4368 6563 6b50 6c61 6e52  atchedCheckPlanR
-0001b630: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
-0001b640: 6174 6368 6564 4368 6563 6b65 7252 6573  atchedCheckerRes
-0001b650: 756c 7452 6571 7565 7374 5d28 646f 6373  ultRequest](docs
-0001b660: 2f50 6174 6368 6564 4368 6563 6b65 7252  /PatchedCheckerR
-0001b670: 6573 756c 7452 6571 7565 7374 2e6d 6429  esultRequest.md)
-0001b680: 0a20 2d20 5b50 6174 6368 6564 436c 6173  . - [PatchedClas
-0001b690: 7369 6669 6361 7469 6f6e 5265 7175 6573  sificationReques
-0001b6a0: 745d 2864 6f63 732f 5061 7463 6865 6443  t](docs/PatchedC
-0001b6b0: 6c61 7373 6966 6963 6174 696f 6e52 6571  lassificationReq
-0001b6c0: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001b6d0: 6368 6564 436c 6f75 6452 6571 7565 7374  chedCloudRequest
-0001b6e0: 5d28 646f 6373 2f50 6174 6368 6564 436c  ](docs/PatchedCl
-0001b6f0: 6f75 6452 6571 7565 7374 2e6d 6429 0a20  oudRequest.md). 
-0001b700: 2d20 5b50 6174 6368 6564 436f 6d6d 656e  - [PatchedCommen
-0001b710: 7452 6571 7565 7374 5d28 646f 6373 2f50  tRequest](docs/P
-0001b720: 6174 6368 6564 436f 6d6d 656e 7452 6571  atchedCommentReq
-0001b730: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001b740: 6368 6564 446f 6375 6d65 6e74 5265 7175  chedDocumentRequ
-0001b750: 6573 745d 2864 6f63 732f 5061 7463 6865  est](docs/Patche
-0001b760: 6444 6f63 756d 656e 7452 6571 7565 7374  dDocumentRequest
-0001b770: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001b780: 456c 656d 656e 7452 6571 7565 7374 5d28  ElementRequest](
-0001b790: 646f 6373 2f50 6174 6368 6564 456c 656d  docs/PatchedElem
-0001b7a0: 656e 7452 6571 7565 7374 2e6d 6429 0a20  entRequest.md). 
-0001b7b0: 2d20 5b50 6174 6368 6564 466f 6c64 6572  - [PatchedFolder
-0001b7c0: 5769 7468 6f75 7443 6869 6c64 7265 6e52  WithoutChildrenR
-0001b7d0: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
-0001b7e0: 6368 6564 466f 6c64 6572 5769 7468 6f75  chedFolderWithou
-0001b7f0: 7443 6869 6c64 7265 6e52 6571 7565 7374  tChildrenRequest
-0001b800: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001b810: 4675 6c6c 546f 7069 6352 6571 7565 7374  FullTopicRequest
-0001b820: 5d28 646f 6373 2f50 6174 6368 6564 4675  ](docs/PatchedFu
-0001b830: 6c6c 546f 7069 6352 6571 7565 7374 2e6d  llTopicRequest.m
-0001b840: 6429 0a20 2d20 5b50 6174 6368 6564 4772  d). - [PatchedGr
-0001b850: 6f75 7046 6f6c 6465 7252 6571 7565 7374  oupFolderRequest
-0001b860: 5d28 646f 6373 2f50 6174 6368 6564 4772  ](docs/PatchedGr
-0001b870: 6f75 7046 6f6c 6465 7252 6571 7565 7374  oupFolderRequest
-0001b880: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001b890: 4772 6f75 7052 6571 7565 7374 5d28 646f  GroupRequest](do
-0001b8a0: 6373 2f50 6174 6368 6564 4772 6f75 7052  cs/PatchedGroupR
-0001b8b0: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
-0001b8c0: 6174 6368 6564 4966 6341 6363 6573 7354  atchedIfcAccessT
-0001b8d0: 6f6b 656e 5265 7175 6573 745d 2864 6f63  okenRequest](doc
-0001b8e0: 732f 5061 7463 6865 6449 6663 4163 6365  s/PatchedIfcAcce
-0001b8f0: 7373 546f 6b65 6e52 6571 7565 7374 2e6d  ssTokenRequest.m
-0001b900: 6429 0a20 2d20 5b50 6174 6368 6564 4966  d). - [PatchedIf
-0001b910: 6343 6865 636b 6572 5265 7175 6573 745d  cCheckerRequest]
-0001b920: 2864 6f63 732f 5061 7463 6865 6449 6663  (docs/PatchedIfc
-0001b930: 4368 6563 6b65 7252 6571 7565 7374 2e6d  CheckerRequest.m
-0001b940: 6429 0a20 2d20 5b50 6174 6368 6564 4c61  d). - [PatchedLa
-0001b950: 6265 6c52 6571 7565 7374 5d28 646f 6373  belRequest](docs
-0001b960: 2f50 6174 6368 6564 4c61 6265 6c52 6571  /PatchedLabelReq
-0001b970: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001b980: 6368 6564 4c61 7965 7252 6571 7565 7374  chedLayerRequest
-0001b990: 5d28 646f 6373 2f50 6174 6368 6564 4c61  ](docs/PatchedLa
-0001b9a0: 7965 7252 6571 7565 7374 2e6d 6429 0a20  yerRequest.md). 
-0001b9b0: 2d20 5b50 6174 6368 6564 4d6f 6465 6c52  - [PatchedModelR
-0001b9c0: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
-0001b9d0: 6368 6564 4d6f 6465 6c52 6571 7565 7374  chedModelRequest
-0001b9e0: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001b9f0: 506f 7369 7469 6f6e 696e 6750 6c61 6e52  PositioningPlanR
-0001ba00: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
-0001ba10: 6368 6564 506f 7369 7469 6f6e 696e 6750  chedPositioningP
-0001ba20: 6c61 6e52 6571 7565 7374 2e6d 6429 0a20  lanRequest.md). 
-0001ba30: 2d20 5b50 6174 6368 6564 5072 696f 7269  - [PatchedPriori
-0001ba40: 7479 5265 7175 6573 745d 2864 6f63 732f  tyRequest](docs/
-0001ba50: 5061 7463 6865 6450 7269 6f72 6974 7952  PatchedPriorityR
-0001ba60: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
-0001ba70: 6174 6368 6564 5072 6f63 6573 736f 7248  atchedProcessorH
-0001ba80: 616e 646c 6572 5265 7175 6573 745d 2864  andlerRequest](d
-0001ba90: 6f63 732f 5061 7463 6865 6450 726f 6365  ocs/PatchedProce
-0001baa0: 7373 6f72 4861 6e64 6c65 7252 6571 7565  ssorHandlerReque
-0001bab0: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001bac0: 6564 5072 6f6a 6563 7441 6363 6573 7354  edProjectAccessT
-0001bad0: 6f6b 656e 5265 7175 6573 745d 2864 6f63  okenRequest](doc
-0001bae0: 732f 5061 7463 6865 6450 726f 6a65 6374  s/PatchedProject
-0001baf0: 4163 6365 7373 546f 6b65 6e52 6571 7565  AccessTokenReque
-0001bb00: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001bb10: 6564 5072 6f6a 6563 7452 6571 7565 7374  edProjectRequest
-0001bb20: 5d28 646f 6373 2f50 6174 6368 6564 5072  ](docs/PatchedPr
-0001bb30: 6f6a 6563 7452 6571 7565 7374 2e6d 6429  ojectRequest.md)
-0001bb40: 0a20 2d20 5b50 6174 6368 6564 5072 6f70  . - [PatchedProp
-0001bb50: 6572 7479 4465 6669 6e69 7469 6f6e 5265  ertyDefinitionRe
-0001bb60: 7175 6573 745d 2864 6f63 732f 5061 7463  quest](docs/Patc
-0001bb70: 6865 6450 726f 7065 7274 7944 6566 696e  hedPropertyDefin
-0001bb80: 6974 696f 6e52 6571 7565 7374 2e6d 6429  itionRequest.md)
-0001bb90: 0a20 2d20 5b50 6174 6368 6564 5072 6f70  . - [PatchedProp
-0001bba0: 6572 7479 5265 7175 6573 745d 2864 6f63  ertyRequest](doc
-0001bbb0: 732f 5061 7463 6865 6450 726f 7065 7274  s/PatchedPropert
-0001bbc0: 7952 6571 7565 7374 2e6d 6429 0a20 2d20  yRequest.md). - 
-0001bbd0: 5b50 6174 6368 6564 5072 6f70 6572 7479  [PatchedProperty
-0001bbe0: 5365 7452 6571 7565 7374 5d28 646f 6373  SetRequest](docs
-0001bbf0: 2f50 6174 6368 6564 5072 6f70 6572 7479  /PatchedProperty
-0001bc00: 5365 7452 6571 7565 7374 2e6d 6429 0a20  SetRequest.md). 
-0001bc10: 2d20 5b50 6174 6368 6564 5275 6c65 436f  - [PatchedRuleCo
-0001bc20: 6d70 6f6e 656e 7452 6571 7565 7374 5d28  mponentRequest](
-0001bc30: 646f 6373 2f50 6174 6368 6564 5275 6c65  docs/PatchedRule
-0001bc40: 436f 6d70 6f6e 656e 7452 6571 7565 7374  ComponentRequest
-0001bc50: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001bc60: 5275 6c65 5265 7175 6573 745d 2864 6f63  RuleRequest](doc
-0001bc70: 732f 5061 7463 6865 6452 756c 6552 6571  s/PatchedRuleReq
-0001bc80: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001bc90: 6368 6564 5275 6c65 7365 7452 6571 7565  chedRulesetReque
-0001bca0: 7374 5d28 646f 6373 2f50 6174 6368 6564  st](docs/Patched
-0001bcb0: 5275 6c65 7365 7452 6571 7565 7374 2e6d  RulesetRequest.m
-0001bcc0: 6429 0a20 2d20 5b50 6174 6368 6564 5370  d). - [PatchedSp
-0001bcd0: 6163 6552 6571 7565 7374 5d28 646f 6373  aceRequest](docs
-0001bce0: 2f50 6174 6368 6564 5370 6163 6552 6571  /PatchedSpaceReq
-0001bcf0: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001bd00: 6368 6564 5374 6167 6552 6571 7565 7374  chedStageRequest
-0001bd10: 5d28 646f 6373 2f50 6174 6368 6564 5374  ](docs/PatchedSt
-0001bd20: 6167 6552 6571 7565 7374 2e6d 6429 0a20  ageRequest.md). 
-0001bd30: 2d20 5b50 6174 6368 6564 5374 6f72 6579  - [PatchedStorey
-0001bd40: 4275 696c 6469 6e67 5265 7175 6573 745d  BuildingRequest]
-0001bd50: 2864 6f63 732f 5061 7463 6865 6453 746f  (docs/PatchedSto
-0001bd60: 7265 7942 7569 6c64 696e 6752 6571 7565  reyBuildingReque
-0001bd70: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001bd80: 6564 5379 7374 656d 5265 7175 6573 745d  edSystemRequest]
-0001bd90: 2864 6f63 732f 5061 7463 6865 6453 7973  (docs/PatchedSys
-0001bda0: 7465 6d52 6571 7565 7374 2e6d 6429 0a20  temRequest.md). 
-0001bdb0: 2d20 5b50 6174 6368 6564 5461 6752 6571  - [PatchedTagReq
-0001bdc0: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
-0001bdd0: 6564 5461 6752 6571 7565 7374 2e6d 6429  edTagRequest.md)
-0001bde0: 0a20 2d20 5b50 6174 6368 6564 546f 7069  . - [PatchedTopi
-0001bdf0: 6352 6571 7565 7374 5d28 646f 6373 2f50  cRequest](docs/P
-0001be00: 6174 6368 6564 546f 7069 6352 6571 7565  atchedTopicReque
-0001be10: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001be20: 6564 546f 7069 6353 7461 7475 7352 6571  edTopicStatusReq
-0001be30: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
-0001be40: 6564 546f 7069 6353 7461 7475 7352 6571  edTopicStatusReq
-0001be50: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001be60: 6368 6564 546f 7069 6354 7970 6552 6571  chedTopicTypeReq
-0001be70: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
-0001be80: 6564 546f 7069 6354 7970 6552 6571 7565  edTopicTypeReque
-0001be90: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001bea0: 6564 556e 6974 5265 7175 6573 745d 2864  edUnitRequest](d
-0001beb0: 6f63 732f 5061 7463 6865 6455 6e69 7452  ocs/PatchedUnitR
-0001bec0: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
-0001bed0: 6174 6368 6564 5573 6572 436c 6f75 6455  atchedUserCloudU
-0001bee0: 7064 6174 6552 6571 7565 7374 5d28 646f  pdateRequest](do
-0001bef0: 6373 2f50 6174 6368 6564 5573 6572 436c  cs/PatchedUserCl
-0001bf00: 6f75 6455 7064 6174 6552 6571 7565 7374  oudUpdateRequest
-0001bf10: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
-0001bf20: 5573 6572 5072 6f6a 6563 7455 7064 6174  UserProjectUpdat
-0001bf30: 6552 6571 7565 7374 5d28 646f 6373 2f50  eRequest](docs/P
-0001bf40: 6174 6368 6564 5573 6572 5072 6f6a 6563  atchedUserProjec
-0001bf50: 7455 7064 6174 6552 6571 7565 7374 2e6d  tUpdateRequest.m
-0001bf60: 6429 0a20 2d20 5b50 6174 6368 6564 5669  d). - [PatchedVi
-0001bf70: 6577 706f 696e 7452 6571 7565 7374 5d28  ewpointRequest](
-0001bf80: 646f 6373 2f50 6174 6368 6564 5669 6577  docs/PatchedView
-0001bf90: 706f 696e 7452 6571 7565 7374 2e6d 6429  pointRequest.md)
-0001bfa0: 0a20 2d20 5b50 6174 6368 6564 5669 7361  . - [PatchedVisa
-0001bfb0: 436f 6d6d 656e 7452 6571 7565 7374 5d28  CommentRequest](
-0001bfc0: 646f 6373 2f50 6174 6368 6564 5669 7361  docs/PatchedVisa
-0001bfd0: 436f 6d6d 656e 7452 6571 7565 7374 2e6d  CommentRequest.m
-0001bfe0: 6429 0a20 2d20 5b50 6174 6368 6564 5669  d). - [PatchedVi
-0001bff0: 7361 5265 7175 6573 745d 2864 6f63 732f  saRequest](docs/
-0001c000: 5061 7463 6865 6456 6973 6152 6571 7565  PatchedVisaReque
-0001c010: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
-0001c020: 6564 5669 7361 5661 6c69 6461 7469 6f6e  edVisaValidation
-0001c030: 5265 7175 6573 745d 2864 6f63 732f 5061  Request](docs/Pa
-0001c040: 7463 6865 6456 6973 6156 616c 6964 6174  tchedVisaValidat
-0001c050: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
-0001c060: 2d20 5b50 6174 6368 6564 5765 6248 6f6f  - [PatchedWebHoo
-0001c070: 6b52 6571 7565 7374 5d28 646f 6373 2f50  kRequest](docs/P
-0001c080: 6174 6368 6564 5765 6248 6f6f 6b52 6571  atchedWebHookReq
-0001c090: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
-0001c0a0: 6368 6564 5a6f 6e65 5265 7175 6573 745d  chedZoneRequest]
-0001c0b0: 2864 6f63 732f 5061 7463 6865 645a 6f6e  (docs/PatchedZon
-0001c0c0: 6552 6571 7565 7374 2e6d 6429 0a20 2d20  eRequest.md). - 
-0001c0d0: 5b50 6174 6368 6564 5a6f 6e65 5370 6163  [PatchedZoneSpac
-0001c0e0: 6552 6571 7565 7374 5d28 646f 6373 2f50  eRequest](docs/P
-0001c0f0: 6174 6368 6564 5a6f 6e65 5370 6163 6552  atchedZoneSpaceR
-0001c100: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
-0001c110: 6572 7370 6563 7469 7665 4361 6d65 7261  erspectiveCamera
-0001c120: 5d28 646f 6373 2f50 6572 7370 6563 7469  ](docs/Perspecti
-0001c130: 7665 4361 6d65 7261 2e6d 6429 0a20 2d20  veCamera.md). - 
-0001c140: 5b50 6572 7370 6563 7469 7665 4361 6d65  [PerspectiveCame
-0001c150: 7261 5265 7175 6573 745d 2864 6f63 732f  raRequest](docs/
-0001c160: 5065 7273 7065 6374 6976 6543 616d 6572  PerspectiveCamer
-0001c170: 6152 6571 7565 7374 2e6d 6429 0a20 2d20  aRequest.md). - 
-0001c180: 5b50 696e 5d28 646f 6373 2f50 696e 2e6d  [Pin](docs/Pin.m
-0001c190: 6429 0a20 2d20 5b50 696e 5265 7175 6573  d). - [PinReques
-0001c1a0: 745d 2864 6f63 732f 5069 6e52 6571 7565  t](docs/PinReque
-0001c1b0: 7374 2e6d 6429 0a20 2d20 5b50 6f69 6e74  st.md). - [Point
-0001c1c0: 5d28 646f 6373 2f50 6f69 6e74 2e6d 6429  ](docs/Point.md)
-0001c1d0: 0a20 2d20 5b50 6f69 6e74 5265 7175 6573  . - [PointReques
-0001c1e0: 745d 2864 6f63 732f 506f 696e 7452 6571  t](docs/PointReq
-0001c1f0: 7565 7374 2e6d 6429 0a20 2d20 5b50 6f73  uest.md). - [Pos
-0001c200: 6974 696f 6e69 6e67 506c 616e 5d28 646f  itioningPlan](do
-0001c210: 6373 2f50 6f73 6974 696f 6e69 6e67 506c  cs/PositioningPl
-0001c220: 616e 2e6d 6429 0a20 2d20 5b50 7269 6f72  an.md). - [Prior
-0001c230: 6974 795d 2864 6f63 732f 5072 696f 7269  ity](docs/Priori
-0001c240: 7479 2e6d 6429 0a20 2d20 5b50 7269 6f72  ty.md). - [Prior
-0001c250: 6974 7952 6571 7565 7374 5d28 646f 6373  ityRequest](docs
-0001c260: 2f50 7269 6f72 6974 7952 6571 7565 7374  /PriorityRequest
-0001c270: 2e6d 6429 0a20 2d20 5b50 726f 6365 7373  .md). - [Process
-0001c280: 6f72 4861 6e64 6c65 725d 2864 6f63 732f  orHandler](docs/
-0001c290: 5072 6f63 6573 736f 7248 616e 646c 6572  ProcessorHandler
-0001c2a0: 2e6d 6429 0a20 2d20 5b50 726f 6a65 6374  .md). - [Project
-0001c2b0: 5d28 646f 6373 2f50 726f 6a65 6374 2e6d  ](docs/Project.m
-0001c2c0: 6429 0a20 2d20 5b50 726f 6a65 6374 4163  d). - [ProjectAc
-0001c2d0: 6365 7373 546f 6b65 6e5d 2864 6f63 732f  cessToken](docs/
-0001c2e0: 5072 6f6a 6563 7441 6363 6573 7354 6f6b  ProjectAccessTok
-0001c2f0: 656e 2e6d 6429 0a20 2d20 5b50 726f 6a65  en.md). - [Proje
-0001c300: 6374 4163 6365 7373 546f 6b65 6e52 6571  ctAccessTokenReq
-0001c310: 7565 7374 5d28 646f 6373 2f50 726f 6a65  uest](docs/Proje
-0001c320: 6374 4163 6365 7373 546f 6b65 6e52 6571  ctAccessTokenReq
-0001c330: 7565 7374 2e6d 6429 0a20 2d20 5b50 726f  uest.md). - [Pro
-0001c340: 6a65 6374 466f 6c64 6572 5472 6565 5d28  jectFolderTree](
-0001c350: 646f 6373 2f50 726f 6a65 6374 466f 6c64  docs/ProjectFold
-0001c360: 6572 5472 6565 2e6d 6429 0a20 2d20 5b50  erTree.md). - [P
-0001c370: 726f 6a65 6374 496e 7669 7461 7469 6f6e  rojectInvitation
-0001c380: 5d28 646f 6373 2f50 726f 6a65 6374 496e  ](docs/ProjectIn
-0001c390: 7669 7461 7469 6f6e 2e6d 6429 0a20 2d20  vitation.md). - 
-0001c3a0: 5b50 726f 6a65 6374 496e 7669 7461 7469  [ProjectInvitati
-0001c3b0: 6f6e 5265 7175 6573 745d 2864 6f63 732f  onRequest](docs/
-0001c3c0: 5072 6f6a 6563 7449 6e76 6974 6174 696f  ProjectInvitatio
-0001c3d0: 6e52 6571 7565 7374 2e6d 6429 0a20 2d20  nRequest.md). - 
-0001c3e0: 5b50 726f 6a65 6374 5265 7175 6573 745d  [ProjectRequest]
-0001c3f0: 2864 6f63 732f 5072 6f6a 6563 7452 6571  (docs/ProjectReq
-0001c400: 7565 7374 2e6d 6429 0a20 2d20 5b50 726f  uest.md). - [Pro
-0001c410: 6a65 6374 526f 6c65 5d28 646f 6373 2f50  jectRole](docs/P
-0001c420: 726f 6a65 6374 526f 6c65 2e6d 6429 0a20  rojectRole.md). 
-0001c430: 2d20 5b50 726f 6a65 6374 5369 7a65 5d28  - [ProjectSize](
-0001c440: 646f 6373 2f50 726f 6a65 6374 5369 7a65  docs/ProjectSize
-0001c450: 2e6d 6429 0a20 2d20 5b50 726f 6a65 6374  .md). - [Project
-0001c460: 5769 7468 4368 696c 6472 656e 5d28 646f  WithChildren](do
-0001c470: 6373 2f50 726f 6a65 6374 5769 7468 4368  cs/ProjectWithCh
-0001c480: 696c 6472 656e 2e6d 6429 0a20 2d20 5b50  ildren.md). - [P
-0001c490: 726f 7065 7274 7944 6566 696e 6974 696f  ropertyDefinitio
-0001c4a0: 6e5d 2864 6f63 732f 5072 6f70 6572 7479  n](docs/Property
-0001c4b0: 4465 6669 6e69 7469 6f6e 2e6d 6429 0a20  Definition.md). 
-0001c4c0: 2d20 5b50 726f 7065 7274 7944 6566 696e  - [PropertyDefin
-0001c4d0: 6974 696f 6e52 6571 7565 7374 5d28 646f  itionRequest](do
-0001c4e0: 6373 2f50 726f 7065 7274 7944 6566 696e  cs/PropertyDefin
-0001c4f0: 6974 696f 6e52 6571 7565 7374 2e6d 6429  itionRequest.md)
-0001c500: 0a20 2d20 5b50 726f 7065 7274 7952 6571  . - [PropertyReq
-0001c510: 7565 7374 5d28 646f 6373 2f50 726f 7065  uest](docs/Prope
-0001c520: 7274 7952 6571 7565 7374 2e6d 6429 0a20  rtyRequest.md). 
-0001c530: 2d20 5b50 726f 7065 7274 7953 6574 5d28  - [PropertySet](
-0001c540: 646f 6373 2f50 726f 7065 7274 7953 6574  docs/PropertySet
-0001c550: 2e6d 6429 0a20 2d20 5b50 726f 7065 7274  .md). - [Propert
-0001c560: 7953 6574 5265 7175 6573 745d 2864 6f63  ySetRequest](doc
-0001c570: 732f 5072 6f70 6572 7479 5365 7452 6571  s/PropertySetReq
-0001c580: 7565 7374 2e6d 6429 0a20 2d20 5b50 7562  uest.md). - [Pub
-0001c590: 6c69 634f 7267 616e 697a 6174 696f 6e5d  licOrganization]
-0001c5a0: 2864 6f63 732f 5075 626c 6963 4f72 6761  (docs/PublicOrga
-0001c5b0: 6e69 7a61 7469 6f6e 2e6d 6429 0a20 2d20  nization.md). - 
-0001c5c0: 5b50 7562 6c69 634f 7267 616e 697a 6174  [PublicOrganizat
-0001c5d0: 696f 6e52 6571 7565 7374 5d28 646f 6373  ionRequest](docs
-0001c5e0: 2f50 7562 6c69 634f 7267 616e 697a 6174  /PublicOrganizat
-0001c5f0: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
-0001c600: 2d20 5b52 6177 436c 6173 7369 6669 6361  - [RawClassifica
-0001c610: 7469 6f6e 5d28 646f 6373 2f52 6177 436c  tion](docs/RawCl
-0001c620: 6173 7369 6669 6361 7469 6f6e 2e6d 6429  assification.md)
-0001c630: 0a20 2d20 5b52 6177 436c 6173 7369 6669  . - [RawClassifi
-0001c640: 6361 7469 6f6e 5265 7175 6573 745d 2864  cationRequest](d
-0001c650: 6f63 732f 5261 7743 6c61 7373 6966 6963  ocs/RawClassific
-0001c660: 6174 696f 6e52 6571 7565 7374 2e6d 6429  ationRequest.md)
-0001c670: 0a20 2d20 5b52 6177 4465 6669 6e69 7469  . - [RawDefiniti
-0001c680: 6f6e 5d28 646f 6373 2f52 6177 4465 6669  on](docs/RawDefi
-0001c690: 6e69 7469 6f6e 2e6d 6429 0a20 2d20 5b52  nition.md). - [R
-0001c6a0: 6177 4465 6669 6e69 7469 6f6e 5265 7175  awDefinitionRequ
-0001c6b0: 6573 745d 2864 6f63 732f 5261 7744 6566  est](docs/RawDef
-0001c6c0: 696e 6974 696f 6e52 6571 7565 7374 2e6d  initionRequest.m
-0001c6d0: 6429 0a20 2d20 5b52 6177 456c 656d 656e  d). - [RawElemen
-0001c6e0: 745d 2864 6f63 732f 5261 7745 6c65 6d65  t](docs/RawEleme
-0001c6f0: 6e74 2e6d 6429 0a20 2d20 5b52 6177 456c  nt.md). - [RawEl
-0001c700: 656d 656e 7452 6571 7565 7374 5d28 646f  ementRequest](do
-0001c710: 6373 2f52 6177 456c 656d 656e 7452 6571  cs/RawElementReq
-0001c720: 7565 7374 2e6d 6429 0a20 2d20 5b52 6177  uest.md). - [Raw
-0001c730: 456c 656d 656e 7473 5d28 646f 6373 2f52  Elements](docs/R
-0001c740: 6177 456c 656d 656e 7473 2e6d 6429 0a20  awElements.md). 
-0001c750: 2d20 5b52 6177 456c 656d 656e 7473 5265  - [RawElementsRe
-0001c760: 7175 6573 745d 2864 6f63 732f 5261 7745  quest](docs/RawE
-0001c770: 6c65 6d65 6e74 7352 6571 7565 7374 2e6d  lementsRequest.m
-0001c780: 6429 0a20 2d20 5b52 6177 4c61 7965 725d  d). - [RawLayer]
-0001c790: 2864 6f63 732f 5261 774c 6179 6572 2e6d  (docs/RawLayer.m
-0001c7a0: 6429 0a20 2d20 5b52 6177 4c61 7965 7252  d). - [RawLayerR
-0001c7b0: 6571 7565 7374 5d28 646f 6373 2f52 6177  equest](docs/Raw
-0001c7c0: 4c61 7965 7252 6571 7565 7374 2e6d 6429  LayerRequest.md)
-0001c7d0: 0a20 2d20 5b52 6177 4d61 7465 7269 616c  . - [RawMaterial
-0001c7e0: 5d28 646f 6373 2f52 6177 4d61 7465 7269  ](docs/RawMateri
-0001c7f0: 616c 2e6d 6429 0a20 2d20 5b52 6177 4d61  al.md). - [RawMa
-0001c800: 7465 7269 616c 4c69 7374 5d28 646f 6373  terialList](docs
-0001c810: 2f52 6177 4d61 7465 7269 616c 4c69 7374  /RawMaterialList
-0001c820: 2e6d 6429 0a20 2d20 5b52 6177 4d61 7465  .md). - [RawMate
-0001c830: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
-0001c840: 7473 5d28 646f 6373 2f52 6177 4d61 7465  ts](docs/RawMate
-0001c850: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
-0001c860: 7473 2e6d 6429 0a20 2d20 5b52 6177 4d61  ts.md). - [RawMa
-0001c870: 7465 7269 616c 4c69 7374 436f 6d70 6f6e  terialListCompon
-0001c880: 656e 7473 5265 7175 6573 745d 2864 6f63  entsRequest](doc
-0001c890: 732f 5261 774d 6174 6572 6961 6c4c 6973  s/RawMaterialLis
-0001c8a0: 7443 6f6d 706f 6e65 6e74 7352 6571 7565  tComponentsReque
-0001c8b0: 7374 2e6d 6429 0a20 2d20 5b52 6177 4d61  st.md). - [RawMa
-0001c8c0: 7465 7269 616c 4c69 7374 5265 7175 6573  terialListReques
-0001c8d0: 745d 2864 6f63 732f 5261 774d 6174 6572  t](docs/RawMater
-0001c8e0: 6961 6c4c 6973 7452 6571 7565 7374 2e6d  ialListRequest.m
-0001c8f0: 6429 0a20 2d20 5b52 6177 4d61 7465 7269  d). - [RawMateri
-0001c900: 616c 4f70 7469 6f6e 735d 2864 6f63 732f  alOptions](docs/
-0001c910: 5261 774d 6174 6572 6961 6c4f 7074 696f  RawMaterialOptio
-0001c920: 6e73 2e6d 6429 0a20 2d20 5b52 6177 4d61  ns.md). - [RawMa
-0001c930: 7465 7269 616c 4f70 7469 6f6e 7352 6571  terialOptionsReq
-0001c940: 7565 7374 5d28 646f 6373 2f52 6177 4d61  uest](docs/RawMa
-0001c950: 7465 7269 616c 4f70 7469 6f6e 7352 6571  terialOptionsReq
-0001c960: 7565 7374 2e6d 6429 0a20 2d20 5b52 6177  uest.md). - [Raw
-0001c970: 4d61 7465 7269 616c 5265 7175 6573 745d  MaterialRequest]
-0001c980: 2864 6f63 732f 5261 774d 6174 6572 6961  (docs/RawMateria
-0001c990: 6c52 6571 7565 7374 2e6d 6429 0a20 2d20  lRequest.md). - 
-0001c9a0: 5b52 6177 5072 6f70 6572 7479 5d28 646f  [RawProperty](do
-0001c9b0: 6373 2f52 6177 5072 6f70 6572 7479 2e6d  cs/RawProperty.m
-0001c9c0: 6429 0a20 2d20 5b52 6177 5072 6f70 6572  d). - [RawProper
-0001c9d0: 7479 5265 7175 6573 745d 2864 6f63 732f  tyRequest](docs/
-0001c9e0: 5261 7750 726f 7065 7274 7952 6571 7565  RawPropertyReque
-0001c9f0: 7374 2e6d 6429 0a20 2d20 5b52 6177 5072  st.md). - [RawPr
-0001ca00: 6f70 6572 7479 5365 745d 2864 6f63 732f  opertySet](docs/
-0001ca10: 5261 7750 726f 7065 7274 7953 6574 2e6d  RawPropertySet.m
-0001ca20: 6429 0a20 2d20 5b52 6177 5072 6f70 6572  d). - [RawProper
-0001ca30: 7479 5365 7452 6571 7565 7374 5d28 646f  tySetRequest](do
-0001ca40: 6373 2f52 6177 5072 6f70 6572 7479 5365  cs/RawPropertySe
-0001ca50: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
-0001ca60: 5b52 6177 5379 7374 656d 5d28 646f 6373  [RawSystem](docs
-0001ca70: 2f52 6177 5379 7374 656d 2e6d 6429 0a20  /RawSystem.md). 
-0001ca80: 2d20 5b52 6177 5379 7374 656d 5265 7175  - [RawSystemRequ
-0001ca90: 6573 745d 2864 6f63 732f 5261 7753 7973  est](docs/RawSys
-0001caa0: 7465 6d52 6571 7565 7374 2e6d 6429 0a20  temRequest.md). 
-0001cab0: 2d20 5b52 6177 556e 6974 5d28 646f 6373  - [RawUnit](docs
-0001cac0: 2f52 6177 556e 6974 2e6d 6429 0a20 2d20  /RawUnit.md). - 
-0001cad0: 5b52 6177 556e 6974 5265 7175 6573 745d  [RawUnitRequest]
-0001cae0: 2864 6f63 732f 5261 7755 6e69 7452 6571  (docs/RawUnitReq
-0001caf0: 7565 7374 2e6d 6429 0a20 2d20 5b52 6563  uest.md). - [Rec
-0001cb00: 7572 7369 7665 466f 6c64 6572 4368 696c  ursiveFolderChil
-0001cb10: 6472 656e 5d28 646f 6373 2f52 6563 7572  dren](docs/Recur
-0001cb20: 7369 7665 466f 6c64 6572 4368 696c 6472  siveFolderChildr
-0001cb30: 656e 2e6d 6429 0a20 2d20 5b52 756c 655d  en.md). - [Rule]
-0001cb40: 2864 6f63 732f 5275 6c65 2e6d 6429 0a20  (docs/Rule.md). 
-0001cb50: 2d20 5b52 756c 6543 6f6d 706f 6e65 6e74  - [RuleComponent
-0001cb60: 5d28 646f 6373 2f52 756c 6543 6f6d 706f  ](docs/RuleCompo
-0001cb70: 6e65 6e74 2e6d 6429 0a20 2d20 5b52 756c  nent.md). - [Rul
-0001cb80: 6543 6f6d 706f 6e65 6e74 5265 7175 6573  eComponentReques
-0001cb90: 745d 2864 6f63 732f 5275 6c65 436f 6d70  t](docs/RuleComp
-0001cba0: 6f6e 656e 7452 6571 7565 7374 2e6d 6429  onentRequest.md)
-0001cbb0: 0a20 2d20 5b52 756c 6552 6571 7565 7374  . - [RuleRequest
-0001cbc0: 5d28 646f 6373 2f52 756c 6552 6571 7565  ](docs/RuleReque
-0001cbd0: 7374 2e6d 6429 0a20 2d20 5b52 756c 6573  st.md). - [Rules
-0001cbe0: 6574 5d28 646f 6373 2f52 756c 6573 6574  et](docs/Ruleset
-0001cbf0: 2e6d 6429 0a20 2d20 5b52 756c 6573 6574  .md). - [Ruleset
-0001cc00: 5265 7175 6573 745d 2864 6f63 732f 5275  Request](docs/Ru
-0001cc10: 6c65 7365 7452 6571 7565 7374 2e6d 6429  lesetRequest.md)
-0001cc20: 0a20 2d20 5b53 656c 6642 6366 5573 6572  . - [SelfBcfUser
-0001cc30: 5d28 646f 6373 2f53 656c 6642 6366 5573  ](docs/SelfBcfUs
-0001cc40: 6572 2e6d 6429 0a20 2d20 5b53 656c 6655  er.md). - [SelfU
-0001cc50: 7365 725d 2864 6f63 732f 5365 6c66 5573  ser](docs/SelfUs
-0001cc60: 6572 2e6d 6429 0a20 2d20 5b53 696d 706c  er.md). - [Simpl
-0001cc70: 6545 6c65 6d65 6e74 5d28 646f 6373 2f53  eElement](docs/S
-0001cc80: 696d 706c 6545 6c65 6d65 6e74 2e6d 6429  impleElement.md)
-0001cc90: 0a20 2d20 5b53 697a 655d 2864 6f63 732f  . - [Size](docs/
-0001cca0: 5369 7a65 2e6d 6429 0a20 2d20 5b53 6e61  Size.md). - [Sna
-0001ccb0: 7073 686f 745d 2864 6f63 732f 536e 6170  pshot](docs/Snap
-0001ccc0: 7368 6f74 2e6d 6429 0a20 2d20 5b53 6e61  shot.md). - [Sna
-0001ccd0: 7073 686f 7452 6571 7565 7374 5d28 646f  pshotRequest](do
-0001cce0: 6373 2f53 6e61 7073 686f 7452 6571 7565  cs/SnapshotReque
-0001ccf0: 7374 2e6d 6429 0a20 2d20 5b53 7061 6365  st.md). - [Space
-0001cd00: 5d28 646f 6373 2f53 7061 6365 2e6d 6429  ](docs/Space.md)
-0001cd10: 0a20 2d20 5b53 7061 6365 5265 7175 6573  . - [SpaceReques
-0001cd20: 745d 2864 6f63 732f 5370 6163 6552 6571  t](docs/SpaceReq
-0001cd30: 7565 7374 2e6d 6429 0a20 2d20 5b53 7461  uest.md). - [Sta
-0001cd40: 6765 5d28 646f 6373 2f53 7461 6765 2e6d  ge](docs/Stage.m
-0001cd50: 6429 0a20 2d20 5b53 7461 6765 5265 7175  d). - [StageRequ
-0001cd60: 6573 745d 2864 6f63 732f 5374 6167 6552  est](docs/StageR
-0001cd70: 6571 7565 7374 2e6d 6429 0a20 2d20 5b53  equest.md). - [S
-0001cd80: 746f 7265 795d 2864 6f63 732f 5374 6f72  torey](docs/Stor
-0001cd90: 6579 2e6d 6429 0a20 2d20 5b53 746f 7265  ey.md). - [Store
-0001cda0: 7942 7569 6c64 696e 6752 6571 7565 7374  yBuildingRequest
-0001cdb0: 5d28 646f 6373 2f53 746f 7265 7942 7569  ](docs/StoreyBui
-0001cdc0: 6c64 696e 6752 6571 7565 7374 2e6d 6429  ldingRequest.md)
-0001cdd0: 0a20 2d20 5b53 746f 7265 794d 6f64 656c  . - [StoreyModel
-0001cde0: 506c 616e 5265 7175 6573 745d 2864 6f63  PlanRequest](doc
-0001cdf0: 732f 5374 6f72 6579 4d6f 6465 6c50 6c61  s/StoreyModelPla
-0001ce00: 6e52 6571 7565 7374 2e6d 6429 0a20 2d20  nRequest.md). - 
-0001ce10: 5b53 7973 7465 6d5d 2864 6f63 732f 5379  [System](docs/Sy
-0001ce20: 7374 656d 2e6d 6429 0a20 2d20 5b53 7973  stem.md). - [Sys
-0001ce30: 7465 6d52 6571 7565 7374 5d28 646f 6373  temRequest](docs
-0001ce40: 2f53 7973 7465 6d52 6571 7565 7374 2e6d  /SystemRequest.m
-0001ce50: 6429 0a20 2d20 5b54 6167 5d28 646f 6373  d). - [Tag](docs
-0001ce60: 2f54 6167 2e6d 6429 0a20 2d20 5b54 6167  /Tag.md). - [Tag
-0001ce70: 4964 5265 7175 6573 745d 2864 6f63 732f  IdRequest](docs/
-0001ce80: 5461 6749 6452 6571 7565 7374 2e6d 6429  TagIdRequest.md)
-0001ce90: 0a20 2d20 5b54 6167 5265 7175 6573 745d  . - [TagRequest]
-0001cea0: 2864 6f63 732f 5461 6752 6571 7565 7374  (docs/TagRequest
-0001ceb0: 2e6d 6429 0a20 2d20 5b54 6f70 6963 5d28  .md). - [Topic](
-0001cec0: 646f 6373 2f54 6f70 6963 2e6d 6429 0a20  docs/Topic.md). 
-0001ced0: 2d20 5b54 6f70 6963 5265 7175 6573 745d  - [TopicRequest]
-0001cee0: 2864 6f63 732f 546f 7069 6352 6571 7565  (docs/TopicReque
-0001cef0: 7374 2e6d 6429 0a20 2d20 5b54 6f70 6963  st.md). - [Topic
-0001cf00: 5374 6174 7573 5d28 646f 6373 2f54 6f70  Status](docs/Top
-0001cf10: 6963 5374 6174 7573 2e6d 6429 0a20 2d20  icStatus.md). - 
-0001cf20: 5b54 6f70 6963 5374 6174 7573 5265 7175  [TopicStatusRequ
-0001cf30: 6573 745d 2864 6f63 732f 546f 7069 6353  est](docs/TopicS
-0001cf40: 7461 7475 7352 6571 7565 7374 2e6d 6429  tatusRequest.md)
-0001cf50: 0a20 2d20 5b54 6f70 6963 5479 7065 5d28  . - [TopicType](
-0001cf60: 646f 6373 2f54 6f70 6963 5479 7065 2e6d  docs/TopicType.m
-0001cf70: 6429 0a20 2d20 5b54 6f70 6963 5479 7065  d). - [TopicType
-0001cf80: 5265 7175 6573 745d 2864 6f63 732f 546f  Request](docs/To
-0001cf90: 7069 6354 7970 6552 6571 7565 7374 2e6d  picTypeRequest.m
-0001cfa0: 6429 0a20 2d20 5b55 6e69 745d 2864 6f63  d). - [Unit](doc
-0001cfb0: 732f 556e 6974 2e6d 6429 0a20 2d20 5b55  s/Unit.md). - [U
-0001cfc0: 6e69 7452 6571 7565 7374 5d28 646f 6373  nitRequest](docs
-0001cfd0: 2f55 6e69 7452 6571 7565 7374 2e6d 6429  /UnitRequest.md)
-0001cfe0: 0a20 2d20 5b55 7365 725d 2864 6f63 732f  . - [User](docs/
-0001cff0: 5573 6572 2e6d 6429 0a20 2d20 5b55 7365  User.md). - [Use
-0001d000: 7249 6e76 6974 6174 696f 6e5d 2864 6f63  rInvitation](doc
-0001d010: 732f 5573 6572 496e 7669 7461 7469 6f6e  s/UserInvitation
-0001d020: 2e6d 6429 0a20 2d20 5b55 7365 7250 726f  .md). - [UserPro
-0001d030: 6a65 6374 5d28 646f 6373 2f55 7365 7250  ject](docs/UserP
-0001d040: 726f 6a65 6374 2e6d 6429 0a20 2d20 5b55  roject.md). - [U
-0001d050: 7365 7250 726f 6a65 6374 4964 5265 7175  serProjectIdRequ
-0001d060: 6573 745d 2864 6f63 732f 5573 6572 5072  est](docs/UserPr
-0001d070: 6f6a 6563 7449 6452 6571 7565 7374 2e6d  ojectIdRequest.m
-0001d080: 6429 0a20 2d20 5b56 6965 7753 6574 7570  d). - [ViewSetup
-0001d090: 4869 6e74 735d 2864 6f63 732f 5669 6577  Hints](docs/View
-0001d0a0: 5365 7475 7048 696e 7473 2e6d 6429 0a20  SetupHints.md). 
-0001d0b0: 2d20 5b56 6965 7753 6574 7570 4869 6e74  - [ViewSetupHint
-0001d0c0: 7352 6571 7565 7374 5d28 646f 6373 2f56  sRequest](docs/V
-0001d0d0: 6965 7753 6574 7570 4869 6e74 7352 6571  iewSetupHintsReq
-0001d0e0: 7565 7374 2e6d 6429 0a20 2d20 5b56 6965  uest.md). - [Vie
-0001d0f0: 7770 6f69 6e74 5d28 646f 6373 2f56 6965  wpoint](docs/Vie
-0001d100: 7770 6f69 6e74 2e6d 6429 0a20 2d20 5b56  wpoint.md). - [V
-0001d110: 6965 7770 6f69 6e74 5265 7175 6573 745d  iewpointRequest]
-0001d120: 2864 6f63 732f 5669 6577 706f 696e 7452  (docs/ViewpointR
-0001d130: 6571 7565 7374 2e6d 6429 0a20 2d20 5b56  equest.md). - [V
-0001d140: 6973 615d 2864 6f63 732f 5669 7361 2e6d  isa](docs/Visa.m
-0001d150: 6429 0a20 2d20 5b56 6973 6143 6f6d 6d65  d). - [VisaComme
-0001d160: 6e74 5d28 646f 6373 2f56 6973 6143 6f6d  nt](docs/VisaCom
-0001d170: 6d65 6e74 2e6d 6429 0a20 2d20 5b56 6973  ment.md). - [Vis
-0001d180: 6143 6f6d 6d65 6e74 5265 7175 6573 745d  aCommentRequest]
-0001d190: 2864 6f63 732f 5669 7361 436f 6d6d 656e  (docs/VisaCommen
-0001d1a0: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
-0001d1b0: 5b56 6973 6152 6571 7565 7374 5d28 646f  [VisaRequest](do
-0001d1c0: 6373 2f56 6973 6152 6571 7565 7374 2e6d  cs/VisaRequest.m
-0001d1d0: 6429 0a20 2d20 5b56 6973 6156 616c 6964  d). - [VisaValid
-0001d1e0: 6174 696f 6e5d 2864 6f63 732f 5669 7361  ation](docs/Visa
-0001d1f0: 5661 6c69 6461 7469 6f6e 2e6d 6429 0a20  Validation.md). 
-0001d200: 2d20 5b56 6973 6156 616c 6964 6174 696f  - [VisaValidatio
-0001d210: 6e52 6571 7565 7374 5d28 646f 6373 2f56  nRequest](docs/V
-0001d220: 6973 6156 616c 6964 6174 696f 6e52 6571  isaValidationReq
-0001d230: 7565 7374 2e6d 6429 0a20 2d20 5b56 6973  uest.md). - [Vis
-0001d240: 6962 696c 6974 795d 2864 6f63 732f 5669  ibility](docs/Vi
-0001d250: 7369 6269 6c69 7479 2e6d 6429 0a20 2d20  sibility.md). - 
-0001d260: 5b56 6973 6962 696c 6974 7952 6571 7565  [VisibilityReque
-0001d270: 7374 5d28 646f 6373 2f56 6973 6962 696c  st](docs/Visibil
-0001d280: 6974 7952 6571 7565 7374 2e6d 6429 0a20  ityRequest.md). 
-0001d290: 2d20 5b57 6562 486f 6f6b 5d28 646f 6373  - [WebHook](docs
-0001d2a0: 2f57 6562 486f 6f6b 2e6d 6429 0a20 2d20  /WebHook.md). - 
-0001d2b0: 5b57 6562 486f 6f6b 5265 7175 6573 745d  [WebHookRequest]
-0001d2c0: 2864 6f63 732f 5765 6248 6f6f 6b52 6571  (docs/WebHookReq
-0001d2d0: 7565 7374 2e6d 6429 0a20 2d20 5b57 7269  uest.md). - [Wri
-0001d2e0: 7465 466f 6c64 6572 5265 7175 6573 745d  teFolderRequest]
-0001d2f0: 2864 6f63 732f 5772 6974 6546 6f6c 6465  (docs/WriteFolde
-0001d300: 7252 6571 7565 7374 2e6d 6429 0a20 2d20  rRequest.md). - 
-0001d310: 5b5a 6f6e 655d 2864 6f63 732f 5a6f 6e65  [Zone](docs/Zone
-0001d320: 2e6d 6429 0a20 2d20 5b5a 6f6e 6552 6571  .md). - [ZoneReq
-0001d330: 7565 7374 5d28 646f 6373 2f5a 6f6e 6552  uest](docs/ZoneR
-0001d340: 6571 7565 7374 2e6d 6429 0a20 2d20 5b5a  equest.md). - [Z
-0001d350: 6f6e 6553 7061 6365 5d28 646f 6373 2f5a  oneSpace](docs/Z
-0001d360: 6f6e 6553 7061 6365 2e6d 6429 0a20 2d20  oneSpace.md). - 
-0001d370: 5b5a 6f6e 6553 7061 6365 5265 7175 6573  [ZoneSpaceReques
-0001d380: 745d 2864 6f63 732f 5a6f 6e65 5370 6163  t](docs/ZoneSpac
-0001d390: 6552 6571 7565 7374 2e6d 6429 0a0a 0a23  eRequest.md)...#
-0001d3a0: 2320 446f 6375 6d65 6e74 6174 696f 6e20  # Documentation 
-0001d3b0: 466f 7220 4175 7468 6f72 697a 6174 696f  For Authorizatio
-0001d3c0: 6e0a 0a0a 2323 2041 7069 4b65 790a 0a2d  n...## ApiKey..-
-0001d3d0: 202a 2a54 7970 652a 2a3a 2041 5049 206b   **Type**: API k
-0001d3e0: 6579 0a2d 202a 2a41 5049 206b 6579 2070  ey.- **API key p
-0001d3f0: 6172 616d 6574 6572 206e 616d 652a 2a3a  arameter name**:
-0001d400: 2041 7574 686f 7269 7a61 7469 6f6e 0a2d   Authorization.-
-0001d410: 202a 2a4c 6f63 6174 696f 6e2a 2a3a 2048   **Location**: H
-0001d420: 5454 5020 6865 6164 6572 0a0a 0a23 2320  TTP header...## 
-0001d430: 4249 4d44 6174 615f 436f 6e6e 6563 740a  BIMData_Connect.
-0001d440: 0a2d 202a 2a54 7970 652a 2a3a 204f 4175  .- **Type**: OAu
-0001d450: 7468 0a2d 202a 2a46 6c6f 772a 2a3a 2069  th.- **Flow**: i
-0001d460: 6d70 6c69 6369 740a 2d20 2a2a 4175 7468  mplicit.- **Auth
-0001d470: 6f72 697a 6174 696f 6e20 5552 4c2a 2a3a  orization URL**:
-0001d480: 2068 7474 703a 2f2f 6661 6b65 7572 6c2e   http://fakeurl.
-0001d490: 6269 6d64 6174 612e 696f 2f72 6561 6c6d  bimdata.io/realm
-0001d4a0: 732f 6269 6d64 6174 612f 7072 6f74 6f63  s/bimdata/protoc
-0001d4b0: 6f6c 2f6f 7065 6e69 642d 636f 6e6e 6563  ol/openid-connec
-0001d4c0: 742f 6175 7468 0a2d 202a 2a53 636f 7065  t/auth.- **Scope
-0001d4d0: 732a 2a3a 204e 2f41 0a0a 0a23 2320 4249  s**: N/A...## BI
-0001d4e0: 4d44 6174 615f 436f 6e6e 6563 740a 0a2d  MData_Connect..-
-0001d4f0: 202a 2a54 7970 652a 2a3a 204f 4175 7468   **Type**: OAuth
-0001d500: 0a2d 202a 2a46 6c6f 772a 2a3a 2061 7070  .- **Flow**: app
-0001d510: 6c69 6361 7469 6f6e 0a2d 202a 2a41 7574  lication.- **Aut
-0001d520: 686f 7269 7a61 7469 6f6e 2055 524c 2a2a  horization URL**
-0001d530: 3a20 0a2d 202a 2a53 636f 7065 732a 2a3a  : .- **Scopes**:
-0001d540: 204e 2f41 0a0a 0a23 2320 4265 6172 6572   N/A...## Bearer
-0001d550: 0a0a 2d20 2a2a 5479 7065 2a2a 3a20 4150  ..- **Type**: AP
-0001d560: 4920 6b65 790a 2d20 2a2a 4150 4920 6b65  I key.- **API ke
-0001d570: 7920 7061 7261 6d65 7465 7220 6e61 6d65  y parameter name
-0001d580: 2a2a 3a20 4175 7468 6f72 697a 6174 696f  **: Authorizatio
-0001d590: 6e0a 2d20 2a2a 4c6f 6361 7469 6f6e 2a2a  n.- **Location**
-0001d5a0: 3a20 4854 5450 2068 6561 6465 720a 0a0a  : HTTP header...
-0001d5b0: 2323 2041 7574 686f 720a 0a73 7570 706f  ## Author..suppo
-0001d5c0: 7274 4062 696d 6461 7461 2e69 6f0a 0a0a  rt@bimdata.io...
-0001d5d0: 2323 204e 6f74 6573 2066 6f72 204c 6172  ## Notes for Lar
-0001d5e0: 6765 204f 7065 6e41 5049 2064 6f63 756d  ge OpenAPI docum
-0001d5f0: 656e 7473 0a49 6620 7468 6520 4f70 656e  ents.If the Open
-0001d600: 4150 4920 646f 6375 6d65 6e74 2069 7320  API document is 
-0001d610: 6c61 7267 652c 2069 6d70 6f72 7473 2069  large, imports i
-0001d620: 6e20 6269 6d64 6174 615f 6170 695f 636c  n bimdata_api_cl
-0001d630: 6965 6e74 2e61 7069 7320 616e 6420 6269  ient.apis and bi
-0001d640: 6d64 6174 615f 6170 695f 636c 6965 6e74  mdata_api_client
-0001d650: 2e6d 6f64 656c 7320 6d61 7920 6661 696c  .models may fail
-0001d660: 2077 6974 6820 610a 5265 6375 7273 696f   with a.Recursio
-0001d670: 6e45 7272 6f72 2069 6e64 6963 6174 696e  nError indicatin
-0001d680: 6720 7468 6520 6d61 7869 6d75 6d20 7265  g the maximum re
-0001d690: 6375 7273 696f 6e20 6c69 6d69 7420 6861  cursion limit ha
-0001d6a0: 7320 6265 656e 2065 7863 6565 6465 642e  s been exceeded.
-0001d6b0: 2049 6e20 7468 6174 2063 6173 652c 2074   In that case, t
-0001d6c0: 6865 7265 2061 7265 2061 2063 6f75 706c  here are a coupl
-0001d6d0: 6520 6f66 2073 6f6c 7574 696f 6e73 3a0a  e of solutions:.
-0001d6e0: 0a53 6f6c 7574 696f 6e20 313a 0a55 7365  .Solution 1:.Use
-0001d6f0: 2073 7065 6369 6669 6320 696d 706f 7274   specific import
-0001d700: 7320 666f 7220 6170 6973 2061 6e64 206d  s for apis and m
-0001d710: 6f64 656c 7320 6c69 6b65 3a0a 2d20 6066  odels like:.- `f
-0001d720: 726f 6d20 6269 6d64 6174 615f 6170 695f  rom bimdata_api_
-0001d730: 636c 6965 6e74 2e61 7069 2e64 6566 6175  client.api.defau
-0001d740: 6c74 5f61 7069 2069 6d70 6f72 7420 4465  lt_api import De
-0001d750: 6661 756c 7441 7069 600a 2d20 6066 726f  faultApi`.- `fro
-0001d760: 6d20 6269 6d64 6174 615f 6170 695f 636c  m bimdata_api_cl
-0001d770: 6965 6e74 2e6d 6f64 656c 2e70 6574 2069  ient.model.pet i
-0001d780: 6d70 6f72 7420 5065 7460 0a0a 536f 6c75  mport Pet`..Solu
-0001d790: 7469 6f6e 2032 3a0a 4265 666f 7265 2069  tion 2:.Before i
-0001d7a0: 6d70 6f72 7469 6e67 2074 6865 2070 6163  mporting the pac
-0001d7b0: 6b61 6765 2c20 6164 6a75 7374 2074 6865  kage, adjust the
-0001d7c0: 206d 6178 696d 756d 2072 6563 7572 7369   maximum recursi
-0001d7d0: 6f6e 206c 696d 6974 2061 7320 7368 6f77  on limit as show
-0001d7e0: 6e20 6265 6c6f 773a 0a60 6060 0a69 6d70  n below:.```.imp
-0001d7f0: 6f72 7420 7379 730a 7379 732e 7365 7472  ort sys.sys.setr
-0001d800: 6563 7572 7369 6f6e 6c69 6d69 7428 3135  ecursionlimit(15
-0001d810: 3030 290a 696d 706f 7274 2062 696d 6461  00).import bimda
-0001d820: 7461 5f61 7069 5f63 6c69 656e 740a 6672  ta_api_client.fr
-0001d830: 6f6d 2062 696d 6461 7461 5f61 7069 5f63  om bimdata_api_c
-0001d840: 6c69 656e 742e 6170 6973 2069 6d70 6f72  lient.apis impor
-0001d850: 7420 2a0a 6672 6f6d 2062 696d 6461 7461  t *.from bimdata
-0001d860: 5f61 7069 5f63 6c69 656e 742e 6d6f 6465  _api_client.mode
-0001d870: 6c73 2069 6d70 6f72 7420 2a0a 6060 600a  ls import *.```.
-0001d880: 0a                                       .
+0001b560: 6572 6152 6571 7565 7374 5d28 646f 6373  eraRequest](docs
+0001b570: 2f4f 7274 686f 676f 6e61 6c43 616d 6572  /OrthogonalCamer
+0001b580: 6152 6571 7565 7374 2e6d 6429 0a20 2d20  aRequest.md). - 
+0001b590: 5b50 6174 6368 6564 4263 6650 726f 6a65  [PatchedBcfProje
+0001b5a0: 6374 5265 7175 6573 745d 2864 6f63 732f  ctRequest](docs/
+0001b5b0: 5061 7463 6865 6442 6366 5072 6f6a 6563  PatchedBcfProjec
+0001b5c0: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
+0001b5d0: 5b50 6174 6368 6564 4368 6563 6b50 6c61  [PatchedCheckPla
+0001b5e0: 6e52 6571 7565 7374 5d28 646f 6373 2f50  nRequest](docs/P
+0001b5f0: 6174 6368 6564 4368 6563 6b50 6c61 6e52  atchedCheckPlanR
+0001b600: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
+0001b610: 6174 6368 6564 4368 6563 6b65 7252 6573  atchedCheckerRes
+0001b620: 756c 7452 6571 7565 7374 5d28 646f 6373  ultRequest](docs
+0001b630: 2f50 6174 6368 6564 4368 6563 6b65 7252  /PatchedCheckerR
+0001b640: 6573 756c 7452 6571 7565 7374 2e6d 6429  esultRequest.md)
+0001b650: 0a20 2d20 5b50 6174 6368 6564 436c 6173  . - [PatchedClas
+0001b660: 7369 6669 6361 7469 6f6e 5265 7175 6573  sificationReques
+0001b670: 745d 2864 6f63 732f 5061 7463 6865 6443  t](docs/PatchedC
+0001b680: 6c61 7373 6966 6963 6174 696f 6e52 6571  lassificationReq
+0001b690: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001b6a0: 6368 6564 436c 6f75 6452 6571 7565 7374  chedCloudRequest
+0001b6b0: 5d28 646f 6373 2f50 6174 6368 6564 436c  ](docs/PatchedCl
+0001b6c0: 6f75 6452 6571 7565 7374 2e6d 6429 0a20  oudRequest.md). 
+0001b6d0: 2d20 5b50 6174 6368 6564 436f 6d6d 656e  - [PatchedCommen
+0001b6e0: 7452 6571 7565 7374 5d28 646f 6373 2f50  tRequest](docs/P
+0001b6f0: 6174 6368 6564 436f 6d6d 656e 7452 6571  atchedCommentReq
+0001b700: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001b710: 6368 6564 446f 6375 6d65 6e74 5265 7175  chedDocumentRequ
+0001b720: 6573 745d 2864 6f63 732f 5061 7463 6865  est](docs/Patche
+0001b730: 6444 6f63 756d 656e 7452 6571 7565 7374  dDocumentRequest
+0001b740: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001b750: 456c 656d 656e 7452 6571 7565 7374 5d28  ElementRequest](
+0001b760: 646f 6373 2f50 6174 6368 6564 456c 656d  docs/PatchedElem
+0001b770: 656e 7452 6571 7565 7374 2e6d 6429 0a20  entRequest.md). 
+0001b780: 2d20 5b50 6174 6368 6564 466f 6c64 6572  - [PatchedFolder
+0001b790: 5769 7468 6f75 7443 6869 6c64 7265 6e52  WithoutChildrenR
+0001b7a0: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
+0001b7b0: 6368 6564 466f 6c64 6572 5769 7468 6f75  chedFolderWithou
+0001b7c0: 7443 6869 6c64 7265 6e52 6571 7565 7374  tChildrenRequest
+0001b7d0: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001b7e0: 4675 6c6c 546f 7069 6352 6571 7565 7374  FullTopicRequest
+0001b7f0: 5d28 646f 6373 2f50 6174 6368 6564 4675  ](docs/PatchedFu
+0001b800: 6c6c 546f 7069 6352 6571 7565 7374 2e6d  llTopicRequest.m
+0001b810: 6429 0a20 2d20 5b50 6174 6368 6564 4772  d). - [PatchedGr
+0001b820: 6f75 7046 6f6c 6465 7252 6571 7565 7374  oupFolderRequest
+0001b830: 5d28 646f 6373 2f50 6174 6368 6564 4772  ](docs/PatchedGr
+0001b840: 6f75 7046 6f6c 6465 7252 6571 7565 7374  oupFolderRequest
+0001b850: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001b860: 4772 6f75 7052 6571 7565 7374 5d28 646f  GroupRequest](do
+0001b870: 6373 2f50 6174 6368 6564 4772 6f75 7052  cs/PatchedGroupR
+0001b880: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
+0001b890: 6174 6368 6564 4966 6341 6363 6573 7354  atchedIfcAccessT
+0001b8a0: 6f6b 656e 5265 7175 6573 745d 2864 6f63  okenRequest](doc
+0001b8b0: 732f 5061 7463 6865 6449 6663 4163 6365  s/PatchedIfcAcce
+0001b8c0: 7373 546f 6b65 6e52 6571 7565 7374 2e6d  ssTokenRequest.m
+0001b8d0: 6429 0a20 2d20 5b50 6174 6368 6564 4966  d). - [PatchedIf
+0001b8e0: 6343 6865 636b 6572 5265 7175 6573 745d  cCheckerRequest]
+0001b8f0: 2864 6f63 732f 5061 7463 6865 6449 6663  (docs/PatchedIfc
+0001b900: 4368 6563 6b65 7252 6571 7565 7374 2e6d  CheckerRequest.m
+0001b910: 6429 0a20 2d20 5b50 6174 6368 6564 4c61  d). - [PatchedLa
+0001b920: 6265 6c52 6571 7565 7374 5d28 646f 6373  belRequest](docs
+0001b930: 2f50 6174 6368 6564 4c61 6265 6c52 6571  /PatchedLabelReq
+0001b940: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001b950: 6368 6564 4c61 7965 7252 6571 7565 7374  chedLayerRequest
+0001b960: 5d28 646f 6373 2f50 6174 6368 6564 4c61  ](docs/PatchedLa
+0001b970: 7965 7252 6571 7565 7374 2e6d 6429 0a20  yerRequest.md). 
+0001b980: 2d20 5b50 6174 6368 6564 4d6f 6465 6c52  - [PatchedModelR
+0001b990: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
+0001b9a0: 6368 6564 4d6f 6465 6c52 6571 7565 7374  chedModelRequest
+0001b9b0: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001b9c0: 506f 7369 7469 6f6e 696e 6750 6c61 6e52  PositioningPlanR
+0001b9d0: 6571 7565 7374 5d28 646f 6373 2f50 6174  equest](docs/Pat
+0001b9e0: 6368 6564 506f 7369 7469 6f6e 696e 6750  chedPositioningP
+0001b9f0: 6c61 6e52 6571 7565 7374 2e6d 6429 0a20  lanRequest.md). 
+0001ba00: 2d20 5b50 6174 6368 6564 5072 696f 7269  - [PatchedPriori
+0001ba10: 7479 5265 7175 6573 745d 2864 6f63 732f  tyRequest](docs/
+0001ba20: 5061 7463 6865 6450 7269 6f72 6974 7952  PatchedPriorityR
+0001ba30: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
+0001ba40: 6174 6368 6564 5072 6f63 6573 736f 7248  atchedProcessorH
+0001ba50: 616e 646c 6572 5265 7175 6573 745d 2864  andlerRequest](d
+0001ba60: 6f63 732f 5061 7463 6865 6450 726f 6365  ocs/PatchedProce
+0001ba70: 7373 6f72 4861 6e64 6c65 7252 6571 7565  ssorHandlerReque
+0001ba80: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001ba90: 6564 5072 6f6a 6563 7441 6363 6573 7354  edProjectAccessT
+0001baa0: 6f6b 656e 5265 7175 6573 745d 2864 6f63  okenRequest](doc
+0001bab0: 732f 5061 7463 6865 6450 726f 6a65 6374  s/PatchedProject
+0001bac0: 4163 6365 7373 546f 6b65 6e52 6571 7565  AccessTokenReque
+0001bad0: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001bae0: 6564 5072 6f6a 6563 7452 6571 7565 7374  edProjectRequest
+0001baf0: 5d28 646f 6373 2f50 6174 6368 6564 5072  ](docs/PatchedPr
+0001bb00: 6f6a 6563 7452 6571 7565 7374 2e6d 6429  ojectRequest.md)
+0001bb10: 0a20 2d20 5b50 6174 6368 6564 5072 6f70  . - [PatchedProp
+0001bb20: 6572 7479 4465 6669 6e69 7469 6f6e 5265  ertyDefinitionRe
+0001bb30: 7175 6573 745d 2864 6f63 732f 5061 7463  quest](docs/Patc
+0001bb40: 6865 6450 726f 7065 7274 7944 6566 696e  hedPropertyDefin
+0001bb50: 6974 696f 6e52 6571 7565 7374 2e6d 6429  itionRequest.md)
+0001bb60: 0a20 2d20 5b50 6174 6368 6564 5072 6f70  . - [PatchedProp
+0001bb70: 6572 7479 5265 7175 6573 745d 2864 6f63  ertyRequest](doc
+0001bb80: 732f 5061 7463 6865 6450 726f 7065 7274  s/PatchedPropert
+0001bb90: 7952 6571 7565 7374 2e6d 6429 0a20 2d20  yRequest.md). - 
+0001bba0: 5b50 6174 6368 6564 5072 6f70 6572 7479  [PatchedProperty
+0001bbb0: 5365 7452 6571 7565 7374 5d28 646f 6373  SetRequest](docs
+0001bbc0: 2f50 6174 6368 6564 5072 6f70 6572 7479  /PatchedProperty
+0001bbd0: 5365 7452 6571 7565 7374 2e6d 6429 0a20  SetRequest.md). 
+0001bbe0: 2d20 5b50 6174 6368 6564 5275 6c65 436f  - [PatchedRuleCo
+0001bbf0: 6d70 6f6e 656e 7452 6571 7565 7374 5d28  mponentRequest](
+0001bc00: 646f 6373 2f50 6174 6368 6564 5275 6c65  docs/PatchedRule
+0001bc10: 436f 6d70 6f6e 656e 7452 6571 7565 7374  ComponentRequest
+0001bc20: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001bc30: 5275 6c65 5265 7175 6573 745d 2864 6f63  RuleRequest](doc
+0001bc40: 732f 5061 7463 6865 6452 756c 6552 6571  s/PatchedRuleReq
+0001bc50: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001bc60: 6368 6564 5275 6c65 7365 7452 6571 7565  chedRulesetReque
+0001bc70: 7374 5d28 646f 6373 2f50 6174 6368 6564  st](docs/Patched
+0001bc80: 5275 6c65 7365 7452 6571 7565 7374 2e6d  RulesetRequest.m
+0001bc90: 6429 0a20 2d20 5b50 6174 6368 6564 5370  d). - [PatchedSp
+0001bca0: 6163 6552 6571 7565 7374 5d28 646f 6373  aceRequest](docs
+0001bcb0: 2f50 6174 6368 6564 5370 6163 6552 6571  /PatchedSpaceReq
+0001bcc0: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001bcd0: 6368 6564 5374 6167 6552 6571 7565 7374  chedStageRequest
+0001bce0: 5d28 646f 6373 2f50 6174 6368 6564 5374  ](docs/PatchedSt
+0001bcf0: 6167 6552 6571 7565 7374 2e6d 6429 0a20  ageRequest.md). 
+0001bd00: 2d20 5b50 6174 6368 6564 5374 6f72 6579  - [PatchedStorey
+0001bd10: 4275 696c 6469 6e67 5265 7175 6573 745d  BuildingRequest]
+0001bd20: 2864 6f63 732f 5061 7463 6865 6453 746f  (docs/PatchedSto
+0001bd30: 7265 7942 7569 6c64 696e 6752 6571 7565  reyBuildingReque
+0001bd40: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001bd50: 6564 5379 7374 656d 5265 7175 6573 745d  edSystemRequest]
+0001bd60: 2864 6f63 732f 5061 7463 6865 6453 7973  (docs/PatchedSys
+0001bd70: 7465 6d52 6571 7565 7374 2e6d 6429 0a20  temRequest.md). 
+0001bd80: 2d20 5b50 6174 6368 6564 5461 6752 6571  - [PatchedTagReq
+0001bd90: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
+0001bda0: 6564 5461 6752 6571 7565 7374 2e6d 6429  edTagRequest.md)
+0001bdb0: 0a20 2d20 5b50 6174 6368 6564 546f 7069  . - [PatchedTopi
+0001bdc0: 6352 6571 7565 7374 5d28 646f 6373 2f50  cRequest](docs/P
+0001bdd0: 6174 6368 6564 546f 7069 6352 6571 7565  atchedTopicReque
+0001bde0: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001bdf0: 6564 546f 7069 6353 7461 7475 7352 6571  edTopicStatusReq
+0001be00: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
+0001be10: 6564 546f 7069 6353 7461 7475 7352 6571  edTopicStatusReq
+0001be20: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001be30: 6368 6564 546f 7069 6354 7970 6552 6571  chedTopicTypeReq
+0001be40: 7565 7374 5d28 646f 6373 2f50 6174 6368  uest](docs/Patch
+0001be50: 6564 546f 7069 6354 7970 6552 6571 7565  edTopicTypeReque
+0001be60: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001be70: 6564 556e 6974 5265 7175 6573 745d 2864  edUnitRequest](d
+0001be80: 6f63 732f 5061 7463 6865 6455 6e69 7452  ocs/PatchedUnitR
+0001be90: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
+0001bea0: 6174 6368 6564 5573 6572 436c 6f75 6455  atchedUserCloudU
+0001beb0: 7064 6174 6552 6571 7565 7374 5d28 646f  pdateRequest](do
+0001bec0: 6373 2f50 6174 6368 6564 5573 6572 436c  cs/PatchedUserCl
+0001bed0: 6f75 6455 7064 6174 6552 6571 7565 7374  oudUpdateRequest
+0001bee0: 2e6d 6429 0a20 2d20 5b50 6174 6368 6564  .md). - [Patched
+0001bef0: 5573 6572 5072 6f6a 6563 7455 7064 6174  UserProjectUpdat
+0001bf00: 6552 6571 7565 7374 5d28 646f 6373 2f50  eRequest](docs/P
+0001bf10: 6174 6368 6564 5573 6572 5072 6f6a 6563  atchedUserProjec
+0001bf20: 7455 7064 6174 6552 6571 7565 7374 2e6d  tUpdateRequest.m
+0001bf30: 6429 0a20 2d20 5b50 6174 6368 6564 5669  d). - [PatchedVi
+0001bf40: 6577 706f 696e 7452 6571 7565 7374 5d28  ewpointRequest](
+0001bf50: 646f 6373 2f50 6174 6368 6564 5669 6577  docs/PatchedView
+0001bf60: 706f 696e 7452 6571 7565 7374 2e6d 6429  pointRequest.md)
+0001bf70: 0a20 2d20 5b50 6174 6368 6564 5669 7361  . - [PatchedVisa
+0001bf80: 436f 6d6d 656e 7452 6571 7565 7374 5d28  CommentRequest](
+0001bf90: 646f 6373 2f50 6174 6368 6564 5669 7361  docs/PatchedVisa
+0001bfa0: 436f 6d6d 656e 7452 6571 7565 7374 2e6d  CommentRequest.m
+0001bfb0: 6429 0a20 2d20 5b50 6174 6368 6564 5669  d). - [PatchedVi
+0001bfc0: 7361 5265 7175 6573 745d 2864 6f63 732f  saRequest](docs/
+0001bfd0: 5061 7463 6865 6456 6973 6152 6571 7565  PatchedVisaReque
+0001bfe0: 7374 2e6d 6429 0a20 2d20 5b50 6174 6368  st.md). - [Patch
+0001bff0: 6564 5669 7361 5661 6c69 6461 7469 6f6e  edVisaValidation
+0001c000: 5265 7175 6573 745d 2864 6f63 732f 5061  Request](docs/Pa
+0001c010: 7463 6865 6456 6973 6156 616c 6964 6174  tchedVisaValidat
+0001c020: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
+0001c030: 2d20 5b50 6174 6368 6564 5765 6248 6f6f  - [PatchedWebHoo
+0001c040: 6b52 6571 7565 7374 5d28 646f 6373 2f50  kRequest](docs/P
+0001c050: 6174 6368 6564 5765 6248 6f6f 6b52 6571  atchedWebHookReq
+0001c060: 7565 7374 2e6d 6429 0a20 2d20 5b50 6174  uest.md). - [Pat
+0001c070: 6368 6564 5a6f 6e65 5265 7175 6573 745d  chedZoneRequest]
+0001c080: 2864 6f63 732f 5061 7463 6865 645a 6f6e  (docs/PatchedZon
+0001c090: 6552 6571 7565 7374 2e6d 6429 0a20 2d20  eRequest.md). - 
+0001c0a0: 5b50 6174 6368 6564 5a6f 6e65 5370 6163  [PatchedZoneSpac
+0001c0b0: 6552 6571 7565 7374 5d28 646f 6373 2f50  eRequest](docs/P
+0001c0c0: 6174 6368 6564 5a6f 6e65 5370 6163 6552  atchedZoneSpaceR
+0001c0d0: 6571 7565 7374 2e6d 6429 0a20 2d20 5b50  equest.md). - [P
+0001c0e0: 6572 7370 6563 7469 7665 4361 6d65 7261  erspectiveCamera
+0001c0f0: 5d28 646f 6373 2f50 6572 7370 6563 7469  ](docs/Perspecti
+0001c100: 7665 4361 6d65 7261 2e6d 6429 0a20 2d20  veCamera.md). - 
+0001c110: 5b50 6572 7370 6563 7469 7665 4361 6d65  [PerspectiveCame
+0001c120: 7261 5265 7175 6573 745d 2864 6f63 732f  raRequest](docs/
+0001c130: 5065 7273 7065 6374 6976 6543 616d 6572  PerspectiveCamer
+0001c140: 6152 6571 7565 7374 2e6d 6429 0a20 2d20  aRequest.md). - 
+0001c150: 5b50 696e 5d28 646f 6373 2f50 696e 2e6d  [Pin](docs/Pin.m
+0001c160: 6429 0a20 2d20 5b50 696e 5265 7175 6573  d). - [PinReques
+0001c170: 745d 2864 6f63 732f 5069 6e52 6571 7565  t](docs/PinReque
+0001c180: 7374 2e6d 6429 0a20 2d20 5b50 6f69 6e74  st.md). - [Point
+0001c190: 5d28 646f 6373 2f50 6f69 6e74 2e6d 6429  ](docs/Point.md)
+0001c1a0: 0a20 2d20 5b50 6f69 6e74 5265 7175 6573  . - [PointReques
+0001c1b0: 745d 2864 6f63 732f 506f 696e 7452 6571  t](docs/PointReq
+0001c1c0: 7565 7374 2e6d 6429 0a20 2d20 5b50 6f73  uest.md). - [Pos
+0001c1d0: 6974 696f 6e69 6e67 506c 616e 5d28 646f  itioningPlan](do
+0001c1e0: 6373 2f50 6f73 6974 696f 6e69 6e67 506c  cs/PositioningPl
+0001c1f0: 616e 2e6d 6429 0a20 2d20 5b50 7269 6f72  an.md). - [Prior
+0001c200: 6974 795d 2864 6f63 732f 5072 696f 7269  ity](docs/Priori
+0001c210: 7479 2e6d 6429 0a20 2d20 5b50 7269 6f72  ty.md). - [Prior
+0001c220: 6974 7952 6571 7565 7374 5d28 646f 6373  ityRequest](docs
+0001c230: 2f50 7269 6f72 6974 7952 6571 7565 7374  /PriorityRequest
+0001c240: 2e6d 6429 0a20 2d20 5b50 726f 6365 7373  .md). - [Process
+0001c250: 6f72 4861 6e64 6c65 725d 2864 6f63 732f  orHandler](docs/
+0001c260: 5072 6f63 6573 736f 7248 616e 646c 6572  ProcessorHandler
+0001c270: 2e6d 6429 0a20 2d20 5b50 726f 6a65 6374  .md). - [Project
+0001c280: 5d28 646f 6373 2f50 726f 6a65 6374 2e6d  ](docs/Project.m
+0001c290: 6429 0a20 2d20 5b50 726f 6a65 6374 4163  d). - [ProjectAc
+0001c2a0: 6365 7373 546f 6b65 6e5d 2864 6f63 732f  cessToken](docs/
+0001c2b0: 5072 6f6a 6563 7441 6363 6573 7354 6f6b  ProjectAccessTok
+0001c2c0: 656e 2e6d 6429 0a20 2d20 5b50 726f 6a65  en.md). - [Proje
+0001c2d0: 6374 4163 6365 7373 546f 6b65 6e52 6571  ctAccessTokenReq
+0001c2e0: 7565 7374 5d28 646f 6373 2f50 726f 6a65  uest](docs/Proje
+0001c2f0: 6374 4163 6365 7373 546f 6b65 6e52 6571  ctAccessTokenReq
+0001c300: 7565 7374 2e6d 6429 0a20 2d20 5b50 726f  uest.md). - [Pro
+0001c310: 6a65 6374 466f 6c64 6572 5472 6565 5d28  jectFolderTree](
+0001c320: 646f 6373 2f50 726f 6a65 6374 466f 6c64  docs/ProjectFold
+0001c330: 6572 5472 6565 2e6d 6429 0a20 2d20 5b50  erTree.md). - [P
+0001c340: 726f 6a65 6374 496e 7669 7461 7469 6f6e  rojectInvitation
+0001c350: 5d28 646f 6373 2f50 726f 6a65 6374 496e  ](docs/ProjectIn
+0001c360: 7669 7461 7469 6f6e 2e6d 6429 0a20 2d20  vitation.md). - 
+0001c370: 5b50 726f 6a65 6374 496e 7669 7461 7469  [ProjectInvitati
+0001c380: 6f6e 5265 7175 6573 745d 2864 6f63 732f  onRequest](docs/
+0001c390: 5072 6f6a 6563 7449 6e76 6974 6174 696f  ProjectInvitatio
+0001c3a0: 6e52 6571 7565 7374 2e6d 6429 0a20 2d20  nRequest.md). - 
+0001c3b0: 5b50 726f 6a65 6374 5265 7175 6573 745d  [ProjectRequest]
+0001c3c0: 2864 6f63 732f 5072 6f6a 6563 7452 6571  (docs/ProjectReq
+0001c3d0: 7565 7374 2e6d 6429 0a20 2d20 5b50 726f  uest.md). - [Pro
+0001c3e0: 6a65 6374 526f 6c65 5d28 646f 6373 2f50  jectRole](docs/P
+0001c3f0: 726f 6a65 6374 526f 6c65 2e6d 6429 0a20  rojectRole.md). 
+0001c400: 2d20 5b50 726f 6a65 6374 5369 7a65 5d28  - [ProjectSize](
+0001c410: 646f 6373 2f50 726f 6a65 6374 5369 7a65  docs/ProjectSize
+0001c420: 2e6d 6429 0a20 2d20 5b50 726f 6a65 6374  .md). - [Project
+0001c430: 5769 7468 4368 696c 6472 656e 5d28 646f  WithChildren](do
+0001c440: 6373 2f50 726f 6a65 6374 5769 7468 4368  cs/ProjectWithCh
+0001c450: 696c 6472 656e 2e6d 6429 0a20 2d20 5b50  ildren.md). - [P
+0001c460: 726f 7065 7274 7944 6566 696e 6974 696f  ropertyDefinitio
+0001c470: 6e5d 2864 6f63 732f 5072 6f70 6572 7479  n](docs/Property
+0001c480: 4465 6669 6e69 7469 6f6e 2e6d 6429 0a20  Definition.md). 
+0001c490: 2d20 5b50 726f 7065 7274 7944 6566 696e  - [PropertyDefin
+0001c4a0: 6974 696f 6e52 6571 7565 7374 5d28 646f  itionRequest](do
+0001c4b0: 6373 2f50 726f 7065 7274 7944 6566 696e  cs/PropertyDefin
+0001c4c0: 6974 696f 6e52 6571 7565 7374 2e6d 6429  itionRequest.md)
+0001c4d0: 0a20 2d20 5b50 726f 7065 7274 7952 6571  . - [PropertyReq
+0001c4e0: 7565 7374 5d28 646f 6373 2f50 726f 7065  uest](docs/Prope
+0001c4f0: 7274 7952 6571 7565 7374 2e6d 6429 0a20  rtyRequest.md). 
+0001c500: 2d20 5b50 726f 7065 7274 7953 6574 5d28  - [PropertySet](
+0001c510: 646f 6373 2f50 726f 7065 7274 7953 6574  docs/PropertySet
+0001c520: 2e6d 6429 0a20 2d20 5b50 726f 7065 7274  .md). - [Propert
+0001c530: 7953 6574 5265 7175 6573 745d 2864 6f63  ySetRequest](doc
+0001c540: 732f 5072 6f70 6572 7479 5365 7452 6571  s/PropertySetReq
+0001c550: 7565 7374 2e6d 6429 0a20 2d20 5b50 7562  uest.md). - [Pub
+0001c560: 6c69 634f 7267 616e 697a 6174 696f 6e5d  licOrganization]
+0001c570: 2864 6f63 732f 5075 626c 6963 4f72 6761  (docs/PublicOrga
+0001c580: 6e69 7a61 7469 6f6e 2e6d 6429 0a20 2d20  nization.md). - 
+0001c590: 5b50 7562 6c69 634f 7267 616e 697a 6174  [PublicOrganizat
+0001c5a0: 696f 6e52 6571 7565 7374 5d28 646f 6373  ionRequest](docs
+0001c5b0: 2f50 7562 6c69 634f 7267 616e 697a 6174  /PublicOrganizat
+0001c5c0: 696f 6e52 6571 7565 7374 2e6d 6429 0a20  ionRequest.md). 
+0001c5d0: 2d20 5b52 6177 436c 6173 7369 6669 6361  - [RawClassifica
+0001c5e0: 7469 6f6e 5d28 646f 6373 2f52 6177 436c  tion](docs/RawCl
+0001c5f0: 6173 7369 6669 6361 7469 6f6e 2e6d 6429  assification.md)
+0001c600: 0a20 2d20 5b52 6177 436c 6173 7369 6669  . - [RawClassifi
+0001c610: 6361 7469 6f6e 5265 7175 6573 745d 2864  cationRequest](d
+0001c620: 6f63 732f 5261 7743 6c61 7373 6966 6963  ocs/RawClassific
+0001c630: 6174 696f 6e52 6571 7565 7374 2e6d 6429  ationRequest.md)
+0001c640: 0a20 2d20 5b52 6177 4465 6669 6e69 7469  . - [RawDefiniti
+0001c650: 6f6e 5d28 646f 6373 2f52 6177 4465 6669  on](docs/RawDefi
+0001c660: 6e69 7469 6f6e 2e6d 6429 0a20 2d20 5b52  nition.md). - [R
+0001c670: 6177 4465 6669 6e69 7469 6f6e 5265 7175  awDefinitionRequ
+0001c680: 6573 745d 2864 6f63 732f 5261 7744 6566  est](docs/RawDef
+0001c690: 696e 6974 696f 6e52 6571 7565 7374 2e6d  initionRequest.m
+0001c6a0: 6429 0a20 2d20 5b52 6177 456c 656d 656e  d). - [RawElemen
+0001c6b0: 745d 2864 6f63 732f 5261 7745 6c65 6d65  t](docs/RawEleme
+0001c6c0: 6e74 2e6d 6429 0a20 2d20 5b52 6177 456c  nt.md). - [RawEl
+0001c6d0: 656d 656e 7452 6571 7565 7374 5d28 646f  ementRequest](do
+0001c6e0: 6373 2f52 6177 456c 656d 656e 7452 6571  cs/RawElementReq
+0001c6f0: 7565 7374 2e6d 6429 0a20 2d20 5b52 6177  uest.md). - [Raw
+0001c700: 456c 656d 656e 7473 5d28 646f 6373 2f52  Elements](docs/R
+0001c710: 6177 456c 656d 656e 7473 2e6d 6429 0a20  awElements.md). 
+0001c720: 2d20 5b52 6177 456c 656d 656e 7473 5265  - [RawElementsRe
+0001c730: 7175 6573 745d 2864 6f63 732f 5261 7745  quest](docs/RawE
+0001c740: 6c65 6d65 6e74 7352 6571 7565 7374 2e6d  lementsRequest.m
+0001c750: 6429 0a20 2d20 5b52 6177 4c61 7965 725d  d). - [RawLayer]
+0001c760: 2864 6f63 732f 5261 774c 6179 6572 2e6d  (docs/RawLayer.m
+0001c770: 6429 0a20 2d20 5b52 6177 4c61 7965 7252  d). - [RawLayerR
+0001c780: 6571 7565 7374 5d28 646f 6373 2f52 6177  equest](docs/Raw
+0001c790: 4c61 7965 7252 6571 7565 7374 2e6d 6429  LayerRequest.md)
+0001c7a0: 0a20 2d20 5b52 6177 4d61 7465 7269 616c  . - [RawMaterial
+0001c7b0: 5d28 646f 6373 2f52 6177 4d61 7465 7269  ](docs/RawMateri
+0001c7c0: 616c 2e6d 6429 0a20 2d20 5b52 6177 4d61  al.md). - [RawMa
+0001c7d0: 7465 7269 616c 4c69 7374 5d28 646f 6373  terialList](docs
+0001c7e0: 2f52 6177 4d61 7465 7269 616c 4c69 7374  /RawMaterialList
+0001c7f0: 2e6d 6429 0a20 2d20 5b52 6177 4d61 7465  .md). - [RawMate
+0001c800: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
+0001c810: 7473 5d28 646f 6373 2f52 6177 4d61 7465  ts](docs/RawMate
+0001c820: 7269 616c 4c69 7374 436f 6d70 6f6e 656e  rialListComponen
+0001c830: 7473 2e6d 6429 0a20 2d20 5b52 6177 4d61  ts.md). - [RawMa
+0001c840: 7465 7269 616c 4c69 7374 436f 6d70 6f6e  terialListCompon
+0001c850: 656e 7473 5265 7175 6573 745d 2864 6f63  entsRequest](doc
+0001c860: 732f 5261 774d 6174 6572 6961 6c4c 6973  s/RawMaterialLis
+0001c870: 7443 6f6d 706f 6e65 6e74 7352 6571 7565  tComponentsReque
+0001c880: 7374 2e6d 6429 0a20 2d20 5b52 6177 4d61  st.md). - [RawMa
+0001c890: 7465 7269 616c 4c69 7374 5265 7175 6573  terialListReques
+0001c8a0: 745d 2864 6f63 732f 5261 774d 6174 6572  t](docs/RawMater
+0001c8b0: 6961 6c4c 6973 7452 6571 7565 7374 2e6d  ialListRequest.m
+0001c8c0: 6429 0a20 2d20 5b52 6177 4d61 7465 7269  d). - [RawMateri
+0001c8d0: 616c 4f70 7469 6f6e 735d 2864 6f63 732f  alOptions](docs/
+0001c8e0: 5261 774d 6174 6572 6961 6c4f 7074 696f  RawMaterialOptio
+0001c8f0: 6e73 2e6d 6429 0a20 2d20 5b52 6177 4d61  ns.md). - [RawMa
+0001c900: 7465 7269 616c 4f70 7469 6f6e 7352 6571  terialOptionsReq
+0001c910: 7565 7374 5d28 646f 6373 2f52 6177 4d61  uest](docs/RawMa
+0001c920: 7465 7269 616c 4f70 7469 6f6e 7352 6571  terialOptionsReq
+0001c930: 7565 7374 2e6d 6429 0a20 2d20 5b52 6177  uest.md). - [Raw
+0001c940: 4d61 7465 7269 616c 5265 7175 6573 745d  MaterialRequest]
+0001c950: 2864 6f63 732f 5261 774d 6174 6572 6961  (docs/RawMateria
+0001c960: 6c52 6571 7565 7374 2e6d 6429 0a20 2d20  lRequest.md). - 
+0001c970: 5b52 6177 5072 6f70 6572 7479 5d28 646f  [RawProperty](do
+0001c980: 6373 2f52 6177 5072 6f70 6572 7479 2e6d  cs/RawProperty.m
+0001c990: 6429 0a20 2d20 5b52 6177 5072 6f70 6572  d). - [RawProper
+0001c9a0: 7479 5265 7175 6573 745d 2864 6f63 732f  tyRequest](docs/
+0001c9b0: 5261 7750 726f 7065 7274 7952 6571 7565  RawPropertyReque
+0001c9c0: 7374 2e6d 6429 0a20 2d20 5b52 6177 5072  st.md). - [RawPr
+0001c9d0: 6f70 6572 7479 5365 745d 2864 6f63 732f  opertySet](docs/
+0001c9e0: 5261 7750 726f 7065 7274 7953 6574 2e6d  RawPropertySet.m
+0001c9f0: 6429 0a20 2d20 5b52 6177 5072 6f70 6572  d). - [RawProper
+0001ca00: 7479 5365 7452 6571 7565 7374 5d28 646f  tySetRequest](do
+0001ca10: 6373 2f52 6177 5072 6f70 6572 7479 5365  cs/RawPropertySe
+0001ca20: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
+0001ca30: 5b52 6177 5379 7374 656d 5d28 646f 6373  [RawSystem](docs
+0001ca40: 2f52 6177 5379 7374 656d 2e6d 6429 0a20  /RawSystem.md). 
+0001ca50: 2d20 5b52 6177 5379 7374 656d 5265 7175  - [RawSystemRequ
+0001ca60: 6573 745d 2864 6f63 732f 5261 7753 7973  est](docs/RawSys
+0001ca70: 7465 6d52 6571 7565 7374 2e6d 6429 0a20  temRequest.md). 
+0001ca80: 2d20 5b52 6177 556e 6974 5d28 646f 6373  - [RawUnit](docs
+0001ca90: 2f52 6177 556e 6974 2e6d 6429 0a20 2d20  /RawUnit.md). - 
+0001caa0: 5b52 6177 556e 6974 5265 7175 6573 745d  [RawUnitRequest]
+0001cab0: 2864 6f63 732f 5261 7755 6e69 7452 6571  (docs/RawUnitReq
+0001cac0: 7565 7374 2e6d 6429 0a20 2d20 5b52 6563  uest.md). - [Rec
+0001cad0: 7572 7369 7665 466f 6c64 6572 4368 696c  ursiveFolderChil
+0001cae0: 6472 656e 5d28 646f 6373 2f52 6563 7572  dren](docs/Recur
+0001caf0: 7369 7665 466f 6c64 6572 4368 696c 6472  siveFolderChildr
+0001cb00: 656e 2e6d 6429 0a20 2d20 5b52 756c 655d  en.md). - [Rule]
+0001cb10: 2864 6f63 732f 5275 6c65 2e6d 6429 0a20  (docs/Rule.md). 
+0001cb20: 2d20 5b52 756c 6543 6f6d 706f 6e65 6e74  - [RuleComponent
+0001cb30: 5d28 646f 6373 2f52 756c 6543 6f6d 706f  ](docs/RuleCompo
+0001cb40: 6e65 6e74 2e6d 6429 0a20 2d20 5b52 756c  nent.md). - [Rul
+0001cb50: 6543 6f6d 706f 6e65 6e74 5265 7175 6573  eComponentReques
+0001cb60: 745d 2864 6f63 732f 5275 6c65 436f 6d70  t](docs/RuleComp
+0001cb70: 6f6e 656e 7452 6571 7565 7374 2e6d 6429  onentRequest.md)
+0001cb80: 0a20 2d20 5b52 756c 6552 6571 7565 7374  . - [RuleRequest
+0001cb90: 5d28 646f 6373 2f52 756c 6552 6571 7565  ](docs/RuleReque
+0001cba0: 7374 2e6d 6429 0a20 2d20 5b52 756c 6573  st.md). - [Rules
+0001cbb0: 6574 5d28 646f 6373 2f52 756c 6573 6574  et](docs/Ruleset
+0001cbc0: 2e6d 6429 0a20 2d20 5b52 756c 6573 6574  .md). - [Ruleset
+0001cbd0: 5265 7175 6573 745d 2864 6f63 732f 5275  Request](docs/Ru
+0001cbe0: 6c65 7365 7452 6571 7565 7374 2e6d 6429  lesetRequest.md)
+0001cbf0: 0a20 2d20 5b53 656c 6642 6366 5573 6572  . - [SelfBcfUser
+0001cc00: 5d28 646f 6373 2f53 656c 6642 6366 5573  ](docs/SelfBcfUs
+0001cc10: 6572 2e6d 6429 0a20 2d20 5b53 656c 6655  er.md). - [SelfU
+0001cc20: 7365 725d 2864 6f63 732f 5365 6c66 5573  ser](docs/SelfUs
+0001cc30: 6572 2e6d 6429 0a20 2d20 5b53 696d 706c  er.md). - [Simpl
+0001cc40: 6545 6c65 6d65 6e74 5d28 646f 6373 2f53  eElement](docs/S
+0001cc50: 696d 706c 6545 6c65 6d65 6e74 2e6d 6429  impleElement.md)
+0001cc60: 0a20 2d20 5b53 697a 655d 2864 6f63 732f  . - [Size](docs/
+0001cc70: 5369 7a65 2e6d 6429 0a20 2d20 5b53 6e61  Size.md). - [Sna
+0001cc80: 7073 686f 745d 2864 6f63 732f 536e 6170  pshot](docs/Snap
+0001cc90: 7368 6f74 2e6d 6429 0a20 2d20 5b53 6e61  shot.md). - [Sna
+0001cca0: 7073 686f 7452 6571 7565 7374 5d28 646f  pshotRequest](do
+0001ccb0: 6373 2f53 6e61 7073 686f 7452 6571 7565  cs/SnapshotReque
+0001ccc0: 7374 2e6d 6429 0a20 2d20 5b53 7061 6365  st.md). - [Space
+0001ccd0: 5d28 646f 6373 2f53 7061 6365 2e6d 6429  ](docs/Space.md)
+0001cce0: 0a20 2d20 5b53 7061 6365 5265 7175 6573  . - [SpaceReques
+0001ccf0: 745d 2864 6f63 732f 5370 6163 6552 6571  t](docs/SpaceReq
+0001cd00: 7565 7374 2e6d 6429 0a20 2d20 5b53 7461  uest.md). - [Sta
+0001cd10: 6765 5d28 646f 6373 2f53 7461 6765 2e6d  ge](docs/Stage.m
+0001cd20: 6429 0a20 2d20 5b53 7461 6765 5265 7175  d). - [StageRequ
+0001cd30: 6573 745d 2864 6f63 732f 5374 6167 6552  est](docs/StageR
+0001cd40: 6571 7565 7374 2e6d 6429 0a20 2d20 5b53  equest.md). - [S
+0001cd50: 746f 7265 795d 2864 6f63 732f 5374 6f72  torey](docs/Stor
+0001cd60: 6579 2e6d 6429 0a20 2d20 5b53 746f 7265  ey.md). - [Store
+0001cd70: 7942 7569 6c64 696e 6752 6571 7565 7374  yBuildingRequest
+0001cd80: 5d28 646f 6373 2f53 746f 7265 7942 7569  ](docs/StoreyBui
+0001cd90: 6c64 696e 6752 6571 7565 7374 2e6d 6429  ldingRequest.md)
+0001cda0: 0a20 2d20 5b53 746f 7265 794d 6f64 656c  . - [StoreyModel
+0001cdb0: 506c 616e 5265 7175 6573 745d 2864 6f63  PlanRequest](doc
+0001cdc0: 732f 5374 6f72 6579 4d6f 6465 6c50 6c61  s/StoreyModelPla
+0001cdd0: 6e52 6571 7565 7374 2e6d 6429 0a20 2d20  nRequest.md). - 
+0001cde0: 5b53 7973 7465 6d5d 2864 6f63 732f 5379  [System](docs/Sy
+0001cdf0: 7374 656d 2e6d 6429 0a20 2d20 5b53 7973  stem.md). - [Sys
+0001ce00: 7465 6d52 6571 7565 7374 5d28 646f 6373  temRequest](docs
+0001ce10: 2f53 7973 7465 6d52 6571 7565 7374 2e6d  /SystemRequest.m
+0001ce20: 6429 0a20 2d20 5b54 6167 5d28 646f 6373  d). - [Tag](docs
+0001ce30: 2f54 6167 2e6d 6429 0a20 2d20 5b54 6167  /Tag.md). - [Tag
+0001ce40: 4964 5265 7175 6573 745d 2864 6f63 732f  IdRequest](docs/
+0001ce50: 5461 6749 6452 6571 7565 7374 2e6d 6429  TagIdRequest.md)
+0001ce60: 0a20 2d20 5b54 6167 5265 7175 6573 745d  . - [TagRequest]
+0001ce70: 2864 6f63 732f 5461 6752 6571 7565 7374  (docs/TagRequest
+0001ce80: 2e6d 6429 0a20 2d20 5b54 6f70 6963 5d28  .md). - [Topic](
+0001ce90: 646f 6373 2f54 6f70 6963 2e6d 6429 0a20  docs/Topic.md). 
+0001cea0: 2d20 5b54 6f70 6963 5265 7175 6573 745d  - [TopicRequest]
+0001ceb0: 2864 6f63 732f 546f 7069 6352 6571 7565  (docs/TopicReque
+0001cec0: 7374 2e6d 6429 0a20 2d20 5b54 6f70 6963  st.md). - [Topic
+0001ced0: 5374 6174 7573 5d28 646f 6373 2f54 6f70  Status](docs/Top
+0001cee0: 6963 5374 6174 7573 2e6d 6429 0a20 2d20  icStatus.md). - 
+0001cef0: 5b54 6f70 6963 5374 6174 7573 5265 7175  [TopicStatusRequ
+0001cf00: 6573 745d 2864 6f63 732f 546f 7069 6353  est](docs/TopicS
+0001cf10: 7461 7475 7352 6571 7565 7374 2e6d 6429  tatusRequest.md)
+0001cf20: 0a20 2d20 5b54 6f70 6963 5479 7065 5d28  . - [TopicType](
+0001cf30: 646f 6373 2f54 6f70 6963 5479 7065 2e6d  docs/TopicType.m
+0001cf40: 6429 0a20 2d20 5b54 6f70 6963 5479 7065  d). - [TopicType
+0001cf50: 5265 7175 6573 745d 2864 6f63 732f 546f  Request](docs/To
+0001cf60: 7069 6354 7970 6552 6571 7565 7374 2e6d  picTypeRequest.m
+0001cf70: 6429 0a20 2d20 5b55 6e69 745d 2864 6f63  d). - [Unit](doc
+0001cf80: 732f 556e 6974 2e6d 6429 0a20 2d20 5b55  s/Unit.md). - [U
+0001cf90: 6e69 7452 6571 7565 7374 5d28 646f 6373  nitRequest](docs
+0001cfa0: 2f55 6e69 7452 6571 7565 7374 2e6d 6429  /UnitRequest.md)
+0001cfb0: 0a20 2d20 5b55 7365 725d 2864 6f63 732f  . - [User](docs/
+0001cfc0: 5573 6572 2e6d 6429 0a20 2d20 5b55 7365  User.md). - [Use
+0001cfd0: 7249 6e76 6974 6174 696f 6e5d 2864 6f63  rInvitation](doc
+0001cfe0: 732f 5573 6572 496e 7669 7461 7469 6f6e  s/UserInvitation
+0001cff0: 2e6d 6429 0a20 2d20 5b55 7365 7250 726f  .md). - [UserPro
+0001d000: 6a65 6374 5d28 646f 6373 2f55 7365 7250  ject](docs/UserP
+0001d010: 726f 6a65 6374 2e6d 6429 0a20 2d20 5b55  roject.md). - [U
+0001d020: 7365 7250 726f 6a65 6374 4964 5265 7175  serProjectIdRequ
+0001d030: 6573 745d 2864 6f63 732f 5573 6572 5072  est](docs/UserPr
+0001d040: 6f6a 6563 7449 6452 6571 7565 7374 2e6d  ojectIdRequest.m
+0001d050: 6429 0a20 2d20 5b56 6965 7753 6574 7570  d). - [ViewSetup
+0001d060: 4869 6e74 735d 2864 6f63 732f 5669 6577  Hints](docs/View
+0001d070: 5365 7475 7048 696e 7473 2e6d 6429 0a20  SetupHints.md). 
+0001d080: 2d20 5b56 6965 7753 6574 7570 4869 6e74  - [ViewSetupHint
+0001d090: 7352 6571 7565 7374 5d28 646f 6373 2f56  sRequest](docs/V
+0001d0a0: 6965 7753 6574 7570 4869 6e74 7352 6571  iewSetupHintsReq
+0001d0b0: 7565 7374 2e6d 6429 0a20 2d20 5b56 6965  uest.md). - [Vie
+0001d0c0: 7770 6f69 6e74 5d28 646f 6373 2f56 6965  wpoint](docs/Vie
+0001d0d0: 7770 6f69 6e74 2e6d 6429 0a20 2d20 5b56  wpoint.md). - [V
+0001d0e0: 6965 7770 6f69 6e74 5265 7175 6573 745d  iewpointRequest]
+0001d0f0: 2864 6f63 732f 5669 6577 706f 696e 7452  (docs/ViewpointR
+0001d100: 6571 7565 7374 2e6d 6429 0a20 2d20 5b56  equest.md). - [V
+0001d110: 6973 615d 2864 6f63 732f 5669 7361 2e6d  isa](docs/Visa.m
+0001d120: 6429 0a20 2d20 5b56 6973 6143 6f6d 6d65  d). - [VisaComme
+0001d130: 6e74 5d28 646f 6373 2f56 6973 6143 6f6d  nt](docs/VisaCom
+0001d140: 6d65 6e74 2e6d 6429 0a20 2d20 5b56 6973  ment.md). - [Vis
+0001d150: 6143 6f6d 6d65 6e74 5265 7175 6573 745d  aCommentRequest]
+0001d160: 2864 6f63 732f 5669 7361 436f 6d6d 656e  (docs/VisaCommen
+0001d170: 7452 6571 7565 7374 2e6d 6429 0a20 2d20  tRequest.md). - 
+0001d180: 5b56 6973 6152 6571 7565 7374 5d28 646f  [VisaRequest](do
+0001d190: 6373 2f56 6973 6152 6571 7565 7374 2e6d  cs/VisaRequest.m
+0001d1a0: 6429 0a20 2d20 5b56 6973 6156 616c 6964  d). - [VisaValid
+0001d1b0: 6174 696f 6e5d 2864 6f63 732f 5669 7361  ation](docs/Visa
+0001d1c0: 5661 6c69 6461 7469 6f6e 2e6d 6429 0a20  Validation.md). 
+0001d1d0: 2d20 5b56 6973 6156 616c 6964 6174 696f  - [VisaValidatio
+0001d1e0: 6e52 6571 7565 7374 5d28 646f 6373 2f56  nRequest](docs/V
+0001d1f0: 6973 6156 616c 6964 6174 696f 6e52 6571  isaValidationReq
+0001d200: 7565 7374 2e6d 6429 0a20 2d20 5b56 6973  uest.md). - [Vis
+0001d210: 6962 696c 6974 795d 2864 6f63 732f 5669  ibility](docs/Vi
+0001d220: 7369 6269 6c69 7479 2e6d 6429 0a20 2d20  sibility.md). - 
+0001d230: 5b56 6973 6962 696c 6974 7952 6571 7565  [VisibilityReque
+0001d240: 7374 5d28 646f 6373 2f56 6973 6962 696c  st](docs/Visibil
+0001d250: 6974 7952 6571 7565 7374 2e6d 6429 0a20  ityRequest.md). 
+0001d260: 2d20 5b57 6562 486f 6f6b 5d28 646f 6373  - [WebHook](docs
+0001d270: 2f57 6562 486f 6f6b 2e6d 6429 0a20 2d20  /WebHook.md). - 
+0001d280: 5b57 6562 486f 6f6b 5265 7175 6573 745d  [WebHookRequest]
+0001d290: 2864 6f63 732f 5765 6248 6f6f 6b52 6571  (docs/WebHookReq
+0001d2a0: 7565 7374 2e6d 6429 0a20 2d20 5b57 7269  uest.md). - [Wri
+0001d2b0: 7465 466f 6c64 6572 5265 7175 6573 745d  teFolderRequest]
+0001d2c0: 2864 6f63 732f 5772 6974 6546 6f6c 6465  (docs/WriteFolde
+0001d2d0: 7252 6571 7565 7374 2e6d 6429 0a20 2d20  rRequest.md). - 
+0001d2e0: 5b5a 6f6e 655d 2864 6f63 732f 5a6f 6e65  [Zone](docs/Zone
+0001d2f0: 2e6d 6429 0a20 2d20 5b5a 6f6e 6552 6571  .md). - [ZoneReq
+0001d300: 7565 7374 5d28 646f 6373 2f5a 6f6e 6552  uest](docs/ZoneR
+0001d310: 6571 7565 7374 2e6d 6429 0a20 2d20 5b5a  equest.md). - [Z
+0001d320: 6f6e 6553 7061 6365 5d28 646f 6373 2f5a  oneSpace](docs/Z
+0001d330: 6f6e 6553 7061 6365 2e6d 6429 0a20 2d20  oneSpace.md). - 
+0001d340: 5b5a 6f6e 6553 7061 6365 5265 7175 6573  [ZoneSpaceReques
+0001d350: 745d 2864 6f63 732f 5a6f 6e65 5370 6163  t](docs/ZoneSpac
+0001d360: 6552 6571 7565 7374 2e6d 6429 0a0a 0a23  eRequest.md)...#
+0001d370: 2320 446f 6375 6d65 6e74 6174 696f 6e20  # Documentation 
+0001d380: 466f 7220 4175 7468 6f72 697a 6174 696f  For Authorizatio
+0001d390: 6e0a 0a0a 2323 2041 7069 4b65 790a 0a2d  n...## ApiKey..-
+0001d3a0: 202a 2a54 7970 652a 2a3a 2041 5049 206b   **Type**: API k
+0001d3b0: 6579 0a2d 202a 2a41 5049 206b 6579 2070  ey.- **API key p
+0001d3c0: 6172 616d 6574 6572 206e 616d 652a 2a3a  arameter name**:
+0001d3d0: 2041 7574 686f 7269 7a61 7469 6f6e 0a2d   Authorization.-
+0001d3e0: 202a 2a4c 6f63 6174 696f 6e2a 2a3a 2048   **Location**: H
+0001d3f0: 5454 5020 6865 6164 6572 0a0a 0a23 2320  TTP header...## 
+0001d400: 4249 4d44 6174 615f 436f 6e6e 6563 740a  BIMData_Connect.
+0001d410: 0a2d 202a 2a54 7970 652a 2a3a 204f 4175  .- **Type**: OAu
+0001d420: 7468 0a2d 202a 2a46 6c6f 772a 2a3a 2069  th.- **Flow**: i
+0001d430: 6d70 6c69 6369 740a 2d20 2a2a 4175 7468  mplicit.- **Auth
+0001d440: 6f72 697a 6174 696f 6e20 5552 4c2a 2a3a  orization URL**:
+0001d450: 2068 7474 703a 2f2f 6661 6b65 7572 6c2e   http://fakeurl.
+0001d460: 6269 6d64 6174 612e 696f 2f72 6561 6c6d  bimdata.io/realm
+0001d470: 732f 6269 6d64 6174 612f 7072 6f74 6f63  s/bimdata/protoc
+0001d480: 6f6c 2f6f 7065 6e69 642d 636f 6e6e 6563  ol/openid-connec
+0001d490: 742f 6175 7468 0a2d 202a 2a53 636f 7065  t/auth.- **Scope
+0001d4a0: 732a 2a3a 204e 2f41 0a0a 0a23 2320 4249  s**: N/A...## BI
+0001d4b0: 4d44 6174 615f 436f 6e6e 6563 740a 0a2d  MData_Connect..-
+0001d4c0: 202a 2a54 7970 652a 2a3a 204f 4175 7468   **Type**: OAuth
+0001d4d0: 0a2d 202a 2a46 6c6f 772a 2a3a 2061 7070  .- **Flow**: app
+0001d4e0: 6c69 6361 7469 6f6e 0a2d 202a 2a41 7574  lication.- **Aut
+0001d4f0: 686f 7269 7a61 7469 6f6e 2055 524c 2a2a  horization URL**
+0001d500: 3a20 0a2d 202a 2a53 636f 7065 732a 2a3a  : .- **Scopes**:
+0001d510: 204e 2f41 0a0a 0a23 2320 4265 6172 6572   N/A...## Bearer
+0001d520: 0a0a 2d20 2a2a 5479 7065 2a2a 3a20 4150  ..- **Type**: AP
+0001d530: 4920 6b65 790a 2d20 2a2a 4150 4920 6b65  I key.- **API ke
+0001d540: 7920 7061 7261 6d65 7465 7220 6e61 6d65  y parameter name
+0001d550: 2a2a 3a20 4175 7468 6f72 697a 6174 696f  **: Authorizatio
+0001d560: 6e0a 2d20 2a2a 4c6f 6361 7469 6f6e 2a2a  n.- **Location**
+0001d570: 3a20 4854 5450 2068 6561 6465 720a 0a0a  : HTTP header...
+0001d580: 2323 2041 7574 686f 720a 0a73 7570 706f  ## Author..suppo
+0001d590: 7274 4062 696d 6461 7461 2e69 6f0a 0a0a  rt@bimdata.io...
+0001d5a0: 2323 204e 6f74 6573 2066 6f72 204c 6172  ## Notes for Lar
+0001d5b0: 6765 204f 7065 6e41 5049 2064 6f63 756d  ge OpenAPI docum
+0001d5c0: 656e 7473 0a49 6620 7468 6520 4f70 656e  ents.If the Open
+0001d5d0: 4150 4920 646f 6375 6d65 6e74 2069 7320  API document is 
+0001d5e0: 6c61 7267 652c 2069 6d70 6f72 7473 2069  large, imports i
+0001d5f0: 6e20 6269 6d64 6174 615f 6170 695f 636c  n bimdata_api_cl
+0001d600: 6965 6e74 2e61 7069 7320 616e 6420 6269  ient.apis and bi
+0001d610: 6d64 6174 615f 6170 695f 636c 6965 6e74  mdata_api_client
+0001d620: 2e6d 6f64 656c 7320 6d61 7920 6661 696c  .models may fail
+0001d630: 2077 6974 6820 610a 5265 6375 7273 696f   with a.Recursio
+0001d640: 6e45 7272 6f72 2069 6e64 6963 6174 696e  nError indicatin
+0001d650: 6720 7468 6520 6d61 7869 6d75 6d20 7265  g the maximum re
+0001d660: 6375 7273 696f 6e20 6c69 6d69 7420 6861  cursion limit ha
+0001d670: 7320 6265 656e 2065 7863 6565 6465 642e  s been exceeded.
+0001d680: 2049 6e20 7468 6174 2063 6173 652c 2074   In that case, t
+0001d690: 6865 7265 2061 7265 2061 2063 6f75 706c  here are a coupl
+0001d6a0: 6520 6f66 2073 6f6c 7574 696f 6e73 3a0a  e of solutions:.
+0001d6b0: 0a53 6f6c 7574 696f 6e20 313a 0a55 7365  .Solution 1:.Use
+0001d6c0: 2073 7065 6369 6669 6320 696d 706f 7274   specific import
+0001d6d0: 7320 666f 7220 6170 6973 2061 6e64 206d  s for apis and m
+0001d6e0: 6f64 656c 7320 6c69 6b65 3a0a 2d20 6066  odels like:.- `f
+0001d6f0: 726f 6d20 6269 6d64 6174 615f 6170 695f  rom bimdata_api_
+0001d700: 636c 6965 6e74 2e61 7069 2e64 6566 6175  client.api.defau
+0001d710: 6c74 5f61 7069 2069 6d70 6f72 7420 4465  lt_api import De
+0001d720: 6661 756c 7441 7069 600a 2d20 6066 726f  faultApi`.- `fro
+0001d730: 6d20 6269 6d64 6174 615f 6170 695f 636c  m bimdata_api_cl
+0001d740: 6965 6e74 2e6d 6f64 656c 2e70 6574 2069  ient.model.pet i
+0001d750: 6d70 6f72 7420 5065 7460 0a0a 536f 6c75  mport Pet`..Solu
+0001d760: 7469 6f6e 2032 3a0a 4265 666f 7265 2069  tion 2:.Before i
+0001d770: 6d70 6f72 7469 6e67 2074 6865 2070 6163  mporting the pac
+0001d780: 6b61 6765 2c20 6164 6a75 7374 2074 6865  kage, adjust the
+0001d790: 206d 6178 696d 756d 2072 6563 7572 7369   maximum recursi
+0001d7a0: 6f6e 206c 696d 6974 2061 7320 7368 6f77  on limit as show
+0001d7b0: 6e20 6265 6c6f 773a 0a60 6060 0a69 6d70  n below:.```.imp
+0001d7c0: 6f72 7420 7379 730a 7379 732e 7365 7472  ort sys.sys.setr
+0001d7d0: 6563 7572 7369 6f6e 6c69 6d69 7428 3135  ecursionlimit(15
+0001d7e0: 3030 290a 696d 706f 7274 2062 696d 6461  00).import bimda
+0001d7f0: 7461 5f61 7069 5f63 6c69 656e 740a 6672  ta_api_client.fr
+0001d800: 6f6d 2062 696d 6461 7461 5f61 7069 5f63  om bimdata_api_c
+0001d810: 6c69 656e 742e 6170 6973 2069 6d70 6f72  lient.apis impor
+0001d820: 7420 2a0a 6672 6f6d 2062 696d 6461 7461  t *.from bimdata
+0001d830: 5f61 7069 5f63 6c69 656e 742e 6d6f 6465  _api_client.mode
+0001d840: 6c73 2069 6d70 6f72 7420 2a0a 6060 600a  ls import *.```.
+0001d850: 0a                                       .
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/__init__.py` & `bimdata-api-client-9.9.0/bimdata_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/bcf_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/bcf_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/checker_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/checker_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/collaboration_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/collaboration_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -8236,15 +8236,15 @@
         project_pk,
         name,
         file,
         **kwargs
     ):
         """Create a document  # noqa: E501
 
-        Create a document. If the document is one of {'PDF', 'GLTF', 'BFX', 'DAE', 'POINT_CLOUD', 'IFC', 'DXF', 'OBJ', 'DWG'}, a model will be created and attached to this document  Required scopes: document:write  # noqa: E501
+        Create a document. If the document is one of {'DAE', 'DWG', 'OBJ', 'DXF', 'PDF', 'IFC', 'GLTF', 'BFX', 'POINT_CLOUD'}, a model will be created and attached to this document  Required scopes: document:write  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_document(cloud_pk, project_pk, name, file, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/ifc_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/ifc_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/model_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/model_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/sso_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/sso_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api/webhook_api.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api/webhook_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/api_client.py` & `bimdata-api-client-9.9.0/bimdata_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/apis/__init__.py` & `bimdata-api-client-9.9.0/bimdata_api_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/configuration.py` & `bimdata-api-client-9.9.0/bimdata_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/exceptions.py` & `bimdata-api-client-9.9.0/bimdata_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/bcf_project.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/bcf_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/bcf_project_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/bcf_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/building.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/building.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/building_model_plan_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/building_model_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/check_plan.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/check_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/check_plan_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/check_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/check_project_access.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/check_project_access.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/checker_result.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/checker_result.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/checker_result_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/checker_result_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/classification.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/classification.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/classification_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/clipping_plane.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/clipping_plane.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/clipping_plane_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/clipping_plane_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/cloud.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from bimdata_api_client.model.feature import Feature
-    from bimdata_api_client.model.marketplace_app import MarketplaceApp
+    from bimdata_api_client.model.marketplace_app_light import MarketplaceAppLight
     from bimdata_api_client.model.organization import Organization
     from bimdata_api_client.model.user import User
     globals()['Feature'] = Feature
-    globals()['MarketplaceApp'] = MarketplaceApp
+    globals()['MarketplaceAppLight'] = MarketplaceAppLight
     globals()['Organization'] = Organization
     globals()['User'] = User
 
 
 class Cloud(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -96,15 +96,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (int,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'features': ([Feature],),  # noqa: E501
-            'marketplace_apps': ([MarketplaceApp],),  # noqa: E501
+            'marketplace_apps': ([MarketplaceAppLight],),  # noqa: E501
             'organization': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'creator': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'creator_app': (str,),  # noqa: E501
             'is_default': (bool,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
             'image': (str, none_type,),  # noqa: E501
@@ -148,15 +148,15 @@
     def _from_openapi_data(cls, id, name, features, marketplace_apps, organization, creator, creator_app, is_default, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """Cloud - a model defined in OpenAPI
 
         Args:
             id (int):
             name (str): Name of the cloud
             features ([Feature]):
-            marketplace_apps ([MarketplaceApp]):
+            marketplace_apps ([MarketplaceAppLight]):
             organization (bool, date, datetime, dict, float, int, list, str, none_type):
             creator (bool, date, datetime, dict, float, int, list, str, none_type):
             creator_app (str):
             is_default (bool):
             created_at (datetime): Creation date
             updated_at (datetime): Date of the last update
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_invitation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_invitation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_invitation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/cloud_role.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/cloud_role.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/coloring.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/coloring.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/coloring_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/coloring_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/comment.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/comment.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/comment_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/component.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/component_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/components_parent.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/components_parent.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/components_parent_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/components_parent_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/create_building_by_name_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/create_building_by_name_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/create_model_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/create_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/create_multi_page_model_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/create_multi_page_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/detailed_extensions.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/detailed_extensions.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/direction.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/direction.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/direction_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/direction_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/document.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/document.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/document_with_element_list.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/document_with_element_list.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/element.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/element_classification_relation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/element_classification_relation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/element_classification_relation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/element_classification_relation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/element_property_set_relation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/element_property_set_relation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/element_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/extensions.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/extensions.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/feature.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/feature.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/feature_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/feature_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_group_permission.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_group_permission.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_group_permission_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_group_permission_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_tree.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_tree.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_user_project.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_user_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_without_children.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_without_children.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/folder_without_children_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/folder_without_children_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/full_topic.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/full_topic.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/full_topic_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/full_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/group.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/group.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/group_folder.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/group_folder.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/group_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_access_token.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_access_token.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_access_token_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_checker.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_checker.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_checker_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_checker_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_export_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_export_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_merge_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_merge_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ifc_optimize_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ifc_optimize_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/import_group_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/import_group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/invitation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/label.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/label.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/label_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/label_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/layer.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/layer.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/layer_element.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/layer_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/layer_element_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/layer_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/layer_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/line.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/line.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/line_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/line_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,24 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from bimdata_api_client.model.marketplace_app_image import MarketplaceAppImage
-    from bimdata_api_client.model.public_organization import PublicOrganization
-    from bimdata_api_client.model.user import User
-    globals()['MarketplaceAppImage'] = MarketplaceAppImage
-    globals()['PublicOrganization'] = PublicOrganization
-    globals()['User'] = User
 
-
-class MarketplaceApp(ModelNormal):
+class Unit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,122 +55,81 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 256,
-        },
-        ('short_description',): {
-            'max_length': 130,
-        },
-        ('activation_webhook_url',): {
-            'max_length': 1024,
-        },
-        ('post_activation_redirect_uri',): {
-            'max_length': 1024,
-        },
-        ('settings_url',): {
-            'max_length': 1024,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'short_description': (str,),  # noqa: E501
-            'long_description': (str,),  # noqa: E501
-            'creator': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'scopes': ([str],),  # noqa: E501
-            'is_public': (bool,),  # noqa: E501
-            'images': ([MarketplaceAppImage],),  # noqa: E501
-            'organization': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'activation_webhook_url': (str, none_type,),  # noqa: E501
-            'post_activation_redirect_uri': (str, none_type,),  # noqa: E501
-            'viewer_plugins_urls': ([str], none_type,),  # noqa: E501
-            'settings_url': (str, none_type,),  # noqa: E501
-            'tags': ([str],),  # noqa: E501
-            'logo': (str, none_type,),  # noqa: E501
-            'file': (str, none_type,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'unit_type': (str, none_type,),  # noqa: E501
+            'prefix': (str, none_type,),  # noqa: E501
+            'dimensions': ([float], none_type,),  # noqa: E501
+            'conversion_factor': (float, none_type,),  # noqa: E501
+            'conversion_baseunit': (Unit,),  # noqa: E501
+            'elements': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'is_default': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'short_description': 'short_description',  # noqa: E501
-        'long_description': 'long_description',  # noqa: E501
-        'creator': 'creator',  # noqa: E501
-        'scopes': 'scopes',  # noqa: E501
-        'is_public': 'is_public',  # noqa: E501
-        'images': 'images',  # noqa: E501
-        'organization': 'organization',  # noqa: E501
-        'activation_webhook_url': 'activation_webhook_url',  # noqa: E501
-        'post_activation_redirect_uri': 'post_activation_redirect_uri',  # noqa: E501
-        'viewer_plugins_urls': 'viewer_plugins_urls',  # noqa: E501
-        'settings_url': 'settings_url',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'logo': 'logo',  # noqa: E501
-        'file': 'file',  # noqa: E501
+        'unit_type': 'unit_type',  # noqa: E501
+        'prefix': 'prefix',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'conversion_factor': 'conversion_factor',  # noqa: E501
+        'conversion_baseunit': 'conversion_baseunit',  # noqa: E501
+        'elements': 'elements',  # noqa: E501
+        'is_default': 'is_default',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
-        'creator',  # noqa: E501
-        'scopes',  # noqa: E501
-        'is_public',  # noqa: E501
-        'images',  # noqa: E501
-        'organization',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, short_description, long_description, creator, scopes, is_public, images, organization, *args, **kwargs):  # noqa: E501
-        """MarketplaceApp - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, type, *args, **kwargs):  # noqa: E501
+        """Unit - a model defined in OpenAPI
 
         Args:
             id (int):
-            name (str):
-            short_description (str):
-            long_description (str):
-            creator (bool, date, datetime, dict, float, int, list, str, none_type):
-            scopes ([str]):
-            is_public (bool):
-            images ([MarketplaceAppImage]):
-            organization (bool, date, datetime, dict, float, int, list, str, none_type):
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -203,21 +154,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            activation_webhook_url (str, none_type): [optional]  # noqa: E501
-            post_activation_redirect_uri (str, none_type): [optional]  # noqa: E501
-            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
-            settings_url (str, none_type): this URL will be called with query params ?cloud_id=. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            logo (str, none_type): [optional]  # noqa: E501
-            file (str, none_type): [optional]  # noqa: E501
+            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
+            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
+            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
+            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
+            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
+            conversion_baseunit (Unit): [optional]  # noqa: E501
+            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
+            is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,22 +190,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.name = name
-        self.short_description = short_description
-        self.long_description = long_description
-        self.creator = creator
-        self.scopes = scopes
-        self.is_public = is_public
-        self.images = images
-        self.organization = organization
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -266,20 +211,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, short_description, long_description, *args, **kwargs):  # noqa: E501
-        """MarketplaceApp - a model defined in OpenAPI
+    def __init__(self, type, *args, **kwargs):  # noqa: E501
+        """Unit - a model defined in OpenAPI
+
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
 
-            name (str):
-            short_description (str):
-            long_description (str):
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -303,21 +247,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            activation_webhook_url (str, none_type): [optional]  # noqa: E501
-            post_activation_redirect_uri (str, none_type): [optional]  # noqa: E501
-            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
-            settings_url (str, none_type): this URL will be called with query params ?cloud_id=. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            logo (str, none_type): [optional]  # noqa: E501
-            file (str, none_type): [optional]  # noqa: E501
+            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
+            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
+            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
+            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
+            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
+            conversion_baseunit (Unit): [optional]  # noqa: E501
+            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
+            is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -335,17 +280,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.short_description = short_description
-        self.long_description = long_description
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_image.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_image.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_image_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/storey_model_plan_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class MarketplaceAppImageRequest(ModelNormal):
+class StoreyModelPlanRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'image': (file_type,),  # noqa: E501
+            'id': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'image': 'image',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, image, *args, **kwargs):  # noqa: E501
-        """MarketplaceAppImageRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """StoreyModelPlanRequest - a model defined in OpenAPI
 
         Args:
-            image (file_type):
+            id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.image = image
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, image, *args, **kwargs):  # noqa: E501
-        """MarketplaceAppImageRequest - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """StoreyModelPlanRequest - a model defined in OpenAPI
 
         Args:
-            image (file_type):
+            id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.image = image
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/marketplace_app_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_unit_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from bimdata_api_client.model.unit_request import UnitRequest
+    globals()['UnitRequest'] = UnitRequest
 
-class MarketplaceAppRequest(ModelNormal):
+
+class PatchedUnitRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,106 +59,79 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 256,
-            'min_length': 1,
-        },
-        ('short_description',): {
-            'max_length': 130,
-            'min_length': 1,
-        },
-        ('long_description',): {
-            'min_length': 1,
-        },
-        ('activation_webhook_url',): {
-            'max_length': 1024,
-        },
-        ('post_activation_redirect_uri',): {
-            'max_length': 1024,
-        },
-        ('webhook_secret',): {
+        ('type',): {
             'min_length': 1,
         },
-        ('settings_url',): {
-            'max_length': 1024,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'short_description': (str,),  # noqa: E501
-            'long_description': (str,),  # noqa: E501
-            'activation_webhook_url': (str, none_type,),  # noqa: E501
-            'post_activation_redirect_uri': (str, none_type,),  # noqa: E501
-            'viewer_plugins_urls': ([str], none_type,),  # noqa: E501
-            'webhook_secret': (str,),  # noqa: E501
-            'settings_url': (str, none_type,),  # noqa: E501
-            'tags': ([str],),  # noqa: E501
-            'logo': (file_type, none_type,),  # noqa: E501
-            'file': (file_type, none_type,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'unit_type': (str, none_type,),  # noqa: E501
+            'prefix': (str, none_type,),  # noqa: E501
+            'dimensions': ([float], none_type,),  # noqa: E501
+            'conversion_factor': (float, none_type,),  # noqa: E501
+            'conversion_baseunit': (UnitRequest,),  # noqa: E501
+            'elements': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'is_default': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'type': 'type',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'short_description': 'short_description',  # noqa: E501
-        'long_description': 'long_description',  # noqa: E501
-        'activation_webhook_url': 'activation_webhook_url',  # noqa: E501
-        'post_activation_redirect_uri': 'post_activation_redirect_uri',  # noqa: E501
-        'viewer_plugins_urls': 'viewer_plugins_urls',  # noqa: E501
-        'webhook_secret': 'webhook_secret',  # noqa: E501
-        'settings_url': 'settings_url',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'logo': 'logo',  # noqa: E501
-        'file': 'file',  # noqa: E501
+        'unit_type': 'unit_type',  # noqa: E501
+        'prefix': 'prefix',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'conversion_factor': 'conversion_factor',  # noqa: E501
+        'conversion_baseunit': 'conversion_baseunit',  # noqa: E501
+        'elements': 'elements',  # noqa: E501
+        'is_default': 'is_default',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, short_description, long_description, *args, **kwargs):  # noqa: E501
-        """MarketplaceAppRequest - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            short_description (str):
-            long_description (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PatchedUnitRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -179,22 +156,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            activation_webhook_url (str, none_type): [optional]  # noqa: E501
-            post_activation_redirect_uri (str, none_type): [optional]  # noqa: E501
-            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
-            webhook_secret (str): [optional]  # noqa: E501
-            settings_url (str, none_type): this URL will be called with query params ?cloud_id=. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            logo (file_type, none_type): [optional]  # noqa: E501
-            file (file_type, none_type): [optional]  # noqa: E501
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit. [optional]  # noqa: E501
+            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
+            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
+            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
+            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
+            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
+            conversion_baseunit (UnitRequest): [optional]  # noqa: E501
+            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
+            is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,17 +192,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.short_description = short_description
-        self.long_description = long_description
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -237,21 +212,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, short_description, long_description, *args, **kwargs):  # noqa: E501
-        """MarketplaceAppRequest - a model defined in OpenAPI
-
-        Args:
-            name (str):
-            short_description (str):
-            long_description (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PatchedUnitRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -276,22 +246,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            activation_webhook_url (str, none_type): [optional]  # noqa: E501
-            post_activation_redirect_uri (str, none_type): [optional]  # noqa: E501
-            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
-            webhook_secret (str): [optional]  # noqa: E501
-            settings_url (str, none_type): this URL will be called with query params ?cloud_id=. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
-            logo (file_type, none_type): [optional]  # noqa: E501
-            file (file_type, none_type): [optional]  # noqa: E501
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit. [optional]  # noqa: E501
+            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
+            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
+            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
+            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
+            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
+            conversion_baseunit (UnitRequest): [optional]  # noqa: E501
+            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
+            is_default (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -309,17 +280,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.short_description = short_description
-        self.long_description = long_description
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/material.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/material.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/material_list_component.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/material_list_component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/material_list_component_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/material_list_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/material_option.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/material_option.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/material_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/material_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_errors.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_errors.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_errors_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_errors_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_files.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_files.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_property.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_property.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/model_with_positioning_plan.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/model_with_positioning_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/organization.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/organization.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/organization_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/organization_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/orthogonal_camera.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/orthogonal_camera.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/orthogonal_camera_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/orthogonal_camera_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_bcf_project_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_bcf_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_check_plan_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_check_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_checker_result_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_checker_result_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_classification_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_cloud_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_cloud_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_comment_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_document_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_document_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_element_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_folder_without_children_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_folder_without_children_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_full_topic_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_full_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_group_folder_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_group_folder_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_group_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ifc_access_token_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ifc_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ifc_checker_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ifc_checker_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_label_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_label_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_layer_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_model_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_positioning_plan_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_positioning_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_priority_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_priority_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_processor_handler_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_processor_handler_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_project_access_token_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_project_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_project_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_definition_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_property_set_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_rule_component_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_rule_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_rule_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_rule_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_ruleset_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_ruleset_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_space_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_stage_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_stage_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_storey_building_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_storey_building_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_system_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_system_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_tag_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_tag_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_status_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_status_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_topic_type_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_topic_type_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_unit_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/unit_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from bimdata_api_client.model.unit_request import UnitRequest
-    globals()['UnitRequest'] = UnitRequest
 
-
-class PatchedUnitRequest(ModelNormal):
+class UnitRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -70,30 +66,28 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'type': (str,),  # noqa: E501
             'name': (str, none_type,),  # noqa: E501
             'unit_type': (str, none_type,),  # noqa: E501
             'prefix': (str, none_type,),  # noqa: E501
             'dimensions': ([float], none_type,),  # noqa: E501
             'conversion_factor': (float, none_type,),  # noqa: E501
@@ -122,16 +116,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchedUnitRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
+        """UnitRequest - a model defined in OpenAPI
+
+        Args:
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -156,15 +153,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit. [optional]  # noqa: E501
             name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
             unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
             prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
             dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
             conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
             conversion_baseunit (UnitRequest): [optional]  # noqa: E501
             elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
@@ -192,14 +188,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -212,16 +209,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchedUnitRequest - a model defined in OpenAPI
+    def __init__(self, type, *args, **kwargs):  # noqa: E501
+        """UnitRequest - a model defined in OpenAPI
+
+        Args:
+            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -246,15 +246,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit. [optional]  # noqa: E501
             name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
             unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
             prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
             dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
             conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
             conversion_baseunit (UnitRequest): [optional]  # noqa: E501
             elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
@@ -280,14 +279,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_user_cloud_update_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_user_cloud_update_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_user_project_update_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_user_project_update_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_viewpoint_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_viewpoint_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_comment_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_visa_validation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_visa_validation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_web_hook_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_web_hook_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_zone_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_zone_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/patched_zone_space_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/patched_zone_space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/perspective_camera.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/perspective_camera.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/perspective_camera_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/perspective_camera_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/pin.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/pin.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/pin_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/pin_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/point.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/point.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/point_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/point_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/positioning_plan.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/positioning_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/priority.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/priority.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/priority_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/priority_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/processor_handler.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/processor_handler.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_access_token.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_access_token.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_access_token_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_folder_tree.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_folder_tree.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_invitation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_invitation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_invitation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_role.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_role.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_size.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_size.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/project_with_children.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/project_with_children.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/property_definition.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/property_definition.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/property_definition_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/property_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/property_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/property_set.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/property_set.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/property_set_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/public_organization.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/public_organization.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/public_organization_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/public_organization_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_classification.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_classification.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_classification_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_definition.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_definition.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_definition_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_element.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_element_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_elements.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_elements.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_elements_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_elements_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_layer.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_layer.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_layer_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_components.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_components.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_components_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_components_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_list_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_list_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_options.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_options.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_options_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_options_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_material_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_material_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_set.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_set.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_property_set_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_system.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_system.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_system_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_system_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_unit.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_unit.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/raw_unit_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/raw_unit_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/recursive_folder_children.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/recursive_folder_children.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from bimdata_api_client.model.document import Document
-    from bimdata_api_client.model.folder_group_permission import FolderGroupPermission
     from bimdata_api_client.model.tag import Tag
     from bimdata_api_client.model.user import User
-    globals()['Document'] = Document
-    globals()['FolderGroupPermission'] = FolderGroupPermission
     globals()['Tag'] = Tag
     globals()['User'] = User
 
 
 class RecursiveFolderChildren(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -135,18 +131,18 @@
             'nature': (str,),  # noqa: E501
             'model_type': (str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
             'model_id': (int, none_type,),  # noqa: E501
             'ifc_id': (int, none_type,),  # noqa: E501
-            'groups_permissions': ([FolderGroupPermission], none_type,),  # noqa: E501
+            'groups_permissions': (bool, none_type,),  # noqa: E501
             'default_permission': (int,),  # noqa: E501
             'user_permission': (int,),  # noqa: E501
-            'history': ([Document], none_type,),  # noqa: E501
+            'history_count': (int, none_type,),  # noqa: E501
             'tags': ([Tag], none_type,),  # noqa: E501
             'created_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'creator': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'file_name': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
             'size': (int, none_type,),  # noqa: E501
             'file': (str, none_type,),  # noqa: E501
@@ -168,15 +164,15 @@
         'created_at': 'created_at',  # noqa: E501
         'updated_at': 'updated_at',  # noqa: E501
         'model_id': 'model_id',  # noqa: E501
         'ifc_id': 'ifc_id',  # noqa: E501
         'groups_permissions': 'groups_permissions',  # noqa: E501
         'default_permission': 'default_permission',  # noqa: E501
         'user_permission': 'user_permission',  # noqa: E501
-        'history': 'history',  # noqa: E501
+        'history_count': 'history_count',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'creator': 'creator',  # noqa: E501
         'file_name': 'file_name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'size': 'size',  # noqa: E501
         'file': 'file',  # noqa: E501
@@ -189,40 +185,40 @@
         'nature',  # noqa: E501
         'model_type',  # noqa: E501
         'model_id',  # noqa: E501
         'ifc_id',  # noqa: E501
         'groups_permissions',  # noqa: E501
         'default_permission',  # noqa: E501
         'user_permission',  # noqa: E501
-        'history',  # noqa: E501
+        'history_count',  # noqa: E501
         'tags',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, parent_id, type, nature, model_type, name, created_at, updated_at, model_id, ifc_id, groups_permissions, default_permission, user_permission, history, tags, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, parent_id, type, nature, model_type, name, created_at, updated_at, model_id, ifc_id, groups_permissions, default_permission, user_permission, history_count, tags, *args, **kwargs):  # noqa: E501
         """RecursiveFolderChildren - a model defined in OpenAPI
 
         Args:
             id (int):
             parent_id (int, none_type):
             type (str): DEPRECATED: Use 'nature' instead. Values can be 'Folder', 'Document' or 'Ifc'. It is usefull to parse the tree and discriminate folders and files
             nature (str): Values can be 'Folder', 'Document' or 'Model'. It is usefull to parse the tree and discriminate folders and files
             model_type (str, none_type): Model's type. Values can be IFC, DWG, DXF, GLTF, PDF, JPEG, PNG, OBJ, DAE, BFX, POINT_CLOUD
             name (str):
             created_at (datetime):
             updated_at (datetime):
             model_id (int, none_type):
             ifc_id (int, none_type): DEPRECATED: Use 'model_id' instead
-            groups_permissions ([FolderGroupPermission], none_type): Groups permissions of folder
+            groups_permissions (bool, none_type): DEPRECATED: This field must be present because of legacy constraints but will always be empty. If you want to see group permissions of a folder, see `getFolder`
             default_permission (int): Default permissions of folder
             user_permission (int): Aggregate of group user permissions and folder default permission
-            history ([Document], none_type): History of a document
+            history_count (int, none_type): Number of previous versions
             tags ([Tag], none_type): Tags of a document
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -295,15 +291,15 @@
         self.created_at = created_at
         self.updated_at = updated_at
         self.model_id = model_id
         self.ifc_id = ifc_id
         self.groups_permissions = groups_permissions
         self.default_permission = default_permission
         self.user_permission = user_permission
-        self.history = history
+        self.history_count = history_count
         self.tags = tags
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/rule.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/rule.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/rule_component.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/rule_component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/rule_component_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/rule_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/rule_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/rule_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ruleset.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ruleset.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/ruleset_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/ruleset_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/self_bcf_user.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/self_bcf_user.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/self_user.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/self_user.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/simple_element.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/simple_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/size.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/size.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/snapshot.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/snapshot.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/snapshot_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/snapshot_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/space.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/space.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/space_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/stage.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/stage.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/stage_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/stage_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/storey.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/storey.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/storey_building_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/storey_building_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/storey_model_plan_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/tag_id_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class StoreyModelPlanRequest(ModelNormal):
+class TagIdRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
+            'tag_id': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'tag_id': 'tag_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """StoreyModelPlanRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, tag_id, *args, **kwargs):  # noqa: E501
+        """TagIdRequest - a model defined in OpenAPI
 
         Args:
-            id (int):
+            tag_id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.tag_id = tag_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """StoreyModelPlanRequest - a model defined in OpenAPI
+    def __init__(self, tag_id, *args, **kwargs):  # noqa: E501
+        """TagIdRequest - a model defined in OpenAPI
 
         Args:
-            id (int):
+            tag_id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.tag_id = tag_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/system.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/system.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/system_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/system_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/tag.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/tag.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/tag_id_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic_type_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class TagIdRequest(ModelNormal):
+class TopicTypeRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,14 +55,18 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('topic_type',): {
+            'max_length': 255,
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -78,38 +82,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'tag_id': (int,),  # noqa: E501
+            'topic_type': (str,),  # noqa: E501
+            'project': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tag_id': 'tag_id',  # noqa: E501
+        'topic_type': 'topic_type',  # noqa: E501
+        'project': 'project',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, tag_id, *args, **kwargs):  # noqa: E501
-        """TagIdRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, topic_type, *args, **kwargs):  # noqa: E501
+        """TopicTypeRequest - a model defined in OpenAPI
 
         Args:
-            tag_id (int):
+            topic_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,14 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            project (int): This field is automatically provided by the route, you don't need to provide it in the body. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,15 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tag_id = tag_id
+        self.topic_type = topic_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, tag_id, *args, **kwargs):  # noqa: E501
-        """TagIdRequest - a model defined in OpenAPI
+    def __init__(self, topic_type, *args, **kwargs):  # noqa: E501
+        """TopicTypeRequest - a model defined in OpenAPI
 
         Args:
-            tag_id (int):
+            topic_type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,14 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            project (int): This field is automatically provided by the route, you don't need to provide it in the body. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tag_id = tag_id
+        self.topic_type = topic_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/tag_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/tag_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic_status.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic_status.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic_status_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic_status_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic_type.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/topic_type.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/topic_type_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa_comment_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class TopicTypeRequest(ModelNormal):
+class VisaCommentRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,18 +55,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('topic_type',): {
-            'max_length': 255,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -82,40 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'topic_type': (str,),  # noqa: E501
-            'project': (int,),  # noqa: E501
+            'author_id': (int,),  # noqa: E501
+            'content': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'topic_type': 'topic_type',  # noqa: E501
-        'project': 'project',  # noqa: E501
+        'author_id': 'author_id',  # noqa: E501
+        'content': 'content',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, topic_type, *args, **kwargs):  # noqa: E501
-        """TopicTypeRequest - a model defined in OpenAPI
-
-        Args:
-            topic_type (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """VisaCommentRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            project (int): This field is automatically provided by the route, you don't need to provide it in the body. [optional]  # noqa: E501
+            author_id (int): This is the userproject_id. This field is only used if the call is made from an App. [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.topic_type = topic_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, topic_type, *args, **kwargs):  # noqa: E501
-        """TopicTypeRequest - a model defined in OpenAPI
-
-        Args:
-            topic_type (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """VisaCommentRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            project (int): This field is automatically provided by the route, you don't need to provide it in the body. [optional]  # noqa: E501
+            author_id (int): This is the userproject_id. This field is only used if the call is made from an App. [optional]  # noqa: E501
+            content (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -252,15 +243,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.topic_type = topic_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/unit.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_light.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from bimdata_api_client.model.marketplace_app_image import MarketplaceAppImage
+    from bimdata_api_client.model.public_organization import PublicOrganization
+    globals()['MarketplaceAppImage'] = MarketplaceAppImage
+    globals()['PublicOrganization'] = PublicOrganization
 
-class Unit(ModelNormal):
+
+class MarketplaceAppLight(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,81 +61,82 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'max_length': 256,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'id': (int,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
-            'unit_type': (str, none_type,),  # noqa: E501
-            'prefix': (str, none_type,),  # noqa: E501
-            'dimensions': ([float], none_type,),  # noqa: E501
-            'conversion_factor': (float, none_type,),  # noqa: E501
-            'conversion_baseunit': (Unit,),  # noqa: E501
-            'elements': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'is_default': (bool,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'organization': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'images': ([MarketplaceAppImage],),  # noqa: E501
+            'viewer_plugins_urls': ([str], none_type,),  # noqa: E501
+            'file': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'unit_type': 'unit_type',  # noqa: E501
-        'prefix': 'prefix',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
-        'conversion_factor': 'conversion_factor',  # noqa: E501
-        'conversion_baseunit': 'conversion_baseunit',  # noqa: E501
-        'elements': 'elements',  # noqa: E501
-        'is_default': 'is_default',  # noqa: E501
+        'organization': 'organization',  # noqa: E501
+        'images': 'images',  # noqa: E501
+        'viewer_plugins_urls': 'viewer_plugins_urls',  # noqa: E501
+        'file': 'file',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
+        'organization',  # noqa: E501
+        'images',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, type, *args, **kwargs):  # noqa: E501
-        """Unit - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, organization, images, *args, **kwargs):  # noqa: E501
+        """MarketplaceAppLight - a model defined in OpenAPI
 
         Args:
             id (int):
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
+            name (str):
+            organization (bool, date, datetime, dict, float, int, list, str, none_type):
+            images ([MarketplaceAppImage]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,22 +161,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
-            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
-            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
-            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
-            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
-            conversion_baseunit (Unit): [optional]  # noqa: E501
-            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
+            file (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +191,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.type = type
+        self.name = name
+        self.organization = organization
+        self.images = images
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -211,19 +214,18 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """Unit - a model defined in OpenAPI
-
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """MarketplaceAppLight - a model defined in OpenAPI
 
+            name (str):
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -247,22 +249,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
-            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
-            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
-            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
-            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
-            conversion_baseunit (Unit): [optional]  # noqa: E501
-            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
+            file (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -280,15 +276,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/unit_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/viewpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,32 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from bimdata_api_client.model.clipping_plane import ClippingPlane
+    from bimdata_api_client.model.components_parent import ComponentsParent
+    from bimdata_api_client.model.line import Line
+    from bimdata_api_client.model.orthogonal_camera import OrthogonalCamera
+    from bimdata_api_client.model.perspective_camera import PerspectiveCamera
+    from bimdata_api_client.model.pin import Pin
+    from bimdata_api_client.model.snapshot import Snapshot
+    globals()['ClippingPlane'] = ClippingPlane
+    globals()['ComponentsParent'] = ComponentsParent
+    globals()['Line'] = Line
+    globals()['OrthogonalCamera'] = OrthogonalCamera
+    globals()['PerspectiveCamera'] = PerspectiveCamera
+    globals()['Pin'] = Pin
+    globals()['Snapshot'] = Snapshot
 
-class UnitRequest(ModelNormal):
+
+class Viewpoint(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,80 +71,90 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('type',): {
-            'min_length': 1,
+        ('index',): {
+            'inclusive_maximum': 2147483647,
+            'inclusive_minimum': 0,
+        },
+        ('originating_system',): {
+            'max_length': 256,
+        },
+        ('authoring_tool_id',): {
+            'max_length': 256,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
-            'unit_type': (str, none_type,),  # noqa: E501
-            'prefix': (str, none_type,),  # noqa: E501
-            'dimensions': ([float], none_type,),  # noqa: E501
-            'conversion_factor': (float, none_type,),  # noqa: E501
-            'conversion_baseunit': (UnitRequest,),  # noqa: E501
-            'elements': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'is_default': (bool,),  # noqa: E501
+            'index': (int, none_type,),  # noqa: E501
+            'guid': (str,),  # noqa: E501
+            'originating_system': (str, none_type,),  # noqa: E501
+            'authoring_tool_id': (str, none_type,),  # noqa: E501
+            'orthogonal_camera': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'perspective_camera': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'lines': ([Line], none_type,),  # noqa: E501
+            'clipping_planes': ([ClippingPlane], none_type,),  # noqa: E501
+            'snapshot': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'components': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'pins': ([Pin], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'unit_type': 'unit_type',  # noqa: E501
-        'prefix': 'prefix',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
-        'conversion_factor': 'conversion_factor',  # noqa: E501
-        'conversion_baseunit': 'conversion_baseunit',  # noqa: E501
-        'elements': 'elements',  # noqa: E501
-        'is_default': 'is_default',  # noqa: E501
+        'index': 'index',  # noqa: E501
+        'guid': 'guid',  # noqa: E501
+        'originating_system': 'originating_system',  # noqa: E501
+        'authoring_tool_id': 'authoring_tool_id',  # noqa: E501
+        'orthogonal_camera': 'orthogonal_camera',  # noqa: E501
+        'perspective_camera': 'perspective_camera',  # noqa: E501
+        'lines': 'lines',  # noqa: E501
+        'clipping_planes': 'clipping_planes',  # noqa: E501
+        'snapshot': 'snapshot',  # noqa: E501
+        'components': 'components',  # noqa: E501
+        'pins': 'pins',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """UnitRequest - a model defined in OpenAPI
-
-        Args:
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Viewpoint - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,22 +179,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
-            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
-            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
-            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
-            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
-            conversion_baseunit (UnitRequest): [optional]  # noqa: E501
-            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            index (int, none_type): [optional]  # noqa: E501
+            guid (str): [optional]  # noqa: E501
+            originating_system (str, none_type): Name of the system in which the viewpoint is originated. [optional]  # noqa: E501
+            authoring_tool_id (str, none_type): System specific identifier of the viewpoint in the originating BIM tool. [optional]  # noqa: E501
+            orthogonal_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            perspective_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            lines ([Line], none_type): [optional]  # noqa: E501
+            clipping_planes ([ClippingPlane], none_type): [optional]  # noqa: E501
+            snapshot (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            components (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            pins ([Pin], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +217,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -209,19 +237,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """UnitRequest - a model defined in OpenAPI
-
-        Args:
-            type (str): IfcDerivedUnit, IfcContextDependentUnit, IfcConversionBasedUnit, IfcSIUnit or IfcMonetaryUnit
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Viewpoint - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -246,22 +271,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): Name of the unit (ex: DEGREE). [optional]  # noqa: E501
-            unit_type (str, none_type): IFC type of the unit or user defined type (ex: PLANEANGLEUNIT for DEGREE and RADIAN). [optional]  # noqa: E501
-            prefix (str, none_type): Litteral prefix for scale (ex: MILLI, KILO, etc..). [optional]  # noqa: E501
-            dimensions ([float], none_type): List of 7 units dimensions. [optional]  # noqa: E501
-            conversion_factor (float, none_type): Factor of conversion and base unit id (ex: DEGREE from RADIAN with factor 0.0174532925199433). [optional]  # noqa: E501
-            conversion_baseunit (UnitRequest): [optional]  # noqa: E501
-            elements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): List of constitutive unit elements by id with corresponding exponent (ex: [meterID/1, secondID/-1] for velocity). [optional]  # noqa: E501
-            is_default (bool): [optional]  # noqa: E501
+            index (int, none_type): [optional]  # noqa: E501
+            guid (str): [optional]  # noqa: E501
+            originating_system (str, none_type): Name of the system in which the viewpoint is originated. [optional]  # noqa: E501
+            authoring_tool_id (str, none_type): System specific identifier of the viewpoint in the originating BIM tool. [optional]  # noqa: E501
+            orthogonal_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            perspective_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            lines ([Line], none_type): [optional]  # noqa: E501
+            clipping_planes ([ClippingPlane], none_type): [optional]  # noqa: E501
+            snapshot (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            components (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            pins ([Pin], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -279,15 +307,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/user.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/user.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/user_invitation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/user_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/user_project.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/user_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/user_project_id_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/user_project_id_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/view_setup_hints.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/view_setup_hints.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/view_setup_hints_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/view_setup_hints_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/viewpoint.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/viewpoint_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,31 +27,31 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from bimdata_api_client.model.clipping_plane import ClippingPlane
-    from bimdata_api_client.model.components_parent import ComponentsParent
-    from bimdata_api_client.model.line import Line
-    from bimdata_api_client.model.orthogonal_camera import OrthogonalCamera
-    from bimdata_api_client.model.perspective_camera import PerspectiveCamera
-    from bimdata_api_client.model.pin import Pin
-    from bimdata_api_client.model.snapshot import Snapshot
-    globals()['ClippingPlane'] = ClippingPlane
-    globals()['ComponentsParent'] = ComponentsParent
-    globals()['Line'] = Line
-    globals()['OrthogonalCamera'] = OrthogonalCamera
-    globals()['PerspectiveCamera'] = PerspectiveCamera
-    globals()['Pin'] = Pin
-    globals()['Snapshot'] = Snapshot
+    from bimdata_api_client.model.clipping_plane_request import ClippingPlaneRequest
+    from bimdata_api_client.model.components_parent_request import ComponentsParentRequest
+    from bimdata_api_client.model.line_request import LineRequest
+    from bimdata_api_client.model.orthogonal_camera_request import OrthogonalCameraRequest
+    from bimdata_api_client.model.perspective_camera_request import PerspectiveCameraRequest
+    from bimdata_api_client.model.pin_request import PinRequest
+    from bimdata_api_client.model.snapshot_request import SnapshotRequest
+    globals()['ClippingPlaneRequest'] = ClippingPlaneRequest
+    globals()['ComponentsParentRequest'] = ComponentsParentRequest
+    globals()['LineRequest'] = LineRequest
+    globals()['OrthogonalCameraRequest'] = OrthogonalCameraRequest
+    globals()['PerspectiveCameraRequest'] = PerspectiveCameraRequest
+    globals()['PinRequest'] = PinRequest
+    globals()['SnapshotRequest'] = SnapshotRequest
 
 
-class Viewpoint(ModelNormal):
+class ViewpointRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -112,19 +112,20 @@
         return {
             'index': (int, none_type,),  # noqa: E501
             'guid': (str,),  # noqa: E501
             'originating_system': (str, none_type,),  # noqa: E501
             'authoring_tool_id': (str, none_type,),  # noqa: E501
             'orthogonal_camera': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'perspective_camera': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'lines': ([Line], none_type,),  # noqa: E501
-            'clipping_planes': ([ClippingPlane], none_type,),  # noqa: E501
+            'lines': ([LineRequest], none_type,),  # noqa: E501
+            'clipping_planes': ([ClippingPlaneRequest], none_type,),  # noqa: E501
             'snapshot': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'components': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'pins': ([Pin], none_type,),  # noqa: E501
+            'pins': ([PinRequest], none_type,),  # noqa: E501
+            'temp_id': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -136,25 +137,26 @@
         'orthogonal_camera': 'orthogonal_camera',  # noqa: E501
         'perspective_camera': 'perspective_camera',  # noqa: E501
         'lines': 'lines',  # noqa: E501
         'clipping_planes': 'clipping_planes',  # noqa: E501
         'snapshot': 'snapshot',  # noqa: E501
         'components': 'components',  # noqa: E501
         'pins': 'pins',  # noqa: E501
+        'temp_id': 'temp_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Viewpoint - a model defined in OpenAPI
+        """ViewpointRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -185,19 +187,20 @@
                                 _visited_composed_classes = (Animal,)
             index (int, none_type): [optional]  # noqa: E501
             guid (str): [optional]  # noqa: E501
             originating_system (str, none_type): Name of the system in which the viewpoint is originated. [optional]  # noqa: E501
             authoring_tool_id (str, none_type): System specific identifier of the viewpoint in the originating BIM tool. [optional]  # noqa: E501
             orthogonal_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             perspective_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            lines ([Line], none_type): [optional]  # noqa: E501
-            clipping_planes ([ClippingPlane], none_type): [optional]  # noqa: E501
+            lines ([LineRequest], none_type): [optional]  # noqa: E501
+            clipping_planes ([ClippingPlaneRequest], none_type): [optional]  # noqa: E501
             snapshot (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             components (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            pins ([Pin], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
+            pins ([PinRequest], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
+            temp_id (int, none_type): Only used when using POST on the full-topic route to bind viewpoint with comment. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,15 +241,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Viewpoint - a model defined in OpenAPI
+        """ViewpointRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -277,19 +280,20 @@
                                 _visited_composed_classes = (Animal,)
             index (int, none_type): [optional]  # noqa: E501
             guid (str): [optional]  # noqa: E501
             originating_system (str, none_type): Name of the system in which the viewpoint is originated. [optional]  # noqa: E501
             authoring_tool_id (str, none_type): System specific identifier of the viewpoint in the originating BIM tool. [optional]  # noqa: E501
             orthogonal_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             perspective_camera (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            lines ([Line], none_type): [optional]  # noqa: E501
-            clipping_planes ([ClippingPlane], none_type): [optional]  # noqa: E501
+            lines ([LineRequest], none_type): [optional]  # noqa: E501
+            clipping_planes ([ClippingPlaneRequest], none_type): [optional]  # noqa: E501
             snapshot (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             components (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            pins ([Pin], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
+            pins ([PinRequest], none_type): Non standard field. Pins (or markers/annotations) are points of interest. [optional]  # noqa: E501
+            temp_id (int, none_type): Only used when using POST on the full-topic route to bind viewpoint with comment. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa_comment.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa_comment.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa_comment_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/zone_space_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class VisaCommentRequest(ModelNormal):
+class ZoneSpaceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,14 +55,24 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('uuid',): {
+            'max_length': 512,
+            'min_length': 1,
+        },
+        ('name',): {
+            'max_length': 255,
+        },
+        ('longname',): {
+            'max_length': 255,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -78,37 +88,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'author_id': (int,),  # noqa: E501
-            'content': (str,),  # noqa: E501
+            'uuid': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'longname': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'author_id': 'author_id',  # noqa: E501
-        'content': 'content',  # noqa: E501
+        'uuid': 'uuid',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'longname': 'longname',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VisaCommentRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, uuid, *args, **kwargs):  # noqa: E501
+        """ZoneSpaceRequest - a model defined in OpenAPI
+
+        Args:
+            uuid (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +148,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            author_id (int): This is the userproject_id. This field is only used if the call is made from an App. [optional]  # noqa: E501
-            content (str): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            longname (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -162,14 +177,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.uuid = uuid
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,16 +198,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """VisaCommentRequest - a model defined in OpenAPI
+    def __init__(self, uuid, *args, **kwargs):  # noqa: E501
+        """ZoneSpaceRequest - a model defined in OpenAPI
+
+        Args:
+            uuid (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +235,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            author_id (int): This is the userproject_id. This field is only used if the call is made from an App. [optional]  # noqa: E501
-            content (str): [optional]  # noqa: E501
+            name (str, none_type): [optional]  # noqa: E501
+            longname (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -243,14 +262,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.uuid = uuid
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa_validation.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa_validation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visa_validation_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visa_validation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visibility.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visibility.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/visibility_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/visibility_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/web_hook.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/web_hook.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/web_hook_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/web_hook_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/write_folder_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/write_folder_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/zone.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/zone.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/zone_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/zone_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/zone_space.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/zone_space.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model/zone_space_request.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model/marketplace_app_light_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from bimdata_api_client.exceptions import ApiAttributeError
 
 
 
-class ZoneSpaceRequest(ModelNormal):
+class MarketplaceAppLightRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,23 +55,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('uuid',): {
-            'max_length': 512,
-            'min_length': 1,
-        },
         ('name',): {
-            'max_length': 255,
-        },
-        ('longname',): {
-            'max_length': 255,
+            'max_length': 256,
+            'min_length': 1,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -88,42 +82,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'uuid': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
-            'longname': (str, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'viewer_plugins_urls': ([str], none_type,),  # noqa: E501
+            'file': (file_type, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uuid': 'uuid',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'longname': 'longname',  # noqa: E501
+        'viewer_plugins_urls': 'viewer_plugins_urls',  # noqa: E501
+        'file': 'file',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, uuid, *args, **kwargs):  # noqa: E501
-        """ZoneSpaceRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """MarketplaceAppLightRequest - a model defined in OpenAPI
 
         Args:
-            uuid (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -148,16 +142,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            longname (str, none_type): [optional]  # noqa: E501
+            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
+            file (file_type, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.uuid = uuid
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, uuid, *args, **kwargs):  # noqa: E501
-        """ZoneSpaceRequest - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """MarketplaceAppLightRequest - a model defined in OpenAPI
 
         Args:
-            uuid (str):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,16 +229,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str, none_type): [optional]  # noqa: E501
-            longname (str, none_type): [optional]  # noqa: E501
+            viewer_plugins_urls ([str], none_type): [optional]  # noqa: E501
+            file (file_type, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -262,15 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.uuid = uuid
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/model_utils.py` & `bimdata-api-client-9.9.0/bimdata_api_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/models/__init__.py` & `bimdata-api-client-9.9.0/bimdata_api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,18 +76,17 @@
 from bimdata_api_client.model.label_request import LabelRequest
 from bimdata_api_client.model.layer import Layer
 from bimdata_api_client.model.layer_element import LayerElement
 from bimdata_api_client.model.layer_element_request import LayerElementRequest
 from bimdata_api_client.model.layer_request import LayerRequest
 from bimdata_api_client.model.line import Line
 from bimdata_api_client.model.line_request import LineRequest
-from bimdata_api_client.model.marketplace_app import MarketplaceApp
 from bimdata_api_client.model.marketplace_app_image import MarketplaceAppImage
-from bimdata_api_client.model.marketplace_app_image_request import MarketplaceAppImageRequest
-from bimdata_api_client.model.marketplace_app_request import MarketplaceAppRequest
+from bimdata_api_client.model.marketplace_app_light import MarketplaceAppLight
+from bimdata_api_client.model.marketplace_app_light_request import MarketplaceAppLightRequest
 from bimdata_api_client.model.material import Material
 from bimdata_api_client.model.material_list_component import MaterialListComponent
 from bimdata_api_client.model.material_list_component_request import MaterialListComponentRequest
 from bimdata_api_client.model.material_option import MaterialOption
 from bimdata_api_client.model.material_request import MaterialRequest
 from bimdata_api_client.model.model import Model
 from bimdata_api_client.model.model_errors import ModelErrors
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client/rest.py` & `bimdata-api-client-9.9.0/bimdata_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client.egg-info/PKG-INFO` & `bimdata-api-client-9.9.0/bimdata_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimdata-api-client
-Version: 9.8.1
+Version: 9.9.0
 Summary: BIMData API
 Home-page: https://github.com/bimdata/python-api-client
 Author: BIMData.io
 Author-email: contact@bimdata.io
 License: UNKNOWN
 Keywords: Swagger,BIMData API
 Platform: UNKNOWN
@@ -741,18 +741,17 @@
  - [LabelRequest](docs/LabelRequest.md)
  - [Layer](docs/Layer.md)
  - [LayerElement](docs/LayerElement.md)
  - [LayerElementRequest](docs/LayerElementRequest.md)
  - [LayerRequest](docs/LayerRequest.md)
  - [Line](docs/Line.md)
  - [LineRequest](docs/LineRequest.md)
- - [MarketplaceApp](docs/MarketplaceApp.md)
  - [MarketplaceAppImage](docs/MarketplaceAppImage.md)
- - [MarketplaceAppImageRequest](docs/MarketplaceAppImageRequest.md)
- - [MarketplaceAppRequest](docs/MarketplaceAppRequest.md)
+ - [MarketplaceAppLight](docs/MarketplaceAppLight.md)
+ - [MarketplaceAppLightRequest](docs/MarketplaceAppLightRequest.md)
  - [Material](docs/Material.md)
  - [MaterialListComponent](docs/MaterialListComponent.md)
  - [MaterialListComponentRequest](docs/MaterialListComponentRequest.md)
  - [MaterialOption](docs/MaterialOption.md)
  - [MaterialRequest](docs/MaterialRequest.md)
  - [Model](docs/Model.md)
  - [ModelErrors](docs/ModelErrors.md)
```

### Comparing `bimdata-api-client-9.8.1/bimdata_api_client.egg-info/SOURCES.txt` & `bimdata-api-client-9.9.0/bimdata_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,17 @@
 bimdata_api_client/model/label_request.py
 bimdata_api_client/model/layer.py
 bimdata_api_client/model/layer_element.py
 bimdata_api_client/model/layer_element_request.py
 bimdata_api_client/model/layer_request.py
 bimdata_api_client/model/line.py
 bimdata_api_client/model/line_request.py
-bimdata_api_client/model/marketplace_app.py
 bimdata_api_client/model/marketplace_app_image.py
-bimdata_api_client/model/marketplace_app_image_request.py
-bimdata_api_client/model/marketplace_app_request.py
+bimdata_api_client/model/marketplace_app_light.py
+bimdata_api_client/model/marketplace_app_light_request.py
 bimdata_api_client/model/material.py
 bimdata_api_client/model/material_list_component.py
 bimdata_api_client/model/material_list_component_request.py
 bimdata_api_client/model/material_option.py
 bimdata_api_client/model/material_request.py
 bimdata_api_client/model/model.py
 bimdata_api_client/model/model_errors.py
@@ -341,18 +340,17 @@
 test/test_label_request.py
 test/test_layer.py
 test/test_layer_element.py
 test/test_layer_element_request.py
 test/test_layer_request.py
 test/test_line.py
 test/test_line_request.py
-test/test_marketplace_app.py
 test/test_marketplace_app_image.py
-test/test_marketplace_app_image_request.py
-test/test_marketplace_app_request.py
+test/test_marketplace_app_light.py
+test/test_marketplace_app_light_request.py
 test/test_material.py
 test/test_material_list_component.py
 test/test_material_list_component_request.py
 test/test_material_option.py
 test/test_material_request.py
 test/test_model.py
 test/test_model_api.py
```

### Comparing `bimdata-api-client-9.8.1/setup.py` & `bimdata-api-client-9.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from io import open
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 NAME = "bimdata-api-client"
-VERSION = "9.8.1"
+VERSION = "9.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `bimdata-api-client-9.8.1/test/test_bcf_api.py` & `bimdata-api-client-9.9.0/test/test_bcf_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_bcf_project.py` & `bimdata-api-client-9.9.0/test/test_bcf_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_bcf_project_request.py` & `bimdata-api-client-9.9.0/test/test_bcf_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_building.py` & `bimdata-api-client-9.9.0/test/test_building.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_building_model_plan_request.py` & `bimdata-api-client-9.9.0/test/test_building_model_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_check_plan.py` & `bimdata-api-client-9.9.0/test/test_check_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_check_plan_request.py` & `bimdata-api-client-9.9.0/test/test_check_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_check_project_access.py` & `bimdata-api-client-9.9.0/test/test_check_project_access.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_checker_api.py` & `bimdata-api-client-9.9.0/test/test_checker_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_checker_result.py` & `bimdata-api-client-9.9.0/test/test_checker_result.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_checker_result_request.py` & `bimdata-api-client-9.9.0/test/test_checker_result_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_classification.py` & `bimdata-api-client-9.9.0/test/test_classification.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_classification_request.py` & `bimdata-api-client-9.9.0/test/test_classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_clipping_plane.py` & `bimdata-api-client-9.9.0/test/test_clipping_plane.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_clipping_plane_request.py` & `bimdata-api-client-9.9.0/test/test_clipping_plane_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_cloud.py` & `bimdata-api-client-9.9.0/test/test_self_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,36 +9,34 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.feature import Feature
-from bimdata_api_client.model.marketplace_app import MarketplaceApp
+from bimdata_api_client.model.cloud_role import CloudRole
 from bimdata_api_client.model.organization import Organization
-from bimdata_api_client.model.user import User
-globals()['Feature'] = Feature
-globals()['MarketplaceApp'] = MarketplaceApp
+from bimdata_api_client.model.project_role import ProjectRole
+globals()['CloudRole'] = CloudRole
 globals()['Organization'] = Organization
-globals()['User'] = User
-from bimdata_api_client.model.cloud import Cloud
+globals()['ProjectRole'] = ProjectRole
+from bimdata_api_client.model.self_user import SelfUser
 
 
-class TestCloud(unittest.TestCase):
-    """Cloud unit test stubs"""
+class TestSelfUser(unittest.TestCase):
+    """SelfUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCloud(self):
-        """Test Cloud"""
+    def testSelfUser(self):
+        """Test SelfUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Cloud()  # noqa: E501
+        # model = SelfUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_cloud_invitation.py` & `bimdata-api-client-9.9.0/test/test_cloud_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_cloud_invitation_request.py` & `bimdata-api-client-9.9.0/test/test_cloud_invitation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_cloud_request.py` & `bimdata-api-client-9.9.0/test/test_cloud_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_cloud_role.py` & `bimdata-api-client-9.9.0/test/test_cloud_role.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_collaboration_api.py` & `bimdata-api-client-9.9.0/test/test_collaboration_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_coloring.py` & `bimdata-api-client-9.9.0/test/test_coloring.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_coloring_request.py` & `bimdata-api-client-9.9.0/test/test_coloring_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_comment.py` & `bimdata-api-client-9.9.0/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_comment_request.py` & `bimdata-api-client-9.9.0/test/test_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_component.py` & `bimdata-api-client-9.9.0/test/test_component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_component_request.py` & `bimdata-api-client-9.9.0/test/test_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_components_parent.py` & `bimdata-api-client-9.9.0/test/test_components_parent.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_components_parent_request.py` & `bimdata-api-client-9.9.0/test/test_components_parent_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_create_building_by_name_request.py` & `bimdata-api-client-9.9.0/test/test_create_building_by_name_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_create_model_request.py` & `bimdata-api-client-9.9.0/test/test_create_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_create_multi_page_model_request.py` & `bimdata-api-client-9.9.0/test/test_create_multi_page_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_detailed_extensions.py` & `bimdata-api-client-9.9.0/test/test_detailed_extensions.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_direction.py` & `bimdata-api-client-9.9.0/test/test_direction.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_direction_request.py` & `bimdata-api-client-9.9.0/test/test_direction_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_document.py` & `bimdata-api-client-9.9.0/test/test_document.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_document_with_element_list.py` & `bimdata-api-client-9.9.0/test/test_document_with_element_list.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_element.py` & `bimdata-api-client-9.9.0/test/test_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_element_classification_relation.py` & `bimdata-api-client-9.9.0/test/test_element_classification_relation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_element_classification_relation_request.py` & `bimdata-api-client-9.9.0/test/test_element_classification_relation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_element_property_set_relation_request.py` & `bimdata-api-client-9.9.0/test/test_element_property_set_relation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_element_request.py` & `bimdata-api-client-9.9.0/test/test_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_extensions.py` & `bimdata-api-client-9.9.0/test/test_extensions.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_feature.py` & `bimdata-api-client-9.9.0/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_feature_request.py` & `bimdata-api-client-9.9.0/test/test_feature_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder.py` & `bimdata-api-client-9.9.0/test/test_folder.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_group_permission.py` & `bimdata-api-client-9.9.0/test/test_folder_group_permission.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_group_permission_request.py` & `bimdata-api-client-9.9.0/test/test_folder_group_permission_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_tree.py` & `bimdata-api-client-9.9.0/test/test_folder_tree.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_user_project.py` & `bimdata-api-client-9.9.0/test/test_folder_user_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_without_children.py` & `bimdata-api-client-9.9.0/test/test_folder_without_children.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_folder_without_children_request.py` & `bimdata-api-client-9.9.0/test/test_folder_without_children_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_full_topic.py` & `bimdata-api-client-9.9.0/test/test_full_topic.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_full_topic_request.py` & `bimdata-api-client-9.9.0/test/test_full_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_group.py` & `bimdata-api-client-9.9.0/test/test_group.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_group_folder.py` & `bimdata-api-client-9.9.0/test/test_group_folder.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_group_request.py` & `bimdata-api-client-9.9.0/test/test_group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_access_token.py` & `bimdata-api-client-9.9.0/test/test_ifc_access_token.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_access_token_request.py` & `bimdata-api-client-9.9.0/test/test_ifc_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_api.py` & `bimdata-api-client-9.9.0/test/test_ifc_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_checker.py` & `bimdata-api-client-9.9.0/test/test_ifc_checker.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_checker_request.py` & `bimdata-api-client-9.9.0/test/test_ifc_checker_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_export_request.py` & `bimdata-api-client-9.9.0/test/test_ifc_export_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_merge_request.py` & `bimdata-api-client-9.9.0/test/test_ifc_merge_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ifc_optimize_request.py` & `bimdata-api-client-9.9.0/test/test_ifc_optimize_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_import_group_request.py` & `bimdata-api-client-9.9.0/test/test_import_group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_invitation.py` & `bimdata-api-client-9.9.0/test/test_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_label.py` & `bimdata-api-client-9.9.0/test/test_label.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_label_request.py` & `bimdata-api-client-9.9.0/test/test_label_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_layer.py` & `bimdata-api-client-9.9.0/test/test_layer.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_layer_element.py` & `bimdata-api-client-9.9.0/test/test_layer_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_layer_element_request.py` & `bimdata-api-client-9.9.0/test/test_layer_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_layer_request.py` & `bimdata-api-client-9.9.0/test/test_layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_line.py` & `bimdata-api-client-9.9.0/test/test_line.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_line_request.py` & `bimdata-api-client-9.9.0/test/test_line_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_marketplace_app.py` & `bimdata-api-client-9.9.0/test/test_marketplace_app_light.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,32 +11,30 @@
 
 import sys
 import unittest
 
 import bimdata_api_client
 from bimdata_api_client.model.marketplace_app_image import MarketplaceAppImage
 from bimdata_api_client.model.public_organization import PublicOrganization
-from bimdata_api_client.model.user import User
 globals()['MarketplaceAppImage'] = MarketplaceAppImage
 globals()['PublicOrganization'] = PublicOrganization
-globals()['User'] = User
-from bimdata_api_client.model.marketplace_app import MarketplaceApp
+from bimdata_api_client.model.marketplace_app_light import MarketplaceAppLight
 
 
-class TestMarketplaceApp(unittest.TestCase):
-    """MarketplaceApp unit test stubs"""
+class TestMarketplaceAppLight(unittest.TestCase):
+    """MarketplaceAppLight unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMarketplaceApp(self):
-        """Test MarketplaceApp"""
+    def testMarketplaceAppLight(self):
+        """Test MarketplaceAppLight"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MarketplaceApp()  # noqa: E501
+        # model = MarketplaceAppLight()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_marketplace_app_image.py` & `bimdata-api-client-9.9.0/test/test_marketplace_app_image.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_marketplace_app_image_request.py` & `bimdata-api-client-9.9.0/test/test_raw_unit_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.marketplace_app_image_request import MarketplaceAppImageRequest
+from bimdata_api_client.model.raw_unit_request import RawUnitRequest
 
 
-class TestMarketplaceAppImageRequest(unittest.TestCase):
-    """MarketplaceAppImageRequest unit test stubs"""
+class TestRawUnitRequest(unittest.TestCase):
+    """RawUnitRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMarketplaceAppImageRequest(self):
-        """Test MarketplaceAppImageRequest"""
+    def testRawUnitRequest(self):
+        """Test RawUnitRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MarketplaceAppImageRequest()  # noqa: E501
+        # model = RawUnitRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_marketplace_app_request.py` & `bimdata-api-client-9.9.0/test/test_marketplace_app_light_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.marketplace_app_request import MarketplaceAppRequest
+from bimdata_api_client.model.marketplace_app_light_request import MarketplaceAppLightRequest
 
 
-class TestMarketplaceAppRequest(unittest.TestCase):
-    """MarketplaceAppRequest unit test stubs"""
+class TestMarketplaceAppLightRequest(unittest.TestCase):
+    """MarketplaceAppLightRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMarketplaceAppRequest(self):
-        """Test MarketplaceAppRequest"""
+    def testMarketplaceAppLightRequest(self):
+        """Test MarketplaceAppLightRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MarketplaceAppRequest()  # noqa: E501
+        # model = MarketplaceAppLightRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_material.py` & `bimdata-api-client-9.9.0/test/test_material.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_material_list_component.py` & `bimdata-api-client-9.9.0/test/test_material_list_component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_material_list_component_request.py` & `bimdata-api-client-9.9.0/test/test_material_list_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_material_option.py` & `bimdata-api-client-9.9.0/test/test_material_option.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_material_request.py` & `bimdata-api-client-9.9.0/test/test_material_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model.py` & `bimdata-api-client-9.9.0/test/test_model.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_api.py` & `bimdata-api-client-9.9.0/test/test_model_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_errors.py` & `bimdata-api-client-9.9.0/test/test_model_errors.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_errors_request.py` & `bimdata-api-client-9.9.0/test/test_model_errors_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_files.py` & `bimdata-api-client-9.9.0/test/test_model_files.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_property.py` & `bimdata-api-client-9.9.0/test/test_model_property.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_request.py` & `bimdata-api-client-9.9.0/test/test_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_model_with_positioning_plan.py` & `bimdata-api-client-9.9.0/test/test_model_with_positioning_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_organization.py` & `bimdata-api-client-9.9.0/test/test_organization.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_organization_request.py` & `bimdata-api-client-9.9.0/test/test_organization_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_orthogonal_camera.py` & `bimdata-api-client-9.9.0/test/test_orthogonal_camera.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_orthogonal_camera_request.py` & `bimdata-api-client-9.9.0/test/test_orthogonal_camera_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_bcf_project_request.py` & `bimdata-api-client-9.9.0/test/test_patched_bcf_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_check_plan_request.py` & `bimdata-api-client-9.9.0/test/test_patched_check_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_checker_result_request.py` & `bimdata-api-client-9.9.0/test/test_patched_checker_result_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_classification_request.py` & `bimdata-api-client-9.9.0/test/test_patched_classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_cloud_request.py` & `bimdata-api-client-9.9.0/test/test_patched_cloud_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_comment_request.py` & `bimdata-api-client-9.9.0/test/test_patched_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_document_request.py` & `bimdata-api-client-9.9.0/test/test_patched_document_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_element_request.py` & `bimdata-api-client-9.9.0/test/test_patched_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_folder_without_children_request.py` & `bimdata-api-client-9.9.0/test/test_patched_folder_without_children_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_full_topic_request.py` & `bimdata-api-client-9.9.0/test/test_patched_full_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_group_folder_request.py` & `bimdata-api-client-9.9.0/test/test_patched_group_folder_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_group_request.py` & `bimdata-api-client-9.9.0/test/test_patched_group_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_ifc_access_token_request.py` & `bimdata-api-client-9.9.0/test/test_patched_ifc_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_ifc_checker_request.py` & `bimdata-api-client-9.9.0/test/test_patched_ifc_checker_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_label_request.py` & `bimdata-api-client-9.9.0/test/test_patched_label_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_layer_request.py` & `bimdata-api-client-9.9.0/test/test_patched_layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_model_request.py` & `bimdata-api-client-9.9.0/test/test_patched_model_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_positioning_plan_request.py` & `bimdata-api-client-9.9.0/test/test_patched_positioning_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_priority_request.py` & `bimdata-api-client-9.9.0/test/test_patched_priority_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_processor_handler_request.py` & `bimdata-api-client-9.9.0/test/test_patched_processor_handler_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_project_access_token_request.py` & `bimdata-api-client-9.9.0/test/test_patched_project_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_project_request.py` & `bimdata-api-client-9.9.0/test/test_patched_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_property_definition_request.py` & `bimdata-api-client-9.9.0/test/test_patched_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_property_request.py` & `bimdata-api-client-9.9.0/test/test_patched_property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_property_set_request.py` & `bimdata-api-client-9.9.0/test/test_patched_property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_rule_component_request.py` & `bimdata-api-client-9.9.0/test/test_patched_rule_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_rule_request.py` & `bimdata-api-client-9.9.0/test/test_patched_rule_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_ruleset_request.py` & `bimdata-api-client-9.9.0/test/test_patched_ruleset_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_space_request.py` & `bimdata-api-client-9.9.0/test/test_patched_space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_stage_request.py` & `bimdata-api-client-9.9.0/test/test_patched_stage_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_storey_building_request.py` & `bimdata-api-client-9.9.0/test/test_patched_storey_building_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_system_request.py` & `bimdata-api-client-9.9.0/test/test_patched_system_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_tag_request.py` & `bimdata-api-client-9.9.0/test/test_patched_tag_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_topic_request.py` & `bimdata-api-client-9.9.0/test/test_patched_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_topic_status_request.py` & `bimdata-api-client-9.9.0/test/test_patched_topic_status_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_topic_type_request.py` & `bimdata-api-client-9.9.0/test/test_patched_topic_type_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_unit_request.py` & `bimdata-api-client-9.9.0/test/test_patched_unit_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_user_cloud_update_request.py` & `bimdata-api-client-9.9.0/test/test_patched_user_cloud_update_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_user_project_update_request.py` & `bimdata-api-client-9.9.0/test/test_patched_user_project_update_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_viewpoint_request.py` & `bimdata-api-client-9.9.0/test/test_patched_viewpoint_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_visa_comment_request.py` & `bimdata-api-client-9.9.0/test/test_patched_visa_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_visa_request.py` & `bimdata-api-client-9.9.0/test/test_patched_visa_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_visa_validation_request.py` & `bimdata-api-client-9.9.0/test/test_patched_visa_validation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_web_hook_request.py` & `bimdata-api-client-9.9.0/test/test_patched_web_hook_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_zone_request.py` & `bimdata-api-client-9.9.0/test/test_patched_zone_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_patched_zone_space_request.py` & `bimdata-api-client-9.9.0/test/test_patched_zone_space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_perspective_camera.py` & `bimdata-api-client-9.9.0/test/test_perspective_camera.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_perspective_camera_request.py` & `bimdata-api-client-9.9.0/test/test_perspective_camera_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_pin.py` & `bimdata-api-client-9.9.0/test/test_pin.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_pin_request.py` & `bimdata-api-client-9.9.0/test/test_pin_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_point.py` & `bimdata-api-client-9.9.0/test/test_point.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_point_request.py` & `bimdata-api-client-9.9.0/test/test_point_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_positioning_plan.py` & `bimdata-api-client-9.9.0/test/test_positioning_plan.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_priority.py` & `bimdata-api-client-9.9.0/test/test_priority.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_priority_request.py` & `bimdata-api-client-9.9.0/test/test_priority_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_processor_handler.py` & `bimdata-api-client-9.9.0/test/test_processor_handler.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project.py` & `bimdata-api-client-9.9.0/test/test_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_access_token.py` & `bimdata-api-client-9.9.0/test/test_project_access_token.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_access_token_request.py` & `bimdata-api-client-9.9.0/test/test_project_access_token_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_folder_tree.py` & `bimdata-api-client-9.9.0/test/test_project_folder_tree.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_invitation.py` & `bimdata-api-client-9.9.0/test/test_project_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_invitation_request.py` & `bimdata-api-client-9.9.0/test/test_project_invitation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_request.py` & `bimdata-api-client-9.9.0/test/test_project_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_role.py` & `bimdata-api-client-9.9.0/test/test_project_role.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_size.py` & `bimdata-api-client-9.9.0/test/test_project_size.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_project_with_children.py` & `bimdata-api-client-9.9.0/test/test_project_with_children.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_property_definition.py` & `bimdata-api-client-9.9.0/test/test_property_definition.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_property_definition_request.py` & `bimdata-api-client-9.9.0/test/test_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_property_request.py` & `bimdata-api-client-9.9.0/test/test_property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_property_set.py` & `bimdata-api-client-9.9.0/test/test_property_set.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_property_set_request.py` & `bimdata-api-client-9.9.0/test/test_property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_public_organization.py` & `bimdata-api-client-9.9.0/test/test_public_organization.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_public_organization_request.py` & `bimdata-api-client-9.9.0/test/test_public_organization_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_classification.py` & `bimdata-api-client-9.9.0/test/test_raw_classification.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_classification_request.py` & `bimdata-api-client-9.9.0/test/test_raw_classification_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_definition.py` & `bimdata-api-client-9.9.0/test/test_raw_definition.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_definition_request.py` & `bimdata-api-client-9.9.0/test/test_raw_definition_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_element.py` & `bimdata-api-client-9.9.0/test/test_raw_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_element_request.py` & `bimdata-api-client-9.9.0/test/test_raw_element_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_elements.py` & `bimdata-api-client-9.9.0/test/test_raw_elements.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_elements_request.py` & `bimdata-api-client-9.9.0/test/test_raw_elements_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_layer.py` & `bimdata-api-client-9.9.0/test/test_raw_layer.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_layer_request.py` & `bimdata-api-client-9.9.0/test/test_raw_layer_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material.py` & `bimdata-api-client-9.9.0/test/test_raw_material.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_list.py` & `bimdata-api-client-9.9.0/test/test_raw_material_list.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_list_components.py` & `bimdata-api-client-9.9.0/test/test_raw_material_list_components.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_list_components_request.py` & `bimdata-api-client-9.9.0/test/test_raw_material_list_components_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_list_request.py` & `bimdata-api-client-9.9.0/test/test_raw_material_list_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_options.py` & `bimdata-api-client-9.9.0/test/test_raw_material_options.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_options_request.py` & `bimdata-api-client-9.9.0/test/test_raw_material_options_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_material_request.py` & `bimdata-api-client-9.9.0/test/test_raw_material_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_property.py` & `bimdata-api-client-9.9.0/test/test_raw_property.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_property_request.py` & `bimdata-api-client-9.9.0/test/test_raw_property_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_property_set.py` & `bimdata-api-client-9.9.0/test/test_raw_property_set.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_property_set_request.py` & `bimdata-api-client-9.9.0/test/test_raw_property_set_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_system.py` & `bimdata-api-client-9.9.0/test/test_raw_system.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_system_request.py` & `bimdata-api-client-9.9.0/test/test_raw_system_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_unit.py` & `bimdata-api-client-9.9.0/test/test_raw_unit.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_raw_unit_request.py` & `bimdata-api-client-9.9.0/test/test_system_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.raw_unit_request import RawUnitRequest
+from bimdata_api_client.model.system_request import SystemRequest
 
 
-class TestRawUnitRequest(unittest.TestCase):
-    """RawUnitRequest unit test stubs"""
+class TestSystemRequest(unittest.TestCase):
+    """SystemRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRawUnitRequest(self):
-        """Test RawUnitRequest"""
+    def testSystemRequest(self):
+        """Test SystemRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = RawUnitRequest()  # noqa: E501
+        # model = SystemRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_recursive_folder_children.py` & `bimdata-api-client-9.9.0/test/test_recursive_folder_children.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,16 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.document import Document
-from bimdata_api_client.model.folder_group_permission import FolderGroupPermission
 from bimdata_api_client.model.tag import Tag
 from bimdata_api_client.model.user import User
-globals()['Document'] = Document
-globals()['FolderGroupPermission'] = FolderGroupPermission
 globals()['Tag'] = Tag
 globals()['User'] = User
 from bimdata_api_client.model.recursive_folder_children import RecursiveFolderChildren
 
 
 class TestRecursiveFolderChildren(unittest.TestCase):
     """RecursiveFolderChildren unit test stubs"""
```

### Comparing `bimdata-api-client-9.8.1/test/test_rule.py` & `bimdata-api-client-9.9.0/test/test_rule.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_rule_component.py` & `bimdata-api-client-9.9.0/test/test_rule_component.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_rule_component_request.py` & `bimdata-api-client-9.9.0/test/test_rule_component_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_rule_request.py` & `bimdata-api-client-9.9.0/test/test_rule_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ruleset.py` & `bimdata-api-client-9.9.0/test/test_ruleset.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_ruleset_request.py` & `bimdata-api-client-9.9.0/test/test_ruleset_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_self_bcf_user.py` & `bimdata-api-client-9.9.0/test/test_self_bcf_user.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_self_user.py` & `bimdata-api-client-9.9.0/test/test_zone.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,34 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.cloud_role import CloudRole
-from bimdata_api_client.model.organization import Organization
-from bimdata_api_client.model.project_role import ProjectRole
-globals()['CloudRole'] = CloudRole
-globals()['Organization'] = Organization
-globals()['ProjectRole'] = ProjectRole
-from bimdata_api_client.model.self_user import SelfUser
+from bimdata_api_client.model.space import Space
+globals()['Space'] = Space
+from bimdata_api_client.model.zone import Zone
 
 
-class TestSelfUser(unittest.TestCase):
-    """SelfUser unit test stubs"""
+class TestZone(unittest.TestCase):
+    """Zone unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSelfUser(self):
-        """Test SelfUser"""
+    def testZone(self):
+        """Test Zone"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SelfUser()  # noqa: E501
+        # model = Zone()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_simple_element.py` & `bimdata-api-client-9.9.0/test/test_simple_element.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_size.py` & `bimdata-api-client-9.9.0/test/test_size.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_snapshot.py` & `bimdata-api-client-9.9.0/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_snapshot_request.py` & `bimdata-api-client-9.9.0/test/test_snapshot_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_space.py` & `bimdata-api-client-9.9.0/test/test_space.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_space_request.py` & `bimdata-api-client-9.9.0/test/test_space_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_sso_api.py` & `bimdata-api-client-9.9.0/test/test_sso_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_stage.py` & `bimdata-api-client-9.9.0/test/test_stage.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_stage_request.py` & `bimdata-api-client-9.9.0/test/test_stage_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_storey.py` & `bimdata-api-client-9.9.0/test/test_storey.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_storey_building_request.py` & `bimdata-api-client-9.9.0/test/test_storey_building_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_storey_model_plan_request.py` & `bimdata-api-client-9.9.0/test/test_storey_model_plan_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_system.py` & `bimdata-api-client-9.9.0/test/test_system.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_system_request.py` & `bimdata-api-client-9.9.0/test/test_tag_id_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.system_request import SystemRequest
+from bimdata_api_client.model.tag_id_request import TagIdRequest
 
 
-class TestSystemRequest(unittest.TestCase):
-    """SystemRequest unit test stubs"""
+class TestTagIdRequest(unittest.TestCase):
+    """TagIdRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSystemRequest(self):
-        """Test SystemRequest"""
+    def testTagIdRequest(self):
+        """Test TagIdRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SystemRequest()  # noqa: E501
+        # model = TagIdRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_tag.py` & `bimdata-api-client-9.9.0/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_tag_id_request.py` & `bimdata-api-client-9.9.0/test/test_web_hook_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.tag_id_request import TagIdRequest
+from bimdata_api_client.model.web_hook_request import WebHookRequest
 
 
-class TestTagIdRequest(unittest.TestCase):
-    """TagIdRequest unit test stubs"""
+class TestWebHookRequest(unittest.TestCase):
+    """WebHookRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTagIdRequest(self):
-        """Test TagIdRequest"""
+    def testWebHookRequest(self):
+        """Test WebHookRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TagIdRequest()  # noqa: E501
+        # model = WebHookRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_tag_request.py` & `bimdata-api-client-9.9.0/test/test_tag_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic.py` & `bimdata-api-client-9.9.0/test/test_topic.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic_request.py` & `bimdata-api-client-9.9.0/test/test_topic_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic_status.py` & `bimdata-api-client-9.9.0/test/test_topic_status.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic_status_request.py` & `bimdata-api-client-9.9.0/test/test_topic_status_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic_type.py` & `bimdata-api-client-9.9.0/test/test_topic_type.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_topic_type_request.py` & `bimdata-api-client-9.9.0/test/test_topic_type_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_unit.py` & `bimdata-api-client-9.9.0/test/test_unit.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_unit_request.py` & `bimdata-api-client-9.9.0/test/test_unit_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_user.py` & `bimdata-api-client-9.9.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_user_invitation.py` & `bimdata-api-client-9.9.0/test/test_user_invitation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_user_project.py` & `bimdata-api-client-9.9.0/test/test_user_project.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_user_project_id_request.py` & `bimdata-api-client-9.9.0/test/test_user_project_id_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_view_setup_hints.py` & `bimdata-api-client-9.9.0/test/test_view_setup_hints.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_view_setup_hints_request.py` & `bimdata-api-client-9.9.0/test/test_view_setup_hints_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_viewpoint.py` & `bimdata-api-client-9.9.0/test/test_viewpoint.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_viewpoint_request.py` & `bimdata-api-client-9.9.0/test/test_viewpoint_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa.py` & `bimdata-api-client-9.9.0/test/test_visa.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa_comment.py` & `bimdata-api-client-9.9.0/test/test_visa_comment.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa_comment_request.py` & `bimdata-api-client-9.9.0/test/test_visa_comment_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa_request.py` & `bimdata-api-client-9.9.0/test/test_visa_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa_validation.py` & `bimdata-api-client-9.9.0/test/test_visa_validation.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visa_validation_request.py` & `bimdata-api-client-9.9.0/test/test_visa_validation_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visibility.py` & `bimdata-api-client-9.9.0/test/test_visibility.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_visibility_request.py` & `bimdata-api-client-9.9.0/test/test_visibility_request.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_web_hook.py` & `bimdata-api-client-9.9.0/test/test_web_hook.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_web_hook_request.py` & `bimdata-api-client-9.9.0/test/test_write_folder_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.web_hook_request import WebHookRequest
+from bimdata_api_client.model.write_folder_request import WriteFolderRequest
 
 
-class TestWebHookRequest(unittest.TestCase):
-    """WebHookRequest unit test stubs"""
+class TestWriteFolderRequest(unittest.TestCase):
+    """WriteFolderRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebHookRequest(self):
-        """Test WebHookRequest"""
+    def testWriteFolderRequest(self):
+        """Test WriteFolderRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WebHookRequest()  # noqa: E501
+        # model = WriteFolderRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_webhook_api.py` & `bimdata-api-client-9.9.0/test/test_webhook_api.py`

 * *Files identical despite different names*

### Comparing `bimdata-api-client-9.8.1/test/test_write_folder_request.py` & `bimdata-api-client-9.9.0/test/test_zone_space_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.write_folder_request import WriteFolderRequest
+from bimdata_api_client.model.zone_space_request import ZoneSpaceRequest
 
 
-class TestWriteFolderRequest(unittest.TestCase):
-    """WriteFolderRequest unit test stubs"""
+class TestZoneSpaceRequest(unittest.TestCase):
+    """ZoneSpaceRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWriteFolderRequest(self):
-        """Test WriteFolderRequest"""
+    def testZoneSpaceRequest(self):
+        """Test ZoneSpaceRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WriteFolderRequest()  # noqa: E501
+        # model = ZoneSpaceRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_zone.py` & `bimdata-api-client-9.9.0/test/test_zone_space.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import bimdata_api_client
-from bimdata_api_client.model.space import Space
-globals()['Space'] = Space
-from bimdata_api_client.model.zone import Zone
+from bimdata_api_client.model.zone_space import ZoneSpace
 
 
-class TestZone(unittest.TestCase):
-    """Zone unit test stubs"""
+class TestZoneSpace(unittest.TestCase):
+    """ZoneSpace unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testZone(self):
-        """Test Zone"""
+    def testZoneSpace(self):
+        """Test ZoneSpace"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Zone()  # noqa: E501
+        # model = ZoneSpace()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bimdata-api-client-9.8.1/test/test_zone_request.py` & `bimdata-api-client-9.9.0/test/test_zone_request.py`

 * *Files identical despite different names*

