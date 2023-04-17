# Comparing `tmp/jina-now-0.0.9.tar.gz` & `tmp/jina-now-0.0.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jina-now-0.0.9.tar", last modified: Thu Jun  2 10:24:43 2022, max compression
+gzip compressed data, was "jina-now-0.0.9.dev2.tar", last modified: Thu Jun  2 10:19:25 2022, max compression
```

## Comparing `jina-now-0.0.9.tar` & `jina-now-0.0.9.dev2.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-06-02 10:24:27.000000 jina-now-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-02 10:24:27.000000 jina-now-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11230 2022-06-02 10:24:43.000000 jina-now-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-06-02 10:24:27.000000 jina-now-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/bff/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/bff/app/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/bff/app/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/bff/app/v1/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/models/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/models/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/models/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/deployment/bff/app/v1/routers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/routers/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/routers/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-06-02 10:24:27.000000 jina-now-0.0.9/deployment/bff/app/v1/routers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11230 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-02 10:24:43.000000 jina-now-0.0.9/jina_now.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/base/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/base/bff.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/base/flow.yml
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/base/playground.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/image_to_image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/image_to_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/image_to_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/image_to_text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/image_to_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/image_to_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/music_to_music/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/music_to_music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/music_to_music/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/apps/text_to_image/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/text_to_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/apps/text_to_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/cloud_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/custom-spinners.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/data_loading/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23904 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/build_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/convert_datasets_to_jpeg.py
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/embed_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/migrate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/data_loading/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/datasource/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/datasource/datasource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/datasource/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/deployment/flow/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/flow/flow-clip.yml
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/flow/ft-flow-clip.yml
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/flow/ft-flow-music.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5559 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/k8s_backend-svc-lb.yml
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/k8s_backend-svc-node.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/k8s_playground-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/k8s_playground-svc-lb.yml
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/deployment/k8s_playground-svc-node.yml
--rw-r--r--   0 runner    (1001) docker     (121)    10782 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/finetuning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/finetuning/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/finetuning/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7325 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/finetuning/run_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/finetuning/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   367112 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/fonts/arial.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/hub/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/hub/head_encoder/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/hub/head_encoder/.jina/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/.jina/secret.key
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/head_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/manifest.yml
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/head_encoder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/improvements/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/improvements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/improvements/improvements.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/kind.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/log/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/log/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/run_all_k8s.py
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/run_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/run_bff_playground.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      371 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/scripts/install_kind.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      770 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/scripts/install_kubectl.sh
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/system_information.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/color_print.py
--rw-r--r--   0 runner    (1001) docker     (121)     4268 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9273 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6613 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6229 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/expand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/list.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/password.py
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/rawlist.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/separator.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/PyInquirer/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9934 2022-06-02 10:24:27.000000 jina-now-0.0.9/now/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:43.000000 jina-now-0.0.9/now_common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:24:27.000000 jina-now-0.0.9/now_common/datasource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-06-02 10:24:27.000000 jina-now-0.0.9/now_common/options.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-02 10:24:27.000000 jina-now-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-02 10:24:27.000000 jina-now-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-06-02 10:24:43.000000 jina-now-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-06-02 10:24:27.000000 jina-now-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.762603 jina-now-0.0.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11235 2022-06-02 10:19:25.762603 jina-now-0.0.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/bff/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/bff/app/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/bff/app/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/bff/app/v1/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/models/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/models/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.750603 jina-now-0.0.9.dev2/jina_now.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11235 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/jina_now.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-02 10:19:25.000000 jina-now-0.0.9.dev2/now/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/base/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/base/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/base/bff.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/base/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/base/playground.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/image_to_image/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/image_to_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/image_to_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/image_to_text/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/image_to_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/image_to_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/music_to_music/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/music_to_music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/music_to_music/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/apps/text_to_image/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/text_to_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/apps/text_to_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/cloud_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/custom-spinners.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/data_loading/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23904 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/build_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/convert_datasets_to_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6276 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/embed_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/migrate_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/data_loading/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/datasource/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/datasource/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/datasource/example.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.754603 jina-now-0.0.9.dev2/now/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/deployment/flow/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/flow/flow-clip.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/flow/ft-flow-clip.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/flow/ft-flow-music.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5559 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/k8s_backend-svc-lb.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/k8s_backend-svc-node.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/k8s_playground-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/k8s_playground-svc-lb.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/deployment/k8s_playground-svc-node.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    10782 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/finetuning/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/finetuning/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7325 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/finetuning/run_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/finetuning/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)   367112 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/fonts/arial.ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/hub/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/hub/head_encoder/
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/hub/head_encoder/.jina/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/.jina/secret.key
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/head_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/head_encoder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/improvements/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/improvements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/improvements/improvements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/kind.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/log/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5304 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/run_all_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/run_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/run_bff_playground.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      371 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/scripts/install_kind.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      770 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/scripts/install_kubectl.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/system_information.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/color_print.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4268 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.758603 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9273 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6613 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6229 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/expand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6428 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/password.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/rawlist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/separator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9934 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:25.762603 jina-now-0.0.9.dev2/now_common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now_common/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/now_common/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-06-02 10:19:25.762603 jina-now-0.0.9.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-06-02 10:19:18.000000 jina-now-0.0.9.dev2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jina-now-0.0.9/LICENSE` & `jina-now-0.0.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/PKG-INFO` & `jina-now-0.0.9.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jina-now
-Version: 0.0.9
+Version: 0.0.9.dev2
 Summary: Jina NOW - get your neural search case up and running in minutes.
 Home-page: https://github.com/jina-ai/now/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/now/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: jina-now Version: 0.0.9 Summary: Jina NOW - get
-your neural search case up and running in minutes. Home-page: https://
+Metadata-Version: 2.1 Name: jina-now Version: 0.0.9.dev2 Summary: Jina NOW -
+get your neural search case up and running in minutes. Home-page: https://
 github.com/jina-ai/now/ Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/now/tags Project-URL:
 Documentation, https://docs.jina.ai Project-URL: Source, https://github.com/
 jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/issues
 Description:
           [Jina NOW logo: The data structure for unstructured data]
 One command to host them all. Bring your search case into the cloud in minutes.
```

### Comparing `jina-now-0.0.9/README.md` & `jina-now-0.0.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/app.py` & `jina-now-0.0.9.dev2/deployment/bff/app/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/decorators.py` & `jina-now-0.0.9.dev2/deployment/bff/app/decorators.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/settings.py` & `jina-now-0.0.9.dev2/deployment/bff/app/settings.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/models/helper.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/models/helper.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/models/image.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/models/image.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/models/text.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/models/text.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/routers/helper.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/helper.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/routers/image.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/image.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/deployment/bff/app/v1/routers/text.py` & `jina-now-0.0.9.dev2/deployment/bff/app/v1/routers/text.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/jina_now.egg-info/PKG-INFO` & `jina-now-0.0.9.dev2/jina_now.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jina-now
-Version: 0.0.9
+Version: 0.0.9.dev2
 Summary: Jina NOW - get your neural search case up and running in minutes.
 Home-page: https://github.com/jina-ai/now/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/now/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: jina-now Version: 0.0.9 Summary: Jina NOW - get
-your neural search case up and running in minutes. Home-page: https://
+Metadata-Version: 2.1 Name: jina-now Version: 0.0.9.dev2 Summary: Jina NOW -
+get your neural search case up and running in minutes. Home-page: https://
 github.com/jina-ai/now/ Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/now/tags Project-URL:
 Documentation, https://docs.jina.ai Project-URL: Source, https://github.com/
 jina-ai/now Project-URL: Tracker, https://github.com/jina-ai/now/issues
 Description:
           [Jina NOW logo: The data structure for unstructured data]
 One command to host them all. Bring your search case into the cloud in minutes.
```

### Comparing `jina-now-0.0.9/jina_now.egg-info/SOURCES.txt` & `jina-now-0.0.9.dev2/jina_now.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/apps/base/app.py` & `jina-now-0.0.9.dev2/now/apps/base/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/apps/image_to_image/app.py` & `jina-now-0.0.9.dev2/now/apps/image_to_image/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/apps/image_to_text/app.py` & `jina-now-0.0.9.dev2/now/apps/image_to_text/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/apps/music_to_music/app.py` & `jina-now-0.0.9.dev2/now/apps/music_to_music/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/apps/text_to_image/app.py` & `jina-now-0.0.9.dev2/now/apps/text_to_image/app.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/cli/__init__.py` & `jina-now-0.0.9.dev2/now/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/cli/parser.py` & `jina-now-0.0.9.dev2/now/cli/parser.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/cloud_manager.py` & `jina-now-0.0.9.dev2/now/cloud_manager.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/constants.py` & `jina-now-0.0.9.dev2/now/constants.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/build_datasets.py` & `jina-now-0.0.9.dev2/now/data_loading/build_datasets.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/convert_datasets_to_jpeg.py` & `jina-now-0.0.9.dev2/now/data_loading/convert_datasets_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/data_loading.py` & `jina-now-0.0.9.dev2/now/data_loading/data_loading.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/embed_datasets.py` & `jina-now-0.0.9.dev2/now/data_loading/embed_datasets.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/migrate_datasets.py` & `jina-now-0.0.9.dev2/now/data_loading/migrate_datasets.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/data_loading/requirements.txt` & `jina-now-0.0.9.dev2/now/data_loading/requirements.txt`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/dataclasses.py` & `jina-now-0.0.9.dev2/now/dataclasses.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/datasource/example.py` & `jina-now-0.0.9.dev2/now/datasource/example.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/deployment/deployment.py` & `jina-now-0.0.9.dev2/now/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/deployment/flow/ft-flow-clip.yml` & `jina-now-0.0.9.dev2/now/deployment/flow/ft-flow-clip.yml`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/deployment/flow/ft-flow-music.yml` & `jina-now-0.0.9.dev2/now/deployment/flow/ft-flow-music.yml`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/deployment/flow.py` & `jina-now-0.0.9.dev2/now/deployment/flow.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/deployment/k8s_playground-deployment.yml` & `jina-now-0.0.9.dev2/now/deployment/k8s_playground-deployment.yml`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/dialog.py` & `jina-now-0.0.9.dev2/now/dialog.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/finetuning/dataset.py` & `jina-now-0.0.9.dev2/now/finetuning/dataset.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/finetuning/embeddings.py` & `jina-now-0.0.9.dev2/now/finetuning/embeddings.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/finetuning/run_finetuning.py` & `jina-now-0.0.9.dev2/now/finetuning/run_finetuning.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/finetuning/settings.py` & `jina-now-0.0.9.dev2/now/finetuning/settings.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/fonts/arial.ttf` & `jina-now-0.0.9.dev2/now/fonts/arial.ttf`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/hub/head_encoder/head_encoder.py` & `jina-now-0.0.9.dev2/now/hub/head_encoder/head_encoder.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/hub/hub.py` & `jina-now-0.0.9.dev2/now/hub/hub.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/improvements/improvements.py` & `jina-now-0.0.9.dev2/now/improvements/improvements.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/kind.yml` & `jina-now-0.0.9.dev2/now/kind.yml`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/log/log.py` & `jina-now-0.0.9.dev2/now/log/log.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/run_all_k8s.py` & `jina-now-0.0.9.dev2/now/run_all_k8s.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/run_backend.py` & `jina-now-0.0.9.dev2/now/run_backend.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/run_bff_playground.py` & `jina-now-0.0.9.dev2/now/run_bff_playground.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/scripts/install_kubectl.sh` & `jina-now-0.0.9.dev2/now/scripts/install_kubectl.sh`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/system_information.py` & `jina-now-0.0.9.dev2/now/system_information.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/__init__.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/color_print.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/color_print.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompt.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompt.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/checkbox.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/common.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/common.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/confirm.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/editor.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/editor.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/expand.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/expand.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/input.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/input.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/list.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/list.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/prompts/rawlist.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/prompts/rawlist.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/thirdparty/PyInquirer/utils.py` & `jina-now-0.0.9.dev2/now/thirdparty/PyInquirer/utils.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now/utils.py` & `jina-now-0.0.9.dev2/now/utils.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/now_common/options.py` & `jina-now-0.0.9.dev2/now_common/options.py`

 * *Files identical despite different names*

### Comparing `jina-now-0.0.9/setup.py` & `jina-now-0.0.9.dev2/setup.py`

 * *Files identical despite different names*

