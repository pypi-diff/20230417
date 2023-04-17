# Comparing `tmp/fake-bpy-module-latest-20230416.tar.gz` & `tmp/fake-bpy-module-latest-20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230416.tar", last modified: Sun Apr 16 06:21:12 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230417.tar", last modified: Mon Apr 17 06:22:15 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230416.tar` & `fake-bpy-module-latest-20230417.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-16 06:21:11.000000 fake-bpy-module-latest-20230416/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-16 06:19:15.000000 fake-bpy-module-latest-20230416/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-16 06:19:12.000000 fake-bpy-module-latest-20230416/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-16 06:21:05.000000 fake-bpy-module-latest-20230416/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-16 06:21:06.000000 fake-bpy-module-latest-20230416/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-16 06:21:07.000000 fake-bpy-module-latest-20230416/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-16 06:21:05.000000 fake-bpy-module-latest-20230416/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-16 06:21:08.000000 fake-bpy-module-latest-20230416/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-16 06:21:05.000000 fake-bpy-module-latest-20230416/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-16 06:20:22.000000 fake-bpy-module-latest-20230416/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-16 06:20:54.000000 fake-bpy-module-latest-20230416/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-16 06:20:54.000000 fake-bpy-module-latest-20230416/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-16 06:20:25.000000 fake-bpy-module-latest-20230416/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-16 06:19:24.000000 fake-bpy-module-latest-20230416/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-16 06:20:47.000000 fake-bpy-module-latest-20230416/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-16 06:19:19.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-16 06:20:23.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-16 06:20:25.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-16 06:20:26.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-16 06:19:19.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-16 06:20:26.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-16 06:20:23.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-16 06:19:22.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-16 06:20:19.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-16 06:20:59.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-16 06:19:23.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-16 06:19:18.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-16 06:20:59.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-16 06:20:59.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-16 06:20:54.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-16 06:20:25.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-16 06:20:53.000000 fake-bpy-module-latest-20230416/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-16 06:20:24.000000 fake-bpy-module-latest-20230416/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-16 06:20:47.000000 fake-bpy-module-latest-20230416/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-16 06:20:27.000000 fake-bpy-module-latest-20230416/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-16 06:20:22.000000 fake-bpy-module-latest-20230416/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-16 06:19:28.000000 fake-bpy-module-latest-20230416/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-16 06:20:13.000000 fake-bpy-module-latest-20230416/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-16 06:20:53.000000 fake-bpy-module-latest-20230416/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-16 06:20:55.000000 fake-bpy-module-latest-20230416/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-16 06:20:51.000000 fake-bpy-module-latest-20230416/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-16 06:19:23.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-16 06:20:54.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-16 06:19:21.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-16 06:20:27.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-16 06:20:49.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-16 06:20:14.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-16 06:19:24.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-16 06:20:19.000000 fake-bpy-module-latest-20230416/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-16 06:20:36.000000 fake-bpy-module-latest-20230416/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-16 06:20:12.000000 fake-bpy-module-latest-20230416/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-16 06:19:20.000000 fake-bpy-module-latest-20230416/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-16 06:20:28.000000 fake-bpy-module-latest-20230416/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-16 06:21:03.000000 fake-bpy-module-latest-20230416/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-16 06:20:27.000000 fake-bpy-module-latest-20230416/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-16 06:21:03.000000 fake-bpy-module-latest-20230416/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-16 06:20:25.000000 fake-bpy-module-latest-20230416/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-16 06:20:21.000000 fake-bpy-module-latest-20230416/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71754 2023-04-16 06:20:22.000000 fake-bpy-module-latest-20230416/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-16 06:21:00.000000 fake-bpy-module-latest-20230416/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-16 06:19:28.000000 fake-bpy-module-latest-20230416/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-16 06:20:23.000000 fake-bpy-module-latest-20230416/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-16 06:19:22.000000 fake-bpy-module-latest-20230416/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-16 06:20:19.000000 fake-bpy-module-latest-20230416/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-16 06:20:52.000000 fake-bpy-module-latest-20230416/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-16 06:19:19.000000 fake-bpy-module-latest-20230416/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-16 06:20:58.000000 fake-bpy-module-latest-20230416/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-16 06:20:28.000000 fake-bpy-module-latest-20230416/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-16 06:19:20.000000 fake-bpy-module-latest-20230416/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-16 06:20:25.000000 fake-bpy-module-latest-20230416/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-16 06:20:12.000000 fake-bpy-module-latest-20230416/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-16 06:19:20.000000 fake-bpy-module-latest-20230416/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-04-16 06:20:36.000000 fake-bpy-module-latest-20230416/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-16 06:19:19.000000 fake-bpy-module-latest-20230416/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-16 06:20:18.000000 fake-bpy-module-latest-20230416/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-16 06:20:12.000000 fake-bpy-module-latest-20230416/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   234684 2023-04-16 06:20:34.000000 fake-bpy-module-latest-20230416/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-16 06:19:22.000000 fake-bpy-module-latest-20230416/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-16 06:19:12.000000 fake-bpy-module-latest-20230416/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-16 06:19:15.000000 fake-bpy-module-latest-20230416/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-16 06:19:15.000000 fake-bpy-module-latest-20230416/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-16 06:19:15.000000 fake-bpy-module-latest-20230416/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-16 06:18:31.000000 fake-bpy-module-latest-20230416/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-16 06:19:07.000000 fake-bpy-module-latest-20230416/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-16 06:18:34.000000 fake-bpy-module-latest-20230416/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-16 06:18:48.000000 fake-bpy-module-latest-20230416/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-16 06:18:49.000000 fake-bpy-module-latest-20230416/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-16 06:18:55.000000 fake-bpy-module-latest-20230416/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-16 06:18:50.000000 fake-bpy-module-latest-20230416/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-16 06:19:07.000000 fake-bpy-module-latest-20230416/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-16 06:18:43.000000 fake-bpy-module-latest-20230416/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-16 06:18:49.000000 fake-bpy-module-latest-20230416/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-16 06:19:06.000000 fake-bpy-module-latest-20230416/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-16 06:18:33.000000 fake-bpy-module-latest-20230416/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-16 06:18:43.000000 fake-bpy-module-latest-20230416/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-16 06:18:48.000000 fake-bpy-module-latest-20230416/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-16 06:18:39.000000 fake-bpy-module-latest-20230416/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-16 06:19:03.000000 fake-bpy-module-latest-20230416/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40576 2023-04-16 06:18:41.000000 fake-bpy-module-latest-20230416/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    28761 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-04-16 06:18:49.000000 fake-bpy-module-latest-20230416/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-16 06:18:43.000000 fake-bpy-module-latest-20230416/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   131531 2023-04-16 06:19:06.000000 fake-bpy-module-latest-20230416/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-16 06:18:47.000000 fake-bpy-module-latest-20230416/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 06:18:55.000000 fake-bpy-module-latest-20230416/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-16 06:19:06.000000 fake-bpy-module-latest-20230416/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-16 06:19:06.000000 fake-bpy-module-latest-20230416/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-16 06:18:51.000000 fake-bpy-module-latest-20230416/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 06:18:39.000000 fake-bpy-module-latest-20230416/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-16 06:18:47.000000 fake-bpy-module-latest-20230416/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-16 06:18:46.000000 fake-bpy-module-latest-20230416/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-16 06:19:02.000000 fake-bpy-module-latest-20230416/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-16 06:19:03.000000 fake-bpy-module-latest-20230416/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   219005 2023-04-16 06:18:54.000000 fake-bpy-module-latest-20230416/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-16 06:18:38.000000 fake-bpy-module-latest-20230416/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-16 06:18:44.000000 fake-bpy-module-latest-20230416/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-16 06:18:31.000000 fake-bpy-module-latest-20230416/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-16 06:18:42.000000 fake-bpy-module-latest-20230416/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-16 06:18:50.000000 fake-bpy-module-latest-20230416/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-16 06:18:42.000000 fake-bpy-module-latest-20230416/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-16 06:18:34.000000 fake-bpy-module-latest-20230416/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-16 06:18:38.000000 fake-bpy-module-latest-20230416/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-16 06:18:39.000000 fake-bpy-module-latest-20230416/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-16 06:18:46.000000 fake-bpy-module-latest-20230416/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-16 06:18:31.000000 fake-bpy-module-latest-20230416/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-16 06:19:06.000000 fake-bpy-module-latest-20230416/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46532 2023-04-16 06:18:39.000000 fake-bpy-module-latest-20230416/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-16 06:19:04.000000 fake-bpy-module-latest-20230416/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-16 06:18:33.000000 fake-bpy-module-latest-20230416/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-16 06:18:48.000000 fake-bpy-module-latest-20230416/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-16 06:18:49.000000 fake-bpy-module-latest-20230416/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-16 06:18:47.000000 fake-bpy-module-latest-20230416/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-16 06:19:07.000000 fake-bpy-module-latest-20230416/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-16 06:18:54.000000 fake-bpy-module-latest-20230416/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-16 06:19:02.000000 fake-bpy-module-latest-20230416/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-16 06:18:33.000000 fake-bpy-module-latest-20230416/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-16 06:18:49.000000 fake-bpy-module-latest-20230416/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-16 06:18:50.000000 fake-bpy-module-latest-20230416/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-16 06:19:09.000000 fake-bpy-module-latest-20230416/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   245270 2023-04-16 06:19:00.000000 fake-bpy-module-latest-20230416/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-16 06:18:35.000000 fake-bpy-module-latest-20230416/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-16 06:19:08.000000 fake-bpy-module-latest-20230416/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3484883 2023-04-16 06:18:31.000000 fake-bpy-module-latest-20230416/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-16 06:19:10.000000 fake-bpy-module-latest-20230416/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-16 06:19:15.000000 fake-bpy-module-latest-20230416/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-16 06:19:14.000000 fake-bpy-module-latest-20230416/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26857 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-16 06:21:09.000000 fake-bpy-module-latest-20230416/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-16 06:19:13.000000 fake-bpy-module-latest-20230416/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 06:12:19.000000 fake-bpy-module-latest-20230416/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-16 06:21:03.000000 fake-bpy-module-latest-20230416/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-16 06:19:17.000000 fake-bpy-module-latest-20230416/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-16 06:21:10.000000 fake-bpy-module-latest-20230416/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 06:21:12.000000 fake-bpy-module-latest-20230416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-16 06:21:11.000000 fake-bpy-module-latest-20230416/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-16 06:21:04.000000 fake-bpy-module-latest-20230416/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-17 06:22:14.000000 fake-bpy-module-latest-20230417/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-17 06:20:16.000000 fake-bpy-module-latest-20230417/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-17 06:20:22.000000 fake-bpy-module-latest-20230417/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-17 06:20:22.000000 fake-bpy-module-latest-20230417/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-17 06:20:27.000000 fake-bpy-module-latest-20230417/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-17 06:20:27.000000 fake-bpy-module-latest-20230417/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-17 06:20:22.000000 fake-bpy-module-latest-20230417/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-17 06:20:24.000000 fake-bpy-module-latest-20230417/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-17 06:20:25.000000 fake-bpy-module-latest-20230417/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-17 06:20:23.000000 fake-bpy-module-latest-20230417/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-17 06:20:27.000000 fake-bpy-module-latest-20230417/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-17 06:21:52.000000 fake-bpy-module-latest-20230417/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 06:21:50.000000 fake-bpy-module-latest-20230417/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-17 06:21:48.000000 fake-bpy-module-latest-20230417/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 06:22:00.000000 fake-bpy-module-latest-20230417/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-17 06:22:05.000000 fake-bpy-module-latest-20230417/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-17 06:21:27.000000 fake-bpy-module-latest-20230417/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-17 06:22:10.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-17 06:21:45.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-17 06:22:14.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-17 06:21:15.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-17 06:22:04.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-17 06:21:38.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-17 06:21:38.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-17 06:22:00.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-17 06:20:30.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-17 06:21:48.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-17 06:21:53.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-17 06:20:30.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-17 06:21:48.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-17 06:20:30.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-17 06:22:00.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-17 06:21:38.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-17 06:21:49.000000 fake-bpy-module-latest-20230417/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-17 06:21:28.000000 fake-bpy-module-latest-20230417/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-17 06:21:52.000000 fake-bpy-module-latest-20230417/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-17 06:21:36.000000 fake-bpy-module-latest-20230417/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-17 06:21:14.000000 fake-bpy-module-latest-20230417/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-17 06:21:49.000000 fake-bpy-module-latest-20230417/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-17 06:21:49.000000 fake-bpy-module-latest-20230417/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-17 06:21:52.000000 fake-bpy-module-latest-20230417/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-17 06:21:35.000000 fake-bpy-module-latest-20230417/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-17 06:21:56.000000 fake-bpy-module-latest-20230417/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-17 06:21:36.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-17 06:20:29.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-17 06:21:16.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-17 06:22:05.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-17 06:22:11.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-17 06:20:29.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-17 06:21:48.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-17 06:21:29.000000 fake-bpy-module-latest-20230417/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-17 06:21:30.000000 fake-bpy-module-latest-20230417/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-17 06:22:13.000000 fake-bpy-module-latest-20230417/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-17 06:22:06.000000 fake-bpy-module-latest-20230417/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-17 06:21:50.000000 fake-bpy-module-latest-20230417/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-17 06:22:10.000000 fake-bpy-module-latest-20230417/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-17 06:21:37.000000 fake-bpy-module-latest-20230417/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-17 06:21:34.000000 fake-bpy-module-latest-20230417/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-17 06:21:36.000000 fake-bpy-module-latest-20230417/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-17 06:21:46.000000 fake-bpy-module-latest-20230417/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71754 2023-04-17 06:20:29.000000 fake-bpy-module-latest-20230417/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-17 06:21:36.000000 fake-bpy-module-latest-20230417/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-17 06:22:10.000000 fake-bpy-module-latest-20230417/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-17 06:21:16.000000 fake-bpy-module-latest-20230417/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-17 06:21:35.000000 fake-bpy-module-latest-20230417/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-17 06:22:13.000000 fake-bpy-module-latest-20230417/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-17 06:21:27.000000 fake-bpy-module-latest-20230417/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-17 06:22:13.000000 fake-bpy-module-latest-20230417/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-17 06:22:04.000000 fake-bpy-module-latest-20230417/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-17 06:22:05.000000 fake-bpy-module-latest-20230417/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-17 06:21:53.000000 fake-bpy-module-latest-20230417/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-17 06:21:31.000000 fake-bpy-module-latest-20230417/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-17 06:21:53.000000 fake-bpy-module-latest-20230417/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-17 06:22:10.000000 fake-bpy-module-latest-20230417/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-04-17 06:21:46.000000 fake-bpy-module-latest-20230417/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-17 06:21:51.000000 fake-bpy-module-latest-20230417/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-17 06:22:00.000000 fake-bpy-module-latest-20230417/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-17 06:21:13.000000 fake-bpy-module-latest-20230417/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234684 2023-04-17 06:21:45.000000 fake-bpy-module-latest-20230417/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-17 06:22:10.000000 fake-bpy-module-latest-20230417/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-17 06:20:16.000000 fake-bpy-module-latest-20230417/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-17 06:20:19.000000 fake-bpy-module-latest-20230417/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-17 06:20:19.000000 fake-bpy-module-latest-20230417/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-17 06:20:14.000000 fake-bpy-module-latest-20230417/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-17 06:19:35.000000 fake-bpy-module-latest-20230417/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-17 06:20:04.000000 fake-bpy-module-latest-20230417/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-17 06:19:38.000000 fake-bpy-module-latest-20230417/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-17 06:20:07.000000 fake-bpy-module-latest-20230417/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-17 06:19:43.000000 fake-bpy-module-latest-20230417/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-17 06:20:01.000000 fake-bpy-module-latest-20230417/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-17 06:20:00.000000 fake-bpy-module-latest-20230417/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-17 06:20:00.000000 fake-bpy-module-latest-20230417/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 06:19:35.000000 fake-bpy-module-latest-20230417/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-17 06:20:04.000000 fake-bpy-module-latest-20230417/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-17 06:19:43.000000 fake-bpy-module-latest-20230417/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-17 06:20:03.000000 fake-bpy-module-latest-20230417/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-17 06:19:48.000000 fake-bpy-module-latest-20230417/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 06:19:37.000000 fake-bpy-module-latest-20230417/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40576 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28761 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-17 06:19:37.000000 fake-bpy-module-latest-20230417/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-04-17 06:20:03.000000 fake-bpy-module-latest-20230417/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131531 2023-04-17 06:20:03.000000 fake-bpy-module-latest-20230417/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-17 06:19:45.000000 fake-bpy-module-latest-20230417/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-17 06:19:46.000000 fake-bpy-module-latest-20230417/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-17 06:19:43.000000 fake-bpy-module-latest-20230417/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-17 06:20:03.000000 fake-bpy-module-latest-20230417/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-17 06:19:48.000000 fake-bpy-module-latest-20230417/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-17 06:20:11.000000 fake-bpy-module-latest-20230417/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-17 06:20:11.000000 fake-bpy-module-latest-20230417/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-17 06:19:41.000000 fake-bpy-module-latest-20230417/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219005 2023-04-17 06:19:57.000000 fake-bpy-module-latest-20230417/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-17 06:20:04.000000 fake-bpy-module-latest-20230417/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-17 06:19:46.000000 fake-bpy-module-latest-20230417/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-17 06:19:37.000000 fake-bpy-module-latest-20230417/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-17 06:19:37.000000 fake-bpy-module-latest-20230417/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-17 06:20:06.000000 fake-bpy-module-latest-20230417/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-17 06:20:11.000000 fake-bpy-module-latest-20230417/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-17 06:19:49.000000 fake-bpy-module-latest-20230417/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-17 06:19:41.000000 fake-bpy-module-latest-20230417/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-17 06:20:00.000000 fake-bpy-module-latest-20230417/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-17 06:19:44.000000 fake-bpy-module-latest-20230417/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-17 06:20:03.000000 fake-bpy-module-latest-20230417/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-17 06:19:59.000000 fake-bpy-module-latest-20230417/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-17 06:20:08.000000 fake-bpy-module-latest-20230417/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-17 06:19:35.000000 fake-bpy-module-latest-20230417/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-17 06:19:48.000000 fake-bpy-module-latest-20230417/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-17 06:19:43.000000 fake-bpy-module-latest-20230417/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-17 06:19:48.000000 fake-bpy-module-latest-20230417/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-17 06:20:11.000000 fake-bpy-module-latest-20230417/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-17 06:19:38.000000 fake-bpy-module-latest-20230417/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-17 06:19:42.000000 fake-bpy-module-latest-20230417/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-17 06:20:11.000000 fake-bpy-module-latest-20230417/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-17 06:19:36.000000 fake-bpy-module-latest-20230417/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-17 06:20:06.000000 fake-bpy-module-latest-20230417/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-17 06:19:48.000000 fake-bpy-module-latest-20230417/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-17 06:19:37.000000 fake-bpy-module-latest-20230417/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245270 2023-04-17 06:19:54.000000 fake-bpy-module-latest-20230417/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-17 06:20:06.000000 fake-bpy-module-latest-20230417/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-17 06:19:58.000000 fake-bpy-module-latest-20230417/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-17 06:20:13.000000 fake-bpy-module-latest-20230417/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-17 06:20:14.000000 fake-bpy-module-latest-20230417/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3484883 2023-04-17 06:19:35.000000 fake-bpy-module-latest-20230417/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-17 06:20:14.000000 fake-bpy-module-latest-20230417/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-17 06:20:14.000000 fake-bpy-module-latest-20230417/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-17 06:20:14.000000 fake-bpy-module-latest-20230417/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 06:20:27.000000 fake-bpy-module-latest-20230417/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-17 06:20:18.000000 fake-bpy-module-latest-20230417/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26857 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-17 06:20:22.000000 fake-bpy-module-latest-20230417/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-17 06:20:16.000000 fake-bpy-module-latest-20230417/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-17 06:20:17.000000 fake-bpy-module-latest-20230417/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:13:23.000000 fake-bpy-module-latest-20230417/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 06:20:28.000000 fake-bpy-module-latest-20230417/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-17 06:20:27.000000 fake-bpy-module-latest-20230417/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 06:20:22.000000 fake-bpy-module-latest-20230417/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:22:15.000000 fake-bpy-module-latest-20230417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-17 06:22:14.000000 fake-bpy-module-latest-20230417/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-17 06:20:21.000000 fake-bpy-module-latest-20230417/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230416/PKG-INFO` & `fake-bpy-module-latest-20230417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230416
+Version: 20230417
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230416/README.rst` & `fake-bpy-module-latest-20230417/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/addon_utils.py` & `fake-bpy-module-latest-20230417/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/animsys_refactor.py` & `fake-bpy-module-latest-20230417/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/aud.py` & `fake-bpy-module-latest-20230417/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bgl.py` & `fake-bpy-module-latest-20230417/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230417/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230417/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230417/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230417/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230417/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_math.py` & `fake-bpy-module-latest-20230417/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/__init__.py` & `fake-bpy-module-latest-20230417/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import wm
-from . import vertexpaint_dirt
-from . import mesh
-from . import presets
-from . import add_mesh_torus
-from . import object_randomize_transform
-from . import object_align
-from . import uvcalc_follow_active
+from . import constraint
 from . import object_quick_effects
-from . import uvcalc_transform
-from . import console
-from . import bmesh
+from . import presets
 from . import assets
+from . import file
 from . import spreadsheet
-from . import geometry_nodes
-from . import image
-from . import anim
-from . import uvcalc_lightmap
-from . import object
+from . import bmesh
+from . import vertexpaint_dirt
+from . import add_mesh_torus
+from . import view3d
+from . import uvcalc_transform
 from . import node
-from . import sequencer
+from . import uvcalc_follow_active
 from . import rigidbody
 from . import freestyle
-from . import view3d
-from . import clip
-from . import file
-from . import constraint
 from . import userpref
+from . import object_align
+from . import anim
+from . import uvcalc_lightmap
 from . import screen_play_rendered_anim
+from . import console
+from . import object_randomize_transform
+from . import mesh
+from . import geometry_nodes
+from . import sequencer
+from . import clip
+from . import wm
+from . import image
+from . import object
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230416/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230417/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/anim.py` & `fake-bpy-module-latest-20230417/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/assets.py` & `fake-bpy-module-latest-20230417/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230417/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/clip.py` & `fake-bpy-module-latest-20230417/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/console.py` & `fake-bpy-module-latest-20230417/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/constraint.py` & `fake-bpy-module-latest-20230417/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/file.py` & `fake-bpy-module-latest-20230417/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230417/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230417/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/image.py` & `fake-bpy-module-latest-20230417/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/mesh.py` & `fake-bpy-module-latest-20230417/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/node.py` & `fake-bpy-module-latest-20230417/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/object.py` & `fake-bpy-module-latest-20230417/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/object_align.py` & `fake-bpy-module-latest-20230417/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230417/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230417/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/presets.py` & `fake-bpy-module-latest-20230417/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230417/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230417/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230417/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230417/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/userpref.py` & `fake-bpy-module-latest-20230417/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230417/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230417/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230417/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230417/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/view3d.py` & `fake-bpy-module-latest-20230417/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_operators/wm.py` & `fake-bpy-module-latest-20230417/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230417/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/__init__.py` & `fake-bpy-module-latest-20230417/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_data_metaball
-from . import space_topbar
-from . import space_properties
-from . import properties_data_armature
-from . import properties_data_curves
-from . import properties_texture
-from . import space_toolsystem_common
-from . import space_statusbar
-from . import properties_physics_dynamicpaint
-from . import space_nla
-from . import utils
-from . import properties_data_lattice
-from . import properties_data_mesh
-from . import properties_physics_cloth
-from . import properties_physics_rigidbody_constraint
-from . import properties_collection
-from . import space_image
-from . import properties_material_gpencil
-from . import space_view3d
-from . import space_time
-from . import properties_scene
-from . import properties_object
+from . import space_filebrowser
 from . import properties_physics_rigidbody
-from . import space_userpref
-from . import space_node
+from . import properties_physics_common
+from . import properties_data_metaball
 from . import properties_data_light
-from . import properties_physics_softbody
-from . import space_dopesheet
-from . import space_filebrowser
-from . import generic_ui_list
+from . import properties_data_pointcloud
+from . import space_view3d
 from . import properties_material
-from . import properties_data_gpencil
-from . import properties_data_bone
+from . import properties_data_curve
+from . import properties_physics_dynamicpaint
 from . import space_info
+from . import properties_constraint
+from . import space_outliner
 from . import properties_freestyle
+from . import properties_physics_softbody
+from . import properties_render
 from . import space_text
-from . import properties_data_speaker
-from . import properties_animviz
-from . import properties_data_camera
+from . import space_clip
+from . import properties_paint_common
+from . import space_nla
+from . import properties_physics_cloth
+from . import space_graph
 from . import space_console
-from . import properties_data_empty
-from . import properties_data_curve
-from . import properties_physics_field
-from . import properties_world
 from . import properties_mask_common
-from . import properties_view_layer
-from . import space_spreadsheet
+from . import properties_world
+from . import properties_data_gpencil
+from . import properties_data_empty
+from . import properties_data_speaker
 from . import space_view3d_toolbar
-from . import properties_render
+from . import properties_data_bone
+from . import space_dopesheet
 from . import space_toolsystem_toolbar
-from . import properties_constraint
+from . import node_add_menu_geometry
+from . import properties_data_lightprobe
+from . import properties_physics_rigidbody_constraint
+from . import properties_data_modifier
+from . import properties_data_volume
+from . import properties_material_gpencil
+from . import properties_object
+from . import properties_view_layer
+from . import node_add_menu
+from . import space_topbar
+from . import properties_output
+from . import generic_ui_list
 from . import properties_grease_pencil_common
-from . import properties_physics_fluid
+from . import properties_data_mesh
+from . import space_statusbar
+from . import space_time
 from . import properties_particle
-from . import space_outliner
-from . import properties_output
-from . import properties_data_volume
-from . import node_add_menu_geometry
+from . import space_userpref
 from . import properties_data_shaderfx
-from . import properties_physics_common
-from . import node_add_menu
-from . import properties_paint_common
+from . import properties_data_lattice
+from . import properties_animviz
 from . import space_sequencer
-from . import properties_data_lightprobe
-from . import properties_data_pointcloud
-from . import properties_data_modifier
-from . import space_graph
-from . import space_clip
+from . import properties_data_curves
+from . import properties_physics_field
+from . import space_spreadsheet
+from . import properties_collection
+from . import properties_texture
+from . import space_image
+from . import space_toolsystem_common
 from . import properties_workspace
+from . import utils
+from . import properties_data_armature
+from . import properties_physics_fluid
+from . import space_node
+from . import space_properties
+from . import properties_scene
+from . import properties_data_camera
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230416/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230417/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230417/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230417/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230417/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_console.py` & `fake-bpy-module-latest-20230417/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230417/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230417/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230417/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_image.py` & `fake-bpy-module-latest-20230417/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_info.py` & `fake-bpy-module-latest-20230417/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230417/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_node.py` & `fake-bpy-module-latest-20230417/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230417/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230417/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230417/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230417/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230417/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_text.py` & `fake-bpy-module-latest-20230417/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_time.py` & `fake-bpy-module-latest-20230417/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230417/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230417/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230417/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230417/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230417/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230417/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bl_ui/utils.py` & `fake-bpy-module-latest-20230417/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/blf.py` & `fake-bpy-module-latest-20230417/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bmesh/__init__.py` & `fake-bpy-module-latest-20230417/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bmesh/geometry.py` & `fake-bpy-module-latest-20230417/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bmesh/ops.py` & `fake-bpy-module-latest-20230417/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bmesh/types.py` & `fake-bpy-module-latest-20230417/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bmesh/utils.py` & `fake-bpy-module-latest-20230417/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/app/__init__.py` & `fake-bpy-module-latest-20230417/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
+from . import handlers
 from . import timers
-from . import icons
 from . import translations
-from . import handlers
+from . import icons
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230416/bpy/app/handlers.py` & `fake-bpy-module-latest-20230417/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/app/icons.py` & `fake-bpy-module-latest-20230417/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/app/timers.py` & `fake-bpy-module-latest-20230417/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/app/translations.py` & `fake-bpy-module-latest-20230417/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/msgbus.py` & `fake-bpy-module-latest-20230417/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230417/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
-from . import scene
-from . import paintcurve
-from . import sequencer
-from . import curve
-from . import ui
-from . import armature
-from . import poselib
-from . import mask
+from . import collection
+from . import sculpt_curves
+from . import nla
+from . import boid
 from . import cycles
-from . import workspace
-from . import export_mesh
-from . import graph
+from . import curve
+from . import dpaint
 from . import uilist
-from . import outliner
-from . import preferences
-from . import sculpt
-from . import ed
-from . import ptcache
-from . import material
-from . import export_scene
-from . import pose
+from . import view3d
+from . import fluid
+from . import paintcurve
+from . import export_anim
 from . import palette
-from . import clip
-from . import gizmogroup
-from . import curves
-from . import paint
-from . import mesh
+from . import anim
+from . import texture
+from . import node
 from . import render
-from . import image
-from . import mball
-from . import surface
-from . import dpaint
-from . import sound
-from . import asset
-from . import uv
-from . import spreadsheet
+from . import transform
 from . import brush
-from . import cloth
-from . import font
-from . import particle
-from . import view2d
-from . import cachefile
-from . import action
-from . import marker
-from . import info
-from . import collection
+from . import constraint
+from . import sound
+from . import import_scene
 from . import file
-from . import import_anim
-from . import object
-from . import texture
-from . import buttons
+from . import cachefile
+from . import scene
+from . import export_mesh
 from . import import_curve
-from . import wm
-from . import transform
-from . import nla
-from . import node
-from . import export_anim
-from . import sculpt_curves
-from . import gpencil
-from . import import_scene
+from . import material
+from . import image
+from . import paint
 from . import import_mesh
-from . import constraint
+from . import sequencer
+from . import lattice
+from . import ed
+from . import view2d
+from . import spreadsheet
+from . import preferences
+from . import wm
+from . import object
+from . import mask
+from . import import_anim
+from . import gizmogroup
+from . import world
+from . import geometry
+from . import ptcache
+from . import surface
+from . import graph
 from . import script
-from . import anim
-from . import text
+from . import mball
 from . import camera
+from . import particle
+from . import asset
+from . import clip
+from . import cloth
+from . import rigidbody
+from . import buttons
+from . import gpencil
 from . import screen
-from . import geometry
-from . import lattice
-from . import fluid
-from . import boid
-from . import world
+from . import font
+from . import info
+from . import curves
 from . import console
-from . import rigidbody
-from . import view3d
+from . import action
+from . import outliner
+from . import uv
+from . import workspace
+from . import pose
+from . import armature
+from . import sculpt
+from . import mesh
+from . import poselib
+from . import text
+from . import marker
+from . import ui
+from . import export_scene
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/action.py` & `fake-bpy-module-latest-20230417/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/anim.py` & `fake-bpy-module-latest-20230417/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/armature.py` & `fake-bpy-module-latest-20230417/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/asset.py` & `fake-bpy-module-latest-20230417/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/boid.py` & `fake-bpy-module-latest-20230417/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/brush.py` & `fake-bpy-module-latest-20230417/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230417/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230417/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/camera.py` & `fake-bpy-module-latest-20230417/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/clip.py` & `fake-bpy-module-latest-20230417/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230417/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/collection.py` & `fake-bpy-module-latest-20230417/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/console.py` & `fake-bpy-module-latest-20230417/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230417/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/curve.py` & `fake-bpy-module-latest-20230417/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/curves.py` & `fake-bpy-module-latest-20230417/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230417/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230417/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/ed.py` & `fake-bpy-module-latest-20230417/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230417/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230417/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230417/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/file.py` & `fake-bpy-module-latest-20230417/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230417/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/font.py` & `fake-bpy-module-latest-20230417/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230417/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230417/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230417/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/graph.py` & `fake-bpy-module-latest-20230417/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/image.py` & `fake-bpy-module-latest-20230417/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230417/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230417/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230417/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230417/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/info.py` & `fake-bpy-module-latest-20230417/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230417/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/marker.py` & `fake-bpy-module-latest-20230417/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/mask.py` & `fake-bpy-module-latest-20230417/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/material.py` & `fake-bpy-module-latest-20230417/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/mball.py` & `fake-bpy-module-latest-20230417/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230417/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/nla.py` & `fake-bpy-module-latest-20230417/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/node.py` & `fake-bpy-module-latest-20230417/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/object.py` & `fake-bpy-module-latest-20230417/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230417/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/paint.py` & `fake-bpy-module-latest-20230417/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230417/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/palette.py` & `fake-bpy-module-latest-20230417/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/particle.py` & `fake-bpy-module-latest-20230417/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/pose.py` & `fake-bpy-module-latest-20230417/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230417/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230417/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230417/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/render.py` & `fake-bpy-module-latest-20230417/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230417/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/scene.py` & `fake-bpy-module-latest-20230417/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/screen.py` & `fake-bpy-module-latest-20230417/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/script.py` & `fake-bpy-module-latest-20230417/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230417/bpy/ops/sculpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,16 @@
                  *,
                  start_mouse: typing.Optional[typing.Any] = (0, 0),
                  area_normal_radius: typing.Optional[typing.Any] = 0.25,
                  strength: typing.Optional[typing.Any] = 1.0,
                  iteration_count: typing.Optional[typing.Any] = 1,
                  event_history: typing.Optional[bpy.types.bpy_prop_collection[
                      'bpy.types.OperatorStrokeElement']] = None,
-                 type: typing.Optional[typing.Any] = 'HUE',
-                 fill_color: typing.Optional[typing.Any] = (0.0, 0.0, 0.0)):
+                 type: typing.Optional[typing.Any] = 'FILL',
+                 fill_color: typing.Optional[typing.Any] = (1.0, 1.0, 1.0)):
     ''' Applies a filter to modify the active color attribute
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param start_mouse: Starting Mouse
     :type start_mouse: typing.Optional[typing.Any]
```

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230417/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230417/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/sound.py` & `fake-bpy-module-latest-20230417/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230417/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/surface.py` & `fake-bpy-module-latest-20230417/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/text.py` & `fake-bpy-module-latest-20230417/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/texture.py` & `fake-bpy-module-latest-20230417/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/transform.py` & `fake-bpy-module-latest-20230417/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/ui.py` & `fake-bpy-module-latest-20230417/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230417/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/uv.py` & `fake-bpy-module-latest-20230417/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230417/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230417/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/wm.py` & `fake-bpy-module-latest-20230417/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230417/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/ops/world.py` & `fake-bpy-module-latest-20230417/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/path.py` & `fake-bpy-module-latest-20230417/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/props.py` & `fake-bpy-module-latest-20230417/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/types.py` & `fake-bpy-module-latest-20230417/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1050 +1,1050 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f6f   bpy.import bl_o
-00000040: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
-00000050: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000060: 6965 735f 6461 7461 5f6d 6574 6162 616c  ies_data_metabal
-00000070: 6c0a 696d 706f 7274 2062 6c5f 7569 2e73  l.import bl_ui.s
-00000080: 7061 6365 5f74 6f70 6261 720a 696d 706f  pace_topbar.impo
-00000090: 7274 2062 6c5f 7569 2e73 7061 6365 5f70  rt bl_ui.space_p
-000000a0: 726f 7065 7274 6965 730a 696d 706f 7274  roperties.import
+00000040: 7065 7261 746f 7273 2e63 6f6e 7374 7261  perators.constra
+00000050: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
+00000060: 2e73 7061 6365 5f66 696c 6562 726f 7773  .space_filebrows
+00000070: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000080: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
+00000090: 6373 5f72 6967 6964 626f 6479 0a69 6d70  cs_rigidbody.imp
+000000a0: 6f72 7420 626c 5f75 690a 696d 706f 7274  ort bl_ui.import
 000000b0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000000c0: 735f 6461 7461 5f61 726d 6174 7572 650a  s_data_armature.
-000000d0: 696d 706f 7274 2062 6c5f 7569 0a69 6d70  import bl_ui.imp
-000000e0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000000f0: 7469 6573 5f64 6174 615f 6375 7276 6573  ties_data_curves
-00000100: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000110: 6f70 6572 7469 6573 5f74 6578 7475 7265  operties_texture
-00000120: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000130: 6163 655f 746f 6f6c 7379 7374 656d 5f63  ace_toolsystem_c
-00000140: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
-00000150: 7569 2e73 7061 6365 5f73 7461 7475 7362  ui.space_statusb
-00000160: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
-00000170: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000180: 6373 5f64 796e 616d 6963 7061 696e 740a  cs_dynamicpaint.
-00000190: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000001a0: 6365 5f6e 6c61 0a69 6d70 6f72 7420 626c  ce_nla.import bl
-000001b0: 5f6f 7065 7261 746f 7273 2e70 7265 7365  _operators.prese
-000001c0: 7473 0a69 6d70 6f72 7420 626c 5f75 692e  ts.import bl_ui.
-000001d0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000001e0: 6c61 7474 6963 650a 696d 706f 7274 2062  lattice.import b
-000001f0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000200: 6461 7461 5f6d 6573 680a 696d 706f 7274  data_mesh.import
-00000210: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000220: 735f 7068 7973 6963 735f 636c 6f74 680a  s_physics_cloth.
-00000230: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000240: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
-00000250: 7269 6769 6462 6f64 795f 636f 6e73 7472  rigidbody_constr
-00000260: 6169 6e74 0a69 6d70 6f72 7420 626c 5f75  aint.import bl_u
-00000270: 692e 7072 6f70 6572 7469 6573 5f63 6f6c  i.properties_col
-00000280: 6c65 6374 696f 6e0a 696d 706f 7274 2062  lection.import b
-00000290: 6c5f 7569 2e73 7061 6365 5f69 6d61 6765  l_ui.space_image
-000002a0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000002b0: 6f70 6572 7469 6573 5f6d 6174 6572 6961  operties_materia
-000002c0: 6c5f 6770 656e 6369 6c0a 696d 706f 7274  l_gpencil.import
-000002d0: 2062 6c5f 7569 2e73 7061 6365 5f76 6965   bl_ui.space_vie
-000002e0: 7733 640a 696d 706f 7274 2062 6c5f 7569  w3d.import bl_ui
-000002f0: 2e73 7061 6365 5f74 696d 650a 696d 706f  .space_time.impo
-00000300: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000310: 6965 735f 7363 656e 650a 696d 706f 7274  ies_scene.import
-00000320: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000330: 735f 6f62 6a65 6374 0a69 6d70 6f72 7420  s_object.import 
-00000340: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000350: 5f70 6879 7369 6373 5f72 6967 6964 626f  _physics_rigidbo
-00000360: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
-00000370: 7370 6163 655f 7573 6572 7072 6566 0a69  space_userpref.i
-00000380: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000390: 655f 6e6f 6465 0a69 6d70 6f72 7420 626c  e_node.import bl
-000003a0: 5f6f 7065 7261 746f 7273 2e61 7373 6574  _operators.asset
-000003b0: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
-000003c0: 726f 7065 7274 6965 735f 6461 7461 5f6c  roperties_data_l
-000003d0: 6967 6874 0a69 6d70 6f72 7420 626c 5f75  ight.import bl_u
-000003e0: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-000003f0: 7369 6373 5f73 6f66 7462 6f64 790a 696d  sics_softbody.im
-00000400: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000410: 5f64 6f70 6573 6865 6574 0a69 6d70 6f72  _dopesheet.impor
-00000420: 7420 626c 5f6f 7065 7261 746f 7273 2e73  t bl_operators.s
-00000430: 7072 6561 6473 6865 6574 0a69 6d70 6f72  preadsheet.impor
-00000440: 7420 626c 5f75 692e 7370 6163 655f 6669  t bl_ui.space_fi
-00000450: 6c65 6272 6f77 7365 720a 696d 706f 7274  lebrowser.import
-00000460: 2062 6c5f 7569 2e67 656e 6572 6963 5f75   bl_ui.generic_u
-00000470: 695f 6c69 7374 0a69 6d70 6f72 7420 626c  i_list.import bl
-00000480: 5f75 692e 7072 6f70 6572 7469 6573 5f6d  _ui.properties_m
-00000490: 6174 6572 6961 6c0a 696d 706f 7274 2062  aterial.import b
-000004a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000004b0: 6461 7461 5f67 7065 6e63 696c 0a69 6d70  data_gpencil.imp
-000004c0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000004d0: 7469 6573 5f64 6174 615f 626f 6e65 0a69  ties_data_bone.i
-000004e0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000004f0: 655f 696e 666f 0a69 6d70 6f72 7420 626c  e_info.import bl
-00000500: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-00000510: 7265 6573 7479 6c65 0a69 6d70 6f72 7420  reestyle.import 
-00000520: 626c 5f75 692e 7370 6163 655f 7465 7874  bl_ui.space_text
-00000530: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000540: 6f70 6572 7469 6573 5f64 6174 615f 7370  operties_data_sp
-00000550: 6561 6b65 720a 696d 706f 7274 2062 6c5f  eaker.import bl_
-00000560: 6f70 6572 6174 6f72 732e 616e 696d 0a69  operators.anim.i
-00000570: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000580: 6572 7469 6573 5f64 6174 615f 6361 6d65  erties_data_came
-00000590: 7261 0a69 6d70 6f72 7420 626c 5f75 692e  ra.import bl_ui.
-000005a0: 7370 6163 655f 636f 6e73 6f6c 650a 696d  space_console.im
-000005b0: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-000005c0: 732e 6f62 6a65 6374 0a69 6d70 6f72 7420  s.object.import 
-000005d0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000005e0: 5f64 6174 615f 656d 7074 790a 696d 706f  _data_empty.impo
-000005f0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000600: 6965 735f 6461 7461 5f63 7572 7665 0a69  ies_data_curve.i
-00000610: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000620: 6572 7469 6573 5f70 6879 7369 6373 5f66  erties_physics_f
-00000630: 6965 6c64 0a69 6d70 6f72 7420 626c 5f75  ield.import bl_u
-00000640: 692e 7072 6f70 6572 7469 6573 5f77 6f72  i.properties_wor
-00000650: 6c64 0a69 6d70 6f72 7420 626c 5f75 692e  ld.import bl_ui.
-00000660: 7072 6f70 6572 7469 6573 5f6d 6173 6b5f  properties_mask_
-00000670: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
-00000680: 5f75 692e 7072 6f70 6572 7469 6573 5f76  _ui.properties_v
-00000690: 6965 775f 6c61 7965 720a 696d 706f 7274  iew_layer.import
-000006a0: 2062 6c5f 7569 2e73 7061 6365 5f73 7072   bl_ui.space_spr
-000006b0: 6561 6473 6865 6574 0a69 6d70 6f72 7420  eadsheet.import 
-000006c0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-000006d0: 3364 5f74 6f6f 6c62 6172 0a69 6d70 6f72  3d_toolbar.impor
-000006e0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000006f0: 6573 5f72 656e 6465 720a 696d 706f 7274  es_render.import
-00000700: 2062 6c5f 7569 2e73 7061 6365 5f74 6f6f   bl_ui.space_too
-00000710: 6c73 7973 7465 6d5f 746f 6f6c 6261 720a  lsystem_toolbar.
-00000720: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000730: 7065 7274 6965 735f 636f 6e73 7472 6169  perties_constrai
-00000740: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-00000750: 7072 6f70 6572 7469 6573 5f67 7265 6173  properties_greas
-00000760: 655f 7065 6e63 696c 5f63 6f6d 6d6f 6e0a  e_pencil_common.
-00000770: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-00000780: 6f72 732e 6e6f 6465 0a69 6d70 6f72 7420  ors.node.import 
-00000790: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000007a0: 5f70 6879 7369 6373 5f66 6c75 6964 0a69  _physics_fluid.i
-000007b0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000007c0: 6572 7469 6573 5f70 6172 7469 636c 650a  erties_particle.
-000007d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000007e0: 6365 5f6f 7574 6c69 6e65 720a 696d 706f  ce_outliner.impo
-000007f0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000800: 6965 735f 6f75 7470 7574 0a69 6d70 6f72  ies_output.impor
-00000810: 7420 626c 5f6f 7065 7261 746f 7273 2e66  t bl_operators.f
-00000820: 7265 6573 7479 6c65 0a69 6d70 6f72 7420  reestyle.import 
-00000830: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000840: 5f64 6174 615f 766f 6c75 6d65 0a69 6d70  _data_volume.imp
-00000850: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000860: 2e76 6965 7733 640a 696d 706f 7274 2062  .view3d.import b
-00000870: 6c5f 7569 2e6e 6f64 655f 6164 645f 6d65  l_ui.node_add_me
-00000880: 6e75 5f67 656f 6d65 7472 790a 696d 706f  nu_geometry.impo
-00000890: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000008a0: 6965 735f 6461 7461 5f73 6861 6465 7266  ies_data_shaderf
-000008b0: 780a 696d 706f 7274 2062 6c5f 7569 2e70  x.import bl_ui.p
-000008c0: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
-000008d0: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
-000008e0: 626c 5f6f 7065 7261 746f 7273 2e63 6c69  bl_operators.cli
-000008f0: 700a 696d 706f 7274 2062 6c5f 6f70 6572  p.import bl_oper
-00000900: 6174 6f72 732e 6669 6c65 0a69 6d70 6f72  ators.file.impor
-00000910: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000920: 6573 5f70 6169 6e74 5f63 6f6d 6d6f 6e0a  es_paint_common.
-00000930: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000940: 6365 5f73 6571 7565 6e63 6572 0a69 6d70  ce_sequencer.imp
-00000950: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000960: 7469 6573 5f64 6174 615f 6c69 6768 7470  ties_data_lightp
-00000970: 726f 6265 0a69 6d70 6f72 7420 626c 5f6f  robe.import bl_o
-00000980: 7065 7261 746f 7273 2e63 6f6e 7374 7261  perators.constra
-00000990: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
-000009a0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-000009b0: 5f70 6f69 6e74 636c 6f75 640a 696d 706f  _pointcloud.impo
-000009c0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000009d0: 6965 735f 6461 7461 5f6d 6f64 6966 6965  ies_data_modifie
-000009e0: 720a 696d 706f 7274 2062 6c5f 7569 2e73  r.import bl_ui.s
-000009f0: 7061 6365 5f67 7261 7068 0a69 6d70 6f72  pace_graph.impor
-00000a00: 7420 626c 5f75 692e 7370 6163 655f 636c  t bl_ui.space_cl
-00000a10: 6970 0a69 6d70 6f72 7420 626c 5f75 692e  ip.import bl_ui.
-00000a20: 7072 6f70 6572 7469 6573 5f77 6f72 6b73  properties_works
-00000a30: 7061 6365 0a69 6d70 6f72 7420 626c 5f6f  pace.import bl_o
-00000a40: 7065 7261 746f 7273 2e75 7365 7270 7265  perators.userpre
-00000a50: 660a 0a47 656e 6572 6963 5479 7065 203d  f..GenericType =
+000000c0: 735f 7068 7973 6963 735f 636f 6d6d 6f6e  s_physics_common
+000000d0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000000e0: 6f70 6572 7469 6573 5f64 6174 615f 6d65  operties_data_me
+000000f0: 7461 6261 6c6c 0a69 6d70 6f72 7420 626c  taball.import bl
+00000100: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000110: 6174 615f 6c69 6768 740a 696d 706f 7274  ata_light.import
+00000120: 2062 6c5f 6f70 6572 6174 6f72 732e 7072   bl_operators.pr
+00000130: 6573 6574 730a 696d 706f 7274 2062 6c5f  esets.import bl_
+00000140: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000150: 7461 5f70 6f69 6e74 636c 6f75 640a 696d  ta_pointcloud.im
+00000160: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000170: 5f76 6965 7733 640a 696d 706f 7274 2062  _view3d.import b
+00000180: 6c5f 6f70 6572 6174 6f72 732e 6173 7365  l_operators.asse
+00000190: 7473 0a69 6d70 6f72 7420 626c 5f75 692e  ts.import bl_ui.
+000001a0: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
+000001b0: 6961 6c0a 696d 706f 7274 2062 6c5f 6f70  ial.import bl_op
+000001c0: 6572 6174 6f72 732e 6669 6c65 0a69 6d70  erators.file.imp
+000001d0: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+000001e0: 2e73 7072 6561 6473 6865 6574 0a69 6d70  .spreadsheet.imp
+000001f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000200: 7469 6573 5f64 6174 615f 6375 7276 650a  ties_data_curve.
+00000210: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000220: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
+00000230: 6479 6e61 6d69 6370 6169 6e74 0a69 6d70  dynamicpaint.imp
+00000240: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000250: 696e 666f 0a69 6d70 6f72 7420 626c 5f75  info.import bl_u
+00000260: 692e 7072 6f70 6572 7469 6573 5f63 6f6e  i.properties_con
+00000270: 7374 7261 696e 740a 696d 706f 7274 2062  straint.import b
+00000280: 6c5f 7569 2e73 7061 6365 5f6f 7574 6c69  l_ui.space_outli
+00000290: 6e65 720a 696d 706f 7274 2062 6c5f 7569  ner.import bl_ui
+000002a0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+000002b0: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+000002c0: 6f70 6572 6174 6f72 732e 7669 6577 3364  operators.view3d
+000002d0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000002e0: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
+000002f0: 5f73 6f66 7462 6f64 790a 696d 706f 7274  _softbody.import
+00000300: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000310: 735f 7265 6e64 6572 0a69 6d70 6f72 7420  s_render.import 
+00000320: 626c 5f75 692e 7370 6163 655f 7465 7874  bl_ui.space_text
+00000330: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000340: 6163 655f 636c 6970 0a69 6d70 6f72 7420  ace_clip.import 
+00000350: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000360: 5f70 6169 6e74 5f63 6f6d 6d6f 6e0a 696d  _paint_common.im
+00000370: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000380: 5f6e 6c61 0a69 6d70 6f72 7420 626c 5f75  _nla.import bl_u
+00000390: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+000003a0: 7369 6373 5f63 6c6f 7468 0a69 6d70 6f72  sics_cloth.impor
+000003b0: 7420 626c 5f75 692e 7370 6163 655f 6772  t bl_ui.space_gr
+000003c0: 6170 680a 696d 706f 7274 2062 6c5f 7569  aph.import bl_ui
+000003d0: 2e73 7061 6365 5f63 6f6e 736f 6c65 0a69  .space_console.i
+000003e0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000003f0: 6572 7469 6573 5f6d 6173 6b5f 636f 6d6d  erties_mask_comm
+00000400: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
+00000410: 7072 6f70 6572 7469 6573 5f77 6f72 6c64  properties_world
+00000420: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000430: 6f70 6572 7469 6573 5f64 6174 615f 6770  operties_data_gp
+00000440: 656e 6369 6c0a 696d 706f 7274 2062 6c5f  encil.import bl_
+00000450: 6f70 6572 6174 6f72 732e 6e6f 6465 0a69  operators.node.i
+00000460: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000470: 6572 7469 6573 5f64 6174 615f 656d 7074  erties_data_empt
+00000480: 790a 696d 706f 7274 2062 6c5f 7569 2e70  y.import bl_ui.p
+00000490: 726f 7065 7274 6965 735f 6461 7461 5f73  roperties_data_s
+000004a0: 7065 616b 6572 0a69 6d70 6f72 7420 626c  peaker.import bl
+000004b0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+000004c0: 5f74 6f6f 6c62 6172 0a69 6d70 6f72 7420  _toolbar.import 
+000004d0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000004e0: 5f64 6174 615f 626f 6e65 0a69 6d70 6f72  _data_bone.impor
+000004f0: 7420 626c 5f75 692e 7370 6163 655f 646f  t bl_ui.space_do
+00000500: 7065 7368 6565 740a 696d 706f 7274 2062  pesheet.import b
+00000510: 6c5f 7569 2e73 7061 6365 5f74 6f6f 6c73  l_ui.space_tools
+00000520: 7973 7465 6d5f 746f 6f6c 6261 720a 696d  ystem_toolbar.im
+00000530: 706f 7274 2062 6c5f 7569 2e6e 6f64 655f  port bl_ui.node_
+00000540: 6164 645f 6d65 6e75 5f67 656f 6d65 7472  add_menu_geometr
+00000550: 790a 696d 706f 7274 2062 6c5f 7569 2e70  y.import bl_ui.p
+00000560: 726f 7065 7274 6965 735f 6461 7461 5f6c  roperties_data_l
+00000570: 6967 6874 7072 6f62 650a 696d 706f 7274  ightprobe.import
+00000580: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000590: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
+000005a0: 6f64 795f 636f 6e73 7472 6169 6e74 0a69  ody_constraint.i
+000005b0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000005c0: 6572 7469 6573 5f64 6174 615f 6d6f 6469  erties_data_modi
+000005d0: 6669 6572 0a69 6d70 6f72 7420 626c 5f75  fier.import bl_u
+000005e0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000005f0: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
+00000600: 626c 5f6f 7065 7261 746f 7273 2e66 7265  bl_operators.fre
+00000610: 6573 7479 6c65 0a69 6d70 6f72 7420 626c  estyle.import bl
+00000620: 5f6f 7065 7261 746f 7273 2e75 7365 7270  _operators.userp
+00000630: 7265 660a 696d 706f 7274 2062 6c5f 7569  ref.import bl_ui
+00000640: 2e70 726f 7065 7274 6965 735f 6d61 7465  .properties_mate
+00000650: 7269 616c 5f67 7065 6e63 696c 0a69 6d70  rial_gpencil.imp
+00000660: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000670: 7469 6573 5f6f 626a 6563 740a 696d 706f  ties_object.impo
+00000680: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000690: 6965 735f 7669 6577 5f6c 6179 6572 0a69  ies_view_layer.i
+000006a0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000006b0: 7273 2e61 6e69 6d0a 696d 706f 7274 2062  rs.anim.import b
+000006c0: 6c5f 7569 2e73 7061 6365 5f74 6f70 6261  l_ui.space_topba
+000006d0: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
+000006e0: 726f 7065 7274 6965 735f 6f75 7470 7574  roperties_output
+000006f0: 0a69 6d70 6f72 7420 626c 5f75 692e 6765  .import bl_ui.ge
+00000700: 6e65 7269 635f 7569 5f6c 6973 740a 696d  neric_ui_list.im
+00000710: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000720: 7274 6965 735f 6772 6561 7365 5f70 656e  rties_grease_pen
+00000730: 6369 6c5f 636f 6d6d 6f6e 0a69 6d70 6f72  cil_common.impor
+00000740: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000750: 6573 5f64 6174 615f 6d65 7368 0a69 6d70  es_data_mesh.imp
+00000760: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000770: 7374 6174 7573 6261 720a 696d 706f 7274  statusbar.import
+00000780: 2062 6c5f 7569 2e73 7061 6365 5f74 696d   bl_ui.space_tim
+00000790: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
+000007a0: 726f 7065 7274 6965 735f 7061 7274 6963  roperties_partic
+000007b0: 6c65 0a69 6d70 6f72 7420 626c 5f75 692e  le.import bl_ui.
+000007c0: 7370 6163 655f 7573 6572 7072 6566 0a69  space_userpref.i
+000007d0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000007e0: 6572 7469 6573 5f64 6174 615f 7368 6164  erties_data_shad
+000007f0: 6572 6678 0a69 6d70 6f72 7420 626c 5f75  erfx.import bl_u
+00000800: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000810: 615f 6c61 7474 6963 650a 696d 706f 7274  a_lattice.import
+00000820: 2062 6c5f 7569 2e73 7061 6365 5f73 6571   bl_ui.space_seq
+00000830: 7565 6e63 6572 0a69 6d70 6f72 7420 626c  uencer.import bl
+00000840: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000850: 6174 615f 6375 7276 6573 0a69 6d70 6f72  ata_curves.impor
+00000860: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000870: 6573 5f70 6879 7369 6373 5f66 6965 6c64  es_physics_field
+00000880: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000890: 6163 655f 7370 7265 6164 7368 6565 740a  ace_spreadsheet.
+000008a0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000008b0: 6f72 732e 636c 6970 0a69 6d70 6f72 7420  ors.clip.import 
+000008c0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000008d0: 5f63 6f6c 6c65 6374 696f 6e0a 696d 706f  _collection.impo
+000008e0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000008f0: 6965 735f 7465 7874 7572 650a 696d 706f  ies_texture.impo
+00000900: 7274 2062 6c5f 7569 2e73 7061 6365 5f69  rt bl_ui.space_i
+00000910: 6d61 6765 0a69 6d70 6f72 7420 626c 5f6f  mage.import bl_o
+00000920: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
+00000930: 7274 2062 6c5f 7569 2e73 7061 6365 5f74  rt bl_ui.space_t
+00000940: 6f6f 6c73 7973 7465 6d5f 636f 6d6d 6f6e  oolsystem_common
+00000950: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000960: 6f70 6572 7469 6573 5f77 6f72 6b73 7061  operties_workspa
+00000970: 6365 0a69 6d70 6f72 7420 626c 5f75 692e  ce.import bl_ui.
+00000980: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000990: 6172 6d61 7475 7265 0a69 6d70 6f72 7420  armature.import 
+000009a0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000009b0: 5f70 6879 7369 6373 5f66 6c75 6964 0a69  _physics_fluid.i
+000009c0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+000009d0: 655f 6e6f 6465 0a69 6d70 6f72 7420 626c  e_node.import bl
+000009e0: 5f75 692e 7370 6163 655f 7072 6f70 6572  _ui.space_proper
+000009f0: 7469 6573 0a69 6d70 6f72 7420 626c 5f75  ties.import bl_u
+00000a00: 692e 7072 6f70 6572 7469 6573 5f73 6365  i.properties_sce
+00000a10: 6e65 0a69 6d70 6f72 7420 626c 5f6f 7065  ne.import bl_ope
+00000a20: 7261 746f 7273 2e6f 626a 6563 740a 696d  rators.object.im
+00000a30: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000a40: 7274 6965 735f 6461 7461 5f63 616d 6572  rties_data_camer
+00000a50: 610a 0a47 656e 6572 6963 5479 7065 203d  a..GenericType =
 00000a60: 2074 7970 696e 672e 5479 7065 5661 7228   typing.TypeVar(
 00000a70: 2247 656e 6572 6963 5479 7065 2229 0a0a  "GenericType")..
-00000a80: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
-00000a90: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
-00000aa0: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
-00000ab0: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
-00000ac0: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
-00000ad0: 2027 2727 0a0a 2020 2020 6964 5f64 6174   '''..    id_dat
-00000ae0: 6120 3d20 4e6f 6e65 0a20 2020 2027 2727  a = None.    '''
-00000af0: 2054 6865 2060 6270 792e 7479 7065 732e   The `bpy.types.
-00000b00: 4944 6020 6f62 6a65 6374 2074 6869 7320  ID` object this 
-00000b10: 6461 7461 626c 6f63 6b20 6973 2066 726f  datablock is fro
-00000b20: 6d20 6f72 204e 6f6e 652c 2028 6e6f 7420  m or None, (not 
-00000b30: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
-00000b40: 6c20 6461 7461 2074 7970 6573 2927 2727  l data types)'''
-00000b50: 0a0a 2020 2020 6465 6620 6173 5f70 6f69  ..    def as_poi
-00000b60: 6e74 6572 2873 656c 6629 202d 3e20 696e  nter(self) -> in
-00000b70: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
-00000b80: 6574 7572 6e73 2074 6865 206d 656d 6f72  eturns the memor
-00000b90: 7920 6164 6472 6573 7320 7768 6963 6820  y address which 
-00000ba0: 686f 6c64 7320 6120 706f 696e 7465 7220  holds a pointer 
-00000bb0: 746f 2042 6c65 6e64 6572 2773 2069 6e74  to Blender's int
-00000bc0: 6572 6e61 6c20 6461 7461 0a0a 2020 2020  ernal data..    
-00000bd0: 2020 2020 3a72 7479 7065 3a20 696e 740a      :rtype: int.
-00000be0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000bf0: 2069 6e74 2028 6d65 6d6f 7279 2061 6464   int (memory add
-00000c00: 7265 7373 292e 0a20 2020 2020 2020 2027  ress)..        '
-00000c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00000c20: 0a20 2020 2064 6566 2064 7269 7665 725f  .    def driver_
-00000c30: 6164 6428 7365 6c66 2c0a 2020 2020 2020  add(self,.      
-00000c40: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00000c50: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00000c60: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
-00000c70: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00000c80: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00000c90: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
-00000ca0: 2027 4643 7572 7665 273a 0a20 2020 2020   'FCurve':.     
-00000cb0: 2020 2027 2727 2041 6464 7320 6472 6976     ''' Adds driv
-00000cc0: 6572 2873 2920 746f 2074 6865 2067 6976  er(s) to the giv
-00000cd0: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
-00000ce0: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
-00000cf0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
-00000d00: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
-00000d10: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
-00000d20: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
-00000d30: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
-00000d40: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
-00000d50: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00000d60: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00000d70: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
-00000d80: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00000d90: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
-00000da0: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
-00000db0: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
-00000dc0: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
-00000dd0: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
-00000de0: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
-00000df0: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
-00000e00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00000e10: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
-00000e20: 7479 7065 3a20 2746 4375 7276 6527 0a20  type: 'FCurve'. 
-00000e30: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00000e40: 5468 6520 6472 6976 6572 2873 2920 6164  The driver(s) ad
-00000e50: 6465 642e 0a20 2020 2020 2020 2027 2727  ded..        '''
-00000e60: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00000e70: 2020 2064 6566 2064 7269 7665 725f 7265     def driver_re
-00000e80: 6d6f 7665 2873 656c 662c 0a20 2020 2020  move(self,.     
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ea0: 2070 6174 683a 2074 7970 696e 672e 4f70   path: typing.Op
-00000eb0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
-00000ee0: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
-00000ef0: 202d 3129 202d 3e20 626f 6f6c 3a0a 2020   -1) -> bool:.  
-00000f00: 2020 2020 2020 2727 2720 5265 6d6f 7665        ''' Remove
-00000f10: 2064 7269 7665 7228 7329 2066 726f 6d20   driver(s) from 
-00000f20: 7468 6520 6769 7665 6e20 7072 6f70 6572  the given proper
-00000f30: 7479 0a0a 2020 2020 2020 2020 3a70 6172  ty..        :par
-00000f40: 616d 2070 6174 683a 2070 6174 6820 746f  am path: path to
-00000f50: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
-00000f60: 2064 7269 7665 2c20 616e 616c 6f67 6f75   drive, analogou
-00000f70: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
-00000f80: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
-00000f90: 2020 2020 203a 7479 7065 2070 6174 683a       :type path:
-00000fa0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00000fb0: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
-00000fc0: 6172 616d 2069 6e64 6578 3a20 6172 7261  aram index: arra
-00000fd0: 7920 696e 6465 7820 6f66 2074 6865 2070  y index of the p
-00000fe0: 726f 7065 7274 7920 6472 6976 652e 2044  roperty drive. D
-00000ff0: 6566 6175 6c74 7320 746f 202d 3120 666f  efaults to -1 fo
-00001000: 7220 616c 6c20 696e 6469 6365 7320 6f72  r all indices or
-00001010: 2061 2073 696e 676c 6520 6368 616e 6e65   a single channe
-00001020: 6c20 6966 2074 6865 2070 726f 7065 7274  l if the propert
-00001030: 7920 6973 206e 6f74 2061 6e20 6172 7261  y is not an arra
-00001040: 792e 0a20 2020 2020 2020 203a 7479 7065  y..        :type
-00001050: 2069 6e64 6578 3a20 7479 7069 6e67 2e4f   index: typing.O
-00001060: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
-00001070: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00001080: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00001090: 6e3a 2053 7563 6365 7373 206f 6620 6472  n: Success of dr
-000010a0: 6976 6572 2072 656d 6f76 616c 2e0a 2020  iver removal..  
-000010b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000010c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-000010d0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
-000010e0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
-000010f0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
-00001100: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00001110: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
-00001120: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
-00001130: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
-00001140: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
-00001150: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00001160: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
-00001170: 6173 7369 676e 6564 2074 6f20 6b65 7920  assigned to key 
-00001180: 6f72 2064 6566 6175 6c74 2077 6865 6e20  or default when 
-00001190: 6e6f 7420 666f 756e 6420 286d 6174 6368  not found (match
-000011a0: 6573 2050 7974 686f 6e27 7320 6469 6374  es Python's dict
-000011b0: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
-000011c0: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-000011d0: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
-000011e0: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
-000011f0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00001200: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
-00001210: 7274 792e 0a20 2020 2020 2020 203a 7479  rty..        :ty
-00001220: 7065 206b 6579 3a20 7479 7069 6e67 2e4f  pe key: typing.O
-00001230: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
-00001240: 2020 2020 203a 7061 7261 6d20 6465 6661       :param defa
-00001250: 756c 743a 204f 7074 696f 6e61 6c20 6172  ult: Optional ar
-00001260: 6775 6d65 6e74 2066 6f72 2074 6865 2076  gument for the v
-00001270: 616c 7565 2074 6f20 7265 7475 726e 2069  alue to return i
-00001280: 6620 2a6b 6579 2a20 6973 206e 6f74 2066  f *key* is not f
-00001290: 6f75 6e64 2e0a 2020 2020 2020 2020 3a74  ound..        :t
-000012a0: 7970 6520 6465 6661 756c 743a 2074 7970  ype default: typ
-000012b0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-000012c0: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
-000012d0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-000012e0: 730a 0a20 2020 2064 6566 2069 645f 7072  s..    def id_pr
-000012f0: 6f70 6572 7469 6573 5f63 6c65 6172 2873  operties_clear(s
-00001300: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
-00001310: 2720 0a0a 2020 2020 2020 2020 2727 270a  ' ..        '''.
-00001320: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00001330: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
-00001340: 6965 735f 656e 7375 7265 2873 656c 6629  ies_ensure(self)
-00001350: 202d 3e20 7479 7069 6e67 2e41 6e79 3a0a   -> typing.Any:.
-00001360: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00001370: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00001380: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
-00001390: 203a 7265 7475 726e 3a20 7468 6520 7061   :return: the pa
-000013a0: 7265 6e74 2067 726f 7570 2066 6f72 2061  rent group for a
-000013b0: 6e20 524e 4120 7374 7275 6374 2773 2063  n RNA struct's c
-000013c0: 7573 746f 6d20 4944 5072 6f70 6572 7469  ustom IDProperti
-000013d0: 6573 2e0a 2020 2020 2020 2020 2727 270a  es..        '''.
-000013e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000013f0: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
-00001400: 6965 735f 7569 2873 656c 662c 206b 6579  ies_ui(self, key
-00001410: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001420: 6c5b 7479 7069 6e67 2e41 6e79 5d29 202d  l[typing.Any]) -
-00001430: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
-00001440: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
-00001450: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00001460: 2053 7472 696e 6720 6e61 6d65 206f 6620   String name of 
-00001470: 7468 6520 7072 6f70 6572 7479 2e0a 2020  the property..  
-00001480: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00001490: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000014a0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
-000014b0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
-000014c0: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
-000014d0: 3a72 6574 7572 6e3a 2052 6574 7572 6e20  :return: Return 
-000014e0: 616e 206f 626a 6563 7420 7573 6564 2074  an object used t
-000014f0: 6f20 6d61 6e61 6765 2061 6e20 4944 5072  o manage an IDPr
-00001500: 6f70 6572 7479 2773 2055 4920 6461 7461  operty's UI data
-00001510: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00001520: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001530: 6465 6620 6973 5f70 726f 7065 7274 795f  def is_property_
-00001540: 6869 6464 656e 2873 656c 662c 2070 726f  hidden(self, pro
-00001550: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
-00001560: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
-00001570: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
-00001580: 6973 2068 6964 6465 6e2e 0a0a 2020 2020  is hidden...    
-00001590: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-000015a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000015b0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
-000015c0: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
-000015d0: 656e 2e0a 2020 2020 2020 2020 2727 270a  en..        '''.
-000015e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000015f0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
-00001600: 795f 6f76 6572 7269 6461 626c 655f 6c69  y_overridable_li
-00001610: 6272 6172 7928 7365 6c66 2c20 7072 6f70  brary(self, prop
-00001620: 6572 7479 2920 2d3e 2062 6f6f 6c3a 0a20  erty) -> bool:. 
-00001630: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
-00001640: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
-00001650: 7320 6f76 6572 7269 6461 626c 652e 0a0a  s overridable...
-00001660: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00001670: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
-00001680: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
-00001690: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
-000016a0: 6f76 6572 7269 6461 626c 652e 0a20 2020  overridable..   
-000016b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000016c0: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-000016d0: 735f 7072 6f70 6572 7479 5f72 6561 646f  s_property_reado
-000016e0: 6e6c 7928 7365 6c66 2c20 7072 6f70 6572  nly(self, proper
-000016f0: 7479 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ty) -> bool:.   
-00001700: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
-00001710: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
-00001720: 7265 6164 6f6e 6c79 2e0a 0a20 2020 2020  readonly...     
-00001730: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00001740: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00001750: 2054 7275 6520 7768 656e 2074 6865 2070   True when the p
-00001760: 726f 7065 7274 7920 6973 2072 6561 646f  roperty is reado
-00001770: 6e6c 7920 286e 6f74 2077 7269 7461 626c  nly (not writabl
-00001780: 6529 2e0a 2020 2020 2020 2020 2727 270a  e)..        '''.
-00001790: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000017a0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
-000017b0: 795f 7365 7428 7365 6c66 2c20 7072 6f70  y_set(self, prop
-000017c0: 6572 7479 2c0a 2020 2020 2020 2020 2020  erty,.          
-000017d0: 2020 2020 2020 2020 2020 2020 2020 6768                gh
-000017e0: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
-000017f0: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
-00001800: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
-00001810: 2020 2020 2727 2720 4368 6563 6b20 6966      ''' Check if
-00001820: 2061 2070 726f 7065 7274 7920 6973 2073   a property is s
-00001830: 6574 2c20 7573 6520 666f 7220 7465 7374  et, use for test
-00001840: 696e 6720 6f70 6572 6174 6f72 2070 726f  ing operator pro
-00001850: 7065 7274 6965 732e 0a0a 2020 2020 2020  perties...      
-00001860: 2020 3a70 6172 616d 2067 686f 7374 3a20    :param ghost: 
-00001870: 5573 6564 2066 6f72 206f 7065 7261 746f  Used for operato
-00001880: 7273 2074 6861 7420 7265 2d72 756e 2077  rs that re-run w
-00001890: 6974 6820 7072 6576 696f 7573 2073 6574  ith previous set
-000018a0: 7469 6e67 732e 2049 6e20 7468 6973 2063  tings. In this c
-000018b0: 6173 6520 7468 6520 7072 6f70 6572 7479  ase the property
-000018c0: 2069 7320 6e6f 7420 6d61 726b 6564 2061   is not marked a
-000018d0: 7320 7365 742c 2079 6574 2074 6865 2076  s set, yet the v
-000018e0: 616c 7565 2066 726f 6d20 7468 6520 7072  alue from the pr
-000018f0: 6576 696f 7573 2065 7865 6375 7469 6f6e  evious execution
-00001900: 2069 7320 7573 6564 2e20 496e 2072 6172   is used. In rar
-00001910: 6520 6361 7365 7320 796f 7520 6d61 7920  e cases you may 
-00001920: 7761 6e74 2074 6f20 7365 7420 7468 6973  want to set this
-00001930: 206f 7074 696f 6e20 746f 2066 616c 7365   option to false
-00001940: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00001950: 6768 6f73 743a 2074 7970 696e 672e 4f70  ghost: typing.Op
-00001960: 7469 6f6e 616c 5b62 6f6f 6c5d 0a20 2020  tional[bool].   
-00001970: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00001980: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00001990: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
-000019a0: 2070 726f 7065 7274 7920 6861 7320 6265   property has be
-000019b0: 656e 2073 6574 2e0a 2020 2020 2020 2020  en set..        
-000019c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000019d0: 0a0a 2020 2020 6465 6620 6974 656d 7328  ..    def items(
-000019e0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
-000019f0: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
-00001a00: 2052 6574 7572 6e73 2074 6865 2069 7465   Returns the ite
-00001a10: 6d73 206f 6620 7468 6973 206f 626a 6563  ms of this objec
-00001a20: 7473 2063 7573 746f 6d20 7072 6f70 6572  ts custom proper
-00001a30: 7469 6573 2028 6d61 7463 6865 7320 5079  ties (matches Py
-00001a40: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
-00001a50: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
-00001a60: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
-00001a70: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-00001a80: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
-00001a90: 2020 3a72 6574 7572 6e3a 2063 7573 746f    :return: custo
-00001aa0: 6d20 7072 6f70 6572 7479 206b 6579 2c20  m property key, 
-00001ab0: 7661 6c75 6520 7061 6972 732e 0a20 2020  value pairs..   
-00001ac0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00001ad0: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
-00001ae0: 6579 6672 616d 655f 6465 6c65 7465 280a  eyframe_delete(.
-00001af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001b00: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00001b10: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
-00001b20: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
-00001b30: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00000a80: 0a63 6c61 7373 2062 7079 5f70 726f 705f  .class bpy_prop_
+00000a90: 636f 6c6c 6563 7469 6f6e 2874 7970 696e  collection(typin
+00000aa0: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
+00000ab0: 6354 7970 655d 293a 0a20 2020 2027 2727  cType]):.    '''
+00000ac0: 2062 7569 6c74 2d69 6e20 636c 6173 7320   built-in class 
+00000ad0: 7573 6564 2066 6f72 2061 6c6c 2063 6f6c  used for all col
+00000ae0: 6c65 6374 696f 6e73 2e0a 2020 2020 2727  lections..    ''
+00000af0: 270a 0a20 2020 2064 6566 2066 696e 6428  '..    def find(
+00000b00: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00000b10: 672e 4f70 7469 6f6e 616c 5b73 7472 5d29  g.Optional[str])
+00000b20: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00000b30: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
+00000b40: 2069 6e64 6578 206f 6620 6120 6b65 7920   index of a key 
+00000b50: 696e 2061 2063 6f6c 6c65 6374 696f 6e20  in a collection 
+00000b60: 6f72 202d 3120 7768 656e 206e 6f74 2066  or -1 when not f
+00000b70: 6f75 6e64 2028 6d61 7463 6865 7320 5079  ound (matches Py
+00000b80: 7468 6f6e 2773 2073 7472 696e 6720 6669  thon's string fi
+00000b90: 6e64 2066 756e 6374 696f 6e20 6f66 2074  nd function of t
+00000ba0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+00000bb0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00000bc0: 6579 3a20 5468 6520 6964 656e 7469 6669  ey: The identifi
+00000bd0: 6572 2066 6f72 2074 6865 2063 6f6c 6c65  er for the colle
+00000be0: 6374 696f 6e20 6d65 6d62 6572 2e0a 2020  ction member..  
+00000bf0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00000c00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00000c10: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
+00000c20: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00000c30: 2020 3a72 6574 7572 6e3a 2069 6e64 6578    :return: index
+00000c40: 206f 6620 7468 6520 6b65 792e 0a20 2020   of the key..   
+00000c50: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00000c60: 2070 6173 730a 0a20 2020 2064 6566 2066   pass..    def f
+00000c70: 6f72 6561 6368 5f67 6574 2873 656c 662c  oreach_get(self,
+00000c80: 2061 7474 722c 2073 6571 293a 0a20 2020   attr, seq):.   
+00000c90: 2020 2020 2027 2727 2054 6869 7320 6973       ''' This is
+00000ca0: 2061 2066 756e 6374 696f 6e20 746f 2067   a function to g
+00000cb0: 6976 6520 6661 7374 2061 6363 6573 7320  ive fast access 
+00000cc0: 746f 2061 7474 7269 6275 7465 7320 7769  to attributes wi
+00000cd0: 7468 696e 2061 2063 6f6c 6c65 6374 696f  thin a collectio
+00000ce0: 6e2e 204f 6e6c 7920 776f 726b 7320 666f  n. Only works fo
+00000cf0: 7220 2762 6173 6963 2074 7970 6527 2070  r 'basic type' p
+00000d00: 726f 7065 7274 6965 7320 2862 6f6f 6c2c  roperties (bool,
+00000d10: 2069 6e74 2061 6e64 2066 6c6f 6174 2921   int and float)!
+00000d20: 204d 756c 7469 2d64 696d 656e 7369 6f6e   Multi-dimension
+00000d30: 616c 2061 7272 6179 7320 286c 696b 6520  al arrays (like 
+00000d40: 6172 7261 7920 6f66 2076 6563 746f 7273  array of vectors
+00000d50: 2920 7769 6c6c 2062 6520 666c 6174 7465  ) will be flatte
+00000d60: 6e65 6420 696e 746f 2073 6571 2e0a 0a20  ned into seq... 
+00000d70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00000d80: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00000d90: 2066 6f72 6561 6368 5f73 6574 2873 656c   foreach_set(sel
+00000da0: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):. 
+00000db0: 2020 2020 2020 2027 2727 2054 6869 7320         ''' This 
+00000dc0: 6973 2061 2066 756e 6374 696f 6e20 746f  is a function to
+00000dd0: 2067 6976 6520 6661 7374 2061 6363 6573   give fast acces
+00000de0: 7320 746f 2061 7474 7269 6275 7465 7320  s to attributes 
+00000df0: 7769 7468 696e 2061 2063 6f6c 6c65 6374  within a collect
+00000e00: 696f 6e2e 204f 6e6c 7920 776f 726b 7320  ion. Only works 
+00000e10: 666f 7220 2762 6173 6963 2074 7970 6527  for 'basic type'
+00000e20: 2070 726f 7065 7274 6965 7320 2862 6f6f   properties (boo
+00000e30: 6c2c 2069 6e74 2061 6e64 2066 6c6f 6174  l, int and float
+00000e40: 2921 2073 6571 206d 7573 7420 6265 2075  )! seq must be u
+00000e50: 6e69 2d64 696d 656e 7369 6f6e 616c 2c20  ni-dimensional, 
+00000e60: 6d75 6c74 692d 6469 6d65 6e73 696f 6e61  multi-dimensiona
+00000e70: 6c20 6172 7261 7973 2028 6c69 6b65 2061  l arrays (like a
+00000e80: 7272 6179 206f 6620 7665 6374 6f72 7329  rray of vectors)
+00000e90: 2077 696c 6c20 6265 2072 652d 6372 6561   will be re-crea
+00000ea0: 7465 6420 6672 6f6d 2069 742e 0a0a 2020  ted from it...  
+00000eb0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00000ec0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00000ed0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
+00000ee0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
+00000ef0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
+00000f00: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00000f10: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00000f20: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00000f30: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+00000f40: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+00000f50: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00000f60: 6974 656d 2061 7373 6967 6e65 6420 746f  item assigned to
+00000f70: 206b 6579 206f 7220 6465 6661 756c 7420   key or default 
+00000f80: 7768 656e 206e 6f74 2066 6f75 6e64 2028  when not found (
+00000f90: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
+00000fa0: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
+00000fb0: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
+00000fc0: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
+00000fd0: 203a 7061 7261 6d20 6b65 793a 2054 6865   :param key: The
+00000fe0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
+00000ff0: 7468 6520 636f 6c6c 6563 7469 6f6e 206d  the collection m
+00001000: 656d 6265 722e 0a20 2020 2020 2020 203a  ember..        :
+00001010: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
+00001020: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00001030: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
+00001040: 6661 756c 743a 204f 7074 696f 6e61 6c20  fault: Optional 
+00001050: 6172 6775 6d65 6e74 2066 6f72 2074 6865  argument for the
+00001060: 2076 616c 7565 2074 6f20 7265 7475 726e   value to return
+00001070: 2069 6620 2a6b 6579 2a20 6973 206e 6f74   if *key* is not
+00001080: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
+00001090: 3a74 7970 6520 6465 6661 756c 743a 2074  :type default: t
+000010a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000010b0: 7970 696e 672e 416e 795d 0a20 2020 2020  yping.Any].     
+000010c0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+000010d0: 6173 730a 0a20 2020 2064 6566 2069 7465  ass..    def ite
+000010e0: 6d73 2873 656c 6629 202d 3e20 7479 7069  ms(self) -> typi
+000010f0: 6e67 2e4c 6973 743a 0a20 2020 2020 2020  ng.List:.       
+00001100: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
+00001110: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
+00001120: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
+00001130: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
+00001140: 6f6e 2773 2064 6963 742e 6974 656d 7328  on's dict.items(
+00001150: 2920 6675 6e63 7469 6f6e 616c 6974 7929  ) functionality)
+00001160: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+00001170: 653a 2074 7970 696e 672e 4c69 7374 0a20  e: typing.List. 
+00001180: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001190: 286b 6579 2c20 7661 6c75 6529 2070 6169  (key, value) pai
+000011a0: 7273 2066 6f72 2065 6163 6820 6d65 6d62  rs for each memb
+000011b0: 6572 206f 6620 7468 6973 2063 6f6c 6c65  er of this colle
+000011c0: 6374 696f 6e2e 0a20 2020 2020 2020 2027  ction..        '
+000011d0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000011e0: 0a20 2020 2064 6566 206b 6579 7328 7365  .    def keys(se
+000011f0: 6c66 2920 2d3e 2074 7970 696e 672e 4c69  lf) -> typing.Li
+00001200: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
+00001210: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
+00001220: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
+00001230: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
+00001240: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
+00001250: 6f6e 2773 2064 6963 742e 6b65 7973 2829  on's dict.keys()
+00001260: 2066 756e 6374 696f 6e61 6c69 7479 292e   functionality).
+00001270: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00001280: 3a20 7479 7069 6e67 2e4c 6973 745b 7374  : typing.List[st
+00001290: 725d 0a20 2020 2020 2020 203a 7265 7475  r].        :retu
+000012a0: 726e 3a20 7468 6520 6964 656e 7469 6669  rn: the identifi
+000012b0: 6572 7320 666f 7220 6561 6368 206d 656d  ers for each mem
+000012c0: 6265 7220 6f66 2074 6869 7320 636f 6c6c  ber of this coll
+000012d0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+000012e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000012f0: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
+00001300: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+00001310: 2e4c 6973 743a 0a20 2020 2020 2020 2027  .List:.        '
+00001320: 2727 2052 6574 7572 6e20 7468 6520 7661  '' Return the va
+00001330: 6c75 6573 206f 6620 636f 6c6c 6563 7469  lues of collecti
+00001340: 6f6e 2028 6d61 7463 6869 6e67 2050 7974  on (matching Pyt
+00001350: 686f 6e27 7320 6469 6374 2e76 616c 7565  hon's dict.value
+00001360: 7328 2920 6675 6e63 7469 6f6e 616c 6974  s() functionalit
+00001370: 7929 2e0a 0a20 2020 2020 2020 203a 7274  y)...        :rt
+00001380: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
+00001390: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000013a0: 3a20 7468 6520 6d65 6d62 6572 7320 6f66  : the members of
+000013b0: 2074 6869 7320 636f 6c6c 6563 7469 6f6e   this collection
+000013c0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+000013d0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000013e0: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
+000013f0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00001400: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00001410: 5d29 202d 3e20 2747 656e 6572 6963 5479  ]) -> 'GenericTy
+00001420: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
+00001430: 200a 0a20 2020 2020 2020 203a 7061 7261   ..        :para
+00001440: 6d20 6b65 793a 200a 2020 2020 2020 2020  m key: .        
+00001450: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+00001460: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00001470: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
+00001480: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
+00001490: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+000014a0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000014b0: 6620 5f5f 7365 7469 7465 6d5f 5f28 7365  f __setitem__(se
+000014c0: 6c66 2c20 6b65 793a 2074 7970 696e 672e  lf, key: typing.
+000014d0: 556e 696f 6e5b 696e 742c 2073 7472 5d2c  Union[int, str],
+000014e0: 2076 616c 7565 3a20 2747 656e 6572 6963   value: 'Generic
+000014f0: 5479 7065 2729 3a0a 2020 2020 2020 2020  Type'):.        
+00001500: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+00001510: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+00001520: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00001530: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00001540: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+00001550: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
+00001560: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
+00001570: 2027 4765 6e65 7269 6354 7970 6527 0a20   'GenericType'. 
+00001580: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001590: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000015a0: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
+000015b0: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
+000015c0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
+000015d0: 2d3e 2027 4765 6e65 7269 6354 7970 6527  -> 'GenericType'
+000015e0: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
+000015f0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00001600: 6579 3a20 0a20 2020 2020 2020 203a 7479  ey: .        :ty
+00001610: 7065 206b 6579 3a20 7479 7069 6e67 2e55  pe key: typing.U
+00001620: 6e69 6f6e 5b69 6e74 2c20 7374 725d 0a20  nion[int, str]. 
+00001630: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
+00001640: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
+00001650: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001660: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+00001670: 5f69 7465 725f 5f28 7365 6c66 2920 2d3e  _iter__(self) ->
+00001680: 2074 7970 696e 672e 4974 6572 6174 6f72   typing.Iterator
+00001690: 5b27 4765 6e65 7269 6354 7970 6527 5d3a  ['GenericType']:
+000016a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000016b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+000016c0: 7970 696e 672e 4974 6572 6174 6f72 5b27  yping.Iterator['
+000016d0: 4765 6e65 7269 6354 7970 6527 5d0a 2020  GenericType'].  
+000016e0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000016f0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00001700: 5f5f 6e65 7874 5f5f 2873 656c 6629 202d  __next__(self) -
+00001710: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
+00001720: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00001730: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
+00001740: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
+00001750: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001760: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+00001770: 5f6c 656e 5f5f 2873 656c 6629 202d 3e20  _len__(self) -> 
+00001780: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
+00001790: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
+000017a0: 653a 2069 6e74 0a20 2020 2020 2020 2027  e: int.        '
+000017b0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000017c0: 0a0a 636c 6173 7320 6270 795f 7374 7275  ..class bpy_stru
+000017d0: 6374 3a0a 2020 2020 2727 2720 6275 696c  ct:.    ''' buil
+000017e0: 742d 696e 2062 6173 6520 636c 6173 7320  t-in base class 
+000017f0: 666f 7220 616c 6c20 636c 6173 7365 7320  for all classes 
+00001800: 696e 2062 7079 2e74 7970 6573 2e0a 2020  in bpy.types..  
+00001810: 2020 2727 270a 0a20 2020 2069 645f 6461    '''..    id_da
+00001820: 7461 203d 204e 6f6e 650a 2020 2020 2727  ta = None.    ''
+00001830: 2720 5468 6520 6062 7079 2e74 7970 6573  ' The `bpy.types
+00001840: 2e49 4460 206f 626a 6563 7420 7468 6973  .ID` object this
+00001850: 2064 6174 6162 6c6f 636b 2069 7320 6672   datablock is fr
+00001860: 6f6d 206f 7220 4e6f 6e65 2c20 286e 6f74  om or None, (not
+00001870: 2061 7661 696c 6162 6c65 2066 6f72 2061   available for a
+00001880: 6c6c 2064 6174 6120 7479 7065 7329 2727  ll data types)''
+00001890: 270a 0a20 2020 2064 6566 2061 735f 706f  '..    def as_po
+000018a0: 696e 7465 7228 7365 6c66 2920 2d3e 2069  inter(self) -> i
+000018b0: 6e74 3a0a 2020 2020 2020 2020 2727 2720  nt:.        ''' 
+000018c0: 5265 7475 726e 7320 7468 6520 6d65 6d6f  Returns the memo
+000018d0: 7279 2061 6464 7265 7373 2077 6869 6368  ry address which
+000018e0: 2068 6f6c 6473 2061 2070 6f69 6e74 6572   holds a pointer
+000018f0: 2074 6f20 426c 656e 6465 7227 7320 696e   to Blender's in
+00001900: 7465 726e 616c 2064 6174 610a 0a20 2020  ternal data..   
+00001910: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+00001920: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00001930: 3a20 696e 7420 286d 656d 6f72 7920 6164  : int (memory ad
+00001940: 6472 6573 7329 2e0a 2020 2020 2020 2020  dress)..        
+00001950: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00001960: 0a0a 2020 2020 6465 6620 6472 6976 6572  ..    def driver
+00001970: 5f61 6464 2873 656c 662c 0a20 2020 2020  _add(self,.     
+00001980: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00001990: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
+000019a0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
+000019b0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+000019c0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+000019d0: 6e61 6c5b 696e 745d 203d 202d 3129 202d  nal[int] = -1) -
+000019e0: 3e20 2746 4375 7276 6527 3a0a 2020 2020  > 'FCurve':.    
+000019f0: 2020 2020 2727 2720 4164 6473 2064 7269      ''' Adds dri
+00001a00: 7665 7228 7329 2074 6f20 7468 6520 6769  ver(s) to the gi
+00001a10: 7665 6e20 7072 6f70 6572 7479 0a0a 2020  ven property..  
+00001a20: 2020 2020 2020 3a70 6172 616d 2070 6174        :param pat
+00001a30: 683a 2070 6174 6820 746f 2074 6865 2070  h: path to the p
+00001a40: 726f 7065 7274 7920 746f 2064 7269 7665  roperty to drive
+00001a50: 2c20 616e 616c 6f67 6f75 7320 746f 2074  , analogous to t
+00001a60: 6865 2066 6375 7276 6527 7320 6461 7461  he fcurve's data
+00001a70: 2070 6174 682e 0a20 2020 2020 2020 203a   path..        :
+00001a80: 7479 7065 2070 6174 683a 2074 7970 696e  type path: typin
+00001a90: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00001aa0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00001ab0: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
+00001ac0: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
+00001ad0: 7920 6472 6976 652e 2044 6566 6175 6c74  y drive. Default
+00001ae0: 7320 746f 202d 3120 666f 7220 616c 6c20  s to -1 for all 
+00001af0: 696e 6469 6365 7320 6f72 2061 2073 696e  indices or a sin
+00001b00: 676c 6520 6368 616e 6e65 6c20 6966 2074  gle channel if t
+00001b10: 6865 2070 726f 7065 7274 7920 6973 206e  he property is n
+00001b20: 6f74 2061 6e20 6172 7261 792e 0a20 2020  ot an array..   
+00001b30: 2020 2020 203a 7479 7065 2069 6e64 6578       :type index
 00001b40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001b50: 6c5b 696e 745d 203d 202d 312c 0a20 2020  l[int] = -1,.   
-00001b60: 2020 2020 2020 2020 2066 7261 6d65 3a20           frame: 
-00001b70: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001b80: 666c 6f61 745d 203d 2027 6270 792e 636f  float] = 'bpy.co
-00001b90: 6e74 6578 742e 7363 656e 652e 6672 616d  ntext.scene.fram
-00001ba0: 655f 6375 7272 656e 7427 2c0a 2020 2020  e_current',.    
-00001bb0: 2020 2020 2020 2020 6772 6f75 703a 2074          group: t
-00001bc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00001bd0: 7472 5d20 3d20 2222 2920 2d3e 2062 6f6f  tr] = "") -> boo
-00001be0: 6c3a 0a20 2020 2020 2020 2027 2727 2052  l:.        ''' R
-00001bf0: 656d 6f76 6520 6120 6b65 7966 7261 6d65  emove a keyframe
-00001c00: 2066 726f 6d20 7468 6973 2070 726f 7065   from this prope
-00001c10: 7274 6965 7320 6663 7572 7665 2e0a 0a20  rties fcurve... 
-00001c20: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
-00001c30: 7461 5f70 6174 683a 2070 6174 6820 746f  ta_path: path to
-00001c40: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
-00001c50: 2072 656d 6f76 6520 6120 6b65 792c 2061   remove a key, a
-00001c60: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
-00001c70: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
-00001c80: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
-00001c90: 6520 6461 7461 5f70 6174 683a 2074 7970  e data_path: typ
-00001ca0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00001cb0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-00001cc0: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
-00001cd0: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
-00001ce0: 7274 7920 746f 2072 656d 6f76 6520 6120  rty to remove a 
-00001cf0: 6b65 792e 2044 6566 6175 6c74 7320 746f  key. Defaults to
-00001d00: 202d 3120 7265 6d6f 7669 6e67 2061 6c6c   -1 removing all
-00001d10: 2069 6e64 6963 6573 206f 7220 6120 7369   indices or a si
-00001d20: 6e67 6c65 2063 6861 6e6e 656c 2069 6620  ngle channel if 
-00001d30: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
-00001d40: 6e6f 7420 616e 2061 7272 6179 2e0a 2020  not an array..  
-00001d50: 2020 2020 2020 3a74 7970 6520 696e 6465        :type inde
-00001d60: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00001d70: 616c 5b69 6e74 5d0a 2020 2020 2020 2020  al[int].        
-00001d80: 3a70 6172 616d 2066 7261 6d65 3a20 5468  :param frame: Th
-00001d90: 6520 6672 616d 6520 6f6e 2077 6869 6368  e frame on which
-00001da0: 2074 6865 206b 6579 6672 616d 6520 6973   the keyframe is
-00001db0: 2064 656c 6574 6564 2c20 6465 6661 756c   deleted, defaul
-00001dc0: 7469 6e67 2074 6f20 7468 6520 6375 7272  ting to the curr
-00001dd0: 656e 7420 6672 616d 652e 0a20 2020 2020  ent frame..     
-00001de0: 2020 203a 7479 7065 2066 7261 6d65 3a20     :type frame: 
-00001df0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001e00: 666c 6f61 745d 0a20 2020 2020 2020 203a  float].        :
-00001e10: 7061 7261 6d20 6772 6f75 703a 2054 6865  param group: The
-00001e20: 206e 616d 6520 6f66 2074 6865 2067 726f   name of the gro
-00001e30: 7570 2074 6865 2046 2d43 7572 7665 2073  up the F-Curve s
-00001e40: 686f 756c 6420 6265 2061 6464 6564 2074  hould be added t
-00001e50: 6f20 6966 2069 7420 646f 6573 6e27 7420  o if it doesn't 
-00001e60: 6578 6973 7420 7965 742e 0a20 2020 2020  exist yet..     
-00001e70: 2020 203a 7479 7065 2067 726f 7570 3a20     :type group: 
-00001e80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001e90: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-00001ea0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-00001eb0: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
-00001ec0: 7373 206f 6620 6b65 7966 7261 6d65 2064  ss of keyframe d
-00001ed0: 656c 6574 696f 6e2e 0a20 2020 2020 2020  eletion..       
-00001ee0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00001ef0: 730a 0a20 2020 2064 6566 206b 6579 6672  s..    def keyfr
-00001f00: 616d 655f 696e 7365 7274 280a 2020 2020  ame_insert(.    
-00001f10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00001f20: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
-00001f30: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
-00001f40: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
-00001f50: 2020 2020 2020 2069 6e64 6578 3a20 7479         index: ty
-00001f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00001f70: 745d 203d 202d 312c 0a20 2020 2020 2020  t] = -1,.       
-00001f80: 2020 2020 2066 7261 6d65 3a20 7479 7069       frame: typi
-00001f90: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
-00001fa0: 745d 203d 2027 6270 792e 636f 6e74 6578  t] = 'bpy.contex
-00001fb0: 742e 7363 656e 652e 6672 616d 655f 6375  t.scene.frame_cu
-00001fc0: 7272 656e 7427 2c0a 2020 2020 2020 2020  rrent',.        
-00001fd0: 2020 2020 6772 6f75 703a 2074 7970 696e      group: typin
-00001fe0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
-00001ff0: 3d20 2222 2c0a 2020 2020 2020 2020 2020  = "",.          
-00002000: 2020 6f70 7469 6f6e 733a 2074 7970 696e    options: typin
-00002010: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00002020: 672e 416e 795d 203d 2027 7365 7428 2927  g.Any] = 'set()'
-00002030: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00002040: 2020 2027 2727 2049 6e73 6572 7420 6120     ''' Insert a 
-00002050: 6b65 7966 7261 6d65 206f 6e20 7468 6520  keyframe on the 
-00002060: 7072 6f70 6572 7479 2067 6976 656e 2c20  property given, 
-00002070: 6164 6469 6e67 2066 6375 7276 6573 2061  adding fcurves a
-00002080: 6e64 2061 6e69 6d61 7469 6f6e 2064 6174  nd animation dat
-00002090: 6120 7768 656e 206e 6563 6573 7361 7279  a when necessary
-000020a0: 2e20 5468 6973 2069 7320 7468 6520 6d6f  . This is the mo
-000020b0: 7374 2073 696d 706c 6520 6578 616d 706c  st simple exampl
-000020c0: 6520 6f66 2069 6e73 6572 7469 6e67 2061  e of inserting a
-000020d0: 206b 6579 6672 616d 6520 6672 6f6d 2070   keyframe from p
-000020e0: 7974 686f 6e2e 204e 6f74 6520 7468 6174  ython. Note that
-000020f0: 2077 6865 6e20 6b65 7969 6e67 2064 6174   when keying dat
-00002100: 6120 7061 7468 7320 7768 6963 6820 636f  a paths which co
-00002110: 6e74 6169 6e20 6e65 7374 6564 2070 726f  ntain nested pro
-00002120: 7065 7274 6965 7320 7468 6973 206d 7573  perties this mus
-00002130: 7420 6265 2064 6f6e 6520 6672 6f6d 2074  t be done from t
-00002140: 6865 2060 4944 6020 7375 6263 6c61 7373  he `ID` subclass
-00002150: 2c20 696e 2074 6869 7320 6361 7365 2074  , in this case t
-00002160: 6865 2060 4172 6d61 7475 7265 6020 7261  he `Armature` ra
-00002170: 7468 6572 2074 6861 6e20 7468 6520 626f  ther than the bo
-00002180: 6e65 2e0a 0a20 2020 2020 2020 203a 7061  ne...        :pa
-00002190: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
-000021a0: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
-000021b0: 7274 7920 746f 206b 6579 2c20 616e 616c  rty to key, anal
-000021c0: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
-000021d0: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
-000021e0: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
-000021f0: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
-00002200: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00002210: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00002220: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
-00002230: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00002240: 2074 6f20 6b65 792e 2044 6566 6175 6c74   to key. Default
-00002250: 7320 746f 202d 3120 7768 6963 6820 7769  s to -1 which wi
-00002260: 6c6c 206b 6579 2061 6c6c 2069 6e64 6963  ll key all indic
-00002270: 6573 206f 7220 6120 7369 6e67 6c65 2063  es or a single c
-00002280: 6861 6e6e 656c 2069 6620 7468 6520 7072  hannel if the pr
-00002290: 6f70 6572 7479 2069 7320 6e6f 7420 616e  operty is not an
-000022a0: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
-000022b0: 3a74 7970 6520 696e 6465 783a 2074 7970  :type index: typ
-000022c0: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
-000022d0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-000022e0: 2066 7261 6d65 3a20 5468 6520 6672 616d   frame: The fram
-000022f0: 6520 6f6e 2077 6869 6368 2074 6865 206b  e on which the k
-00002300: 6579 6672 616d 6520 6973 2069 6e73 6572  eyframe is inser
-00002310: 7465 642c 2064 6566 6175 6c74 696e 6720  ted, defaulting 
-00002320: 746f 2074 6865 2063 7572 7265 6e74 2066  to the current f
-00002330: 7261 6d65 2e0a 2020 2020 2020 2020 3a74  rame..        :t
-00002340: 7970 6520 6672 616d 653a 2074 7970 696e  ype frame: typin
-00002350: 672e 4f70 7469 6f6e 616c 5b66 6c6f 6174  g.Optional[float
-00002360: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-00002370: 2067 726f 7570 3a20 5468 6520 6e61 6d65   group: The name
-00002380: 206f 6620 7468 6520 6772 6f75 7020 7468   of the group th
-00002390: 6520 462d 4375 7276 6520 7368 6f75 6c64  e F-Curve should
-000023a0: 2062 6520 6164 6465 6420 746f 2069 6620   be added to if 
-000023b0: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
-000023c0: 2079 6574 2e0a 2020 2020 2020 2020 3a74   yet..        :t
-000023d0: 7970 6520 6772 6f75 703a 2074 7970 696e  ype group: typin
-000023e0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-000023f0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00002400: 6c61 673a 200a 2020 2020 2020 2020 3a74  lag: .        :t
-00002410: 7970 6520 666c 6167 3a20 7479 7069 6e67  ype flag: typing
-00002420: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00002430: 2e53 6574 5d0a 2020 2020 2020 2020 3a70  .Set].        :p
-00002440: 6172 616d 206f 7074 696f 6e73 3a20 202d  aram options:  -
-00002450: 2060 6049 4e53 4552 544b 4559 5f4e 4545   ``INSERTKEY_NEE
-00002460: 4445 4460 6020 4f6e 6c79 2069 6e73 6572  DED`` Only inser
-00002470: 7420 6b65 7966 7261 6d65 7320 7768 6572  t keyframes wher
-00002480: 6520 7468 6579 2772 6520 6e65 6564 6564  e they're needed
-00002490: 2069 6e20 7468 6520 7265 6c65 7661 6e74   in the relevant
-000024a0: 2046 2d43 7572 7665 732e 202d 2060 6049   F-Curves. - ``I
-000024b0: 4e53 4552 544b 4559 5f56 4953 5541 4c60  NSERTKEY_VISUAL`
-000024c0: 6020 496e 7365 7274 206b 6579 6672 616d  ` Insert keyfram
-000024d0: 6573 2062 6173 6564 206f 6e20 2776 6973  es based on 'vis
-000024e0: 7561 6c20 7472 616e 7366 6f72 6d73 272e  ual transforms'.
-000024f0: 202d 2060 6049 4e53 4552 544b 4559 5f58   - ``INSERTKEY_X
-00002500: 595a 5f54 4f5f 5247 4260 6020 436f 6c6f  YZ_TO_RGB`` Colo
-00002510: 7220 666f 7220 6e65 776c 7920 6164 6465  r for newly adde
-00002520: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
-00002530: 2046 2d43 7572 7665 7320 284c 6f63 6174   F-Curves (Locat
-00002540: 696f 6e2c 2052 6f74 6174 696f 6e2c 2053  ion, Rotation, S
-00002550: 6361 6c65 2920 6973 2062 6173 6564 206f  cale) is based o
-00002560: 6e20 7468 6520 7472 616e 7366 6f72 6d20  n the transform 
-00002570: 6178 6973 2e20 2d20 6060 494e 5345 5254  axis. - ``INSERT
-00002580: 4b45 595f 5245 504c 4143 4560 6020 4f6e  KEY_REPLACE`` On
-00002590: 6c79 2072 6570 6c61 6365 2061 6c72 6561  ly replace alrea
-000025a0: 6479 2065 7869 7374 696e 6720 6b65 7966  dy existing keyf
-000025b0: 7261 6d65 732e 202d 2060 6049 4e53 4552  rames. - ``INSER
-000025c0: 544b 4559 5f41 5641 494c 4142 4c45 6060  TKEY_AVAILABLE``
-000025d0: 204f 6e6c 7920 696e 7365 7274 2069 6e74   Only insert int
-000025e0: 6f20 616c 7265 6164 7920 6578 6973 7469  o already existi
-000025f0: 6e67 2046 2d43 7572 7665 732e 202d 2060  ng F-Curves. - `
-00002600: 6049 4e53 4552 544b 4559 5f43 5943 4c45  `INSERTKEY_CYCLE
-00002610: 5f41 5741 5245 6060 2054 616b 6520 6379  _AWARE`` Take cy
-00002620: 636c 6963 2065 7874 7261 706f 6c61 7469  clic extrapolati
-00002630: 6f6e 2069 6e74 6f20 6163 636f 756e 7420  on into account 
-00002640: 2843 7963 6c65 2d41 7761 7265 204b 6579  (Cycle-Aware Key
-00002650: 696e 6720 6f70 7469 6f6e 292e 0a20 2020  ing option)..   
-00002660: 2020 2020 203a 7479 7065 206f 7074 696f       :type optio
-00002670: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
-00002680: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
-00002690: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000026a0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
-000026b0: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
-000026c0: 206b 6579 6672 616d 6520 696e 7365 7274   keyframe insert
-000026d0: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
-000026e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000026f0: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
-00002700: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
-00002710: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00002720: 7572 6e73 2074 6865 206b 6579 7320 6f66  urns the keys of
-00002730: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
-00002740: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
-00002750: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
-00002760: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
-00002770: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
-00002780: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
-00002790: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
-000027a0: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
-000027b0: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
-000027c0: 7065 7274 7920 6b65 7973 2e0a 2020 2020  perty keys..    
-000027d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000027e0: 7061 7373 0a0a 2020 2020 6465 6620 7061  pass..    def pa
-000027f0: 7468 5f66 726f 6d5f 6964 2873 656c 662c  th_from_id(self,
-00002800: 2070 726f 7065 7274 793a 2074 7970 696e   property: typin
-00002810: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
-00002820: 3d20 2222 2920 2d3e 2073 7472 3a0a 2020  = "") -> str:.  
-00002830: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00002840: 7320 7468 6520 6461 7461 2070 6174 6820  s the data path 
-00002850: 6672 6f6d 2074 6865 2049 4420 746f 2074  from the ID to t
-00002860: 6869 7320 6f62 6a65 6374 2028 7374 7269  his object (stri
-00002870: 6e67 292e 0a0a 2020 2020 2020 2020 3a70  ng)...        :p
-00002880: 6172 616d 2070 726f 7065 7274 793a 204f  aram property: O
-00002890: 7074 696f 6e61 6c20 7072 6f70 6572 7479  ptional property
-000028a0: 206e 616d 6520 7768 6963 6820 6361 6e20   name which can 
-000028b0: 6265 2075 7365 6420 6966 2074 6865 2070  be used if the p
-000028c0: 6174 6820 6973 2074 6f20 6120 7072 6f70  ath is to a prop
-000028d0: 6572 7479 206f 6620 7468 6973 206f 626a  erty of this obj
-000028e0: 6563 742e 0a20 2020 2020 2020 203a 7479  ect..        :ty
-000028f0: 7065 2070 726f 7065 7274 793a 2074 7970  pe property: typ
-00002900: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00002910: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-00002920: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
-00002930: 6574 7572 6e3a 2060 6270 792e 7479 7065  eturn: `bpy.type
-00002940: 732e 6270 795f 7374 7275 6374 2e69 645f  s.bpy_struct.id_
-00002950: 6461 7461 6020 746f 2074 6869 7320 7374  data` to this st
-00002960: 7275 6374 2061 6e64 2070 726f 7065 7274  ruct and propert
-00002970: 7920 2877 6865 6e20 6769 7665 6e29 2e0a  y (when given)..
-00002980: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00002990: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000029a0: 6620 7061 7468 5f72 6573 6f6c 7665 2873  f path_resolve(s
-000029b0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000029c0: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
-000029d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000029e0: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
-000029f0: 2020 2020 2020 2020 2020 2063 6f65 7263             coerc
-00002a00: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
-00002a10: 616c 5b62 6f6f 6c5d 203d 2054 7275 6529  al[bool] = True)
-00002a20: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00002a30: 7475 726e 7320 7468 6520 7072 6f70 6572  turns the proper
-00002a40: 7479 2066 726f 6d20 7468 6520 7061 7468  ty from the path
-00002a50: 2c20 7261 6973 6520 616e 2065 7863 6570  , raise an excep
-00002a60: 7469 6f6e 2077 6865 6e20 6e6f 7420 666f  tion when not fo
-00002a70: 756e 642e 0a0a 2020 2020 2020 2020 3a70  und...        :p
-00002a80: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
-00002a90: 7768 6963 6820 7468 6973 2070 726f 7065  which this prope
-00002aa0: 7274 7920 7265 736f 6c76 6573 2e0a 2020  rty resolves..  
-00002ab0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
-00002ac0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002ad0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00002ae0: 7061 7261 6d20 636f 6572 6365 3a20 6f70  param coerce: op
-00002af0: 7469 6f6e 616c 2061 7267 756d 656e 742c  tional argument,
-00002b00: 2077 6865 6e20 5472 7565 2c20 7468 6520   when True, the 
-00002b10: 7072 6f70 6572 7479 2077 696c 6c20 6265  property will be
-00002b20: 2063 6f6e 7665 7274 6564 2069 6e74 6f20   converted into 
-00002b30: 6974 7320 5079 7468 6f6e 2072 6570 7265  its Python repre
-00002b40: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
-00002b50: 2020 203a 7479 7065 2063 6f65 7263 653a     :type coerce:
-00002b60: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002b70: 5b62 6f6f 6c5d 0a20 2020 2020 2020 2027  [bool].        '
-00002b80: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00002b90: 0a20 2020 2064 6566 2070 6f70 2873 656c  .    def pop(sel
-00002ba0: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
-00002bb0: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-00002bc0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-00002bd0: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
-00002be0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00002bf0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
-00002c00: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
-00002c10: 5265 6d6f 7665 2061 6e64 2072 6574 7572  Remove and retur
-00002c20: 6e20 7468 6520 7661 6c75 6520 6f66 2074  n the value of t
-00002c30: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
-00002c40: 7479 2061 7373 6967 6e65 6420 746f 206b  ty assigned to k
-00002c50: 6579 206f 7220 6465 6661 756c 7420 7768  ey or default wh
-00002c60: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
-00002c70: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
-00002c80: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
-00002c90: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
-00002ca0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
-00002cb0: 7061 7261 6d20 6b65 793a 2054 6865 206b  param key: The k
-00002cc0: 6579 2061 7373 6f63 6961 7465 6420 7769  ey associated wi
-00002cd0: 7468 2074 6865 2063 7573 746f 6d20 7072  th the custom pr
-00002ce0: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
-00002cf0: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
-00002d00: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-00002d10: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00002d20: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
-00002d30: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
-00002d40: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
-00002d50: 6e20 6966 202a 6b65 792a 2069 7320 6e6f  n if *key* is no
-00002d60: 7420 666f 756e 642e 0a20 2020 2020 2020  t found..       
-00002d70: 203a 7479 7065 2064 6566 6175 6c74 3a20   :type default: 
-00002d80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002d90: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
-00002da0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00002db0: 7061 7373 0a0a 2020 2020 6465 6620 7072  pass..    def pr
-00002dc0: 6f70 6572 7479 5f6f 7665 7272 6964 6162  operty_overridab
-00002dd0: 6c65 5f6c 6962 7261 7279 5f73 6574 2873  le_library_set(s
-00002de0: 656c 662c 2070 726f 7065 7274 792c 206f  elf, property, o
-00002df0: 7665 7272 6964 6162 6c65 2920 2d3e 2062  verridable) -> b
-00002e00: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-00002e10: 2044 6566 696e 6520 6120 7072 6f70 6572   Define a proper
-00002e20: 7479 2061 7320 6f76 6572 7269 6461 626c  ty as overridabl
-00002e30: 6520 6f72 206e 6f74 2028 6f6e 6c79 2066  e or not (only f
-00002e40: 6f72 2063 7573 746f 6d20 7072 6f70 6572  or custom proper
-00002e50: 7469 6573 2129 2e0a 0a20 2020 2020 2020  ties!)...       
-00002e60: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00002e70: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-00002e80: 7275 6520 7768 656e 2074 6865 206f 7665  rue when the ove
-00002e90: 7272 6964 6162 6c65 2073 7461 7475 7320  rridable status 
-00002ea0: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00002eb0: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
-00002ec0: 2073 6574 2e0a 2020 2020 2020 2020 2727   set..        ''
-00002ed0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00002ee0: 2020 2020 6465 6620 7072 6f70 6572 7479      def property
-00002ef0: 5f75 6e73 6574 2873 656c 662c 2070 726f  _unset(self, pro
-00002f00: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
-00002f10: 2727 2720 556e 7365 7420 6120 7072 6f70  ''' Unset a prop
-00002f20: 6572 7479 2c20 7769 6c6c 2075 7365 2064  erty, will use d
-00002f30: 6566 6175 6c74 2076 616c 7565 2061 6674  efault value aft
-00002f40: 6572 7761 7264 2e0a 0a20 2020 2020 2020  erward...       
-00002f50: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00002f60: 730a 0a20 2020 2064 6566 2074 7970 655f  s..    def type_
-00002f70: 7265 6361 7374 2873 656c 6629 202d 3e20  recast(self) -> 
-00002f80: 2762 7079 5f73 7472 7563 7427 3a0a 2020  'bpy_struct':.  
-00002f90: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00002fa0: 2061 206e 6577 2069 6e73 7461 6e63 652c   a new instance,
-00002fb0: 2074 6869 7320 6973 206e 6565 6465 6420   this is needed 
-00002fc0: 6265 6361 7573 6520 7479 7065 7320 7375  because types su
-00002fd0: 6368 2061 7320 7465 7874 7572 6573 2063  ch as textures c
-00002fe0: 616e 2062 6520 6368 616e 6765 6420 6174  an be changed at
-00002ff0: 2072 756e 7469 6d65 2e0a 0a20 2020 2020   runtime...     
-00003000: 2020 203a 7274 7970 653a 2027 6270 795f     :rtype: 'bpy_
-00003010: 7374 7275 6374 270a 2020 2020 2020 2020  struct'.        
-00003020: 3a72 6574 7572 6e3a 2061 206e 6577 2069  :return: a new i
-00003030: 6e73 7461 6e63 6520 6f66 2074 6869 7320  nstance of this 
-00003040: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00003050: 7479 7065 2069 6e69 7469 616c 697a 6564  type initialized
-00003060: 2061 6761 696e 2e0a 2020 2020 2020 2020   again..        
-00003070: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00003080: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
-00003090: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-000030a0: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
-000030b0: 2720 5265 7475 726e 7320 7468 6520 7661  ' Returns the va
-000030c0: 6c75 6573 206f 6620 7468 6973 206f 626a  lues of this obj
-000030d0: 6563 7473 2063 7573 746f 6d20 7072 6f70  ects custom prop
-000030e0: 6572 7469 6573 2028 6d61 7463 6865 7320  erties (matches 
-000030f0: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
-00003100: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
-00003110: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
-00003120: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00003130: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
-00003140: 2020 2020 3a72 6574 7572 6e3a 2063 7573      :return: cus
-00003150: 746f 6d20 7072 6f70 6572 7479 2076 616c  tom property val
-00003160: 7565 732e 0a20 2020 2020 2020 2027 2727  ues..        '''
-00003170: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003180: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
-00003190: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
-000031a0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-000031b0: 7374 725d 2920 2d3e 2027 7479 7069 6e67  str]) -> 'typing
-000031c0: 2e41 6e79 273a 0a20 2020 2020 2020 2027  .Any':.        '
-000031d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
-000031e0: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
-000031f0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-00003200: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003210: 7472 5d0a 2020 2020 2020 2020 3a72 7479  tr].        :rty
-00003220: 7065 3a20 2774 7970 696e 672e 416e 7927  pe: 'typing.Any'
-00003230: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003240: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003250: 6566 205f 5f73 6574 6974 656d 5f5f 2873  ef __setitem__(s
-00003260: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
-00003270: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
-00003280: 2c20 7661 6c75 653a 2027 7479 7069 6e67  , value: 'typing
-00003290: 2e41 6e79 2729 3a0a 2020 2020 2020 2020  .Any'):.        
-000032a0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-000032b0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-000032c0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-000032d0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-000032e0: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
-000032f0: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
-00003300: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
-00003310: 2027 7479 7069 6e67 2e41 6e79 270a 2020   'typing.Any'.  
-00003320: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003330: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003340: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
-00003350: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
-00003360: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
-00003370: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
-00003380: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00003390: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
-000033a0: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
-000033b0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-000033c0: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
-000033d0: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
-000033e0: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
-000033f0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003400: 7373 0a0a 0a63 6c61 7373 2062 7079 5f70  ss...class bpy_p
-00003410: 726f 705f 636f 6c6c 6563 7469 6f6e 2874  rop_collection(t
-00003420: 7970 696e 672e 4765 6e65 7269 635b 4765  yping.Generic[Ge
-00003430: 6e65 7269 6354 7970 655d 293a 0a20 2020  nericType]):.   
-00003440: 2027 2727 2062 7569 6c74 2d69 6e20 636c   ''' built-in cl
-00003450: 6173 7320 7573 6564 2066 6f72 2061 6c6c  ass used for all
-00003460: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
-00003470: 2020 2727 270a 0a20 2020 2064 6566 2066    '''..    def f
-00003480: 696e 6428 7365 6c66 2c20 6b65 793a 2074  ind(self, key: t
-00003490: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-000034a0: 7472 5d29 202d 3e20 696e 743a 0a20 2020  tr]) -> int:.   
-000034b0: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
-000034c0: 2074 6865 2069 6e64 6578 206f 6620 6120   the index of a 
-000034d0: 6b65 7920 696e 2061 2063 6f6c 6c65 6374  key in a collect
-000034e0: 696f 6e20 6f72 202d 3120 7768 656e 206e  ion or -1 when n
-000034f0: 6f74 2066 6f75 6e64 2028 6d61 7463 6865  ot found (matche
-00003500: 7320 5079 7468 6f6e 2773 2073 7472 696e  s Python's strin
-00003510: 6720 6669 6e64 2066 756e 6374 696f 6e20  g find function 
-00003520: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-00003530: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
-00003540: 616d 206b 6579 3a20 5468 6520 6964 656e  am key: The iden
-00003550: 7469 6669 6572 2066 6f72 2074 6865 2063  tifier for the c
-00003560: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
-00003570: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003580: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
-00003590: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
-000035a0: 2020 3a72 7479 7065 3a20 696e 740a 2020    :rtype: int.  
-000035b0: 2020 2020 2020 3a72 6574 7572 6e3a 2069        :return: i
-000035c0: 6e64 6578 206f 6620 7468 6520 6b65 792e  ndex of the key.
-000035d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000035e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000035f0: 6566 2066 6f72 6561 6368 5f67 6574 2873  ef foreach_get(s
-00003600: 656c 662c 2061 7474 722c 2073 6571 293a  elf, attr, seq):
-00003610: 0a20 2020 2020 2020 2027 2727 2054 6869  .        ''' Thi
-00003620: 7320 6973 2061 2066 756e 6374 696f 6e20  s is a function 
-00003630: 746f 2067 6976 6520 6661 7374 2061 6363  to give fast acc
-00003640: 6573 7320 746f 2061 7474 7269 6275 7465  ess to attribute
-00003650: 7320 7769 7468 696e 2061 2063 6f6c 6c65  s within a colle
-00003660: 6374 696f 6e2e 204f 6e6c 7920 776f 726b  ction. Only work
-00003670: 7320 666f 7220 2762 6173 6963 2074 7970  s for 'basic typ
-00003680: 6527 2070 726f 7065 7274 6965 7320 2862  e' properties (b
-00003690: 6f6f 6c2c 2069 6e74 2061 6e64 2066 6c6f  ool, int and flo
-000036a0: 6174 2921 204d 756c 7469 2d64 696d 656e  at)! Multi-dimen
-000036b0: 7369 6f6e 616c 2061 7272 6179 7320 286c  sional arrays (l
-000036c0: 696b 6520 6172 7261 7920 6f66 2076 6563  ike array of vec
-000036d0: 746f 7273 2920 7769 6c6c 2062 6520 666c  tors) will be fl
-000036e0: 6174 7465 6e65 6420 696e 746f 2073 6571  attened into seq
-000036f0: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-00003700: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003710: 2064 6566 2066 6f72 6561 6368 5f73 6574   def foreach_set
-00003720: 2873 656c 662c 2061 7474 722c 2073 6571  (self, attr, seq
-00003730: 293a 0a20 2020 2020 2020 2027 2727 2054  ):.        ''' T
-00003740: 6869 7320 6973 2061 2066 756e 6374 696f  his is a functio
-00003750: 6e20 746f 2067 6976 6520 6661 7374 2061  n to give fast a
-00003760: 6363 6573 7320 746f 2061 7474 7269 6275  ccess to attribu
-00003770: 7465 7320 7769 7468 696e 2061 2063 6f6c  tes within a col
-00003780: 6c65 6374 696f 6e2e 204f 6e6c 7920 776f  lection. Only wo
-00003790: 726b 7320 666f 7220 2762 6173 6963 2074  rks for 'basic t
-000037a0: 7970 6527 2070 726f 7065 7274 6965 7320  ype' properties 
-000037b0: 2862 6f6f 6c2c 2069 6e74 2061 6e64 2066  (bool, int and f
-000037c0: 6c6f 6174 2921 2073 6571 206d 7573 7420  loat)! seq must 
-000037d0: 6265 2075 6e69 2d64 696d 656e 7369 6f6e  be uni-dimension
-000037e0: 616c 2c20 6d75 6c74 692d 6469 6d65 6e73  al, multi-dimens
-000037f0: 696f 6e61 6c20 6172 7261 7973 2028 6c69  ional arrays (li
-00003800: 6b65 2061 7272 6179 206f 6620 7665 6374  ke array of vect
-00003810: 6f72 7329 2077 696c 6c20 6265 2072 652d  ors) will be re-
-00003820: 6372 6561 7465 6420 6672 6f6d 2069 742e  created from it.
-00003830: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00003840: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003850: 6465 6620 6765 7428 7365 6c66 2c0a 2020  def get(self,.  
-00003860: 2020 2020 2020 2020 2020 6b65 793a 2074            key: t
-00003870: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00003880: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00003890: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
-000038a0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000038b0: 2e41 6e79 5d20 3d20 4e6f 6e65 293a 0a20  .Any] = None):. 
-000038c0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-000038d0: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
-000038e0: 7468 6520 6974 656d 2061 7373 6967 6e65  the item assigne
-000038f0: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
-00003900: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
-00003910: 6e64 2028 6d61 7463 6865 7320 5079 7468  nd (matches Pyth
-00003920: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
-00003930: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-00003940: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
-00003950: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00003960: 2054 6865 2069 6465 6e74 6966 6965 7220   The identifier 
-00003970: 666f 7220 7468 6520 636f 6c6c 6563 7469  for the collecti
-00003980: 6f6e 206d 656d 6265 722e 0a20 2020 2020  on member..     
-00003990: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-000039a0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-000039b0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
-000039c0: 6d20 6465 6661 756c 743a 204f 7074 696f  m default: Optio
-000039d0: 6e61 6c20 6172 6775 6d65 6e74 2066 6f72  nal argument for
-000039e0: 2074 6865 2076 616c 7565 2074 6f20 7265   the value to re
-000039f0: 7475 726e 2069 6620 2a6b 6579 2a20 6973  turn if *key* is
-00003a00: 206e 6f74 2066 6f75 6e64 2e0a 2020 2020   not found..    
-00003a10: 2020 2020 3a74 7970 6520 6465 6661 756c      :type defaul
-00003a20: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-00003a30: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
-00003a40: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00003a50: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00003a60: 2069 7465 6d73 2873 656c 6629 202d 3e20   items(self) -> 
-00003a70: 7479 7069 6e67 2e4c 6973 743a 0a20 2020  typing.List:.   
-00003a80: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
-00003a90: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
-00003aa0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
-00003ab0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
-00003ac0: 5079 7468 6f6e 2773 2064 6963 742e 6974  Python's dict.it
-00003ad0: 656d 7328 2920 6675 6e63 7469 6f6e 616c  ems() functional
-00003ae0: 6974 7929 2e0a 0a20 2020 2020 2020 203a  ity)...        :
-00003af0: 7274 7970 653a 2074 7970 696e 672e 4c69  rtype: typing.Li
-00003b00: 7374 0a20 2020 2020 2020 203a 7265 7475  st.        :retu
-00003b10: 726e 3a20 286b 6579 2c20 7661 6c75 6529  rn: (key, value)
-00003b20: 2070 6169 7273 2066 6f72 2065 6163 6820   pairs for each 
-00003b30: 6d65 6d62 6572 206f 6620 7468 6973 2063  member of this c
-00003b40: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00003b50: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003b60: 6173 730a 0a20 2020 2064 6566 206b 6579  ass..    def key
-00003b70: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
-00003b80: 672e 4c69 7374 5b73 7472 5d3a 0a20 2020  g.List[str]:.   
-00003b90: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
-00003ba0: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
-00003bb0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
-00003bc0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
-00003bd0: 5079 7468 6f6e 2773 2064 6963 742e 6b65  Python's dict.ke
-00003be0: 7973 2829 2066 756e 6374 696f 6e61 6c69  ys() functionali
-00003bf0: 7479 292e 0a0a 2020 2020 2020 2020 3a72  ty)...        :r
-00003c00: 7479 7065 3a20 7479 7069 6e67 2e4c 6973  type: typing.Lis
-00003c10: 745b 7374 725d 0a20 2020 2020 2020 203a  t[str].        :
-00003c20: 7265 7475 726e 3a20 7468 6520 6964 656e  return: the iden
-00003c30: 7469 6669 6572 7320 666f 7220 6561 6368  tifiers for each
-00003c40: 206d 656d 6265 7220 6f66 2074 6869 7320   member of this 
-00003c50: 636f 6c6c 6563 7469 6f6e 2e0a 2020 2020  collection..    
-00003c60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00003c70: 7061 7373 0a0a 2020 2020 6465 6620 7661  pass..    def va
-00003c80: 6c75 6573 2873 656c 6629 202d 3e20 7479  lues(self) -> ty
-00003c90: 7069 6e67 2e4c 6973 743a 0a20 2020 2020  ping.List:.     
-00003ca0: 2020 2027 2727 2052 6574 7572 6e20 7468     ''' Return th
-00003cb0: 6520 7661 6c75 6573 206f 6620 636f 6c6c  e values of coll
-00003cc0: 6563 7469 6f6e 2028 6d61 7463 6869 6e67  ection (matching
-00003cd0: 2050 7974 686f 6e27 7320 6469 6374 2e76   Python's dict.v
-00003ce0: 616c 7565 7328 2920 6675 6e63 7469 6f6e  alues() function
-00003cf0: 616c 6974 7929 2e0a 0a20 2020 2020 2020  ality)...       
-00003d00: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
-00003d10: 4c69 7374 0a20 2020 2020 2020 203a 7265  List.        :re
-00003d20: 7475 726e 3a20 7468 6520 6d65 6d62 6572  turn: the member
-00003d30: 7320 6f66 2074 6869 7320 636f 6c6c 6563  s of this collec
-00003d40: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
-00003d50: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00003d60: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
-00003d70: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
-00003d80: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00003d90: 2073 7472 5d29 202d 3e20 2747 656e 6572   str]) -> 'Gener
-00003da0: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
-00003db0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00003dc0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
-00003dd0: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
-00003de0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00003df0: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
-00003e00: 7479 7065 3a20 2747 656e 6572 6963 5479  type: 'GenericTy
-00003e10: 7065 270a 2020 2020 2020 2020 2727 270a  pe'.        '''.
-00003e20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00003e30: 2020 6465 6620 5f5f 7365 7469 7465 6d5f    def __setitem_
-00003e40: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
-00003e50: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003e60: 7472 5d2c 2076 616c 7565 3a20 2747 656e  tr], value: 'Gen
-00003e70: 6572 6963 5479 7065 2729 3a0a 2020 2020  ericType'):.    
-00003e80: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
-00003e90: 2020 3a70 6172 616d 206b 6579 3a20 0a20    :param key: . 
-00003ea0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-00003eb0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
-00003ec0: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
-00003ed0: 203a 7061 7261 6d20 7661 6c75 653a 200a   :param value: .
-00003ee0: 2020 2020 2020 2020 3a74 7970 6520 7661          :type va
-00003ef0: 6c75 653a 2027 4765 6e65 7269 6354 7970  lue: 'GenericTyp
-00003f00: 6527 0a20 2020 2020 2020 2027 2727 0a20  e'.        '''. 
-00003f10: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003f20: 2064 6566 205f 5f64 656c 6974 656d 5f5f   def __delitem__
-00003f30: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
-00003f40: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003f50: 725d 2920 2d3e 2027 4765 6e65 7269 6354  r]) -> 'GenericT
-00003f60: 7970 6527 3a0a 2020 2020 2020 2020 2727  ype':.        ''
-00003f70: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
-00003f80: 616d 206b 6579 3a20 0a20 2020 2020 2020  am key: .       
-00003f90: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
-00003fa0: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003fb0: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
-00003fc0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
-00003fd0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003fe0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003ff0: 6566 205f 5f69 7465 725f 5f28 7365 6c66  ef __iter__(self
-00004000: 2920 2d3e 2074 7970 696e 672e 4974 6572  ) -> typing.Iter
-00004010: 6174 6f72 5b27 4765 6e65 7269 6354 7970  ator['GenericTyp
-00004020: 6527 5d3a 0a20 2020 2020 2020 2027 2727  e']:.        '''
-00004030: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
-00004040: 653a 2074 7970 696e 672e 4974 6572 6174  e: typing.Iterat
-00004050: 6f72 5b27 4765 6e65 7269 6354 7970 6527  or['GenericType'
-00004060: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
-00004070: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00004080: 6465 6620 5f5f 6e65 7874 5f5f 2873 656c  def __next__(sel
-00004090: 6629 202d 3e20 2747 656e 6572 6963 5479  f) -> 'GenericTy
-000040a0: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
-000040b0: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
-000040c0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
-000040d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000040e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000040f0: 6566 205f 5f6c 656e 5f5f 2873 656c 6629  ef __len__(self)
-00004100: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00004110: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00004120: 7274 7970 653a 2069 6e74 0a20 2020 2020  rtype: int.     
+00001b50: 6c5b 696e 745d 0a20 2020 2020 2020 203a  l[int].        :
+00001b60: 7274 7970 653a 2027 4643 7572 7665 270a  rtype: 'FCurve'.
+00001b70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001b80: 2054 6865 2064 7269 7665 7228 7329 2061   The driver(s) a
+00001b90: 6464 6564 2e0a 2020 2020 2020 2020 2727  dded..        ''
+00001ba0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00001bb0: 2020 2020 6465 6620 6472 6976 6572 5f72      def driver_r
+00001bc0: 656d 6f76 6528 7365 6c66 2c0a 2020 2020  emove(self,.    
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 7061 7468 3a20 7479 7069 6e67 2e4f    path: typing.O
+00001bf0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
+00001c20: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+00001c30: 3d20 2d31 2920 2d3e 2062 6f6f 6c3a 0a20  = -1) -> bool:. 
+00001c40: 2020 2020 2020 2027 2727 2052 656d 6f76         ''' Remov
+00001c50: 6520 6472 6976 6572 2873 2920 6672 6f6d  e driver(s) from
+00001c60: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
+00001c70: 7274 790a 0a20 2020 2020 2020 203a 7061  rty..        :pa
+00001c80: 7261 6d20 7061 7468 3a20 7061 7468 2074  ram path: path t
+00001c90: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
+00001ca0: 6f20 6472 6976 652c 2061 6e61 6c6f 676f  o drive, analogo
+00001cb0: 7573 2074 6f20 7468 6520 6663 7572 7665  us to the fcurve
+00001cc0: 2773 2064 6174 6120 7061 7468 2e0a 2020  's data path..  
+00001cd0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
+00001ce0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00001cf0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00001d00: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
+00001d10: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
+00001d20: 7072 6f70 6572 7479 2064 7269 7665 2e20  property drive. 
+00001d30: 4465 6661 756c 7473 2074 6f20 2d31 2066  Defaults to -1 f
+00001d40: 6f72 2061 6c6c 2069 6e64 6963 6573 206f  or all indices o
+00001d50: 7220 6120 7369 6e67 6c65 2063 6861 6e6e  r a single chann
+00001d60: 656c 2069 6620 7468 6520 7072 6f70 6572  el if the proper
+00001d70: 7479 2069 7320 6e6f 7420 616e 2061 7272  ty is not an arr
+00001d80: 6179 2e0a 2020 2020 2020 2020 3a74 7970  ay..        :typ
+00001d90: 6520 696e 6465 783a 2074 7970 696e 672e  e index: typing.
+00001da0: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
+00001db0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+00001dc0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+00001dd0: 726e 3a20 5375 6363 6573 7320 6f66 2064  rn: Success of d
+00001de0: 7269 7665 7220 7265 6d6f 7661 6c2e 0a20  river removal.. 
+00001df0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001e00: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00001e10: 2067 6574 2873 656c 662c 0a20 2020 2020   get(self,.     
+00001e20: 2020 2020 2020 206b 6579 3a20 7479 7069         key: typi
+00001e30: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00001e40: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00001e50: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
+00001e60: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
+00001e70: 795d 203d 204e 6f6e 6529 3a0a 2020 2020  y] = None):.    
+00001e80: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
+00001e90: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
+00001ea0: 2063 7573 746f 6d20 7072 6f70 6572 7479   custom property
+00001eb0: 2061 7373 6967 6e65 6420 746f 206b 6579   assigned to key
+00001ec0: 206f 7220 6465 6661 756c 7420 7768 656e   or default when
+00001ed0: 206e 6f74 2066 6f75 6e64 2028 6d61 7463   not found (matc
+00001ee0: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
+00001ef0: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
+00001f00: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
+00001f10: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
+00001f20: 7261 6d20 6b65 793a 2054 6865 206b 6579  ram key: The key
+00001f30: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00001f40: 2074 6865 2063 7573 746f 6d20 7072 6f70   the custom prop
+00001f50: 6572 7479 2e0a 2020 2020 2020 2020 3a74  erty..        :t
+00001f60: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+00001f70: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00001f80: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
+00001f90: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
+00001fa0: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
+00001fb0: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
+00001fc0: 6966 202a 6b65 792a 2069 7320 6e6f 7420  if *key* is not 
+00001fd0: 666f 756e 642e 0a20 2020 2020 2020 203a  found..        :
+00001fe0: 7479 7065 2064 6566 6175 6c74 3a20 7479  type default: ty
+00001ff0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00002000: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
+00002010: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00002020: 7373 0a0a 2020 2020 6465 6620 6964 5f70  ss..    def id_p
+00002030: 726f 7065 7274 6965 735f 636c 6561 7228  roperties_clear(
+00002040: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
+00002050: 2727 200a 0a20 2020 2020 2020 2027 2727  '' ..        '''
+00002060: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002070: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
+00002080: 7469 6573 5f65 6e73 7572 6528 7365 6c66  ties_ensure(self
+00002090: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
+000020a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000020b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+000020c0: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
+000020d0: 2020 3a72 6574 7572 6e3a 2074 6865 2070    :return: the p
+000020e0: 6172 656e 7420 6772 6f75 7020 666f 7220  arent group for 
+000020f0: 616e 2052 4e41 2073 7472 7563 7427 7320  an RNA struct's 
+00002100: 6375 7374 6f6d 2049 4450 726f 7065 7274  custom IDPropert
+00002110: 6965 732e 0a20 2020 2020 2020 2027 2727  ies..        '''
+00002120: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002130: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
+00002140: 7469 6573 5f75 6928 7365 6c66 2c20 6b65  ties_ui(self, ke
+00002150: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00002160: 616c 5b74 7970 696e 672e 416e 795d 2920  al[typing.Any]) 
+00002170: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
+00002180: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
+00002190: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+000021a0: 2020 5374 7269 6e67 206e 616d 6520 6f66    String name of
+000021b0: 2074 6865 2070 726f 7065 7274 792e 0a20   the property.. 
+000021c0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+000021d0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000021e0: 6c5b 7479 7069 6e67 2e41 6e79 5d0a 2020  l[typing.Any].  
+000021f0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+00002200: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
+00002210: 203a 7265 7475 726e 3a20 5265 7475 726e   :return: Return
+00002220: 2061 6e20 6f62 6a65 6374 2075 7365 6420   an object used 
+00002230: 746f 206d 616e 6167 6520 616e 2049 4450  to manage an IDP
+00002240: 726f 7065 7274 7927 7320 5549 2064 6174  roperty's UI dat
+00002250: 612e 0a20 2020 2020 2020 2027 2727 0a20  a..        '''. 
+00002260: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00002270: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
+00002280: 5f68 6964 6465 6e28 7365 6c66 2c20 7072  _hidden(self, pr
+00002290: 6f70 6572 7479 2920 2d3e 2062 6f6f 6c3a  operty) -> bool:
+000022a0: 0a20 2020 2020 2020 2027 2727 2043 6865  .        ''' Che
+000022b0: 636b 2069 6620 6120 7072 6f70 6572 7479  ck if a property
+000022c0: 2069 7320 6869 6464 656e 2e0a 0a20 2020   is hidden...   
+000022d0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+000022e0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+000022f0: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
+00002300: 2070 726f 7065 7274 7920 6973 2068 6964   property is hid
+00002310: 6465 6e2e 0a20 2020 2020 2020 2027 2727  den..        '''
+00002320: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002330: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+00002340: 7479 5f6f 7665 7272 6964 6162 6c65 5f6c  ty_overridable_l
+00002350: 6962 7261 7279 2873 656c 662c 2070 726f  ibrary(self, pro
+00002360: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
+00002370: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
+00002380: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
+00002390: 6973 206f 7665 7272 6964 6162 6c65 2e0a  is overridable..
+000023a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000023b0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+000023c0: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
+000023d0: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+000023e0: 206f 7665 7272 6964 6162 6c65 2e0a 2020   overridable..  
+000023f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00002400: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00002410: 6973 5f70 726f 7065 7274 795f 7265 6164  is_property_read
+00002420: 6f6e 6c79 2873 656c 662c 2070 726f 7065  only(self, prope
+00002430: 7274 7929 202d 3e20 626f 6f6c 3a0a 2020  rty) -> bool:.  
+00002440: 2020 2020 2020 2727 2720 4368 6563 6b20        ''' Check 
+00002450: 6966 2061 2070 726f 7065 7274 7920 6973  if a property is
+00002460: 2072 6561 646f 6e6c 792e 0a0a 2020 2020   readonly...    
+00002470: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00002480: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002490: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+000024a0: 7072 6f70 6572 7479 2069 7320 7265 6164  property is read
+000024b0: 6f6e 6c79 2028 6e6f 7420 7772 6974 6162  only (not writab
+000024c0: 6c65 292e 0a20 2020 2020 2020 2027 2727  le)..        '''
+000024d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000024e0: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+000024f0: 7479 5f73 6574 2873 656c 662c 2070 726f  ty_set(self, pro
+00002500: 7065 7274 792c 0a20 2020 2020 2020 2020  perty,.         
+00002510: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00002520: 686f 7374 3a20 7479 7069 6e67 2e4f 7074  host: typing.Opt
+00002530: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
+00002540: 7565 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ue) -> bool:.   
+00002550: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
+00002560: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
+00002570: 7365 742c 2075 7365 2066 6f72 2074 6573  set, use for tes
+00002580: 7469 6e67 206f 7065 7261 746f 7220 7072  ting operator pr
+00002590: 6f70 6572 7469 6573 2e0a 0a20 2020 2020  operties...     
+000025a0: 2020 203a 7061 7261 6d20 6768 6f73 743a     :param ghost:
+000025b0: 2055 7365 6420 666f 7220 6f70 6572 6174   Used for operat
+000025c0: 6f72 7320 7468 6174 2072 652d 7275 6e20  ors that re-run 
+000025d0: 7769 7468 2070 7265 7669 6f75 7320 7365  with previous se
+000025e0: 7474 696e 6773 2e20 496e 2074 6869 7320  ttings. In this 
+000025f0: 6361 7365 2074 6865 2070 726f 7065 7274  case the propert
+00002600: 7920 6973 206e 6f74 206d 6172 6b65 6420  y is not marked 
+00002610: 6173 2073 6574 2c20 7965 7420 7468 6520  as set, yet the 
+00002620: 7661 6c75 6520 6672 6f6d 2074 6865 2070  value from the p
+00002630: 7265 7669 6f75 7320 6578 6563 7574 696f  revious executio
+00002640: 6e20 6973 2075 7365 642e 2049 6e20 7261  n is used. In ra
+00002650: 7265 2063 6173 6573 2079 6f75 206d 6179  re cases you may
+00002660: 2077 616e 7420 746f 2073 6574 2074 6869   want to set thi
+00002670: 7320 6f70 7469 6f6e 2074 6f20 6661 6c73  s option to fals
+00002680: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+00002690: 2067 686f 7374 3a20 7479 7069 6e67 2e4f   ghost: typing.O
+000026a0: 7074 696f 6e61 6c5b 626f 6f6c 5d0a 2020  ptional[bool].  
+000026b0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+000026c0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+000026d0: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
+000026e0: 6520 7072 6f70 6572 7479 2068 6173 2062  e property has b
+000026f0: 6565 6e20 7365 742e 0a20 2020 2020 2020  een set..       
+00002700: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002710: 730a 0a20 2020 2064 6566 2069 7465 6d73  s..    def items
+00002720: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+00002730: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
+00002740: 2720 5265 7475 726e 7320 7468 6520 6974  ' Returns the it
+00002750: 656d 7320 6f66 2074 6869 7320 6f62 6a65  ems of this obje
+00002760: 6374 7320 6375 7374 6f6d 2070 726f 7065  cts custom prope
+00002770: 7274 6965 7320 286d 6174 6368 6573 2050  rties (matches P
+00002780: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
+00002790: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
+000027a0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+000027b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000027c0: 7479 7069 6e67 2e41 6e79 0a20 2020 2020  typing.Any.     
+000027d0: 2020 203a 7265 7475 726e 3a20 6375 7374     :return: cust
+000027e0: 6f6d 2070 726f 7065 7274 7920 6b65 792c  om property key,
+000027f0: 2076 616c 7565 2070 6169 7273 2e0a 2020   value pairs..  
+00002800: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00002810: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00002820: 6b65 7966 7261 6d65 5f64 656c 6574 6528  keyframe_delete(
+00002830: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002840: 662c 0a20 2020 2020 2020 2020 2020 2064  f,.            d
+00002850: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
+00002860: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
+00002870: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00002880: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00002890: 616c 5b69 6e74 5d20 3d20 2d31 2c0a 2020  al[int] = -1,.  
+000028a0: 2020 2020 2020 2020 2020 6672 616d 653a            frame:
+000028b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000028c0: 5b66 6c6f 6174 5d20 3d20 2762 7079 2e63  [float] = 'bpy.c
+000028d0: 6f6e 7465 7874 2e73 6365 6e65 2e66 7261  ontext.scene.fra
+000028e0: 6d65 5f63 7572 7265 6e74 272c 0a20 2020  me_current',.   
+000028f0: 2020 2020 2020 2020 2067 726f 7570 3a20           group: 
+00002900: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002910: 7374 725d 203d 2022 2229 202d 3e20 626f  str] = "") -> bo
+00002920: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
+00002930: 5265 6d6f 7665 2061 206b 6579 6672 616d  Remove a keyfram
+00002940: 6520 6672 6f6d 2074 6869 7320 7072 6f70  e from this prop
+00002950: 6572 7469 6573 2066 6375 7276 652e 0a0a  erties fcurve...
+00002960: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00002970: 6174 615f 7061 7468 3a20 7061 7468 2074  ata_path: path t
+00002980: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
+00002990: 6f20 7265 6d6f 7665 2061 206b 6579 2c20  o remove a key, 
+000029a0: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
+000029b0: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
+000029c0: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
+000029d0: 7065 2064 6174 615f 7061 7468 3a20 7479  pe data_path: ty
+000029e0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+000029f0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
+00002a00: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
+00002a10: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
+00002a20: 6572 7479 2074 6f20 7265 6d6f 7665 2061  erty to remove a
+00002a30: 206b 6579 2e20 4465 6661 756c 7473 2074   key. Defaults t
+00002a40: 6f20 2d31 2072 656d 6f76 696e 6720 616c  o -1 removing al
+00002a50: 6c20 696e 6469 6365 7320 6f72 2061 2073  l indices or a s
+00002a60: 696e 676c 6520 6368 616e 6e65 6c20 6966  ingle channel if
+00002a70: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+00002a80: 206e 6f74 2061 6e20 6172 7261 792e 0a20   not an array.. 
+00002a90: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
+00002aa0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+00002ab0: 6e61 6c5b 696e 745d 0a20 2020 2020 2020  nal[int].       
+00002ac0: 203a 7061 7261 6d20 6672 616d 653a 2054   :param frame: T
+00002ad0: 6865 2066 7261 6d65 206f 6e20 7768 6963  he frame on whic
+00002ae0: 6820 7468 6520 6b65 7966 7261 6d65 2069  h the keyframe i
+00002af0: 7320 6465 6c65 7465 642c 2064 6566 6175  s deleted, defau
+00002b00: 6c74 696e 6720 746f 2074 6865 2063 7572  lting to the cur
+00002b10: 7265 6e74 2066 7261 6d65 2e0a 2020 2020  rent frame..    
+00002b20: 2020 2020 3a74 7970 6520 6672 616d 653a      :type frame:
+00002b30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002b40: 5b66 6c6f 6174 5d0a 2020 2020 2020 2020  [float].        
+00002b50: 3a70 6172 616d 2067 726f 7570 3a20 5468  :param group: Th
+00002b60: 6520 6e61 6d65 206f 6620 7468 6520 6772  e name of the gr
+00002b70: 6f75 7020 7468 6520 462d 4375 7276 6520  oup the F-Curve 
+00002b80: 7368 6f75 6c64 2062 6520 6164 6465 6420  should be added 
+00002b90: 746f 2069 6620 6974 2064 6f65 736e 2774  to if it doesn't
+00002ba0: 2065 7869 7374 2079 6574 2e0a 2020 2020   exist yet..    
+00002bb0: 2020 2020 3a74 7970 6520 6772 6f75 703a      :type group:
+00002bc0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002bd0: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
+00002be0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+00002bf0: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
+00002c00: 6573 7320 6f66 206b 6579 6672 616d 6520  ess of keyframe 
+00002c10: 6465 6c65 7469 6f6e 2e0a 2020 2020 2020  deletion..      
+00002c20: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00002c30: 7373 0a0a 2020 2020 6465 6620 6b65 7966  ss..    def keyf
+00002c40: 7261 6d65 5f69 6e73 6572 7428 0a20 2020  rame_insert(.   
+00002c50: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00002c60: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00002c70: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
+00002c80: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
+00002c90: 2020 2020 2020 2020 696e 6465 783a 2074          index: t
+00002ca0: 7970 696e 672e 4f70 7469 6f6e 616c 5b69  yping.Optional[i
+00002cb0: 6e74 5d20 3d20 2d31 2c0a 2020 2020 2020  nt] = -1,.      
+00002cc0: 2020 2020 2020 6672 616d 653a 2074 7970        frame: typ
+00002cd0: 696e 672e 4f70 7469 6f6e 616c 5b66 6c6f  ing.Optional[flo
+00002ce0: 6174 5d20 3d20 2762 7079 2e63 6f6e 7465  at] = 'bpy.conte
+00002cf0: 7874 2e73 6365 6e65 2e66 7261 6d65 5f63  xt.scene.frame_c
+00002d00: 7572 7265 6e74 272c 0a20 2020 2020 2020  urrent',.       
+00002d10: 2020 2020 2067 726f 7570 3a20 7479 7069       group: typi
+00002d20: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00002d30: 203d 2022 222c 0a20 2020 2020 2020 2020   = "",.         
+00002d40: 2020 206f 7074 696f 6e73 3a20 7479 7069     options: typi
+00002d50: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+00002d60: 6e67 2e41 6e79 5d20 3d20 2773 6574 2829  ng.Any] = 'set()
+00002d70: 2729 202d 3e20 626f 6f6c 3a0a 2020 2020  ') -> bool:.    
+00002d80: 2020 2020 2727 2720 496e 7365 7274 2061      ''' Insert a
+00002d90: 206b 6579 6672 616d 6520 6f6e 2074 6865   keyframe on the
+00002da0: 2070 726f 7065 7274 7920 6769 7665 6e2c   property given,
+00002db0: 2061 6464 696e 6720 6663 7572 7665 7320   adding fcurves 
+00002dc0: 616e 6420 616e 696d 6174 696f 6e20 6461  and animation da
+00002dd0: 7461 2077 6865 6e20 6e65 6365 7373 6172  ta when necessar
+00002de0: 792e 2054 6869 7320 6973 2074 6865 206d  y. This is the m
+00002df0: 6f73 7420 7369 6d70 6c65 2065 7861 6d70  ost simple examp
+00002e00: 6c65 206f 6620 696e 7365 7274 696e 6720  le of inserting 
+00002e10: 6120 6b65 7966 7261 6d65 2066 726f 6d20  a keyframe from 
+00002e20: 7079 7468 6f6e 2e20 4e6f 7465 2074 6861  python. Note tha
+00002e30: 7420 7768 656e 206b 6579 696e 6720 6461  t when keying da
+00002e40: 7461 2070 6174 6873 2077 6869 6368 2063  ta paths which c
+00002e50: 6f6e 7461 696e 206e 6573 7465 6420 7072  ontain nested pr
+00002e60: 6f70 6572 7469 6573 2074 6869 7320 6d75  operties this mu
+00002e70: 7374 2062 6520 646f 6e65 2066 726f 6d20  st be done from 
+00002e80: 7468 6520 6049 4460 2073 7562 636c 6173  the `ID` subclas
+00002e90: 732c 2069 6e20 7468 6973 2063 6173 6520  s, in this case 
+00002ea0: 7468 6520 6041 726d 6174 7572 6560 2072  the `Armature` r
+00002eb0: 6174 6865 7220 7468 616e 2074 6865 2062  ather than the b
+00002ec0: 6f6e 652e 0a0a 2020 2020 2020 2020 3a70  one...        :p
+00002ed0: 6172 616d 2064 6174 615f 7061 7468 3a20  aram data_path: 
+00002ee0: 7061 7468 2074 6f20 7468 6520 7072 6f70  path to the prop
+00002ef0: 6572 7479 2074 6f20 6b65 792c 2061 6e61  erty to key, ana
+00002f00: 6c6f 676f 7573 2074 6f20 7468 6520 6663  logous to the fc
+00002f10: 7572 7665 2773 2064 6174 6120 7061 7468  urve's data path
+00002f20: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00002f30: 6461 7461 5f70 6174 683a 2074 7970 696e  data_path: typin
+00002f40: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00002f50: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00002f60: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
+00002f70: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
+00002f80: 7920 746f 206b 6579 2e20 4465 6661 756c  y to key. Defaul
+00002f90: 7473 2074 6f20 2d31 2077 6869 6368 2077  ts to -1 which w
+00002fa0: 696c 6c20 6b65 7920 616c 6c20 696e 6469  ill key all indi
+00002fb0: 6365 7320 6f72 2061 2073 696e 676c 6520  ces or a single 
+00002fc0: 6368 616e 6e65 6c20 6966 2074 6865 2070  channel if the p
+00002fd0: 726f 7065 7274 7920 6973 206e 6f74 2061  roperty is not a
+00002fe0: 6e20 6172 7261 792e 0a20 2020 2020 2020  n array..       
+00002ff0: 203a 7479 7065 2069 6e64 6578 3a20 7479   :type index: ty
+00003000: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
+00003010: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
+00003020: 6d20 6672 616d 653a 2054 6865 2066 7261  m frame: The fra
+00003030: 6d65 206f 6e20 7768 6963 6820 7468 6520  me on which the 
+00003040: 6b65 7966 7261 6d65 2069 7320 696e 7365  keyframe is inse
+00003050: 7274 6564 2c20 6465 6661 756c 7469 6e67  rted, defaulting
+00003060: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
+00003070: 6672 616d 652e 0a20 2020 2020 2020 203a  frame..        :
+00003080: 7479 7065 2066 7261 6d65 3a20 7479 7069  type frame: typi
+00003090: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
+000030a0: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
+000030b0: 6d20 6772 6f75 703a 2054 6865 206e 616d  m group: The nam
+000030c0: 6520 6f66 2074 6865 2067 726f 7570 2074  e of the group t
+000030d0: 6865 2046 2d43 7572 7665 2073 686f 756c  he F-Curve shoul
+000030e0: 6420 6265 2061 6464 6564 2074 6f20 6966  d be added to if
+000030f0: 2069 7420 646f 6573 6e27 7420 6578 6973   it doesn't exis
+00003100: 7420 7965 742e 0a20 2020 2020 2020 203a  t yet..        :
+00003110: 7479 7065 2067 726f 7570 3a20 7479 7069  type group: typi
+00003120: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003130: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003140: 666c 6167 3a20 0a20 2020 2020 2020 203a  flag: .        :
+00003150: 7479 7065 2066 6c61 673a 2074 7970 696e  type flag: typin
+00003160: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00003170: 672e 5365 745d 0a20 2020 2020 2020 203a  g.Set].        :
+00003180: 7061 7261 6d20 6f70 7469 6f6e 733a 2020  param options:  
+00003190: 2d20 6060 494e 5345 5254 4b45 595f 4e45  - ``INSERTKEY_NE
+000031a0: 4544 4544 6060 204f 6e6c 7920 696e 7365  EDED`` Only inse
+000031b0: 7274 206b 6579 6672 616d 6573 2077 6865  rt keyframes whe
+000031c0: 7265 2074 6865 7927 7265 206e 6565 6465  re they're neede
+000031d0: 6420 696e 2074 6865 2072 656c 6576 616e  d in the relevan
+000031e0: 7420 462d 4375 7276 6573 2e20 2d20 6060  t F-Curves. - ``
+000031f0: 494e 5345 5254 4b45 595f 5649 5355 414c  INSERTKEY_VISUAL
+00003200: 6060 2049 6e73 6572 7420 6b65 7966 7261  `` Insert keyfra
+00003210: 6d65 7320 6261 7365 6420 6f6e 2027 7669  mes based on 'vi
+00003220: 7375 616c 2074 7261 6e73 666f 726d 7327  sual transforms'
+00003230: 2e20 2d20 6060 494e 5345 5254 4b45 595f  . - ``INSERTKEY_
+00003240: 5859 5a5f 544f 5f52 4742 6060 2043 6f6c  XYZ_TO_RGB`` Col
+00003250: 6f72 2066 6f72 206e 6577 6c79 2061 6464  or for newly add
+00003260: 6564 2074 7261 6e73 666f 726d 6174 696f  ed transformatio
+00003270: 6e20 462d 4375 7276 6573 2028 4c6f 6361  n F-Curves (Loca
+00003280: 7469 6f6e 2c20 526f 7461 7469 6f6e 2c20  tion, Rotation, 
+00003290: 5363 616c 6529 2069 7320 6261 7365 6420  Scale) is based 
+000032a0: 6f6e 2074 6865 2074 7261 6e73 666f 726d  on the transform
+000032b0: 2061 7869 732e 202d 2060 6049 4e53 4552   axis. - ``INSER
+000032c0: 544b 4559 5f52 4550 4c41 4345 6060 204f  TKEY_REPLACE`` O
+000032d0: 6e6c 7920 7265 706c 6163 6520 616c 7265  nly replace alre
+000032e0: 6164 7920 6578 6973 7469 6e67 206b 6579  ady existing key
+000032f0: 6672 616d 6573 2e20 2d20 6060 494e 5345  frames. - ``INSE
+00003300: 5254 4b45 595f 4156 4149 4c41 424c 4560  RTKEY_AVAILABLE`
+00003310: 6020 4f6e 6c79 2069 6e73 6572 7420 696e  ` Only insert in
+00003320: 746f 2061 6c72 6561 6479 2065 7869 7374  to already exist
+00003330: 696e 6720 462d 4375 7276 6573 2e20 2d20  ing F-Curves. - 
+00003340: 6060 494e 5345 5254 4b45 595f 4359 434c  ``INSERTKEY_CYCL
+00003350: 455f 4157 4152 4560 6020 5461 6b65 2063  E_AWARE`` Take c
+00003360: 7963 6c69 6320 6578 7472 6170 6f6c 6174  yclic extrapolat
+00003370: 696f 6e20 696e 746f 2061 6363 6f75 6e74  ion into account
+00003380: 2028 4379 636c 652d 4177 6172 6520 4b65   (Cycle-Aware Ke
+00003390: 7969 6e67 206f 7074 696f 6e29 2e0a 2020  ying option)..  
+000033a0: 2020 2020 2020 3a74 7970 6520 6f70 7469        :type opti
+000033b0: 6f6e 733a 2074 7970 696e 672e 4f70 7469  ons: typing.Opti
+000033c0: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
+000033d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000033e0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+000033f0: 6574 7572 6e3a 2053 7563 6365 7373 206f  eturn: Success o
+00003400: 6620 6b65 7966 7261 6d65 2069 6e73 6572  f keyframe inser
+00003410: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
+00003420: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003430: 2020 2020 6465 6620 6b65 7973 2873 656c      def keys(sel
+00003440: 6629 202d 3e20 7479 7069 6e67 2e41 6e79  f) -> typing.Any
+00003450: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
+00003460: 7475 726e 7320 7468 6520 6b65 7973 206f  turns the keys o
+00003470: 6620 7468 6973 206f 626a 6563 7473 2063  f this objects c
+00003480: 7573 746f 6d20 7072 6f70 6572 7469 6573  ustom properties
+00003490: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
+000034a0: 2773 2064 6963 7469 6f6e 6172 7920 6675  's dictionary fu
+000034b0: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
+000034c0: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
+000034d0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
+000034e0: 672e 416e 790a 2020 2020 2020 2020 3a72  g.Any.        :r
+000034f0: 6574 7572 6e3a 2063 7573 746f 6d20 7072  eturn: custom pr
+00003500: 6f70 6572 7479 206b 6579 732e 0a20 2020  operty keys..   
+00003510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003520: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
+00003530: 6174 685f 6672 6f6d 5f69 6428 7365 6c66  ath_from_id(self
+00003540: 2c20 7072 6f70 6572 7479 3a20 7479 7069  , property: typi
+00003550: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003560: 203d 2022 2229 202d 3e20 7374 723a 0a20   = "") -> str:. 
+00003570: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00003580: 6e73 2074 6865 2064 6174 6120 7061 7468  ns the data path
+00003590: 2066 726f 6d20 7468 6520 4944 2074 6f20   from the ID to 
+000035a0: 7468 6973 206f 626a 6563 7420 2873 7472  this object (str
+000035b0: 696e 6729 2e0a 0a20 2020 2020 2020 203a  ing)...        :
+000035c0: 7061 7261 6d20 7072 6f70 6572 7479 3a20  param property: 
+000035d0: 4f70 7469 6f6e 616c 2070 726f 7065 7274  Optional propert
+000035e0: 7920 6e61 6d65 2077 6869 6368 2063 616e  y name which can
+000035f0: 2062 6520 7573 6564 2069 6620 7468 6520   be used if the 
+00003600: 7061 7468 2069 7320 746f 2061 2070 726f  path is to a pro
+00003610: 7065 7274 7920 6f66 2074 6869 7320 6f62  perty of this ob
+00003620: 6a65 6374 2e0a 2020 2020 2020 2020 3a74  ject..        :t
+00003630: 7970 6520 7072 6f70 6572 7479 3a20 7479  ype property: ty
+00003640: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00003650: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
+00003660: 653a 2073 7472 0a20 2020 2020 2020 203a  e: str.        :
+00003670: 7265 7475 726e 3a20 6062 7079 2e74 7970  return: `bpy.typ
+00003680: 6573 2e62 7079 5f73 7472 7563 742e 6964  es.bpy_struct.id
+00003690: 5f64 6174 6160 2074 6f20 7468 6973 2073  _data` to this s
+000036a0: 7472 7563 7420 616e 6420 7072 6f70 6572  truct and proper
+000036b0: 7479 2028 7768 656e 2067 6976 656e 292e  ty (when given).
+000036c0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000036d0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000036e0: 6566 2070 6174 685f 7265 736f 6c76 6528  ef path_resolve(
+000036f0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00003700: 2020 2020 2020 2020 2020 2070 6174 683a             path:
+00003710: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003720: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
+00003730: 2020 2020 2020 2020 2020 2020 636f 6572              coer
+00003740: 6365 3a20 7479 7069 6e67 2e4f 7074 696f  ce: typing.Optio
+00003750: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
+00003760: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
+00003770: 6574 7572 6e73 2074 6865 2070 726f 7065  eturns the prope
+00003780: 7274 7920 6672 6f6d 2074 6865 2070 6174  rty from the pat
+00003790: 682c 2072 6169 7365 2061 6e20 6578 6365  h, raise an exce
+000037a0: 7074 696f 6e20 7768 656e 206e 6f74 2066  ption when not f
+000037b0: 6f75 6e64 2e0a 0a20 2020 2020 2020 203a  ound...        :
+000037c0: 7061 7261 6d20 7061 7468 3a20 7061 7468  param path: path
+000037d0: 2077 6869 6368 2074 6869 7320 7072 6f70   which this prop
+000037e0: 6572 7479 2072 6573 6f6c 7665 732e 0a20  erty resolves.. 
+000037f0: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
+00003800: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00003810: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00003820: 3a70 6172 616d 2063 6f65 7263 653a 206f  :param coerce: o
+00003830: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+00003840: 2c20 7768 656e 2054 7275 652c 2074 6865  , when True, the
+00003850: 2070 726f 7065 7274 7920 7769 6c6c 2062   property will b
+00003860: 6520 636f 6e76 6572 7465 6420 696e 746f  e converted into
+00003870: 2069 7473 2050 7974 686f 6e20 7265 7072   its Python repr
+00003880: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
+00003890: 2020 2020 3a74 7970 6520 636f 6572 6365      :type coerce
+000038a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000038b0: 6c5b 626f 6f6c 5d0a 2020 2020 2020 2020  l[bool].        
+000038c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000038d0: 0a0a 2020 2020 6465 6620 706f 7028 7365  ..    def pop(se
+000038e0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+000038f0: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
+00003900: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
+00003910: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
+00003920: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00003930: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
+00003940: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
+00003950: 2052 656d 6f76 6520 616e 6420 7265 7475   Remove and retu
+00003960: 726e 2074 6865 2076 616c 7565 206f 6620  rn the value of 
+00003970: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
+00003980: 7274 7920 6173 7369 676e 6564 2074 6f20  rty assigned to 
+00003990: 6b65 7920 6f72 2064 6566 6175 6c74 2077  key or default w
+000039a0: 6865 6e20 6e6f 7420 666f 756e 6420 286d  hen not found (m
+000039b0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
+000039c0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
+000039d0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+000039e0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+000039f0: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
+00003a00: 6b65 7920 6173 736f 6369 6174 6564 2077  key associated w
+00003a10: 6974 6820 7468 6520 6375 7374 6f6d 2070  ith the custom p
+00003a20: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
+00003a30: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
+00003a40: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003a50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003a60: 6465 6661 756c 743a 204f 7074 696f 6e61  default: Optiona
+00003a70: 6c20 6172 6775 6d65 6e74 2066 6f72 2074  l argument for t
+00003a80: 6865 2076 616c 7565 2074 6f20 7265 7475  he value to retu
+00003a90: 726e 2069 6620 2a6b 6579 2a20 6973 206e  rn if *key* is n
+00003aa0: 6f74 2066 6f75 6e64 2e0a 2020 2020 2020  ot found..      
+00003ab0: 2020 3a74 7970 6520 6465 6661 756c 743a    :type default:
+00003ac0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003ad0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
+00003ae0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003af0: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
+00003b00: 726f 7065 7274 795f 6f76 6572 7269 6461  roperty_overrida
+00003b10: 626c 655f 6c69 6272 6172 795f 7365 7428  ble_library_set(
+00003b20: 7365 6c66 2c20 7072 6f70 6572 7479 2c20  self, property, 
+00003b30: 6f76 6572 7269 6461 626c 6529 202d 3e20  overridable) -> 
+00003b40: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00003b50: 2720 4465 6669 6e65 2061 2070 726f 7065  ' Define a prope
+00003b60: 7274 7920 6173 206f 7665 7272 6964 6162  rty as overridab
+00003b70: 6c65 206f 7220 6e6f 7420 286f 6e6c 7920  le or not (only 
+00003b80: 666f 7220 6375 7374 6f6d 2070 726f 7065  for custom prope
+00003b90: 7274 6965 7321 292e 0a0a 2020 2020 2020  rties!)...      
+00003ba0: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
+00003bb0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003bc0: 5472 7565 2077 6865 6e20 7468 6520 6f76  True when the ov
+00003bd0: 6572 7269 6461 626c 6520 7374 6174 7573  erridable status
+00003be0: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00003bf0: 2077 6173 2073 7563 6365 7373 6675 6c6c   was successfull
+00003c00: 7920 7365 742e 0a20 2020 2020 2020 2027  y set..        '
+00003c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00003c20: 0a20 2020 2064 6566 2070 726f 7065 7274  .    def propert
+00003c30: 795f 756e 7365 7428 7365 6c66 2c20 7072  y_unset(self, pr
+00003c40: 6f70 6572 7479 293a 0a20 2020 2020 2020  operty):.       
+00003c50: 2027 2727 2055 6e73 6574 2061 2070 726f   ''' Unset a pro
+00003c60: 7065 7274 792c 2077 696c 6c20 7573 6520  perty, will use 
+00003c70: 6465 6661 756c 7420 7661 6c75 6520 6166  default value af
+00003c80: 7465 7277 6172 642e 0a0a 2020 2020 2020  terward...      
+00003c90: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00003ca0: 7373 0a0a 2020 2020 6465 6620 7479 7065  ss..    def type
+00003cb0: 5f72 6563 6173 7428 7365 6c66 2920 2d3e  _recast(self) ->
+00003cc0: 2027 6270 795f 7374 7275 6374 273a 0a20   'bpy_struct':. 
+00003cd0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00003ce0: 6e20 6120 6e65 7720 696e 7374 616e 6365  n a new instance
+00003cf0: 2c20 7468 6973 2069 7320 6e65 6564 6564  , this is needed
+00003d00: 2062 6563 6175 7365 2074 7970 6573 2073   because types s
+00003d10: 7563 6820 6173 2074 6578 7475 7265 7320  uch as textures 
+00003d20: 6361 6e20 6265 2063 6861 6e67 6564 2061  can be changed a
+00003d30: 7420 7275 6e74 696d 652e 0a0a 2020 2020  t runtime...    
+00003d40: 2020 2020 3a72 7479 7065 3a20 2762 7079      :rtype: 'bpy
+00003d50: 5f73 7472 7563 7427 0a20 2020 2020 2020  _struct'.       
+00003d60: 203a 7265 7475 726e 3a20 6120 6e65 7720   :return: a new 
+00003d70: 696e 7374 616e 6365 206f 6620 7468 6973  instance of this
+00003d80: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+00003d90: 2074 7970 6520 696e 6974 6961 6c69 7a65   type initialize
+00003da0: 6420 6167 6169 6e2e 0a20 2020 2020 2020  d again..       
+00003db0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003dc0: 730a 0a20 2020 2064 6566 2076 616c 7565  s..    def value
+00003dd0: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
+00003de0: 672e 416e 793a 0a20 2020 2020 2020 2027  g.Any:.        '
+00003df0: 2727 2052 6574 7572 6e73 2074 6865 2076  '' Returns the v
+00003e00: 616c 7565 7320 6f66 2074 6869 7320 6f62  alues of this ob
+00003e10: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
+00003e20: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
+00003e30: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
+00003e40: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
+00003e50: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+00003e60: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00003e70: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
+00003e80: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
+00003e90: 7374 6f6d 2070 726f 7065 7274 7920 7661  stom property va
+00003ea0: 6c75 6573 2e0a 2020 2020 2020 2020 2727  lues..        ''
+00003eb0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003ec0: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00003ed0: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+00003ee0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00003ef0: 2073 7472 5d29 202d 3e20 2774 7970 696e   str]) -> 'typin
+00003f00: 672e 416e 7927 3a0a 2020 2020 2020 2020  g.Any':.        
+00003f10: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+00003f20: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+00003f30: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00003f40: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00003f50: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00003f60: 7970 653a 2027 7479 7069 6e67 2e41 6e79  ype: 'typing.Any
+00003f70: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
+00003f80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00003f90: 6465 6620 5f5f 7365 7469 7465 6d5f 5f28  def __setitem__(
+00003fa0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00003fb0: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00003fc0: 5d2c 2076 616c 7565 3a20 2774 7970 696e  ], value: 'typin
+00003fd0: 672e 416e 7927 293a 0a20 2020 2020 2020  g.Any'):.       
+00003fe0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00003ff0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
+00004000: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
+00004010: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00004020: 2073 7472 5d0a 2020 2020 2020 2020 3a70   str].        :p
+00004030: 6172 616d 2076 616c 7565 3a20 0a20 2020  aram value: .   
+00004040: 2020 2020 203a 7479 7065 2076 616c 7565       :type value
+00004050: 3a20 2774 7970 696e 672e 416e 7927 0a20  : 'typing.Any'. 
+00004060: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00004070: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00004080: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
+00004090: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
+000040a0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
+000040b0: 2d3e 2027 7479 7069 6e67 2e41 6e79 273a  -> 'typing.Any':
+000040c0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000040d0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+000040e0: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
+000040f0: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
+00004100: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
+00004110: 2020 2020 2020 3a72 7479 7065 3a20 2774        :rtype: 't
+00004120: 7970 696e 672e 416e 7927 0a20 2020 2020  yping.Any'.     
 00004130: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 00004140: 6173 730a 0a0a 636c 6173 7320 6270 795f  ass...class bpy_
 00004150: 7072 6f70 5f61 7272 6179 2874 7970 696e  prop_array(typin
 00004160: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
 00004170: 6354 7970 655d 293a 0a20 2020 2064 6566  cType]):.    def
 00004180: 2066 6f72 6561 6368 5f67 6574 2873 656c   foreach_get(sel
 00004190: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):. 
@@ -23163,16 +23163,16 @@
 0005a7a0: 3a20 2745 7665 6e74 272c 0a20 2020 2020  : 'Event',.     
 0005a7b0: 2020 2020 2020 2020 2074 7765 616b 3a20           tweak: 
 0005a7c0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
 0005a7d0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
 0005a7e0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 0005a7f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 0005a800: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-0005a810: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
-0005a820: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
+0005a810: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
+0005a820: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
 0005a830: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
 0005a840: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 0005a850: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 0005a860: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 0005a870: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0005a880: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 0005a890: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
@@ -23181,42 +23181,42 @@
 0005a8c0: 616b 3a20 5477 6561 6b0a 2020 2020 2020  ak: Tweak.      
 0005a8d0: 2020 3a74 7970 6520 7477 6561 6b3a 2074    :type tweak: t
 0005a8e0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
 0005a8f0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
 0005a900: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0005a910: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 0005a920: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0005a930: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-0005a940: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
+0005a930: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+0005a940: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
 0005a950: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 0005a960: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 0005a970: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 0005a980: 2020 2064 6566 2073 6574 7570 2873 656c     def setup(sel
 0005a990: 6629 3a0a 2020 2020 2020 2020 2727 2720  f):.        ''' 
 0005a9a0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
 0005a9b0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0005a9c0: 6465 6620 696e 766f 6b65 2873 656c 662c  def invoke(self,
 0005a9d0: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0005a9e0: 7874 272c 2065 7665 6e74 3a20 2745 7665  xt', event: 'Eve
 0005a9f0: 6e74 270a 2020 2020 2020 2020 2020 2020  nt'.            
 0005aa00: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 0005aa10: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0005aa20: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-0005aa30: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+0005aa20: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+0005aa30: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
 0005aa40: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
 0005aa50: 6172 616d 2063 6f6e 7465 7874 3a20 0a20  aram context: . 
 0005aa60: 2020 2020 2020 203a 7479 7065 2063 6f6e         :type con
 0005aa70: 7465 7874 3a20 2743 6f6e 7465 7874 270a  text: 'Context'.
 0005aa80: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 0005aa90: 7665 6e74 3a20 0a20 2020 2020 2020 203a  vent: .        :
 0005aaa0: 7479 7065 2065 7665 6e74 3a20 2745 7665  type event: 'Eve
 0005aab0: 6e74 270a 2020 2020 2020 2020 3a72 7479  nt'.        :rty
 0005aac0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-0005aad0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+0005aad0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 0005aaf0: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 0005ab00: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 0005ab10: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 0005ab20: 6173 730a 0a20 2020 2064 6566 2065 7869  ass..    def exi
 0005ab30: 7428 7365 6c66 2c20 636f 6e74 6578 743a  t(self, context:
 0005ab40: 2027 436f 6e74 6578 7427 2c20 6361 6e63   'Context', canc
 0005ab50: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
@@ -27324,24 +27324,24 @@
 0006abb0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
 0006abc0: 650a 2020 2020 2727 2720 0a0a 2020 2020  e.    ''' ..    
 0006abd0: 3a74 7970 653a 2074 7970 696e 672e 556e  :type: typing.Un
 0006abe0: 696f 6e5b 7374 722c 2074 7970 696e 672e  ion[str, typing.
 0006abf0: 416e 795d 0a20 2020 2027 2727 0a0a 2020  Any].    '''..  
 0006ac00: 2020 626c 5f6f 7074 696f 6e73 3a20 7479    bl_options: ty
 0006ac10: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0006ac20: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-0006ac30: 6e67 2e53 6574 5b73 7472 5d5d 203d 204e  ng.Set[str]] = N
+0006ac20: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+0006ac30: 6e67 2e53 6574 5b69 6e74 5d5d 203d 204e  ng.Set[int]] = N
 0006ac40: 6f6e 650a 2020 2020 2727 2720 4b65 7969  one.    ''' Keyi
 0006ac50: 6e67 2053 6574 206f 7074 696f 6e73 2074  ng Set options t
 0006ac60: 6f20 7573 6520 7768 656e 2069 6e73 6572  o use when inser
 0006ac70: 7469 6e67 206b 6579 6672 616d 6573 0a0a  ting keyframes..
 0006ac80: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 0006ac90: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0006aca0: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-0006acb0: 5365 745b 7374 725d 5d0a 2020 2020 2727  Set[str]].    ''
+0006aca0: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+0006acb0: 5365 745b 696e 745d 5d0a 2020 2020 2727  Set[int]].    ''
 0006acc0: 270a 0a20 2020 2064 6566 2070 6f6c 6c28  '..    def poll(
 0006acd0: 7365 6c66 2c20 636f 6e74 6578 743a 2074  self, context: t
 0006ace0: 7970 696e 672e 4f70 7469 6f6e 616c 5b27  yping.Optional['
 0006acf0: 436f 6e74 6578 7427 5d29 3a0a 2020 2020  Context']):.    
 0006ad00: 2020 2020 2727 2720 5465 7374 2069 6620      ''' Test if 
 0006ad10: 4b65 7969 6e67 2053 6574 2063 616e 2062  Keying Set can b
 0006ad20: 6520 7573 6564 206f 7220 6e6f 740a 0a20  e used or not.. 
@@ -28084,23 +28084,23 @@
 0006db30: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
 0006db40: 6e79 5d20 3d20 4e6f 6e65 0a20 2020 2027  ny] = None.    '
 0006db50: 2727 200a 0a20 2020 203a 7479 7065 3a20  '' ..    :type: 
 0006db60: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 0006db70: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 0006db80: 2020 2727 270a 0a20 2020 2062 6c5f 6f70    '''..    bl_op
 0006db90: 7469 6f6e 733a 2074 7970 696e 672e 556e  tions: typing.Un
-0006dba0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-0006dbb0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-0006dbc0: 7374 725d 5d20 3d20 4e6f 6e65 0a20 2020  str]] = None.   
+0006dba0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+0006dbb0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+0006dbc0: 696e 745d 5d20 3d20 4e6f 6e65 0a20 2020  int]] = None.   
 0006dbd0: 2027 2727 204f 7074 696f 6e73 2066 6f72   ''' Options for
 0006dbe0: 2074 6869 7320 6f70 6572 6174 6f72 2074   this operator t
 0006dbf0: 7970 650a 0a20 2020 203a 7479 7065 3a20  ype..    :type: 
 0006dc00: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-0006dc10: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-0006dc20: 7069 6e67 2e53 6574 5b73 7472 5d5d 0a20  ping.Set[str]]. 
+0006dc10: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+0006dc20: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 0006dc30: 2020 2027 2727 0a0a 2020 2020 626c 5f74     '''..    bl_t
 0006dc40: 7261 6e73 6c61 7469 6f6e 5f63 6f6e 7465  ranslation_conte
 0006dc50: 7874 3a20 7479 7069 6e67 2e55 6e69 6f6e  xt: typing.Union
 0006dc60: 5b73 7472 2c20 7479 7069 6e67 2e41 6e79  [str, typing.Any
 0006dc70: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 0006dc80: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 0006dc90: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
@@ -28136,26 +28136,26 @@
 0006de70: 6573 2720 3d20 4e6f 6e65 0a20 2020 2027  es' = None.    '
 0006de80: 2727 200a 0a20 2020 203a 7479 7065 3a20  '' ..    :type: 
 0006de90: 274f 7065 7261 746f 7250 726f 7065 7274  'OperatorPropert
 0006dea0: 6965 7327 0a20 2020 2027 2727 0a0a 2020  ies'.    '''..  
 0006deb0: 2020 6465 6620 7265 706f 7274 2873 656c    def report(sel
 0006dec0: 662c 2074 7970 653a 2074 7970 696e 672e  f, type: typing.
 0006ded0: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-0006dee0: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-0006def0: 745b 7374 725d 5d2c 0a20 2020 2020 2020  t[str]],.       
+0006dee0: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+0006def0: 745b 696e 745d 5d2c 0a20 2020 2020 2020  t[int]],.       
 0006df00: 2020 2020 2020 2020 6d65 7373 6167 653a          message:
 0006df10: 2074 7970 696e 672e 556e 696f 6e5b 7374   typing.Union[st
 0006df20: 722c 2074 7970 696e 672e 416e 795d 293a  r, typing.Any]):
 0006df30: 0a20 2020 2020 2020 2027 2727 2072 6570  .        ''' rep
 0006df40: 6f72 740a 0a20 2020 2020 2020 203a 7061  ort..        :pa
 0006df50: 7261 6d20 7479 7065 3a20 5479 7065 0a20  ram type: Type. 
 0006df60: 2020 2020 2020 203a 7479 7065 2074 7970         :type typ
 0006df70: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0006df80: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-0006df90: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+0006df80: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+0006df90: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 0006dfa0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
 0006dfb0: 206d 6573 7361 6765 3a20 5265 706f 7274   message: Report
 0006dfc0: 204d 6573 7361 6765 0a20 2020 2020 2020   Message.       
 0006dfd0: 203a 7479 7065 206d 6573 7361 6765 3a20   :type message: 
 0006dfe0: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 0006dff0: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 0006e000: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
@@ -37207,23 +37207,23 @@
 00091560: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
 00091570: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 00091580: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 00091590: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 000915a0: 2e41 6e79 5d0a 2020 2020 2727 270a 0a20  .Any].    '''.. 
 000915b0: 2020 2062 6c5f 6f70 7469 6f6e 733a 2074     bl_options: t
 000915c0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-000915d0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-000915e0: 696e 672e 5365 745b 7374 725d 5d20 3d20  ing.Set[str]] = 
+000915d0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+000915e0: 696e 672e 5365 745b 696e 745d 5d20 3d20  ing.Set[int]] = 
 000915f0: 4e6f 6e65 0a20 2020 2027 2727 204f 7074  None.    ''' Opt
 00091600: 696f 6e73 2066 6f72 2074 6869 7320 6f70  ions for this op
 00091610: 6572 6174 6f72 2074 7970 650a 0a20 2020  erator type..   
 00091620: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 00091630: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-00091640: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-00091650: 5b73 7472 5d5d 0a20 2020 2027 2727 0a0a  [str]].    '''..
+00091640: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+00091650: 5b69 6e74 5d5d 0a20 2020 2027 2727 0a0a  [int]].    '''..
 00091660: 2020 2020 626c 5f74 7261 6e73 6c61 7469      bl_translati
 00091670: 6f6e 5f63 6f6e 7465 7874 3a20 7479 7069  on_context: typi
 00091680: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 00091690: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
 000916a0: 0a20 2020 2027 2727 200a 0a20 2020 203a  .    ''' ..    :
 000916b0: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
 000916c0: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
@@ -37290,26 +37290,26 @@
 00091a90: 656e 2065 7870 616e 6469 6e67 2061 6e20  en expanding an 
 00091aa0: 6f70 6572 6174 6f72 2069 6e74 6f20 6120  operator into a 
 00091ab0: 6d65 6e75 2e0a 0a20 2020 203a 7479 7065  menu...    :type
 00091ac0: 3a20 7374 720a 2020 2020 2727 270a 0a20  : str.    '''.. 
 00091ad0: 2020 2064 6566 2072 6570 6f72 7428 7365     def report(se
 00091ae0: 6c66 2c20 7479 7065 3a20 7479 7069 6e67  lf, type: typing
 00091af0: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-00091b00: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-00091b10: 6574 5b73 7472 5d5d 2c0a 2020 2020 2020  et[str]],.      
+00091b00: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+00091b10: 6574 5b69 6e74 5d5d 2c0a 2020 2020 2020  et[int]],.      
 00091b20: 2020 2020 2020 2020 206d 6573 7361 6765           message
 00091b30: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b73  : typing.Union[s
 00091b40: 7472 2c20 7479 7069 6e67 2e41 6e79 5d29  tr, typing.Any])
 00091b50: 3a0a 2020 2020 2020 2020 2727 2720 7265  :.        ''' re
 00091b60: 706f 7274 0a0a 2020 2020 2020 2020 3a70  port..        :p
 00091b70: 6172 616d 2074 7970 653a 2054 7970 650a  aram type: Type.
 00091b80: 2020 2020 2020 2020 3a74 7970 6520 7479          :type ty
 00091b90: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-00091ba0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-00091bb0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+00091ba0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+00091bb0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 00091bc0: 5d5d 0a20 2020 2020 2020 203a 7061 7261  ]].        :para
 00091bd0: 6d20 6d65 7373 6167 653a 2052 6570 6f72  m message: Repor
 00091be0: 7420 4d65 7373 6167 650a 2020 2020 2020  t Message.      
 00091bf0: 2020 3a74 7970 6520 6d65 7373 6167 653a    :type message:
 00091c00: 2074 7970 696e 672e 556e 696f 6e5b 7374   typing.Union[st
 00091c10: 722c 2074 7970 696e 672e 416e 795d 0a20  r, typing.Any]. 
 00091c20: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
@@ -37335,26 +37335,26 @@
 00091d60: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 00091d70: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
 00091d80: 6566 2065 7865 6375 7465 2873 656c 662c  ef execute(self,
 00091d90: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 00091da0: 7874 270a 2020 2020 2020 2020 2020 2020  xt'.            
 00091db0: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
 00091dc0: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-00091dd0: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-00091de0: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
+00091dd0: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+00091de0: 745b 696e 745d 5d3a 0a20 2020 2020 2020  t[int]]:.       
 00091df0: 2027 2727 2045 7865 6375 7465 2074 6865   ''' Execute the
 00091e00: 206f 7065 7261 746f 720a 0a20 2020 2020   operator..     
 00091e10: 2020 203a 7061 7261 6d20 636f 6e74 6578     :param contex
 00091e20: 743a 200a 2020 2020 2020 2020 3a74 7970  t: .        :typ
 00091e30: 6520 636f 6e74 6578 743a 2027 436f 6e74  e context: 'Cont
 00091e40: 6578 7427 0a20 2020 2020 2020 203a 7274  ext'.        :rt
 00091e50: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
-00091e60: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
-00091e70: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
-00091e80: 725d 5d0a 2020 2020 2020 2020 3a72 6574  r]].        :ret
+00091e60: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
+00091e70: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
+00091e80: 745d 5d0a 2020 2020 2020 2020 3a72 6574  t]].        :ret
 00091e90: 7572 6e3a 2072 6573 756c 740a 2020 2020  urn: result.    
 00091ea0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
 00091eb0: 7061 7373 0a0a 2020 2020 6465 6620 6368  pass..    def ch
 00091ec0: 6563 6b28 7365 6c66 2c20 636f 6e74 6578  eck(self, contex
 00091ed0: 743a 2027 436f 6e74 6578 7427 2920 2d3e  t: 'Context') ->
 00091ee0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
 00091ef0: 2727 2043 6865 636b 2074 6865 206f 7065  '' Check the ope
@@ -37371,53 +37371,53 @@
 00091fa0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 00091fb0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
 00091fc0: 6566 2069 6e76 6f6b 6528 7365 6c66 2c20  ef invoke(self, 
 00091fd0: 636f 6e74 6578 743a 2027 436f 6e74 6578  context: 'Contex
 00091fe0: 7427 2c20 6576 656e 743a 2027 4576 656e  t', event: 'Even
 00091ff0: 7427 0a20 2020 2020 2020 2020 2020 2020  t'.             
 00092000: 2020 2920 2d3e 2074 7970 696e 672e 556e    ) -> typing.Un
-00092010: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-00092020: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-00092030: 7374 725d 5d3a 0a20 2020 2020 2020 2027  str]]:.        '
+00092010: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+00092020: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+00092030: 696e 745d 5d3a 0a20 2020 2020 2020 2027  int]]:.        '
 00092040: 2727 2049 6e76 6f6b 6520 7468 6520 6f70  '' Invoke the op
 00092050: 6572 6174 6f72 0a0a 2020 2020 2020 2020  erator..        
 00092060: 3a70 6172 616d 2063 6f6e 7465 7874 3a20  :param context: 
 00092070: 0a20 2020 2020 2020 203a 7479 7065 2063  .        :type c
 00092080: 6f6e 7465 7874 3a20 2743 6f6e 7465 7874  ontext: 'Context
 00092090: 270a 2020 2020 2020 2020 3a70 6172 616d  '.        :param
 000920a0: 2065 7665 6e74 3a20 0a20 2020 2020 2020   event: .       
 000920b0: 203a 7479 7065 2065 7665 6e74 3a20 2745   :type event: 'E
 000920c0: 7665 6e74 270a 2020 2020 2020 2020 3a72  vent'.        :r
 000920d0: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
-000920e0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-000920f0: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-00092100: 7472 5d5d 0a20 2020 2020 2020 203a 7265  tr]].        :re
+000920e0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+000920f0: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+00092100: 6e74 5d5d 0a20 2020 2020 2020 203a 7265  nt]].        :re
 00092110: 7475 726e 3a20 7265 7375 6c74 0a20 2020  turn: result.   
 00092120: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
 00092130: 2070 6173 730a 0a20 2020 2064 6566 206d   pass..    def m
 00092140: 6f64 616c 2873 656c 662c 2063 6f6e 7465  odal(self, conte
 00092150: 7874 3a20 2743 6f6e 7465 7874 272c 2065  xt: 'Context', e
 00092160: 7665 6e74 3a20 2745 7665 6e74 270a 2020  vent: 'Event'.  
 00092170: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
 00092180: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-00092190: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-000921a0: 7970 696e 672e 5365 745b 7374 725d 5d3a  yping.Set[str]]:
+00092190: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+000921a0: 7970 696e 672e 5365 745b 696e 745d 5d3a  yping.Set[int]]:
 000921b0: 0a20 2020 2020 2020 2027 2727 204d 6f64  .        ''' Mod
 000921c0: 616c 206f 7065 7261 746f 7220 6675 6e63  al operator func
 000921d0: 7469 6f6e 0a0a 2020 2020 2020 2020 3a70  tion..        :p
 000921e0: 6172 616d 2063 6f6e 7465 7874 3a20 0a20  aram context: . 
 000921f0: 2020 2020 2020 203a 7479 7065 2063 6f6e         :type con
 00092200: 7465 7874 3a20 2743 6f6e 7465 7874 270a  text: 'Context'.
 00092210: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 00092220: 7665 6e74 3a20 0a20 2020 2020 2020 203a  vent: .        :
 00092230: 7479 7065 2065 7665 6e74 3a20 2745 7665  type event: 'Eve
 00092240: 6e74 270a 2020 2020 2020 2020 3a72 7479  nt'.        :rty
 00092250: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-00092260: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-00092270: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+00092260: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+00092270: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 00092280: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 00092290: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 000922a0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 000922b0: 6173 730a 0a20 2020 2064 6566 2064 7261  ass..    def dra
 000922c0: 7728 7365 6c66 2c20 636f 6e74 6578 743a  w(self, context:
 000922d0: 2027 436f 6e74 6578 7427 293a 0a20 2020   'Context'):.   
 000922e0: 2020 2020 2027 2727 2044 7261 7720 6675       ''' Draw fu
@@ -47060,29 +47060,29 @@
 000b7d30: 7065 206d 656d 6f72 795f 7065 616b 3a20  pe memory_peak: 
 000b7d40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
 000b7d50: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 000b7d60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
 000b7d70: 7061 7373 0a0a 2020 2020 6465 6620 7265  pass..    def re
 000b7d80: 706f 7274 2873 656c 662c 2074 7970 653a  port(self, type:
 000b7d90: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-000b7da0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-000b7db0: 7970 696e 672e 5365 745b 7374 725d 5d2c  yping.Set[str]],
+000b7da0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+000b7db0: 7970 696e 672e 5365 745b 696e 745d 5d2c  yping.Set[int]],
 000b7dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000b7dd0: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 000b7de0: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 000b7df0: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
 000b7e00: 2027 2727 2052 6570 6f72 7420 696e 666f   ''' Report info
 000b7e10: 2c20 7761 726e 696e 6720 6f72 2065 7272  , warning or err
 000b7e20: 6f72 206d 6573 7361 6765 730a 0a20 2020  or messages..   
 000b7e30: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
 000b7e40: 3a20 5479 7065 0a20 2020 2020 2020 203a  : Type.        :
 000b7e50: 7479 7065 2074 7970 653a 2074 7970 696e  type type: typin
 000b7e60: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-000b7e70: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-000b7e80: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
+000b7e70: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+000b7e80: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
 000b7e90: 2020 3a70 6172 616d 206d 6573 7361 6765    :param message
 000b7ea0: 3a20 5265 706f 7274 204d 6573 7361 6765  : Report Message
 000b7eb0: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
 000b7ec0: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 000b7ed0: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 000b7ee0: 2e41 6e79 5d0a 2020 2020 2020 2020 2727  .Any].        ''
 000b7ef0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
@@ -66579,22 +66579,22 @@
 00104120: 2077 6974 6820 7468 6520 6375 7272 656e   with the curren
 00104130: 746c 7920 6469 7370 6c61 7965 6420 696d  tly displayed im
 00104140: 6167 6520 6173 7369 676e 6564 0a0a 2020  age assigned..  
 00104150: 2020 3a74 7970 653a 2062 6f6f 6c0a 2020    :type: bool.  
 00104160: 2020 2727 270a 0a20 2020 2073 6e61 705f    '''..    snap_
 00104170: 656c 656d 656e 7473 3a20 7479 7069 6e67  elements: typing
 00104180: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-00104190: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-001041a0: 6574 5b73 7472 5d5d 203d 204e 6f6e 650a  et[str]] = None.
+00104190: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+001041a0: 6574 5b69 6e74 5d5d 203d 204e 6f6e 650a  et[int]] = None.
 001041b0: 2020 2020 2727 2720 5479 7065 206f 6620      ''' Type of 
 001041c0: 656c 656d 656e 7420 746f 2073 6e61 7020  element to snap 
 001041d0: 746f 0a0a 2020 2020 3a74 7970 653a 2074  to..    :type: t
 001041e0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-001041f0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-00104200: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
+001041f0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+00104200: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 00104210: 2020 2727 270a 0a20 2020 2073 6e61 705f    '''..    snap_
 00104220: 6661 6365 5f6e 6561 7265 7374 5f73 7465  face_nearest_ste
 00104230: 7073 3a20 696e 7420 3d20 4e6f 6e65 0a20  ps: int = None. 
 00104240: 2020 2027 2727 204e 756d 6265 7220 6f66     ''' Number of
 00104250: 2073 7465 7073 2074 6f20 6272 6561 6b20   steps to break 
 00104260: 7472 616e 7366 6f72 6d61 7469 6f6e 2069  transformation i
 00104270: 6e74 6f20 666f 7220 6661 6365 206e 6561  nto for face nea
@@ -108209,17 +108209,17 @@
 001a6b00: 6572 6174 6f72 275d 2c0a 2020 2020 2020  erator'],.      
 001a6b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a6b20: 2020 2020 2065 7665 6e74 3a20 7479 7069       event: typi
 001a6b30: 6e67 2e4f 7074 696f 6e61 6c5b 2745 7665  ng.Optional['Eve
 001a6b40: 6e74 275d 0a20 2020 2020 2020 2020 2020  nt'].           
 001a6b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a6b60: 2920 2d3e 2074 7970 696e 672e 556e 696f  ) -> typing.Unio
-001a6b70: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
-001a6b80: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
-001a6b90: 725d 5d3a 0a20 2020 2020 2020 2027 2727  r]]:.        '''
+001a6b70: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
+001a6b80: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
+001a6b90: 745d 5d3a 0a20 2020 2020 2020 2027 2727  t]]:.        '''
 001a6ba0: 204f 7065 7261 746f 7220 706f 7075 7020   Operator popup 
 001a6bb0: 696e 766f 6b65 2028 7368 6f77 206f 7065  invoke (show ope
 001a6bc0: 7261 746f 7220 7072 6f70 6572 7469 6573  rator properties
 001a6bd0: 2061 6e64 2065 7865 6375 7465 2069 7420   and execute it 
 001a6be0: 6175 746f 6d61 7469 6361 6c6c 7920 6f6e  automatically on
 001a6bf0: 2063 6861 6e67 6573 290a 0a20 2020 2020   changes)..     
 001a6c00: 2020 203a 7061 7261 6d20 6f70 6572 6174     :param operat
@@ -108230,16 +108230,16 @@
 001a6c50: 6572 6174 6f72 275d 0a20 2020 2020 2020  erator'].       
 001a6c60: 203a 7061 7261 6d20 6576 656e 743a 2045   :param event: E
 001a6c70: 7665 6e74 0a20 2020 2020 2020 203a 7479  vent.        :ty
 001a6c80: 7065 2065 7665 6e74 3a20 7479 7069 6e67  pe event: typing
 001a6c90: 2e4f 7074 696f 6e61 6c5b 2745 7665 6e74  .Optional['Event
 001a6ca0: 275d 0a20 2020 2020 2020 203a 7274 7970  '].        :rtyp
 001a6cb0: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-001a6cc0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-001a6cd0: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+001a6cc0: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+001a6cd0: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 001a6ce0: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
 001a6cf0: 6e3a 2072 6573 756c 740a 2020 2020 2020  n: result.      
 001a6d00: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 001a6d10: 7373 0a0a 2020 2020 4063 6c61 7373 6d65  ss..    @classme
 001a6d20: 7468 6f64 0a20 2020 2064 6566 2069 6e76  thod.    def inv
 001a6d30: 6f6b 655f 7072 6f70 735f 6469 616c 6f67  oke_props_dialog
 001a6d40: 280a 2020 2020 2020 2020 2020 2020 636c  (.            cl
@@ -108247,16 +108247,16 @@
 001a6d60: 7065 7261 746f 723a 2074 7970 696e 672e  perator: typing.
 001a6d70: 4f70 7469 6f6e 616c 5b27 4f70 6572 6174  Optional['Operat
 001a6d80: 6f72 275d 2c0a 2020 2020 2020 2020 2020  or'],.          
 001a6d90: 2020 7769 6474 683a 2074 7970 696e 672e    width: typing.
 001a6da0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
 001a6db0: 416e 795d 203d 2033 3030 0a20 2020 2029  Any] = 300.    )
 001a6dc0: 202d 3e20 7479 7069 6e67 2e55 6e69 6f6e   -> typing.Union
-001a6dd0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-001a6de0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+001a6dd0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+001a6de0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 001a6df0: 5d5d 3a0a 2020 2020 2020 2020 2727 2720  ]]:.        ''' 
 001a6e00: 4f70 6572 6174 6f72 2064 6961 6c6f 6720  Operator dialog 
 001a6e10: 286e 6f6e 2d61 7574 6f65 7865 6320 706f  (non-autoexec po
 001a6e20: 7075 7029 2069 6e76 6f6b 6520 2873 686f  pup) invoke (sho
 001a6e30: 7720 6f70 6572 6174 6f72 2070 726f 7065  w operator prope
 001a6e40: 7274 6965 7320 616e 6420 6f6e 6c79 2065  rties and only e
 001a6e50: 7865 6375 7465 2069 7420 6f6e 2063 6c69  xecute it on cli
@@ -108271,16 +108271,16 @@
 001a6ee0: 6964 7468 3a20 5769 6474 6820 6f66 2074  idth: Width of t
 001a6ef0: 6865 2070 6f70 7570 0a20 2020 2020 2020  he popup.       
 001a6f00: 203a 7479 7065 2077 6964 7468 3a20 7479   :type width: ty
 001a6f10: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
 001a6f20: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
 001a6f30: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a6f40: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a6f50: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-001a6f60: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
+001a6f50: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+001a6f60: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
 001a6f70: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a6f80: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a6f90: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a6fa0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a6fb0: 6465 6620 696e 766f 6b65 5f73 6561 7263  def invoke_searc
 001a6fc0: 685f 706f 7075 7028 636c 732c 206f 7065  h_popup(cls, ope
 001a6fd0: 7261 746f 723a 2074 7970 696e 672e 4f70  rator: typing.Op
@@ -108313,16 +108313,16 @@
 001a7180: 7227 5d2c 0a20 2020 2020 2020 2020 2020  r'],.           
 001a7190: 2020 2020 2020 2020 2020 7769 6474 683a            width:
 001a71a0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a71b0: 5b74 7970 696e 672e 416e 795d 203d 2033  [typing.Any] = 3
 001a71c0: 3030 0a20 2020 2020 2020 2020 2020 2020  00.             
 001a71d0: 2020 2020 2020 2020 2920 2d3e 2074 7970          ) -> typ
 001a71e0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-001a71f0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
-001a7200: 672e 5365 745b 7374 725d 5d3a 0a20 2020  g.Set[str]]:.   
+001a71f0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
+001a7200: 672e 5365 745b 696e 745d 5d3a 0a20 2020  g.Set[int]]:.   
 001a7210: 2020 2020 2027 2727 204f 7065 7261 746f       ''' Operato
 001a7220: 7220 706f 7075 7020 696e 766f 6b65 2028  r popup invoke (
 001a7230: 6f6e 6c79 2073 686f 7773 206f 7065 7261  only shows opera
 001a7240: 746f 7227 7320 7072 6f70 6572 7469 6573  tor's properties
 001a7250: 2c20 7769 7468 6f75 7420 6578 6563 7574  , without execut
 001a7260: 696e 6720 6974 290a 0a20 2020 2020 2020  ing it)..       
 001a7270: 203a 7061 7261 6d20 6f70 6572 6174 6f72   :param operator
@@ -108334,16 +108334,16 @@
 001a72d0: 7061 7261 6d20 7769 6474 683a 2057 6964  param width: Wid
 001a72e0: 7468 206f 6620 7468 6520 706f 7075 700a  th of the popup.
 001a72f0: 2020 2020 2020 2020 3a74 7970 6520 7769          :type wi
 001a7300: 6474 683a 2074 7970 696e 672e 4f70 7469  dth: typing.Opti
 001a7310: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
 001a7320: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
 001a7330: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001a7340: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001a7350: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001a7340: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001a7350: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001a7360: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
 001a7370: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
 001a7380: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
 001a7390: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
 001a73a0: 6f64 0a20 2020 2064 6566 2069 6e76 6f6b  od.    def invok
 001a73b0: 655f 636f 6e66 6972 6d28 636c 732c 206f  e_confirm(cls, o
 001a73c0: 7065 7261 746f 723a 2074 7970 696e 672e  perator: typing.
@@ -108351,16 +108351,16 @@
 001a73e0: 6f72 275d 2c0a 2020 2020 2020 2020 2020  or'],.          
 001a73f0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
 001a7400: 6e74 3a20 7479 7069 6e67 2e4f 7074 696f  nt: typing.Optio
 001a7410: 6e61 6c5b 2745 7665 6e74 275d 0a20 2020  nal['Event'].   
 001a7420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a7430: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
 001a7440: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-001a7450: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-001a7460: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
+001a7450: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+001a7460: 745b 696e 745d 5d3a 0a20 2020 2020 2020  t[int]]:.       
 001a7470: 2027 2727 204f 7065 7261 746f 7220 636f   ''' Operator co
 001a7480: 6e66 6972 6d61 7469 6f6e 2070 6f70 7570  nfirmation popup
 001a7490: 2028 6f6e 6c79 2074 6f20 6c65 7420 7573   (only to let us
 001a74a0: 6572 2063 6f6e 6669 726d 2074 6865 2065  er confirm the e
 001a74b0: 7865 6375 7469 6f6e 2c20 6e6f 206f 7065  xecution, no ope
 001a74c0: 7261 746f 7220 7072 6f70 6572 7469 6573  rator properties
 001a74d0: 2073 686f 776e 290a 0a20 2020 2020 2020   shown)..       
@@ -108372,16 +108372,16 @@
 001a7530: 6174 6f72 275d 0a20 2020 2020 2020 203a  ator'].        :
 001a7540: 7061 7261 6d20 6576 656e 743a 2045 7665  param event: Eve
 001a7550: 6e74 0a20 2020 2020 2020 203a 7479 7065  nt.        :type
 001a7560: 2065 7665 6e74 3a20 7479 7069 6e67 2e4f   event: typing.O
 001a7570: 7074 696f 6e61 6c5b 2745 7665 6e74 275d  ptional['Event']
 001a7580: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
 001a7590: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001a75a0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001a75b0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001a75a0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001a75b0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001a75c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
 001a75d0: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
 001a75e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
 001a75f0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
 001a7600: 6f64 0a20 2020 2064 6566 2070 6f70 6d65  od.    def popme
 001a7610: 6e75 5f62 6567 696e 5f5f 696e 7465 726e  nu_begin__intern
 001a7620: 616c 2863 6c73 2c0a 2020 2020 2020 2020  al(cls,.        
@@ -114337,22 +114337,22 @@
 001bea00: 6973 736f 6c76 6520 6765 6f6d 6574 7279  issolve geometry
 001bea10: 2074 6f20 666f 726d 2070 6c61 6e61 7220   to form planar 
 001bea20: 706f 6c79 676f 6e73 2e0a 0a20 2020 203a  polygons...    :
 001bea30: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
 001bea40: 6f6e 5b73 7472 2c20 696e 745d 0a20 2020  on[str, int].   
 001bea50: 2027 2727 0a0a 2020 2020 6465 6c69 6d69   '''..    delimi
 001bea60: 743a 2074 7970 696e 672e 556e 696f 6e5b  t: typing.Union[
-001bea70: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-001bea80: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+001bea70: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+001bea80: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 001bea90: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 001beaa0: 204c 696d 6974 206d 6572 6769 6e67 2067   Limit merging g
 001beab0: 656f 6d65 7472 790a 0a20 2020 203a 7479  eometry..    :ty
 001beac0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-001bead0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-001beae0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+001bead0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+001beae0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 001beaf0: 5d5d 0a20 2020 2027 2727 0a0a 2020 2020  ]].    '''..    
 001beb00: 6661 6365 5f63 6f75 6e74 3a20 696e 7420  face_count: int 
 001beb10: 3d20 4e6f 6e65 0a20 2020 2027 2727 2054  = None.    ''' T
 001beb20: 6865 2063 7572 7265 6e74 206e 756d 6265  he current numbe
 001beb30: 7220 6f66 2066 6163 6573 2069 6e20 7468  r of faces in th
 001beb40: 6520 6465 6369 6d61 7465 6420 6d65 7368  e decimated mesh
 001beb50: 0a0a 2020 2020 3a74 7970 653a 2069 6e74  ..    :type: int
@@ -115621,21 +115621,21 @@
 001c3a40: 746f 2065 7874 6572 6e61 6c20 6469 7370  to external disp
 001c3a50: 6c61 6365 6d65 6e74 7320 6669 6c65 0a0a  lacements file..
 001c3a60: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001c3a70: 672e 556e 696f 6e5b 7374 722c 2074 7970  g.Union[str, typ
 001c3a80: 696e 672e 416e 795d 0a20 2020 2027 2727  ing.Any].    '''
 001c3a90: 0a0a 2020 2020 666c 6970 5f61 7869 733a  ..    flip_axis:
 001c3aa0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001c3ab0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001c3ac0: 7970 696e 672e 5365 745b 7374 725d 5d20  yping.Set[str]] 
+001c3ab0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001c3ac0: 7970 696e 672e 5365 745b 696e 745d 5d20  yping.Set[int]] 
 001c3ad0: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 001c3ae0: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 001c3af0: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-001c3b00: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-001c3b10: 2e53 6574 5b73 7472 5d5d 0a20 2020 2027  .Set[str]].    '
+001c3b00: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+001c3b10: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2027  .Set[int]].    '
 001c3b20: 2727 0a0a 2020 2020 666f 7277 6172 645f  ''..    forward_
 001c3b30: 6178 6973 3a20 7479 7069 6e67 2e55 6e69  axis: typing.Uni
 001c3b40: 6f6e 5b73 7472 2c20 696e 745d 203d 204e  on[str, int] = N
 001c3b50: 6f6e 650a 2020 2020 2727 2720 0a0a 2020  one.    ''' ..  
 001c3b60: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 001c3b70: 556e 696f 6e5b 7374 722c 2069 6e74 5d0a  Union[str, int].
 001c3b80: 2020 2020 2727 270a 0a20 2020 2066 7261      '''..    fra
```

### Comparing `fake-bpy-module-latest-20230416/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230417/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import units
 from . import previews
+from . import units
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230416/bpy/utils/previews.py` & `fake-bpy-module-latest-20230417/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy/utils/units.py` & `fake-bpy-module-latest-20230417/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence'],
+        Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence']
+    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230417/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230417/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/bpy_types.py` & `fake-bpy-module-latest-20230417/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230416
+Version: 20230417
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230416/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230417/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230417/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/functions.py` & `fake-bpy-module-latest-20230417/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/predicates.py` & `fake-bpy-module-latest-20230417/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/shaders.py` & `fake-bpy-module-latest-20230417/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/types.py` & `fake-bpy-module-latest-20230417/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230417/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230417/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/capabilities.py` & `fake-bpy-module-latest-20230417/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/matrix.py` & `fake-bpy-module-latest-20230417/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/platform.py` & `fake-bpy-module-latest-20230417/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/shader.py` & `fake-bpy-module-latest-20230417/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/state.py` & `fake-bpy-module-latest-20230417/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/texture.py` & `fake-bpy-module-latest-20230417/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu/types.py` & `fake-bpy-module-latest-20230417/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu_extras/batch.py` & `fake-bpy-module-latest-20230417/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/gpu_extras/presets.py` & `fake-bpy-module-latest-20230417/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/idprop/types.py` & `fake-bpy-module-latest-20230417/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/imbuf/__init__.py` & `fake-bpy-module-latest-20230417/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/imbuf/types.py` & `fake-bpy-module-latest-20230417/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/keyingsets_builtins.py` & `fake-bpy-module-latest-20230417/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/keyingsets_utils.py` & `fake-bpy-module-latest-20230417/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/mathutils/__init__.py` & `fake-bpy-module-latest-20230417/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230417/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/mathutils/geometry.py` & `fake-bpy-module-latest-20230417/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/mathutils/kdtree.py` & `fake-bpy-module-latest-20230417/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/mathutils/noise.py` & `fake-bpy-module-latest-20230417/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/nodeitems_builtins.py` & `fake-bpy-module-latest-20230417/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/nodeitems_utils.py` & `fake-bpy-module-latest-20230417/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/rna_info.py` & `fake-bpy-module-latest-20230417/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/rna_keymap_ui.py` & `fake-bpy-module-latest-20230417/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/rna_prop_ui.py` & `fake-bpy-module-latest-20230417/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/rna_xml.py` & `fake-bpy-module-latest-20230417/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230416/setup.py` & `fake-bpy-module-latest-20230417/setup.py`

 * *Files identical despite different names*

