# Comparing `tmp/alfred-py-3.0.6.tar.gz` & `tmp/alfred-py-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-py-3.0.6.tar", last modified: Wed Apr 12 11:13:40 2023, max compression
+gzip compressed data, was "alfred-py-3.0.7.tar", last modified: Mon Apr 17 14:03:03 2023, max compression
```

## Comparing `alfred-py-3.0.6.tar` & `alfred-py-3.0.7.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.074607 alfred-py-3.0.6/
--rw-rw-rw-   0        0        0    35786 2023-02-10 05:13:33.000000 alfred-py-3.0.6/LICENSE
--rw-rw-rw-   0        0        0      151 2023-02-10 05:13:33.000000 alfred-py-3.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    25052 2023-04-12 11:13:40.075152 alfred-py-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    24015 2023-02-10 05:13:33.000000 alfred-py-3.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.842231 alfred-py-3.0.6/alfred/
--rw-rw-rw-   0        0        0     1303 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/__init__.py
--rw-rw-rw-   0        0        0    26424 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/alfred.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.817298 alfred-py-3.0.6/alfred/deploy/
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.849214 alfred-py-3.0.6/alfred/deploy/tensorrt/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/__init__.py
--rw-rw-rw-   0        0        0     2234 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/calibrator.py
--rw-rw-rw-   0        0        0    20962 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/common.py
--rw-rw-rw-   0        0        0     3337 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/process.py
--rw-rw-rw-   0        0        0     4021 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/deploy/tensorrt/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.850211 alfred-py-3.0.6/alfred/dl/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.819292 alfred-py-3.0.6/alfred/dl/data/
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.853202 alfred-py-3.0.6/alfred/dl/data/common/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/common/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/common/coco_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.859186 alfred-py-3.0.6/alfred/dl/data/meta/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/concatenated_dataset.py
--rw-rw-rw-   0        0        0     3032 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/dataset_mixin.py
--rw-rw-rw-   0        0        0     3261 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/getter_dataset.py
--rw-rw-rw-   0        0        0     5205 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/data/meta/sliceable_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.861181 alfred-py-3.0.6/alfred/dl/evaluator/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/evaluator/__init__.py
--rw-rw-rw-   0        0        0    11447 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/evaluator/yolo_evaluator.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.864173 alfred-py-3.0.6/alfred/dl/inference/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/inference/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/inference/image_inference.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.868162 alfred-py-3.0.6/alfred/dl/metrics/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/__init__.py
--rw-rw-rw-   0        0        0    11818 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/iou_loss.py
--rw-rw-rw-   0        0        0     7993 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/metrics/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.869161 alfred-py-3.0.6/alfred/dl/tf/
--rw-rw-rw-   0        0        0     1133 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/tf/common.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.879134 alfred-py-3.0.6/alfred/dl/torch/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/__init__.py
--rw-rw-rw-   0        0        0     3054 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/common.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.880131 alfred-py-3.0.6/alfred/dl/torch/distribute/
--rw-rw-rw-   0        0        0     8464 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/distribute/utils.py
--rw-rw-rw-   0        0        0     3374 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/env.py
--rw-rw-rw-   0        0        0     1101 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/gpu.py
--rw-rw-rw-   0        0        0    11624 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/metrics.py
--rw-rw-rw-   0        0        0     6369 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/model_summary.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.885118 alfred-py-3.0.6/alfred/dl/torch/nn/
--rw-rw-rw-   0        0        0     1038 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/__init__.py
--rw-rw-rw-   0        0        0     1205 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/functional.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.889107 alfred-py-3.0.6/alfred/dl/torch/nn/modules/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     3882 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/common.py
--rw-rw-rw-   0        0        0     1195 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/modules/normalization.py
--rw-rw-rw-   0        0        0     2049 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/nn/weights_init.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.891101 alfred-py-3.0.6/alfred/dl/torch/ops/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/ops/__init__.py
--rw-rw-rw-   0        0        0     2003 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/ops/array_ops.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.893095 alfred-py-3.0.6/alfred/dl/torch/runner/
--rw-rw-rw-   0        0        0    10080 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/runner/checkpoint.py
--rw-rw-rw-   0        0        0     3245 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.903070 alfred-py-3.0.6/alfred/dl/torch/train/
--rw-rw-rw-   0        0        0     1216 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/__init__.py
--rw-rw-rw-   0        0        0     7564 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/checkpoint.py
--rw-rw-rw-   0        0        0     1651 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/common.py
--rw-rw-rw-   0        0        0    12713 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/fastai_optim.py
--rw-rw-rw-   0        0        0     7598 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules.py
--rw-rw-rw-   0        0        0     6500 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules_fastai.py
--rw-rw-rw-   0        0        0     5101 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/dl/torch/train/optim.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.904067 alfred-py-3.0.6/alfred/fonts/
--rw-rw-rw-   0        0        0  2763148 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fonts/FZSSJW.TTF
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.914040 alfred-py-3.0.6/alfred/fusion/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/common.py
--rw-rw-rw-   0        0        0     2097 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/geometry.py
--rw-rw-rw-   0        0        0     9435 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/kitti_fusion.py
--rw-rw-rw-   0        0        0     4013 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/fusion/nuscenes_fusion.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.914981 alfred-py-3.0.6/alfred/modules/
--rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.927984 alfred-py-3.0.6/alfred/modules/cabinet/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/__init__.py
--rw-rw-rw-   0        0        0     1075 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/changesource.py
--rw-rw-rw-   0        0        0     1660 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/count_file.py
--rw-rw-rw-   0        0        0    19617 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/gtrend.py
--rw-rw-rw-   0        0        0    24437 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/license.py
--rw-rw-rw-   0        0        0     5791 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/markdown_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.932971 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.937958 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/__init__.py
--rw-rw-rw-   0        0        0      346 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/html.py
--rw-rw-rw-   0        0        0      945 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/pdf.py
--rw-rw-rw-   0        0        0      214 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/simple.py
--rw-rw-rw-   0        0        0     4992 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/image_downloader.py
--rw-rw-rw-   0        0        0      437 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/string_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.939952 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.941946 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/__init__.py
--rw-rw-rw-   0        0        0     2209 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.945936 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/transformer.py
--rw-rw-rw-   0        0        0     1842 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/mdparse/www_tools.py
--rw-rw-rw-   0        0        0     2657 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/split_txt.py
--rw-rw-rw-   0        0        0     1780 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/stack_imgs.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.957904 alfred-py-3.0.6/alfred/modules/cabinet/templates/
--rw-rw-rw-   0        0        0      742 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/agpl-v3.tmpl
--rw-rw-rw-   0        0        0      868 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/apache-2.tmpl
--rw-rw-rw-   0        0        0      170 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/bsd-3.tmpl
--rw-rw-rw-   0        0        0     1448 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-B.tmpl
--rw-rw-rw-   0        0        0     1448 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-C.tmpl
--rw-rw-rw-   0        0        0     1442 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill.tmpl
--rw-rw-rw-   0        0        0      721 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/gpl-v3.tmpl
--rw-rw-rw-   0        0        0      744 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl
--rw-rw-rw-   0        0        0      742 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v3.tmpl
--rw-rw-rw-   0        0        0     2140 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/cabinet/webcam.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.987824 alfred-py-3.0.6/alfred/modules/data/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/coco2voc.py
--rw-rw-rw-   0        0        0     2928 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/coco2yolo.py
--rw-rw-rw-   0        0        0     3618 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_csv2voc.py
--rw-rw-rw-   0        0        0     7363 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_cvat2voc.py
--rw-rw-rw-   0        0        0     4280 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/convert_labelone2voc.py
--rw-rw-rw-   0        0        0      156 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/eval_coco.py
--rw-rw-rw-   0        0        0    38129 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/eval_voc.py
--rw-rw-rw-   0        0        0     5868 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/extract_voc.py
--rw-rw-rw-   0        0        0     2546 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/gather_voclabels.py
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/labelone_view.py
--rw-rw-rw-   0        0        0     4422 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/mergevoc.py
--rw-rw-rw-   0        0        0     2366 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/split_coco.py
--rw-rw-rw-   0        0        0     1629 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/split_voc.py
--rw-rw-rw-   0        0        0     3580 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/txt2voc.py
--rw-rw-rw-   0        0        0    10384 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/view_coco.py
--rw-rw-rw-   0        0        0     3218 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/view_txt.py
--rw-rw-rw-   0        0        0     4921 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/view_voc.py
--rw-rw-rw-   0        0        0     2894 2023-04-04 07:40:56.000000 alfred-py-3.0.6/alfred/modules/data/view_yolo.py
--rw-rw-rw-   0        0        0     8501 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/voc2coco.py
--rw-rw-rw-   0        0        0     1986 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/voc2yolo.py
--rw-rw-rw-   0        0        0     4373 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/data/yolo2voc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.990834 alfred-py-3.0.6/alfred/modules/dltool/
--rw-rw-rw-   0        0        0        0 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/dltool/__init__.py
--rw-rw-rw-   0        0        0     5475 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/dltool/cal_anchors.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.994805 alfred-py-3.0.6/alfred/modules/scrap/
--rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/__init__.py
--rw-rw-rw-   0        0        0     4430 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/image_scraper.py
--rw-rw-rw-   0        0        0     5017 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/scrap/scraper_images.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:39.995803 alfred-py-3.0.6/alfred/modules/text/
--rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.003781 alfred-py-3.0.6/alfred/modules/vision/
--rw-rw-rw-   0        0        0      937 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/__init__.py
--rw-rw-rw-   0        0        0     4315 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/face_extractor.py
--rw-rw-rw-   0        0        0     3104 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/to_video.py
--rw-rw-rw-   0        0        0     2849 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/video_extractor.py
--rw-rw-rw-   0        0        0     2972 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/video_reducer.py
--rw-rw-rw-   0        0        0     9581 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/modules/vision/vis_kit.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.004780 alfred-py-3.0.6/alfred/protos/
--rw-rw-rw-   0        0        0     5249 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/protos/labelmap_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.008767 alfred-py-3.0.6/alfred/siren/
--rw-rw-rw-   0        0        0     9211 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/handler.py
--rw-rw-rw-   0        0        0     3808 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/models.py
--rw-rw-rw-   0        0        0      552 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/siren/topicgen.py
--rw-rw-rw-   0        0        0     2118 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.022730 alfred-py-3.0.6/alfred/utils/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/__init__.py
--rw-rw-rw-   0        0        0     1323 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/base_config.py
--rw-rw-rw-   0        0        0     1509 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/communicate.py
--rw-rw-rw-   0        0        0      792 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/cv_wrapper.py
--rw-rw-rw-   0        0        0    29308 2023-04-11 03:00:54.000000 alfred-py-3.0.6/alfred/utils/file_io.py
--rw-rw-rw-   0        0        0      695 2023-04-10 06:58:27.000000 alfred-py-3.0.6/alfred/utils/image_convertor.py
--rw-rw-rw-   0        0        0     2084 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/log.py
--rw-rw-rw-   0        0        0     1782 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/mana.py
--rw-rw-rw-   0        0        0     1093 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/math_utils.py
--rw-rw-rw-   0        0        0      572 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/pprint.py
--rw-rw-rw-   0        0        0     3327 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/utils/timer.py
--rw-rw-rw-   0        0        0      595 2023-04-12 11:13:37.000000 alfred-py-3.0.6/alfred/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.023728 alfred-py-3.0.6/alfred/vis/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.040682 alfred-py-3.0.6/alfred/vis/image/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/__init__.py
--rw-rw-rw-   0        0        0     5377 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/common.py
--rw-rw-rw-   0        0        0     4804 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/constants.py
--rw-rw-rw-   0        0        0    33098 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/det.py
--rw-rw-rw-   0        0        0     1228 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/face.py
--rw-rw-rw-   0        0        0    12540 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/get_dataset_color_map.py
--rw-rw-rw-   0        0        0    57388 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/get_dataset_label_map.py
--rw-rw-rw-   0        0        0    16379 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/mask.py
--rw-rw-rw-   0        0        0    21942 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose.py
--rw-rw-rw-   0        0        0     6154 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_dataset_info.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.053648 alfred-py-3.0.6/alfred/vis/image/pose_datasets/
--rw-rw-rw-   0        0        0     5581 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/animalpose.py
--rw-rw-rw-   0        0        0     5433 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco.py
--rw-rw-rw-   0        0        0    31889 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody.py
--rw-rw-rw-   0        0        0    11622 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_face.py
--rw-rw-rw-   0        0        0     5145 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_hand.py
--rw-rw-rw-   0        0        0     4915 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand2d.py
--rw-rw-rw-   0        0        0    13576 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/interhand3d.py
--rw-rw-rw-   0        0        0     4765 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/mpii.py
--rw-rw-rw-   0        0        0     4918 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_datasets/onehand10k.py
--rw-rw-rw-   0        0        0     6115 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/pose_hand.py
--rw-rw-rw-   0        0        0      355 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/process.py
--rw-rw-rw-   0        0        0     2544 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/image/seg.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.059632 alfred-py-3.0.6/alfred/vis/mesh3d/
--rw-rw-rw-   0        0        0    36188 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3d_visconfig.py
--rw-rw-rw-   0        0        0     8595 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3dsocket.py
--rw-rw-rw-   0        0        0    15713 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/o3dwrapper.py
--rw-rw-rw-   0        0        0     5696 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/skelmodel.py
--rw-rw-rw-   0        0        0     9602 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/mesh3d/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.061627 alfred-py-3.0.6/alfred/vis/pointcloud/
--rw-rw-rw-   0        0        0      912 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/pointcloud/__init__.py
--rw-rw-rw-   0        0        0     4572 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/pointcloud/pointcloud_vis.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.064619 alfred-py-3.0.6/alfred/vis/renders/
--rw-rw-rw-   0        0        0     8587 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/renders/render_p3d.py
--rw-rw-rw-   0        0        0     4753 2023-02-10 05:13:33.000000 alfred-py-3.0.6/alfred/vis/renders/render_prd.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:13:40.073011 alfred-py-3.0.6/alfred_py.egg-info/
--rw-rw-rw-   0        0        0    25052 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6148 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      174 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-12 11:13:39.000000 alfred-py-3.0.6/alfred_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      441 2023-04-12 11:13:40.075701 alfred-py-3.0.6/setup.cfg
--rw-rw-rw-   0        0        0     5160 2023-02-10 05:13:33.000000 alfred-py-3.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.082780 alfred-py-3.0.7/
+-rw-rw-rw-   0        0        0    35786 2023-04-08 07:17:55.000000 alfred-py-3.0.7/LICENSE
+-rw-rw-rw-   0        0        0      151 2023-04-08 07:17:55.000000 alfred-py-3.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    25052 2023-04-17 14:03:03.082780 alfred-py-3.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    24015 2023-04-08 07:17:55.000000 alfred-py-3.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.789880 alfred-py-3.0.7/alfred/
+-rw-rw-rw-   0        0        0     1349 2023-04-17 14:01:22.000000 alfred-py-3.0.7/alfred/__init__.py
+-rw-rw-rw-   0        0        0    27005 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/alfred.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.754462 alfred-py-3.0.7/alfred/deploy/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.797859 alfred-py-3.0.7/alfred/deploy/tensorrt/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/deploy/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/deploy/tensorrt/calibrator.py
+-rw-rw-rw-   0        0        0    20879 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/deploy/tensorrt/common.py
+-rw-rw-rw-   0        0        0     3366 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/deploy/tensorrt/process.py
+-rw-rw-rw-   0        0        0     3967 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/deploy/tensorrt/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.799853 alfred-py-3.0.7/alfred/dl/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.756456 alfred-py-3.0.7/alfred/dl/data/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.801848 alfred-py-3.0.7/alfred/dl/data/common/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/data/common/__init__.py
+-rw-rw-rw-   0        0        0     6472 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/data/common/coco_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.808829 alfred-py-3.0.7/alfred/dl/data/meta/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/data/meta/__init__.py
+-rw-rw-rw-   0        0        0     1534 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/data/meta/concatenated_dataset.py
+-rw-rw-rw-   0        0        0     3013 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/data/meta/dataset_mixin.py
+-rw-rw-rw-   0        0        0     3262 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/data/meta/getter_dataset.py
+-rw-rw-rw-   0        0        0     5224 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/data/meta/sliceable_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.810824 alfred-py-3.0.7/alfred/dl/evaluator/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/evaluator/__init__.py
+-rw-rw-rw-   0        0        0    11951 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/evaluator/yolo_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.814813 alfred-py-3.0.7/alfred/dl/inference/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/inference/__init__.py
+-rw-rw-rw-   0        0        0     5058 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/inference/image_inference.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.818802 alfred-py-3.0.7/alfred/dl/metrics/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/metrics/__init__.py
+-rw-rw-rw-   0        0        0    11854 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/metrics/iou_loss.py
+-rw-rw-rw-   0        0        0     7873 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/metrics/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.819800 alfred-py-3.0.7/alfred/dl/tf/
+-rw-rw-rw-   0        0        0     1135 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/tf/common.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.830771 alfred-py-3.0.7/alfred/dl/torch/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/torch/__init__.py
+-rw-rw-rw-   0        0        0     3054 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/torch/common.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.832765 alfred-py-3.0.7/alfred/dl/torch/distribute/
+-rw-rw-rw-   0        0        0     8515 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/distribute/utils.py
+-rw-rw-rw-   0        0        0     3406 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/env.py
+-rw-rw-rw-   0        0        0     1150 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/gpu.py
+-rw-rw-rw-   0        0        0    11295 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/metrics.py
+-rw-rw-rw-   0        0        0     6458 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/model_summary.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.836755 alfred-py-3.0.7/alfred/dl/torch/nn/
+-rw-rw-rw-   0        0        0     1038 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/torch/nn/__init__.py
+-rw-rw-rw-   0        0        0     1213 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/nn/functional.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.840744 alfred-py-3.0.7/alfred/dl/torch/nn/modules/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/torch/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0     3880 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/nn/modules/common.py
+-rw-rw-rw-   0        0        0     1166 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/nn/modules/normalization.py
+-rw-rw-rw-   0        0        0     1957 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/nn/weights_init.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.844734 alfred-py-3.0.7/alfred/dl/torch/ops/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/dl/torch/ops/__init__.py
+-rw-rw-rw-   0        0        0     2005 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/ops/array_ops.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.845731 alfred-py-3.0.7/alfred/dl/torch/runner/
+-rw-rw-rw-   0        0        0    10031 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/runner/checkpoint.py
+-rw-rw-rw-   0        0        0     3253 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.856701 alfred-py-3.0.7/alfred/dl/torch/train/
+-rw-rw-rw-   0        0        0     1177 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/__init__.py
+-rw-rw-rw-   0        0        0     7458 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/checkpoint.py
+-rw-rw-rw-   0        0        0     1655 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/common.py
+-rw-rw-rw-   0        0        0    12651 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/fastai_optim.py
+-rw-rw-rw-   0        0        0     7479 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/learning_schedules.py
+-rw-rw-rw-   0        0        0     6666 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/learning_schedules_fastai.py
+-rw-rw-rw-   0        0        0     5081 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/dl/torch/train/optim.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.857699 alfred-py-3.0.7/alfred/fonts/
+-rw-rw-rw-   0        0        0  2763148 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/fonts/FZSSJW.TTF
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.877647 alfred-py-3.0.7/alfred/fusion/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/fusion/__init__.py
+-rw-rw-rw-   0        0        0     5794 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/fusion/common.py
+-rw-rw-rw-   0        0        0     2165 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/fusion/geometry.py
+-rw-rw-rw-   0        0        0     9735 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/fusion/kitti_fusion.py
+-rw-rw-rw-   0        0        0     4048 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/fusion/nuscenes_fusion.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.879641 alfred-py-3.0.7/alfred/modules/
+-rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.894115 alfred-py-3.0.7/alfred/modules/cabinet/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/__init__.py
+-rw-rw-rw-   0        0        0     1075 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/changesource.py
+-rw-rw-rw-   0        0        0     1658 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/count_file.py
+-rw-rw-rw-   0        0        0    19615 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/gtrend.py
+-rw-rw-rw-   0        0        0    25291 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/license.py
+-rw-rw-rw-   0        0        0     6046 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/markdown_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.901096 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.908079 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/html.py
+-rw-rw-rw-   0        0        0      951 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/pdf.py
+-rw-rw-rw-   0        0        0      214 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/simple.py
+-rw-rw-rw-   0        0        0     5356 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/image_downloader.py
+-rw-rw-rw-   0        0        0      437 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/string_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.911070 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.914062 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/html/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/html/__init__.py
+-rw-rw-rw-   0        0        0     2209 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/html/transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.917054 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/md/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/md/__init__.py
+-rw-rw-rw-   0        0        0     2220 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/md/transformer.py
+-rw-rw-rw-   0        0        0     1859 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/mdparse/www_tools.py
+-rw-rw-rw-   0        0        0     2710 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/split_txt.py
+-rw-rw-rw-   0        0        0     1802 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/stack_imgs.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.934009 alfred-py-3.0.7/alfred/modules/cabinet/templates/
+-rw-rw-rw-   0        0        0      742 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/agpl-v3.tmpl
+-rw-rw-rw-   0        0        0      868 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/apache-2.tmpl
+-rw-rw-rw-   0        0        0      170 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/bsd-3.tmpl
+-rw-rw-rw-   0        0        0     1448 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill-B.tmpl
+-rw-rw-rw-   0        0        0     1448 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill-C.tmpl
+-rw-rw-rw-   0        0        0     1442 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill.tmpl
+-rw-rw-rw-   0        0        0      721 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/gpl-v3.tmpl
+-rw-rw-rw-   0        0        0      744 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl
+-rw-rw-rw-   0        0        0      742 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/cabinet/templates/lgpl-v3.tmpl
+-rw-rw-rw-   0        0        0     2125 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/cabinet/webcam.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.969913 alfred-py-3.0.7/alfred/modules/data/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/data/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/data/coco2voc.py
+-rw-rw-rw-   0        0        0     2943 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/coco2yolo.py
+-rw-rw-rw-   0        0        0     3639 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/convert_csv2voc.py
+-rw-rw-rw-   0        0        0     7674 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/convert_cvat2voc.py
+-rw-rw-rw-   0        0        0     4297 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/convert_labelone2voc.py
+-rw-rw-rw-   0        0        0      158 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/eval_coco.py
+-rw-rw-rw-   0        0        0    40286 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/eval_voc.py
+-rw-rw-rw-   0        0        0     6034 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/extract_voc.py
+-rw-rw-rw-   0        0        0     2566 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/gather_voclabels.py
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/data/labelone_view.py
+-rw-rw-rw-   0        0        0     4540 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/mergevoc.py
+-rw-rw-rw-   0        0        0     2641 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/split_coco.py
+-rw-rw-rw-   0        0        0     1639 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/split_voc.py
+-rw-rw-rw-   0        0        0     3580 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/txt2voc.py
+-rw-rw-rw-   0        0        0    10384 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/view_coco.py
+-rw-rw-rw-   0        0        0     3776 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/view_txt.py
+-rw-rw-rw-   0        0        0     5778 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/view_voc.py
+-rw-rw-rw-   0        0        0     3159 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/view_yolo.py
+-rw-rw-rw-   0        0        0     8501 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/data/voc2coco.py
+-rw-rw-rw-   0        0        0     2044 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/voc2yolo.py
+-rw-rw-rw-   0        0        0     4363 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/data/yolo2voc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.971907 alfred-py-3.0.7/alfred/modules/dltool/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/dltool/__init__.py
+-rw-rw-rw-   0        0        0     5554 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/dltool/cal_anchors.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.975899 alfred-py-3.0.7/alfred/modules/scrap/
+-rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/scrap/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/scrap/image_scraper.py
+-rw-rw-rw-   0        0        0     5459 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/scrap/scraper_images.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.976896 alfred-py-3.0.7/alfred/modules/text/
+-rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.985872 alfred-py-3.0.7/alfred/modules/vision/
+-rw-rw-rw-   0        0        0      937 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/modules/vision/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/vision/face_extractor.py
+-rw-rw-rw-   0        0        0     3221 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/vision/to_video.py
+-rw-rw-rw-   0        0        0     3161 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/vision/video_extractor.py
+-rw-rw-rw-   0        0        0     3219 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/vision/video_reducer.py
+-rw-rw-rw-   0        0        0    10334 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/modules/vision/vis_kit.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.987378 alfred-py-3.0.7/alfred/protos/
+-rw-rw-rw-   0        0        0     6299 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/protos/labelmap_pb2.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:02.992366 alfred-py-3.0.7/alfred/siren/
+-rw-rw-rw-   0        0        0     9187 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/siren/handler.py
+-rw-rw-rw-   0        0        0     3759 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/siren/models.py
+-rw-rw-rw-   0        0        0      563 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/siren/topicgen.py
+-rw-rw-rw-   0        0        0     2120 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.015304 alfred-py-3.0.7/alfred/utils/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/utils/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/base_config.py
+-rw-rw-rw-   0        0        0     1509 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/communicate.py
+-rw-rw-rw-   0        0        0      808 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/cv_wrapper.py
+-rw-rw-rw-   0        0        0    30265 2023-04-17 14:01:42.000000 alfred-py-3.0.7/alfred/utils/file_io.py
+-rw-rw-rw-   0        0        0      697 2023-04-17 14:02:00.000000 alfred-py-3.0.7/alfred/utils/image_convertor.py
+-rw-rw-rw-   0        0        0     2084 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/log.py
+-rw-rw-rw-   0        0        0     1858 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/mana.py
+-rw-rw-rw-   0        0        0     1093 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/utils/math_utils.py
+-rw-rw-rw-   0        0        0      574 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/pprint.py
+-rw-rw-rw-   0        0        0     1416 2023-04-17 14:01:22.000000 alfred-py-3.0.7/alfred/utils/progress.py
+-rw-rw-rw-   0        0        0     3434 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/utils/timer.py
+-rw-rw-rw-   0        0        0      595 2023-04-17 14:02:32.000000 alfred-py-3.0.7/alfred/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.016302 alfred-py-3.0.7/alfred/vis/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.037898 alfred-py-3.0.7/alfred/vis/image/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/image/__init__.py
+-rw-rw-rw-   0        0        0     5570 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/common.py
+-rw-rw-rw-   0        0        0     4804 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/image/constants.py
+-rw-rw-rw-   0        0        0    33415 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/det.py
+-rw-rw-rw-   0        0        0     1226 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/face.py
+-rw-rw-rw-   0        0        0    13825 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/get_dataset_color_map.py
+-rw-rw-rw-   0        0        0    39672 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/get_dataset_label_map.py
+-rw-rw-rw-   0        0        0    16375 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/mask.py
+-rw-rw-rw-   0        0        0    21942 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/image/pose.py
+-rw-rw-rw-   0        0        0     6152 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_dataset_info.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.051861 alfred-py-3.0.7/alfred/vis/image/pose_datasets/
+-rw-rw-rw-   0        0        0     5024 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/animalpose.py
+-rw-rw-rw-   0        0        0     5026 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco.py
+-rw-rw-rw-   0        0        0    26998 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco_wholebody.py
+-rw-rw-rw-   0        0        0     7804 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco_wholebody_face.py
+-rw-rw-rw-   0        0        0     4404 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco_wholebody_hand.py
+-rw-rw-rw-   0        0        0     4020 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/interhand2d.py
+-rw-rw-rw-   0        0        0    12466 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/interhand3d.py
+-rw-rw-rw-   0        0        0     4455 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/mpii.py
+-rw-rw-rw-   0        0        0     4014 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/pose_datasets/onehand10k.py
+-rw-rw-rw-   0        0        0     6115 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/image/pose_hand.py
+-rw-rw-rw-   0        0        0      361 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/process.py
+-rw-rw-rw-   0        0        0     2614 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/image/seg.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.058842 alfred-py-3.0.7/alfred/vis/mesh3d/
+-rw-rw-rw-   0        0        0    27243 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/mesh3d/o3d_visconfig.py
+-rw-rw-rw-   0        0        0     8501 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/mesh3d/o3dsocket.py
+-rw-rw-rw-   0        0        0    19729 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/mesh3d/o3dwrapper.py
+-rw-rw-rw-   0        0        0     5883 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/mesh3d/skelmodel.py
+-rw-rw-rw-   0        0        0     9857 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/mesh3d/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.061834 alfred-py-3.0.7/alfred/vis/pointcloud/
+-rw-rw-rw-   0        0        0      912 2023-04-08 07:17:55.000000 alfred-py-3.0.7/alfred/vis/pointcloud/__init__.py
+-rw-rw-rw-   0        0        0     4718 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/pointcloud/pointcloud_vis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.065823 alfred-py-3.0.7/alfred/vis/renders/
+-rw-rw-rw-   0        0        0     8719 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/renders/render_p3d.py
+-rw-rw-rw-   0        0        0     4721 2023-04-17 14:01:15.000000 alfred-py-3.0.7/alfred/vis/renders/render_prd.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:03:03.079788 alfred-py-3.0.7/alfred_py.egg-info/
+-rw-rw-rw-   0        0        0    25052 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6173 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 14:03:02.000000 alfred-py-3.0.7/alfred_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      441 2023-04-17 14:03:03.084775 alfred-py-3.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     5004 2023-04-17 14:01:15.000000 alfred-py-3.0.7/setup.py
```

### Comparing `alfred-py-3.0.6/LICENSE` & `alfred-py-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/PKG-INFO` & `alfred-py-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-py
-Version: 3.0.6
+Version: 3.0.7
 Summary: Alfred is a DeepLearning utility library.
 Home-page: https://github.com/jinfagang/alfred
 Author: Lucas Jin
 Author-email: jinfagang19@163.com
 License: GPL-3.0
 Keywords: deep learning,script helper,tools
 Platform: any
```

### Comparing `alfred-py-3.0.6/README.md` & `alfred-py-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/__init__.py` & `alfred-py-3.0.7/alfred/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 """Bring in all of the public Alfred interface into this module."""
 import importlib
+
 # pylint: disable=g-bad-import-order
 
 from .modules import *
 from .vis import *
 from .fusion import *
 from .dl.torch.common import print_shape
 from .utils.log import logger
 from .dl.torch.common import device
+from .utils.progress import pbar, prange
 
-globals().update(importlib.import_module('alfred').__dict__)
+globals().update(importlib.import_module("alfred").__dict__)
```

### Comparing `alfred-py-3.0.6/alfred/alfred.py` & `alfred-py-3.0.7/alfred/alfred.py`

 * *Files 17% similar despite different names*

```diff
@@ -63,510 +63,595 @@
 from .utils.log import logger as logging
 from .version import __version__, short_version
 from datetime import datetime
 
 dt = datetime.now()
 
 
-__VERSION__ = f'👍    {__version__}'
-__AUTHOR__ = '😀    Lucas Jin'
-__CONTACT__ = '😍    telegram: lucasjin'
+__VERSION__ = f"👍    {__version__}"
+__AUTHOR__ = "😀    Lucas Jin"
+__CONTACT__ = "😍    telegram: lucasjin"
 __DATE__ = f"👉    {dt.strftime('%Y.%m.%d')}, since 2019.11.11"
-__LOC__ = '👉    Shenzhen, China'
-__git__ = '👍    http://github.com/jinfagang/alfred'
+__LOC__ = "👉    Shenzhen, China"
+__git__ = "👍    http://github.com/jinfagang/alfred"
 
 
 def arg_parse():
     """
     parse arguments
     :return:
     """
     parser = argparse.ArgumentParser(prog="alfred")
-    parser.add_argument('--version', '-v',
-                        action="store_true", help='show version info.')
+    parser.add_argument(
+        "--version", "-v", action="store_true", help="show version info."
+    )
 
     # vision, text, scrap
     main_sub_parser = parser.add_subparsers()
 
     # =============== vision part ================
     vision_parser = main_sub_parser.add_parser(
-        'vision', help='vision related commands.')
+        "vision", help="vision related commands."
+    )
     vision_sub_parser = vision_parser.add_subparsers()
 
-    vision_extract_parser = vision_sub_parser.add_parser('extract', help='extract image from video: alfred vision '
-                                                                         'extract -v tt.mp4')
-    vision_extract_parser.set_defaults(which='vision-extract')
+    vision_extract_parser = vision_sub_parser.add_parser(
+        "extract", help="extract image from video: alfred vision " "extract -v tt.mp4"
+    )
+    vision_extract_parser.set_defaults(which="vision-extract")
+    vision_extract_parser.add_argument("--video", "-v", help="video to extract")
     vision_extract_parser.add_argument(
-        '--video', '-v', help='video to extract')
-    vision_extract_parser.add_argument(
-        '--jumps', '-j', help='jump frames for wide extract')
+        "--jumps", "-j", help="jump frames for wide extract"
+    )
 
-    vision_reduce_parser = vision_sub_parser.add_parser('reduce', help='reduce video by drop frames'
-                                                                       '\nalfred vision reduce -v a.mp4 -j 10')
-    vision_reduce_parser.set_defaults(which='vision-reduce')
-    vision_reduce_parser.add_argument('--video', '-v', help='video to extract')
+    vision_reduce_parser = vision_sub_parser.add_parser(
+        "reduce",
+        help="reduce video by drop frames" "\nalfred vision reduce -v a.mp4 -j 10",
+    )
+    vision_reduce_parser.set_defaults(which="vision-reduce")
+    vision_reduce_parser.add_argument("--video", "-v", help="video to extract")
     vision_reduce_parser.add_argument(
-        '--jumps', '-j', help='jump frames for wide extract')
+        "--jumps", "-j", help="jump frames for wide extract"
+    )
 
-    vision_2video_parser = vision_sub_parser.add_parser('2video', help='combine into a video: alfred vision '
-                                                                       '2video  -d ./images')
-    vision_2video_parser.set_defaults(which='vision-2video')
+    vision_2video_parser = vision_sub_parser.add_parser(
+        "2video", help="combine into a video: alfred vision " "2video  -d ./images"
+    )
+    vision_2video_parser.set_defaults(which="vision-2video")
     vision_2video_parser.add_argument(
-        '--dir', '-d', help='dir contains image sequences.')
+        "--dir", "-d", help="dir contains image sequences."
+    )
 
     vision_clean_parser = vision_sub_parser.add_parser(
-        'clean', help='clean images in a dir.')
-    vision_clean_parser.set_defaults(which='vision-clean')
-    vision_clean_parser.add_argument(
-        '--dir', '-d', help='dir contains images.')
+        "clean", help="clean images in a dir."
+    )
+    vision_clean_parser.set_defaults(which="vision-clean")
+    vision_clean_parser.add_argument("--dir", "-d", help="dir contains images.")
 
     vision_getface_parser = vision_sub_parser.add_parser(
-        'getface', help='get all faces inside an image and save it.')
-    vision_getface_parser.set_defaults(which='vision-getface')
+        "getface", help="get all faces inside an image and save it."
+    )
+    vision_getface_parser.set_defaults(which="vision-getface")
     vision_getface_parser.add_argument(
-        '--dir', '-d', help='dir contains images to extract faces.')
+        "--dir", "-d", help="dir contains images to extract faces."
+    )
 
     # =============== text part ================
-    text_parser = main_sub_parser.add_parser(
-        'text', help='text related commands.')
+    text_parser = main_sub_parser.add_parser("text", help="text related commands.")
     text_sub_parser = text_parser.add_subparsers()
 
-    text_clean_parser = text_sub_parser.add_parser('clean', help='clean text.')
-    text_clean_parser.set_defaults(which='text-clean')
-    text_clean_parser.add_argument('--file', '-f', help='file to clean')
-
-    text_translate_parser = text_sub_parser.add_parser(
-        'translate', help='translate')
-    text_translate_parser.set_defaults(which='text-translate')
+    text_clean_parser = text_sub_parser.add_parser("clean", help="clean text.")
+    text_clean_parser.set_defaults(which="text-clean")
+    text_clean_parser.add_argument("--file", "-f", help="file to clean")
+
+    text_translate_parser = text_sub_parser.add_parser("translate", help="translate")
+    text_translate_parser.set_defaults(which="text-translate")
     text_translate_parser.add_argument(
-        '--file', '-f', help='translate a words to target language')
+        "--file", "-f", help="translate a words to target language"
+    )
 
     # =============== scrap part ================
-    scrap_parser = main_sub_parser.add_parser(
-        'scrap', help='scrap related commands.')
+    scrap_parser = main_sub_parser.add_parser("scrap", help="scrap related commands.")
     scrap_sub_parser = scrap_parser.add_subparsers()
 
-    scrap_image_parser = scrap_sub_parser.add_parser(
-        'image', help='scrap images.')
-    scrap_image_parser.set_defaults(which='scrap-image')
-    scrap_image_parser.add_argument('--query', '-q', help='query words.')
+    scrap_image_parser = scrap_sub_parser.add_parser("image", help="scrap images.")
+    scrap_image_parser.set_defaults(which="scrap-image")
+    scrap_image_parser.add_argument("--query", "-q", help="query words.")
 
     # =============== cabinet part ================
-    cabinet_parser = main_sub_parser.add_parser(
-        'cab', help='cabinet related commands.')
+    cabinet_parser = main_sub_parser.add_parser("cab", help="cabinet related commands.")
     cabinet_sub_parser = cabinet_parser.add_subparsers()
 
-    count_file_parser = cabinet_sub_parser.add_parser(
-        'count', help='scrap images.')
-    count_file_parser.set_defaults(which='cab-count')
-    count_file_parser.add_argument(
-        '--dir', '-d', default='./', help='dir to count.')
-    count_file_parser.add_argument('--type', '-t', help='dir to count.')
-
-    split_txt_parser = cabinet_sub_parser.add_parser(
-        'split', help='split txt file.')
-    split_txt_parser.set_defaults(which='cab-split')
-    split_txt_parser.add_argument(
-        '--file', '-f', required=True, help='file to split.')
-    split_txt_parser.add_argument('--ratios', '-r', help='ratios.')
-    split_txt_parser.add_argument('--names', '-n', help='names.')
+    count_file_parser = cabinet_sub_parser.add_parser("count", help="scrap images.")
+    count_file_parser.set_defaults(which="cab-count")
+    count_file_parser.add_argument("--dir", "-d", default="./", help="dir to count.")
+    count_file_parser.add_argument("--type", "-t", help="dir to count.")
+
+    split_txt_parser = cabinet_sub_parser.add_parser("split", help="split txt file.")
+    split_txt_parser.set_defaults(which="cab-split")
+    split_txt_parser.add_argument("--file", "-f", required=True, help="file to split.")
+    split_txt_parser.add_argument("--ratios", "-r", help="ratios.")
+    split_txt_parser.add_argument("--names", "-n", help="names.")
 
     stackimgs_parser = cabinet_sub_parser.add_parser(
-        'stackimgs', help='stack images into one')
-    stackimgs_parser.set_defaults(which='cab-stackimgs')
+        "stackimgs", help="stack images into one"
+    )
+    stackimgs_parser.set_defaults(which="cab-stackimgs")
     stackimgs_parser.add_argument(
-        '--imgs', '-i', required=True, nargs='+', help='images list.')
-    stackimgs_parser.add_argument('--dim', '-d', help='dims like 2x3.')
+        "--imgs", "-i", required=True, nargs="+", help="images list."
+    )
+    stackimgs_parser.add_argument("--dim", "-d", help="dims like 2x3.")
 
     apply_license_parser = cabinet_sub_parser.add_parser(
-        'license', help='automatically add/update license.')
-    apply_license_parser.set_defaults(which='cab-license')
-    apply_license_parser.add_argument(
-        '--owner', '-o', required=True, help='owner of license.')
-    apply_license_parser.add_argument('--name', '-n', help='project name.')
+        "license", help="automatically add/update license."
+    )
+    apply_license_parser.set_defaults(which="cab-license")
     apply_license_parser.add_argument(
-        '--year', '-y', help='project year: 2016-2020.')
+        "--owner", "-o", required=True, help="owner of license."
+    )
+    apply_license_parser.add_argument("--name", "-n", help="project name.")
+    apply_license_parser.add_argument("--year", "-y", help="project year: 2016-2020.")
     apply_license_parser.add_argument(
-        '--url', '-u', default='manaai.cn', help='your website url.')
+        "--url", "-u", default="manaai.cn", help="your website url."
+    )
     apply_license_parser.add_argument(
-        '--dir', '-d', default='./', help='to apply license dir.')
+        "--dir", "-d", default="./", help="to apply license dir."
+    )
     apply_license_parser.add_argument(
-        '--except', '-e', help='except extensions: xml,cc,h')
+        "--except", "-e", help="except extensions: xml,cc,h"
+    )
+
+    webcam_parser = cabinet_sub_parser.add_parser("webcam", help="Test your webcam.")
+    webcam_parser.set_defaults(which="cab-webcam")
+    webcam_parser.add_argument("--file", "-f", help="Also can set file.")
 
-    webcam_parser = cabinet_sub_parser.add_parser(
-        'webcam', help='Test your webcam.')
-    webcam_parser.set_defaults(which='cab-webcam')
-    webcam_parser.add_argument(
-        '--file', '-f', help='Also can set file.')
-    
     gtrend_parser = cabinet_sub_parser.add_parser(
-        'gtrend', help='Get github trending in terminal.')
-    gtrend_parser.set_defaults(which='cab-gtrend')
+        "gtrend", help="Get github trending in terminal."
+    )
+    gtrend_parser.set_defaults(which="cab-gtrend")
     gtrend_parser.add_argument(
-        '--language', '-l', default='', help='Also can set file.')
+        "--language", "-l", default="", help="Also can set file."
+    )
     gtrend_parser.add_argument(
-        '--layout', '-L', default='table', help='default layout.')
+        "--layout", "-L", default="table", help="default layout."
+    )
 
     changesource_parser = cabinet_sub_parser.add_parser(
-        'changesource', help='Test your changesource_parser.')
-    changesource_parser.set_defaults(which='cab-changesource')
+        "changesource", help="Test your changesource_parser."
+    )
+    changesource_parser.set_defaults(which="cab-changesource")
     changesource_parser.add_argument(
-        '--source', '-s', help='aliyun or tsinghua or douban.')
+        "--source", "-s", help="aliyun or tsinghua or douban."
+    )
 
     downmd_parser = cabinet_sub_parser.add_parser(
-        'downmd', help='Download all images to local from a markdown file.')
-    downmd_parser.set_defaults(which='cab-downmd')
-    downmd_parser.add_argument(
-        '--file', '-f', help='Also can set file.')
+        "downmd", help="Download all images to local from a markdown file."
+    )
+    downmd_parser.set_defaults(which="cab-downmd")
+    downmd_parser.add_argument("--file", "-f", help="Also can set file.")
 
     # =============== dl tools part =============
     dltool_parser = main_sub_parser.add_parser(
-        'dltool', help='dltool related commands.')
+        "dltool", help="dltool related commands."
+    )
     dltool_sub_parser = dltool_parser.add_subparsers()
 
     anchor_parser = dltool_sub_parser.add_parser(
-        'anchor', help='calculate anchors for you.')
-    anchor_parser.set_defaults(which='dltool-anchor')
+        "anchor", help="calculate anchors for you."
+    )
+    anchor_parser.set_defaults(which="dltool-anchor")
     anchor_parser.add_argument(
-        '--annotation_dir', '-a', help='VOC xml dir or yolo lables dir.')
+        "--annotation_dir", "-a", help="VOC xml dir or yolo lables dir."
+    )
     anchor_parser.add_argument(
-        '--cluster_num', '-c', default=9, help='how many clusters to kmeans.')
+        "--cluster_num", "-c", default=9, help="how many clusters to kmeans."
+    )
     anchor_parser.add_argument(
-        '--format', '-f', default='voc', help='Your annotation format: voc | yolo.')
+        "--format", "-f", default="voc", help="Your annotation format: voc | yolo."
+    )
 
     # =============== data part ================
-    data_parser = main_sub_parser.add_parser(
-        'data', help='data related commands.')
+    data_parser = main_sub_parser.add_parser("data", help="data related commands.")
     data_sub_parser = data_parser.add_subparsers()
 
-    view_voc_parser = data_sub_parser.add_parser('vocview', help='view voc.')
-    view_voc_parser.set_defaults(which='data-vocview')
-    view_voc_parser.add_argument(
-        '--image_dir', '-i', help='Root path of VOC image.')
-    view_voc_parser.add_argument(
-        '--label_dir', '-l', help='Root path of VOC label.')
-
-    view_txt_parser = data_sub_parser.add_parser('txtview', help='view voc.')
-    view_txt_parser.set_defaults(which='data-txtview')
-    view_txt_parser.add_argument(
-        '--image_dir', '-i', help='Root path of VOC image.')
-    view_txt_parser.add_argument(
-        '--label_dir', '-l', help='Root path of VOC label.')
-
-    view_txt_parser = data_sub_parser.add_parser('yoloview', help='view yolo.')
-    view_txt_parser.set_defaults(which='data-yoloview')
-    view_txt_parser.add_argument(
-        '--image_dir', '-i', help='Root path of VOC image.')
-    view_txt_parser.add_argument(
-        '--label_dir', '-l', help='Root path of VOC label.')
-
-    view_coco_parser = data_sub_parser.add_parser('cocoview', help='view voc.')
-    view_coco_parser.set_defaults(which='data-cocoview')
+    view_voc_parser = data_sub_parser.add_parser("vocview", help="view voc.")
+    view_voc_parser.set_defaults(which="data-vocview")
+    view_voc_parser.add_argument("--image_dir", "-i", help="Root path of VOC image.")
+    view_voc_parser.add_argument("--label_dir", "-l", help="Root path of VOC label.")
+
+    view_txt_parser = data_sub_parser.add_parser("txtview", help="view voc.")
+    view_txt_parser.set_defaults(which="data-txtview")
+    view_txt_parser.add_argument("--image_dir", "-i", help="Root path of VOC image.")
+    view_txt_parser.add_argument("--label_dir", "-l", help="Root path of VOC label.")
+
+    view_txt_parser = data_sub_parser.add_parser("yoloview", help="view yolo.")
+    view_txt_parser.set_defaults(which="data-yoloview")
+    view_txt_parser.add_argument("--image_dir", "-i", help="Root path of VOC image.")
+    view_txt_parser.add_argument("--label_dir", "-l", help="Root path of VOC label.")
+
+    view_coco_parser = data_sub_parser.add_parser("cocoview", help="view voc.")
+    view_coco_parser.set_defaults(which="data-cocoview")
+    view_coco_parser.add_argument("--image_dir", "-i", help="Root path of COCO images.")
     view_coco_parser.add_argument(
-        '--image_dir', '-i', help='Root path of COCO images.')
-    view_coco_parser.add_argument(
-        '--json', '-j', help='Root path of COCO annotations.json .')
+        "--json", "-j", help="Root path of COCO annotations.json ."
+    )
 
     voc_label_parser = data_sub_parser.add_parser(
-        'voclabel', help='gather labels from annotations dir.')
-    voc_label_parser.set_defaults(which='data-voclabel')
-    voc_label_parser.add_argument(
-        '--anno_dir', '-d', help='dir to annotations.')
+        "voclabel", help="gather labels from annotations dir."
+    )
+    voc_label_parser.set_defaults(which="data-voclabel")
+    voc_label_parser.add_argument("--anno_dir", "-d", help="dir to annotations.")
 
     split_voc_parser = data_sub_parser.add_parser(
-        'splitvoc', help='split VOC to train and val.')
-    split_voc_parser.set_defaults(which='data-splitvoc')
-    split_voc_parser.add_argument(
-        '--image_dir', '-i', help='Root path of VOC image.')
-    split_voc_parser.add_argument(
-        '--label_dir', '-l', help='Root path of VOC label.')
+        "splitvoc", help="split VOC to train and val."
+    )
+    split_voc_parser.set_defaults(which="data-splitvoc")
+    split_voc_parser.add_argument("--image_dir", "-i", help="Root path of VOC image.")
+    split_voc_parser.add_argument("--label_dir", "-l", help="Root path of VOC label.")
 
     split_coco_parser = data_sub_parser.add_parser(
-        'splitcoco', help='split coco to train and val.')
-    split_coco_parser.set_defaults(which='data-splitcoco')
+        "splitcoco", help="split coco to train and val."
+    )
+    split_coco_parser.set_defaults(which="data-splitcoco")
     split_coco_parser.add_argument(
-        '--image_dir', '-i', help='Root path of coco image. [optional]')
-    split_coco_parser.add_argument('--json_file', '-j', help='coco json file.')
+        "--image_dir", "-i", help="Root path of coco image. [optional]"
+    )
+    split_coco_parser.add_argument("--json_file", "-j", help="coco json file.")
     split_coco_parser.add_argument(
-        '--split', '-s', default=0.8, help='coco json file split.')
+        "--split", "-s", default=0.8, help="coco json file split."
+    )
 
     labelone2voc_parser = data_sub_parser.add_parser(
-        'labelone2voc', help='convert labelone to VOC.')
-    labelone2voc_parser.set_defaults(which='data-labelone2voc')
+        "labelone2voc", help="convert labelone to VOC."
+    )
+    labelone2voc_parser.set_defaults(which="data-labelone2voc")
     labelone2voc_parser.add_argument(
-        '--json_dir', '-j', help='Root of labelone json dir.')
+        "--json_dir", "-j", help="Root of labelone json dir."
+    )
 
     voc2coco_parser = data_sub_parser.add_parser(
-        'voc2coco', help='convert VOC to coco.')
-    voc2coco_parser.set_defaults(which='data-voc2coco')
+        "voc2coco", help="convert VOC to coco."
+    )
+    voc2coco_parser.set_defaults(which="data-voc2coco")
     voc2coco_parser.add_argument(
-        '--xml_dir', '-d', help='Root of xmls dir (Annotations/).')
+        "--xml_dir", "-d", help="Root of xmls dir (Annotations/)."
+    )
     voc2coco_parser.add_argument(
-        '--img_dir', '-i', help='Root of xmls dir (JPEGImages/).')
+        "--img_dir", "-i", help="Root of xmls dir (JPEGImages/)."
+    )
     voc2coco_parser.add_argument(
-        '--index_1', default=False, help='if index with 1 or not.')
+        "--index_1", default=False, help="if index with 1 or not."
+    )
 
     coco2yolo_parser = data_sub_parser.add_parser(
-        'coco2yolo', help='convert COCO to yolo.')
-    coco2yolo_parser.set_defaults(which='data-coco2yolo')
+        "coco2yolo", help="convert COCO to yolo."
+    )
+    coco2yolo_parser.set_defaults(which="data-coco2yolo")
     coco2yolo_parser.add_argument(
-        '--image_dir', '-i', help='Root of images dir (images/).')
+        "--image_dir", "-i", help="Root of images dir (images/)."
+    )
     coco2yolo_parser.add_argument(
-        '--json_file', '-j', help='coco json annotation file.')
+        "--json_file", "-j", help="coco json annotation file."
+    )
 
     yolo2voc_parser = data_sub_parser.add_parser(
-        'yolo2voc', help='convert yolo to VOC.')
-    yolo2voc_parser.set_defaults(which='data-yolo2voc')
-    yolo2voc_parser.add_argument(
-        '--image_dir', '-i', help='Root of images dir (images/).')
-    yolo2voc_parser.add_argument(
-        '--text_dir', '-t', help='Root of text files.')
+        "yolo2voc", help="convert yolo to VOC."
+    )
+    yolo2voc_parser.set_defaults(which="data-yolo2voc")
     yolo2voc_parser.add_argument(
-        '--class_file', '-c', help='classes name file.')
+        "--image_dir", "-i", help="Root of images dir (images/)."
+    )
+    yolo2voc_parser.add_argument("--text_dir", "-t", help="Root of text files.")
+    yolo2voc_parser.add_argument("--class_file", "-c", help="classes name file.")
 
     voc2yolo_parser = data_sub_parser.add_parser(
-        'voc2yolo', help='convert VOC to yolo.')
-    voc2yolo_parser.set_defaults(which='data-voc2yolo')
-    voc2yolo_parser.add_argument(
-        '--image_dir', '-i', help='Root of images dir (images/).')
-    voc2yolo_parser.add_argument(
-        '--xml_dir', '-x', help='Root of XML files.')
+        "voc2yolo", help="convert VOC to yolo."
+    )
+    voc2yolo_parser.set_defaults(which="data-voc2yolo")
     voc2yolo_parser.add_argument(
-        '--class_file', '-c', help='classes name file.')
+        "--image_dir", "-i", help="Root of images dir (images/)."
+    )
+    voc2yolo_parser.add_argument("--xml_dir", "-x", help="Root of XML files.")
+    voc2yolo_parser.add_argument("--class_file", "-c", help="classes name file.")
 
-    mergevoc_parser = data_sub_parser.add_parser(
-        'mergevoc', help='merge multiple voc.')
-    mergevoc_parser.set_defaults(which='data-mergevoc')
+    mergevoc_parser = data_sub_parser.add_parser("mergevoc", help="merge multiple voc.")
+    mergevoc_parser.set_defaults(which="data-mergevoc")
     mergevoc_parser.add_argument(
-        '--dirs', '-d', nargs='+', help='Root of xmls dir (multiple dirs to merge).')
+        "--dirs", "-d", nargs="+", help="Root of xmls dir (multiple dirs to merge)."
+    )
 
-    evalvoc_parser = data_sub_parser.add_parser(
-        'evalvoc', help='evaluation on VOC.')
-    evalvoc_parser.set_defaults(which='data-evalvoc')
-    evalvoc_parser.add_argument('-g', '--gt_dir', type=str, required=True,
-                                help="Ground truth path (can be xml dir or txt dir, coco json will support soon)")
-    evalvoc_parser.add_argument('-d', '--det_dir', type=str, required=True,
-                                help="Detection result (should saved into txt format)")
-    evalvoc_parser.add_argument('-im', '--images_dir', type=str,
-                                default='images', help="Raw images dir for animation.")
+    evalvoc_parser = data_sub_parser.add_parser("evalvoc", help="evaluation on VOC.")
+    evalvoc_parser.set_defaults(which="data-evalvoc")
     evalvoc_parser.add_argument(
-        '-na', '--no-animation', help="no animation is shown.", action="store_true")
+        "-g",
+        "--gt_dir",
+        type=str,
+        required=True,
+        help="Ground truth path (can be xml dir or txt dir, coco json will support soon)",
+    )
     evalvoc_parser.add_argument(
-        '-np', '--no-plot', help="no plot is shown.", action="store_true")
+        "-d",
+        "--det_dir",
+        type=str,
+        required=True,
+        help="Detection result (should saved into txt format)",
+    )
     evalvoc_parser.add_argument(
-        '-q', '--quiet', help="minimalistic console output.", action="store_true")
+        "-im",
+        "--images_dir",
+        type=str,
+        default="images",
+        help="Raw images dir for animation.",
+    )
     evalvoc_parser.add_argument(
-        '--min_overlap', type=float, default=0.5, help="min overlap, default is 0.5")
+        "-na", "--no-animation", help="no animation is shown.", action="store_true"
+    )
     evalvoc_parser.add_argument(
-        '-i', '--ignore', nargs='+', type=str, help="ignore a list of classes.")
+        "-np", "--no-plot", help="no plot is shown.", action="store_true"
+    )
     evalvoc_parser.add_argument(
-        '--set-class-iou', nargs='+', type=str, help="set IoU for a specific class.")
+        "-q", "--quiet", help="minimalistic console output.", action="store_true"
+    )
+    evalvoc_parser.add_argument(
+        "--min_overlap", type=float, default=0.5, help="min overlap, default is 0.5"
+    )
+    evalvoc_parser.add_argument(
+        "-i", "--ignore", nargs="+", type=str, help="ignore a list of classes."
+    )
+    evalvoc_parser.add_argument(
+        "--set-class-iou", nargs="+", type=str, help="set IoU for a specific class."
+    )
 
     return parser.parse_args()
 
 
 def print_welcome_msg():
-    print('-'*70)
-    print(Fore.BLUE + Style.BRIGHT + '              Alfred ' + Style.RESET_ALL +
-          Fore.WHITE + '- Valet of Artificial Intelligence.' + Style.RESET_ALL)
-    print('         Author : ' + Fore.CYAN +
-          Style.BRIGHT + __AUTHOR__ + Style.RESET_ALL)
-    print('         Contact: ' + Fore.BLUE +
-          Style.BRIGHT + __CONTACT__ + Style.RESET_ALL)
-    print('         At     : ' + Fore.LIGHTGREEN_EX +
-          Style.BRIGHT + __DATE__ + Style.RESET_ALL)
-    print('         Loc    : ' + Fore.LIGHTMAGENTA_EX +
-          Style.BRIGHT + __LOC__ + Style.RESET_ALL)
-    print('         Star   : ' + Fore.MAGENTA +
-          Style.BRIGHT + __git__ + Style.RESET_ALL)
-    print('         Ver.   : ' + Fore.GREEN +
-          Style.BRIGHT + __VERSION__ + Style.RESET_ALL)
-    print('-'*70)
-    print('\n')
+    print("-" * 70)
+    print(
+        Fore.BLUE
+        + Style.BRIGHT
+        + "              Alfred "
+        + Style.RESET_ALL
+        + Fore.WHITE
+        + "- Valet of Artificial Intelligence."
+        + Style.RESET_ALL
+    )
+    print(
+        "         Author : " + Fore.CYAN + Style.BRIGHT + __AUTHOR__ + Style.RESET_ALL
+    )
+    print(
+        "         Contact: " + Fore.BLUE + Style.BRIGHT + __CONTACT__ + Style.RESET_ALL
+    )
+    print(
+        "         At     : "
+        + Fore.LIGHTGREEN_EX
+        + Style.BRIGHT
+        + __DATE__
+        + Style.RESET_ALL
+    )
+    print(
+        "         Loc    : "
+        + Fore.LIGHTMAGENTA_EX
+        + Style.BRIGHT
+        + __LOC__
+        + Style.RESET_ALL
+    )
+    print(
+        "         Star   : " + Fore.MAGENTA + Style.BRIGHT + __git__ + Style.RESET_ALL
+    )
+    print(
+        "         Ver.   : " + Fore.GREEN + Style.BRIGHT + __VERSION__ + Style.RESET_ALL
+    )
+    print("-" * 70)
+    print("\n")
 
 
 def main(args=None):
     args = arg_parse()
     if args.version:
         print(print_welcome_msg())
         exit(0)
     else:
         args_dict = vars(args)
         print_welcome_msg()
         try:
-            module = args_dict['which'].split('-')[0]
-            action = args_dict['which'].split('-')[1]
+            module = args_dict["which"].split("-")[0]
+            action = args_dict["which"].split("-")[1]
             print(Fore.GREEN + Style.BRIGHT)
-            print('=> Module: ' + Fore.WHITE + Style.BRIGHT +
-                  module + Fore.GREEN + Style.BRIGHT)
-            print('=> Action: ' + Fore.WHITE + Style.BRIGHT + action)
-            if module == 'vision':
-                if action == 'extract':
-                    v_f = args_dict['video']
-                    j = args_dict['jumps']
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Extracting from {}'.format(v_f))
+            print(
+                "=> Module: "
+                + Fore.WHITE
+                + Style.BRIGHT
+                + module
+                + Fore.GREEN
+                + Style.BRIGHT
+            )
+            print("=> Action: " + Fore.WHITE + Style.BRIGHT + action)
+            if module == "vision":
+                if action == "extract":
+                    v_f = args_dict["video"]
+                    j = args_dict["jumps"]
+                    print(Fore.BLUE + Style.BRIGHT + "Extracting from {}".format(v_f))
                     video_extractor = VideoExtractor(jump_frames=j)
                     video_extractor.extract(v_f)
-                elif action == 'reduce':
-                    v_f = args_dict['video']
-                    j = args_dict['jumps']
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Reduce from {}, jumps: {}'.format(v_f, j))
+                elif action == "reduce":
+                    v_f = args_dict["video"]
+                    j = args_dict["jumps"]
+                    print(
+                        Fore.BLUE
+                        + Style.BRIGHT
+                        + "Reduce from {}, jumps: {}".format(v_f, j)
+                    )
                     video_reducer = VideoReducer(jump_frames=j)
                     video_reducer.act(v_f)
-                elif action == '2video':
-                    d = args_dict['dir']
+                elif action == "2video":
+                    d = args_dict["dir"]
                     combiner = VideoCombiner(img_dir=d)
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Combine video from {}'.format(d))
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'What the hell.. {}'.format(d))
+                    print(Fore.BLUE + Style.BRIGHT + "Combine video from {}".format(d))
+                    print(Fore.BLUE + Style.BRIGHT + "What the hell.. {}".format(d))
                     combiner.combine()
 
-                elif action == 'clean':
-                    d = args_dict['dir']
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Cleaning from {}'.format(d))
+                elif action == "clean":
+                    d = args_dict["dir"]
+                    print(Fore.BLUE + Style.BRIGHT + "Cleaning from {}".format(d))
 
-                elif action == 'getface':
+                elif action == "getface":
                     try:
                         from .modules.vision.face_extractor import FaceExtractor
                         import dlib
 
-                        d = args_dict['dir']
-                        print(Fore.BLUE + Style.BRIGHT +
-                              'Extract faces from {}'.format(d))
+                        d = args_dict["dir"]
+                        print(
+                            Fore.BLUE + Style.BRIGHT + "Extract faces from {}".format(d)
+                        )
 
                         face_extractor = FaceExtractor()
                         face_extractor.get_faces(d)
                     except ImportError:
                         print(
-                            'This action needs to install dlib first. http://dlib.net')
+                            "This action needs to install dlib first. http://dlib.net"
+                        )
 
-            elif module == 'text':
-                if action == 'clean':
-                    f = args_dict['file']
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Cleaning from {}'.format(f))
-                elif action == 'translate':
+            elif module == "text":
+                if action == "clean":
+                    f = args_dict["file"]
+                    print(Fore.BLUE + Style.BRIGHT + "Cleaning from {}".format(f))
+                elif action == "translate":
                     f = args.v
-                    print(Fore.BLUE + Style.BRIGHT +
-                          'Translate from {}'.format(f))
-            elif module == 'scrap':
-                if action == 'image':
-                    q = args_dict['query']
-                    q_list = q.split(',')
-                    q_list = [i.replace(' ', '') for i in q_list]
+                    print(Fore.BLUE + Style.BRIGHT + "Translate from {}".format(f))
+            elif module == "scrap":
+                if action == "image":
+                    q = args_dict["query"]
+                    q_list = q.split(",")
+                    q_list = [i.replace(" ", "") for i in q_list]
                     image_scraper = ImageScraper()
                     image_scraper.scrap(q_list)
-            elif module == 'cab':
-                if action == 'count':
-                    d = args_dict['dir']
-                    t = args_dict['type']
-                    logging.info('dir: {}, types: {}'.format(d, t))
+            elif module == "cab":
+                if action == "count":
+                    d = args_dict["dir"]
+                    t = args_dict["type"]
+                    logging.info("dir: {}, types: {}".format(d, t))
                     count_file(d, t)
-                elif action == 'split':
-                    f = args_dict['file']
-                    r = args_dict['ratios']
-                    n = args_dict['names']
-                    logging.info(
-                        'files: {}, ratios: {}, names: {}'.format(f, r, n))
+                elif action == "split":
+                    f = args_dict["file"]
+                    r = args_dict["ratios"]
+                    n = args_dict["names"]
+                    logging.info("files: {}, ratios: {}, names: {}".format(f, r, n))
                     split_txt_file(f, r, n)
-                elif action == 'stackimgs':
-                    f = args_dict['imgs']
-                    r = args_dict['dim']
-                    logging.info('files: {}, dim: {}'.format(f, r))
+                elif action == "stackimgs":
+                    f = args_dict["imgs"]
+                    r = args_dict["dim"]
+                    logging.info("files: {}, dim: {}".format(f, r))
                     stack_imgs(f, r)
-                elif action == 'license':
-                    owner = args_dict['owner']
-                    project_name = args_dict['name']
-                    year = args_dict['year']
-                    url = args_dict['url']
-                    d = args_dict['dir']
+                elif action == "license":
+                    owner = args_dict["owner"]
+                    project_name = args_dict["name"]
+                    year = args_dict["year"]
+                    url = args_dict["url"]
+                    d = args_dict["dir"]
                     apply_license(owner, project_name, year, url, d)
-                elif action == 'webcam':
-                    f = args_dict['file']
+                elif action == "webcam":
+                    f = args_dict["file"]
                     webcam_test(f)
-                elif action == 'downmd':
-                    f = args_dict['file']
+                elif action == "downmd":
+                    f = args_dict["file"]
                     download_images_from_md(f)
-                elif action == 'changesource':
+                elif action == "changesource":
                     change_pypi_source()
-                elif action == 'gtrend':
-                    lan = args_dict['language']
-                    layout = args_dict['layout']
+                elif action == "gtrend":
+                    lan = args_dict["language"]
+                    layout = args_dict["layout"]
                     get_github_trending(lang=lan, layout=layout)
-            elif module == 'dltool':
-                if action == 'anchor':
-                    ann_dir = args_dict['annotation_dir']
-                    n = args_dict['cluster_num']
-                    form = args_dict['format']
+            elif module == "dltool":
+                if action == "anchor":
+                    ann_dir = args_dict["annotation_dir"]
+                    n = args_dict["cluster_num"]
+                    form = args_dict["format"]
                     kmeans = KmeansYolo(ann_dir, n, form)
                     kmeans.txt2clusters()
                 else:
-                    ValueError('unsupported action: {}'.format(action))
-            elif module == 'data':
-                if action == 'vocview':
-                    image_dir = args_dict['image_dir']
-                    label_dir = args_dict['label_dir']
+                    ValueError("unsupported action: {}".format(action))
+            elif module == "data":
+                if action == "vocview":
+                    image_dir = args_dict["image_dir"]
+                    label_dir = args_dict["label_dir"]
                     vis_voc(img_root=image_dir, label_root=label_dir)
-                elif action == 'cocoview':
-                    img_d = args_dict['image_dir']
-                    json_f = args_dict['json']
+                elif action == "cocoview":
+                    img_d = args_dict["image_dir"]
+                    json_f = args_dict["json"]
                     vis_coco(img_d, json_f)
-                elif action == 'txtview':
-                    image_dir = args_dict['image_dir']
-                    label_dir = args_dict['label_dir']
+                elif action == "txtview":
+                    image_dir = args_dict["image_dir"]
+                    label_dir = args_dict["label_dir"]
                     vis_det_txt(img_root=image_dir, label_root=label_dir)
-                elif action == 'yoloview':
-                    image_dir = args_dict['image_dir']
-                    label_dir = args_dict['label_dir']
+                elif action == "yoloview":
+                    image_dir = args_dict["image_dir"]
+                    label_dir = args_dict["label_dir"]
                     vis_det_yolo(img_root=image_dir, label_root=label_dir)
-                elif action == 'voclabel':
-                    anno_dir = args_dict['anno_dir']
+                elif action == "voclabel":
+                    anno_dir = args_dict["anno_dir"]
                     gather_labels(anno_dir)
-                elif action == 'splitvoc':
-                    logging.info(
-                        'split VOC to train and val not implement yet.')
+                elif action == "splitvoc":
+                    logging.info("split VOC to train and val not implement yet.")
                     pass
-                elif action == 'splitcoco':
-                    json_f = args_dict['json_file']
-                    s = args_dict['split']
+                elif action == "splitcoco":
+                    json_f = args_dict["json_file"]
+                    s = args_dict["split"]
                     split_coco(ann_f=json_f, split=s)
-                elif action == 'labelone2voc':
-                    logging.info('labelone2voc not implement yet.')
+                elif action == "labelone2voc":
+                    logging.info("labelone2voc not implement yet.")
                     pass
-                elif action == 'voc2coco':
-                    logging.info('start convert VOC to coco... Annotations root: {}'.format(
-                        args_dict['xml_dir']))
+                elif action == "voc2coco":
+                    logging.info(
+                        "start convert VOC to coco... Annotations root: {}".format(
+                            args_dict["xml_dir"]
+                        )
+                    )
                     convert(
-                        args_dict['xml_dir'], args_dict['img_dir'], index_1=args_dict['index_1'])
-                elif action == 'coco2yolo':
-                    logging.info('start convert COCO to yolo... images root: {}, json file: {}'.format(
-                        args_dict['image_dir'], args_dict['json_file']))
-                    coco2yolo(args_dict['image_dir'], args_dict['json_file'])
-                elif action == 'yolo2voc':
-                    logging.info('start convert yolo to VOC... images root: {}, text root: {}'.format(
-                        args_dict['image_dir'], args_dict['text_dir']))
+                        args_dict["xml_dir"],
+                        args_dict["img_dir"],
+                        index_1=args_dict["index_1"],
+                    )
+                elif action == "coco2yolo":
+                    logging.info(
+                        "start convert COCO to yolo... images root: {}, json file: {}".format(
+                            args_dict["image_dir"], args_dict["json_file"]
+                        )
+                    )
+                    coco2yolo(args_dict["image_dir"], args_dict["json_file"])
+                elif action == "yolo2voc":
+                    logging.info(
+                        "start convert yolo to VOC... images root: {}, text root: {}".format(
+                            args_dict["image_dir"], args_dict["text_dir"]
+                        )
+                    )
                     yolo2voc(
-                        args_dict['image_dir'], args_dict['text_dir'], args_dict['class_file'])
-                elif action == 'voc2yolo':
-                    logging.info('start convert VOC to yolo... images root: {}, text root: {}'.format(
-                        args_dict['image_dir'], args_dict['xml_dir']))
+                        args_dict["image_dir"],
+                        args_dict["text_dir"],
+                        args_dict["class_file"],
+                    )
+                elif action == "voc2yolo":
+                    logging.info(
+                        "start convert VOC to yolo... images root: {}, text root: {}".format(
+                            args_dict["image_dir"], args_dict["xml_dir"]
+                        )
+                    )
                     voc2yolo(
-                        args_dict['image_dir'], args_dict['xml_dir'], args_dict['class_file'])
-                elif action == 'evalvoc':
-                    logging.info('start eval on VOC dataset..')
+                        args_dict["image_dir"],
+                        args_dict["xml_dir"],
+                        args_dict["class_file"],
+                    )
+                elif action == "evalvoc":
+                    logging.info("start eval on VOC dataset..")
                     eval_voc(args)
-                elif action == 'mergevoc':
-                    logging.info('start merge VOC dataset..')
-                    merge_list = args_dict['dirs']
+                elif action == "mergevoc":
+                    logging.info("start merge VOC dataset..")
+                    merge_list = args_dict["dirs"]
                     merge_voc(merge_list)
 
         except Exception as e:
             traceback.print_exc()
-            print(Fore.RED, 'parse args error, type -h to see help. msg: {}'.format(e))
+            print(Fore.RED, "parse args error, type -h to see help. msg: {}".format(e))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `alfred-py-3.0.6/alfred/deploy/tensorrt/calibrator.py` & `alfred-py-3.0.7/alfred/deploy/tensorrt/calibrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,51 +18,49 @@
 import tensorrt as trt
 import numpy as np
 import ctypes
 
 try:
     import pycuda.driver as cuda
 except ImportError as e:
-    print('pycuda not installed, calibrator will be disabled.')
-
+    print("pycuda not installed, calibrator will be disabled.")
 
 
 class Calibrator(trt.IInt8EntropyCalibrator2):
-    '''calibrator
-        IInt8EntropyCalibrator2
-        IInt8LegacyCalibrator
-        IInt8EntropyCalibrator
-        IInt8MinMaxCalibrator
+    """calibrator
+    IInt8EntropyCalibrator2
+    IInt8LegacyCalibrator
+    IInt8EntropyCalibrator
+    IInt8MinMaxCalibrator
+
+    """
 
-    '''
     def __init__(self, stream, cache_file=""):
-        trt.IInt8EntropyCalibrator2.__init__(self)       
+        trt.IInt8EntropyCalibrator2.__init__(self)
         self.stream = stream
         self.d_input = cuda.mem_alloc(self.stream.calibration_data.nbytes)
         self.cache_file = cache_file
         # print(self.cache_file)
         stream.reset()
-        
 
     def get_batch_size(self):
         return self.stream.batch_size
 
     def get_batch(self, names):
-
         batch = self.stream.next_batch()
-        if not batch.size:  
+        if not batch.size:
             return None
 
         cuda.memcpy_htod(self.d_input, batch)
         return [int(self.d_input)]
 
     def read_calibration_cache(self):
         # If there is a cache, use it instead of calibrating again. Otherwise, implicitly return None.
         if os.path.exists(self.cache_file):
             with open(self.cache_file, "rb") as f:
                 print(f"[INFO] Using calibration cache to save time: {self.cache_file}")
                 return f.read()
 
-    def write_calibration_cache(self, cache): 
+    def write_calibration_cache(self, cache):
         with open(self.cache_file, "wb") as f:
             print(f"[INFO] Caching calibration data for future use: {self.cache_file}")
             f.write(cache)
```

### Comparing `alfred-py-3.0.6/alfred/deploy/tensorrt/common.py` & `alfred-py-3.0.7/alfred/deploy/tensorrt/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 import time
 import os
 import os.path as osp
 import ctypes
 
 try:
     import pycuda.driver as cuda
+
     # https://documen.tician.de/pycuda/driver.html
     import pycuda.autoinit
 except ImportError as e:
     print(
-        f'pycuda not installed, or import failed. inference on trt will be disabled. error: {e}')
+        f"pycuda not installed, or import failed. inference on trt will be disabled. error: {e}"
+    )
 
 TRT8 = 8
 TRT7 = 7
 
 TRT_LOGGER = trt.Logger(trt.Logger.INFO)
 # TRT_LOGGER = trt.Logger()
 trt.init_libnvinfer_plugins(TRT_LOGGER, namespace="")
@@ -79,16 +81,17 @@
 
 def allocate_buffers_v2(engine):
     inputs = []
     outputs = []
     bindings = []
     stream = cuda.Stream()
     for binding in engine:
-        size = abs(trt.volume(engine.get_binding_shape(binding))) * \
-            engine.max_batch_size
+        size = (
+            abs(trt.volume(engine.get_binding_shape(binding))) * engine.max_batch_size
+        )
         dtype = trt.nptype(engine.get_binding_dtype(binding))
         # Allocate host and device buffers
         host_mem = cuda.pagelocked_empty(size, dtype)
         device_mem = cuda.mem_alloc(host_mem.nbytes)
         # Append the device buffer to device bindings.
         bindings.append(int(device_mem))
         # Append to the appropriate list.
@@ -192,23 +195,21 @@
     FP16=False,
     verbose=False,
     dynamic_input=False,
     batch_size=1,
     chw_shape=None,
 ):
     def get_engine():
-        EXPLICIT_BATCH = 1 << (int)(
-            trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
+        EXPLICIT_BATCH = 1 << (int)(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
         # with trt.Builder(TRT_LOGGER) as builder, builder.create_network(EXPLICIT_BATCH) as network,builder.create_builder_config() as config, trt.OnnxParser(network,TRT_LOGGER) as parser:
         with trt.Builder(TRT_LOGGER) as builder, builder.create_network(
             EXPLICIT_BATCH
         ) as network, builder.create_builder_config() as config, trt.OnnxParser(
             network, TRT_LOGGER
         ) as parser:
-
             trt_version = int(trt.__version__[0])
             # Workspace size is the maximum amount of memory available to the builder while building an engine.
 
             if trt_version == TRT8:
                 config.max_workspace_size = 6 << 30  # 2GB
             else:
                 builder.max_workspace_size = 6 << 30  # 2GB
@@ -229,16 +230,15 @@
             # network.get_input(0).shape = [batch_size, 3, 800, 800]
             if chw_shape:
                 network.get_input(0).shape = [batch_size, *chw_shape]
 
             if dynamic_input:
                 profile = builder.create_optimization_profile()
                 profile.set_shape(
-                    "inputs", (1, 3, 800, 800), (8, 3,
-                                                 800, 800), (64, 3, 800, 800)
+                    "inputs", (1, 3, 800, 800), (8, 3, 800, 800), (64, 3, 800, 800)
                 )
                 config.add_optimization_profile(profile)
 
             # builder engine
             engine = None
             if trt_version == TRT8:
                 engine = builder.build_engine(network, config)
@@ -279,21 +279,19 @@
     def build_engine(max_batch_size, save_engine, opt_params=None):
         """Takes an ONNX file and creates a TensorRT engine to run inference with"""
         with trt.Builder(TRT_LOGGER) as builder, builder.create_network(
             1
         ) as network, builder.create_builder_config() as config, trt.OnnxParser(
             network, TRT_LOGGER
         ) as parser, builder.create_builder_config() as trt_config:
-
             trt_version = int(trt.__version__[0])
             # parse onnx model file
             if not os.path.exists(onnx_file_path):
                 quit(f"[Error]ONNX file {onnx_file_path} not found")
-            logger.info(
-                f"[INFO] Loading ONNX file from path {onnx_file_path}...")
+            logger.info(f"[INFO] Loading ONNX file from path {onnx_file_path}...")
             with open(onnx_file_path, "rb") as model:
                 logger.info("[INFO] Beginning ONNX file parsing")
                 parser.parse(model.read())
                 assert (
                     network.num_layers > 0
                 ), "[Error] Failed to parse ONNX model. \
                             Please check if the ONNX model is compatible "
@@ -312,15 +310,15 @@
                     'input': [
                         [1, 3, 416, 502], # min shape
                         [1, 3, 416, 502], # opt shape
                         [1, 3, 416, 502], # max shape
                     ]
                 }
                 """
-                logger.info('using opt_params: {}'.format(opt_params))
+                logger.info("using opt_params: {}".format(opt_params))
                 for input_index, input_tensor_name in enumerate(opt_params.keys()):
                     min_shape = tuple(opt_params[input_tensor_name][0][:])
                     opt_shape = tuple(opt_params[input_tensor_name][1][:])
                     max_shape = tuple(opt_params[input_tensor_name][2][:])
                     profile.set_shape(
                         input_tensor_name, min_shape, opt_shape, max_shape
                     )
@@ -333,24 +331,24 @@
                 trt_config.max_workspace_size = 2 << 30  # 2GB
             else:
                 builder.max_workspace_size = 2 << 30  # 2GB
 
             if trt_version == TRT8:
                 if fp16_mode:
                     trt_config.set_flag(trt.BuilderFlag.FP16)
-                    logger.info('enabled fp16 mode.')
+                    logger.info("enabled fp16 mode.")
             else:
                 if fp16_mode:
                     builder.fp16_mode = fp16_mode
-                    logger.info('enabled fp16 mode.')
+                    logger.info("enabled fp16 mode.")
 
             if int8_mode:
                 if trt_version == TRT8:
                     trt_config.set_flag(trt.BuilderFlag.INT8)
-                    logger.info('enabled int8 mode.')
+                    logger.info("enabled int8 mode.")
                 else:
                     builder.fp16_mode = fp16_mode
 
                 assert (
                     calibration_stream
                 ), "[Error] a calibration_stream should be provided for int8 mode"
                 config.int8_calibrator = Calibrator(
@@ -394,18 +392,17 @@
         exit(1)
 
 
 def load_torchtrt_plugins():
     # ctypes.CDLL(osp.join(dir_path, 'libamirstan_plugin.so'))
     # suppose plugins lib installed into HOME
     lib_path = osp.join(
-        osp.expanduser(
-            "~"), "torchtrt_plugins/build/lib/libtorchtrt_plugins.so"
+        osp.expanduser("~"), "torchtrt_plugins/build/lib/libtorchtrt_plugins.so"
     )
-    lib_path2 = '/usr/local/lib/libtorchtrt_plugins.so'
+    lib_path2 = "/usr/local/lib/libtorchtrt_plugins.so"
     if os.path.exists(lib_path):
         ctypes.CDLL(lib_path)
     elif os.path.exists(lib_path2):
         ctypes.CDLL(lib_path2)
     else:
         logger.warning(f"{lib_path} not found.")
 
@@ -431,15 +428,14 @@
     def build_engine(max_batch_size, save_engine):
         """Takes an ONNX file and creates a TensorRT engine to run inference with"""
         with trt.Builder(TRT_LOGGER) as builder, builder.create_network(
             1
         ) as network, builder.create_builder_config() as config, trt.OnnxParser(
             network, TRT_LOGGER
         ) as parser, builder.create_builder_config() as trt_config:
-
             trt_version = int(trt.__version__[0])
             # parse onnx model file
             if not os.path.exists(onnx_file_path):
                 quit(f"[Error]ONNX file {onnx_file_path} not found")
             logger.info(f"Loading ONNX file from path {onnx_file_path}...")
             with open(onnx_file_path, "rb") as model:
                 logger.info("Beginning ONNX file parsing")
```

### Comparing `alfred-py-3.0.6/alfred/deploy/tensorrt/process.py` & `alfred-py-3.0.7/alfred/deploy/tensorrt/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,64 +20,67 @@
 
 import pycuda.driver as cuda
 import pycuda.autoinit
 
 try:
     import cupy as cp
 except ImportError:
-    print('You should install cupy for preprocess with CUDA: https://docs.cupy.dev/en/stable/install.html')
+    print(
+        "You should install cupy for preprocess with CUDA: https://docs.cupy.dev/en/stable/install.html"
+    )
 # from cupy.core.dlpack import toDlpack
 # from cupy.core.dlpack import fromDlpack
 from torch.utils.dlpack import to_dlpack
 from torch.utils.dlpack import from_dlpack
 from alfred.dl.torch.common import device
 
 
 def preprocess_np(img_path):
-    '''process use numpy
-    '''
+    """process use numpy"""
     im = Image.open(img_path)
     img = im.resize((800, 800), Image.BILINEAR)
     img = np.array(img).astype(np.float32) / 255.0
     img = img.transpose(2, 0, 1)
     # print(img.shape)
-    img = (img - np.array([[[0.485]], [[0.456]], [[0.406]]])
-           )/np.array([[[0.229]], [[0.224]], [[0.225]]])
+    img = (img - np.array([[[0.485]], [[0.456]], [[0.406]]])) / np.array(
+        [[[0.229]], [[0.224]], [[0.225]]]
+    )
 
     # img = img.transpose(1,2,0)
     img = np.expand_dims(img, axis=0)
     img = np.ascontiguousarray(img)
     img = np.array(img).astype(np.float32)
 
     return img, im, im.size
 
 
 class PyTorchTensorHolder(pycuda.driver.PointerHolderBase):
-    '''代码来源:
-        https://github.com/NVIDIA/trt-samples-for-hackathon-cn/blob/master/python/app_onnx_resnet50.py
-    '''
+    """代码来源:
+    https://github.com/NVIDIA/trt-samples-for-hackathon-cn/blob/master/python/app_onnx_resnet50.py
+    """
 
     def __init__(self, tensor):
         super(PyTorchTensorHolder, self).__init__()
         self.tensor = tensor
 
     def get_pointer(self):
         return self.tensor.data_ptr()
 
 
-transform = T.Compose([
-    T.Resize((800, 800)),  # PIL.Image.BILINEAR
-    T.ToTensor(),
-    # T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
-])
+transform = T.Compose(
+    [
+        T.Resize((800, 800)),  # PIL.Image.BILINEAR
+        T.ToTensor(),
+        # T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
+    ]
+)
 
 
 def preprocess_torch(img_path):
-    '''process use torchvision
-    '''
+    """process use torchvision"""
     im = Image.open(img_path)
     img = transform(im).unsqueeze(0)
     img = PyTorchTensorHolder(img)
     return img, im, im.size
 
 
 def preprocess_torch_v1(img_path):
```

### Comparing `alfred-py-3.0.6/alfred/deploy/tensorrt/wrapper.py` & `alfred-py-3.0.7/alfred/deploy/tensorrt/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,252 +1,248 @@
-00000000: 0d0a 6672 6f6d 2061 6c66 7265 642e 6465  ..from alfred.de
-00000010: 706c 6f79 2e74 656e 736f 7272 742e 636f  ploy.tensorrt.co
-00000020: 6d6d 6f6e 2069 6d70 6f72 7420 280d 0a20  mmon import (.. 
-00000030: 2020 2064 6f5f 696e 6665 7265 6e63 655f     do_inference_
-00000040: 7632 2c0d 0a20 2020 2062 7569 6c64 5f65  v2,..    build_e
-00000050: 6e67 696e 655f 6f6e 6e78 5f76 322c 0d0a  ngine_onnx_v2,..
-00000060: 2020 2020 616c 6c6f 6361 7465 5f62 7566      allocate_buf
-00000070: 6665 7273 5f76 325f 6479 6e61 6d69 632c  fers_v2_dynamic,
-00000080: 0d0a 2020 2020 616c 6c6f 6361 7465 5f62  ..    allocate_b
-00000090: 7566 6665 7273 5f76 322c 0d0a 2020 2020  uffers_v2,..    
-000000a0: 6c6f 6164 5f65 6e67 696e 655f 6672 6f6d  load_engine_from
-000000b0: 5f6c 6f63 616c 2c0d 0a20 2020 206c 6f61  _local,..    loa
-000000c0: 645f 746f 7263 6874 7274 5f70 6c75 6769  d_torchtrt_plugi
-000000d0: 6e73 2c0d 0a20 2020 2063 6865 636b 5f65  ns,..    check_e
-000000e0: 6e67 696e 652c 0d0a 290d 0a69 6d70 6f72  ngine,..)..impor
-000000f0: 7420 6e75 6d70 7920 6173 206e 700d 0a66  t numpy as np..f
-00000100: 726f 6d20 616c 6672 6564 2e75 7469 6c73  rom alfred.utils
-00000110: 2e6c 6f67 2069 6d70 6f72 7420 6c6f 6767  .log import logg
-00000120: 6572 0d0a 696d 706f 7274 2074 696d 650d  er..import time.
-00000130: 0a69 6d70 6f72 7420 7079 6375 6461 2e64  .import pycuda.d
-00000140: 7269 7665 7220 6173 2063 7564 610d 0a0d  river as cuda...
-00000150: 0a0d 0a63 6c61 7373 2054 656e 736f 7252  ...class TensorR
-00000160: 5449 6e66 6572 656e 6365 723a 0d0a 2020  TInferencer:..  
-00000170: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000180: 656c 662c 2065 6e67 696e 655f 662c 2064  elf, engine_f, d
-00000190: 6576 6963 655f 6964 3d30 2c20 6375 6461  evice_id=0, cuda
-000001a0: 5f63 7478 3d4e 6f6e 652c 2074 696d 696e  _ctx=None, timin
-000001b0: 673d 4661 6c73 6529 202d 3e20 4e6f 6e65  g=False) -> None
-000001c0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-000001d0: 656e 6769 6e65 5f66 203d 2065 6e67 696e  engine_f = engin
-000001e0: 655f 660d 0a20 2020 2020 2020 2073 656c  e_f..        sel
-000001f0: 662e 6465 7669 6365 5f69 6420 3d20 6465  f.device_id = de
-00000200: 7669 6365 5f69 640d 0a20 2020 2020 2020  vice_id..       
-00000210: 2073 656c 662e 6375 6461 5f63 7478 203d   self.cuda_ctx =
-00000220: 2063 7564 615f 6374 780d 0a20 2020 2020   cuda_ctx..     
-00000230: 2020 2069 6620 7365 6c66 2e63 7564 615f     if self.cuda_
-00000240: 6374 783a 0d0a 2020 2020 2020 2020 2020  ctx:..          
-00000250: 2020 7365 6c66 2e63 7564 615f 6374 782e    self.cuda_ctx.
-00000260: 7075 7368 2829 0d0a 2020 2020 2020 2020  push()..        
-00000270: 7365 6c66 2e74 696d 696e 6720 3d20 7469  self.timing = ti
-00000280: 6d69 6e67 0d0a 2020 2020 2020 2020 7365  ming..        se
-00000290: 6c66 2e5f 696e 6974 5f65 6e67 696e 6528  lf._init_engine(
-000002a0: 290d 0a0d 0a20 2020 2064 6566 205f 696e  )....    def _in
-000002b0: 6974 5f65 6e67 696e 6528 7365 6c66 293a  it_engine(self):
-000002c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-000002d0: 6e67 696e 6520 3d20 6c6f 6164 5f65 6e67  ngine = load_eng
-000002e0: 696e 655f 6672 6f6d 5f6c 6f63 616c 2873  ine_from_local(s
-000002f0: 656c 662e 656e 6769 6e65 5f66 290d 0a20  elf.engine_f).. 
-00000300: 2020 2020 2020 2073 7073 203d 2063 6865         sps = che
-00000310: 636b 5f65 6e67 696e 6528 7365 6c66 2e65  ck_engine(self.e
-00000320: 6e67 696e 6529 0d0a 2020 2020 2020 2020  ngine)..        
-00000330: 7365 6c66 2e69 6e70 7574 5f73 6861 7065  self.input_shape
-00000340: 7320 3d20 5b73 7073 5b69 5d5b 2273 6861  s = [sps[i]["sha
-00000350: 7065 225d 0d0a 2020 2020 2020 2020 2020  pe"]..          
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 2066 6f72 2069 2069 6e20 7370 732e     for i in sps.
-00000380: 6b65 7973 2829 2069 6620 7370 735b 695d  keys() if sps[i]
-00000390: 5b22 6973 5f69 6e70 7574 225d 5d0d 0a20  ["is_input"]].. 
-000003a0: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
-000003b0: 7574 5f73 6861 7065 7320 3d20 5b0d 0a20  ut_shapes = [.. 
-000003c0: 2020 2020 2020 2020 2020 2073 7073 5b69             sps[i
-000003d0: 5d5b 2273 6861 7065 225d 2066 6f72 2069  ]["shape"] for i
-000003e0: 2069 6e20 7370 732e 6b65 7973 2829 2069   in sps.keys() i
-000003f0: 6620 6e6f 7420 7370 735b 695d 5b22 6973  f not sps[i]["is
-00000400: 5f69 6e70 7574 225d 0d0a 2020 2020 2020  _input"]..      
-00000410: 2020 5d0d 0a20 2020 2020 2020 2073 656c    ]..        sel
-00000420: 662e 6f72 695f 696e 7075 745f 7368 6170  f.ori_input_shap
-00000430: 6520 3d20 7365 6c66 2e65 6e67 696e 652e  e = self.engine.
-00000440: 6765 745f 6269 6e64 696e 675f 7368 6170  get_binding_shap
-00000450: 6528 3029 0d0a 2020 2020 2020 2020 7365  e(0)..        se
-00000460: 6c66 2e69 735f 6479 6e61 6d69 635f 6261  lf.is_dynamic_ba
-00000470: 7463 6820 3d20 7365 6c66 2e6f 7269 5f69  tch = self.ori_i
-00000480: 6e70 7574 5f73 6861 7065 5b30 5d20 3d3d  nput_shape[0] ==
-00000490: 202d 310d 0a20 2020 2020 2020 2073 656c   -1..        sel
-000004a0: 662e 6973 5f64 796e 616d 6963 5f73 6861  f.is_dynamic_sha
-000004b0: 7065 203d 2073 656c 662e 6f72 695f 696e  pe = self.ori_in
-000004c0: 7075 745f 7368 6170 655b 2d31 5d20 3d3d  put_shape[-1] ==
-000004d0: 202d 310d 0a20 2020 2020 2020 2069 6620   -1..        if 
-000004e0: 7365 6c66 2e69 735f 6479 6e61 6d69 635f  self.is_dynamic_
-000004f0: 6261 7463 683a 0d0a 2020 2020 2020 2020  batch:..        
-00000500: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00000510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000520: 2020 6622 656e 6769 6e65 2069 7320 6479    f"engine is dy
-00000530: 6e61 6d69 6320 6f6e 2062 6174 6368 2e20  namic on batch. 
-00000540: 656e 6769 6e65 206d 6178 5f62 6174 6368  engine max_batch
-00000550: 7369 7a65 3a20 7b73 656c 662e 656e 6769  size: {self.engi
-00000560: 6e65 2e6d 6178 5f62 6174 6368 5f73 697a  ne.max_batch_siz
-00000570: 657d 220d 0a20 2020 2020 2020 2020 2020  e}"..           
-00000580: 2029 0d0a 2020 2020 2020 2020 6966 2073   )..        if s
-00000590: 656c 662e 6973 5f64 796e 616d 6963 5f73  elf.is_dynamic_s
-000005a0: 6861 7065 3a0d 0a20 2020 2020 2020 2020  hape:..         
-000005b0: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-000005c0: 656e 6769 6e65 2069 7320 6479 6e61 6d69  engine is dynami
-000005d0: 6320 6f6e 2073 6861 7065 2e22 290d 0a0d  c on shape.")...
-000005e0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-000005f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000600: 636f 6e74 6578 7420 3d20 7365 6c66 2e65  context = self.e
-00000610: 6e67 696e 652e 6372 6561 7465 5f65 7865  ngine.create_exe
-00000620: 6375 7469 6f6e 5f63 6f6e 7465 7874 2829  cution_context()
-00000630: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000640: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
-00000650: 5f73 6861 7065 3a0d 0a20 2020 2020 2020  _shape:..       
-00000660: 2020 2020 2020 2020 2028 0d0a 2020 2020           (..    
+00000000: 6672 6f6d 2061 6c66 7265 642e 6465 706c  from alfred.depl
+00000010: 6f79 2e74 656e 736f 7272 742e 636f 6d6d  oy.tensorrt.comm
+00000020: 6f6e 2069 6d70 6f72 7420 280d 0a20 2020  on import (..   
+00000030: 2064 6f5f 696e 6665 7265 6e63 655f 7632   do_inference_v2
+00000040: 2c0d 0a20 2020 2062 7569 6c64 5f65 6e67  ,..    build_eng
+00000050: 696e 655f 6f6e 6e78 5f76 322c 0d0a 2020  ine_onnx_v2,..  
+00000060: 2020 616c 6c6f 6361 7465 5f62 7566 6665    allocate_buffe
+00000070: 7273 5f76 325f 6479 6e61 6d69 632c 0d0a  rs_v2_dynamic,..
+00000080: 2020 2020 616c 6c6f 6361 7465 5f62 7566      allocate_buf
+00000090: 6665 7273 5f76 322c 0d0a 2020 2020 6c6f  fers_v2,..    lo
+000000a0: 6164 5f65 6e67 696e 655f 6672 6f6d 5f6c  ad_engine_from_l
+000000b0: 6f63 616c 2c0d 0a20 2020 206c 6f61 645f  ocal,..    load_
+000000c0: 746f 7263 6874 7274 5f70 6c75 6769 6e73  torchtrt_plugins
+000000d0: 2c0d 0a20 2020 2063 6865 636b 5f65 6e67  ,..    check_eng
+000000e0: 696e 652c 0d0a 290d 0a69 6d70 6f72 7420  ine,..)..import 
+000000f0: 6e75 6d70 7920 6173 206e 700d 0a66 726f  numpy as np..fro
+00000100: 6d20 616c 6672 6564 2e75 7469 6c73 2e6c  m alfred.utils.l
+00000110: 6f67 2069 6d70 6f72 7420 6c6f 6767 6572  og import logger
+00000120: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
+00000130: 6d70 6f72 7420 7079 6375 6461 2e64 7269  mport pycuda.dri
+00000140: 7665 7220 6173 2063 7564 610d 0a0d 0a0d  ver as cuda.....
+00000150: 0a63 6c61 7373 2054 656e 736f 7252 5449  .class TensorRTI
+00000160: 6e66 6572 656e 6365 723a 0d0a 2020 2020  nferencer:..    
+00000170: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000180: 662c 2065 6e67 696e 655f 662c 2064 6576  f, engine_f, dev
+00000190: 6963 655f 6964 3d30 2c20 6375 6461 5f63  ice_id=0, cuda_c
+000001a0: 7478 3d4e 6f6e 652c 2074 696d 696e 673d  tx=None, timing=
+000001b0: 4661 6c73 6529 202d 3e20 4e6f 6e65 3a0d  False) -> None:.
+000001c0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+000001d0: 6769 6e65 5f66 203d 2065 6e67 696e 655f  gine_f = engine_
+000001e0: 660d 0a20 2020 2020 2020 2073 656c 662e  f..        self.
+000001f0: 6465 7669 6365 5f69 6420 3d20 6465 7669  device_id = devi
+00000200: 6365 5f69 640d 0a20 2020 2020 2020 2073  ce_id..        s
+00000210: 656c 662e 6375 6461 5f63 7478 203d 2063  elf.cuda_ctx = c
+00000220: 7564 615f 6374 780d 0a20 2020 2020 2020  uda_ctx..       
+00000230: 2069 6620 7365 6c66 2e63 7564 615f 6374   if self.cuda_ct
+00000240: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
+00000250: 7365 6c66 2e63 7564 615f 6374 782e 7075  self.cuda_ctx.pu
+00000260: 7368 2829 0d0a 2020 2020 2020 2020 7365  sh()..        se
+00000270: 6c66 2e74 696d 696e 6720 3d20 7469 6d69  lf.timing = timi
+00000280: 6e67 0d0a 2020 2020 2020 2020 7365 6c66  ng..        self
+00000290: 2e5f 696e 6974 5f65 6e67 696e 6528 290d  ._init_engine().
+000002a0: 0a0d 0a20 2020 2064 6566 205f 696e 6974  ...    def _init
+000002b0: 5f65 6e67 696e 6528 7365 6c66 293a 0d0a  _engine(self):..
+000002c0: 2020 2020 2020 2020 7365 6c66 2e65 6e67          self.eng
+000002d0: 696e 6520 3d20 6c6f 6164 5f65 6e67 696e  ine = load_engin
+000002e0: 655f 6672 6f6d 5f6c 6f63 616c 2873 656c  e_from_local(sel
+000002f0: 662e 656e 6769 6e65 5f66 290d 0a20 2020  f.engine_f)..   
+00000300: 2020 2020 2073 7073 203d 2063 6865 636b       sps = check
+00000310: 5f65 6e67 696e 6528 7365 6c66 2e65 6e67  _engine(self.eng
+00000320: 696e 6529 0d0a 2020 2020 2020 2020 7365  ine)..        se
+00000330: 6c66 2e69 6e70 7574 5f73 6861 7065 7320  lf.input_shapes 
+00000340: 3d20 5b73 7073 5b69 5d5b 2273 6861 7065  = [sps[i]["shape
+00000350: 225d 2066 6f72 2069 2069 6e20 7370 732e  "] for i in sps.
+00000360: 6b65 7973 2829 2069 6620 7370 735b 695d  keys() if sps[i]
+00000370: 5b22 6973 5f69 6e70 7574 225d 5d0d 0a20  ["is_input"]].. 
+00000380: 2020 2020 2020 2073 656c 662e 6f75 7470         self.outp
+00000390: 7574 5f73 6861 7065 7320 3d20 5b0d 0a20  ut_shapes = [.. 
+000003a0: 2020 2020 2020 2020 2020 2073 7073 5b69             sps[i
+000003b0: 5d5b 2273 6861 7065 225d 2066 6f72 2069  ]["shape"] for i
+000003c0: 2069 6e20 7370 732e 6b65 7973 2829 2069   in sps.keys() i
+000003d0: 6620 6e6f 7420 7370 735b 695d 5b22 6973  f not sps[i]["is
+000003e0: 5f69 6e70 7574 225d 0d0a 2020 2020 2020  _input"]..      
+000003f0: 2020 5d0d 0a20 2020 2020 2020 2073 656c    ]..        sel
+00000400: 662e 6f72 695f 696e 7075 745f 7368 6170  f.ori_input_shap
+00000410: 6520 3d20 7365 6c66 2e65 6e67 696e 652e  e = self.engine.
+00000420: 6765 745f 6269 6e64 696e 675f 7368 6170  get_binding_shap
+00000430: 6528 3029 0d0a 2020 2020 2020 2020 7365  e(0)..        se
+00000440: 6c66 2e69 735f 6479 6e61 6d69 635f 6261  lf.is_dynamic_ba
+00000450: 7463 6820 3d20 7365 6c66 2e6f 7269 5f69  tch = self.ori_i
+00000460: 6e70 7574 5f73 6861 7065 5b30 5d20 3d3d  nput_shape[0] ==
+00000470: 202d 310d 0a20 2020 2020 2020 2073 656c   -1..        sel
+00000480: 662e 6973 5f64 796e 616d 6963 5f73 6861  f.is_dynamic_sha
+00000490: 7065 203d 2073 656c 662e 6f72 695f 696e  pe = self.ori_in
+000004a0: 7075 745f 7368 6170 655b 2d31 5d20 3d3d  put_shape[-1] ==
+000004b0: 202d 310d 0a20 2020 2020 2020 2069 6620   -1..        if 
+000004c0: 7365 6c66 2e69 735f 6479 6e61 6d69 635f  self.is_dynamic_
+000004d0: 6261 7463 683a 0d0a 2020 2020 2020 2020  batch:..        
+000004e0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000004f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000500: 2020 6622 656e 6769 6e65 2069 7320 6479    f"engine is dy
+00000510: 6e61 6d69 6320 6f6e 2062 6174 6368 2e20  namic on batch. 
+00000520: 656e 6769 6e65 206d 6178 5f62 6174 6368  engine max_batch
+00000530: 7369 7a65 3a20 7b73 656c 662e 656e 6769  size: {self.engi
+00000540: 6e65 2e6d 6178 5f62 6174 6368 5f73 697a  ne.max_batch_siz
+00000550: 657d 220d 0a20 2020 2020 2020 2020 2020  e}"..           
+00000560: 2029 0d0a 2020 2020 2020 2020 6966 2073   )..        if s
+00000570: 656c 662e 6973 5f64 796e 616d 6963 5f73  elf.is_dynamic_s
+00000580: 6861 7065 3a0d 0a20 2020 2020 2020 2020  hape:..         
+00000590: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
+000005a0: 656e 6769 6e65 2069 7320 6479 6e61 6d69  engine is dynami
+000005b0: 6320 6f6e 2073 6861 7065 2e22 290d 0a0d  c on shape.")...
+000005c0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+000005d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000005e0: 636f 6e74 6578 7420 3d20 7365 6c66 2e65  context = self.e
+000005f0: 6e67 696e 652e 6372 6561 7465 5f65 7865  ngine.create_exe
+00000600: 6375 7469 6f6e 5f63 6f6e 7465 7874 2829  cution_context()
+00000610: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000620: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
+00000630: 5f73 6861 7065 3a0d 0a20 2020 2020 2020  _shape:..       
+00000640: 2020 2020 2020 2020 2028 0d0a 2020 2020           (..    
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 7365 6c66 2e69 6e70 7574 732c 0d0a 2020  self.inputs,..  
 00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 7365 6c66 2e69 6e70 7574 732c 0d0a 2020  self.inputs,..  
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 7365 6c66 2e6f 7574 7075 7473 2c0d    self.outputs,.
-000006b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006c0: 2020 2020 2073 656c 662e 6269 6e64 696e       self.bindin
-000006d0: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
-000006e0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000006f0: 7265 616d 2c0d 0a20 2020 2020 2020 2020  ream,..         
-00000700: 2020 2020 2020 2029 203d 2061 6c6c 6f63         ) = alloc
-00000710: 6174 655f 6275 6666 6572 735f 7632 5f64  ate_buffers_v2_d
-00000720: 796e 616d 6963 2873 656c 662e 656e 6769  ynamic(self.engi
-00000730: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-00000740: 2020 2020 2073 656c 662e 636f 6e74 6578       self.contex
-00000750: 742e 7365 745f 6f70 7469 6d69 7a61 7469  t.set_optimizati
-00000760: 6f6e 5f70 726f 6669 6c65 5f61 7379 6e63  on_profile_async
-00000770: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00000780: 2020 2020 2020 2030 2c20 7365 6c66 2e73         0, self.s
-00000790: 7472 6561 6d2e 6861 6e64 6c65 290d 0a20  tream.handle).. 
-000007a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000007b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007c0: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
-000007d0: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-000007e0: 7075 7473 2c0d 0a20 2020 2020 2020 2020  puts,..         
-000007f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000800: 6f75 7470 7574 732c 0d0a 2020 2020 2020  outputs,..      
-00000810: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000820: 6c66 2e62 696e 6469 6e67 732c 0d0a 2020  lf.bindings,..  
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 7365 6c66 2e73 7472 6561 6d2c 0d0a    self.stream,..
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2920 3d20 616c 6c6f 6361 7465 5f62 7566  ) = allocate_buf
-00000870: 6665 7273 5f76 3228 7365 6c66 2e65 6e67  fers_v2(self.eng
-00000880: 696e 6529 0d0a 2020 2020 2020 2020 2020  ine)..          
-00000890: 2020 7072 696e 7428 2254 5254 2065 6e67    print("TRT eng
-000008a0: 696e 6520 6c6f 6164 6564 2e22 290d 0a20  ine loaded.").. 
-000008b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000008c0: 6c66 2e63 7564 615f 6374 783a 0d0a 2020  lf.cuda_ctx:..  
-000008d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000008e0: 6c66 2e63 7564 615f 6374 782e 706f 7028  lf.cuda_ctx.pop(
-000008f0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-00000900: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00000910: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000920: 656c 662e 6375 6461 5f63 7478 2e70 6f70  elf.cuda_ctx.pop
-00000930: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000940: 6465 6c20 7365 6c66 2e63 7564 615f 6374  del self.cuda_ct
-00000950: 780d 0a20 2020 2020 2020 2020 2020 2072  x..            r
-00000960: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-00000970: 7228 2246 6169 6c20 746f 2061 6c6c 6f63  r("Fail to alloc
-00000980: 6174 6520 4355 4441 2072 6573 6f75 7263  ate CUDA resourc
-00000990: 6573 2229 2066 726f 6d20 650d 0a0d 0a20  es") from e.... 
-000009a0: 2020 2064 6566 2069 6e66 6572 2873 656c     def infer(sel
-000009b0: 662c 2069 6d67 7329 3a0d 0a20 2020 2020  f, imgs):..     
-000009c0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-000009d0: 616e 6365 2869 6d67 732c 206e 702e 6e64  ance(imgs, np.nd
-000009e0: 6172 7261 7929 2c20 2269 6d67 7320 6d75  array), "imgs mu
-000009f0: 7374 2062 6520 6e75 6d70 7920 6172 7261  st be numpy arra
-00000a00: 7922 0d0a 2020 2020 2020 2020 6966 2073  y"..        if s
-00000a10: 656c 662e 6375 6461 5f63 7478 3a0d 0a20  elf.cuda_ctx:.. 
-00000a20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000a30: 6375 6461 5f63 7478 2e70 7573 6828 290d  cuda_ctx.push().
-00000a40: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
-00000a50: 6c66 2e69 735f 6479 6e61 6d69 635f 6261  lf.is_dynamic_ba
-00000a60: 7463 683a 0d0a 2020 2020 2020 2020 2020  tch:..          
-00000a70: 2020 6273 203d 2069 6d67 732e 7368 6170    bs = imgs.shap
-00000a80: 655b 305d 0d0a 2020 2020 2020 2020 2020  e[0]..          
-00000a90: 2020 7365 6c66 2e69 6e70 7574 735b 305d    self.inputs[0]
-00000aa0: 2e68 6f73 7420 3d20 696d 6773 2e72 6176  .host = imgs.rav
-00000ab0: 656c 2829 0d0a 2020 2020 2020 2020 2020  el()..          
-00000ac0: 2020 2320 6d61 6b65 2063 6f6e 7465 7874    # make context
-00000ad0: 2061 7761 7265 2077 6861 7427 7320 6261   aware what's ba
-00000ae0: 7463 6873 697a 6520 6375 7272 656e 740d  tchsize current.
-00000af0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000b00: 662e 6f72 695f 696e 7075 745f 7368 6170  f.ori_input_shap
-00000b10: 655b 305d 203d 2062 730d 0a20 2020 2020  e[0] = bs..     
-00000b20: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00000b30: 6578 742e 7365 745f 6269 6e64 696e 675f  ext.set_binding_
-00000b40: 7368 6170 6528 302c 2028 7365 6c66 2e6f  shape(0, (self.o
-00000b50: 7269 5f69 6e70 7574 5f73 6861 7065 2929  ri_input_shape))
-00000b60: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00000b70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000b80: 662e 696e 7075 7473 5b30 5d2e 686f 7374  f.inputs[0].host
-00000b90: 203d 2069 6d67 732e 7261 7665 6c28 290d   = imgs.ravel().
-00000ba0: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
-00000bb0: 6c66 2e74 696d 696e 673a 0d0a 2020 2020  lf.timing:..    
-00000bc0: 2020 2020 2020 2020 7430 203d 2074 696d          t0 = tim
-00000bd0: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
-00000be0: 0d0a 2020 2020 2020 2020 6f75 7473 203d  ..        outs =
-00000bf0: 2064 6f5f 696e 6665 7265 6e63 655f 7632   do_inference_v2
-00000c00: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00000c10: 656c 662e 636f 6e74 6578 742c 0d0a 2020  elf.context,..  
-00000c20: 2020 2020 2020 2020 2020 6269 6e64 696e            bindin
-00000c30: 6773 3d73 656c 662e 6269 6e64 696e 6773  gs=self.bindings
-00000c40: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-00000c50: 6e70 7574 733d 7365 6c66 2e69 6e70 7574  nputs=self.input
-00000c60: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00000c70: 6f75 7470 7574 733d 7365 6c66 2e6f 7574  outputs=self.out
-00000c80: 7075 7473 2c0d 0a20 2020 2020 2020 2020  puts,..         
-00000c90: 2020 2073 7472 6561 6d3d 7365 6c66 2e73     stream=self.s
-00000ca0: 7472 6561 6d2c 0d0a 2020 2020 2020 2020  tream,..        
-00000cb0: 2020 2020 696e 7075 745f 7465 6e73 6f72      input_tensor
-00000cc0: 3d69 6d67 732c 0d0a 2020 2020 2020 2020  =imgs,..        
-00000cd0: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00000ce0: 6c66 2e63 7564 615f 6374 783a 0d0a 2020  lf.cuda_ctx:..  
-00000cf0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00000d00: 7564 615f 6374 782e 706f 7028 290d 0a20  uda_ctx.pop().. 
-00000d10: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00000d20: 696d 696e 673a 0d0a 2020 2020 2020 2020  iming:..        
-00000d30: 2020 2020 7431 203d 2074 696d 652e 7065      t1 = time.pe
-00000d40: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
-00000d50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00000d60: 6622 656e 6769 6e65 2063 6f73 743a 207b  f"engine cost: {
-00000d70: 7431 202d 2074 307d 2c20 6670 733a 207b  t1 - t0}, fps: {
-00000d80: 312f 2874 312d 7430 297d 2229 0d0a 2020  1/(t1-t0)}")..  
-00000d90: 2020 2020 2020 6f75 7473 5f72 6573 6861        outs_resha
-00000da0: 7065 6420 3d20 5b5d 0d0a 2020 2020 2020  ped = []..      
-00000db0: 2020 666f 7220 692c 206f 2069 6e20 656e    for i, o in en
-00000dc0: 756d 6572 6174 6528 6f75 7473 293a 0d0a  umerate(outs):..
-00000dd0: 2020 2020 2020 2020 2020 2020 6f5f 7320              o_s 
-00000de0: 3d20 7365 6c66 2e6f 7574 7075 745f 7368  = self.output_sh
-00000df0: 6170 6573 5b69 5d0d 0a20 2020 2020 2020  apes[i]..       
-00000e00: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-00000e10: 6479 6e61 6d69 635f 6261 7463 683a 0d0a  dynamic_batch:..
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 6f5f 735b 305d 203d 2073 656c 662e 656e  o_s[0] = self.en
-00000e40: 6769 6e65 2e6d 6178 5f62 6174 6368 5f73  gine.max_batch_s
-00000e50: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
-00000e60: 206f 203d 206e 702e 7265 7368 6170 6528   o = np.reshape(
-00000e70: 6f2c 206f 5f73 290d 0a20 2020 2020 2020  o, o_s)..       
-00000e80: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-00000e90: 6479 6e61 6d69 635f 6261 7463 683a 0d0a  dynamic_batch:..
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 6f75 7473 5f72 6573 6861 7065 642e 6170  outs_reshaped.ap
-00000ec0: 7065 6e64 286f 5b3a 6273 2c20 2e2e 2e5d  pend(o[:bs, ...]
-00000ed0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000ee0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000ef0: 2020 2020 2020 6f75 7473 5f72 6573 6861        outs_resha
-00000f00: 7065 642e 6170 7065 6e64 286f 290d 0a20  ped.append(o).. 
-00000f10: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-00000f20: 7473 5f72 6573 6861 7065 640d 0a0d 0a20  ts_reshaped.... 
-00000f30: 2020 2064 6566 205f 5f64 656c 5f5f 2873     def __del__(s
-00000f40: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00000f50: 2222 4672 6565 2043 5544 4120 6d65 6d6f  ""Free CUDA memo
-00000f60: 7269 6573 2222 220d 0a20 2020 2020 2020  ries"""..       
-00000f70: 2064 656c 2073 656c 662e 6f75 7470 7574   del self.output
-00000f80: 730d 0a20 2020 2020 2020 2064 656c 2073  s..        del s
-00000f90: 656c 662e 696e 7075 7473 0d0a 2020 2020  elf.inputs..    
-00000fa0: 2020 2020 6465 6c20 7365 6c66 2e73 7472      del self.str
-00000fb0: 6561 6d0d 0a                             eam..
+00000680: 2020 7365 6c66 2e6f 7574 7075 7473 2c0d    self.outputs,.
+00000690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006a0: 2020 2020 2073 656c 662e 6269 6e64 696e       self.bindin
+000006b0: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
+000006c0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000006d0: 7265 616d 2c0d 0a20 2020 2020 2020 2020  ream,..         
+000006e0: 2020 2020 2020 2029 203d 2061 6c6c 6f63         ) = alloc
+000006f0: 6174 655f 6275 6666 6572 735f 7632 5f64  ate_buffers_v2_d
+00000700: 796e 616d 6963 2873 656c 662e 656e 6769  ynamic(self.engi
+00000710: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+00000720: 2020 2020 2073 656c 662e 636f 6e74 6578       self.contex
+00000730: 742e 7365 745f 6f70 7469 6d69 7a61 7469  t.set_optimizati
+00000740: 6f6e 5f70 726f 6669 6c65 5f61 7379 6e63  on_profile_async
+00000750: 2830 2c20 7365 6c66 2e73 7472 6561 6d2e  (0, self.stream.
+00000760: 6861 6e64 6c65 290d 0a20 2020 2020 2020  handle)..       
+00000770: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000780: 2020 2020 2020 2020 2020 2020 280d 0a20              (.. 
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 2073 656c 662e 696e 7075 7473 2c0d     self.inputs,.
+000007b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007c0: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
+000007d0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+000007e0: 2020 2020 2020 2020 7365 6c66 2e62 696e          self.bin
+000007f0: 6469 6e67 732c 0d0a 2020 2020 2020 2020  dings,..        
+00000800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000810: 2e73 7472 6561 6d2c 0d0a 2020 2020 2020  .stream,..      
+00000820: 2020 2020 2020 2020 2020 2920 3d20 616c            ) = al
+00000830: 6c6f 6361 7465 5f62 7566 6665 7273 5f76  locate_buffers_v
+00000840: 3228 7365 6c66 2e65 6e67 696e 6529 0d0a  2(self.engine)..
+00000850: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000860: 7428 2254 5254 2065 6e67 696e 6520 6c6f  t("TRT engine lo
+00000870: 6164 6564 2e22 290d 0a20 2020 2020 2020  aded.")..       
+00000880: 2020 2020 2069 6620 7365 6c66 2e63 7564       if self.cud
+00000890: 615f 6374 783a 0d0a 2020 2020 2020 2020  a_ctx:..        
+000008a0: 2020 2020 2020 2020 7365 6c66 2e63 7564          self.cud
+000008b0: 615f 6374 782e 706f 7028 290d 0a20 2020  a_ctx.pop()..   
+000008c0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000008d0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+000008e0: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
+000008f0: 6461 5f63 7478 2e70 6f70 2829 0d0a 2020  da_ctx.pop()..  
+00000900: 2020 2020 2020 2020 2020 6465 6c20 7365            del se
+00000910: 6c66 2e63 7564 615f 6374 780d 0a20 2020  lf.cuda_ctx..   
+00000920: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+00000930: 756e 7469 6d65 4572 726f 7228 2246 6169  untimeError("Fai
+00000940: 6c20 746f 2061 6c6c 6f63 6174 6520 4355  l to allocate CU
+00000950: 4441 2072 6573 6f75 7263 6573 2229 2066  DA resources") f
+00000960: 726f 6d20 650d 0a0d 0a20 2020 2064 6566  rom e....    def
+00000970: 2069 6e66 6572 2873 656c 662c 2069 6d67   infer(self, img
+00000980: 7329 3a0d 0a20 2020 2020 2020 2061 7373  s):..        ass
+00000990: 6572 7420 6973 696e 7374 616e 6365 2869  ert isinstance(i
+000009a0: 6d67 732c 206e 702e 6e64 6172 7261 7929  mgs, np.ndarray)
+000009b0: 2c20 2269 6d67 7320 6d75 7374 2062 6520  , "imgs must be 
+000009c0: 6e75 6d70 7920 6172 7261 7922 0d0a 2020  numpy array"..  
+000009d0: 2020 2020 2020 6966 2073 656c 662e 6375        if self.cu
+000009e0: 6461 5f63 7478 3a0d 0a20 2020 2020 2020  da_ctx:..       
+000009f0: 2020 2020 2073 656c 662e 6375 6461 5f63       self.cuda_c
+00000a00: 7478 2e70 7573 6828 290d 0a0d 0a20 2020  tx.push()....   
+00000a10: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+00000a20: 6479 6e61 6d69 635f 6261 7463 683a 0d0a  dynamic_batch:..
+00000a30: 2020 2020 2020 2020 2020 2020 6273 203d              bs =
+00000a40: 2069 6d67 732e 7368 6170 655b 305d 0d0a   imgs.shape[0]..
+00000a50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000a60: 2e69 6e70 7574 735b 305d 2e68 6f73 7420  .inputs[0].host 
+00000a70: 3d20 696d 6773 2e72 6176 656c 2829 0d0a  = imgs.ravel()..
+00000a80: 2020 2020 2020 2020 2020 2020 2320 6d61              # ma
+00000a90: 6b65 2063 6f6e 7465 7874 2061 7761 7265  ke context aware
+00000aa0: 2077 6861 7427 7320 6261 7463 6873 697a   what's batchsiz
+00000ab0: 6520 6375 7272 656e 740d 0a20 2020 2020  e current..     
+00000ac0: 2020 2020 2020 2073 656c 662e 6f72 695f         self.ori_
+00000ad0: 696e 7075 745f 7368 6170 655b 305d 203d  input_shape[0] =
+00000ae0: 2062 730d 0a20 2020 2020 2020 2020 2020   bs..           
+00000af0: 2073 656c 662e 636f 6e74 6578 742e 7365   self.context.se
+00000b00: 745f 6269 6e64 696e 675f 7368 6170 6528  t_binding_shape(
+00000b10: 302c 2028 7365 6c66 2e6f 7269 5f69 6e70  0, (self.ori_inp
+00000b20: 7574 5f73 6861 7065 2929 0d0a 2020 2020  ut_shape))..    
+00000b30: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000b40: 2020 2020 2020 2073 656c 662e 696e 7075         self.inpu
+00000b50: 7473 5b30 5d2e 686f 7374 203d 2069 6d67  ts[0].host = img
+00000b60: 732e 7261 7665 6c28 290d 0a0d 0a20 2020  s.ravel()....   
+00000b70: 2020 2020 2069 6620 7365 6c66 2e74 696d       if self.tim
+00000b80: 696e 673a 0d0a 2020 2020 2020 2020 2020  ing:..          
+00000b90: 2020 7430 203d 2074 696d 652e 7065 7266    t0 = time.perf
+00000ba0: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
+00000bb0: 2020 2020 6f75 7473 203d 2064 6f5f 696e      outs = do_in
+00000bc0: 6665 7265 6e63 655f 7632 280d 0a20 2020  ference_v2(..   
+00000bd0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00000be0: 6e74 6578 742c 0d0a 2020 2020 2020 2020  ntext,..        
+00000bf0: 2020 2020 6269 6e64 696e 6773 3d73 656c      bindings=sel
+00000c00: 662e 6269 6e64 696e 6773 2c0d 0a20 2020  f.bindings,..   
+00000c10: 2020 2020 2020 2020 2069 6e70 7574 733d           inputs=
+00000c20: 7365 6c66 2e69 6e70 7574 732c 0d0a 2020  self.inputs,..  
+00000c30: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00000c40: 733d 7365 6c66 2e6f 7574 7075 7473 2c0d  s=self.outputs,.
+00000c50: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00000c60: 6561 6d3d 7365 6c66 2e73 7472 6561 6d2c  eam=self.stream,
+00000c70: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00000c80: 7075 745f 7465 6e73 6f72 3d69 6d67 732c  put_tensor=imgs,
+00000c90: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+00000ca0: 2020 2020 2069 6620 7365 6c66 2e63 7564       if self.cud
+00000cb0: 615f 6374 783a 0d0a 2020 2020 2020 2020  a_ctx:..        
+00000cc0: 2020 2020 7365 6c66 2e63 7564 615f 6374      self.cuda_ct
+00000cd0: 782e 706f 7028 290d 0a20 2020 2020 2020  x.pop()..       
+00000ce0: 2069 6620 7365 6c66 2e74 696d 696e 673a   if self.timing:
+00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 7431  ..            t1
+00000d00: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+00000d10: 6e74 6572 2829 0d0a 2020 2020 2020 2020  nter()..        
+00000d20: 2020 2020 7072 696e 7428 6622 656e 6769      print(f"engi
+00000d30: 6e65 2063 6f73 743a 207b 7431 202d 2074  ne cost: {t1 - t
+00000d40: 307d 2c20 6670 733a 207b 312f 2874 312d  0}, fps: {1/(t1-
+00000d50: 7430 297d 2229 0d0a 2020 2020 2020 2020  t0)}")..        
+00000d60: 6f75 7473 5f72 6573 6861 7065 6420 3d20  outs_reshaped = 
+00000d70: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00000d80: 692c 206f 2069 6e20 656e 756d 6572 6174  i, o in enumerat
+00000d90: 6528 6f75 7473 293a 0d0a 2020 2020 2020  e(outs):..      
+00000da0: 2020 2020 2020 6f5f 7320 3d20 7365 6c66        o_s = self
+00000db0: 2e6f 7574 7075 745f 7368 6170 6573 5b69  .output_shapes[i
+00000dc0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+00000dd0: 6620 7365 6c66 2e69 735f 6479 6e61 6d69  f self.is_dynami
+00000de0: 635f 6261 7463 683a 0d0a 2020 2020 2020  c_batch:..      
+00000df0: 2020 2020 2020 2020 2020 6f5f 735b 305d            o_s[0]
+00000e00: 203d 2073 656c 662e 656e 6769 6e65 2e6d   = self.engine.m
+00000e10: 6178 5f62 6174 6368 5f73 697a 650d 0a20  ax_batch_size.. 
+00000e20: 2020 2020 2020 2020 2020 206f 203d 206e             o = n
+00000e30: 702e 7265 7368 6170 6528 6f2c 206f 5f73  p.reshape(o, o_s
+00000e40: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00000e50: 6620 7365 6c66 2e69 735f 6479 6e61 6d69  f self.is_dynami
+00000e60: 635f 6261 7463 683a 0d0a 2020 2020 2020  c_batch:..      
+00000e70: 2020 2020 2020 2020 2020 6f75 7473 5f72            outs_r
+00000e80: 6573 6861 7065 642e 6170 7065 6e64 286f  eshaped.append(o
+00000e90: 5b3a 6273 2c20 2e2e 2e5d 290d 0a20 2020  [:bs, ...])..   
+00000ea0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 6f75 7473 5f72 6573 6861 7065 642e 6170  outs_reshaped.ap
+00000ed0: 7065 6e64 286f 290d 0a20 2020 2020 2020  pend(o)..       
+00000ee0: 2072 6574 7572 6e20 6f75 7473 5f72 6573   return outs_res
+00000ef0: 6861 7065 640d 0a0d 0a20 2020 2064 6566  haped....    def
+00000f00: 205f 5f64 656c 5f5f 2873 656c 6629 3a0d   __del__(self):.
+00000f10: 0a20 2020 2020 2020 2022 2222 4672 6565  .        """Free
+00000f20: 2043 5544 4120 6d65 6d6f 7269 6573 2222   CUDA memories""
+00000f30: 220d 0a20 2020 2020 2020 2064 656c 2073  "..        del s
+00000f40: 656c 662e 6f75 7470 7574 730d 0a20 2020  elf.outputs..   
+00000f50: 2020 2020 2064 656c 2073 656c 662e 696e       del self.in
+00000f60: 7075 7473 0d0a 2020 2020 2020 2020 6465  puts..        de
+00000f70: 6c20 7365 6c66 2e73 7472 6561 6d0d 0a    l self.stream..
```

### Comparing `alfred-py-3.0.6/alfred/dl/__init__.py` & `alfred-py-3.0.7/alfred/dl/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/data/common/coco_dataset.py` & `alfred-py-3.0.7/alfred/dl/data/common/coco_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,126 +11,131 @@
 try:
     from pycocotools import mask as coco_mask
 except ImportError:
     pass
 
 
 class COCOInstancesBaseDataset(GetterDataset):
-
-    def __init__(self, data_dir='auto', split='train', year='2017',
-                 use_crowded=False, read_img_with='pil'):
-        if year == '2017' and split in ['minival', 'valminusminival']:
+    def __init__(
+        self,
+        data_dir="auto",
+        split="train",
+        year="2017",
+        use_crowded=False,
+        read_img_with="pil",
+    ):
+        if year == "2017" and split in ["minival", "valminusminival"]:
             raise ValueError(
-                'coco2017 dataset does not support given split: {}'
-                .format(split))
+                "coco2017 dataset does not support given split: {}".format(split)
+            )
 
         super(COCOInstancesBaseDataset, self).__init__()
         self.use_crowded = use_crowded
         self.read_img_with = read_img_with
 
-        if split in ['val', 'minival', 'valminusminival']:
-            img_split = 'val'
+        if split in ["val", "minival", "valminusminival"]:
+            img_split = "val"
         else:
-            img_split = 'train'
+            img_split = "train"
 
-        self.img_root = os.path.join(
-            data_dir, '{}{}'.format(img_split, year))
+        self.img_root = os.path.join(data_dir, "{}{}".format(img_split, year))
         tmp = self.img_root
         if not os.path.exists(self.img_root):
-            self.img_root = os.path.join(data_dir, 'images')
+            self.img_root = os.path.join(data_dir, "images")
         assert os.path.exists(
-            self.img_root), 'we have tried img_root: {} and {}, either found, did u make sure it exists?'.format(tmp, self.img_root)
+            self.img_root
+        ), "we have tried img_root: {} and {}, either found, did u make sure it exists?".format(
+            tmp, self.img_root
+        )
         anno_path = os.path.join(
-            data_dir, 'annotations', 'instances_{}{}.json'.format(split, year))
+            data_dir, "annotations", "instances_{}{}.json".format(split, year)
+        )
 
         self.data_dir = data_dir
-        annos = json.load(open(anno_path, 'r'))
+        annos = json.load(open(anno_path, "r"))
 
         self.id_to_prop = {}
-        for prop in annos['images']:
-            self.id_to_prop[prop['id']] = prop
+        for prop in annos["images"]:
+            self.id_to_prop[prop["id"]] = prop
         self.ids = sorted(list(self.id_to_prop.keys()))
 
-        self.cat_ids = [cat['id'] for cat in annos['categories']]
+        self.cat_ids = [cat["id"] for cat in annos["categories"]]
 
         self.id_to_anno = defaultdict(list)
-        for anno in annos['annotations']:
-            self.id_to_anno[anno['image_id']].append(anno)
+        for anno in annos["annotations"]:
+            self.id_to_anno[anno["image_id"]].append(anno)
 
-        self.add_getter('img', self._get_image)
-        self.add_getter('mask', self._get_mask)
-        self.add_getter(
-            ['bbox', 'label', 'area', 'crowded'],
-            self._get_annotations)
+        self.add_getter("img", self._get_image)
+        self.add_getter("mask", self._get_mask)
+        self.add_getter(["bbox", "label", "area", "crowded"], self._get_annotations)
 
     def __len__(self):
         return len(self.ids)
 
     def _get_image(self, i):
         img_path = os.path.join(
-            self.img_root, self.id_to_prop[self.ids[i]]['file_name'])
-        if self.read_img_with == 'cv2':
+            self.img_root, self.id_to_prop[self.ids[i]]["file_name"]
+        )
+        if self.read_img_with == "cv2":
             img = cv2.imread(img_path)
         else:
             img = PIL.Image.open(img_path)
         return img
 
     def _get_mask(self, i):
         # List[{'segmentation', 'area', 'iscrowd',
         #       'image_id', 'bbox', 'category_id', 'id'}]
         annotation = self.id_to_anno[self.ids[i]]
-        H = self.id_to_prop[self.ids[i]]['height']
-        W = self.id_to_prop[self.ids[i]]['width']
+        H = self.id_to_prop[self.ids[i]]["height"]
+        W = self.id_to_prop[self.ids[i]]["width"]
 
         mask = []
         crowded = []
         for anno in annotation:
-            msk = self._segm_to_mask(anno['segmentation'], (H, W))
+            msk = self._segm_to_mask(anno["segmentation"], (H, W))
             # FIXME: some of minival annotations are malformed.
             if msk.shape != (H, W):
                 continue
             mask.append(msk)
-            crowded.append(anno['iscrowd'])
+            crowded.append(anno["iscrowd"])
         mask = np.array(mask, dtype=np.bool)
         crowded = np.array(crowded, dtype=np.bool)
         if len(mask) == 0:
             mask = np.zeros((0, H, W), dtype=np.bool)
 
         if not self.use_crowded:
             not_crowded = np.logical_not(crowded)
             mask = mask[not_crowded]
         return mask
 
     def _get_annotations(self, i):
         # List[{'segmentation', 'area', 'iscrowd',
         #       'image_id', 'bbox', 'category_id', 'id'}]
         annotation = self.id_to_anno[self.ids[i]]
-        bbox = np.array([ann['bbox'] for ann in annotation],
-                        dtype=np.float32)
+        bbox = np.array([ann["bbox"] for ann in annotation], dtype=np.float32)
         if len(bbox) == 0:
             bbox = np.zeros((0, 4), dtype=np.float32)
         # (x, y, width, height)  -> (x_min, y_min, x_max, y_max)
         bbox[:, 2] = bbox[:, 0] + bbox[:, 2]
         bbox[:, 3] = bbox[:, 1] + bbox[:, 3]
         # (x_min, y_min, x_max, y_max) -> (y_min, x_min, y_max, x_max)
         bbox = bbox[:, [1, 0, 3, 2]]
 
-        label = np.array([self.cat_ids.index(ann['category_id'])
-                          for ann in annotation], dtype=np.int32)
+        label = np.array(
+            [self.cat_ids.index(ann["category_id"]) for ann in annotation],
+            dtype=np.int32,
+        )
 
-        area = np.array([ann['area']
-                         for ann in annotation], dtype=np.float32)
+        area = np.array([ann["area"] for ann in annotation], dtype=np.float32)
 
-        crowded = np.array([ann['iscrowd']
-                            for ann in annotation], dtype=np.bool)
+        crowded = np.array([ann["iscrowd"] for ann in annotation], dtype=np.bool)
 
         # Remove invalid boxes
         bbox_area = np.prod(bbox[:, 2:] - bbox[:, :2], axis=1)
-        keep_mask = np.logical_and(bbox[:, 0] <= bbox[:, 2],
-                                   bbox[:, 1] <= bbox[:, 3])
+        keep_mask = np.logical_and(bbox[:, 0] <= bbox[:, 2], bbox[:, 1] <= bbox[:, 3])
         keep_mask = np.logical_and(keep_mask, bbox_area > 0)
 
         if not self.use_crowded:
             keep_mask = np.logical_and(keep_mask, np.logical_not(crowded))
 
         bbox = bbox[keep_mask]
         label = label[keep_mask]
@@ -147,27 +152,35 @@
             mask = np.zeros((H, W), dtype=np.uint8)
             mask = PIL.Image.fromarray(mask)
             for sgm in segm:
                 xy = np.array(sgm).reshape((-1, 2))
                 xy = [tuple(xy_i) for xy_i in xy]
                 PIL.ImageDraw.Draw(mask).polygon(xy=xy, outline=1, fill=1)
             mask = np.asarray(mask)
-        elif isinstance(segm['counts'], list):
+        elif isinstance(segm["counts"], list):
             rle = coco_mask.frPyObjects(segm, H, W)
             mask = coco_mask.decode(rle)
         else:
             mask = coco_mask.decode(segm)
         return mask.astype(np.bool)
 
 
 class COCOBboxDataset(COCOInstancesBaseDataset):
-
-    def __init__(self, data_dir='auto', split='train', year='2017',
-                 use_crowded=False, read_img_with='pil', return_area=False, return_crowded=False):
+    def __init__(
+        self,
+        data_dir="auto",
+        split="train",
+        year="2017",
+        use_crowded=False,
+        read_img_with="pil",
+        return_area=False,
+        return_crowded=False,
+    ):
         super(COCOBboxDataset, self).__init__(
-            data_dir, split, year, use_crowded, read_img_with)
-        keys = ('img', 'bbox', 'label')
+            data_dir, split, year, use_crowded, read_img_with
+        )
+        keys = ("img", "bbox", "label")
         if return_area:
-            keys += ('area',)
+            keys += ("area",)
         if return_crowded:
-            keys += ('crowded',)
+            keys += ("crowded",)
         self.keys = keys
```

### Comparing `alfred-py-3.0.6/alfred/dl/data/meta/concatenated_dataset.py` & `alfred-py-3.0.7/alfred/dl/data/meta/concatenated_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
             Each dataset should inherit
             :class:`~chainercv.chainer_experimental.datasets.sliceable.Sliceabledataset`
             and should have the same keys.
     """
 
     def __init__(self, *datasets):
         if len(datasets) == 0:
-            raise ValueError('At least one dataset is required')
+            raise ValueError("At least one dataset is required")
         self._datasets = datasets
         self._keys = datasets[0].keys
         for dataset in datasets[1:]:
             if not dataset.keys == self._keys:
-                raise ValueError('All datasets should have the same keys')
+                raise ValueError("All datasets should have the same keys")
 
     def __len__(self):
         return sum(len(dataset) for dataset in self._datasets)
 
     @property
     def keys(self):
         return self._keys
@@ -38,8 +38,8 @@
     def get_example_by_keys(self, index, key_indices):
         if index < 0:
             raise IndexError
         for dataset in self._datasets:
             if index < len(dataset):
                 return dataset.get_example_by_keys(index, key_indices)
             index -= len(dataset)
-        raise IndexError
+        raise IndexError
```

### Comparing `alfred-py-3.0.6/alfred/dl/data/meta/dataset_mixin.py` & `alfred-py-3.0.7/alfred/dl/data/meta/dataset_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy
 import six
 
 # below code from Chianer
 
+
 class DatasetMixin(object):
 
     """Default implementation of dataset indexing.
 
     DatasetMixin provides the :meth:`__getitem__` operator. The default
     implementation uses :meth:`get_example` to extract each example, and
     combines the results into a list. This mixin makes it easy to implement a
@@ -56,16 +57,15 @@
            >>> index = numpy.arange(3)
            >>> ds[index]  # Access by one-dimensional integer numpy.ndarray
            [0, 1, 2]
 
         """
         if isinstance(index, slice):
             current, stop, step = index.indices(len(self))
-            return [self.get_example(i) for i in
-                    six.moves.range(current, stop, step)]
+            return [self.get_example(i) for i in six.moves.range(current, stop, step)]
         elif isinstance(index, list) or isinstance(index, numpy.ndarray):
             return [self.get_example(i) for i in index]
         else:
             return self.get_example(index)
 
     def __len__(self):
         """Returns the number of data points."""
```

### Comparing `alfred-py-3.0.6/alfred/dl/data/meta/getter_dataset.py` & `alfred-py-3.0.7/alfred/dl/data/meta/getter_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         if self._return_tuple:
             return tuple(key for key, _, _ in self._keys)
         else:
             return self._keys[0][0]
 
     @keys.setter
     def keys(self, keys):
-        self._keys = [self._keys[key_index]
-                      for key_index in _as_key_indices(keys, self.keys)]
+        self._keys = [
+            self._keys[key_index] for key_index in _as_key_indices(keys, self.keys)
+        ]
         self._return_tuple = _is_iterable(keys)
 
     def add_getter(self, keys, getter):
         """Register a getter function
 
         Args:
             keys (string or tuple of strings): The name(s) of data
```

### Comparing `alfred-py-3.0.6/alfred/dl/data/meta/sliceable_dataset.py` & `alfred-py-3.0.7/alfred/dl/data/meta/sliceable_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,57 +4,60 @@
 
 from .dataset_mixin import DatasetMixin
 
 
 def _is_iterable(x):
     if isinstance(x, str):
         return False
-    return hasattr(x, '__iter__')
+    return hasattr(x, "__iter__")
 
 
 def _as_tuple(t):
     if _is_iterable(t):
         return tuple(t)
     else:
-        return t,
+        return (t,)
 
 
 def _bool_to_indices(indices, len_):
     true_indices = []
     for i, index in enumerate(indices):
         if isinstance(index, (bool, np.bool_)):
             if index:
                 true_indices.append(i)
         else:
             return indices
 
     if not len(indices) == len_:
         raise ValueError(
-            'The number of booleans is different from the length of dataset')
+            "The number of booleans is different from the length of dataset"
+        )
     return true_indices
 
 
 def _as_key_indices(keys, key_names):
     key_names = _as_tuple(key_names)
     keys = _bool_to_indices(_as_tuple(keys), len(key_names))
 
     for key in keys:
         if isinstance(key, numbers.Integral):
             key_index = key
             if key_index < 0:
                 key_index += len(key_names)
             if key_index not in range(0, len(key_names)):
                 raise IndexError(
-                    'index {} is out of bounds for keys with size {}'.format(
-                        key, len(key_names)))
+                    "index {} is out of bounds for keys with size {}".format(
+                        key, len(key_names)
+                    )
+                )
         else:
             try:
                 key_index = key_names.index(key)
             except ValueError:
-                raise KeyError('{} does not exists'.format(key))
+                raise KeyError("{} does not exists".format(key))
         yield key_index
 
 
 class SliceableDataset(DatasetMixin):
     """An abstract dataset class that supports slicing.
 
     This ia a dataset class that supports slicing.
@@ -90,16 +93,15 @@
         Returns:
             tuple of data
         """
         raise NotImplementedError
 
     def get_example(self, index):
         if isinstance(self.keys, tuple):
-            return self.get_example_by_keys(
-                index, tuple(range(len(self.keys))))
+            return self.get_example_by_keys(index, tuple(range(len(self.keys))))
         else:
             return self.get_example_by_keys(index, (0,))[0]
 
     @property
     def slice(self):
         return SliceHelper(self)
 
@@ -122,16 +124,18 @@
 
         if not isinstance(indices, slice):
             indices = _bool_to_indices(indices, len(self._dataset))
         key_indices = tuple(_as_key_indices(keys, self._dataset.keys))
         return_tuple = _is_iterable(keys)
 
         return SlicedDataset(
-            self._dataset, indices,
-            tuple(key_indices) if return_tuple else key_indices[0])
+            self._dataset,
+            indices,
+            tuple(key_indices) if return_tuple else key_indices[0],
+        )
 
 
 class SlicedDataset(SliceableDataset):
     """A sliced view for :class:`SliceableDataset`."""
 
     def __init__(self, dataset, indices, key_indices):
         self._dataset = dataset
@@ -152,19 +156,17 @@
             return tuple(keys[key_index] for key_index in self._key_indices)
         else:
             return keys[self._key_indices]
 
     def get_example_by_keys(self, index, key_indices):
         if isinstance(key_indices, tuple):
             key_indices = tuple(
-                _as_tuple(self._key_indices)[key_index]
-                for key_index in key_indices)
+                _as_tuple(self._key_indices)[key_index] for key_index in key_indices
+            )
         else:
             key_indices = _as_tuple(self._key_indices)[key_indices]
 
         if isinstance(self._indices, slice):
             start, _, step = self._indices.indices(len(self._dataset))
-            return self._dataset.get_example_by_keys(
-                start + index * step, key_indices)
+            return self._dataset.get_example_by_keys(start + index * step, key_indices)
         else:
-            return self._dataset.get_example_by_keys(
-                self._indices[index], key_indices)
+            return self._dataset.get_example_by_keys(self._indices[index], key_indices)
```

### Comparing `alfred-py-3.0.6/alfred/dl/evaluator/yolo_evaluator.py` & `alfred-py-3.0.7/alfred/dl/evaluator/yolo_evaluator.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,110 +5,126 @@
 from PIL import Image
 import numpy as np
 import cv2
 import shutil
 from tqdm import tqdm
 
 
-__all__ = ['YoloEvaluator']
+__all__ = ["YoloEvaluator"]
 
 
 """
 
 Parsing any dataset in Yolo format.
 You can simply change classes names to yours.
 """
 
-img_formats = ['bmp', 'jpg', 'jpeg', 'png', 'tif',
-               'tiff', 'dng']  # acceptable image suffixes
+img_formats = [
+    "bmp",
+    "jpg",
+    "jpeg",
+    "png",
+    "tif",
+    "tiff",
+    "dng",
+]  # acceptable image suffixes
 
 
 class YoloEvaluator:
-
-    def __init__(self,
-                 imgs_root,
-                 labels_root,
-                 infer_func,
-                 model=None,
-                 prep_func=None,
-                 posp_func=None,
-                 conf_thr=0.4,
-                 iou_thr=0.5):
+    def __init__(
+        self,
+        imgs_root,
+        labels_root,
+        infer_func,
+        model=None,
+        prep_func=None,
+        posp_func=None,
+        conf_thr=0.4,
+        iou_thr=0.5,
+    ):
         assert os.path.exists(imgs_root)
         assert os.path.exists(labels_root)
 
         self.infer_func = infer_func
         self.model_ = model
         self.prep_func = prep_func
         self.posp_func = posp_func
 
         self.conf_thr = conf_thr
         self.iou_thr = iou_thr
 
         self._data_root = imgs_root
-        logger.info('data_root: {}'.format(self._data_root))
+        logger.info("data_root: {}".format(self._data_root))
 
         self.img_files = []
         self.label_files = []
         self.load_combined_imgs_and_labels(imgs_root, labels_root)
 
         self.hold_vis = True
-        logger.info(
-            'Press space to vis image, press q to skip and continue eval.')
+        logger.info("Press space to vis image, press q to skip and continue eval.")
 
     def load_combined_imgs_and_labels(self, imgs_root, labels_root):
-        logger.info('labels root path: {}, img root: {}, pls check it they right or not.'.format(
-            imgs_root, labels_root))
+        logger.info(
+            "labels root path: {}, img root: {}, pls check it they right or not.".format(
+                imgs_root, labels_root
+            )
+        )
         self.label_files = glob.glob(os.path.join(labels_root, "*.txt"))
         for ext in img_formats:
             self.img_files.extend(
-                glob.glob(os.path.join(imgs_root, '*.{}'.format(ext))))
+                glob.glob(os.path.join(imgs_root, "*.{}".format(ext)))
+            )
         if len(self.img_files) != len(self.label_files):
-            imgs_names = [os.path.basename(i).split('.')[0]
-                          for i in self.img_files]
-            labels_names = [os.path.basename(i).split(
-                '.')[0] for i in self.label_files]
+            imgs_names = [os.path.basename(i).split(".")[0] for i in self.img_files]
+            labels_names = [os.path.basename(i).split(".")[0] for i in self.label_files]
             valid_files = [i for i in imgs_names if i in labels_names]
-            logger.info('original imgs: {}, original labels: {}, valid num: {}'.format(
-                len(self.img_files), len(self.label_files), len(valid_files)))
+            logger.info(
+                "original imgs: {}, original labels: {}, valid num: {}".format(
+                    len(self.img_files), len(self.label_files), len(valid_files)
+                )
+            )
             # labels is more than images
-            self.label_files = [os.path.join(
-                labels_root, i + '.txt') for i in valid_files]
-            self.img_files = [os.path.join(
-                imgs_root, i + '.jpg') for i in valid_files]
+            self.label_files = [
+                os.path.join(labels_root, i + ".txt") for i in valid_files
+            ]
+            self.img_files = [os.path.join(imgs_root, i + ".jpg") for i in valid_files]
         self.img_files = sorted(self.img_files)
         self.label_files = sorted(self.label_files)
-        logger.info('img num: {}, label num: {}'.format(
-            len(self.img_files), len(self.label_files)))
+        logger.info(
+            "img num: {}, label num: {}".format(
+                len(self.img_files), len(self.label_files)
+            )
+        )
         logger.info(self.img_files[89])
         logger.info(self.label_files[89])
-        logger.info('Please check if images and labels are paired properly.')
+        logger.info("Please check if images and labels are paired properly.")
 
     def _load_yolo_boxes_and_labels(self, lb_file, ori_w, ori_h):
-        with open(lb_file, 'r') as f:
-            l = np.array([x.split() for x in f.read().strip(
-            ).splitlines()], dtype=np.float32)  # labels
-            l = np.clip(l, 0, 1.)
+        with open(lb_file, "r") as f:
+            l = np.array(
+                [x.split() for x in f.read().strip().splitlines()], dtype=np.float32
+            )  # labels
+            l = np.clip(l, 0, 1.0)
         res_boxes = []
         res_labels = []
         if len(l):
             boxes = l[:, 1:]
             labels = l[:, 0]
 
             for i, b in enumerate(boxes):
                 cx, cy, w, h = b
                 cx *= ori_w
                 cy *= ori_h
                 w *= ori_w
                 h *= ori_h
-                x = cx - w/2
-                y = cy - h/2
+                x = cx - w / 2
+                y = cy - h / 2
                 if x < 0 or y < 0 or w <= 2 or h <= 2:
                     continue
-                res_boxes.append(np.array([x, y, x+w, y+h]).astype(np.int))
+                res_boxes.append(np.array([x, y, x + w, y + h]).astype(np.int))
                 res_labels.append(labels[i])
         return res_boxes, res_labels
 
     def exif_size(self, img):
         # Returns exif-corrected PIL size
         s = img.size  # (width, height)
         try:
@@ -144,15 +160,15 @@
         bottom_line = min(rec1[3], rec2[3])
 
         # judge if there is an intersect
         if left_line >= right_line or top_line >= bottom_line:
             return 0
         else:
             intersect = (right_line - left_line) * (bottom_line - top_line)
-            return (intersect / (sum_area - intersect))*1.0
+            return (intersect / (sum_area - intersect)) * 1.0
 
     def recall_precision(self, gt, pre, iou_thr=0.5):
         # recall
         recall_sum = len(gt)
         recall_cnt = 0
         precision_sum = len(pre)
         precision_cnt = 0
@@ -174,15 +190,15 @@
         if recall_cnt > recall_sum:
             print(" ----------------------》》》 error recall")
         if precision_cnt > precision_sum:
             print(" ----------------------》》》 error precision")
         return (recall_sum, recall_cnt, precision_sum, precision_cnt)
 
     def eval_precisely(self):
-        recall_sum, recall_cnt, precision_sum, precision_cnt = 0., 0., 0., 0.
+        recall_sum, recall_cnt, precision_sum, precision_cnt = 0.0, 0.0, 0.0, 0.0
         mAPs = []
         mrecall = []
         pic_cnt = 0
 
         tbar = tqdm(self.img_files)
         for i, identity in enumerate(tbar):
             # load ground truth
@@ -212,47 +228,59 @@
                 x1, y1, x2, y2, cls_id, conf = m_
                 x1, y1, x2, y2 = int(x1), int(y1), int(x2), int(y2)
                 if conf >= self.conf_thr:
                     pre_list.append((x1, y1, x2, y2))
                     cv2.rectangle(img, (x1, y1), (x2, y2), (0, 255, 0), 2)
 
             pic_cnt += 1
-            eval_list = self.recall_precision(
-                gt_list, pre_list, iou_thr=self.iou_thr)
+            eval_list = self.recall_precision(gt_list, pre_list, iou_thr=self.iou_thr)
             # logger.info(eval_list)
 
             recall_sum += eval_list[0]
             recall_cnt += eval_list[1]
             precision_sum += eval_list[2]
             precision_cnt += eval_list[3]
             # print('{} {} {} {}'.format(recall_sum, recall_cnt, precision_sum, precision_cnt))
             if (recall_sum > 0) and (precision_sum > 0):
                 if eval_list[2] > 0:
-                    mAPs.append(eval_list[3]/eval_list[2])
+                    mAPs.append(eval_list[3] / eval_list[2])
                 else:
                     if eval_list[0] > 0:
                         mAPs.append(0)
                 if eval_list[0] > 0:
-                    mrecall.append(eval_list[1]/eval_list[0])
+                    mrecall.append(eval_list[1] / eval_list[0])
                 # print(recall_cnt,recall_sum,precision_cnt,precision_sum)
 
-            tbar.set_postfix(recall='{:.3f}'.format(recall_cnt/recall_sum), precision='{:.3f}'.format(
-                precision_cnt/precision_sum), mAP='{:.3f}'.format(np.mean(mAPs)), refresh=True)
+            tbar.set_postfix(
+                recall="{:.3f}".format(recall_cnt / recall_sum),
+                precision="{:.3f}".format(precision_cnt / precision_sum),
+                mAP="{:.3f}".format(np.mean(mAPs)),
+                refresh=True,
+            )
 
             if self.hold_vis:
-                cv2.imshow('aa', img)
-                if cv2.waitKey(0) & 0xFF == ord('q'):
-                    print('Pressed Q, continue eval without vis.')
+                cv2.imshow("aa", img)
+                if cv2.waitKey(0) & 0xFF == ord("q"):
+                    print("Pressed Q, continue eval without vis.")
                     self.hold_vis = False
                     cv2.destroyAllWindows()
-        print("[\n{:6d}] conf_thr: {:.2f}, iou_thr: {:.2f}, recall: {:.5f}, precision: {:.5f}, mrecall: {:.3f}, map: {:.3f}".
-              format(pic_cnt, self.conf_thr, self.iou_thr, recall_cnt/recall_sum, precision_cnt/precision_sum, np.mean(mrecall), np.mean(mAPs)))
+        print(
+            "[\n{:6d}] conf_thr: {:.2f}, iou_thr: {:.2f}, recall: {:.5f}, precision: {:.5f}, mrecall: {:.3f}, map: {:.3f}".format(
+                pic_cnt,
+                self.conf_thr,
+                self.iou_thr,
+                recall_cnt / recall_sum,
+                precision_cnt / precision_sum,
+                np.mean(mrecall),
+                np.mean(mAPs),
+            )
+        )
 
     def eval(self):
-        recall_sum, recall_cnt, precision_sum, precision_cnt = 0., 0., 0., 0.
+        recall_sum, recall_cnt, precision_sum, precision_cnt = 0.0, 0.0, 0.0, 0.0
         mAPs = []
         mrecall = []
         pic_cnt = 0
 
         for i, identity in enumerate(self.img_files):
             # load ground truth
             im = Image.open(identity)
@@ -274,27 +302,35 @@
             for m_ in out:
                 x1, y1, x2, y2, conf = m_
                 x1, y1, x2, y2 = int(x1), int(y1), int(x2), int(y2)
                 if conf >= self.conf_thr:
                     pre_list.append((y1, x1, y2, x2))
 
             pic_cnt += 1
-            eval_list = self.recall_precision(
-                gt_list, pre_list, iou_thr=self.iou_thr)
+            eval_list = self.recall_precision(gt_list, pre_list, iou_thr=self.iou_thr)
 
             recall_sum += eval_list[0]
             recall_cnt += eval_list[1]
             precision_sum += eval_list[2]
             precision_cnt += eval_list[3]
             if (recall_sum > 0) and (precision_sum > 0):
                 if eval_list[2] > 0:
-                    mAPs.append(eval_list[3]/eval_list[2])
+                    mAPs.append(eval_list[3] / eval_list[2])
                 else:
                     if eval_list[0] > 0:
                         mAPs.append(0)
                 if eval_list[0] > 0:
-                    mrecall.append(eval_list[1]/eval_list[0])
+                    mrecall.append(eval_list[1] / eval_list[0])
                 # print(recall_cnt,recall_sum,precision_cnt,precision_sum)
-                print("  {:6d}>  -->>conf_thr :{:.2f} , iou_thr :{:.2f} , recall :{:.5f} , precision :{:.5f}, mrecall :{:.3f}, map :{:.3f}".
-                      format(pic_cnt, self.conf_thr, self.iou_thr, recall_cnt/recall_sum, precision_cnt/precision_sum, np.mean(mrecall), np.mean(map)), end='\r')
-            print('all recall: {}, all precision: {}'.format(
-                recall_sum, precision_sum))
+                print(
+                    "  {:6d}>  -->>conf_thr :{:.2f} , iou_thr :{:.2f} , recall :{:.5f} , precision :{:.5f}, mrecall :{:.3f}, map :{:.3f}".format(
+                        pic_cnt,
+                        self.conf_thr,
+                        self.iou_thr,
+                        recall_cnt / recall_sum,
+                        precision_cnt / precision_sum,
+                        np.mean(mrecall),
+                        np.mean(map),
+                    ),
+                    end="\r",
+                )
+            print("all recall: {}, all precision: {}".format(recall_sum, precision_sum))
```

### Comparing `alfred-py-3.0.6/alfred/dl/inference/__init__.py` & `alfred-py-3.0.7/alfred/dl/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/inference/image_inference.py` & `alfred-py-3.0.7/alfred/dl/inference/image_inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,119 +34,120 @@
 import sys
 import time
 from deprecated import deprecated
 from alfred.utils.log import logger as logging
 
 
 class ImageInferEngine(object):
-
     def __init__(self, f, is_show=False, record=False):
         """
         run on
 
         1. single file
         2. video file
         3. webcam
         :param f:
         """
-        self.img_ext = ['png', 'jpg', 'jpeg']
-        self.video_ext = ['avi', 'mp4']
+        self.img_ext = ["png", "jpg", "jpeg"]
+        self.video_ext = ["avi", "mp4"]
         self.f = f
         self.is_show = is_show
         self.record = record
         self.crt_cost = 0
 
         if not f:
-            self.mode = 'webcam'
-        elif os.path.basename(f).split('.')[-1] in self.img_ext:
-            self.mode = 'image'
-        elif os.path.basename(f).split('.')[-1] in self.video_ext:
-            self.mode = 'video'
-        logging.info('[Demo] in {} mode.'.format(self.mode))
+            self.mode = "webcam"
+        elif os.path.basename(f).split(".")[-1] in self.img_ext:
+            self.mode = "image"
+        elif os.path.basename(f).split(".")[-1] in self.video_ext:
+            self.mode = "video"
+        logging.info("[Demo] in {} mode.".format(self.mode))
 
     def read_image_file(self, img_f):
         """
         this method should return image read result
 
         :param img_f:
         :return:
         """
-        if self.mode == 'image':
-            raise NotImplementedError('read_image_file must be implemented when using image mode ')
+        if self.mode == "image":
+            raise NotImplementedError(
+                "read_image_file must be implemented when using image mode "
+            )
         else:
             pass
 
     @deprecated(reason="This method has been deprecated, using solve_one_image instead")
     def solve_a_image(self, img):
         """
         this method must be implemented to solve a single image
 
         img must be a numpy array
         then return the detection or segmentation out
         :param img:
         :return:
         """
-        raise NotImplementedError('solve_a_image method must be implemented')
+        raise NotImplementedError("solve_a_image method must be implemented")
 
     def solve_one_image(self, img):
         """
         this method must be implemented to solve a single image
 
         img must be a numpy array
         then return the detection or segmentation out
         :param img:
         :return:
         """
-        raise NotImplementedError('solve_a_image method must be implemented')
+        raise NotImplementedError("solve_a_image method must be implemented")
 
     def vis_result(self, img, net_out):
         """
         this method must be implement to visualize result on image
 
         :param img
         :param net_out:
         :return:
         """
-        raise NotImplementedError('Visualize network output on image')
+        raise NotImplementedError("Visualize network output on image")
 
     def run(self):
-        if self.mode == 'image':
+        if self.mode == "image":
             img = self.read_image_file(self.f)
             res = self.solve_a_image(img)
             res_img = self.vis_result(img, res)
             if self.is_show:
-                cv2.imshow('result', res_img)
+                cv2.imshow("result", res_img)
                 cv2.waitKey(0)
-        elif self.mode == 'video' or self.mode == 'webcam':
+        elif self.mode == "video" or self.mode == "webcam":
             cap = cv2.VideoCapture(self.f)
-            if self.record and self.mode == 'video':
+            if self.record and self.mode == "video":
                 fps = cap.get(cv2.CAP_PROP_FPS)
-                size = (int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
-                        int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)))
-                save_f = os.path.join(os.path.dirname(self.f), 'result_' + os.path.basename(self.f))
-                logging.info('Result video will record into {}'.format(save_f))
-                video_writer = cv2.VideoWriter(save_f, cv2.VideoWriter_fourcc(*'DIVX'), fps, size)
+                size = (
+                    int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
+                    int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
+                )
+                save_f = os.path.join(
+                    os.path.dirname(self.f), "result_" + os.path.basename(self.f)
+                )
+                logging.info("Result video will record into {}".format(save_f))
+                video_writer = cv2.VideoWriter(
+                    save_f, cv2.VideoWriter_fourcc(*"DIVX"), fps, size
+                )
 
             while cap.isOpened():
                 ok, frame = cap.read()
                 if ok:
                     tic = time.time()
                     res = self.solve_a_image(frame)
                     if self.is_show:
-                        logging.info('fps: {}'.format(1 / (time.time() - tic)))
+                        logging.info("fps: {}".format(1 / (time.time() - tic)))
                     self.crt_cost = time.time() - tic
                     res_img = self.vis_result(frame, res)
-                    if self.record and self.mode == 'video':
+                    if self.record and self.mode == "video":
                         video_writer.write(res_img)
 
                     if self.is_show:
-                        cv2.imshow('result', res_img)
+                        cv2.imshow("result", res_img)
                         cv2.waitKey(1)
                 else:
-                    logging.info('Done')
+                    logging.info("Done")
                     exit(0)
-
-
-
-
-
-
```

### Comparing `alfred-py-3.0.6/alfred/dl/metrics/iou_loss.py` & `alfred-py-3.0.7/alfred/dl/metrics/iou_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,30 @@
         target_w = target[:, 2] - target[:, 0]
         target_h = target[:, 3] - target[:, 1]
 
     dx = target_ctrx - pred_ctrx
     dy = target_ctry - pred_ctry
 
     loss_dx = 1 - torch.max(
-        (target_w - 2 * dx.abs()) /
-        (target_w + 2 * dx.abs() + eps), torch.zeros_like(dx))
+        (target_w - 2 * dx.abs()) / (target_w + 2 * dx.abs() + eps),
+        torch.zeros_like(dx),
+    )
     loss_dy = 1 - torch.max(
-        (target_h - 2 * dy.abs()) /
-        (target_h + 2 * dy.abs() + eps), torch.zeros_like(dy))
-    loss_dw = 1 - torch.min(target_w / (pred_w + eps), pred_w /
-                            (target_w + eps))
-    loss_dh = 1 - torch.min(target_h / (pred_h + eps), pred_h /
-                            (target_h + eps))
-    loss_comb = torch.stack([loss_dx, loss_dy, loss_dw, loss_dh],
-                            dim=-1).view(loss_dx.size(0), -1)
-
-    loss = torch.where(loss_comb < beta, 0.5 * loss_comb * loss_comb / beta,
-                       loss_comb - 0.5 * beta)
+        (target_h - 2 * dy.abs()) / (target_h + 2 * dy.abs() + eps),
+        torch.zeros_like(dy),
+    )
+    loss_dw = 1 - torch.min(target_w / (pred_w + eps), pred_w / (target_w + eps))
+    loss_dh = 1 - torch.min(target_h / (pred_h + eps), pred_h / (target_h + eps))
+    loss_comb = torch.stack([loss_dx, loss_dy, loss_dw, loss_dh], dim=-1).view(
+        loss_dx.size(0), -1
+    )
+
+    loss = torch.where(
+        loss_comb < beta, 0.5 * loss_comb * loss_comb / beta, loss_comb - 0.5 * beta
+    )
     return loss
 
 
 @weighted_loss
 def giou_loss(pred, target, eps=1e-7):
     r"""`Generalized Intersection over Union: A Metric and A Loss for Bounding
     Box Regression <https://arxiv.org/abs/1902.09630>`_.
@@ -82,15 +84,15 @@
             shape (n, 4).
         target (torch.Tensor): Corresponding gt bboxes, shape (n, 4).
         eps (float): Eps to avoid log(0).
 
     Return:
         Tensor: Loss tensor.
     """
-    gious = bbox_overlaps(pred, target, mode='giou', is_aligned=True, eps=eps)
+    gious = bbox_overlaps(pred, target, mode="giou", is_aligned=True, eps=eps)
     loss = 1 - gious
     return loss
 
 
 @weighted_loss
 def diou_loss(pred, target, eps=1e-7):
     r"""`Implementation of Distance-IoU Loss: Faster and Better
@@ -131,16 +133,16 @@
     c2 = cw**2 + ch**2 + eps
 
     b1_x1, b1_y1 = pred[:, 0], pred[:, 1]
     b1_x2, b1_y2 = pred[:, 2], pred[:, 3]
     b2_x1, b2_y1 = target[:, 0], target[:, 1]
     b2_x2, b2_y2 = target[:, 2], target[:, 3]
 
-    left = ((b2_x1 + b2_x2) - (b1_x1 + b1_x2))**2 / 4
-    right = ((b2_y1 + b2_y2) - (b1_y1 + b1_y2))**2 / 4
+    left = ((b2_x1 + b2_x2) - (b1_x1 + b1_x2)) ** 2 / 4
+    right = ((b2_y1 + b2_y2) - (b1_y1 + b1_y2)) ** 2 / 4
     rho2 = left + right
 
     # DIoU
     dious = ious - rho2 / c2
     loss = 1 - dious
     return loss
 
@@ -160,18 +162,18 @@
         eps (float): Eps to avoid log(0).
     Return:
         Tensor: Loss tensor.
     """
     # if xyxy is false, make to xyxy
     if not xyxy:
         # cxcywh -> xyxy
-        pred[:, :2] = pred[:, :2] - pred[:, 2:]/2
+        pred[:, :2] = pred[:, :2] - pred[:, 2:] / 2
         pred[:, 2:] = pred[:, :2] + pred[:, 2:]
 
-        target[:, :2] = target[:, :2] - target[:, 2:]/2
+        target[:, :2] = target[:, :2] - target[:, 2:] / 2
         target[:, 2:] = target[:, :2] + target[:, 2:]
     # overlap
     lt = torch.max(pred[:, :2], target[:, :2])
     rb = torch.min(pred[:, 2:], target[:, 2:])
     wh = (rb - lt).clamp(min=0)
     overlap = wh[:, 0] * wh[:, 1]
 
@@ -197,16 +199,16 @@
     b1_x2, b1_y2 = pred[:, 2], pred[:, 3]
     b2_x1, b2_y1 = target[:, 0], target[:, 1]
     b2_x2, b2_y2 = target[:, 2], target[:, 3]
 
     w1, h1 = b1_x2 - b1_x1, b1_y2 - b1_y1 + eps
     w2, h2 = b2_x2 - b2_x1, b2_y2 - b2_y1 + eps
 
-    left = ((b2_x1 + b2_x2) - (b1_x1 + b1_x2))**2 / 4
-    right = ((b2_y1 + b2_y2) - (b1_y1 + b1_y2))**2 / 4
+    left = ((b2_x1 + b2_x2) - (b1_x1 + b1_x2)) ** 2 / 4
+    right = ((b2_y1 + b2_y2) - (b1_y1 + b1_y2)) ** 2 / 4
     rho2 = left + right
 
     factor = 4 / math.pi**2
     v = factor * torch.pow(torch.atan(w2 / h2) - torch.atan(w1 / h1), 2)
 
     # CIoU
     cious = ious - (rho2 / c2 + v**2 / (1 - ious + v))
@@ -242,42 +244,41 @@
     center_x2 = bboxes2[:, 0]
     center_y2 = bboxes2[:, 1]
 
     inter_l = torch.max(center_x1 - w1 / 2, center_x2 - w2 / 2)
     inter_r = torch.min(center_x1 + w1 / 2, center_x2 + w2 / 2)
     inter_t = torch.max(center_y1 - h1 / 2, center_y2 - h2 / 2)
     inter_b = torch.min(center_y1 + h1 / 2, center_y2 + h2 / 2)
-    inter_area = torch.clamp((inter_r - inter_l), min=0) * \
-        torch.clamp((inter_b - inter_t), min=0)
+    inter_area = torch.clamp((inter_r - inter_l), min=0) * torch.clamp(
+        (inter_b - inter_t), min=0
+    )
 
     c_l = torch.min(center_x1 - w1 / 2, center_x2 - w2 / 2)
     c_r = torch.max(center_x1 + w1 / 2, center_x2 + w2 / 2)
     c_t = torch.min(center_y1 - h1 / 2, center_y2 - h2 / 2)
     c_b = torch.max(center_y1 + h1 / 2, center_y2 + h2 / 2)
 
-    inter_diag = (center_x2 - center_x1)**2 + (center_y2 - center_y1)**2
-    c_diag = torch.clamp((c_r - c_l), min=0)**2 + \
-        torch.clamp((c_b - c_t), min=0)**2
+    inter_diag = (center_x2 - center_x1) ** 2 + (center_y2 - center_y1) ** 2
+    c_diag = torch.clamp((c_r - c_l), min=0) ** 2 + torch.clamp((c_b - c_t), min=0) ** 2
 
-    union = area1+area2-inter_area
+    union = area1 + area2 - inter_area
     u = (inter_diag) / c_diag
     iou = inter_area / union
-    v = (4 / (math.pi ** 2)) * \
-        torch.pow((torch.atan(w2 / h2) - torch.atan(w1 / h1)), 2)
+    v = (4 / (math.pi**2)) * torch.pow((torch.atan(w2 / h2) - torch.atan(w1 / h1)), 2)
     with torch.no_grad():
         S = (iou > 0.5).float()
-        alpha = S*v/(1-iou+v)
+        alpha = S * v / (1 - iou + v)
     cious = iou - u - alpha * v
     cious = torch.clamp(cious, min=-1.0, max=1.0)
     if exchange:
         cious = cious.T
     if sum:
-        return torch.sum(1-cious)
+        return torch.sum(1 - cious)
     else:
-        return 1-cious
+        return 1 - cious
 
 
 def bbox_iou(box1, box2, x1y1x2y2=True, GIoU=False, DIoU=False, CIoU=False, eps=1e-7):
     # Returns the IoU of box1 to box2. box1 is 4, box2 is nx4
     box2 = box2.T
 
     # Get the coordinates of bounding boxes
@@ -287,52 +288,61 @@
     else:  # transform from xywh to xyxy
         b1_x1, b1_x2 = box1[0] - box1[2] / 2, box1[0] + box1[2] / 2
         b1_y1, b1_y2 = box1[1] - box1[3] / 2, box1[1] + box1[3] / 2
         b2_x1, b2_x2 = box2[0] - box2[2] / 2, box2[0] + box2[2] / 2
         b2_y1, b2_y2 = box2[1] - box2[3] / 2, box2[1] + box2[3] / 2
 
     # Intersection area
-    inter = (torch.min(b1_x2, b2_x2) - torch.max(b1_x1, b2_x1)).clamp(0) * \
-            (torch.min(b1_y2, b2_y2) - torch.max(b1_y1, b2_y1)).clamp(0)
+    inter = (torch.min(b1_x2, b2_x2) - torch.max(b1_x1, b2_x1)).clamp(0) * (
+        torch.min(b1_y2, b2_y2) - torch.max(b1_y1, b2_y1)
+    ).clamp(0)
 
     # Union Area
     w1, h1 = b1_x2 - b1_x1, b1_y2 - b1_y1 + eps
     w2, h2 = b2_x2 - b2_x1, b2_y2 - b2_y1 + eps
     union = w1 * h1 + w2 * h2 - inter + eps
 
     iou = inter / union
     if GIoU or DIoU or CIoU:
         # convex (smallest enclosing box) width
         cw = torch.max(b1_x2, b2_x2) - torch.min(b1_x1, b2_x1)
         ch = torch.max(b1_y2, b2_y2) - torch.min(b1_y1, b2_y1)  # convex height
         if CIoU or DIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
-            c2 = cw ** 2 + ch ** 2 + eps  # convex diagonal squared
-            rho2 = ((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 +
-                    (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4  # center distance squared
+            c2 = cw**2 + ch**2 + eps  # convex diagonal squared
+            rho2 = (
+                (b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2
+                + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2
+            ) / 4  # center distance squared
             if DIoU:
                 return iou - rho2 / c2  # DIoU
-            elif CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
-                v = (4 / math.pi ** 2) * \
-                    torch.pow(torch.atan(w2 / h2) - torch.atan(w1 / h1), 2)
+            elif (
+                CIoU
+            ):  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
+                v = (4 / math.pi**2) * torch.pow(
+                    torch.atan(w2 / h2) - torch.atan(w1 / h1), 2
+                )
                 with torch.no_grad():
                     alpha = v / (v - iou + (1 + eps))
                 return iou - (rho2 / c2 + v * alpha)  # CIoU
         else:  # GIoU https://arxiv.org/pdf/1902.09630.pdf
             c_area = cw * ch + eps  # convex area
             return iou - (c_area - union) / c_area  # GIoU
     else:
         return iou  # IoU
 
 
-def bboxes_iou(boxes1, boxes2, x1y1x2y2=True, GIoU=False, DIoU=False, CIoU=False, eps=1e-7):
+def bboxes_iou(
+    boxes1, boxes2, x1y1x2y2=True, GIoU=False, DIoU=False, CIoU=False, eps=1e-7
+):
     """
     box1 is N,4 xyxy format
     box2 is N,4 xyxy format
     """
     n = boxes1.shape[0]
     res = torch.zeros([n, boxes2.shape[0]])
     for i in range(n):
         box1 = boxes1[i]
-        a = bbox_iou(box1, boxes2, x1y1x2y2=x1y1x2y2,
-                     GIoU=GIoU, DIoU=DIoU, CIoU=CIoU, eps=eps)
+        a = bbox_iou(
+            box1, boxes2, x1y1x2y2=x1y1x2y2, GIoU=GIoU, DIoU=DIoU, CIoU=CIoU, eps=eps
+        )
         res[i, :] = a
     return res
```

### Comparing `alfred-py-3.0.6/alfred/dl/metrics/utils.py` & `alfred-py-3.0.7/alfred/dl/metrics/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import torch
 import torch.nn.functional as F
 
 
-def bbox_overlaps(bboxes1, bboxes2, mode='iou', is_aligned=False, eps=1e-6):
+def bbox_overlaps(bboxes1, bboxes2, mode="iou", is_aligned=False, eps=1e-6):
     """Calculate overlap between two set of bboxes.
 
     If ``is_aligned `` is ``False``, then calculate the overlaps between each
     bbox of bboxes1 and bboxes2, otherwise the overlaps between each aligned
     pair of bboxes1 and bboxes2.
 
     Args:
@@ -51,77 +51,79 @@
         >>>     [0, 0, 10, 9],
         >>> ])
         >>> assert tuple(bbox_overlaps(empty, nonempty).shape) == (0, 1)
         >>> assert tuple(bbox_overlaps(nonempty, empty).shape) == (1, 0)
         >>> assert tuple(bbox_overlaps(empty, empty).shape) == (0, 0)
     """
 
-    assert mode in ['iou', 'iof', 'giou'], f'Unsupported mode {mode}'
+    assert mode in ["iou", "iof", "giou"], f"Unsupported mode {mode}"
     # Either the boxes are empty or the length of boxes's last dimenstion is 4
-    assert (bboxes1.size(-1) == 4 or bboxes1.size(0) == 0)
-    assert (bboxes2.size(-1) == 4 or bboxes2.size(0) == 0)
+    assert bboxes1.size(-1) == 4 or bboxes1.size(0) == 0
+    assert bboxes2.size(-1) == 4 or bboxes2.size(0) == 0
 
     # Batch dim must be the same
     # Batch dim: (B1, B2, ... Bn)
     assert bboxes1.shape[:-2] == bboxes2.shape[:-2]
     batch_shape = bboxes1.shape[:-2]
 
     rows = bboxes1.size(-2)
     cols = bboxes2.size(-2)
     if is_aligned:
         assert rows == cols
 
     if rows * cols == 0:
         if is_aligned:
-            return bboxes1.new(batch_shape + (rows, ))
+            return bboxes1.new(batch_shape + (rows,))
         else:
             return bboxes1.new(batch_shape + (rows, cols))
 
-    area1 = (bboxes1[..., 2] - bboxes1[..., 0]) * (
-        bboxes1[..., 3] - bboxes1[..., 1])
-    area2 = (bboxes2[..., 2] - bboxes2[..., 0]) * (
-        bboxes2[..., 3] - bboxes2[..., 1])
+    area1 = (bboxes1[..., 2] - bboxes1[..., 0]) * (bboxes1[..., 3] - bboxes1[..., 1])
+    area2 = (bboxes2[..., 2] - bboxes2[..., 0]) * (bboxes2[..., 3] - bboxes2[..., 1])
 
     if is_aligned:
         lt = torch.max(bboxes1[..., :2], bboxes2[..., :2])  # [B, rows, 2]
         rb = torch.min(bboxes1[..., 2:], bboxes2[..., 2:])  # [B, rows, 2]
 
         wh = (rb - lt).clamp(min=0)  # [B, rows, 2]
         overlap = wh[..., 0] * wh[..., 1]
 
-        if mode in ['iou', 'giou']:
+        if mode in ["iou", "giou"]:
             union = area1 + area2 - overlap
         else:
             union = area1
-        if mode == 'giou':
+        if mode == "giou":
             enclosed_lt = torch.min(bboxes1[..., :2], bboxes2[..., :2])
             enclosed_rb = torch.max(bboxes1[..., 2:], bboxes2[..., 2:])
     else:
-        lt = torch.max(bboxes1[..., :, None, :2],
-                       bboxes2[..., None, :, :2])  # [B, rows, cols, 2]
-        rb = torch.min(bboxes1[..., :, None, 2:],
-                       bboxes2[..., None, :, 2:])  # [B, rows, cols, 2]
+        lt = torch.max(
+            bboxes1[..., :, None, :2], bboxes2[..., None, :, :2]
+        )  # [B, rows, cols, 2]
+        rb = torch.min(
+            bboxes1[..., :, None, 2:], bboxes2[..., None, :, 2:]
+        )  # [B, rows, cols, 2]
 
         wh = (rb - lt).clamp(min=0)  # [B, rows, cols, 2]
         overlap = wh[..., 0] * wh[..., 1]
 
-        if mode in ['iou', 'giou']:
+        if mode in ["iou", "giou"]:
             union = area1[..., None] + area2[..., None, :] - overlap
         else:
             union = area1[..., None]
-        if mode == 'giou':
-            enclosed_lt = torch.min(bboxes1[..., :, None, :2],
-                                    bboxes2[..., None, :, :2])
-            enclosed_rb = torch.max(bboxes1[..., :, None, 2:],
-                                    bboxes2[..., None, :, 2:])
+        if mode == "giou":
+            enclosed_lt = torch.min(
+                bboxes1[..., :, None, :2], bboxes2[..., None, :, :2]
+            )
+            enclosed_rb = torch.max(
+                bboxes1[..., :, None, 2:], bboxes2[..., None, :, 2:]
+            )
 
     eps = union.new_tensor([eps])
     union = torch.max(union, eps)
     ious = overlap / union
-    if mode in ['iou', 'iof']:
+    if mode in ["iou", "iof"]:
         return ious
     # calculate gious
     enclose_wh = (enclosed_rb - enclosed_lt).clamp(min=0)
     enclose_area = enclose_wh[..., 0] * enclose_wh[..., 1]
     enclose_area = torch.max(enclose_area, eps)
     gious = ious - (enclose_area - union) / enclose_area
     return gious
@@ -143,15 +145,15 @@
         return loss
     elif reduction_enum == 1:
         return loss.mean()
     elif reduction_enum == 2:
         return loss.sum()
 
 
-def weight_reduce_loss(loss, weight=None, reduction='mean', avg_factor=None):
+def weight_reduce_loss(loss, weight=None, reduction="mean", avg_factor=None):
     """Apply element-wise weight and reduce loss.
 
     Args:
         loss (Tensor): Element-wise loss.
         weight (Tensor): Element-wise weights.
         reduction (str): Same as built-in losses of PyTorch.
         avg_factor (float): Avarage factor when computing the mean of losses.
@@ -164,18 +166,18 @@
         loss = loss * weight
 
     # if avg_factor is not specified, just reduce the loss
     if avg_factor is None:
         loss = reduce_loss(loss, reduction)
     else:
         # if reduction is mean, then average the loss by avg_factor
-        if reduction == 'mean':
+        if reduction == "mean":
             loss = loss.sum() / avg_factor
         # if reduction is 'none', then do nothing, otherwise raise an error
-        elif reduction != 'none':
+        elif reduction != "none":
             raise ValueError('avg_factor can not be used with reduction="sum"')
     return loss
 
 
 def weighted_loss(loss_func):
     """Create a weighted version of a given loss function.
 
@@ -204,19 +206,14 @@
     >>> l1_loss(pred, target, reduction='none')
     tensor([1., 1., 2.])
     >>> l1_loss(pred, target, weight, avg_factor=2)
     tensor(1.5000)
     """
 
     @functools.wraps(loss_func)
-    def wrapper(pred,
-                target,
-                weight=None,
-                reduction='mean',
-                avg_factor=None,
-                **kwargs):
+    def wrapper(pred, target, weight=None, reduction="mean", avg_factor=None, **kwargs):
         # get element-wise loss
         loss = loss_func(pred, target, **kwargs)
         loss = weight_reduce_loss(loss, weight, reduction, avg_factor)
         return loss
 
     return wrapper
```

### Comparing `alfred-py-3.0.6/alfred/dl/tf/common.py` & `alfred-py-3.0.7/alfred/dl/tf/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 def mute_tf():
     """
     this function will mute tensorflow
     disable tensorflow logging information
     call this before you import tensorflow
     """
-    os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+    os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/__init__.py` & `alfred-py-3.0.7/alfred/dl/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/torch/common.py` & `alfred-py-3.0.7/alfred/dl/torch/common.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/torch/distribute/utils.py` & `alfred-py-3.0.7/alfred/dl/torch/distribute/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 _LOCAL_PROCESS_GROUP = None
 """
 A torch process group which only includes processes that on the same machine as the current process.
 This variable is set when processes are spawned by `launch()` in "engine/launch.py".
 """
 
+
 # function ported from mmcv
 def get_dist_info():
-    if torch.__version__ < '1.0':
+    if torch.__version__ < "1.0":
         initialized = dist._initialized
     else:
         if dist.is_available():
             initialized = dist.is_initialized()
         else:
             initialized = False
     if initialized:
@@ -111,19 +112,19 @@
 
 def _serialize_to_tensor(data, group):
     backend = dist.get_backend(group)
     assert backend in ["gloo", "nccl"]
     device = torch.device("cpu" if backend == "gloo" else "cuda")
 
     buffer = pickle.dumps(data)
-    if len(buffer) > 1024 ** 3:
+    if len(buffer) > 1024**3:
         logger = logging.getLogger(__name__)
         logger.warning(
             "Rank {} trying to all-gather {:.2f} GB of data on device {}".format(
-                get_rank(), len(buffer) / (1024 ** 3), device
+                get_rank(), len(buffer) / (1024**3), device
             )
         )
     storage = torch.ByteStorage.from_buffer(buffer)
     tensor = torch.ByteTensor(storage).to(device=device)
     return tensor
 
 
@@ -135,25 +136,28 @@
     """
     world_size = dist.get_world_size(group=group)
     assert (
         world_size >= 1
     ), "comm.gather/all_gather must be called from ranks within the given group!"
     local_size = torch.tensor([tensor.numel()], dtype=torch.int64, device=tensor.device)
     size_list = [
-        torch.zeros([1], dtype=torch.int64, device=tensor.device) for _ in range(world_size)
+        torch.zeros([1], dtype=torch.int64, device=tensor.device)
+        for _ in range(world_size)
     ]
     dist.all_gather(size_list, local_size, group=group)
     size_list = [int(size.item()) for size in size_list]
 
     max_size = max(size_list)
 
     # we pad the tensor because torch all_gather does not support
     # gathering tensors of different shapes
     if local_size != max_size:
-        padding = torch.zeros((max_size - local_size,), dtype=torch.uint8, device=tensor.device)
+        padding = torch.zeros(
+            (max_size - local_size,), dtype=torch.uint8, device=tensor.device
+        )
         tensor = torch.cat((tensor, padding), dim=0)
     return size_list, tensor
 
 
 def all_gather(data, group=None):
     """
     Run all_gather on arbitrary picklable data (not necessarily tensors).
@@ -176,15 +180,16 @@
     tensor = _serialize_to_tensor(data, group)
 
     size_list, tensor = _pad_to_largest_tensor(tensor, group)
     max_size = max(size_list)
 
     # receiving Tensor from all ranks
     tensor_list = [
-        torch.empty((max_size,), dtype=torch.uint8, device=tensor.device) for _ in size_list
+        torch.empty((max_size,), dtype=torch.uint8, device=tensor.device)
+        for _ in size_list
     ]
     dist.all_gather(tensor_list, tensor, group=group)
 
     data_list = []
     for size, tensor in zip(size_list, tensor_list):
         buffer = tensor.cpu().numpy().tobytes()[:size]
         data_list.append(pickle.loads(buffer))
@@ -217,15 +222,16 @@
     tensor = _serialize_to_tensor(data, group)
     size_list, tensor = _pad_to_largest_tensor(tensor, group)
 
     # receiving Tensor from all ranks
     if rank == dst:
         max_size = max(size_list)
         tensor_list = [
-            torch.empty((max_size,), dtype=torch.uint8, device=tensor.device) for _ in size_list
+            torch.empty((max_size,), dtype=torch.uint8, device=tensor.device)
+            for _ in size_list
         ]
         dist.gather(tensor, tensor_list, dst=dst, group=group)
 
         data_list = []
         for size, tensor in zip(size_list, tensor_list):
             buffer = tensor.cpu().numpy().tobytes()[:size]
             data_list.append(pickle.loads(buffer))
@@ -240,15 +246,15 @@
     Returns:
         int: a random number that is the same across all workers.
             If workers need a shared RNG, they can use this shared seed to
             create one.
 
     All workers must call this function, otherwise it will deadlock.
     """
-    ints = np.random.randint(2 ** 31)
+    ints = np.random.randint(2**31)
     all_ints = all_gather(ints)
     return all_ints[0]
 
 
 def reduce_dict(input_dict, average=True):
     """
     Reduce the values in the dictionary from all processes so that process with rank
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/env.py` & `alfred-py-3.0.7/alfred/dl/torch/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,12 +95,16 @@
     Load custom environment setup by importing a Python source file or a
     module, and run the setup function.
     """
     if custom_module.endswith(".py"):
         module = _import_file("dl_lib.utils.env.custom_module", custom_module)
     else:
         module = importlib.import_module(custom_module)
-    assert hasattr(module, "setup_environment") and callable(module.setup_environment), (
+    assert hasattr(module, "setup_environment") and callable(
+        module.setup_environment
+    ), (
         "Custom environment module defined in {} does not have the "
         "required callable attribute 'setup_environment'."
-    ).format(custom_module)
+    ).format(
+        custom_module
+    )
     module.setup_environment()
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/gpu.py` & `alfred-py-3.0.7/alfred/dl/torch/gpu.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 
 def get_gpu_prop(show=True):
     ngpus = torch.cuda.device_count()
 
     properties = []
     for dev in range(ngpus):
         prop = torch.cuda.get_device_properties(dev)
-        properties.append({
-            "name": prop.name,
-            "capability": [prop.major, prop.minor],
-            # unit GB
-            "total_momory": round(prop.total_memory / 1073741824, 2),
-            "sm_count": prop.multi_processor_count
-        })
+        properties.append(
+            {
+                "name": prop.name,
+                "capability": [prop.major, prop.minor],
+                # unit GB
+                "total_momory": round(prop.total_memory / 1073741824, 2),
+                "sm_count": prop.multi_processor_count,
+            }
+        )
 
     if show:
         print("cuda: {}".format(torch.cuda.is_available()))
         print("available GPU(s): {}".format(ngpus))
         for i, p in enumerate(properties):
             print("{}: {}".format(i, p))
     return properties
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/metrics.py` & `alfred-py-3.0.7/alfred/dl/torch/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 import torch.nn.functional as F
 from torch import nn
 
 
 class Scalar(nn.Module):
     def __init__(self):
         super().__init__()
-        self.register_buffer('total', torch.FloatTensor([0.0]))
-        self.register_buffer('count', torch.FloatTensor([0.0]))
+        self.register_buffer("total", torch.FloatTensor([0.0]))
+        self.register_buffer("count", torch.FloatTensor([0.0]))
 
     def forward(self, scalar):
         if not scalar.eq(0.0):
             self.count += 1
             self.total += scalar.data.float()
         return self.value.cpu()
 
@@ -43,37 +43,38 @@
     def value(self):
         return self.total / self.count
 
     def clear(self):
         self.total.zero_()
         self.count.zero_()
 
+
 class Accuracy(nn.Module):
-    def __init__(self,
-                 dim=1,
-                 ignore_idx=-1,
-                 threshold=0.5,
-                 encode_background_as_zeros=True):
+    def __init__(
+        self, dim=1, ignore_idx=-1, threshold=0.5, encode_background_as_zeros=True
+    ):
         super().__init__()
-        self.register_buffer('total', torch.FloatTensor([0.0]))
-        self.register_buffer('count', torch.FloatTensor([0.0]))
+        self.register_buffer("total", torch.FloatTensor([0.0]))
+        self.register_buffer("count", torch.FloatTensor([0.0]))
         self._ignore_idx = ignore_idx
         self._dim = dim
         self._threshold = threshold
         self._encode_background_as_zeros = encode_background_as_zeros
 
     def forward(self, labels, preds, weights=None):
         # labels: [N, ...]
         # preds: [N, C, ...]
         if self._encode_background_as_zeros:
             scores = torch.sigmoid(preds)
             labels_pred = torch.max(preds, dim=self._dim)[1] + 1
-            pred_labels = torch.where((scores > self._threshold).any(self._dim),
-                                      labels_pred,
-                                      torch.tensor(0).type_as(labels_pred))
+            pred_labels = torch.where(
+                (scores > self._threshold).any(self._dim),
+                labels_pred,
+                torch.tensor(0).type_as(labels_pred),
+            )
         else:
             pred_labels = torch.max(preds, dim=self._dim)[1]
         N, *Ds = labels.shape
         labels = labels.view(N, int(np.prod(Ds)))
         pred_labels = pred_labels.view(N, int(np.prod(Ds)))
         if weights is None:
             weights = (labels != self._ignore_idx).float()
@@ -83,41 +84,42 @@
         num_examples = torch.sum(weights)
         num_examples = torch.clamp(num_examples, min=1.0).float()
         total = torch.sum((pred_labels == labels.long()).float())
         self.count += num_examples
         self.total += total
         return self.value.cpu()
         # return (total /  num_examples.data).cpu()
+
     @property
     def value(self):
         return self.total / self.count
 
     def clear(self):
         self.total.zero_()
         self.count.zero_()
 
 
 class Precision(nn.Module):
     def __init__(self, dim=1, ignore_idx=-1, threshold=0.5):
         super().__init__()
-        self.register_buffer('total', torch.FloatTensor([0.0]))
-        self.register_buffer('count', torch.FloatTensor([0.0]))
+        self.register_buffer("total", torch.FloatTensor([0.0]))
+        self.register_buffer("count", torch.FloatTensor([0.0]))
         self._ignore_idx = ignore_idx
         self._dim = dim
         self._threshold = threshold
 
     def forward(self, labels, preds, weights=None):
         # labels: [N, ...]
         # preds: [N, C, ...]
         if preds.shape[self._dim] == 1:  # BCE
-            pred_labels = (torch.sigmoid(preds) >
-                           self._threshold).long().squeeze(self._dim)
+            pred_labels = (
+                (torch.sigmoid(preds) > self._threshold).long().squeeze(self._dim)
+            )
         else:
-            assert preds.shape[
-                self._dim] == 2, "precision only support 2 class"
+            assert preds.shape[self._dim] == 2, "precision only support 2 class"
             pred_labels = torch.max(preds, dim=self._dim)[1]
         N, *Ds = labels.shape
         labels = labels.view(N, int(np.prod(Ds)))
         pred_labels = pred_labels.view(N, int(np.prod(Ds)))
         if weights is None:
             weights = (labels != self._ignore_idx).float()
         else:
@@ -134,40 +136,42 @@
         count = true_positives + false_positives
         # print(count, true_positives)
         if count > 0:
             self.count += count
             self.total += true_positives
         return self.value.cpu()
         # return (total /  num_examples.data).cpu()
+
     @property
     def value(self):
         return self.total / self.count
+
     def clear(self):
         self.total.zero_()
         self.count.zero_()
 
 
 class Recall(nn.Module):
     def __init__(self, dim=1, ignore_idx=-1, threshold=0.5):
         super().__init__()
-        self.register_buffer('total', torch.FloatTensor([0.0]))
-        self.register_buffer('count', torch.FloatTensor([0.0]))
+        self.register_buffer("total", torch.FloatTensor([0.0]))
+        self.register_buffer("count", torch.FloatTensor([0.0]))
         self._ignore_idx = ignore_idx
         self._dim = dim
         self._threshold = threshold
 
     def forward(self, labels, preds, weights=None):
         # labels: [N, ...]
         # preds: [N, C, ...]
         if preds.shape[self._dim] == 1:  # BCE
-            pred_labels = (torch.sigmoid(preds) >
-                           self._threshold).long().squeeze(self._dim)
+            pred_labels = (
+                (torch.sigmoid(preds) > self._threshold).long().squeeze(self._dim)
+            )
         else:
-            assert preds.shape[
-                self._dim] == 2, "precision only support 2 class"
+            assert preds.shape[self._dim] == 2, "precision only support 2 class"
             pred_labels = torch.max(preds, dim=self._dim)[1]
         N, *Ds = labels.shape
         labels = labels.view(N, int(np.prod(Ds)))
         pred_labels = pred_labels.view(N, int(np.prod(Ds)))
         if weights is None:
             weights = (labels != self._ignore_idx).float()
         else:
@@ -182,28 +186,25 @@
         false_negatives = (weights * (trues & pred_falses).float()).sum()
         count = true_positives + false_negatives
         if count > 0:
             self.count += count
             self.total += true_positives
         return self.value.cpu()
         # return (total /  num_examples.data).cpu()
+
     @property
     def value(self):
         return self.total / self.count
+
     def clear(self):
         self.total.zero_()
         self.count.zero_()
 
 
-def _calc_binary_metrics(labels,
-                         scores,
-                         weights=None,
-                         ignore_idx=-1,
-                         threshold=0.5):
-
+def _calc_binary_metrics(labels, scores, weights=None, ignore_idx=-1, threshold=0.5):
     pred_labels = (scores > threshold).long()
     N, *Ds = labels.shape
     labels = labels.view(N, int(np.prod(Ds)))
     pred_labels = pred_labels.view(N, int(np.prod(Ds)))
     pred_trues = pred_labels > 0
     pred_falses = pred_labels == 0
     trues = labels > 0
@@ -212,32 +213,30 @@
     true_negatives = (weights * (falses & pred_falses).float()).sum()
     false_positives = (weights * (falses & pred_trues).float()).sum()
     false_negatives = (weights * (trues & pred_falses).float()).sum()
     return true_positives, true_negatives, false_positives, false_negatives
 
 
 class PrecisionRecall(nn.Module):
-    def __init__(self,
-                 dim=1,
-                 ignore_idx=-1,
-                 thresholds=0.5,
-                 use_sigmoid_score=False,
-                 encode_background_as_zeros=True):
+    def __init__(
+        self,
+        dim=1,
+        ignore_idx=-1,
+        thresholds=0.5,
+        use_sigmoid_score=False,
+        encode_background_as_zeros=True,
+    ):
         super().__init__()
         if not isinstance(thresholds, (list, tuple)):
             thresholds = [thresholds]
 
-        self.register_buffer('prec_total',
-                             torch.FloatTensor(len(thresholds)).zero_())
-        self.register_buffer('prec_count',
-                             torch.FloatTensor(len(thresholds)).zero_())
-        self.register_buffer('rec_total',
-                             torch.FloatTensor(len(thresholds)).zero_())
-        self.register_buffer('rec_count',
-                             torch.FloatTensor(len(thresholds)).zero_())
+        self.register_buffer("prec_total", torch.FloatTensor(len(thresholds)).zero_())
+        self.register_buffer("prec_count", torch.FloatTensor(len(thresholds)).zero_())
+        self.register_buffer("rec_total", torch.FloatTensor(len(thresholds)).zero_())
+        self.register_buffer("rec_count", torch.FloatTensor(len(thresholds)).zero_())
 
         self._ignore_idx = ignore_idx
         self._dim = dim
         self._thresholds = thresholds
         self._use_sigmoid_score = use_sigmoid_score
         self._encode_background_as_zeros = encode_background_as_zeros
 
@@ -269,33 +268,37 @@
         """
         scores = torch.max(total_scores, dim=-1)[0]
         if weights is None:
             weights = (labels != self._ignore_idx).float()
         else:
             weights = weights.float()
         for i, thresh in enumerate(self._thresholds):
-            tp, tn, fp, fn = _calc_binary_metrics(labels, scores, weights,
-                                                  self._ignore_idx, thresh)
+            tp, tn, fp, fn = _calc_binary_metrics(
+                labels, scores, weights, self._ignore_idx, thresh
+            )
             rec_count = tp + fn
             prec_count = tp + fp
             if rec_count > 0:
                 self.rec_count[i] += rec_count
                 self.rec_total[i] += tp
             if prec_count > 0:
                 self.prec_count[i] += prec_count
                 self.prec_total[i] += tp
 
         return self.value
         # return (total /  num_examples.data).cpu()
+
     @property
     def value(self):
         prec_count = torch.clamp(self.prec_count, min=1.0)
         rec_count = torch.clamp(self.rec_count, min=1.0)
-        return ((self.prec_total / prec_count).cpu(),
-                (self.rec_total / rec_count).cpu())
+        return (
+            (self.prec_total / prec_count).cpu(),
+            (self.rec_total / rec_count).cpu(),
+        )
 
     @property
     def thresholds(self):
         return self._thresholds
 
     def clear(self):
         self.rec_count.zero_()
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/model_summary.py` & `alfred-py-3.0.7/alfred/dl/torch/model_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             module_idx = len(summary)
 
             m_key = "%s-%i" % (class_name, module_idx + 1)
             summary[m_key] = OrderedDict()
             try:
                 summary[m_key]["input_shape"] = list(input[0].size())
             except Exception as e:
-                print('error when fetching input shape: ', e)
+                print("error when fetching input shape: ", e)
                 summary[m_key]["input_shape"] = [2, -1, -1]
             summary[m_key]["input_shape"][0] = batch_size
             if isinstance(output, (list, tuple)):
                 summary[m_key]["output_shape"] = [
                     [-1] + list(o.size())[1:] for o in output
                 ]
             else:
@@ -62,17 +62,17 @@
                 params += torch.prod(torch.LongTensor(list(module.weight.size())))
                 summary[m_key]["trainable"] = module.weight.requires_grad
             if hasattr(module, "bias") and hasattr(module.bias, "size"):
                 params += torch.prod(torch.LongTensor(list(module.bias.size())))
             summary[m_key]["nb_params"] = params
 
         if (
-                not isinstance(module, nn.Sequential)
-                and not isinstance(module, nn.ModuleList)
-                and not (module == model)
+            not isinstance(module, nn.Sequential)
+            and not isinstance(module, nn.ModuleList)
+            and not (module == model)
         ):
             hooks.append(module.register_forward_hook(hook))
 
     device = device.lower()
     assert device in [
         "cuda",
         "cpu",
@@ -80,38 +80,46 @@
 
     if device == "cuda" and torch.cuda.is_available():
         dtype = torch.cuda.FloatTensor
     else:
         dtype = torch.FloatTensor
 
     # multiple inputs to the network
-    if isinstance(input_size, tuple) or isinstance(input_size, list) and input_size[0] <= 3:
+    if (
+        isinstance(input_size, tuple)
+        or isinstance(input_size, list)
+        and input_size[0] <= 3
+    ):
         # batch_size of 2 for batchnorm
         x = torch.rand(2, *input_size).type(dtype)
     else:
         x = torch.rand(2, *input_size).type(dtype)
-        print('[WARNING] channel more than 3, this may cause some errors. or you does not put channel as first dim.')
+        print(
+            "[WARNING] channel more than 3, this may cause some errors. or you does not put channel as first dim."
+        )
         # print('Wrong! you should send input size specific without batch size, etc: (3, 64, 64), channel first.')
         # exit(0)
     # create properties
     summary = OrderedDict()
     hooks = []
 
     # register hook
     model.apply(register_hook)
 
     # make a forward pass
     try:
-        print('[INFO] fake data input: ', x.size())
+        print("[INFO] fake data input: ", x.size())
         model(x)
     except Exception as e:
-        print('[ERROR] summary failed. error: {}'.format(e))
-        print('[TIPS] make sure your called model.to(device) ')
-        print('also possibly error is input size should specific without batch, and using channel first, etc: (3, 128, 128)')
-        print('full trace back: ', e.with_traceback(0))
+        print("[ERROR] summary failed. error: {}".format(e))
+        print("[TIPS] make sure your called model.to(device) ")
+        print(
+            "also possibly error is input size should specific without batch, and using channel first, etc: (3, 128, 128)"
+        )
+        print("full trace back: ", e.with_traceback(0))
         exit(0)
 
     # remove these hooks
     for h in hooks:
         h.remove()
 
     print("----------------------------------------------------------------")
@@ -132,17 +140,19 @@
         total_output += np.prod(summary[layer]["output_shape"])
         if "trainable" in summary[layer]:
             if summary[layer]["trainable"] == True:
                 trainable_params += summary[layer]["nb_params"]
         print(line_new)
 
     # assume 4 bytes/number (float on cuda).
-    total_input_size = abs(np.prod(input_size) * batch_size * 4. / (1024 ** 2.))
-    total_output_size = abs(2. * total_output * 4. / (1024 ** 2.))  # x2 for gradients
-    total_params_size = abs(total_params.numpy() * 4. / (1024 ** 2.))
+    total_input_size = abs(np.prod(input_size) * batch_size * 4.0 / (1024**2.0))
+    total_output_size = abs(
+        2.0 * total_output * 4.0 / (1024**2.0)
+    )  # x2 for gradients
+    total_params_size = abs(total_params.numpy() * 4.0 / (1024**2.0))
     total_size = total_params_size + total_output_size + total_input_size
 
     print("================================================================")
     print("Total params: {0:,}".format(total_params))
     print("Trainable params: {0:,}".format(trainable_params))
     print("Non-trainable params: {0:,}".format(total_params - trainable_params))
     print("----------------------------------------------------------------")
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/__init__.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/functional.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,14 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import torch
 
+
 def one_hot(tensor, depth, dim=-1, on_value=1.0, dtype=torch.float32):
     tensor_onehot = torch.zeros(
-        *list(tensor.shape), depth, dtype=dtype, device=tensor.device)
+        *list(tensor.shape), depth, dtype=dtype, device=tensor.device
+    )
     tensor_onehot.scatter_(dim, tensor.unsqueeze(dim).long(), on_value)
     return tensor_onehot
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/modules/__init__.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/modules/common.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/modules/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 #
 import sys
 from collections import OrderedDict
 
 import torch
 from torch.nn import functional as F
 
+
 class Empty(torch.nn.Module):
     def __init__(self, *args, **kwargs):
         super(Empty, self).__init__()
 
     def forward(self, *args, **kwargs):
         if len(args) == 1:
             return args[0]
         elif len(args) == 0:
             return None
         return args
 
+
 class Sequential(torch.nn.Module):
     r"""A sequential container.
     Modules will be added to it in the order they are passed in the constructor.
     Alternatively, an ordered dict of modules can also be passed in.
 
     To make it easier to understand, given is a small example::
 
@@ -56,15 +58,15 @@
         # Example of using Sequential with OrderedDict
         model = Sequential(OrderedDict([
                   ('conv1', nn.Conv2d(1,20,5)),
                   ('relu1', nn.ReLU()),
                   ('conv2', nn.Conv2d(20,64,5)),
                   ('relu2', nn.ReLU())
                 ]))
-        
+
         # Example of using Sequential with kwargs(python 3.6+)
         model = Sequential(
                   conv1=nn.Conv2d(1,20,5),
                   relu1=nn.ReLU(),
                   conv2=nn.Conv2d(20,64,5),
                   relu2=nn.ReLU()
                 )
@@ -83,15 +85,15 @@
                 raise ValueError("kwargs only supported in py36+")
             if name in self._modules:
                 raise ValueError("name exists.")
             self.add_module(name, module)
 
     def __getitem__(self, idx):
         if not (-len(self) <= idx < len(self)):
-            raise IndexError('index {} is out of range'.format(idx))
+            raise IndexError("index {} is out of range".format(idx))
         if idx < 0:
             idx += len(self)
         it = iter(self._modules.values())
         for i in range(idx):
             next(it)
         return next(it)
 
@@ -107,8 +109,8 @@
 
     def forward(self, input):
         # i = 0
         for module in self._modules.values():
             # print(i)
             input = module(input)
             # i += 1
-        return input
+        return input
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/modules/normalization.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/modules/normalization.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,11 +23,9 @@
 #
 import torch
 
 
 class GroupNorm(torch.nn.GroupNorm):
     def __init__(self, num_channels, num_groups, eps=1e-5, affine=True):
         super().__init__(
-            num_groups=num_groups,
-            num_channels=num_channels,
-            eps=eps,
-            affine=affine)
+            num_groups=num_groups, num_channels=num_channels, eps=eps, affine=affine
+        )
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/nn/weights_init.py` & `alfred-py-3.0.7/alfred/dl/torch/nn/weights_init.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # Copyright (c) Open-MMLab. All rights reserved.
 import torch.nn as nn
 
 
 def constant_init(module, val, bias=0):
-    if hasattr(module, 'weight') and module.weight is not None:
+    if hasattr(module, "weight") and module.weight is not None:
         nn.init.constant_(module.weight, val)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
-def xavier_init(module, gain=1, bias=0, distribution='normal'):
-    assert distribution in ['uniform', 'normal']
-    if distribution == 'uniform':
+def xavier_init(module, gain=1, bias=0, distribution="normal"):
+    assert distribution in ["uniform", "normal"]
+    if distribution == "uniform":
         nn.init.xavier_uniform_(module.weight, gain=gain)
     else:
         nn.init.xavier_normal_(module.weight, gain=gain)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 def normal_init(module, mean=0, std=1, bias=0):
     nn.init.normal_(module.weight, mean, std)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 def uniform_init(module, a=0, b=1, bias=0):
     nn.init.uniform_(module.weight, a, b)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
-def kaiming_init(module,
-                 a=0,
-                 mode='fan_out',
-                 nonlinearity='relu',
-                 bias=0,
-                 distribution='normal'):
-    assert distribution in ['uniform', 'normal']
-    if distribution == 'uniform':
+def kaiming_init(
+    module, a=0, mode="fan_out", nonlinearity="relu", bias=0, distribution="normal"
+):
+    assert distribution in ["uniform", "normal"]
+    if distribution == "uniform":
         nn.init.kaiming_uniform_(
-            module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
+            module.weight, a=a, mode=mode, nonlinearity=nonlinearity
+        )
     else:
         nn.init.kaiming_normal_(
-            module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
-    if hasattr(module, 'bias') and module.bias is not None:
+            module.weight, a=a, mode=mode, nonlinearity=nonlinearity
+        )
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 def caffe2_xavier_init(module, bias=0):
     # `XavierFill` in Caffe2 corresponds to `kaiming_uniform_` in PyTorch
     # Acknowledgment to FAIR's internal code
     kaiming_init(
-        module,
-        a=1,
-        mode='fan_in',
-        nonlinearity='leaky_relu',
-        distribution='uniform')
+        module, a=1, mode="fan_in", nonlinearity="leaky_relu", distribution="uniform"
+    )
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/ops/__init__.py` & `alfred-py-3.0.7/alfred/dl/torch/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/dl/torch/ops/array_ops.py` & `alfred-py-3.0.7/alfred/dl/torch/ops/array_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     """pytorch edition of tensorflow scatter_nd.
     this function don't contain except handle code. so use this carefully
     when indice repeats, don't support repeat add which is supported
     in tensorflow.
     """
     ret = torch.zeros(*shape, dtype=updates.dtype, device=updates.device)
     ndim = indices.shape[-1]
-    output_shape = list(indices.shape[:-1]) + shape[indices.shape[-1]:]
+    output_shape = list(indices.shape[:-1]) + shape[indices.shape[-1] :]
     flatted_indices = indices.view(-1, ndim)
     slices = [flatted_indices[:, i] for i in range(ndim)]
     slices += [Ellipsis]
     ret[slices] = updates.view(*output_shape)
     return ret
 
 
 def gather_nd(params, indices):
     # this function has a limit that MAX_ADVINDEX_CALC_DIMS=5
     ndim = indices.shape[-1]
-    output_shape = list(indices.shape[:-1]) + list(params.shape[indices.shape[-1]:])
+    output_shape = list(indices.shape[:-1]) + list(params.shape[indices.shape[-1] :])
     flatted_indices = indices.view(-1, ndim)
     slices = [flatted_indices[:, i] for i in range(ndim)]
     slices += [Ellipsis]
     return params[slices].view(*output_shape)
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/runner/checkpoint.py` & `alfred-py-3.0.7/alfred/dl/torch/runner/checkpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 import torchvision
 from torch.utils import model_zoo
 
 from ..distribute.utils import get_dist_info
 
 
 open_mmlab_model_urls = {
-    'vgg16_caffe': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/vgg16_caffe-292e1171.pth',  # noqa: E501
-    'resnet50_caffe': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_caffe-788b5fa3.pth',  # noqa: E501
-    'resnet101_caffe': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_caffe-3ad79236.pth',  # noqa: E501
-    'resnext50_32x4d': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50-32x4d-0ab1a123.pth',  # noqa: E501
-    'resnext101_32x4d': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d-a5af3160.pth',  # noqa: E501
-    'resnext101_64x4d': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_64x4d-ee2c6f71.pth',  # noqa: E501
-    'contrib/resnet50_gn': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn_thangvubk-ad1730dd.pth',  # noqa: E501
-    'detectron/resnet50_gn': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn-9186a21c.pth',  # noqa: E501
-    'detectron/resnet101_gn': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_gn-cac0ab98.pth',  # noqa: E501
-    'jhu/resnet50_gn_ws': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn_ws-15beedd8.pth',  # noqa: E501
-    'jhu/resnet101_gn_ws': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_gn_ws-3e3c308c.pth',  # noqa: E501
-    'jhu/resnext50_32x4d_gn_ws': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50_32x4d_gn_ws-0d87ac85.pth',  # noqa: E501
-    'jhu/resnext101_32x4d_gn_ws': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d_gn_ws-34ac1a9e.pth',  # noqa: E501
-    'jhu/resnext50_32x4d_gn': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50_32x4d_gn-c7e8b754.pth',  # noqa: E501
-    'jhu/resnext101_32x4d_gn': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d_gn-ac3bb84e.pth',  # noqa: E501
-    'msra/hrnetv2_w18': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w18-00eb2006.pth',  # noqa: E501
-    'msra/hrnetv2_w32': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w32-dc9eeb4f.pth',  # noqa: E501
-    'msra/hrnetv2_w40': 'https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w40-ed0b031c.pth',  # noqa: E501
-    'bninception_caffe': 'https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/bn_inception_caffe-ed2e8665.pth',  # noqa: E501
-    'kin400/i3d_r50_f32s2_k400': 'https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/i3d_r50_f32s2_k400-2c57e077.pth',  # noqa: E501
-    'kin400/nl3d_r50_f32s2_k400': 'https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/nl3d_r50_f32s2_k400-fa7e7caa.pth',  # noqa: E501
+    "vgg16_caffe": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/vgg16_caffe-292e1171.pth",  # noqa: E501
+    "resnet50_caffe": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_caffe-788b5fa3.pth",  # noqa: E501
+    "resnet101_caffe": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_caffe-3ad79236.pth",  # noqa: E501
+    "resnext50_32x4d": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50-32x4d-0ab1a123.pth",  # noqa: E501
+    "resnext101_32x4d": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d-a5af3160.pth",  # noqa: E501
+    "resnext101_64x4d": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_64x4d-ee2c6f71.pth",  # noqa: E501
+    "contrib/resnet50_gn": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn_thangvubk-ad1730dd.pth",  # noqa: E501
+    "detectron/resnet50_gn": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn-9186a21c.pth",  # noqa: E501
+    "detectron/resnet101_gn": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_gn-cac0ab98.pth",  # noqa: E501
+    "jhu/resnet50_gn_ws": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet50_gn_ws-15beedd8.pth",  # noqa: E501
+    "jhu/resnet101_gn_ws": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnet101_gn_ws-3e3c308c.pth",  # noqa: E501
+    "jhu/resnext50_32x4d_gn_ws": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50_32x4d_gn_ws-0d87ac85.pth",  # noqa: E501
+    "jhu/resnext101_32x4d_gn_ws": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d_gn_ws-34ac1a9e.pth",  # noqa: E501
+    "jhu/resnext50_32x4d_gn": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext50_32x4d_gn-c7e8b754.pth",  # noqa: E501
+    "jhu/resnext101_32x4d_gn": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/resnext101_32x4d_gn-ac3bb84e.pth",  # noqa: E501
+    "msra/hrnetv2_w18": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w18-00eb2006.pth",  # noqa: E501
+    "msra/hrnetv2_w32": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w32-dc9eeb4f.pth",  # noqa: E501
+    "msra/hrnetv2_w40": "https://s3.ap-northeast-2.amazonaws.com/open-mmlab/pretrain/third_party/hrnetv2_w40-ed0b031c.pth",  # noqa: E501
+    "bninception_caffe": "https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/bn_inception_caffe-ed2e8665.pth",  # noqa: E501
+    "kin400/i3d_r50_f32s2_k400": "https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/i3d_r50_f32s2_k400-2c57e077.pth",  # noqa: E501
+    "kin400/nl3d_r50_f32s2_k400": "https://open-mmlab.s3.ap-northeast-2.amazonaws.com/pretrain/third_party/nl3d_r50_f32s2_k400-fa7e7caa.pth",  # noqa: E501
 }  # yapf: disable
 
 
 def load_state_dict(module, state_dict, strict=False, logger=None):
     """Load state_dict to a module.
 
     This method is modified from :meth:`torch.nn.Module.load_state_dict`.
@@ -55,80 +55,86 @@
         logger (:obj:`logging.Logger`, optional): Logger to log the error
             message. If not specified, print function will be used.
     """
     unexpected_keys = []
     all_missing_keys = []
     err_msg = []
 
-    metadata = getattr(state_dict, '_metadata', None)
+    metadata = getattr(state_dict, "_metadata", None)
     state_dict = state_dict.copy()
     if metadata is not None:
         state_dict._metadata = metadata
 
     # use _load_from_state_dict to enable checkpoint version control
-    def load(module, prefix=''):
-        local_metadata = {} if metadata is None else metadata.get(
-            prefix[:-1], {})
-        module._load_from_state_dict(state_dict, prefix, local_metadata, True,
-                                     all_missing_keys, unexpected_keys,
-                                     err_msg)
+    def load(module, prefix=""):
+        local_metadata = {} if metadata is None else metadata.get(prefix[:-1], {})
+        module._load_from_state_dict(
+            state_dict,
+            prefix,
+            local_metadata,
+            True,
+            all_missing_keys,
+            unexpected_keys,
+            err_msg,
+        )
         for name, child in module._modules.items():
             if child is not None:
-                load(child, prefix + name + '.')
+                load(child, prefix + name + ".")
 
     load(module)
     load = None  # break load->load reference cycle
 
     # ignore "num_batches_tracked" of BN layers
-    missing_keys = [
-        key for key in all_missing_keys if 'num_batches_tracked' not in key
-    ]
+    missing_keys = [key for key in all_missing_keys if "num_batches_tracked" not in key]
 
     if unexpected_keys:
-        err_msg.append('unexpected key in source state_dict: {}\n'.format(
-            ', '.join(unexpected_keys)))
+        err_msg.append(
+            "unexpected key in source state_dict: {}\n".format(
+                ", ".join(unexpected_keys)
+            )
+        )
     if missing_keys:
-        err_msg.append('missing keys in source state_dict: {}\n'.format(
-            ', '.join(missing_keys)))
+        err_msg.append(
+            "missing keys in source state_dict: {}\n".format(", ".join(missing_keys))
+        )
 
     rank, _ = get_dist_info()
     if len(err_msg) > 0 and rank == 0:
-        err_msg.insert(
-            0, 'The model and loaded state dict do not match exactly\n')
-        err_msg = '\n'.join(err_msg)
+        err_msg.insert(0, "The model and loaded state dict do not match exactly\n")
+        err_msg = "\n".join(err_msg)
         if strict:
             raise RuntimeError(err_msg)
         elif logger is not None:
             logger.warning(err_msg)
         else:
             print(err_msg)
 
 
 def load_url_dist(url):
-    """ In distributed setting, this function only download checkpoint at
-    local rank 0 """
+    """In distributed setting, this function only download checkpoint at
+    local rank 0"""
     rank, world_size = get_dist_info()
-    rank = int(os.environ.get('LOCAL_RANK', rank))
+    rank = int(os.environ.get("LOCAL_RANK", rank))
     if rank == 0:
         checkpoint = model_zoo.load_url(url)
     if world_size > 1:
         torch.distributed.barrier()
         if rank > 0:
             checkpoint = model_zoo.load_url(url)
     return checkpoint
 
 
 def get_torchvision_models():
     model_urls = dict()
     for _, name, ispkg in pkgutil.walk_packages(torchvision.models.__path__):
         if ispkg:
             continue
-        _zoo = import_module('torchvision.models.{}'.format(name))
-        if hasattr(_zoo, 'model_urls'):
-            _urls = getattr(_zoo, 'model_urls')
+        _zoo = import_module("torchvision.models.{}".format(name))
+        if hasattr(_zoo, "model_urls"):
+            _urls = getattr(_zoo, "model_urls")
             model_urls.update(_urls)
     return model_urls
 
 
 def _load_checkpoint(filename, map_location=None):
     """Load checkpoint from somewhere (modelzoo, file, url).
 
@@ -137,41 +143,39 @@
         map_location (str | None): Same as :func:`torch.load`. Default: None.
 
     Returns:
         dict | OrderedDict: The loaded checkpoint. It can be either an
             OrderedDict storing model weights or a dict containing other
             information, which depends on the checkpoint.
     """
-    if filename.startswith('modelzoo://'):
-        warnings.warn('The URL scheme of "modelzoo://" is deprecated, please '
-                      'use "torchvision://" instead')
+    if filename.startswith("modelzoo://"):
+        warnings.warn(
+            'The URL scheme of "modelzoo://" is deprecated, please '
+            'use "torchvision://" instead'
+        )
         model_urls = get_torchvision_models()
         model_name = filename[11:]
         checkpoint = load_url_dist(model_urls[model_name])
-    elif filename.startswith('torchvision://'):
+    elif filename.startswith("torchvision://"):
         model_urls = get_torchvision_models()
         model_name = filename[14:]
         checkpoint = load_url_dist(model_urls[model_name])
-    elif filename.startswith('open-mmlab://'):
+    elif filename.startswith("open-mmlab://"):
         model_name = filename[13:]
         checkpoint = load_url_dist(open_mmlab_model_urls[model_name])
-    elif filename.startswith(('http://', 'https://')):
+    elif filename.startswith(("http://", "https://")):
         checkpoint = load_url_dist(filename)
     else:
         if not osp.isfile(filename):
-            raise IOError('{} is not a checkpoint file'.format(filename))
+            raise IOError("{} is not a checkpoint file".format(filename))
         checkpoint = torch.load(filename, map_location=map_location)
     return checkpoint
 
 
-def load_checkpoint(model,
-                    filename,
-                    map_location=None,
-                    strict=False,
-                    logger=None):
+def load_checkpoint(model, filename, map_location=None, strict=False, logger=None):
     """Load checkpoint from a file or URI.
 
     Args:
         model (Module): Module to load checkpoint.
         filename (str): Either a filepath or URL or modelzoo://xxxxxxx.
         map_location (str): Same as :func:`torch.load`.
         strict (bool): Whether to allow different params for the model and
@@ -181,24 +185,23 @@
     Returns:
         dict or OrderedDict: The loaded checkpoint.
     """
     checkpoint = _load_checkpoint(filename, map_location)
     # get state_dict from checkpoint
     if isinstance(checkpoint, OrderedDict):
         state_dict = checkpoint
-    elif isinstance(checkpoint, dict) and 'state_dict' in checkpoint:
-        state_dict = checkpoint['state_dict']
+    elif isinstance(checkpoint, dict) and "state_dict" in checkpoint:
+        state_dict = checkpoint["state_dict"]
     else:
-        raise RuntimeError(
-            'No state_dict found in checkpoint file {}'.format(filename))
+        raise RuntimeError("No state_dict found in checkpoint file {}".format(filename))
     # strip prefix of state_dict
-    if list(state_dict.keys())[0].startswith('module.'):
-        state_dict = {k[7:]: v for k, v in checkpoint['state_dict'].items()}
+    if list(state_dict.keys())[0].startswith("module."):
+        state_dict = {k[7:]: v for k, v in checkpoint["state_dict"].items()}
     # load state_dict
-    if hasattr(model, 'module'):
+    if hasattr(model, "module"):
         load_state_dict(model.module, state_dict, strict, logger)
     else:
         load_state_dict(model, state_dict, strict, logger)
     return checkpoint
 
 
 def weights_to_cpu(state_dict):
@@ -209,8 +212,8 @@
 
     Returns:
         OrderedDict: Model weights on GPU.
     """
     state_dict_cpu = OrderedDict()
     for key, val in state_dict.items():
         state_dict_cpu[key] = val.cpu()
-    return state_dict_cpu
+    return state_dict_cpu
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/tools.py` & `alfred-py-3.0.7/alfred/dl/torch/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                         kw[key] = val
                 super().__init__(*args, **kw)
 
         return DefaultArgLayer
 
     return layer_wrapper
 
+
 def torch_to_np_dtype(ttype):
     type_map = {
         torch.float16: np.dtype(np.float16),
         torch.float32: np.dtype(np.float32),
         torch.float16: np.dtype(np.float64),
         torch.int32: np.dtype(np.int32),
         torch.int64: np.dtype(np.int64),
@@ -90,15 +91,15 @@
 
 
 def torch_load_state_dict_without_module(ckp_file):
     """
     this function using for load a model without module
     """
     checkpoint = torch.load(ckp_file)
-    state_dict =checkpoint['state_dict']
+    state_dict = checkpoint["state_dict"]
 
     new_state_dict = OrderedDict()
     for k, v in state_dict.items():
-        if 'module.' in k:
-            k = k[7:] # remove 'module.' of dataparallel
-        new_state_dict[k]=v
-    return new_state_dict
+        if "module." in k:
+            k = k[7:]  # remove 'module.' of dataparallel
+        new_state_dict[k] = v
+    return new_state_dict
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/__init__.py` & `alfred-py-3.0.7/alfred/dl/torch/train/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,13 +17,18 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from .checkpoint import (latest_checkpoint, restore,
-                         restore_latest_checkpoints,
-                         restore_models, save, save_models,
-                         try_restore_latest_checkpoints)
+from .checkpoint import (
+    latest_checkpoint,
+    restore,
+    restore_latest_checkpoints,
+    restore_models,
+    save,
+    save_models,
+    try_restore_latest_checkpoints,
+)
 from .common import create_folder
 from .optim import MixedPrecisionWrapper
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/checkpoint.py` & `alfred-py-3.0.7/alfred/dl/torch/train/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class DelayedKeyboardInterrupt(object):
     def __enter__(self):
         self.signal_received = False
         self.old_handler = signal.signal(signal.SIGINT, self.handler)
 
     def handler(self, sig, frame):
         self.signal_received = (sig, frame)
-        logging.debug('SIGINT received. Delaying KeyboardInterrupt.')
+        logging.debug("SIGINT received. Delaying KeyboardInterrupt.")
 
     def __exit__(self, type, value, traceback):
         signal.signal(signal.SIGINT, self.old_handler)
         if self.signal_received:
             self.old_handler(*self.signal_received)
 
 
@@ -53,88 +53,85 @@
         model_name: name of your model. we find ckpts by name
     Returns:
         path: None if isn't exist or latest checkpoint path.
     """
     ckpt_info_path = Path(model_dir) / "checkpoints.json"
     if not ckpt_info_path.is_file():
         return None
-    with open(ckpt_info_path, 'r') as f:
+    with open(ckpt_info_path, "r") as f:
         ckpt_dict = json.loads(f.read())
-    if model_name not in ckpt_dict['latest_ckpt']:
+    if model_name not in ckpt_dict["latest_ckpt"]:
         return None
-    latest_ckpt = ckpt_dict['latest_ckpt'][model_name]
+    latest_ckpt = ckpt_dict["latest_ckpt"][model_name]
     ckpt_file_name = Path(model_dir) / latest_ckpt
     if not ckpt_file_name.is_file():
         return None
-    
+
     return str(ckpt_file_name)
 
+
 def _ordered_unique(seq):
     seen = set()
     return [x for x in seq if not (x in seen or seen.add(x))]
 
-def save(model_dir,
-         model,
-         model_name,
-         global_step,
-         max_to_keep=8,
-         keep_latest=True):
+
+def save(model_dir, model, model_name, global_step, max_to_keep=8, keep_latest=True):
     """save a model into model_dir.
     Args:
         model_dir: string, indicate your model dir(save ckpts, summarys,
             logs, etc).
         model: torch.nn.Module instance.
         model_name: name of your model. we find ckpts by name
         global_step: int, indicate current global step.
         max_to_keep: int, maximum checkpoints to keep.
-        keep_latest: bool, if True and there are too much ckpts, 
+        keep_latest: bool, if True and there are too much ckpts,
             will delete oldest ckpt. else will delete ckpt which has
             smallest global step.
     Returns:
         path: None if isn't exist or latest checkpoint path.
     """
 
     # prevent save incomplete checkpoint due to key interrupt
     with DelayedKeyboardInterrupt():
         ckpt_info_path = Path(model_dir) / "checkpoints.json"
         ckpt_filename = "{}-{}.tckpt".format(model_name, global_step)
         ckpt_path = Path(model_dir) / ckpt_filename
         if not ckpt_info_path.is_file():
-            ckpt_info_dict = {'latest_ckpt': {}, 'all_ckpts': {}}
+            ckpt_info_dict = {"latest_ckpt": {}, "all_ckpts": {}}
         else:
-            with open(ckpt_info_path, 'r') as f:
+            with open(ckpt_info_path, "r") as f:
                 ckpt_info_dict = json.loads(f.read())
-        ckpt_info_dict['latest_ckpt'][model_name] = ckpt_filename
-        if model_name in ckpt_info_dict['all_ckpts']:
-            ckpt_info_dict['all_ckpts'][model_name].append(ckpt_filename)
+        ckpt_info_dict["latest_ckpt"][model_name] = ckpt_filename
+        if model_name in ckpt_info_dict["all_ckpts"]:
+            ckpt_info_dict["all_ckpts"][model_name].append(ckpt_filename)
         else:
-            ckpt_info_dict['all_ckpts'][model_name] = [ckpt_filename]
-        all_ckpts = ckpt_info_dict['all_ckpts'][model_name]
+            ckpt_info_dict["all_ckpts"][model_name] = [ckpt_filename]
+        all_ckpts = ckpt_info_dict["all_ckpts"][model_name]
 
         torch.save(model.state_dict(), ckpt_path)
         # check ckpt in all_ckpts is exist, if not, delete it from all_ckpts
         all_ckpts_checked = []
         for ckpt in all_ckpts:
             ckpt_path_uncheck = Path(model_dir) / ckpt
             if ckpt_path_uncheck.is_file():
                 all_ckpts_checked.append(str(ckpt_path_uncheck))
         all_ckpts = all_ckpts_checked
         if len(all_ckpts) > max_to_keep:
             if keep_latest:
                 ckpt_to_delete = all_ckpts.pop(0)
             else:
                 # delete smallest step
-                get_step = lambda name: int(name.split('.')[0].split('-')[1])
+                get_step = lambda name: int(name.split(".")[0].split("-")[1])
                 min_step = min([get_step(name) for name in all_ckpts])
                 ckpt_to_delete = "{}-{}.tckpt".format(model_name, min_step)
                 all_ckpts.remove(ckpt_to_delete)
             os.remove(str(Path(model_dir) / ckpt_to_delete))
         all_ckpts_filename = _ordered_unique([Path(f).name for f in all_ckpts])
-        ckpt_info_dict['all_ckpts'][model_name] = all_ckpts_filename
-        with open(ckpt_info_path, 'w') as f:
+        ckpt_info_dict["all_ckpts"][model_name] = all_ckpts_filename
+        with open(ckpt_info_path, "w") as f:
             f.write(json.dumps(ckpt_info_dict, indent=2))
 
 
 def restore(ckpt_path, model):
     if not Path(ckpt_path).is_file():
         raise ValueError("checkpoint {} not exist.".format(ckpt_path))
     model.load_state_dict(torch.load(ckpt_path))
@@ -144,16 +141,17 @@
 def _check_model_names(models):
     model_names = []
     for model in models:
         if not hasattr(model, "name"):
             raise ValueError("models must have name attr")
         model_names.append(model.name)
     if len(model_names) != len(set(model_names)):
-        raise ValueError("models must have unique name: {}".format(
-            ", ".join(model_names)))
+        raise ValueError(
+            "models must have unique name: {}".format(", ".join(model_names))
+        )
 
 
 def _get_name_to_model_map(models):
     if isinstance(models, dict):
         name_to_model = {name: m for name, m in models.items()}
     else:
         _check_model_names(models)
@@ -164,33 +162,31 @@
 def try_restore_latest_checkpoints(model_dir, models):
     name_to_model = _get_name_to_model_map(models)
     for name, model in name_to_model.items():
         latest_ckpt = latest_checkpoint(model_dir, name)
         if latest_ckpt is not None:
             restore(latest_ckpt, model)
 
+
 def restore_latest_checkpoints(model_dir, models):
     name_to_model = _get_name_to_model_map(models)
     for name, model in name_to_model.items():
         latest_ckpt = latest_checkpoint(model_dir, name)
         if latest_ckpt is not None:
             restore(latest_ckpt, model)
         else:
-            raise ValueError("model {}\'s ckpt isn't exist".format(name))
+            raise ValueError("model {}'s ckpt isn't exist".format(name))
+
 
 def restore_models(model_dir, models, global_step):
     name_to_model = _get_name_to_model_map(models)
     for name, model in name_to_model.items():
         ckpt_filename = "{}-{}.tckpt".format(name, global_step)
         ckpt_path = model_dir + "/" + ckpt_filename
         restore(ckpt_path, model)
 
 
-def save_models(model_dir,
-                models,
-                global_step,
-                max_to_keep=15,
-                keep_latest=True):
+def save_models(model_dir, models, global_step, max_to_keep=15, keep_latest=True):
     with DelayedKeyboardInterrupt():
         name_to_model = _get_name_to_model_map(models)
         for name, model in name_to_model.items():
             save(model_dir, model, name, global_step, max_to_keep, keep_latest)
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/common.py` & `alfred-py-3.0.7/alfred/dl/torch/train/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 import datetime
 import os
 import shutil
 
+
 def create_folder(prefix, add_time=True, add_str=None, delete=False):
-    additional_str = ''
+    additional_str = ""
     if delete is True:
         if os.path.exists(prefix):
             shutil.rmtree(prefix)
         os.makedirs(prefix)
     folder = prefix
     if add_time is True:
         # additional_str has a form such as '170903_220351'
         additional_str += datetime.datetime.now().strftime("%y%m%d_%H%M%S")
         if add_str is not None:
-            folder += '/' + additional_str + '_' + add_str
+            folder += "/" + additional_str + "_" + add_str
         else:
-            folder += '/' + additional_str
+            folder += "/" + additional_str
     if delete is True:
         if os.path.exists(folder):
             shutil.rmtree(folder)
     os.makedirs(folder)
-    return folder
+    return folder
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/fastai_optim.py` & `alfred-py-3.0.7/alfred/dl/torch/train/fastai_optim.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,91 +36,98 @@
 
 def split_bn_bias(layer_groups):
     "Split the layers in `layer_groups` into batchnorm (`bn_types`) and non-batchnorm groups."
     split_groups = []
     for l in layer_groups:
         l1, l2 = [], []
         for c in l.children():
-            if isinstance(c, bn_types): l2.append(c)
-            else: l1.append(c)
+            if isinstance(c, bn_types):
+                l2.append(c)
+            else:
+                l1.append(c)
         split_groups += [nn.Sequential(*l1), nn.Sequential(*l2)]
     return split_groups
 
 
 def get_master(layer_groups, flat_master: bool = False):
     "Return two lists, one for the model parameters in FP16 and one for the master parameters in FP32."
     split_groups = split_bn_bias(layer_groups)
-    model_params = [[
-        param for param in lg.parameters() if param.requires_grad
-    ] for lg in split_groups]
+    model_params = [
+        [param for param in lg.parameters() if param.requires_grad]
+        for lg in split_groups
+    ]
     if flat_master:
         master_params = []
         for lg in model_params:
             if len(lg) != 0:
                 mp = parameters_to_vector([param.data.float() for param in lg])
                 mp = torch.nn.Parameter(mp, requires_grad=True)
-                if mp.grad is None: mp.grad = mp.new(*mp.size())
+                if mp.grad is None:
+                    mp.grad = mp.new(*mp.size())
                 master_params.append([mp])
             else:
                 master_params.append([])
         return model_params, master_params
     else:
-        master_params = [[param.clone().float().detach() for param in lg]
-                         for lg in model_params]
+        master_params = [
+            [param.clone().float().detach() for param in lg] for lg in model_params
+        ]
         for mp in master_params:
             for param in mp:
                 param.requires_grad = True
         return model_params, master_params
 
 
-def model_g2master_g(model_params, master_params,
-                     flat_master: bool = False) -> None:
+def model_g2master_g(model_params, master_params, flat_master: bool = False) -> None:
     "Copy the `model_params` gradients to `master_params` for the optimizer step."
     if flat_master:
         for model_group, master_group in zip(model_params, master_params):
             if len(master_group) != 0:
                 master_group[0].grad.data.copy_(
-                    parameters_to_vector(
-                        [p.grad.data.float() for p in model_group]))
+                    parameters_to_vector([p.grad.data.float() for p in model_group])
+                )
     else:
         for model_group, master_group in zip(model_params, master_params):
             for model, master in zip(model_group, master_group):
                 if model.grad is not None:
                     if master.grad is None:
                         master.grad = master.data.new(*master.data.size())
                     master.grad.data.copy_(model.grad.data)
                 else:
                     master.grad = None
 
 
-def master2model(model_params, master_params,
-                 flat_master: bool = False) -> None:
+def master2model(model_params, master_params, flat_master: bool = False) -> None:
     "Copy `master_params` to `model_params`."
     if flat_master:
         for model_group, master_group in zip(model_params, master_params):
             if len(model_group) != 0:
                 for model, master in zip(
-                        model_group,
-                        _unflatten_dense_tensors(master_group[0].data,
-                                                 model_group)):
+                    model_group,
+                    _unflatten_dense_tensors(master_group[0].data, model_group),
+                ):
                     model.data.copy_(master)
     else:
         for model_group, master_group in zip(model_params, master_params):
             for model, master in zip(model_group, master_group):
                 model.data.copy_(master.data)
 
 
 def listify(p=None, q=None):
     "Make `p` listy and the same length as `q`."
-    if p is None: p = []
-    elif isinstance(p, str): p = [p]
-    elif not isinstance(p, Iterable): p = [p]
+    if p is None:
+        p = []
+    elif isinstance(p, str):
+        p = [p]
+    elif not isinstance(p, Iterable):
+        p = [p]
     n = q if type(q) == int else len(p) if q is None else len(q)
-    if len(p) == 1: p = p * n
-    assert len(p) == n, f'List len mismatch ({len(p)} vs {n})'
+    if len(p) == 1:
+        p = p * n
+    assert len(p) == n, f"List len mismatch ({len(p)} vs {n})"
     return list(p)
 
 
 def trainable_params(m: nn.Module):
     "Return list of trainable params in `m`."
     res = filter(lambda p: p.requires_grad, m.parameters())
     return res
@@ -134,70 +141,68 @@
 class OptimWrapper(torch.optim.Optimizer):
     "Basic wrapper around `opt` to simplify hyper-parameters changes."
 
     def __init__(self, opt, wd, true_wd: bool = False, bn_wd: bool = True):
         # super().__init__(opt.param_groups, dict())
         self.opt, self.true_wd, self.bn_wd = opt, true_wd, bn_wd
         self.opt_keys = list(self.opt.param_groups[0].keys())
-        self.opt_keys.remove('params')
+        self.opt_keys.remove("params")
         self.read_defaults()
         self.wd = wd
 
     @classmethod
     def create(cls, opt_func, lr, layer_groups, **kwargs):
         "Create an `optim.Optimizer` from `opt_func` with `lr`. Set lr on `layer_groups`."
         split_groups = split_bn_bias(layer_groups)
-        opt = opt_func([{
-            'params': trainable_params(l),
-            'lr': 0
-        } for l in split_groups])
+        opt = opt_func([{"params": trainable_params(l), "lr": 0} for l in split_groups])
         opt = cls(opt, **kwargs)
         opt.lr, opt.opt_func = listify(lr, layer_groups), opt_func
         return opt
 
     def new(self, layer_groups):
         "Create a new `OptimWrapper` from `self` with another `layer_groups` but the same hyper-parameters."
-        opt_func = getattr(self, 'opt_func', self.opt.__class__)
+        opt_func = getattr(self, "opt_func", self.opt.__class__)
         split_groups = split_bn_bias(layer_groups)
-        opt = opt_func([{
-            'params': trainable_params(l),
-            'lr': 0
-        } for l in split_groups])
+        opt = opt_func([{"params": trainable_params(l), "lr": 0} for l in split_groups])
         return self.create(
             opt_func,
             self.lr,
             layer_groups,
             wd=self.wd,
             true_wd=self.true_wd,
-            bn_wd=self.bn_wd)
+            bn_wd=self.bn_wd,
+        )
 
     def __repr__(self) -> str:
-        return f'OptimWrapper over {repr(self.opt)}.\nTrue weight decay: {self.true_wd}'
+        return f"OptimWrapper over {repr(self.opt)}.\nTrue weight decay: {self.true_wd}"
 
-    #Pytorch optimizer methods
+    # Pytorch optimizer methods
     def step(self) -> None:
         "Set weight decay and step optimizer."
         # weight decay outside of optimizer step (AdamW)
         if self.true_wd:
-            for lr, wd, pg1, pg2 in zip(self._lr, self._wd,
-                                        self.opt.param_groups[::2],
-                                        self.opt.param_groups[1::2]):
-                for p in pg1['params']:
+            for lr, wd, pg1, pg2 in zip(
+                self._lr,
+                self._wd,
+                self.opt.param_groups[::2],
+                self.opt.param_groups[1::2],
+            ):
+                for p in pg1["params"]:
                     p.data.mul_(1 - wd * lr)
                 if self.bn_wd:
-                    for p in pg2['params']:
+                    for p in pg2["params"]:
                         p.data.mul_(1 - wd * lr)
-            self.set_val('weight_decay', listify(0, self._wd))
+            self.set_val("weight_decay", listify(0, self._wd))
         self.opt.step()
 
     def zero_grad(self) -> None:
         "Clear optimizer gradients."
         self.opt.zero_grad()
 
-    #Passthrough to the inner opt.
+    # Passthrough to the inner opt.
     def __getstate__(self):
         return self.opt.__getstate__()
 
     def __setstate__(self, state):
         return self.opt.__setstate__(state)
 
     def state_dict(self):
@@ -208,137 +213,142 @@
 
     def add_param_group(self, param_group):
         return self.opt.add_param_group(param_group)
 
     def clear(self):
         "Reset the state of the inner optimizer."
         sd = self.state_dict()
-        sd['state'] = {}
+        sd["state"] = {}
         self.load_state_dict(sd)
 
     @property
     def param_groups(self):
         return self.opt.param_groups
 
     @property
     def defaults(self):
         return self.opt.defaults
 
     @property
     def state(self):
         return self.opt.state
 
-
-    #Hyperparameters as properties
+    # Hyperparameters as properties
     @property
     def lr(self) -> float:
         return self._lr[-1]
 
     @lr.setter
     def lr(self, val: float) -> None:
-        self._lr = self.set_val('lr', listify(val, self._lr))
+        self._lr = self.set_val("lr", listify(val, self._lr))
 
     @property
     def mom(self) -> float:
         return self._mom[-1]
 
     @mom.setter
     def mom(self, val: float) -> None:
-        if 'momentum' in self.opt_keys:
-            self.set_val('momentum', listify(val, self._mom))
-        elif 'betas' in self.opt_keys:
-            self.set_val('betas', (listify(val, self._mom), self._beta))
+        if "momentum" in self.opt_keys:
+            self.set_val("momentum", listify(val, self._mom))
+        elif "betas" in self.opt_keys:
+            self.set_val("betas", (listify(val, self._mom), self._beta))
         self._mom = listify(val, self._mom)
 
     @property
     def beta(self) -> float:
         return None if self._beta is None else self._beta[-1]
 
     @beta.setter
     def beta(self, val: float) -> None:
         "Set beta (or alpha as makes sense for given optimizer)."
-        if val is None: return
-        if 'betas' in self.opt_keys:
-            self.set_val('betas', (self._mom, listify(val, self._beta)))
-        elif 'alpha' in self.opt_keys:
-            self.set_val('alpha', listify(val, self._beta))
+        if val is None:
+            return
+        if "betas" in self.opt_keys:
+            self.set_val("betas", (self._mom, listify(val, self._beta)))
+        elif "alpha" in self.opt_keys:
+            self.set_val("alpha", listify(val, self._beta))
         self._beta = listify(val, self._beta)
 
     @property
     def wd(self) -> float:
         return self._wd[-1]
 
     @wd.setter
     def wd(self, val: float) -> None:
         "Set weight decay."
         if not self.true_wd:
-            self.set_val(
-                'weight_decay', listify(val, self._wd), bn_groups=self.bn_wd)
+            self.set_val("weight_decay", listify(val, self._wd), bn_groups=self.bn_wd)
         self._wd = listify(val, self._wd)
 
-    #Helper functions
+    # Helper functions
     def read_defaults(self) -> None:
         "Read the values inside the optimizer for the hyper-parameters."
         self._beta = None
-        if 'lr' in self.opt_keys: self._lr = self.read_val('lr')
-        if 'momentum' in self.opt_keys: self._mom = self.read_val('momentum')
-        if 'alpha' in self.opt_keys: self._beta = self.read_val('alpha')
-        if 'betas' in self.opt_keys:
-            self._mom, self._beta = self.read_val('betas')
-        if 'weight_decay' in self.opt_keys:
-            self._wd = self.read_val('weight_decay')
+        if "lr" in self.opt_keys:
+            self._lr = self.read_val("lr")
+        if "momentum" in self.opt_keys:
+            self._mom = self.read_val("momentum")
+        if "alpha" in self.opt_keys:
+            self._beta = self.read_val("alpha")
+        if "betas" in self.opt_keys:
+            self._mom, self._beta = self.read_val("betas")
+        if "weight_decay" in self.opt_keys:
+            self._wd = self.read_val("weight_decay")
 
     def set_val(self, key: str, val, bn_groups: bool = True):
         "Set `val` inside the optimizer dictionary at `key`."
-        if is_tuple(val): val = [(v1, v2) for v1, v2 in zip(*val)]
-        for v, pg1, pg2 in zip(val, self.opt.param_groups[::2],
-                               self.opt.param_groups[1::2]):
+        if is_tuple(val):
+            val = [(v1, v2) for v1, v2 in zip(*val)]
+        for v, pg1, pg2 in zip(
+            val, self.opt.param_groups[::2], self.opt.param_groups[1::2]
+        ):
             pg1[key] = v
-            if bn_groups: pg2[key] = v
+            if bn_groups:
+                pg2[key] = v
         return val
 
     def read_val(self, key: str):
         "Read a hyperparameter `key` in the optimizer dictionary."
         val = [pg[key] for pg in self.opt.param_groups[::2]]
-        if is_tuple(val[0]): val = [o[0] for o in val], [o[1] for o in val]
+        if is_tuple(val[0]):
+            val = [o[0] for o in val], [o[1] for o in val]
         return val
 
 
 class FastAIMixedOptim(OptimWrapper):
     @classmethod
-    def create(cls,
-               opt_func,
-               lr,
-               layer_groups,
-               model,
-               flat_master=False,
-               loss_scale=512.0,
-               **kwargs):
+    def create(
+        cls,
+        opt_func,
+        lr,
+        layer_groups,
+        model,
+        flat_master=False,
+        loss_scale=512.0,
+        **kwargs,
+    ):
         "Create an `optim.Optimizer` from `opt_func` with `lr`. Set lr on `layer_groups`."
         opt = OptimWrapper.create(opt_func, lr, layer_groups, **kwargs)
-        opt.model_params, opt.master_params = get_master(
-            layer_groups, flat_master)
+        opt.model_params, opt.master_params = get_master(layer_groups, flat_master)
         opt.flat_master = flat_master
         opt.loss_scale = loss_scale
         opt.model = model
-        #Changes the optimizer so that the optimization step is done in FP32.
+        # Changes the optimizer so that the optimization step is done in FP32.
         # opt = self.learn.opt
         mom, wd, beta = opt.mom, opt.wd, opt.beta
         lrs = [lr for lr in opt._lr for _ in range(2)]
-        opt_params = [{
-            'params': mp,
-            'lr': lr
-        } for mp, lr in zip(opt.master_params, lrs)]
+        opt_params = [
+            {"params": mp, "lr": lr} for mp, lr in zip(opt.master_params, lrs)
+        ]
         opt.opt = opt_func(opt_params)
         opt.mom, opt.wd, opt.beta = mom, wd, beta
         return opt
 
     def step(self):
-        model_g2master_g(self.model_params, self.master_params,
-                         self.flat_master)
+        model_g2master_g(self.model_params, self.master_params, self.flat_master)
         for group in self.master_params:
             for param in group:
                 param.grad.div_(self.loss_scale)
         super(FastAIMixedOptim, self).step()
         self.model.zero_grad()
-        #Update the params from master to model.
+        # Update the params from master to model.
         master2model(self.model_params, self.master_params, self.flat_master)
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules.py` & `alfred-py-3.0.7/alfred/dl/torch/train/learning_schedules.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,34 @@
 # under the License.
 #
 """PyTorch edition of TensorFlow learning schedule in tensorflow object
 detection API. 
 """
 import numpy as np
 from torch.optim.optimizer import Optimizer
+
+
 class _LRSchedulerStep(object):
     def __init__(self, optimizer, last_step=-1):
         if not isinstance(optimizer, Optimizer):
-            raise TypeError('{} is not an Optimizer'.format(
-                type(optimizer).__name__))
+            raise TypeError("{} is not an Optimizer".format(type(optimizer).__name__))
         self.optimizer = optimizer
         if last_step == -1:
             for group in optimizer.param_groups:
-                group.setdefault('initial_lr', group['lr'])
+                group.setdefault("initial_lr", group["lr"])
         else:
             for i, group in enumerate(optimizer.param_groups):
-                if 'initial_lr' not in group:
+                if "initial_lr" not in group:
                     raise KeyError(
                         "param 'initial_lr' is not specified "
-                        "in param_groups[{}] when resuming an optimizer".
-                        format(i))
+                        "in param_groups[{}] when resuming an optimizer".format(i)
+                    )
         self.base_lrs = list(
-            map(lambda group: group['initial_lr'], optimizer.param_groups))
+            map(lambda group: group["initial_lr"], optimizer.param_groups)
+        )
         self.step(last_step + 1)
         self.last_step = last_step
 
     """
     def get_lr(self):
         raise NotImplementedError
     """
@@ -60,15 +62,15 @@
         raise NotImplementedError
 
     def step(self, step=None):
         if step is None:
             step = self.last_step + 1
         self.last_step = step
         for param_group, lr in zip(self.optimizer.param_groups, self.get_lr()):
-            param_group['lr'] = lr
+            param_group["lr"] = lr
 
 
 class Constant(_LRSchedulerStep):
     def __init__(self, optimizer, last_step=-1):
         super().__init__(optimizer, last_step)
 
     def _get_lr_per_group(self, base_lr):
@@ -82,120 +84,131 @@
 
     def __init__(self, optimizer, boundaries, rates, last_step=-1):
         self._boundaries = boundaries
         self._num_boundaries = len(boundaries)
         self._learning_rates = rates
 
         if any([b < 0 for b in boundaries]) or any(
-            [not isinstance(b, int) for b in boundaries]):
-            raise ValueError('boundaries must be a list of positive integers')
-        if any(
-            [bnext <= b for bnext, b in zip(boundaries[1:], boundaries[:-1])]):
-            raise ValueError(
-                'Entries in boundaries must be strictly increasing.')
+            [not isinstance(b, int) for b in boundaries]
+        ):
+            raise ValueError("boundaries must be a list of positive integers")
+        if any([bnext <= b for bnext, b in zip(boundaries[1:], boundaries[:-1])]):
+            raise ValueError("Entries in boundaries must be strictly increasing.")
         if any([not isinstance(r, float) for r in rates]):
-            raise ValueError('Learning rates must be floats')
+            raise ValueError("Learning rates must be floats")
         if len(rates) != len(boundaries) + 1:
-            raise ValueError('Number of provided learning rates must exceed '
-                             'number of boundary points by exactly 1.')
+            raise ValueError(
+                "Number of provided learning rates must exceed "
+                "number of boundary points by exactly 1."
+            )
         super().__init__(optimizer, last_step)
 
     def _get_lr_per_group(self, base_lr):
         step = self.last_step
         ret = None
         for i, bound in enumerate(self._boundaries):
             if step > bound:
                 ret = self._learning_rates[i + 1]
         if ret is not None:
             return ret
         return self._learning_rates[0]
 
 
 class ExponentialDecayWithBurnin(_LRSchedulerStep):
-    """Pytorch edition of manual_stepping in tensorflow.
-    """
+    """Pytorch edition of manual_stepping in tensorflow."""
 
-    def __init__(self,
-                 optimizer,
-                 learning_rate_decay_steps,
-                 learning_rate_decay_factor,
-                 burnin_learning_rate,
-                 burnin_steps,
-                 last_step=-1):
+    def __init__(
+        self,
+        optimizer,
+        learning_rate_decay_steps,
+        learning_rate_decay_factor,
+        burnin_learning_rate,
+        burnin_steps,
+        last_step=-1,
+    ):
         self._decay_steps = learning_rate_decay_steps
         self._decay_factor = learning_rate_decay_factor
         self._burnin_learning_rate = burnin_learning_rate
         self._burnin_steps = burnin_steps
 
         super().__init__(optimizer, last_step)
 
     def _get_lr_per_group(self, base_lr):
         if self._burnin_learning_rate == 0:
             burnin_learning_rate = base_lr
         step = self.last_step
-        post_burnin_learning_rate = (base_lr * self._decay_factor ^
-                                     (step // self._decay_steps))
+        post_burnin_learning_rate = base_lr * self._decay_factor ^ (
+            step // self._decay_steps
+        )
         if step < self._burnin_steps:
             return burnin_learning_rate
         else:
             return post_burnin_learning_rate
 
 
 class ExponentialDecay(_LRSchedulerStep):
-    def __init__(self,
-                 optimizer,
-                 learning_rate_decay_steps,
-                 learning_rate_decay_factor,
-                 staircase=True,
-                 last_step=-1):
+    def __init__(
+        self,
+        optimizer,
+        learning_rate_decay_steps,
+        learning_rate_decay_factor,
+        staircase=True,
+        last_step=-1,
+    ):
         self._decay_steps = learning_rate_decay_steps
         self._decay_factor = learning_rate_decay_factor
         self._staircase = staircase
 
         super().__init__(optimizer, last_step)
 
     def _get_lr_per_group(self, base_lr):
         step = self.last_step
         if self._staircase:
-            post_burnin_learning_rate = base_lr * pow(self._decay_factor,
-                                         (step // self._decay_steps))
+            post_burnin_learning_rate = base_lr * pow(
+                self._decay_factor, (step // self._decay_steps)
+            )
         else:
-            post_burnin_learning_rate = base_lr * pow(self._decay_factor,
-                                         (step / self._decay_steps))
+            post_burnin_learning_rate = base_lr * pow(
+                self._decay_factor, (step / self._decay_steps)
+            )
 
         return post_burnin_learning_rate
 
 
 class CosineDecayWithWarmup(_LRSchedulerStep):
-    def __init__(self,
-                 optimizer,
-                 total_steps,
-                 warmup_learning_rate,
-                 warmup_steps,
-                 last_step=-1):
+    def __init__(
+        self, optimizer, total_steps, warmup_learning_rate, warmup_steps, last_step=-1
+    ):
         if total_steps < warmup_steps:
-            raise ValueError('total_steps must be larger or equal to '
-                             'warmup_steps.')
+            raise ValueError("total_steps must be larger or equal to " "warmup_steps.")
         self._total_steps = total_steps
         self._warmup_learning_rate = warmup_learning_rate
         self._warmup_steps = warmup_steps
 
         super().__init__(optimizer, last_step)
 
     def _get_lr_per_group(self, base_lr):
         if base_lr < self._warmup_learning_rate:
-            raise ValueError('learning_rate_base must be larger '
-                             'or equal to warmup_learning_rate.')
+            raise ValueError(
+                "learning_rate_base must be larger " "or equal to warmup_learning_rate."
+            )
 
         step = self.last_step
-        learning_rate = 0.5 * base_lr * (
-            1 + np.cos(np.pi *
-                       (float(step) - self._warmup_steps
-                        ) / float(self._total_steps - self._warmup_steps)))
+        learning_rate = (
+            0.5
+            * base_lr
+            * (
+                1
+                + np.cos(
+                    np.pi
+                    * (float(step) - self._warmup_steps)
+                    / float(self._total_steps - self._warmup_steps)
+                )
+            )
+        )
         if self._warmup_steps > 0:
             slope = (base_lr - self._warmup_learning_rate) / self._warmup_steps
-            pre_cosine_learning_rate = slope * float(
-                step) + self._warmup_learning_rate
+            pre_cosine_learning_rate = slope * float(step) + self._warmup_learning_rate
             if step < self._warmup_steps:
                 return pre_cosine_learning_rate
             else:
                 return learning_rate
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/learning_schedules_fastai.py` & `alfred-py-3.0.7/alfred/dl/torch/train/learning_schedules_fastai.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,42 +21,58 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 import numpy as np
 import math
 from functools import partial
 
+
 class LRSchedulerStep(object):
-    def __init__(self, fai_optimizer, total_step, lr_phases,
-                 mom_phases):
+    def __init__(self, fai_optimizer, total_step, lr_phases, mom_phases):
         self.optimizer = fai_optimizer
         self.total_step = total_step
         self.lr_phases = []
-        
+
         for i, (start, lambda_func) in enumerate(lr_phases):
             if len(self.lr_phases) != 0:
                 assert self.lr_phases[-1][0] < int(start * total_step)
             if isinstance(lambda_func, str):
                 lambda_func = eval(lambda_func)
             if i < len(lr_phases) - 1:
-                self.lr_phases.append((int(start * total_step), int(lr_phases[i + 1][0] * total_step), lambda_func))
+                self.lr_phases.append(
+                    (
+                        int(start * total_step),
+                        int(lr_phases[i + 1][0] * total_step),
+                        lambda_func,
+                    )
+                )
             else:
-                self.lr_phases.append((int(start * total_step), total_step, lambda_func))
+                self.lr_phases.append(
+                    (int(start * total_step), total_step, lambda_func)
+                )
         assert self.lr_phases[0][0] == 0
         self.mom_phases = []
-        
+
         for i, (start, lambda_func) in enumerate(mom_phases):
             if len(self.mom_phases) != 0:
                 assert self.mom_phases[-1][0] < int(start * total_step)
             if isinstance(lambda_func, str):
                 lambda_func = eval(lambda_func)
             if i < len(mom_phases) - 1:
-                self.mom_phases.append((int(start * total_step), int(mom_phases[i + 1][0] * total_step), lambda_func))
+                self.mom_phases.append(
+                    (
+                        int(start * total_step),
+                        int(mom_phases[i + 1][0] * total_step),
+                        lambda_func,
+                    )
+                )
             else:
-                self.mom_phases.append((int(start * total_step), total_step, lambda_func))
+                self.mom_phases.append(
+                    (int(start * total_step), total_step, lambda_func)
+                )
         if len(mom_phases) > 0:
             assert self.mom_phases[0][0] == 0
 
     def step(self, step):
         lrs = []
         moms = []
         for start, end, func in self.lr_phases:
@@ -67,47 +83,53 @@
         for start, end, func in self.mom_phases:
             if step >= start:
                 moms.append(func((step - start) / (end - start)))
                 self.optimizer.mom = func((step - start) / (end - start))
         if len(moms) > 0:
             self.optimizer.mom = moms[-1]
 
+
 def annealing_cos(start, end, pct):
     # print(pct, start, end)
     "Cosine anneal from `start` to `end` as pct goes from 0.0 to 1.0."
     cos_out = np.cos(np.pi * pct) + 1
     return end + (start - end) / 2 * cos_out
 
+
 class OneCycle(LRSchedulerStep):
-    def __init__(self, fai_optimizer, total_step, lr_max, moms, div_factor,
-                 pct_start):
+    def __init__(self, fai_optimizer, total_step, lr_max, moms, div_factor, pct_start):
         self.lr_max = lr_max
         self.moms = moms
         self.div_factor = div_factor
         self.pct_start = pct_start
         a1 = int(total_step * self.pct_start)
         a2 = total_step - a1
         low_lr = self.lr_max / self.div_factor
-        lr_phases = ((0, partial(annealing_cos, low_lr, self.lr_max)),
-                     (self.pct_start,
-                      partial(annealing_cos, self.lr_max, low_lr / 1e4)))
-        mom_phases = ((0, partial(annealing_cos, *self.moms)),
-                      (self.pct_start, partial(annealing_cos,
-                                               *self.moms[::-1])))
+        lr_phases = (
+            (0, partial(annealing_cos, low_lr, self.lr_max)),
+            (self.pct_start, partial(annealing_cos, self.lr_max, low_lr / 1e4)),
+        )
+        mom_phases = (
+            (0, partial(annealing_cos, *self.moms)),
+            (self.pct_start, partial(annealing_cos, *self.moms[::-1])),
+        )
         fai_optimizer.lr, fai_optimizer.mom = low_lr, self.moms[0]
         super().__init__(fai_optimizer, total_step, lr_phases, mom_phases)
 
+
 class ExponentialDecay(LRSchedulerStep):
-    def __init__(self,
-                 fai_optimizer, 
-                 total_step,
-                 initial_learning_rate,
-                 decay_length, 
-                 decay_factor,
-                 staircase=True):
+    def __init__(
+        self,
+        fai_optimizer,
+        total_step,
+        initial_learning_rate,
+        decay_length,
+        decay_factor,
+        staircase=True,
+    ):
         """
         Args:
             decay_length: must in (0, 1)
         """
         assert decay_length > 0
         assert decay_length < 1
         self._decay_steps_unified = decay_length
@@ -123,20 +145,17 @@
                 stage *= decay_factor
                 step += int(decay_length * total_step)
         else:
             func = lambda p: pow(decay_factor, (p / decay_length))
             lr_phases.append((0, func))
         super().__init__(fai_optimizer, total_step, lr_phases, [])
 
+
 class ManualStepping(LRSchedulerStep):
-    def __init__(self,
-                 fai_optimizer, 
-                 total_step,
-                 boundaries,
-                 rates):
+    def __init__(self, fai_optimizer, total_step, boundaries, rates):
         assert all([b > 0 and b < 1 for b in boundaries])
         assert len(boundaries) + 1 == len(rates)
         boundaries.insert(0, 0.0)
         lr_phases = []
         for start, rate in zip(boundaries, rates):
             func = lambda p, _d=rate: _d
             lr_phases.append((start, func))
@@ -144,25 +163,27 @@
 
 
 class FakeOptim:
     def __init__(self):
         self.lr = 0
         self.mom = 0
 
+
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
-    opt = FakeOptim()# 3e-3, wd=0.4, div_factor=10
+
+    opt = FakeOptim()  # 3e-3, wd=0.4, div_factor=10
     # schd = OneCycle(opt, 100, 3e-3, (0.95, 0.85), 10.0, 0.4)
     schd = ExponentialDecay(opt, 100, 3e-4, 0.1, 0.8, staircase=True)
     schd = ManualStepping(opt, 100, [0.8, 0.9], [0.001, 0.0001, 0.00005])
     lrs = []
     moms = []
     for i in range(100):
         schd.step(i)
         lrs.append(opt.lr)
         moms.append(opt.mom)
-    
+
     plt.plot(lrs)
     # plt.plot(moms)
     # plt.show()
     # plt.plot(moms)
     plt.show()
```

### Comparing `alfred-py-3.0.6/alfred/dl/torch/train/optim.py` & `alfred-py-3.0.7/alfred/dl/torch/train/optim.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,62 +26,68 @@
 import torch
 from copy import deepcopy
 from itertools import chain
 from torch.autograd import Variable
 
 required = object()
 
+
 def param_fp32_copy(params):
     param_copy = [
         param.clone().type(torch.cuda.FloatTensor).detach() for param in params
     ]
     for param in param_copy:
         param.requires_grad = True
     return param_copy
 
+
 def set_grad(params, params_with_grad, scale=1.0):
     for param, param_w_grad in zip(params, params_with_grad):
         if param.grad is None:
             param.grad = torch.nn.Parameter(
-                param.data.new().resize_(*param.data.size()))
+                param.data.new().resize_(*param.data.size())
+            )
         grad = param_w_grad.grad.data
         if scale is not None:
             grad /= scale
         if torch.isnan(grad).any() or torch.isinf(grad).any():
-            return True # invalid grad
+            return True  # invalid grad
         param.grad.data.copy_(grad)
     return False
 
+
 class MixedPrecisionWrapper(object):
     """mixed precision optimizer wrapper.
     Arguments:
-        optimizer (torch.optim.Optimizer): an instance of 
+        optimizer (torch.optim.Optimizer): an instance of
             :class:`torch.optim.Optimizer`
         scale: (float): a scalar for grad scale.
         auto_scale: (bool): whether enable auto scale.
-            The algorihm of auto scale is discribled in 
+            The algorihm of auto scale is discribled in
             http://docs.nvidia.com/deeplearning/sdk/mixed-precision-training/index.html
     """
 
-    def __init__(self,
-                 optimizer,
-                 scale=None,
-                 auto_scale=True,
-                 inc_factor=2.0,
-                 dec_factor=0.5,
-                 num_iters_be_stable=500):
+    def __init__(
+        self,
+        optimizer,
+        scale=None,
+        auto_scale=True,
+        inc_factor=2.0,
+        dec_factor=0.5,
+        num_iters_be_stable=500,
+    ):
         if not isinstance(optimizer, torch.optim.Optimizer):
             raise ValueError("must provide a torch.optim.Optimizer")
         self.optimizer = optimizer
-        if hasattr(self.optimizer, 'name'):
+        if hasattr(self.optimizer, "name"):
             self.name = self.optimizer.name  # for ckpt system
         param_groups_copy = []
         for i, group in enumerate(optimizer.param_groups):
-            group_copy = {n: v for n, v in group.items() if n != 'params'}
-            group_copy['params'] = param_fp32_copy(group['params'])
+            group_copy = {n: v for n, v in group.items() if n != "params"}
+            group_copy["params"] = param_fp32_copy(group["params"])
             param_groups_copy.append(group_copy)
 
         # switch param_groups, may be dangerous
         self.param_groups = optimizer.param_groups
         optimizer.param_groups = param_groups_copy
         self.grad_scale = scale
         self.auto_scale = auto_scale
@@ -106,29 +112,28 @@
         return self.optimizer.load_state_dict(state_dict)
 
     def zero_grad(self):
         return self.optimizer.zero_grad()
 
     def step(self, closure=None):
         for g, g_copy in zip(self.param_groups, self.optimizer.param_groups):
-            invalid = set_grad(g_copy['params'], g['params'], self.grad_scale)
+            invalid = set_grad(g_copy["params"], g["params"], self.grad_scale)
             if invalid:
                 if self.grad_scale is None or self.auto_scale is False:
                     raise ValueError("nan/inf detected but auto_scale disabled.")
                 self.grad_scale *= self.dec_factor
-                print('scale decay to {}'.format(self.grad_scale))
+                print("scale decay to {}".format(self.grad_scale))
                 return
         if self.auto_scale is True:
             self.stable_iter_count += 1
             if self.stable_iter_count > self.num_iters_be_stable:
                 if self.grad_scale is not None:
                     self.grad_scale *= self.inc_factor
                 self.stable_iter_count = 0
 
         if closure is None:
             self.optimizer.step()
         else:
             self.optimizer.step(closure)
         for g, g_copy in zip(self.param_groups, self.optimizer.param_groups):
-            for p_copy, p in zip(g_copy['params'], g['params']):
+            for p_copy, p in zip(g_copy["params"], g["params"]):
                 p.data.copy_(p_copy.data)
-
```

### Comparing `alfred-py-3.0.6/alfred/fonts/FZSSJW.TTF` & `alfred-py-3.0.7/alfred/fonts/FZSSJW.TTF`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/fusion/__init__.py` & `alfred-py-3.0.7/alfred/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/fusion/common.py` & `alfred-py-3.0.7/alfred/fusion/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,31 +45,38 @@
     :return:
     """
     # currently, we skip box which not has 8 points
     pts = np.array(pts, dtype=np.int)
     if pts.shape != (8, 2):
         return
         # clockwise face idx
-    face_idx = [[0, 1, 5, 4],
-                [1, 2, 6, 5],
-                [2, 3, 7, 6],
-                [3, 0, 4, 7]]
+    face_idx = [[0, 1, 5, 4], [1, 2, 6, 5], [2, 3, 7, 6], [3, 0, 4, 7]]
     for ind_f in range(3, -1, -1):
         # 3, 2, 1, 0
         f = face_idx[ind_f]
 
         # indicates the direction
         for j in range(4):
             if ind_f == 0 and j == 0:
-                cv2.line(img, (pts[f[0], 0], pts[f[0], 1]),
-                         (pts[f[1], 0], pts[f[1], 1]), (255, 255, 0),
-                         thickness, lineType=cv2.LINE_AA)
-            cv2.line(img, (pts[f[j], 0], pts[f[j], 1]),
-                     (pts[f[(j + 1) % 4], 0], pts[f[(j + 1) % 4], 1]), color,
-                     thickness, lineType=cv2.LINE_AA)
+                cv2.line(
+                    img,
+                    (pts[f[0], 0], pts[f[0], 1]),
+                    (pts[f[1], 0], pts[f[1], 1]),
+                    (255, 255, 0),
+                    thickness,
+                    lineType=cv2.LINE_AA,
+                )
+            cv2.line(
+                img,
+                (pts[f[j], 0], pts[f[j], 1]),
+                (pts[f[(j + 1) % 4], 0], pts[f[(j + 1) % 4], 1]),
+                color,
+                thickness,
+                lineType=cv2.LINE_AA,
+            )
 
 
 def compute_3d_box_cam_coords(xyz, lwh, rotation_y):
     """
     KITTI camera coordinates using -y as up
     this only works on camera coordinates xyz
     center
@@ -95,19 +102,17 @@
 
     corners = np.array([x_corners, y_corners, z_corners], dtype=np.float32)
     corners_3d = np.dot(R, corners)
     corners_3d = corners_3d + np.array(location, dtype=np.float32).reshape(3, 1)
     return corners_3d.transpose(1, 0)
 
 
-def compute_3d_box_lidar_coords(centers,
-                                dims,
-                                angles=None,
-                                origin=(0.5, 0.5, 0.5),
-                                axis=2):
+def compute_3d_box_lidar_coords(
+    centers, dims, angles=None, origin=(0.5, 0.5, 0.5), axis=2
+):
     corners = _corners_nd(dims, origin=origin)
     # corners: [N, 8, 3]
     if angles is not None:
         corners = _rotation_3d_in_axis(corners, angles, axis=axis)
     corners += centers.reshape([-1, 1, 3])
     return corners
 
@@ -116,39 +121,53 @@
 def _rotation_3d_in_axis(points, angles, axis=0):
     # points: [N, point_size, 3]
     rot_sin = np.sin(angles)
     rot_cos = np.cos(angles)
     ones = np.ones_like(rot_cos)
     zeros = np.zeros_like(rot_cos)
     if axis == 1:
-        rot_mat_T = np.stack([[rot_cos, zeros, -rot_sin], [zeros, ones, zeros],
-                              [rot_sin, zeros, rot_cos]])
+        rot_mat_T = np.stack(
+            [
+                [rot_cos, zeros, -rot_sin],
+                [zeros, ones, zeros],
+                [rot_sin, zeros, rot_cos],
+            ]
+        )
     elif axis == 2 or axis == -1:
-        rot_mat_T = np.stack([[rot_cos, -rot_sin, zeros],
-                              [rot_sin, rot_cos, zeros], [zeros, zeros, ones]])
+        rot_mat_T = np.stack(
+            [
+                [rot_cos, -rot_sin, zeros],
+                [rot_sin, rot_cos, zeros],
+                [zeros, zeros, ones],
+            ]
+        )
     elif axis == 0:
-        rot_mat_T = np.stack([[zeros, rot_cos, -rot_sin],
-                              [zeros, rot_sin, rot_cos], [ones, zeros, zeros]])
+        rot_mat_T = np.stack(
+            [
+                [zeros, rot_cos, -rot_sin],
+                [zeros, rot_sin, rot_cos],
+                [ones, zeros, zeros],
+            ]
+        )
     else:
         raise ValueError("axis should in range")
-    return np.einsum('aij,jka->aik', points, rot_mat_T)
+    return np.einsum("aij,jka->aik", points, rot_mat_T)
 
 
 def _corners_nd(dims, origin=0.5):
     ndim = int(dims.shape[1])
     corners_norm = np.stack(
-        np.unravel_index(np.arange(2 ** ndim), [2] * ndim),
-        axis=1).astype(dims.dtype)
+        np.unravel_index(np.arange(2**ndim), [2] * ndim), axis=1
+    ).astype(dims.dtype)
     # now corners_norm has format: (2d) x0y0, x0y1, x1y0, x1y1
     # (3d) x0y0z0, x0y0z1, x0y1z0, x0y1z1, x1y0z0, x1y0z1, x1y1z0, x1y1z1
     # so need to convert to a format which is convenient to do other computing.
     # for 2d boxes, format is clockwise start with minimum point
     # for 3d boxes, please draw lines by your hand.
     if ndim == 2:
         # generate clockwise box corners
         corners_norm = corners_norm[[0, 1, 3, 2]]
     elif ndim == 3:
         corners_norm = corners_norm[[0, 1, 3, 2, 4, 5, 7, 6]]
     corners_norm = corners_norm - np.array(origin, dtype=dims.dtype)
-    corners = dims.reshape([-1, 1, ndim]) * corners_norm.reshape(
-        [1, 2 ** ndim, ndim])
+    corners = dims.reshape([-1, 1, ndim]) * corners_norm.reshape([1, 2**ndim, ndim])
     return corners
```

### Comparing `alfred-py-3.0.6/alfred/fusion/geometry.py` & `alfred-py-3.0.7/alfred/fusion/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,22 +31,26 @@
 import math
 
 
 def euler_to_quaternion(yaw, pitch, roll):
     """
     return a list of [qx, qy, qz, qw]
     """
-    qx = np.sin(roll/2) * np.cos(pitch/2) * np.cos(yaw/2) - \
-        np.cos(roll/2) * np.sin(pitch/2) * np.sin(yaw/2)
-    qy = np.cos(roll/2) * np.sin(pitch/2) * np.cos(yaw/2) + \
-        np.sin(roll/2) * np.cos(pitch/2) * np.sin(yaw/2)
-    qz = np.cos(roll/2) * np.cos(pitch/2) * np.sin(yaw/2) - \
-        np.sin(roll/2) * np.sin(pitch/2) * np.cos(yaw/2)
-    qw = np.cos(roll/2) * np.cos(pitch/2) * np.cos(yaw/2) + \
-        np.sin(roll/2) * np.sin(pitch/2) * np.sin(yaw/2)
+    qx = np.sin(roll / 2) * np.cos(pitch / 2) * np.cos(yaw / 2) - np.cos(
+        roll / 2
+    ) * np.sin(pitch / 2) * np.sin(yaw / 2)
+    qy = np.cos(roll / 2) * np.sin(pitch / 2) * np.cos(yaw / 2) + np.sin(
+        roll / 2
+    ) * np.cos(pitch / 2) * np.sin(yaw / 2)
+    qz = np.cos(roll / 2) * np.cos(pitch / 2) * np.sin(yaw / 2) - np.sin(
+        roll / 2
+    ) * np.sin(pitch / 2) * np.cos(yaw / 2)
+    qw = np.cos(roll / 2) * np.cos(pitch / 2) * np.cos(yaw / 2) + np.sin(
+        roll / 2
+    ) * np.sin(pitch / 2) * np.sin(yaw / 2)
     return [qx, qy, qz, qw]
 
 
 def quaternion_to_euler(x, y, z, w):
     """
     return a list of euler angles [yaw, pitch, roll]
     """
```

### Comparing `alfred-py-3.0.6/alfred/fusion/kitti_fusion.py` & `alfred-py-3.0.7/alfred/fusion/kitti_fusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,32 @@
 
 import numpy as np
 
 
 class LidarCamCalibData(object):
     """
 
-    Load from raw:
+        Load from raw:
 
-    P0: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 0.000000000000e+00 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 0.000000000000e+00
-P1: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 -3.875744000000e+02 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 0.000000000000e+00
-P2: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 4.485728000000e+01 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 2.163791000000e-01 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 2.745884000000e-03
-P3: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 -3.395242000000e+02 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 2.199936000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 2.729905000000e-03
-R0_rect: 9.999239000000e-01 9.837760000000e-03 -7.445048000000e-03 -9.869795000000e-03 9.999421000000e-01 -4.278459000000e-03 7.402527000000e-03 4.351614000000e-03 9.999631000000e-01
-Tr_velo_to_cam: 7.533745000000e-03 -9.999714000000e-01 -6.166020000000e-04 -4.069766000000e-03 1.480249000000e-02 7.280733000000e-04 -9.998902000000e-01 -7.631618000000e-02 9.998621000000e-01 7.523790000000e-03 1.480755000000e-02 -2.717806000000e-01
-Tr_imu_to_velo: 9.999976000000e-01 7.553071000000e-04 -2.035826000000e-03 -8.086759000000e-01 -7.854027000000e-04 9.998898000000e-01 -1.482298000000e-02 3.195559000000e-01 2.024406000000e-03 1.482454000000e-02 9.998881000000e-01 -7.997231000000e-01
+        P0: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 0.000000000000e+00 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 0.000000000000e+00
+    P1: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 -3.875744000000e+02 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 0.000000000000e+00
+    P2: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 4.485728000000e+01 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 2.163791000000e-01 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 2.745884000000e-03
+    P3: 7.215377000000e+02 0.000000000000e+00 6.095593000000e+02 -3.395242000000e+02 0.000000000000e+00 7.215377000000e+02 1.728540000000e+02 2.199936000000e+00 0.000000000000e+00 0.000000000000e+00 1.000000000000e+00 2.729905000000e-03
+    R0_rect: 9.999239000000e-01 9.837760000000e-03 -7.445048000000e-03 -9.869795000000e-03 9.999421000000e-01 -4.278459000000e-03 7.402527000000e-03 4.351614000000e-03 9.999631000000e-01
+    Tr_velo_to_cam: 7.533745000000e-03 -9.999714000000e-01 -6.166020000000e-04 -4.069766000000e-03 1.480249000000e-02 7.280733000000e-04 -9.998902000000e-01 -7.631618000000e-02 9.998621000000e-01 7.523790000000e-03 1.480755000000e-02 -2.717806000000e-01
+    Tr_imu_to_velo: 9.999976000000e-01 7.553071000000e-04 -2.035826000000e-03 -8.086759000000e-01 -7.854027000000e-04 9.998898000000e-01 -1.482298000000e-02 3.195559000000e-01 2.024406000000e-03 1.482454000000e-02 9.998881000000e-01 -7.997231000000e-01
 
-    Suppose we have 1 lidar and 4 cameras,
-    more sensors can add more params too.
+        Suppose we have 1 lidar and 4 cameras,
+        more sensors can add more params too.
 
-    tr: 3x1, transform vector
-    r: 3x3, rotation vector
+        tr: 3x1, transform vector
+        r: 3x3, rotation vector
 
     """
+
     def __init__(self, calib_f=None):
         # transformation between lidar and 4 cameras
         self.T_lidar_to_cam_0 = []
         self.T_lidar_to_cam_1 = []
         self.T_lidar_to_cam_2 = []
         self.T_lidar_to_cam_3 = []
 
@@ -93,52 +94,65 @@
         if self.calib_f is not None:
             self._read_kitti_calib_from_txt()
             self.bootstrap()
 
     def _read_kitti_calib_from_txt(self, is_video=False):
         if not is_video:
             data = {}
-            with open(self.calib_f, 'r') as f:
+            with open(self.calib_f, "r") as f:
                 for line in f.readlines():
                     line = line.strip()
-                    if line != '':
-                        key, value = line.split(': ')
+                    if line != "":
+                        key, value = line.split(": ")
                         # The only non-float values in these files are dates, which
                         # we don't care about anyway
                         try:
                             data[key] = [float(x) for x in value.split()]
                         except ValueError:
                             pass
-            self.TR_lidar_to_cam_0 = data['Tr_velo_to_cam']
-            self.P_cam_0 = data['P2']
-            self.Rect_cam_0 = data['R0_rect']
+            self.TR_lidar_to_cam_0 = data["Tr_velo_to_cam"]
+            self.P_cam_0 = data["P2"]
+            self.Rect_cam_0 = data["R0_rect"]
 
     def bootstrap(self):
         if len(self.TR_lidar_to_cam_0) > 0:
             self.TR_lidar_to_cam_0 = np.reshape(self.TR_lidar_to_cam_0, (3, 4))
         else:
             self.TR_lidar_to_cam_0 = np.concatenate(
-                (np.reshape(self.R_lidar_to_cam_0, (3, 3)),
-                 np.array([self.T_lidar_to_cam_0]).T), axis=1
+                (
+                    np.reshape(self.R_lidar_to_cam_0, (3, 3)),
+                    np.array([self.T_lidar_to_cam_0]).T,
+                ),
+                axis=1,
             )
-        self.TR_lidar_to_cam_0 = np.pad(self.TR_lidar_to_cam_0, ((0, 1), (0, 0)), 'constant')
+        self.TR_lidar_to_cam_0 = np.pad(
+            self.TR_lidar_to_cam_0, ((0, 1), (0, 0)), "constant"
+        )
 
         if isinstance(self.Rect_cam_0, list):
             self.Rect_cam_0 = np.reshape(self.Rect_cam_0, (3, 3))
-        self.Rect_cam_0 = np.pad(self.Rect_cam_0, ((0, 1), (0, 1)), 'constant')
+        self.Rect_cam_0 = np.pad(self.Rect_cam_0, ((0, 1), (0, 1)), "constant")
         if isinstance(self.P_cam_0, list):
             self.P_cam_0 = np.reshape(self.P_cam_0, (3, 4))
 
-        assert self.TR_lidar_to_cam_0.shape == (4, 4), 'TR_lidar_to_cam_0 is R|T, which is 3x4, but received wrong'
-        assert self.Rect_cam_0.shape == (4, 4), 'Rect_cam_0 is 3x3, but solve failed (a 9 length list is also OK)'
-        assert self.P_cam_0.shape == (3, 4), 'P_cam {} vs {} failed'.format('(3, 4)', self.P_cam_0.shape)
+        assert self.TR_lidar_to_cam_0.shape == (
+            4,
+            4,
+        ), "TR_lidar_to_cam_0 is R|T, which is 3x4, but received wrong"
+        assert self.Rect_cam_0.shape == (
+            4,
+            4,
+        ), "Rect_cam_0 is 3x3, but solve failed (a 9 length list is also OK)"
+        assert self.P_cam_0.shape == (3, 4), "P_cam {} vs {} failed".format(
+            "(3, 4)", self.P_cam_0.shape
+        )
         self.checked = True
 
     def __str__(self):
-        return 'TR_lidar_to_cam_0: {}\nP_cam_0: {}\nRect_cam_0: {}\nK_cam_0: {}'.format(
+        return "TR_lidar_to_cam_0: {}\nP_cam_0: {}\nRect_cam_0: {}\nK_cam_0: {}".format(
             self.TR_lidar_to_cam_0, self.P_cam_0, self.Rect_cam_0, self.K_cam_0
         )
 
 
 def lidar_pts_to_cam0_frame(pts3d, calib, filter_intensity=False):
     """
     Directly convert all lidar points to camera frame
@@ -151,39 +165,41 @@
     if filter_intensity:
         pts3d = pts3d[pts3d[:, 3] > 0, :]
     pts3d[:, 3] = 1
     pts3d = np.transpose(pts3d)
     # Pad the r0_rect matrix to a 4x4
     if isinstance(calib, LidarCamCalibData):
         if not calib.checked:
-            ValueError('calib not bootstraped, did you called calib_data.bootstrap()?')
+            ValueError("calib not bootstraped, did you called calib_data.bootstrap()?")
         else:
             cam0_xyz = np.dot(calib.TR_lidar_to_cam_0, pts3d)
 
             ret_xyz = np.dot(calib.Rect_cam_0, cam0_xyz)
-            idx = (ret_xyz[2, :] >= 0)
+            idx = ret_xyz[2, :] >= 0
             pts2d_cam = np.dot(calib.P_cam_0, ret_xyz[:, idx])
             return pts3d[:, idx], pts2d_cam / pts2d_cam[2, :]
     else:
-        ValueError('frame_calib must be an LidarCamCalibData type')
+        ValueError("frame_calib must be an LidarCamCalibData type")
 
 
 def lidar_pt_to_cam0_frame(pt3d, calib):
     """
     Convert a single point of lidar
     :param pt3d:
     :param calib:
     :return:
     """
     # padding the 4th element to 1
     pt3d = np.append(pt3d, 1)
     # Pad the r0_rect matrix to a 4x4
     if isinstance(calib, LidarCamCalibData):
         if not calib.checked:
-            raise ValueError('calib not bootstrap, did you called calib_data.bootstrap()?')
+            raise ValueError(
+                "calib not bootstrap, did you called calib_data.bootstrap()?"
+            )
         else:
             # 1. Get xyz1 on cam0
             cam0_xyz = np.dot(calib.TR_lidar_to_cam_0, pt3d)
 
             # 2. Get cam0 after rectify
             ret_xyz = np.dot(calib.Rect_cam_0, cam0_xyz)
 
@@ -191,42 +207,45 @@
             if ret_xyz[2] >= 0:
                 # 6. Get projected coords
                 pts2d_cam = np.dot(calib.P_cam_0, ret_xyz)
                 return pts2d_cam / pts2d_cam[2]
             else:
                 return None
     else:
-        raise ValueError('frame_calib must be an LidarCamCalibData type')
+        raise ValueError("frame_calib must be an LidarCamCalibData type")
 
 
 def cam3d_to_pixel(cam3d, calib):
     """
     Convert a single point of lidar
     :param cam3d:
     :param calib:
     :return:
     """
     # padding the 4th element to 1
     pt3d = np.append(cam3d, 1)
     # Pad the r0_rect matrix to a 4x4
     if isinstance(calib, LidarCamCalibData):
         if not calib.checked:
-            raise ValueError('calib not bootstrap, did you called calib_data.bootstrap()?')
+            raise ValueError(
+                "calib not bootstrap, did you called calib_data.bootstrap()?"
+            )
         else:
             # 2. Get cam0 after rectify
             ret_xyz = np.dot(calib.Rect_cam_0, pt3d)
 
             # 3. if points not on image, then return None
             if ret_xyz[2] >= 0:
                 # 6. Get projected coords
                 pts2d_cam = np.dot(calib.P_cam_0, ret_xyz)
                 return pts2d_cam / pts2d_cam[2]
             else:
                 return None
     else:
-        raise ValueError('frame_calib must be an LidarCamCalibData type')
+        raise ValueError("frame_calib must be an LidarCamCalibData type")
 
 
 def load_pc_from_file(v_f):
     return np.fromfile(v_f, dtype=np.float32, count=-1).reshape([-1, 4])
-# ------------------------------ Drawing utilities ------------------------------------------
 
+
+# ------------------------------ Drawing utilities ------------------------------------------
```

### Comparing `alfred-py-3.0.6/alfred/fusion/nuscenes_fusion.py` & `alfred-py-3.0.7/alfred/fusion/nuscenes_fusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,21 @@
     [[-1.9, 0.12, 37]] -> [[222, 345]]
     """
     intrinsic = np.array(intrinsic)
     pts3d_cam = np.array(pts3d_cam)
     if pts3d_cam.shape[0] != 3:
         # if not hstack, try to transpose it
         pts3d_cam = pts3d_cam.T
-    assert pts3d_cam.shape[0] == 3, 'pts3d_cam must be 3 rows.'
-    assert intrinsic.shape == (3, 3), 'intrinsic should be 3x3.'
+    assert pts3d_cam.shape[0] == 3, "pts3d_cam must be 3 rows."
+    assert intrinsic.shape == (3, 3), "intrinsic should be 3x3."
     a = np.dot(intrinsic, pts3d_cam)
-    a = a/a[-1, :]
+    a = a / a[-1, :]
     return a.T[:, :2]
 
+
 # def compute_3d_box_cam_coords_nuscenes(xyz, lwh, quarternion):
 #     """
 #         nuScenes camera coordinates using -y as up
 #         using quarternion represents rotation of box
 #     """
 #     # we get rotation_y from quarternion first
 #     quarternion = Quaternion(axis=quarternion[1:], angle=quarternion[0])
@@ -70,36 +71,38 @@
 #     corners4d_trans = np.dot(trans_m, corners4d)
 #     print('corners4d_trans: ', corners4d_trans)
 #     return corners4d_trans
 
 
 def compute_3d_box_cam_coords_nuscenes(xyz, lwh, quarternion):
     """
-        nuScenes camera coordinates using -y as up
-        using quarternion represents rotation of box
+    nuScenes camera coordinates using -y as up
+    using quarternion represents rotation of box
 
-        only calculate rotation_y?: arcsin(2(wy-zx))
+    only calculate rotation_y?: arcsin(2(wy-zx))
     """
     # we get rotation_y from quarternion first
     if isinstance(quarternion, Quaternion):
         l, w, h = lwh[0], lwh[1], lwh[2]
         x_corners = [l / 2, l / 2, -l / 2, -l / 2, l / 2, l / 2, -l / 2, -l / 2]
         # y_corners = [0, 0, 0, 0, -h, -h, -h, -h]
-        y_corners = [-h/2, -h/2, -h/2, -h/2, h/2, h/2, h/2, h/2]
+        y_corners = [-h / 2, -h / 2, -h / 2, -h / 2, h / 2, h / 2, h / 2, h / 2]
         z_corners = [w / 2, -w / 2, -w / 2, w / 2, w / 2, -w / 2, -w / 2, w / 2]
         corners = np.array([x_corners, y_corners, z_corners], dtype=np.float32)
 
-        rotation_y = np.pi/2 - quarternion.radians
+        rotation_y = np.pi / 2 - quarternion.radians
         c, s = np.cos(rotation_y), np.sin(rotation_y)
         R = np.array([[c, 0, s], [0, 1, 0], [-s, 0, c]], dtype=np.float32)
 
         corners_trans = np.dot(R, corners)
         corners_trans += [[i] for i in xyz]
         return corners_trans
     else:
-        raise ValueError('quarternion must be a Quaternion object, make sure '\
-            'you using pyquarternion.')
+        raise ValueError(
+            "quarternion must be a Quaternion object, make sure "
+            "you using pyquarternion."
+        )
 
 
 def load_pc_from_file(pc_f):
     # nuScenes lidar is 5 digits one line (last one the ring index)
-    return np.fromfile(pc_f, dtype=np.float32, count=-1).reshape([-1, 5])
+    return np.fromfile(pc_f, dtype=np.float32, count=-1).reshape([-1, 5])
```

### Comparing `alfred-py-3.0.6/alfred/modules/__init__.py` & `alfred-py-3.0.7/alfred/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/__init__.py` & `alfred-py-3.0.7/alfred/modules/cabinet/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/changesource.py` & `alfred-py-3.0.7/alfred/modules/cabinet/changesource.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     else:
         return False
 
 
 def mkfile(filePath):
     pipfile = "[global]\ntrusted-host=mirrors.aliyun.com\nindex-url=http://mirrors.aliyun.com/pypi/simple/"
     if os.path.exists(filePath):
-        if str(input("File exist!Cover?(Y/N))")).upper() == 'N':
+        if str(input("File exist!Cover?(Y/N))")).upper() == "N":
             print("Not Cover.")
             return
-    with open(filePath, 'w') as fp:
+    with open(filePath, "w") as fp:
         fp.write(pipfile)
     print("Write finish.")
 
 
 def change_pypi_source():
     systype = platform.system()
     print("System type: " + systype)
     if systype == "Windows":
-        path = os.path.join(os.getenv('HOMEPATH'), 'pip')
+        path = os.path.join(os.getenv("HOMEPATH"), "pip")
         mkdir(path)
-        mkfile(os.path.join(path, 'pip.ini'))
+        mkfile(os.path.join(path, "pip.ini"))
     elif systype == "Linux" or systype == "Darwin":
-        path = os.path.join(os.path.expandvars('$HOME'), ".pip")
+        path = os.path.join(os.path.expandvars("$HOME"), ".pip")
         mkdir(path)
-        mkfile(os.path.join(path, 'pip.conf'))
+        mkfile(os.path.join(path, "pip.conf"))
     else:
         print("System type: " + systype + " Not Support!")
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/count_file.py` & `alfred-py-3.0.7/alfred/modules/cabinet/count_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,21 +27,20 @@
 
 """
 import os
 import glob
 from alfred.utils.log import logger as logging
 
 
-
 def count_file(d, f_type):
-    assert os.path.exists(d), '{} not exist.'.format(d)
+    assert os.path.exists(d), "{} not exist.".format(d)
     # f_type can be jpg,png,pdf etc, connected by comma
-    all_types = f_type.split(',')
-    logging.info('count all file types: {} under: {}'.format(all_types, d))
+    all_types = f_type.split(",")
+    logging.info("count all file types: {} under: {}".format(all_types, d))
     all_files = []
     for t in all_types:
-        t = t.replace('.', '')
-        one = glob.glob(os.path.join(d, '*.{}'.format(t)))
+        t = t.replace(".", "")
+        one = glob.glob(os.path.join(d, "*.{}".format(t)))
         one = [i for i in one if os.path.isfile(i)]
-        logging.info('{} num: {}'.format(t, len(one)))
+        logging.info("{} num: {}".format(t, len(one)))
         all_files.extend(one)
-    logging.info('file types: {}, total num: {}'.format(all_types, len(all_files)))
+    logging.info("file types: {}, total num: {}".format(all_types, len(all_files)))
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/gtrend.py` & `alfred-py-3.0.7/alfred/modules/cabinet/gtrend.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,14 @@
 def grid_layout(repos):
     """Displays repositories in a grid format using rich"""
 
     max_desc_len = 90
 
     panels = []
     for repo in repos:
-
         stats = get_stats(repo)
         # '\n' added here as it would group both text and new line together
         # hence if date_range isn't present the new line will also not be displayed
         date_range_str = (
             repo["date_range"].replace("stars", "⭐") + "\n"
             if "date_range" in repo.keys() and repo["date_range"]
             else ""
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/license.py` & `alfred-py-3.0.7/alfred/modules/cabinet/license.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,162 +37,163 @@
 
 LOGGER = logger
 
 type_settings = {
     "java": {
         "extensions": [".java", ".scala", ".groovy", ".jape", ".js"],
         "keepFirst": None,
-        "blockCommentStartPattern": re.compile(r'^\s*/\*'),
-        "blockCommentEndPattern": re.compile(r'\*/\s*$'),
-        "lineCommentStartPattern": re.compile(r'\s*//'),
+        "blockCommentStartPattern": re.compile(r"^\s*/\*"),
+        "blockCommentEndPattern": re.compile(r"\*/\s*$"),
+        "lineCommentStartPattern": re.compile(r"\s*//"),
         "lineCommentEndPattern": None,
         "headerStartLine": "/*\n",
         "headerEndLine": " */\n",
         "headerLinePrefix": " * ",
         "headerLineSuffix": None,
     },
     "script": {
         "extensions": [".sh", ".csh", ".py", ".pl"],
-        "keepFirst": re.compile(r'^#!|^# -\*-'),
+        "keepFirst": re.compile(r"^#!|^# -\*-"),
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
-        "lineCommentStartPattern": re.compile(r'\s*#'),
+        "lineCommentStartPattern": re.compile(r"\s*#"),
         "lineCommentEndPattern": None,
         "headerStartLine": "##\n",
         "headerEndLine": "##\n",
         "headerLinePrefix": "## ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "perl": {
         "extensions": [".pl"],
-        "keepFirst": re.compile(r'^#!|^# -\*-'),
+        "keepFirst": re.compile(r"^#!|^# -\*-"),
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
-        "lineCommentStartPattern": re.compile(r'\s*#'),
+        "lineCommentStartPattern": re.compile(r"\s*#"),
         "lineCommentEndPattern": None,
         "headerStartLine": "##\n",
         "headerEndLine": "##\n",
         "headerLinePrefix": "## ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "python": {
         "extensions": [".py"],
-        "keepFirst": re.compile(r'^#!|^# +pylint|^# +-\*-|^# +coding|^# +encoding'),
+        "keepFirst": re.compile(r"^#!|^# +pylint|^# +-\*-|^# +coding|^# +encoding"),
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
-        "lineCommentStartPattern": re.compile(r'\s*#'),
+        "lineCommentStartPattern": re.compile(r"\s*#"),
         "lineCommentEndPattern": None,
         "headerStartLine": "#\n",
         "headerEndLine": "#\n",
         "headerLinePrefix": "# ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "robot": {
         "extensions": [".robot"],
-        "keepFirst": re.compile(r'^#!|^# +pylint|^# +-\*-|^# +coding|^# +encoding'),
+        "keepFirst": re.compile(r"^#!|^# +pylint|^# +-\*-|^# +coding|^# +encoding"),
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
-        "lineCommentStartPattern": re.compile(r'\s*#'),
+        "lineCommentStartPattern": re.compile(r"\s*#"),
         "lineCommentEndPattern": None,
         "headerStartLine": None,
         "headerEndLine": None,
         "headerLinePrefix": "# ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "xml": {
         "extensions": [".xml"],
-        "keepFirst": re.compile(r'^\s*<\?xml.*\?>'),
-        "blockCommentStartPattern": re.compile(r'^\s*<!--'),
-        "blockCommentEndPattern": re.compile(r'-->\s*$'),
+        "keepFirst": re.compile(r"^\s*<\?xml.*\?>"),
+        "blockCommentStartPattern": re.compile(r"^\s*<!--"),
+        "blockCommentEndPattern": re.compile(r"-->\s*$"),
         "lineCommentStartPattern": None,
         "lineCommentEndPattern": None,
         "headerStartLine": "<!--\n",
         "headerEndLine": "  -->\n",
         "headerLinePrefix": "-- ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "sql": {
         "extensions": [".sql"],
         "keepFirst": None,
         "blockCommentStartPattern": None,  # re.compile('^\s*/\*'),
         "blockCommentEndPattern": None,  # re.compile(r'\*/\s*$'),
-        "lineCommentStartPattern": re.compile(r'\s*--'),
+        "lineCommentStartPattern": re.compile(r"\s*--"),
         "lineCommentEndPattern": None,
         "headerStartLine": "--\n",
         "headerEndLine": "--\n",
         "headerLinePrefix": "-- ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "c": {
         "extensions": [".c", ".cc", ".cpp", "c++", ".h", ".hpp"],
         "keepFirst": None,
-        "blockCommentStartPattern": re.compile(r'^\s*/\*'),
-        "blockCommentEndPattern": re.compile(r'\*/\s*$'),
-        "lineCommentStartPattern": re.compile(r'\s*//'),
+        "blockCommentStartPattern": re.compile(r"^\s*/\*"),
+        "blockCommentEndPattern": re.compile(r"\*/\s*$"),
+        "lineCommentStartPattern": re.compile(r"\s*//"),
         "lineCommentEndPattern": None,
         "headerStartLine": "/*\n",
         "headerEndLine": " */\n",
         "headerLinePrefix": " * ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "ruby": {
         "extensions": [".rb"],
         "keepFirst": "^#!",
-        "blockCommentStartPattern": re.compile('^=begin'),
-        "blockCommentEndPattern": re.compile(r'^=end'),
-        "lineCommentStartPattern": re.compile(r'\s*#'),
+        "blockCommentStartPattern": re.compile("^=begin"),
+        "blockCommentEndPattern": re.compile(r"^=end"),
+        "lineCommentStartPattern": re.compile(r"\s*#"),
         "lineCommentEndPattern": None,
         "headerStartLine": "##\n",
         "headerEndLine": "##\n",
         "headerLinePrefix": "## ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "csharp": {
         "extensions": [".cs"],
         "keepFirst": None,
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
-        "lineCommentStartPattern": re.compile(r'\s*//'),
+        "lineCommentStartPattern": re.compile(r"\s*//"),
         "lineCommentEndPattern": None,
         "headerStartLine": None,
         "headerEndLine": None,
         "headerLinePrefix": "// ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "vb": {
         "extensions": [".vb"],
         "keepFirst": None,
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
         "lineCommentStartPattern": re.compile(r"^\s*\'"),
         "lineCommentEndPattern": None,
         "headerStartLine": None,
         "headerEndLine": None,
         "headerLinePrefix": "' ",
-        "headerLineSuffix": None
+        "headerLineSuffix": None,
     },
     "erlang": {
         "extensions": [".erl", ".src", ".config", ".schema"],
         "keepFirst": None,
         "blockCommentStartPattern": None,
         "blockCommentEndPattern": None,
         "lineCommentStartPattern": None,
         "lineCommentEndPattern": None,
         "headerStartLine": "%% -*- erlang -*-\n%% %CopyrightBegin%\n%%\n",
         "headerEndLine": "%%\n%% %CopyrightEnd%\n\n",
         "headerLinePrefix": "%% ",
         "headerLineSuffix": None,
-    }
+    },
 }
 
 years_pattern = re.compile(
     r"(?<=Copyright\s*(?:\(\s*[Cc©]\s*\)\s*))?([0-9][0-9][0-9][0-9](?:-[0-9][0-9]?[0-9]?[0-9]?)?)",
-    re.IGNORECASE)
+    re.IGNORECASE,
+)
 licensePattern = re.compile(r"license", re.IGNORECASE)
-emptyPattern = re.compile(r'^\s*$')
+emptyPattern = re.compile(r"^\s*$")
 
 # maps each extension to its processing type. Filled from tpeSettings during initialization
 ext2type = {}
 patterns = []
 
 
 # class for dict args. Use --argname key1=val1,val2 key2=val3 key3=val4, val5
@@ -200,15 +201,17 @@
     def __call__(self, parser, namespace, values, option_string=None):
         dict_args = {}
         if not isinstance(values, (list,)):
             values = (values,)
         for value in values:
             n, v = value.split("=")
             if n not in type_settings:
-                LOGGER.error("No valid language '%s' to add additional file extensions for" % n)
+                LOGGER.error(
+                    "No valid language '%s' to add additional file extensions for" % n
+                )
             if v and "," in str(v):
                 dict_args[n] = v.split(",")
             else:
                 dict_args[n] = list()
                 dict_args[n].append(str(v).strip())
         setattr(namespace, self.dest, dict_args)
 
@@ -238,15 +241,15 @@
     Read a template file replace variables from the dict and return the lines.
     Throws exception if a variable cannot be replaced.
     :param template_file: template file with variables
     :param vardict: dictionary to replace variables with values
     :param safe_subst:
     :return: lines of the template, with variables replaced
     """
-    with open(template_file, 'r') as f:
+    with open(template_file, "r") as f:
         lines = f.readlines()
     if safe_subst:
         lines = [Template(line).safe_substitute(vardict) for line in lines]
     else:
         lines = [Template(line).substitute(vardict) for line in lines]
     return lines
 
@@ -264,28 +267,28 @@
     header_end_line = settings["headerEndLine"]
     header_line_prefix = settings["headerLinePrefix"]
     header_line_suffix = settings["headerLineSuffix"]
     if header_start_line is not None:
         lines.append(header_start_line)
     for line in templatelines:
         tmp = line
-        if header_line_prefix is not None and line == '\n':
+        if header_line_prefix is not None and line == "\n":
             tmp = header_line_prefix.rstrip() + tmp
         elif header_line_prefix is not None:
             tmp = header_line_prefix + tmp
         if header_line_suffix is not None:
             tmp = tmp + header_line_suffix
         lines.append(tmp)
     if header_end_line is not None:
         lines.append(header_end_line)
     return lines
 
 
 ##
-def read_file(file, encoding='utf-8'):
+def read_file(file, encoding="utf-8"):
     """
     Read a file and return a dictionary with the following elements:
     :param file: the file to read
     :param encoding: the options specified by the user
     :return: a dictionary with the following entries or None if the file is not supported:
       - skip: number of lines at the beginning to skip (always keep them when replacing or adding something)
        can also be seen as the index of the first line not to skip
@@ -304,15 +307,15 @@
     LOGGER.debug("File extension is %s", extension)
     # if we have no entry in the mapping from extensions to processing type, return None
     ftype = ext2type.get(extension)
     logging.debug("Type for this file is %s", ftype)
     if not ftype:
         return None
     settings = type_settings.get(ftype)
-    with open(file, 'r', encoding=encoding) as f:
+    with open(file, "r", encoding=encoding) as f:
         lines = f.readlines()
     # now iterate throw the lines and try to determine the various indies
     # first try to find the start of the header: skip over shebang or empty lines
     keep_first = settings.get("keepFirst")
     block_comment_start_pattern = settings.get("blockCommentStartPattern")
     block_comment_end_pattern = settings.get("blockCommentEndPattern")
     line_comment_start_pattern = settings.get("lineCommentStartPattern")
@@ -325,149 +328,173 @@
             pass
         elif block_comment_start_pattern and block_comment_start_pattern.findall(line):
             head_start = i
             break
         elif line_comment_start_pattern and line_comment_start_pattern.findall(line):
             head_start = i
             break
-        elif not block_comment_start_pattern and \
-                line_comment_start_pattern and \
-                line_comment_start_pattern.findall(line):
+        elif (
+            not block_comment_start_pattern
+            and line_comment_start_pattern
+            and line_comment_start_pattern.findall(line)
+        ):
             head_start = i
             break
         else:
             # we have reached something else, so no header in this file
             # logging.debug("Did not find the start giving up at line %s, line is >%s<",i,line)
-            return {"type": ftype,
-                    "lines": lines,
-                    "skip": skip,
-                    "headStart": None,
-                    "headEnd": None,
-                    "yearsLine": None,
-                    "settings": settings,
-                    "haveLicense": have_license
-                    }
+            return {
+                "type": ftype,
+                "lines": lines,
+                "skip": skip,
+                "headStart": None,
+                "headEnd": None,
+                "yearsLine": None,
+                "settings": settings,
+                "haveLicense": have_license,
+            }
         i = i + 1
-    LOGGER.debug("Found preliminary start at {}, i={}, lines={}".format(head_start, i, len(lines)))
+    LOGGER.debug(
+        "Found preliminary start at {}, i={}, lines={}".format(
+            head_start, i, len(lines)
+        )
+    )
     # now we have either reached the end, or we are at a line where a block start or line comment occurred
     # if we have reached the end, return default dictionary without info
     if i == len(lines):
         LOGGER.debug("We have reached the end, did not find anything really")
-        return {"type": ftype,
-                "lines": lines,
-                "skip": skip,
-                "headStart": head_start,
-                "headEnd": head_end,
-                "yearsLine": years_line,
-                "settings": settings,
-                "haveLicense": have_license
-                }
+        return {
+            "type": ftype,
+            "lines": lines,
+            "skip": skip,
+            "headStart": head_start,
+            "headEnd": head_end,
+            "yearsLine": years_line,
+            "settings": settings,
+            "haveLicense": have_license,
+        }
     # otherwise process the comment block until it ends
     if block_comment_start_pattern:
         LOGGER.debug("Found comment start, process until end")
         for j in range(i, len(lines)):
             LOGGER.debug("Checking line {}".format(j))
             if licensePattern.findall(lines[j]):
                 have_license = True
             elif block_comment_end_pattern.findall(lines[j]):
-                return {"type": ftype,
-                        "lines": lines,
-                        "skip": skip,
-                        "headStart": head_start,
-                        "headEnd": j,
-                        "yearsLine": years_line,
-                        "settings": settings,
-                        "haveLicense": have_license
-                        }
+                return {
+                    "type": ftype,
+                    "lines": lines,
+                    "skip": skip,
+                    "headStart": head_start,
+                    "headEnd": j,
+                    "yearsLine": years_line,
+                    "settings": settings,
+                    "haveLicense": have_license,
+                }
             elif years_pattern.findall(lines[j]):
                 have_license = True
                 years_line = j
         # if we went through all the lines without finding an end, maybe we have some syntax error or some other
         # unusual situation, so lets return no header
         LOGGER.debug("Did not find the end of a block comment, returning no header")
-        return {"type": ftype,
-                "lines": lines,
-                "skip": skip,
-                "headStart": None,
-                "headEnd": None,
-                "yearsLine": None,
-                "settings": settings,
-                "haveLicense": have_license
-                }
+        return {
+            "type": ftype,
+            "lines": lines,
+            "skip": skip,
+            "headStart": None,
+            "headEnd": None,
+            "yearsLine": None,
+            "settings": settings,
+            "haveLicense": have_license,
+        }
     else:
         LOGGER.debug("ELSE1")
         for j in range(i, len(lines)):
-            if line_comment_start_pattern.findall(lines[j]) and licensePattern.findall(lines[j]):
+            if line_comment_start_pattern.findall(lines[j]) and licensePattern.findall(
+                lines[j]
+            ):
                 have_license = True
             elif not line_comment_start_pattern.findall(lines[j]):
                 LOGGER.debug("ELSE2")
-                return {"type": ftype,
-                        "lines": lines,
-                        "skip": skip,
-                        "headStart": i,
-                        "headEnd": j - 1,
-                        "yearsLine": years_line,
-                        "settings": settings,
-                        "haveLicense": have_license
-                        }
+                return {
+                    "type": ftype,
+                    "lines": lines,
+                    "skip": skip,
+                    "headStart": i,
+                    "headEnd": j - 1,
+                    "yearsLine": years_line,
+                    "settings": settings,
+                    "haveLicense": have_license,
+                }
             elif years_pattern.findall(lines[j]):
                 have_license = True
                 years_line = j
         # if we went through all the lines without finding the end of the block, it could be that the whole
         # file only consisted of the header, so lets return the last line index
         LOGGER.debug("RETURN")
-        return {"type": ftype,
-                "lines": lines,
-                "skip": skip,
-                "headStart": i,
-                "headEnd": len(lines) - 1,
-                "yearsLine": years_line,
-                "settings": settings,
-                "haveLicense": have_license
-                }
+        return {
+            "type": ftype,
+            "lines": lines,
+            "skip": skip,
+            "headStart": i,
+            "headEnd": len(lines) - 1,
+            "yearsLine": years_line,
+            "settings": settings,
+            "haveLicense": have_license,
+        }
 
 
 def make_backup(file, arguments):
     """
     Backup file by copying it to a file with the extension .bak appended to the name.
     :param file: file to back up
     :param arguments: program args, only backs up, if required by an option
     :return:
     """
     if arguments.b:
         LOGGER.info("Backing up file {} to {}".format(file, file + ".bak"))
         copyfile(file, file + ".bak")
 
 
-def apply_license(owner, proj_n, year=None, url='google.com', files_dir='./', tmpl='apache-2', rm_old=True):
+def apply_license(
+    owner,
+    proj_n,
+    year=None,
+    url="google.com",
+    files_dir="./",
+    tmpl="apache-2",
+    rm_old=True,
+):
     """
     Apply new license to all files under target dir
     :param year:
     :param owner:
     :param proj_n:
     :param url:
     :param files_dir:
     :param tmpl:
     :param rm_old:
     :return:
     """
     if not year:
         year = datetime.now().year
-        logger.info('year not specific, using year: {}'.format(year))
-    logger.info('owner: {}'.format(owner))
-    logger.info('project name: {}'.format(proj_n))
-    logger.info('start apply license under: {}'.format(files_dir))
+        logger.info("year not specific, using year: {}".format(year))
+    logger.info("owner: {}".format(owner))
+    logger.info("project name: {}".format(proj_n))
+    logger.info("start apply license under: {}".format(files_dir))
     additional_extensions = []
     for t in type_settings:
         settings = type_settings[t]
         exts = settings["extensions"]
         # if additional file extensions are provided by the user, they are "merged" here:
         if additional_extensions and t in additional_extensions:
             for aext in additional_extensions[t]:
-                LOGGER.debug("Enable custom file extension '%s' for language '%s'" % (aext, t))
+                LOGGER.debug(
+                    "Enable custom file extension '%s' for language '%s'" % (aext, t)
+                )
                 exts.append(aext)
 
         for ext in exts:
             ext2type[ext] = t
             patterns.append("*" + ext)
 
     LOGGER.debug("Allowed file patterns %s" % patterns)
@@ -479,18 +506,20 @@
         settings["years"] = year
         settings["owner"] = owner
         settings["projectname"] = proj_n
         settings["projecturl"] = url
 
         # if we have a template name specified, try to get or load the template
         opt_tmpl = tmpl
-        LOGGER.info('using license TEMPLATE: {}'.format(tmpl))
+        LOGGER.info("using license TEMPLATE: {}".format(tmpl))
         # first get all the names of our own templates
         # for this get first the path of this file
-        templates_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "templates")
+        templates_dir = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)), "templates"
+        )
         if not os.path.exists(templates_dir):
             LOGGER.error("can not found templates dir! {}".format(templates_dir))
             exit(-1)
         LOGGER.info("File path: {}".format(os.path.abspath(__file__)))
         # get all the templates in the templates directory
         templates = [f for f in get_paths("*.tmpl", templates_dir)]
         templates = [(os.path.splitext(os.path.basename(t))[0], t) for t in templates]
@@ -508,19 +537,31 @@
         else:
             if len(tmpls) == 0:
                 # check if we can interpret the option as file
                 if os.path.isfile(opt_tmpl):
                     LOGGER.info("Using file {}".format(os.path.abspath(opt_tmpl)))
                     template_lines = read_template(os.path.abspath(opt_tmpl), settings)
                 else:
-                    LOGGER.error("Not a built-in template and not a file, cannot proceed: {}".format(opt_tmpl))
-                    LOGGER.error("Built in templates: {}".format(", ".join([t[0] for t in templates])))
+                    LOGGER.error(
+                        "Not a built-in template and not a file, cannot proceed: {}".format(
+                            opt_tmpl
+                        )
+                    )
+                    LOGGER.error(
+                        "Built in templates: {}".format(
+                            ", ".join([t[0] for t in templates])
+                        )
+                    )
                     error = True
             else:
-                LOGGER.error("There are multiple matching template names: {}".format([t[0] for t in tmpls]))
+                LOGGER.error(
+                    "There are multiple matching template names: {}".format(
+                        [t[0] for t in tmpls]
+                    )
+                )
                 error = True
 
         if not error:
             # logging.debug("Got template lines: %s",templateLines)
             # now do the actual processing: if we did not get some error, we have a template loaded or
             # no template at all
             # if we have no template, then we will have the years.
@@ -534,46 +575,61 @@
                 if not finfo:
                     LOGGER.debug("File not supported %s", file)
                     continue
                 # logging.debug("FINFO for the file: %s", finfo)
                 lines = finfo["lines"]
                 LOGGER.debug(
                     "Info for the file: headStart=%s, headEnd=%s, haveLicense=%s, skip=%s, len=%s, yearsline=%s",
-                    finfo["headStart"], finfo["headEnd"], finfo["haveLicense"], finfo["skip"], len(lines),
-                    finfo["yearsLine"])
+                    finfo["headStart"],
+                    finfo["headEnd"],
+                    finfo["haveLicense"],
+                    finfo["skip"],
+                    len(lines),
+                    finfo["yearsLine"],
+                )
                 # if we have a template: replace or add
                 if template_lines:
                     # make_backup(file, arguments)
-                    with open(file, 'w', encoding='utf-8') as fw:
+                    with open(file, "w", encoding="utf-8") as fw:
                         # if we found a header, replace it
                         # otherwise, add it after the lines to skip
                         head_start = finfo["headStart"]
                         head_end = finfo["headEnd"]
                         have_license = finfo["haveLicense"]
                         ftype = finfo["type"]
                         skip = finfo["skip"]
-                        if head_start is not None and head_end is not None and have_license:
+                        if (
+                            head_start is not None
+                            and head_end is not None
+                            and have_license
+                        ):
                             LOGGER.debug("Replacing header in file {}".format(file))
                             # first write the lines before the header
                             fw.writelines(lines[0:head_start])
                             #  now write the new header from the template lines
                             fw.writelines(for_type(template_lines, ftype))
                             #  now write the rest of the lines
-                            fw.writelines(lines[head_end + 1:])
+                            fw.writelines(lines[head_end + 1 :])
                         else:
-                            LOGGER.debug("Adding header to file {}, skip={}".format(file, skip))
+                            LOGGER.debug(
+                                "Adding header to file {}, skip={}".format(file, skip)
+                            )
                             fw.writelines(lines[0:skip])
                             fw.writelines(for_type(template_lines, ftype))
                             fw.writelines(lines[skip:])
                     # TODO: optionally remove backup if all worked well?
                 else:
                     # no template lines, just update the line with the year, if we found a year
                     years_line = finfo["yearsLine"]
                     if years_line is not None:
                         # make_backup(file, arguments)
-                        with open(file, 'w', encoding='utf-8') as fw:
-                            LOGGER.debug("Updating years in file {} in line {}".format(file, years_line))
+                        with open(file, "w", encoding="utf-8") as fw:
+                            LOGGER.debug(
+                                "Updating years in file {} in line {}".format(
+                                    file, years_line
+                                )
+                            )
                             fw.writelines(lines[0:years_line])
                             fw.write(years_pattern.sub(year, lines[years_line]))
-                            fw.writelines(lines[years_line + 1:])
+                            fw.writelines(lines[years_line + 1 :])
     finally:
         logging.shutdown()
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/markdown_tool.py` & `alfred-py-3.0.7/alfred/modules/cabinet/markdown_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,142 +11,190 @@
 from mimetypes import types_map
 
 from .mdparse.transformers.md.transformer import ArticleTransformer
 from .mdparse.image_downloader import ImageDownloader
 from .mdparse.www_tools import is_url, get_filename_from_url, download_from_url
 from .mdparse.formatters.simple import SimpleFormatter
 from .mdparse.formatters.html import HTMLFormatter
+
 try:
     from .mdparse.formatters.pdf import PDFFormatter
 except ModuleNotFoundError:
     PDFFormatter = None
 
 
-__version__ = '0.0.4'
+__version__ = "0.0.4"
 FORMATTERS = [SimpleFormatter, HTMLFormatter, PDFFormatter]
-del types_map['.jpe']
+del types_map[".jpe"]
 
 
 def download_images_from_md(md_f):
     article_link = md_f
     if is_url(article_link):
-        response = download_from_url(
-            article_link, timeout=-1)
+        response = download_from_url(article_link, timeout=-1)
         article_path = get_filename_from_url(response)
 
-        with open(article_path, 'wb') as article_file:
+        with open(article_path, "wb") as article_file:
             article_file.write(response.content)
             article_file.close()
     else:
         article_path = os.path.expanduser(article_link)
 
-    img_dir_name = os.path.basename(article_path).split('.')[0]
-    img_dir_name = os.path.join('images', img_dir_name)
+    img_dir_name = os.path.basename(article_path).split(".")[0]
+    img_dir_name = os.path.join("images", img_dir_name)
     os.makedirs(img_dir_name, exist_ok=True)
 
     img_downloader = ImageDownloader(
         article_path=article_path,
         skip_list=[],
         skip_all_errors=True,
         img_dir_name=img_dir_name,
-        img_public_path='',
+        img_public_path="",
         downloading_timeout=-1,
-        deduplication=False
+        deduplication=False,
     )
 
     result = ArticleTransformer(article_path, img_downloader).run()
-    print('Done.')
+    print("Done.")
 
 
 def main(arguments):
     """
     Entrypoint.
     """
 
-    print(f'Markdown tool version {__version__} started...')
+    print(f"Markdown tool version {__version__} started...")
 
     article_link = arguments.article_file_path_or_url
     if is_url(article_link):
         response = download_from_url(
-            article_link, timeout=arguments.downloading_timeout)
+            article_link, timeout=arguments.downloading_timeout
+        )
         article_path = get_filename_from_url(response)
 
-        with open(article_path, 'wb') as article_file:
+        with open(article_path, "wb") as article_file:
             article_file.write(response.content)
             article_file.close()
     else:
         article_path = os.path.expanduser(article_link)
 
     skip_list = arguments.skip_list
     skip_all = arguments.skip_all_incorrect
 
     print(f'File "{article_path}" will be processed...')
 
     if isinstance(skip_list, str):
-        if skip_list.startswith('@'):
+        if skip_list.startswith("@"):
             skip_list = skip_list[1:]
             print(f'Reading skip list from a file "{skip_list}"...')
-            with open(os.path.expanduser(skip_list), 'r') as fsl:
+            with open(os.path.expanduser(skip_list), "r") as fsl:
                 skip_list = [s.strip() for s in fsl.readlines()]
         else:
-            skip_list = [s.strip() for s in skip_list.split(',')]
+            skip_list = [s.strip() for s in skip_list.split(",")]
 
     img_downloader = ImageDownloader(
         article_path=article_path,
         skip_list=skip_list,
         skip_all_errors=skip_all,
         img_dir_name=arguments.images_dirname,
         img_public_path=arguments.images_publicpath,
         downloading_timeout=arguments.downloading_timeout,
-        deduplication=arguments.dedup_with_hash
+        deduplication=arguments.dedup_with_hash,
     )
 
     result = ArticleTransformer(article_path, img_downloader).run()
 
     formatter = [
-        f for f in FORMATTERS if f is not None and f.format == arguments.output_format]
+        f for f in FORMATTERS if f is not None and f.format == arguments.output_format
+    ]
     assert len(formatter) == 1
     formatter = formatter[0]
 
     article_file_name = os.path.splitext(article_path)[0]
-    article_out_path = f'{article_file_name}.{formatter.format}'
+    article_out_path = f"{article_file_name}.{formatter.format}"
     if article_path == article_out_path and not arguments.remove_source:
-        article_out_path = f'{article_file_name}_{strftime("%Y%m%d_%H%M%S")}.{formatter.format}'
+        article_out_path = (
+            f'{article_file_name}_{strftime("%Y%m%d_%H%M%S")}.{formatter.format}'
+        )
     print(f'Writing file into "{article_out_path}"...')
 
-    with open(article_out_path, 'wb') as outfile:
+    with open(article_out_path, "wb") as outfile:
         outfile.write(formatter.write(result))
 
     if arguments.remove_source and article_path != article_out_path:
         os.remove(article_path)
 
-    print('Processing finished successfully...')
+    print("Processing finished successfully...")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     out_format_list = [f.format for f in FORMATTERS if f is not None]
 
     parser = argparse.ArgumentParser(description=__doc__)
-    parser.add_argument('article_file_path_or_url', type=str,
-                        help='path to the article file in the Markdown format')
-    parser.add_argument('-s', '--skip-list', default=None,
-                        help='skip URL\'s from the comma-separated list (or file with a leading \'@\')')
-    parser.add_argument('-d', '--images-dirname', default='images',
-                        help='Folder in which to download images')
-    parser.add_argument('-p', '--images-publicpath', default='',
-                        help='Public path to the folder of downloaded images')
-    parser.add_argument('-a', '--skip-all-incorrect', default=False, action='store_true',
-                        help='skip all incorrect images')
-    parser.add_argument('-t', '--downloading-timeout', type=float, default=-1,
-                        help='how many seconds to wait before downloading will be failed')
-    parser.add_argument('-D', '--dedup-with-hash', default=False, action='store_true',
-                        help='Deduplicate images, using content hash')
-    parser.add_argument('-R', '--remove-source', default=False, action='store_true',
-                        help='Remove or replace source file')
-    parser.add_argument('-o', '--output-format', default=out_format_list[0], choices=out_format_list,
-                        help='output format')
-    parser.add_argument('--version', action='version',
-                        version=f'%(prog)s {__version__}', help='return version number')
+    parser.add_argument(
+        "article_file_path_or_url",
+        type=str,
+        help="path to the article file in the Markdown format",
+    )
+    parser.add_argument(
+        "-s",
+        "--skip-list",
+        default=None,
+        help="skip URL's from the comma-separated list (or file with a leading '@')",
+    )
+    parser.add_argument(
+        "-d",
+        "--images-dirname",
+        default="images",
+        help="Folder in which to download images",
+    )
+    parser.add_argument(
+        "-p",
+        "--images-publicpath",
+        default="",
+        help="Public path to the folder of downloaded images",
+    )
+    parser.add_argument(
+        "-a",
+        "--skip-all-incorrect",
+        default=False,
+        action="store_true",
+        help="skip all incorrect images",
+    )
+    parser.add_argument(
+        "-t",
+        "--downloading-timeout",
+        type=float,
+        default=-1,
+        help="how many seconds to wait before downloading will be failed",
+    )
+    parser.add_argument(
+        "-D",
+        "--dedup-with-hash",
+        default=False,
+        action="store_true",
+        help="Deduplicate images, using content hash",
+    )
+    parser.add_argument(
+        "-R",
+        "--remove-source",
+        default=False,
+        action="store_true",
+        help="Remove or replace source file",
+    )
+    parser.add_argument(
+        "-o",
+        "--output-format",
+        default=out_format_list[0],
+        choices=out_format_list,
+        help="output format",
+    )
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+        help="return version number",
+    )
 
     args = parser.parse_args()
 
     main(args)
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/formatters/pdf.py` & `alfred-py-3.0.7/alfred/modules/cabinet/mdparse/formatters/pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 
 class PDFFormatter:
     """
     Writes lines, into the PDF.
     """
 
-    format = 'pdf'
+    format = "pdf"
 
     @staticmethod
     def _fetcher(url):
         return weasyprint.default_url_fetcher(url, timeout=1)
 
     @staticmethod
     def write(lines):
-        return weasyprint.HTML(string=markdown(''.join(lines), output_format='html'),
-                               url_fetcher=PDFFormatter._fetcher).write_pdf()
+        return weasyprint.HTML(
+            string=markdown("".join(lines), output_format="html"),
+            url_fetcher=PDFFormatter._fetcher,
+        ).write_pdf()
 
         # with BytesIO() as result:
         #     pisa.pisaDocument(markdown(''.join(lines), output_format='html'), dest=result,
         #                       encoding='utf8',
         #                       link_callback=PDFFormatter._link_callback)
         #     result.seek(0)
         #     data = result.read()
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/image_downloader.py` & `alfred-py-3.0.7/alfred/modules/cabinet/mdparse/image_downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,35 @@
 
 
 class ImageDownloader:
     """
     "Smart" images downloader.
     """
 
-    def __init__(self, article_path: str, skip_list: Optional[List[str]] = None, skip_all_errors: bool = False,
-                 img_dir_name: str = 'images', img_public_path: str = '', downloading_timeout: float = -1,
-                 deduplication: bool = False):
+    def __init__(
+        self,
+        article_path: str,
+        skip_list: Optional[List[str]] = None,
+        skip_all_errors: bool = False,
+        img_dir_name: str = "images",
+        img_public_path: str = "",
+        downloading_timeout: float = -1,
+        deduplication: bool = False,
+    ):
         self._img_dir_name = img_dir_name
         self._img_public_path = img_public_path
         self._article_file_path = article_path
         self._skip_list = set(skip_list) if skip_list is not None else []
-        self._images_dir = os.path.join(os.path.dirname(self._article_file_path), self._img_dir_name)
+        self._images_dir = os.path.join(
+            os.path.dirname(self._article_file_path), self._img_dir_name
+        )
         self._skip_all_errors = skip_all_errors
-        self._downloading_timeout = downloading_timeout if downloading_timeout > 0 else None
+        self._downloading_timeout = (
+            downloading_timeout if downloading_timeout > 0 else None
+        )
         self._deduplication = deduplication
 
     def download_images(self, images: List[str]) -> dict:
         """
         Download and save images from the list.
 
         :return URL -> file path mapping.
@@ -42,52 +53,63 @@
         try:
             os.makedirs(self._images_dir)
         except FileExistsError:
             # Existing directory is not error.
             pass
 
         for img_num, img_url in enumerate(images):
-            assert img_url not in replacement_mapping.keys(), f'BUG: already downloaded image "{img_url}"...'
+            assert (
+                img_url not in replacement_mapping.keys()
+            ), f'BUG: already downloaded image "{img_url}"...'
 
             if img_url in skip_list:
-                print(f'Image {img_num + 1} ["{img_url}"] was skipped, because it\'s in the skip list...')
+                print(
+                    f'Image {img_num + 1} ["{img_url}"] was skipped, because it\'s in the skip list...'
+                )
                 continue
 
             if not is_url(img_url):
-                print(f'Image {img_num + 1} ["{img_url}"] was skipped, because it has incorrect URL...')
+                print(
+                    f'Image {img_num + 1} ["{img_url}"] was skipped, because it has incorrect URL...'
+                )
                 continue
 
             print(f'Downloading image {img_num + 1} of {img_count} from "{img_url}"...')
 
             try:
                 img_response = download_from_url(img_url, self._downloading_timeout)
             except Exception as e:
                 if self._skip_all_errors:
-                    print(f'Warning: can\'t download image {img_num + 1}, error: [{str(e)}], '
-                          'but processing will be continued, because `skip_all_errors` flag is set')
+                    print(
+                        f"Warning: can't download image {img_num + 1}, error: [{str(e)}], "
+                        "but processing will be continued, because `skip_all_errors` flag is set"
+                    )
                     continue
                 raise
 
             img_filename = get_filename_from_url(img_response)
             image_content = img_response.content
 
             if deduplication:
                 new_content_hash = hashlib.sha256(image_content).digest()
                 existed_file_name = hash_to_path_mapping.get(new_content_hash)
                 if existed_file_name is not None:
                     img_filename = existed_file_name
-                    document_img_path = path_join(img_public_path or img_dir_name, img_filename)
+                    document_img_path = path_join(
+                        img_public_path or img_dir_name, img_filename
+                    )
                     replacement_mapping.setdefault(img_url, document_img_path)
                     continue
                 else:
                     hash_to_path_mapping[new_content_hash] = img_filename
 
             document_img_path = path_join(img_public_path or img_dir_name, img_filename)
-            img_filename, document_img_path = self._correct_paths(replacement_mapping, document_img_path, img_url,
-                                                                  img_filename)
+            img_filename, document_img_path = self._correct_paths(
+                replacement_mapping, document_img_path, img_url, img_filename
+            )
 
             real_img_path = path_join(images_dir, img_filename)
             replacement_mapping.setdefault(img_url, document_img_path)
 
             ImageDownloader._write_image(real_img_path, image_content)
 
         return replacement_mapping
@@ -95,24 +117,30 @@
     @staticmethod
     def _write_image(img_path: str, data: bytes):
         """
         Write image data into the file.
         """
 
         print(f'Image will be written to the file "{img_path}"...')
-        with open(img_path, 'wb') as img_file:
+        with open(img_path, "wb") as img_file:
             img_file.write(data)
             img_file.close()
 
-    def _correct_paths(self, replacement_mapping, document_img_path, img_url, img_filename):
+    def _correct_paths(
+        self, replacement_mapping, document_img_path, img_url, img_filename
+    ):
         """
         Fix path if a file with the similar name exists already.
         """
 
         # Images can have similar name, but different URLs, but I want to save original filename, if possible.
         for url, path in replacement_mapping.items():
             if document_img_path == path and img_url != url:
-                img_filename = f'{hashlib.md5(img_url.encode()).hexdigest()}_{img_filename}'
-                document_img_path = os.path.join(self._img_public_path or self._img_dir_name, img_filename)
+                img_filename = (
+                    f"{hashlib.md5(img_url.encode()).hexdigest()}_{img_filename}"
+                )
+                document_img_path = os.path.join(
+                    self._img_public_path or self._img_dir_name, img_filename
+                )
                 break
 
         return img_filename, document_img_path
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/html/transformer.py` & `alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/html/transformer.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/transformers/md/transformer.py` & `alfred-py-3.0.7/alfred/modules/cabinet/mdparse/transformers/md/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,67 +5,69 @@
 import markdown
 from markdown.treeprocessors import Treeprocessor
 from markdown.extensions import Extension
 from markdown.inlinepatterns import SimpleTagPattern
 from typing import List
 
 
-__all__ = ['ArticleTransformer']
+__all__ = ["ArticleTransformer"]
 
 
 class ImgExtractor(Treeprocessor):
     def run(self, doc):
         """
         Find all images and append to markdown.images.
         """
 
         self.md.images = []
-        for image in doc.findall('.//img'):
-            self.md.images.append(image.get('src'))
+        for image in doc.findall(".//img"):
+            self.md.images.append(image.get("src"))
 
 
 class ImgExtExtension(Extension):
     def extendMarkdown(self, md, md_globals):
         img_ext = ImgExtractor(md)
-        md.treeprocessors.register(img_ext, 'imgext', 20)
+        md.treeprocessors.register(img_ext, "imgext", 20)
 
 
 class ArticleTransformer:
     """
     Markdown article transformation class.
     """
 
     def __init__(self, article_path: str, image_downloader):
         self._image_downloader = image_downloader
         self._article_file_path = article_path
-        self._md_conv = markdown.Markdown(extensions=[ImgExtExtension(), 'md_in_html'])
+        self._md_conv = markdown.Markdown(extensions=[ImgExtExtension(), "md_in_html"])
         self._replacement_mapping = {}
 
     def _read_article(self) -> List[str]:
-        with open(self._article_file_path, 'r', encoding='utf8') as m_file:
+        with open(self._article_file_path, "r", encoding="utf8") as m_file:
             self._md_conv.convert(m_file.read())
 
-        print(f'Images links count = {len(self._md_conv.images)}')
+        print(f"Images links count = {len(self._md_conv.images)}")
         images = set(self._md_conv.images)
-        print(f'Unique images links count = {len(images)}')
+        print(f"Unique images links count = {len(images)}")
 
         return images
 
     def _fix_document_urls(self) -> List[str]:
         # print('Replacing images urls in the document...')
         replacement_mapping = self._replacement_mapping
         lines = []
-        with open(self._article_file_path, 'r', encoding='utf8') as infile:
+        with open(self._article_file_path, "r", encoding="utf8") as infile:
             for line in infile:
                 for src, target in replacement_mapping.items():
                     line = line.replace(src, target)
                 lines.append(line)
 
         return lines
 
     def run(self):
         """
         Run article conversion.
         """
 
-        self._replacement_mapping = self._image_downloader.download_images(self._read_article())
+        self._replacement_mapping = self._image_downloader.download_images(
+            self._read_article()
+        )
         return self._fix_document_urls()
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/mdparse/www_tools.py` & `alfred-py-3.0.7/alfred/modules/cabinet/mdparse/www_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 import re
 import os
 from mimetypes import guess_extension
 from .string_tools import slugify
 
 
-def is_url(url: str, allowed_url_prefixes=('http', 'ftp')) -> bool:
+def is_url(url: str, allowed_url_prefixes=("http", "ftp")) -> bool:
     """
     Check url for prefix match.
     """
 
     for prefix in set(allowed_url_prefixes):
         if url.startswith(prefix):
             return True
@@ -28,43 +28,47 @@
     :param url: URL to download.
     :param timeout: timeout before fail.
     """
 
     try:
         response = requests.get(url, allow_redirects=True, timeout=timeout)
     except requests.exceptions.SSLError:
-        print('Incorrect SSL certificate, trying to download without verifying...')
-        response = requests.get(url, allow_redirects=True, verify=False,
-                                timeout=timeout)
+        print("Incorrect SSL certificate, trying to download without verifying...")
+        response = requests.get(
+            url, allow_redirects=True, verify=False, timeout=timeout
+        )
 
     if response.status_code != 200:
         raise OSError(str(response))
 
     return response
 
 
 def get_filename_from_url(req: requests.Response) -> Optional[str]:
     """
     Get filename from url and, if not found, try to get from content-disposition.
     """
 
-    if req.url.find('/'):
-        result = req.url.rsplit('/', 1)[1]
+    if req.url.find("/"):
+        result = req.url.rsplit("/", 1)[1]
     else:
-        cd = req.headers.get('content-disposition')
+        cd = req.headers.get("content-disposition")
 
         if cd is None:
             return None
 
-        file_name = re.findall('filename=(.+)', cd)
+        file_name = re.findall("filename=(.+)", cd)
 
         if len(file_name) == 0:
             return None
 
         result = file_name[0]
 
     f_name, f_ext = os.path.splitext(result)
 
-    result = f'{slugify(f_name)}{guess_extension(req.headers["content-type"].partition(";")[0].strip())}' if not f_ext\
-        else f'{slugify(f_name)}.{slugify(f_ext)}'
+    result = (
+        f'{slugify(f_name)}{guess_extension(req.headers["content-type"].partition(";")[0].strip())}'
+        if not f_ext
+        else f"{slugify(f_name)}.{slugify(f_ext)}"
+    )
 
     return result
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/split_txt.py` & `alfred-py-3.0.7/alfred/modules/cabinet/split_txt.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,44 +31,51 @@
 import os
 import glob
 from alfred.utils.log import logger as logging
 import numpy as np
 
 
 def split_txt_file(f, ratios, names):
-    assert os.path.exists(f), '{} not exist.'.format(f)
+    assert os.path.exists(f), "{} not exist.".format(f)
     if not ratios:
         ratios = [0.2, 0.8]
     else:
-        ratios = [float(i) for i in ratios.split(',')]
-    logging.info('split ratios: {}'.format(ratios))
+        ratios = [float(i) for i in ratios.split(",")]
+    logging.info("split ratios: {}".format(ratios))
 
     if not names:
-        names = ['part_{}'.format(i) for i in range(len(ratios))]
+        names = ["part_{}".format(i) for i in range(len(ratios))]
     else:
-        names = names.split(',')
-    names = [i+'.txt' for i in names]
-    logging.info('split save to names: {}'.format(names))
+        names = names.split(",")
+    names = [i + ".txt" for i in names]
+    logging.info("split save to names: {}".format(names))
 
     a = sum(ratios)
-    if a != 1.:
+    if a != 1.0:
         logging.info(
-            'ratios: {} does not sum to 1. you must change it first.'.format(ratios))
+            "ratios: {} does not sum to 1. you must change it first.".format(ratios)
+        )
         exit(1)
 
     # read txt file
-    with open(f, 'r') as f:
+    with open(f, "r") as f:
         lines = f.readlines()
-        lines_no_empty = [i for i in lines if i != '' and i != '\n']
-        logging.info('to split file have all {} lines. droped {} empty lines.'.format(len(lines),
-                                                                                      len(lines) - len(lines_no_empty)))
+        lines_no_empty = [i for i in lines if i != "" and i != "\n"]
+        logging.info(
+            "to split file have all {} lines. droped {} empty lines.".format(
+                len(lines), len(lines) - len(lines_no_empty)
+            )
+        )
         lines = lines_no_empty
         # split with ratios
         last_lines = 0
         for i, r in enumerate(ratios):
-            one = lines[last_lines: last_lines+int(r * len(lines))]
-            with open(names[i], 'w') as ff:
+            one = lines[last_lines : last_lines + int(r * len(lines))]
+            with open(names[i], "w") as ff:
                 ff.writelines(one)
-                logging.info('Part {} saved into: {}. portion: {}/{}={}'.format(
-                    i, names[i], len(one), len(lines), len(one)/(len(lines))))
+                logging.info(
+                    "Part {} saved into: {}. portion: {}/{}={}".format(
+                        i, names[i], len(one), len(lines), len(one) / (len(lines))
+                    )
+                )
             last_lines += len(one)
-    logging.info('split done.')
+    logging.info("split done.")
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/stack_imgs.py` & `alfred-py-3.0.7/alfred/modules/cabinet/stack_imgs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,59 +4,58 @@
 
 """
 import cv2
 import numpy as np
 from alfred.utils.log import logger as logging
 
 
-
 def check_shape_resize_if_possible(imgs):
     shapes = [i.shape for i in imgs]
-    if len(set(shapes))==1:
+    if len(set(shapes)) == 1:
         return imgs
     else:
-        logging.info('detected images shape not equal, resize to the first shape...')
+        logging.info("detected images shape not equal, resize to the first shape...")
         imgs = [cv2.resize(i, (shapes[0][1], shapes[0][0])) for i in imgs]
         return imgs
 
 
-
 def stack_imgs(imgs_list, dim2d):
     """
     send a list of images
     then using dim2d to stack it
 
     for example:
         a.png
         b.png
         c.png
         d.png
-    
+
     dim2d:
         2x2
     """
-    a = int(dim2d.split('x')[0])
-    b = int(dim2d.split('x')[1])
+    a = int(dim2d.split("x")[0])
+    b = int(dim2d.split("x")[1])
     if len(imgs_list) % a != 0 or len(imgs_list) % b:
-        logging.info('dim2d {} is not applicable for {} images.'.format(dim2d, len(imgs_list)))
+        logging.info(
+            "dim2d {} is not applicable for {} images.".format(dim2d, len(imgs_list))
+        )
         exit(0)
-    elif len(imgs_list) != a*b:
-        logging.error('len imgs not equal to: axb={}'.format(a*b))
+    elif len(imgs_list) != a * b:
+        logging.error("len imgs not equal to: axb={}".format(a * b))
         exit(0)
     else:
         imgs_list = [cv2.imread(i) for i in imgs_list]
         all_raws = []
         # 2x1 bug?
         for ri in range(a):
             one_raw = []
             for ci in range(b):
-                one_raw.append(imgs_list[ri*b + ci])
-                logging.info('stacking row: {}, with len: {}'.format(ri, len(one_raw)))
+                one_raw.append(imgs_list[ri * b + ci])
+                logging.info("stacking row: {}, with len: {}".format(ri, len(one_raw)))
             imgs = check_shape_resize_if_possible(one_raw)
             img_a = np.hstack(imgs)
             all_raws.append(img_a)
         all_raws = check_shape_resize_if_possible(all_raws)
         final_img = np.vstack(all_raws)
-        logging.info('final combined img shape: {}'.format(final_img.shape))
-        cv2.imwrite('stacked_img.jpg', final_img)
-        logging.info('done.')
-
+        logging.info("final combined img shape: {}".format(final_img.shape))
+        cv2.imwrite("stacked_img.jpg", final_img)
+        logging.info("done.")
```

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/agpl-v3.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/agpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/apache-2.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/apache-2.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-B.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill-B.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill-C.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill-C.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/cecill.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/cecill.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/gpl-v3.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/gpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/lgpl-v2.1.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/templates/lgpl-v3.tmpl` & `alfred-py-3.0.7/alfred/modules/cabinet/templates/lgpl-v3.tmpl`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/cabinet/webcam.py` & `alfred-py-3.0.7/alfred/modules/cabinet/webcam.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,37 +30,36 @@
 import cv2 as cv
 import os
 from colorama import Fore, Back, Style
 
 
 def webcam_test(vf):
     if vf is not None and os.path.isfile(vf):
-        print(Fore.CYAN + 'webcam on: ',
-              Style.RESET_ALL, vf, ' press q to quit.')
+        print(Fore.CYAN + "webcam on: ", Style.RESET_ALL, vf, " press q to quit.")
         cap = cv.VideoCapture(vf)
         while cap.isOpend():
             ret, frame = cap.read()
 
             if not ret:
                 break
 
             data = preprocess(frame)
             cmap, paf = model(data)
             cmap, paf = cmap.detach().cpu(), paf.detach().cpu()
             # , cmap_threshold=0.15, link_threshold=0.15)
             counts, objects, peaks = parse_objects(cmap, paf)
             draw_objects(frame, counts, objects, peaks)
 
-            cv.imshow('res', frame)
+            cv.imshow("res", frame)
             cv.waitKey(1)
     else:
-        print(Fore.CYAN + 'test webcam, press q to quit.', Style.RESET_ALL)
+        print(Fore.CYAN + "test webcam, press q to quit.", Style.RESET_ALL)
         cap = cv.VideoCapture(0)
         while cap.isOpened():
             ret, frame = cap.read()
 
             if not ret:
                 break
 
-            cv.imshow('Webcam', frame)
-            if cv.waitKey(1) == ord('q'):
+            cv.imshow("Webcam", frame)
+            if cv.waitKey(1) == ord("q"):
                 break
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/__init__.py` & `alfred-py-3.0.7/alfred/modules/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/data/coco2yolo.py` & `alfred-py-3.0.7/alfred/modules/data/coco2yolo.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,89 +4,90 @@
 copy and paste coco annotation
 to yolo
 
 """
 
 import os
 import sys
+
 try:
     from pycocotools.coco import COCO
     from pycocotools import mask as maskUtils
 except ImportError as e:
-    print('[WARN] coco2yolo need pycocotools installed.')
+    print("[WARN] coco2yolo need pycocotools installed.")
     # exit(-1)
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Polygon
 from alfred.utils.log import logger as logging
 import cv2
 from alfred.vis.image.det import visualize_det_cv2_part
 from alfred.vis.image.common import get_unique_color_by_id
 import shutil
 
 
 def convert(size, box):
-    dw = 1./(size[0])
-    dh = 1./(size[1])
-    x = (box[0] + box[1])/2.0 - 1
-    y = (box[2] + box[3])/2.0 - 1
+    dw = 1.0 / (size[0])
+    dh = 1.0 / (size[1])
+    x = (box[0] + box[1]) / 2.0 - 1
+    y = (box[2] + box[3]) / 2.0 - 1
     w = box[1] - box[0]
     h = box[3] - box[2]
-    x = x*dw
-    w = w*dw
-    y = y*dh
-    h = h*dh
+    x = x * dw
+    w = w * dw
+    y = y * dh
+    h = h * dh
     return (x, y, w, h)
 
 
 def coco2yolo(img_r, j_f):
     data_dir = img_r
     coco = COCO(j_f)
 
     cats = coco.loadCats(coco.getCatIds())
-    logging.info('cats: {}'.format(cats))
-    print('cls list for yolo\n')
+    logging.info("cats: {}".format(cats))
+    print("cls list for yolo\n")
     for i in range(len(cats)):
-        print(cats[i]['name'])
-    print('\n')
-    print('all {} categories.'.format(len(cats)))
+        print(cats[i]["name"])
+    print("\n")
+    print("all {} categories.".format(len(cats)))
 
     img_ids = coco.getImgIds()
 
-    target_txt_r = os.path.join(os.path.dirname(img_r), 'yolo', 'labels')
-    target_img_r = os.path.join(os.path.dirname(img_r), 'yolo', 'images')
+    target_txt_r = os.path.join(os.path.dirname(img_r), "yolo", "labels")
+    target_img_r = os.path.join(os.path.dirname(img_r), "yolo", "images")
     os.makedirs(target_txt_r, exist_ok=True)
     os.makedirs(target_img_r, exist_ok=True)
 
-    print('solving, this gonna take some while...')
+    print("solving, this gonna take some while...")
     for img_id in img_ids:
         img = coco.loadImgs(img_id)[0]
         # print('checking img: {}, id: {}'.format(img, img_id))
         # img['file_name'] may be not basename
-        img_f = os.path.join(data_dir, os.path.basename(img['file_name']))
+        img_f = os.path.join(data_dir, os.path.basename(img["file_name"]))
         if not os.path.exists(img_f):
             # if not then pull it back to normal mode
-            img_f = os.path.join(data_dir, img['file_name'])
-        anno_ids = coco.getAnnIds(imgIds=img['id'])
+            img_f = os.path.join(data_dir, img["file_name"])
+        anno_ids = coco.getAnnIds(imgIds=img["id"])
         annos = coco.loadAnns(anno_ids)
 
         img_root, img_ext = os.path.splitext(img_f)
-        out_file = open(os.path.join(target_txt_r, os.path.basename(img_root) + '.txt'), 'w')
+        out_file = open(
+            os.path.join(target_txt_r, os.path.basename(img_root) + ".txt"), "w"
+        )
         # out_file = open(os.path.join(target_txt_r, os.path.basename(img_f).split('.')[0] + '.txt'), 'w')
         img = cv2.imread(img_f)
         h, w, _ = img.shape
         shutil.copy(img_f, os.path.join(target_img_r, os.path.basename(img_f)))
         for ann in annos:
-            b = ann['bbox']
+            b = ann["bbox"]
             x1 = int(b[0])
             y1 = int(b[1])
             x2 = int(x1 + b[2])
             y2 = int(y1 + b[3])
-            cls_id = ann['category_id']
+            cls_id = ann["category_id"]
             b = [x1, x2, y1, y2]
             bb = convert((w, h), b)
-            out_file.write(str(cls_id) + " " +
-                    " ".join([str(a) for a in bb]) + '\n')
+            out_file.write(str(cls_id) + " " + " ".join([str(a) for a in bb]) + "\n")
         out_file.close()
-    print('convert to yolo done!')
-        
+    print("convert to yolo done!")
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/convert_csv2voc.py` & `alfred-py-3.0.7/alfred/modules/data/convert_csv2voc.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,61 +31,62 @@
 
 """
 import os
 import sys
 import glob
 import numpy as np
 from PIL import Image
+
 try:
     from lxml.etree import Element, SubElement, tostring, ElementTree, tostring
 except ImportError:
     pass
 
 
-
-
 def convert_one_csv_to_xml(csv_f, img_f):
     if os.path.exists(csv_f):
         csv_anno = np.loadtxt(csv_f)
         if len(csv_anno.shape) < 2 and csv_anno.shape[0] != 0:
             csv_anno = np.expand_dims(csv_anno, axis=0)
-        target_path = os.path.join(os.path.dirname(csv_f), os.path.basename(csv_f).split('.')[0]+'.xml')
-        # convert xml 
+        target_path = os.path.join(
+            os.path.dirname(csv_f), os.path.basename(csv_f).split(".")[0] + ".xml"
+        )
+        # convert xml
         if os.path.exists(img_f):
             im = Image.open(img_f)
             width = im.size[0]
             height = im.size[1]
-            node_root = Element('annotation')
-            node_folder = SubElement(node_root, 'folder')
-            node_folder.text = 'images'
-            node_filename = SubElement(node_root, 'filename')
+            node_root = Element("annotation")
+            node_folder = SubElement(node_root, "folder")
+            node_folder.text = "images"
+            node_filename = SubElement(node_root, "filename")
             node_filename.text = os.path.basename(img_f)
-            node_size = SubElement(node_root, 'size')
-            node_width = SubElement(node_size, 'width')
+            node_size = SubElement(node_root, "size")
+            node_width = SubElement(node_size, "width")
             node_width.text = str(width)
-            node_height = SubElement(node_size, 'height')
+            node_height = SubElement(node_size, "height")
             node_height.text = str(height)
-            node_depth = SubElement(node_size, 'depth')
-            node_depth.text = '3'
-            
+            node_depth = SubElement(node_size, "depth")
+            node_depth.text = "3"
+
             for item in csv_anno:
-                node_object = SubElement(node_root, 'object')
-                node_name = SubElement(node_object, 'name')
+                node_object = SubElement(node_root, "object")
+                node_name = SubElement(node_object, "name")
                 node_name.text = label_map[item[0]]
-                node_difficult = SubElement(node_object, 'difficult')
-                node_difficult.text = '0'
-                node_bndbox = SubElement(node_object, 'bndbox')
-                node_xmin = SubElement(node_bndbox, 'xmin')
-                node_xmin.text = str(int(item[1]*width))
-                node_ymin = SubElement(node_bndbox, 'ymin')
-                node_ymin.text = str(int(item[1]*height))
-                node_xmax = SubElement(node_bndbox, 'xmax')
-                node_xmax.text = str(int(item[2]*width))
-                node_ymax = SubElement(node_bndbox, 'ymax')
-                node_ymax.text = str(int(item[3]*height))
-            f = open(target_path, 'wb')
+                node_difficult = SubElement(node_object, "difficult")
+                node_difficult.text = "0"
+                node_bndbox = SubElement(node_object, "bndbox")
+                node_xmin = SubElement(node_bndbox, "xmin")
+                node_xmin.text = str(int(item[1] * width))
+                node_ymin = SubElement(node_bndbox, "ymin")
+                node_ymin.text = str(int(item[1] * height))
+                node_xmax = SubElement(node_bndbox, "xmax")
+                node_xmax.text = str(int(item[2] * width))
+                node_ymax = SubElement(node_bndbox, "ymax")
+                node_ymax.text = str(int(item[3] * height))
+            f = open(target_path, "wb")
             f.write(tostring(node_root, pretty_print=True))
             f.close()
         else:
-            print('image: {} not exist.'.format(img_f))
+            print("image: {} not exist.".format(img_f))
     else:
-        print('!! {} not exist.'.format(csv_f))
+        print("!! {} not exist.".format(csv_f))
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/convert_cvat2voc.py` & `alfred-py-3.0.7/alfred/modules/data/convert_cvat2voc.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,30 +39,36 @@
 from pascal_voc_writer import Writer
 from collections import OrderedDict
 
 
 def parse_args():
     """Parse arguments of command line"""
     parser = argparse.ArgumentParser(
-        description='Convert CVAT XML annotations to PASCAL VOC format'
+        description="Convert CVAT XML annotations to PASCAL VOC format"
     )
 
     parser.add_argument(
-        '--cvat-xml', metavar='FILE', required=True,
-        help='input file with CVAT annotation in xml format'
+        "--cvat-xml",
+        metavar="FILE",
+        required=True,
+        help="input file with CVAT annotation in xml format",
     )
 
     parser.add_argument(
-        '--image-dir', metavar='DIRECTORY', required=True,
-        help='directory which contains original images'
+        "--image-dir",
+        metavar="DIRECTORY",
+        required=True,
+        help="directory which contains original images",
     )
 
     parser.add_argument(
-        '--output-dir', metavar='DIRECTORY', required=True,
-        help='directory for output annotations in PASCAL VOC format'
+        "--output-dir",
+        metavar="DIRECTORY",
+        required=True,
+        help="directory for output annotations in PASCAL VOC format",
     )
 
     return parser.parse_args()
 
 
 def process_cvat_xml(xml_file, image_dir, output_dir):
     """
@@ -70,126 +76,139 @@
     XMls.
 
     :param xml_file: CVAT format XML
     :param image_dir: image directory of the dataset
     :param output_dir: directory of annotations with PASCAL VOC format
     :return:
     """
-    KNOWN_TAGS = {'box', 'image', 'attribute'}
+    KNOWN_TAGS = {"box", "image", "attribute"}
     os.makedirs(output_dir, exist_ok=True)
     cvat_xml = etree.parse(xml_file)
 
-    basename = os.path.splitext( os.path.basename( xml_file ) )[0]
+    basename = os.path.splitext(os.path.basename(xml_file))[0]
 
-    tracks= cvat_xml.findall( './/track' )
-    log.info('tracks: {}'.format(tracks))
+    tracks = cvat_xml.findall(".//track")
+    log.info("tracks: {}".format(tracks))
 
     if (tracks is not None) and (len(tracks) > 0):
         frames = {}
 
         for track in tracks:
             trackid = int(track.get("id"))
             label = track.get("label")
-            boxes = track.findall( './box' )
+            boxes = track.findall("./box")
             for box in boxes:
-                frameid  = int(box.get('frame'))
-                outside  = int(box.get('outside'))
-                #occluded = int(box.get('occluded'))  #currently unused
-                #keyframe = int(box.get('keyframe'))  #currently unused
-                xtl      = float(box.get('xtl'))
-                ytl      = float(box.get('ytl'))
-                xbr      = float(box.get('xbr'))
-                ybr      = float(box.get('ybr'))
-                
-                frame = frames.get( frameid, {} )
-                
+                frameid = int(box.get("frame"))
+                outside = int(box.get("outside"))
+                # occluded = int(box.get('occluded'))  #currently unused
+                # keyframe = int(box.get('keyframe'))  #currently unused
+                xtl = float(box.get("xtl"))
+                ytl = float(box.get("ytl"))
+                xbr = float(box.get("xbr"))
+                ybr = float(box.get("ybr"))
+
+                frame = frames.get(frameid, {})
+
                 if outside == 0:
-                    frame[ trackid ] = { 'xtl': xtl, 'ytl': ytl, 'xbr': xbr, 'ybr': ybr, 'label': label }
+                    frame[trackid] = {
+                        "xtl": xtl,
+                        "ytl": ytl,
+                        "xbr": xbr,
+                        "ybr": ybr,
+                        "label": label,
+                    }
 
-                frames[ frameid ] = frame
+                frames[frameid] = frame
 
-        width = int(cvat_xml.find('.//original_size/width').text)
-        height  = int(cvat_xml.find('.//original_size/height').text)
+        width = int(cvat_xml.find(".//original_size/width").text)
+        height = int(cvat_xml.find(".//original_size/height").text)
 
         # Spit out a list of each object for each frame
         for frameid in sorted(frames.keys()):
-            #print( frameid )
+            # print( frameid )
 
             image_name = "%s_%08d.jpg" % (basename, frameid)
             image_path = os.path.join(image_dir, image_name)
             if not os.path.exists(image_path):
-                log.info('{} image cannot be found. Is `{}` image directory correct?'.
-                    format(image_path, image_dir))
+                log.info(
+                    "{} image cannot be found. Is `{}` image directory correct?".format(
+                        image_path, image_dir
+                    )
+                )
             writer = Writer(image_path, width, height)
 
             frame = frames[frameid]
 
             objids = sorted(frame.keys())
 
             for objid in objids:
-
                 box = frame[objid]
 
-                label = box.get('label')
-                xmin = float(box.get('xtl'))
-                ymin = float(box.get('ytl'))
-                xmax = float(box.get('xbr'))
-                ymax = float(box.get('ybr'))
+                label = box.get("label")
+                xmin = float(box.get("xtl"))
+                ymin = float(box.get("ytl"))
+                xmax = float(box.get("xbr"))
+                ymax = float(box.get("ybr"))
 
                 writer.addObject(label, xmin, ymin, xmax, ymax)
 
-            anno_name = os.path.basename(os.path.splitext(image_name)[0] + '.xml')
+            anno_name = os.path.basename(os.path.splitext(image_name)[0] + ".xml")
             anno_dir = os.path.dirname(os.path.join(output_dir, image_name))
             os.makedirs(anno_dir, exist_ok=True)
             writer.save(os.path.join(anno_dir, anno_name))
 
     else:
-        for img_tag in cvat_xml.findall('image'):
-            image_name = img_tag.get('name')
-            width = img_tag.get('width')
-            height = img_tag.get('height')
-            depth = img_tag.get('depth', 3)
+        for img_tag in cvat_xml.findall("image"):
+            image_name = img_tag.get("name")
+            width = img_tag.get("width")
+            height = img_tag.get("height")
+            depth = img_tag.get("depth", 3)
             image_path = os.path.join(image_dir, image_name)
             if not os.path.exists(image_path):
-                log.info('{} image cannot be found. Is `{}` image directory correct?'.
-                    format(image_path, image_dir))
+                log.info(
+                    "{} image cannot be found. Is `{}` image directory correct?".format(
+                        image_path, image_dir
+                    )
+                )
             writer = Writer(image_path, width, height, depth=depth)
 
             unknown_tags = {x.tag for x in img_tag.iter()}.difference(KNOWN_TAGS)
             if unknown_tags:
-                log.info('Ignoring tags for image {}: {}'.format(image_path, unknown_tags))
+                log.info(
+                    "Ignoring tags for image {}: {}".format(image_path, unknown_tags)
+                )
 
-            for box in img_tag.findall('box'):
-                label = box.get('label')
+            for box in img_tag.findall("box"):
+                label = box.get("label")
                 # concat label with attributes
                 # todo: check if exist or not
-                all_attributes = box.findall('attribute')
+                all_attributes = box.findall("attribute")
                 attr_dict = OrderedDict()
                 for attr in all_attributes:
-                    attr_dict[attr.get('name')] = attr.text
+                    attr_dict[attr.get("name")] = attr.text
                 lst = sorted(attr_dict.items(), key=lambda item: item[0])
                 attr_dict = OrderedDict(lst)
                 # label += '_' + '_'.join(attr_dict.values())
                 # we only take color for now
-                label = label.replace('_', '')
-                label += '_' + list(attr_dict.values())[0]
+                label = label.replace("_", "")
+                label += "_" + list(attr_dict.values())[0]
                 # log.info(label)
-                xmin = float(box.get('xtl'))
-                ymin = float(box.get('ytl'))
-                xmax = float(box.get('xbr'))
-                ymax = float(box.get('ybr'))
+                xmin = float(box.get("xtl"))
+                ymin = float(box.get("ytl"))
+                xmax = float(box.get("xbr"))
+                ymax = float(box.get("ybr"))
 
                 writer.addObject(label, xmin, ymin, xmax, ymax)
 
-            anno_name = os.path.basename(os.path.splitext(image_name)[0] + '.xml')
+            anno_name = os.path.basename(os.path.splitext(image_name)[0] + ".xml")
             anno_dir = os.path.dirname(os.path.join(output_dir, image_name))
             os.makedirs(anno_dir, exist_ok=True)
             writer.save(os.path.join(anno_dir, anno_name))
 
 
 def main():
     args = parse_args()
     process_cvat_xml(args.cvat_xml, args.image_dir, args.output_dir)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/convert_labelone2voc.py` & `alfred-py-3.0.7/alfred/modules/data/convert_labelone2voc.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,72 +51,72 @@
 import os
 import json
 import glob
 import sys
 from PIL import Image
 
 try:
-  from lxml.etree import Element, SubElement, tostring, ElementTree, tostring
-  from lxml import etree
+    from lxml.etree import Element, SubElement, tostring, ElementTree, tostring
+    from lxml import etree
 except ImportError:
-  pass
+    pass
 
 
 def convert_one(a):
-    os.makedirs(os.path.dirname(a)+'_voc', exist_ok=True)
+    os.makedirs(os.path.dirname(a) + "_voc", exist_ok=True)
     d = json.load(open(a))
     print(d)
 
-    target_path = os.path.join(os.path.dirname(a)+'_voc', os.path.basename(a).split('.')[0]+'.xml')
-    img_path = os.path.join('images', d['imagePath'])
-    # convert xml 
+    target_path = os.path.join(
+        os.path.dirname(a) + "_voc", os.path.basename(a).split(".")[0] + ".xml"
+    )
+    img_path = os.path.join("images", d["imagePath"])
+    # convert xml
     if os.path.exists(img_path):
         im = Image.open(img_path)
         width = im.size[0]
         height = im.size[1]
-        node_root = Element('annotation')
-        node_folder = SubElement(node_root, 'folder')
-        node_folder.text = 'images'
-        node_filename = SubElement(node_root, 'filename')
-        node_filename.text = d['imagePath']
-        node_size = SubElement(node_root, 'size')
-        node_width = SubElement(node_size, 'width')
+        node_root = Element("annotation")
+        node_folder = SubElement(node_root, "folder")
+        node_folder.text = "images"
+        node_filename = SubElement(node_root, "filename")
+        node_filename.text = d["imagePath"]
+        node_size = SubElement(node_root, "size")
+        node_width = SubElement(node_size, "width")
         node_width.text = str(width)
-        node_height = SubElement(node_size, 'height')
+        node_height = SubElement(node_size, "height")
         node_height.text = str(height)
-        node_depth = SubElement(node_size, 'depth')
-        node_depth.text = '3'
-        
-        for item in d['shapes']:
-            node_object = SubElement(node_root, 'object')
-            node_name = SubElement(node_object, 'name')
-            node_name.text = item['label']
-            node_difficult = SubElement(node_object, 'difficult')
-            node_difficult.text = '0'
-            node_bndbox = SubElement(node_object, 'bndbox')
-            node_xmin = SubElement(node_bndbox, 'xmin')
-            node_xmin.text = str(item['points'][1][0])
-            node_ymin = SubElement(node_bndbox, 'ymin')
-            node_ymin.text = str(item['points'][1][1])
-            node_xmax = SubElement(node_bndbox, 'xmax')
-            node_xmax.text = str(item['points'][3][0])
-            node_ymax = SubElement(node_bndbox, 'ymax')
-            node_ymax.text = str(item['points'][3][1])
-        f = open(target_path, 'wb')
+        node_depth = SubElement(node_size, "depth")
+        node_depth.text = "3"
+
+        for item in d["shapes"]:
+            node_object = SubElement(node_root, "object")
+            node_name = SubElement(node_object, "name")
+            node_name.text = item["label"]
+            node_difficult = SubElement(node_object, "difficult")
+            node_difficult.text = "0"
+            node_bndbox = SubElement(node_object, "bndbox")
+            node_xmin = SubElement(node_bndbox, "xmin")
+            node_xmin.text = str(item["points"][1][0])
+            node_ymin = SubElement(node_bndbox, "ymin")
+            node_ymin.text = str(item["points"][1][1])
+            node_xmax = SubElement(node_bndbox, "xmax")
+            node_xmax.text = str(item["points"][3][0])
+            node_ymax = SubElement(node_bndbox, "ymax")
+            node_ymax.text = str(item["points"][3][1])
+        f = open(target_path, "wb")
         f.write(etree.tostring(node_root, pretty_print=True))
         f.close()
     else:
-        print('xxx {} annotations according image: {} not exist.'.format(a, img_path))
-
+        print("xxx {} annotations according image: {} not exist.".format(a, img_path))
 
 
 def run():
-    all_json_files = glob.glob(os.path.join(sys.argv[1], '*.json'))
+    all_json_files = glob.glob(os.path.join(sys.argv[1], "*.json"))
     print(len(all_json_files))
     for i in all_json_files:
         convert_one(i)
-    print('done!')
-
+    print("done!")
 
 
 if __name__ == "__main__":
-    run()
+    run()
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/eval_voc.py` & `alfred-py-3.0.7/alfred/modules/data/eval_voc.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,40 +33,38 @@
 import xml.etree.ElementTree as ET
 import numpy as np
 import cv2
 from alfred.utils.log import logger as logging
 import matplotlib.pyplot as plt
 
 
-
-
 def log_average_miss_rate(precision, fp_cumsum, num_images):
     """
-        log-average miss rate:
-            Calculated by averaging miss rates at 9 evenly spaced FPPI points
-            between 10e-2 and 10e0, in log-space.
-
-        output:
-                lamr | log-average miss rate
-                mr | miss rate
-                fppi | false positives per image
-
-        references:
-            [1] Dollar, Piotr, et al. "Pedestrian Detection: An Evaluation of the
-               State of the Art." Pattern Analysis and Machine Intelligence, IEEE
-               Transactions on 34.4 (2012): 743 - 761.
+    log-average miss rate:
+        Calculated by averaging miss rates at 9 evenly spaced FPPI points
+        between 10e-2 and 10e0, in log-space.
+
+    output:
+            lamr | log-average miss rate
+            mr | miss rate
+            fppi | false positives per image
+
+    references:
+        [1] Dollar, Piotr, et al. "Pedestrian Detection: An Evaluation of the
+           State of the Art." Pattern Analysis and Machine Intelligence, IEEE
+           Transactions on 34.4 (2012): 743 - 761.
     """
     # if there were no detections of that class
     if precision.size == 0:
         lamr = 0
         mr = 1
         fppi = 0
         return lamr, mr, fppi
     fppi = fp_cumsum / float(num_images)
-    mr = (1 - precision)
+    mr = 1 - precision
 
     fppi_tmp = np.insert(fppi, 0, -1.0)
     mr_tmp = np.insert(mr, 0, 1.0)
     # Use 9 evenly spaced reference points in log-space
     ref = np.logspace(-2.0, 0.0, num=9)
     for i, ref_i in enumerate(ref):
         # np.where() will always find at least 1 index, since min(ref) = 0.01 and min(fppi_tmp) = -1.0
@@ -125,123 +123,141 @@
         matlab: for i=numel(mpre)-1:-1:1
                     mpre(i)=max(mpre(i),mpre(i+1));
     """
     # matlab indexes start in 1 but python in 0, so I have to do:
     #     range(start=(len(mpre) - 2), end=0, step=-1)
     # also the python function range excludes the end, resulting in:
     #     range(start=(len(mpre) - 2), end=-1, step=-1)
-    for i in range(len(mpre)-2, -1, -1):
-        mpre[i] = max(mpre[i], mpre[i+1])
+    for i in range(len(mpre) - 2, -1, -1):
+        mpre[i] = max(mpre[i], mpre[i + 1])
     """
      This part creates a list of indexes where the recall changes
         matlab: i=find(mrec(2:end)~=mrec(1:end-1))+1;
     """
     i_list = []
     for i in range(1, len(mrec)):
-        if mrec[i] != mrec[i-1]:
+        if mrec[i] != mrec[i - 1]:
             i_list.append(i)  # if it was matlab would be i + 1
     """
      The Average Precision (AP) is the area under the curve
         (numerical integration)
         matlab: ap=sum((mrec(i)-mrec(i-1)).*mpre(i));
     """
     ap = 0.0
     for i in i_list:
-        ap += ((mrec[i]-mrec[i-1])*mpre[i])
+        ap += (mrec[i] - mrec[i - 1]) * mpre[i]
     return ap, mrec, mpre
 
 
 def draw_text_in_image(img, text, pos, color, line_width):
     font = cv2.FONT_HERSHEY_PLAIN
     fontScale = 1
     lineType = 1
     bottomLeftCornerOfText = pos
-    cv2.putText(img, text,
-                bottomLeftCornerOfText,
-                font,
-                fontScale,
-                color,
-                lineType)
+    cv2.putText(img, text, bottomLeftCornerOfText, font, fontScale, color, lineType)
     text_width, _ = cv2.getTextSize(text, font, fontScale, lineType)[0]
     return img, (line_width + text_width)
 
 
 def adjust_axes(r, t, fig, axes):
     # get text width for re-scaling
     bb = t.get_window_extent(renderer=r)
     text_width_inches = bb.width / fig.dpi
     # get axis width in inches
     current_fig_width = fig.get_figwidth()
     new_fig_width = current_fig_width + text_width_inches
     propotion = new_fig_width / current_fig_width
     # get axis limit
     x_lim = axes.get_xlim()
-    axes.set_xlim([x_lim[0], x_lim[1]*propotion])
+    axes.set_xlim([x_lim[0], x_lim[1] * propotion])
 
 
-def draw_plot_func(dictionary, n_classes, window_title, plot_title, x_label, output_path, to_show, plot_color, true_p_bar):
+def draw_plot_func(
+    dictionary,
+    n_classes,
+    window_title,
+    plot_title,
+    x_label,
+    output_path,
+    to_show,
+    plot_color,
+    true_p_bar,
+):
     # sort the dictionary by decreasing value, into a list of tuples
-    sorted_dic_by_value = sorted(
-        dictionary.items(), key=operator.itemgetter(1))
+    sorted_dic_by_value = sorted(dictionary.items(), key=operator.itemgetter(1))
     # unpacking the list of tuples into two lists
     sorted_keys, sorted_values = zip(*sorted_dic_by_value)
     #
     if true_p_bar != "":
         """
-         Special case to draw in:
-            - green -> TP: True Positives (object detected and matches ground-truth)
-            - red -> FP: False Positives (object detected but does not match ground-truth)
-            - orange -> FN: False Negatives (object not detected but present in the ground-truth)
+        Special case to draw in:
+           - green -> TP: True Positives (object detected and matches ground-truth)
+           - red -> FP: False Positives (object detected but does not match ground-truth)
+           - orange -> FN: False Negatives (object not detected but present in the ground-truth)
         """
         fp_sorted = []
         tp_sorted = []
         for key in sorted_keys:
             fp_sorted.append(dictionary[key] - true_p_bar[key])
             tp_sorted.append(true_p_bar[key])
-        plt.barh(range(n_classes), fp_sorted, align='center',
-                 color='crimson', label='False Positive')
-        plt.barh(range(n_classes), tp_sorted, align='center',
-                 color='forestgreen', label='True Positive', left=fp_sorted)
+        plt.barh(
+            range(n_classes),
+            fp_sorted,
+            align="center",
+            color="crimson",
+            label="False Positive",
+        )
+        plt.barh(
+            range(n_classes),
+            tp_sorted,
+            align="center",
+            color="forestgreen",
+            label="True Positive",
+            left=fp_sorted,
+        )
         # add legend
-        plt.legend(loc='lower right')
+        plt.legend(loc="lower right")
         """
          Write number on side of bar
         """
         fig = plt.gcf()  # gcf - get current figure
         axes = plt.gca()
         r = fig.canvas.get_renderer()
         for i, val in enumerate(sorted_values):
             fp_val = fp_sorted[i]
             tp_val = tp_sorted[i]
             fp_str_val = " " + str(fp_val)
             tp_str_val = fp_str_val + " " + str(tp_val)
             # trick to paint multicolor with offset:
             # first paint everything and then repaint the first number
-            t = plt.text(val, i, tp_str_val, color='forestgreen',
-                         va='center', fontweight='bold')
-            plt.text(val, i, fp_str_val, color='crimson',
-                     va='center', fontweight='bold')
-            if i == (len(sorted_values)-1):  # largest bar
+            t = plt.text(
+                val, i, tp_str_val, color="forestgreen", va="center", fontweight="bold"
+            )
+            plt.text(
+                val, i, fp_str_val, color="crimson", va="center", fontweight="bold"
+            )
+            if i == (len(sorted_values) - 1):  # largest bar
                 adjust_axes(r, t, fig, axes)
     else:
         plt.barh(range(n_classes), sorted_values, color=plot_color)
         """
          Write number on side of bar
         """
         fig = plt.gcf()  # gcf - get current figure
         axes = plt.gca()
         r = fig.canvas.get_renderer()
         for i, val in enumerate(sorted_values):
             str_val = " " + str(val)  # add a space before
             if val < 1.0:
                 str_val = " {0:.2f}".format(val)
-            t = plt.text(val, i, str_val, color=plot_color,
-                         va='center', fontweight='bold')
+            t = plt.text(
+                val, i, str_val, color=plot_color, va="center", fontweight="bold"
+            )
             # re-set axes to show number inside the figure
-            if i == (len(sorted_values)-1):  # largest bar
+            if i == (len(sorted_values) - 1):  # largest bar
                 adjust_axes(r, t, fig, axes)
     # set window title
     fig.canvas.set_window_title(window_title)
     # write classes in y axis
     tick_font_size = 12
     plt.yticks(range(n_classes), sorted_keys, fontsize=tick_font_size)
     """
@@ -260,48 +276,48 @@
     if figure_height > init_height:
         fig.set_figheight(figure_height)
 
     # set plot title
     plt.title(plot_title, fontsize=14)
     # set axis titles
     # plt.xlabel('classes')
-    plt.xlabel(x_label, fontsize='large')
+    plt.xlabel(x_label, fontsize="large")
     # adjust size of window
     fig.tight_layout()
     # save the plot
     fig.savefig(output_path)
     # show image
     if to_show:
         plt.show()
     # close the plot
     plt.close()
 
 
 def load_txt_or_xml_format(t_f):
-    if t_f.endswith('txt'):
+    if t_f.endswith("txt"):
         # open txt file lines to a list
         with open(t_f) as f:
             content = f.readlines()
         # remove whitespace characters like `\n` at the end of each line
         content = [x.strip() for x in content]
         return content
-    elif t_f.endswith('xml'):
+    elif t_f.endswith("xml"):
         root = ET.parse(t_f).getroot()
         all_gts = []
-        for obj in root.findall('object'):
-            obj_name = obj.find('name').text
-            bndbox = obj.find('bndbox')
-            left = bndbox.find('xmin').text
-            top = bndbox.find('ymin').text
-            right = bndbox.find('xmax').text
-            bottom = bndbox.find('ymax').text
-            all_gts.append(' '.join([obj_name, left, top, right, bottom]))
+        for obj in root.findall("object"):
+            obj_name = obj.find("name").text
+            bndbox = obj.find("bndbox")
+            left = bndbox.find("xmin").text
+            top = bndbox.find("ymin").text
+            right = bndbox.find("xmax").text
+            bottom = bndbox.find("ymax").text
+            all_gts.append(" ".join([obj_name, left, top, right, bottom]))
         return all_gts
     else:
-        logging.error('unsupported gt file format.')
+        logging.error("unsupported gt file format.")
         exit(0)
 
 
 def eval_voc(args):
     if args.ignore is None:
         args.ignore = []
 
@@ -310,91 +326,95 @@
         specific_iou_flagged = True
 
     GT_PATH = args.gt_dir
     DR_PATH = args.det_dir
     IMG_PATH = args.images_dir
     MINOVERLAP = args.min_overlap
 
-    logging.info('Ground truth dir: {}'.format(GT_PATH))
-    logging.info('Detection result dir: {}'.format(DR_PATH))
-    logging.info('Images dir: {}'.format(IMG_PATH))
-    logging.info('Min overlap: {}'.format(MINOVERLAP))
+    logging.info("Ground truth dir: {}".format(GT_PATH))
+    logging.info("Detection result dir: {}".format(DR_PATH))
+    logging.info("Images dir: {}".format(IMG_PATH))
+    logging.info("Min overlap: {}".format(MINOVERLAP))
 
     if os.path.exists(IMG_PATH):
         for dirpath, dirnames, files in os.walk(IMG_PATH):
             if not files:
                 # no image files found
                 args.no_animation = True
     else:
         args.no_animation = True
     show_animation = False
     if not args.no_animation:
         try:
             import cv2
+
             show_animation = True
         except ImportError:
-            print("\"opencv-python\" not found, please install to visualize the results.")
+            print('"opencv-python" not found, please install to visualize the results.')
             args.no_animation = True
     draw_plot = False
     if not args.no_plot:
         try:
             import matplotlib.pyplot as plt
+
             draw_plot = True
         except ImportError:
             print(
-                "\"matplotlib\" not found, please install it to get the resulting plots.")
+                '"matplotlib" not found, please install it to get the resulting plots.'
+            )
             args.no_plot = True
 
     TEMP_FILES_PATH = os.path.join(os.path.dirname(GT_PATH), "temp_files")
-    logging.info('creating a temp path: {}'.format(os.path.abspath(TEMP_FILES_PATH)))
+    logging.info("creating a temp path: {}".format(os.path.abspath(TEMP_FILES_PATH)))
     if not os.path.exists(TEMP_FILES_PATH):  # if it doesn't exist already
         os.makedirs(TEMP_FILES_PATH)
     results_files_path = "./results_{}".format(MINOVERLAP)
     if os.path.exists(results_files_path):  # if it exist already
         # reset the results directory
         shutil.rmtree(results_files_path)
 
     os.makedirs(results_files_path)
     if draw_plot:
         os.makedirs(os.path.join(results_files_path, "classes"))
     if show_animation:
-        os.makedirs(os.path.join(results_files_path,
-                                 "images", "detections_one_by_one"))
+        os.makedirs(os.path.join(results_files_path, "images", "detections_one_by_one"))
 
     # get a list with the ground-truth files
     # Make can solve both txt ground truth and xml ground truth
     if os.path.isfile(GT_PATH):
-        logging.info('{} is a file, eval on coco not support now.'.format(GT_PATH))
+        logging.info("{} is a file, eval on coco not support now.".format(GT_PATH))
         exit(0)
     else:
         all_files_gt = os.listdir(GT_PATH)
         ground_truth_files_list = []
-        gt_format = 'txt'
-        if all_files_gt[0].endswith('txt'):
-            logging.info('detected your ground truth were txt format, start eval....')
-            ground_truth_files_list = glob.glob(os.path.join(GT_PATH, '*.txt'))
-        elif all_files_gt[0].endswith('xml'):
-            logging.info('detected your ground truth were xml format, start eval....')
-            ground_truth_files_list = glob.glob(os.path.join(GT_PATH, '*.xml'))
-            gt_format = 'xml'
+        gt_format = "txt"
+        if all_files_gt[0].endswith("txt"):
+            logging.info("detected your ground truth were txt format, start eval....")
+            ground_truth_files_list = glob.glob(os.path.join(GT_PATH, "*.txt"))
+        elif all_files_gt[0].endswith("xml"):
+            logging.info("detected your ground truth were xml format, start eval....")
+            ground_truth_files_list = glob.glob(os.path.join(GT_PATH, "*.xml"))
+            gt_format = "xml"
         else:
-            logging.error('unsupported ground truth format, pls using xml or txt as ground truth format.')
+            logging.error(
+                "unsupported ground truth format, pls using xml or txt as ground truth format."
+            )
             exit(0)
 
     if len(ground_truth_files_list) == 0:
         logging.error("Error: No ground-truth files found!")
         exit(0)
     ground_truth_files_list.sort()
     # dictionary with counter per class
     gt_counter_per_class = {}
     counter_images_per_class = {}
 
     # todo: Ground truth can be txt or xml both can be converted
     for gt_file in ground_truth_files_list:
-        file_id = os.path.basename(gt_file).split('.')[0]
+        file_id = os.path.basename(gt_file).split(".")[0]
         # check if there is a correspondent detection-results file
         temp_path = os.path.join(DR_PATH, (file_id + ".txt"))
         if not os.path.exists(temp_path):
             error_msg = "Error. File not found: {}\n".format(temp_path)
             error_msg += "(You can avoid this error message by running extra/intersect-gt-and-dr.py)"
             logging.error(error_msg)
         lines_list = load_txt_or_xml_format(gt_file)
@@ -410,27 +430,34 @@
                 else:
                     class_name, left, top, right, bottom = line.split()
             except ValueError:
                 error_msg = "Error: File " + gt_file + " in the wrong format.\n"
                 error_msg += " Expected: <class_name> <left> <top> <right> <bottom> ['difficult']\n"
                 error_msg += " Received: " + line
                 error_msg += "\n\nIf you have a <class_name> with spaces between words you should remove them\n"
-                error_msg += "by running the script \"remove_space.py\" or \"rename_class.py\" in the \"extra/\" folder."
+                error_msg += 'by running the script "remove_space.py" or "rename_class.py" in the "extra/" folder.'
                 logging.error(error_msg)
             # check if class is in the ignore list, if yes skip
             if class_name in args.ignore:
                 continue
             bbox = left + " " + top + " " + right + " " + bottom
             if is_difficult:
                 bounding_boxes.append(
-                    {"class_name": class_name, "bbox": bbox, "used": False, "difficult": True})
+                    {
+                        "class_name": class_name,
+                        "bbox": bbox,
+                        "used": False,
+                        "difficult": True,
+                    }
+                )
                 is_difficult = False
             else:
                 bounding_boxes.append(
-                    {"class_name": class_name, "bbox": bbox, "used": False})
+                    {"class_name": class_name, "bbox": bbox, "used": False}
+                )
                 # count that object
                 if class_name in gt_counter_per_class:
                     gt_counter_per_class[class_name] += 1
                 else:
                     # if class didn't exist yet
                     gt_counter_per_class[class_name] = 1
 
@@ -438,66 +465,78 @@
                     if class_name in counter_images_per_class:
                         counter_images_per_class[class_name] += 1
                     else:
                         # if class didn't exist yet
                         counter_images_per_class[class_name] = 1
                     already_seen_classes.append(class_name)
         # dump bounding_boxes into a ".json" file
-        with open(TEMP_FILES_PATH + "/" + file_id + "_ground_truth.json", 'w') as outfile:
+        with open(
+            TEMP_FILES_PATH + "/" + file_id + "_ground_truth.json", "w"
+        ) as outfile:
             json.dump(bounding_boxes, outfile)
 
     gt_classes = list(gt_counter_per_class.keys())
-    logging.info('gt_classes gathered: {}'.format(gt_classes))
+    logging.info("gt_classes gathered: {}".format(gt_classes))
     # let's sort the classes alphabetically
     gt_classes = sorted(gt_classes)
     n_classes = len(gt_classes)
     # print(gt_classes)
     # print(gt_counter_per_class)
 
     if specific_iou_flagged:
         n_args = len(args.set_class_iou)
-        error_msg = \
-            '\n --set-class-iou [class_1] [IoU_1] [class_2] [IoU_2] [...]'
+        error_msg = "\n --set-class-iou [class_1] [IoU_1] [class_2] [IoU_2] [...]"
         if n_args % 2 != 0:
-            logging.error('Error, missing arguments. Flag usage:' + error_msg)
+            logging.error("Error, missing arguments. Flag usage:" + error_msg)
         # [class_1] [IoU_1] [class_2] [IoU_2]
         # specific_iou_classes = ['class_1', 'class_2']
         specific_iou_classes = args.set_class_iou[::2]  # even
         # iou_list = ['IoU_1', 'IoU_2']
         iou_list = args.set_class_iou[1::2]  # odd
         if len(specific_iou_classes) != len(iou_list):
-            logging.error('Error, missing arguments. Flag usage:' + error_msg)
+            logging.error("Error, missing arguments. Flag usage:" + error_msg)
         for tmp_class in specific_iou_classes:
             if tmp_class not in gt_classes:
-                logging.error('Error, unknown class \"' + tmp_class +
-                      '\". Flag usage:' + error_msg)
+                logging.error(
+                    'Error, unknown class "' + tmp_class + '". Flag usage:' + error_msg
+                )
         for num in iou_list:
             if not is_float_between_0_and_1(num):
-                logging.error('Error, IoU must be between 0.0 and 1.0. Flag usage:' + error_msg)
+                logging.error(
+                    "Error, IoU must be between 0.0 and 1.0. Flag usage:" + error_msg
+                )
 
     # get a list with the detection-results files
-    dr_files_list = glob.glob(os.path.join(DR_PATH, '*.txt'))
-    logging.info('detection files detected: {}, vs ground truth: {}'.format(len(dr_files_list), len(ground_truth_files_list)))
+    dr_files_list = glob.glob(os.path.join(DR_PATH, "*.txt"))
+    logging.info(
+        "detection files detected: {}, vs ground truth: {}".format(
+            len(dr_files_list), len(ground_truth_files_list)
+        )
+    )
     dr_files_list.sort()
 
     for class_index, class_name in enumerate(gt_classes):
         bounding_boxes = []
         for txt_file in dr_files_list:
             # print(txt_file)
             # the first time it checks if all the corresponding ground-truth files exist
             file_id = os.path.basename(txt_file).split(".")[0]
-            temp_path = ''
-            if gt_format == 'txt':
+            temp_path = ""
+            if gt_format == "txt":
                 temp_path = os.path.join(GT_PATH, (file_id + ".txt"))
-            elif gt_format == 'xml':
+            elif gt_format == "xml":
                 temp_path = os.path.join(GT_PATH, (file_id + ".xml"))
 
             if class_index == 0:
                 if not os.path.exists(temp_path):
-                    error_msg = "Error. according ground truth File not found: {}\n".format(temp_path)
+                    error_msg = (
+                        "Error. according ground truth File not found: {}\n".format(
+                            temp_path
+                        )
+                    )
                     error_msg += "(You can avoid this error message by running extra/intersect-gt-and-dr.py)"
                     logging.error(error_msg)
             lines = load_txt_or_xml_format(txt_file)
             for line in lines:
                 try:
                     tmp_class_name, confidence, left, top, right, bottom = line.split()
                 except ValueError:
@@ -505,26 +544,27 @@
                     error_msg += " Expected: <class_name> <confidence> <left> <top> <right> <bottom>\n"
                     error_msg += " Received: " + line
                     logging.error(error_msg)
                 if tmp_class_name == class_name:
                     # print("match")
                     bbox = left + " " + top + " " + right + " " + bottom
                     bounding_boxes.append(
-                        {"confidence": confidence, "file_id": file_id, "bbox": bbox})
+                        {"confidence": confidence, "file_id": file_id, "bbox": bbox}
+                    )
                     # print(bounding_boxes)
         # sort detection-results by decreasing confidence
-        bounding_boxes.sort(key=lambda x: float(x['confidence']), reverse=True)
-        with open(TEMP_FILES_PATH + "/" + class_name + "_dr.json", 'w') as outfile:
+        bounding_boxes.sort(key=lambda x: float(x["confidence"]), reverse=True)
+        with open(TEMP_FILES_PATH + "/" + class_name + "_dr.json", "w") as outfile:
             json.dump(bounding_boxes, outfile)
-    logging.info('ground truth and det files solved, start calculating mAP...')
+    logging.info("ground truth and det files solved, start calculating mAP...")
     sum_AP = 0.0
     ap_dictionary = {}
     lamr_dictionary = {}
     # open file to store the results
-    with open(results_files_path + "/results.txt", 'w') as results_file:
+    with open(results_files_path + "/results.txt", "w") as results_file:
         results_file.write("# AP and precision/recall per class\n")
         count_true_positives = {}
         for class_index, class_name in enumerate(gt_classes):
             count_true_positives[class_name] = 0
             """
             Load detection-results of that class
             """
@@ -538,55 +578,70 @@
             tp = [0] * nd  # creates an array of zeros of size nd
             fp = [0] * nd
             for idx, detection in enumerate(dr_data):
                 file_id = detection["file_id"]
                 if show_animation:
                     # find ground truth image
                     ground_truth_img = glob.glob1(IMG_PATH, file_id + ".*")
-                    #tifCounter = len(glob.glob1(myPath,"*.tif"))
+                    # tifCounter = len(glob.glob1(myPath,"*.tif"))
                     if len(ground_truth_img) == 0:
                         logging.error("Error. Image not found with id: " + file_id)
                     elif len(ground_truth_img) > 1:
                         logging.error("Error. Multiple image with id: " + file_id)
                     else:  # found image
-                        #print(IMG_PATH + "/" + ground_truth_img[0])
+                        # print(IMG_PATH + "/" + ground_truth_img[0])
                         # Load image
                         img = cv2.imread(IMG_PATH + "/" + ground_truth_img[0])
                         # load image with draws of multiple detections
-                        img_cumulative_path = results_files_path + \
-                            "/images/" + ground_truth_img[0]
+                        img_cumulative_path = (
+                            results_files_path + "/images/" + ground_truth_img[0]
+                        )
                         if os.path.isfile(img_cumulative_path):
                             img_cumulative = cv2.imread(img_cumulative_path)
                         else:
                             img_cumulative = img.copy()
                         # Add bottom border to image
                         bottom_border = 60
                         BLACK = [0, 0, 0]
                         img = cv2.copyMakeBorder(
-                            img, 0, bottom_border, 0, 0, cv2.BORDER_CONSTANT, value=BLACK)
+                            img,
+                            0,
+                            bottom_border,
+                            0,
+                            0,
+                            cv2.BORDER_CONSTANT,
+                            value=BLACK,
+                        )
                 # assign detection-results to ground truth object if any
                 # open ground-truth with that file_id
                 gt_file = TEMP_FILES_PATH + "/" + file_id + "_ground_truth.json"
                 ground_truth_data = json.load(open(gt_file))
                 ovmax = -1
                 gt_match = -1
                 # load detected object bounding-box
                 bb = [float(x) for x in detection["bbox"].split()]
                 for obj in ground_truth_data:
                     # look for a class_name match
                     if obj["class_name"] == class_name:
                         bbgt = [float(x) for x in obj["bbox"].split()]
-                        bi = [max(bb[0], bbgt[0]), max(bb[1], bbgt[1]),
-                              min(bb[2], bbgt[2]), min(bb[3], bbgt[3])]
+                        bi = [
+                            max(bb[0], bbgt[0]),
+                            max(bb[1], bbgt[1]),
+                            min(bb[2], bbgt[2]),
+                            min(bb[3], bbgt[3]),
+                        ]
                         iw = bi[2] - bi[0] + 1
                         ih = bi[3] - bi[1] + 1
                         if iw > 0 and ih > 0:
                             # compute overlap (IoU) = area of intersection / area of union
-                            ua = (bb[2] - bb[0] + 1) * (bb[3] - bb[1] + 1) + (bbgt[2] - bbgt[0]
-                                                                              + 1) * (bbgt[3] - bbgt[1] + 1) - iw * ih
+                            ua = (
+                                (bb[2] - bb[0] + 1) * (bb[3] - bb[1] + 1)
+                                + (bbgt[2] - bbgt[0] + 1) * (bbgt[3] - bbgt[1] + 1)
+                                - iw * ih
+                            )
                             ov = iw * ih / ua
                             if ov > ovmax:
                                 ovmax = ov
                                 gt_match = obj
 
                 # assign detection as true positive/don't care/false positive
                 if show_animation:
@@ -601,15 +656,15 @@
                     if "difficult" not in gt_match:
                         if not bool(gt_match["used"]):
                             # true positive
                             tp[idx] = 1
                             gt_match["used"] = True
                             count_true_positives[class_name] += 1
                             # update the ".json" file
-                            with open(gt_file, 'w') as f:
+                            with open(gt_file, "w") as f:
                                 f.write(json.dumps(ground_truth_data))
                             if show_animation:
                                 status = "MATCH!"
                         else:
                             # false positive (multiple detection)
                             fp[idx] = 1
                             if show_animation:
@@ -631,68 +686,115 @@
                     green = (0, 255, 0)
                     light_red = (30, 30, 255)
                     # 1st line
                     margin = 10
                     v_pos = int(height - margin - (bottom_border / 2.0))
                     text = "Image: " + ground_truth_img[0] + " "
                     img, line_width = draw_text_in_image(
-                        img, text, (margin, v_pos), white, 0)
-                    text = "Class [" + str(class_index) + "/" + \
-                        str(n_classes) + "]: " + class_name + " "
+                        img, text, (margin, v_pos), white, 0
+                    )
+                    text = (
+                        "Class ["
+                        + str(class_index)
+                        + "/"
+                        + str(n_classes)
+                        + "]: "
+                        + class_name
+                        + " "
+                    )
                     img, line_width = draw_text_in_image(
-                        img, text, (margin + line_width, v_pos), light_blue, line_width)
+                        img, text, (margin + line_width, v_pos), light_blue, line_width
+                    )
                     if ovmax != -1:
                         color = light_red
                         if status == "INSUFFICIENT OVERLAP":
                             text = "IoU: {0:.2f}% ".format(
-                                ovmax*100) + "< {0:.2f}% ".format(min_overlap*100)
+                                ovmax * 100
+                            ) + "< {0:.2f}% ".format(min_overlap * 100)
                         else:
                             text = "IoU: {0:.2f}% ".format(
-                                ovmax*100) + ">= {0:.2f}% ".format(min_overlap*100)
+                                ovmax * 100
+                            ) + ">= {0:.2f}% ".format(min_overlap * 100)
                             color = green
                         img, _ = draw_text_in_image(
-                            img, text, (margin + line_width, v_pos), color, line_width)
+                            img, text, (margin + line_width, v_pos), color, line_width
+                        )
                     # 2nd line
                     v_pos += int(bottom_border / 2.0)
-                    rank_pos = str(idx+1)  # rank position (idx starts at 0)
-                    text = "Detection #rank: " + rank_pos + \
-                        " confidence: {0:.2f}% ".format(
-                            float(detection["confidence"])*100)
+                    rank_pos = str(idx + 1)  # rank position (idx starts at 0)
+                    text = (
+                        "Detection #rank: "
+                        + rank_pos
+                        + " confidence: {0:.2f}% ".format(
+                            float(detection["confidence"]) * 100
+                        )
+                    )
                     img, line_width = draw_text_in_image(
-                        img, text, (margin, v_pos), white, 0)
+                        img, text, (margin, v_pos), white, 0
+                    )
                     color = light_red
                     if status == "MATCH!":
                         color = green
                     text = "Result: " + status + " "
                     img, line_width = draw_text_in_image(
-                        img, text, (margin + line_width, v_pos), color, line_width)
+                        img, text, (margin + line_width, v_pos), color, line_width
+                    )
 
                     font = cv2.FONT_HERSHEY_SIMPLEX
-                    if ovmax > 0:  # if there is intersections between the bounding-boxes
-                        bbgt = [int(round(float(x)))
-                                for x in gt_match["bbox"].split()]
-                        cv2.rectangle(img, (bbgt[0], bbgt[1]),
-                                      (bbgt[2], bbgt[3]), light_blue, 2)
+                    if (
+                        ovmax > 0
+                    ):  # if there is intersections between the bounding-boxes
+                        bbgt = [int(round(float(x))) for x in gt_match["bbox"].split()]
+                        cv2.rectangle(
+                            img, (bbgt[0], bbgt[1]), (bbgt[2], bbgt[3]), light_blue, 2
+                        )
                         cv2.rectangle(
-                            img_cumulative, (bbgt[0], bbgt[1]), (bbgt[2], bbgt[3]), light_blue, 2)
-                        cv2.putText(img_cumulative, class_name,
-                                    (bbgt[0], bbgt[1] - 5), font, 0.6, light_blue, 1, cv2.LINE_AA)
+                            img_cumulative,
+                            (bbgt[0], bbgt[1]),
+                            (bbgt[2], bbgt[3]),
+                            light_blue,
+                            2,
+                        )
+                        cv2.putText(
+                            img_cumulative,
+                            class_name,
+                            (bbgt[0], bbgt[1] - 5),
+                            font,
+                            0.6,
+                            light_blue,
+                            1,
+                            cv2.LINE_AA,
+                        )
                     bb = [int(i) for i in bb]
-                    cv2.rectangle(img, (bb[0], bb[1]),
-                                  (bb[2], bb[3]), color, 2)
-                    cv2.rectangle(img_cumulative,
-                                  (bb[0], bb[1]), (bb[2], bb[3]), color, 2)
-                    cv2.putText(img_cumulative, class_name,
-                                (bb[0], bb[1] - 5), font, 0.6, color, 1, cv2.LINE_AA)
+                    cv2.rectangle(img, (bb[0], bb[1]), (bb[2], bb[3]), color, 2)
+                    cv2.rectangle(
+                        img_cumulative, (bb[0], bb[1]), (bb[2], bb[3]), color, 2
+                    )
+                    cv2.putText(
+                        img_cumulative,
+                        class_name,
+                        (bb[0], bb[1] - 5),
+                        font,
+                        0.6,
+                        color,
+                        1,
+                        cv2.LINE_AA,
+                    )
                     # show image
                     cv2.imshow("Animation", img)
                     cv2.waitKey(20)  # show for 20 ms
                     # save image to results
-                    output_img_path = results_files_path + "/images/detections_one_by_one/" + \
-                        class_name + "_detection" + str(idx) + ".jpg"
+                    output_img_path = (
+                        results_files_path
+                        + "/images/detections_one_by_one/"
+                        + class_name
+                        + "_detection"
+                        + str(idx)
+                        + ".jpg"
+                    )
                     cv2.imwrite(output_img_path, img)
                     # save the image with all the objects drawn to it
                     cv2.imwrite(img_cumulative_path, img_cumulative)
 
             # print(tp)
             # compute precision/recall
             cumsum = 0
@@ -712,70 +814,77 @@
             for idx, val in enumerate(tp):
                 prec[idx] = float(tp[idx]) / (fp[idx] + tp[idx])
             # print(prec)
 
             ap, mrec, mprec = voc_ap(rec[:], prec[:])
             sum_AP += ap
             # class_name + " AP = {0:.2f}%".format(ap*100)
-            text = "{0:.2f}%".format(ap*100) + " = " + class_name + " AP "
+            text = "{0:.2f}%".format(ap * 100) + " = " + class_name + " AP "
             """
             Write to results.txt
             """
-            rounded_prec = ['%.2f' % elem for elem in prec]
-            rounded_rec = ['%.2f' % elem for elem in rec]
-            results_file.write(text + "\n Precision: " + str(rounded_prec) +
-                               "\n Recall :" + str(rounded_rec) + "\n\n")
+            rounded_prec = ["%.2f" % elem for elem in prec]
+            rounded_rec = ["%.2f" % elem for elem in rec]
+            results_file.write(
+                text
+                + "\n Precision: "
+                + str(rounded_prec)
+                + "\n Recall :"
+                + str(rounded_rec)
+                + "\n\n"
+            )
             if not args.quiet:
                 print(text)
             ap_dictionary[class_name] = ap
 
             n_images = counter_images_per_class[class_name]
             lamr, mr, fppi = log_average_miss_rate(
-                np.array(rec), np.array(fp), n_images)
+                np.array(rec), np.array(fp), n_images
+            )
             lamr_dictionary[class_name] = lamr
 
             """
             Draw plot
             """
             if draw_plot:
-                plt.plot(rec, prec, '-o')
+                plt.plot(rec, prec, "-o")
                 # add a new penultimate point to the list (mrec[-2], 0.0)
                 # since the last line segment (and respective area) do not affect the AP value
                 area_under_curve_x = mrec[:-1] + [mrec[-2]] + [mrec[-1]]
                 area_under_curve_y = mprec[:-1] + [0.0] + [mprec[-1]]
-                plt.fill_between(area_under_curve_x, 0,
-                                 area_under_curve_y, alpha=0.2, edgecolor='r')
+                plt.fill_between(
+                    area_under_curve_x, 0, area_under_curve_y, alpha=0.2, edgecolor="r"
+                )
                 # set window title
                 fig = plt.gcf()  # gcf - get current figure
-                fig.canvas.set_window_title('AP ' + class_name)
+                fig.canvas.set_window_title("AP " + class_name)
                 # set plot title
-                plt.title('class: ' + text)
-                #plt.suptitle('This is a somewhat long figure title', fontsize=16)
+                plt.title("class: " + text)
+                # plt.suptitle('This is a somewhat long figure title', fontsize=16)
                 # set axis titles
-                plt.xlabel('Recall')
-                plt.ylabel('Precision')
+                plt.xlabel("Recall")
+                plt.ylabel("Precision")
                 # optional - set axes
                 axes = plt.gca()  # gca - get current axes
                 axes.set_xlim([0.0, 1.0])
                 axes.set_ylim([0.0, 1.05])  # .05 to give some extra space
                 # Alternative option -> wait for button to be pressed
                 # while not plt.waitforbuttonpress(): pass # wait for key display
                 # Alternative option -> normal display
                 # plt.show()
                 # save the plot
-                fig.savefig(results_files_path +
-                            "/classes/" + class_name + ".png")
+                fig.savefig(results_files_path + "/classes/" + class_name + ".png")
                 plt.cla()  # clear axes for next plot
 
         if show_animation:
             cv2.destroyAllWindows()
 
         results_file.write("\n# mAP of all classes\n")
         mAP = sum_AP / n_classes
-        text = "mAP = {0:.2f}%".format(mAP*100)
+        text = "mAP = {0:.2f}%".format(mAP * 100)
         results_file.write(text + "\n")
         print(text)
 
     # remove the temp_files directory
     shutil.rmtree(TEMP_FILES_PATH)
 
     det_counter_per_class = {}
@@ -795,114 +904,117 @@
                 det_counter_per_class[class_name] = 1
     # print(det_counter_per_class)
     dr_classes = list(det_counter_per_class.keys())
 
     if draw_plot:
         window_title = "ground-truth-info"
         plot_title = "ground-truth\n"
-        plot_title += "(" + str(len(ground_truth_files_list)) + \
-            " files and " + str(n_classes) + " classes)"
+        plot_title += (
+            "("
+            + str(len(ground_truth_files_list))
+            + " files and "
+            + str(n_classes)
+            + " classes)"
+        )
         x_label = "Number of objects per class"
         output_path = results_files_path + "/ground-truth-info.png"
         to_show = False
-        plot_color = 'forestgreen'
+        plot_color = "forestgreen"
         draw_plot_func(
             gt_counter_per_class,
             n_classes,
             window_title,
             plot_title,
             x_label,
             output_path,
             to_show,
             plot_color,
-            '',
+            "",
         )
 
-    with open(results_files_path + "/results.txt", 'a') as results_file:
+    with open(results_files_path + "/results.txt", "a") as results_file:
         results_file.write("\n# Number of ground-truth objects per class\n")
         for class_name in sorted(gt_counter_per_class):
-            results_file.write(class_name + ": " +
-                               str(gt_counter_per_class[class_name]) + "\n")
+            results_file.write(
+                class_name + ": " + str(gt_counter_per_class[class_name]) + "\n"
+            )
 
     for class_name in dr_classes:
         # if class exists in detection-result but not in ground-truth then there are no true positives in that class
         if class_name not in gt_classes:
             count_true_positives[class_name] = 0
     # print(count_true_positives)
 
     # Saving results and ploting
     if draw_plot:
         window_title = "detection-results-info"
         # Plot title
         plot_title = "detection-results\n"
         plot_title += "(" + str(len(dr_files_list)) + " files and "
         count_non_zero_values_in_dictionary = sum(
-            int(x) > 0 for x in list(det_counter_per_class.values()))
-        plot_title += str(count_non_zero_values_in_dictionary) + \
-            " detected classes)"
+            int(x) > 0 for x in list(det_counter_per_class.values())
+        )
+        plot_title += str(count_non_zero_values_in_dictionary) + " detected classes)"
         # end Plot title
         x_label = "Number of objects per class"
         output_path = results_files_path + "/detection-results-info.png"
         to_show = False
-        plot_color = 'forestgreen'
+        plot_color = "forestgreen"
         true_p_bar = count_true_positives
         draw_plot_func(
             det_counter_per_class,
             len(det_counter_per_class),
             window_title,
             plot_title,
             x_label,
             output_path,
             to_show,
             plot_color,
-            true_p_bar
+            true_p_bar,
         )
 
-    with open(results_files_path + "/results.txt", 'a') as results_file:
+    with open(results_files_path + "/results.txt", "a") as results_file:
         results_file.write("\n# Number of detected objects per class\n")
         for class_name in sorted(dr_classes):
             n_det = det_counter_per_class[class_name]
             text = class_name + ": " + str(n_det)
             text += " (tp:" + str(count_true_positives[class_name]) + ""
-            text += ", fp:" + \
-                str(n_det - count_true_positives[class_name]) + ")\n"
+            text += ", fp:" + str(n_det - count_true_positives[class_name]) + ")\n"
             results_file.write(text)
 
     if draw_plot:
         window_title = "lamr"
         plot_title = "log-average miss rate"
         x_label = "log-average miss rate"
         output_path = results_files_path + "/lamr.png"
         to_show = False
-        plot_color = 'royalblue'
+        plot_color = "royalblue"
         draw_plot_func(
             lamr_dictionary,
             n_classes,
             window_title,
             plot_title,
             x_label,
             output_path,
             to_show,
             plot_color,
-            ""
+            "",
         )
 
     if draw_plot:
         window_title = "mAP"
-        plot_title = "mAP = {0:.2f}%".format(mAP*100)
+        plot_title = "mAP = {0:.2f}%".format(mAP * 100)
         x_label = "Average Precision"
         output_path = results_files_path + "/mAP.png"
         to_show = True
-        plot_color = 'royalblue'
+        plot_color = "royalblue"
         draw_plot_func(
             ap_dictionary,
             n_classes,
             window_title,
             plot_title,
             x_label,
             output_path,
             to_show,
             plot_color,
-            ""
+            "",
         )
-
-
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/extract_voc.py` & `alfred-py-3.0.7/alfred/modules/data/extract_voc.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,110 +44,126 @@
     vars = root.findall(name)
     return vars
 
 
 def get_and_check(root, name, length):
     vars = root.findall(name)
     if len(vars) == 0:
-        raise NotImplementedError('Can not find %s in %s.'%(name, root.tag))
+        raise NotImplementedError("Can not find %s in %s." % (name, root.tag))
     if length > 0 and len(vars) != length:
-        raise NotImplementedError('The size of %s is supposed to be %d, but is %d.'%(name, length, len(vars)))
+        raise NotImplementedError(
+            "The size of %s is supposed to be %d, but is %d."
+            % (name, length, len(vars))
+        )
     if length == 1:
         vars = vars[0]
     return vars
 
 
 def get_filename_as_int(filename):
     try:
         filename = os.path.splitext(filename)[0]
         return int(filename)
     except:
-        raise NotImplementedError('Filename %s is supposed to be an integer.'%(filename))
+        raise NotImplementedError(
+            "Filename %s is supposed to be an integer." % (filename)
+        )
 
 
 def convert(xml_dir, output_dir, img_dir, xml_list=None):
-    assert os.path.join('image dir {} not exist'.format(img_dir))
+    assert os.path.join("image dir {} not exist".format(img_dir))
     os.makedirs(output_dir, exist_ok=True)
     if xml_list:
-        list_fp = open(xml_list, 'r')
+        list_fp = open(xml_list, "r")
     else:
         list_fp = os.listdir(xml_dir)
-    logging.info('we got all xml files: {}'.format(len(list_fp)))
-    json_dict = {"images":[], "type": "instances", "annotations": [],
-                 "categories": []}
+    logging.info("we got all xml files: {}".format(len(list_fp)))
+    json_dict = {"images": [], "type": "instances", "annotations": [], "categories": []}
 
     i = 0
     for line in list_fp:
         line = line.strip()
-        print("Processing %s"%(line))
+        print("Processing %s" % (line))
         xml_f = os.path.join(xml_dir, line)
         tree = ET.parse(xml_f)
         root = tree.getroot()
-        path = get(root, 'path')
+        path = get(root, "path")
         if len(path) == 1:
             filename = os.path.basename(path[0].text)
         elif len(path) == 0:
-            filename = get_and_check(root, 'filename', 1).text
+            filename = get_and_check(root, "filename", 1).text
         else:
-            raise NotImplementedError('%d paths found in %s'%(len(path), line))
+            raise NotImplementedError("%d paths found in %s" % (len(path), line))
         # compare filename with xml filename
-        if os.path.basename(xml_f).split('.')[0] != filename.split('.')[0]:
+        if os.path.basename(xml_f).split(".")[0] != filename.split(".")[0]:
             # if not equal, we replace filename with xml file name
             # print('{} != {}'.format(os.path.basename(xml_f).split('.')[0], filename.split('.')[0]))
-            filename = os.path.basename(xml_f).split('.')[0] + '.' + filename.split('.')[-1]
-            print('revise filename to: {}'.format(filename))
+            filename = (
+                os.path.basename(xml_f).split(".")[0] + "." + filename.split(".")[-1]
+            )
+            print("revise filename to: {}".format(filename))
         ## The filename must be a number
         # image_id = get_filename_as_int(filename)
         image_id = i
-        size = get_and_check(root, 'size', 1)
-        width = int(get_and_check(size, 'width', 1).text)
-        height = int(get_and_check(size, 'height', 1).text)
-        image = {'file_name': filename, 'height': height, 'width': width,
-                 'id':image_id}
-        json_dict['images'].append(image)
+        size = get_and_check(root, "size", 1)
+        width = int(get_and_check(size, "width", 1).text)
+        height = int(get_and_check(size, "height", 1).text)
+        image = {
+            "file_name": filename,
+            "height": height,
+            "width": width,
+            "id": image_id,
+        }
+        json_dict["images"].append(image)
         ## Cruuently we do not support segmentation
         #  segmented = get_and_check(root, 'segmented', 1).text
         #  assert segmented == '0'
-        
+
         img_root = img_dir
-        img_f = os.path.join(img_root, os.path.basename(xml_f).replace('xml', 'jpg'))
-        assert img_f, '{} not exist'.format(img_f)
-        logging.info('reading image from: {}'.format(img_f))
+        img_f = os.path.join(img_root, os.path.basename(xml_f).replace("xml", "jpg"))
+        assert img_f, "{} not exist".format(img_f)
+        logging.info("reading image from: {}".format(img_f))
         ori_img = cv2.imread(img_f)
         bx_id = 0
-        for obj in get(root, 'object'):
-            category = get_and_check(obj, 'name', 1).text
-            bndbox = get_and_check(obj, 'bndbox', 1)
-            xmin = float(get_and_check(bndbox, 'xmin', 1).text)
-            ymin = float(get_and_check(bndbox, 'ymin', 1).text)
-            xmax = float(get_and_check(bndbox, 'xmax', 1).text)
-            ymax = float(get_and_check(bndbox, 'ymax', 1).text)
-            assert(xmax > xmin)
-            assert(ymax > ymin)
-            
+        for obj in get(root, "object"):
+            category = get_and_check(obj, "name", 1).text
+            bndbox = get_and_check(obj, "bndbox", 1)
+            xmin = float(get_and_check(bndbox, "xmin", 1).text)
+            ymin = float(get_and_check(bndbox, "ymin", 1).text)
+            xmax = float(get_and_check(bndbox, "xmax", 1).text)
+            ymax = float(get_and_check(bndbox, "ymax", 1).text)
+            assert xmax > xmin
+            assert ymax > ymin
+
             # we got an image patch and will save it
             # print('{} - {}, {} - {}'.format(int(xmin), int(xmax), int(ymin), int(ymax)))
-            img_patch = ori_img[ int(ymin):int(ymax), int(xmin):int(xmax)]
+            img_patch = ori_img[int(ymin) : int(ymax), int(xmin) : int(xmax)]
             # cv2.imshow('rr', img_patch)
             # cv2.waitKey(0)
             # print(category)
             os.makedirs(os.path.join(output_dir, category), exist_ok=True)
-            to_save_f = os.path.join(output_dir, category, '{}_{}.jpg'.format(i, bx_id))
+            to_save_f = os.path.join(output_dir, category, "{}_{}.jpg".format(i, bx_id))
             cv2.imwrite(to_save_f, img_patch)
             bx_id += 1
         # image_id plus 1
         i += 1
-    logging.info('done.')
+    logging.info("done.")
 
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Extract image patchs from VOC annotations.')
-    parser.add_argument('--xml_dir', '-x', type=str, help='xml dir')
-    parser.add_argument('--image_dir', '-i', type=str, default='JPEGImages', help='xml dir')
-    parser.add_argument('--output_dir', '-o', type=str, default='extracted_out', help='xml dir')
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(
+        description="Extract image patchs from VOC annotations."
+    )
+    parser.add_argument("--xml_dir", "-x", type=str, help="xml dir")
+    parser.add_argument(
+        "--image_dir", "-i", type=str, default="JPEGImages", help="xml dir"
+    )
+    parser.add_argument(
+        "--output_dir", "-o", type=str, default="extracted_out", help="xml dir"
+    )
     args = parser.parse_args()
 
     xml = args.xml_dir
     img = args.image_dir
     output = args.output_dir
 
-    convert(xml, output, img)
+    convert(xml, output, img)
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/gather_voclabels.py` & `alfred-py-3.0.7/alfred/modules/data/gather_voclabels.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,50 +32,50 @@
 gather the label from Annotations
 """
 import os
 import pickle
 import os.path
 import sys
 import numpy as np
+
 if sys.version_info[0] == 2:
     import xml.etree.cElementTree as ET
 else:
     import xml.etree.ElementTree as ET
 import glob
 
 
-
 def gather_labels(anno_dir):
-    all_labels = glob.glob(os.path.join(anno_dir, '*.xml'))
+    all_labels = glob.glob(os.path.join(anno_dir, "*.xml"))
     all_names = []
     all_obj_num = 0
     xmls_without_boxes = []
     i = 0
     cls_num_map = dict()
     for label in all_labels:
         if i % 500 == 0:
-            print('parsing [{}/{}] {}'.format(i, len(all_labels), label))
+            print("parsing [{}/{}] {}".format(i, len(all_labels), label))
         i += 1
         root = ET.parse(label).getroot()
         one_sample_obj_num = 0
-        for obj in root.iter('object'):
+        for obj in root.iter("object"):
             one_sample_obj_num += 1
-            name = obj.find('name').text
+            name = obj.find("name").text
             if name in cls_num_map.keys():
                 cls_num_map[name] += 1
             else:
                 cls_num_map[name] = 0
             if name not in all_names:
                 all_names.append(name)
         if one_sample_obj_num == 0:
             xmls_without_boxes.append(label)
         all_obj_num += one_sample_obj_num
-    print('Done. summary...')
-    print('all {} classes.'.format(len(all_names)))
+    print("Done. summary...")
+    print("all {} classes.".format(len(all_names)))
     print(all_names)
     # we also read xmls with empty boxes
-    print('\nclass boxes statistic as: {}'.format(cls_num_map))
+    print("\nclass boxes statistic as: {}".format(cls_num_map))
     if len(xmls_without_boxes) > 0:
-        print('\nalso, we found these files without any detections, you can consider remove it:')
+        print(
+            "\nalso, we found these files without any detections, you can consider remove it:"
+        )
         print(xmls_without_boxes)
-
-
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/labelone_view.py` & `alfred-py-3.0.7/alfred/modules/data/labelone_view.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/data/mergevoc.py` & `alfred-py-3.0.7/alfred/modules/data/mergevoc.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,86 +38,98 @@
 from alfred.utils.log import logger as logging
 from pascal_voc_writer import Writer
 
 
 def get_and_check(root, name, length):
     vars = root.findall(name)
     if len(vars) == 0:
-        raise NotImplementedError('Can not find %s in %s.' % (name, root.tag))
+        raise NotImplementedError("Can not find %s in %s." % (name, root.tag))
     if length > 0 and len(vars) != length:
-        raise NotImplementedError('The size of %s is supposed to be %d, but is %d.' % (name, length, len(vars)))
+        raise NotImplementedError(
+            "The size of %s is supposed to be %d, but is %d."
+            % (name, length, len(vars))
+        )
     if length == 1:
         vars = vars[0]
     return vars
 
 
 def get(root, name):
     vars = root.findall(name)
     return vars
 
+
 def merge_multiple_voc_labels(n_merge_files, target_save_root):
     # one of n_merge_files must exist, but no sure which one, found it out
     f_name = os.path.basename(n_merge_files[0])
     n = len(n_merge_files)
     for f in n_merge_files:
         if os.path.exists(f):
             tree = ET.parse(f)
             root = tree.getroot()
-            objs = get(root, 'object')
+            objs = get(root, "object")
             n_merge_files.remove(f)
             break
     for xml in n_merge_files:
         if os.path.exists(xml):
             t = ET.parse(xml)
             r = t.getroot()
-            for obj in get(r, 'object'):
+            for obj in get(r, "object"):
                 root.append(obj)
-    # how to save 
+    # how to save
 
     # f = open(os.path.join(target_save_root, f_name), 'wb')
     # f.write(etree.tostring(root, pretty_print=True))
     # f.close()
     tree.write(os.path.join(target_save_root, f_name))
-    print('merged {} xmls and saved into: {}'.format(n, os.path.join(target_save_root, f_name)))
+    print(
+        "merged {} xmls and saved into: {}".format(
+            n, os.path.join(target_save_root, f_name)
+        )
+    )
 
 
-def merge_voc(label_root_list, style='intersection', label_major=True):
+def merge_voc(label_root_list, style="intersection", label_major=True):
     """
     For intersection: only merges their intersection part;
     For union: will merge all of them
 
     merge VOC with multiple datasets (one of them may have partial object labeled)
     """
-    logging.info('labels root: {}'.format(label_root_list))
+    logging.info("labels root: {}".format(label_root_list))
     # these labels may not perfectly aligned, we get a union of them
     filenames = []
-    if style == 'union':
-        logging.info('merge with union style.')
+    if style == "union":
+        logging.info("merge with union style.")
         for l in label_root_list:
             xmls = [os.path.basename(i) for i in glob(os.path.join(l, "*.xml"))]
-            logging.info('found {} xmls under: {}'.format(len(xmls), l))
+            logging.info("found {} xmls under: {}".format(len(xmls), l))
             # filenames.extend([i for i in xmls if i not in filenames])
             filenames.extend(xmls)
     else:
-        logging.info('merge with intersection style.')
+        logging.info("merge with intersection style.")
         for l in label_root_list:
             xmls = [os.path.basename(i) for i in glob(os.path.join(l, "*.xml"))]
-            logging.info('found {} xmls under: {}'.format(len(xmls), l))
+            logging.info("found {} xmls under: {}".format(len(xmls), l))
             # filenames.extend([i for i in xmls if i not in filenames])
             if len(filenames) > 0:
                 filenames = set(xmls) & set(filenames)
             filenames = xmls
 
     filenames = list(set(filenames))
-    logging.info('found {} xmls which exist both inside all provided label roots.'.format(len(filenames)))
-    target_save_root = './merged_voc_annotations'
+    logging.info(
+        "found {} xmls which exist both inside all provided label roots.".format(
+            len(filenames)
+        )
+    )
+    target_save_root = "./merged_voc_annotations"
     os.makedirs(target_save_root, exist_ok=True)
     for f in filenames:
         n_merge_files = []
         for l in label_root_list:
             n_merge_files.append(os.path.join(l, f))
         merge_multiple_voc_labels(n_merge_files, target_save_root)
-    print('done.')
+    print("done.")
 
 
 if __name__ == "__main__":
     merge_voc(sys.argv[1], sys.argv[2])
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/split_coco.py` & `alfred-py-3.0.7/alfred/modules/data/split_coco.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,85 @@
-
-
 """
 
 Split coco dataset
 
 """
 import json
 import argparse
 import funcy
 from sklearn.model_selection import train_test_split
 import os
 
 
 def save_coco(file, info, licenses, images, annotations, categories):
-    with open(file, 'wt', encoding='UTF-8') as coco:
-        json.dump({'info': info, 'licenses': licenses, 'images': images,
-                   'annotations': annotations, 'categories': categories}, coco, indent=2, sort_keys=True)
+    with open(file, "wt", encoding="UTF-8") as coco:
+        json.dump(
+            {
+                "info": info,
+                "licenses": licenses,
+                "images": images,
+                "annotations": annotations,
+                "categories": categories,
+            },
+            coco,
+            indent=2,
+            sort_keys=True,
+        )
 
 
 def filter_annotations(annotations, images):
-    image_ids = funcy.lmap(lambda i: int(i['id']), images)
-    return funcy.lfilter(lambda a: int(a['image_id']) in image_ids, annotations)
+    image_ids = funcy.lmap(lambda i: int(i["id"]), images)
+    return funcy.lfilter(lambda a: int(a["image_id"]) in image_ids, annotations)
 
 
 def split_coco(ann_f, split=0.8, remove_empty=False):
-    train_f = os.path.join(os.path.dirname(ann_f), os.path.basename(
-        ann_f).replace('.json', '_train.json'))
-    val_f = os.path.join(os.path.dirname(ann_f), os.path.basename(
-        ann_f).replace('.json', '_val.json'))
-    with open(ann_f, 'rt', encoding='UTF-8') as annotations:
+    train_f = os.path.join(
+        os.path.dirname(ann_f), os.path.basename(ann_f).replace(".json", "_train.json")
+    )
+    val_f = os.path.join(
+        os.path.dirname(ann_f), os.path.basename(ann_f).replace(".json", "_val.json")
+    )
+    with open(ann_f, "rt", encoding="UTF-8") as annotations:
         coco = json.load(annotations)
-        info = ''
-        if 'info' in coco.keys():
-            info = coco['info']
-        licenses = ''
-        if 'licenses' in coco.keys():
-            licenses = coco['licenses']
-        images = coco['images']
-        annotations = coco['annotations']
-        categories = coco['categories']
+        info = ""
+        if "info" in coco.keys():
+            info = coco["info"]
+        licenses = ""
+        if "licenses" in coco.keys():
+            licenses = coco["licenses"]
+        images = coco["images"]
+        annotations = coco["annotations"]
+        categories = coco["categories"]
 
         number_of_images = len(images)
 
         if remove_empty:
             images_with_annotations = funcy.lmap(
-                lambda a: int(a['image_id']), annotations)
+                lambda a: int(a["image_id"]), annotations
+            )
 
             # filter out images without annotations
             images = funcy.lremove(
-                lambda i: i['id'] not in images_with_annotations, images)
-            print('removed {} images without annotations, all images: {}, now: {}'.format(
-                number_of_images-len(images), number_of_images, len(images)
-            ))
+                lambda i: i["id"] not in images_with_annotations, images
+            )
+            print(
+                "removed {} images without annotations, all images: {}, now: {}".format(
+                    number_of_images - len(images), number_of_images, len(images)
+                )
+            )
         else:
-            print('all images: {}'.format(number_of_images))
+            print("all images: {}".format(number_of_images))
 
         x, y = train_test_split(images, train_size=float(split))
 
-        save_coco(train_f, info, licenses, x,
-                  filter_annotations(annotations, x), categories)
-        save_coco(val_f, info, licenses, y,
-                  filter_annotations(annotations, y), categories)
-
-        print("Saved {} entries in {} and {} in {}.".format(
-            len(x), train_f, len(y), val_f))
+        save_coco(
+            train_f, info, licenses, x, filter_annotations(annotations, x), categories
+        )
+        save_coco(
+            val_f, info, licenses, y, filter_annotations(annotations, y), categories
+        )
+
+        print(
+            "Saved {} entries in {} and {} in {}.".format(
+                len(x), train_f, len(y), val_f
+            )
+        )
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/split_voc.py` & `alfred-py-3.0.7/alfred/modules/data/split_voc.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 import os
 import glob
 import numpy as np
 
-save_dir = './ImageSets/Main'
+save_dir = "./ImageSets/Main"
 os.makedirs(save_dir, exist_ok=True)
 
-all_imgs = [os.path.basename(i).split('.')[0]+'\n' for i in glob.glob('./JPEGImages/*.jpg')]
+all_imgs = [
+    os.path.basename(i).split(".")[0] + "\n" for i in glob.glob("./JPEGImages/*.jpg")
+]
 
 ratio = 0.9
-print('Found {} images, spliting ratio is 0.9'.format(len(all_imgs)))
+print("Found {} images, spliting ratio is 0.9".format(len(all_imgs)))
 
 np.random.shuffle(all_imgs)
 split = int(len(all_imgs) * ratio)
-train_ids = all_imgs[: split]
-val_ids = all_imgs[split: ]
-print('{} for train, {} for validation.'.format(len(train_ids), len(val_ids)))
+train_ids = all_imgs[:split]
+val_ids = all_imgs[split:]
+print("{} for train, {} for validation.".format(len(train_ids), len(val_ids)))
 
-print('saving split..')
-with open(os.path.join(save_dir, 'train.txt'), 'w') as f:
+print("saving split..")
+with open(os.path.join(save_dir, "train.txt"), "w") as f:
     f.writelines(train_ids)
-with open(os.path.join(save_dir, 'val.txt'), 'w') as f:
+with open(os.path.join(save_dir, "val.txt"), "w") as f:
     f.writelines(val_ids)
-print('Done.')
+print("Done.")
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/txt2voc.py` & `alfred-py-3.0.7/alfred/modules/data/txt2voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import xml.etree.cElementTree as ET
 from PIL import Image
 import sys
 import glob
 
 
 CLASS_MAPPING = {
-    '0': 'name'
+    "0": "name"
     # Add your remaining classes here.
 }
 
 
 def create_root(file_prefix, width, height):
     root = ET.Element("annotations")
     ET.SubElement(root, "filename").text = "{}.jpg".format(file_prefix)
@@ -70,15 +70,15 @@
 
 
 def read_file(file_path, des_dir):
     file_prefix = os.path.basename(file_path).split(".txt")[0]
     image_file_name = "{}.jpg".format(file_prefix)
     img = Image.open("{}/{}".format("images", image_file_name))
     w, h = img.size
-    with open(file_path, 'r') as file:
+    with open(file_path, "r") as file:
         lines = file.readlines()
         voc_labels = []
         for line in lines:
             voc = []
             line = line.strip()
             data = line.split()
             # voc.append(CLASS_MAPPING.get(data[0]))
@@ -93,16 +93,16 @@
             voc.append(center_y + (bbox_height / 2))
             voc_labels.append(voc)
         create_file(file_prefix, w, h, voc_labels, des_dir)
     print("Processing complete for file: {}".format(file_path))
 
 
 def start(dir_name):
-    des_d = 'output_xmls'
+    des_d = "output_xmls"
     os.makedirs(des_d, exist_ok=True)
-    txts = glob.glob(os.path.join(dir_name, '*.txt'))
+    txts = glob.glob(os.path.join(dir_name, "*.txt"))
     for filename in txts:
         read_file(filename, des_d)
 
 
 if __name__ == "__main__":
     start(sys.argv[1])
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/view_coco.py` & `alfred-py-3.0.7/alfred/modules/data/view_coco.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,20 +161,20 @@
 
     which essential for visualize a custom dataset
     """
     coco = COCO(ann_f)
     cats = coco.loadCats(coco.getCatIds())
 
     res = {}
-    res["class_names"] = [i['name'] for i in cats]
+    res["class_names"] = [i["name"] for i in cats]
 
     skeleton_dict = {}
     for c in cats:
         if "skeleton" in c.keys():
-            skeleton_dict[c['name']] = c["skeleton"]
+            skeleton_dict[c["name"]] = c["skeleton"]
     res["skeleton_dict"] = skeleton_dict
     return res
 
 
 def vis_coco(coco_img_root, ann_f):
     data_dir = coco_img_root
     coco = COCO(ann_f)
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/view_txt.py` & `alfred-py-3.0.7/alfred/modules/data/view_txt.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,47 +34,64 @@
 import os
 import sys
 import cv2
 from alfred.utils.log import logger as logging
 
 
 def vis_det_txt(img_root, label_root):
-    logging.info('img root: {}, label root: {}'.format(img_root, label_root))
+    logging.info("img root: {}, label root: {}".format(img_root, label_root))
     # auto detection .jpg or .png images
-    txt_files = glob(os.path.join(label_root, '*.txt'))
+    txt_files = glob(os.path.join(label_root, "*.txt"))
     for txt_f in txt_files:
-        img_f = os.path.join(img_root, os.path.basename(txt_f).split('.')[0] + '.jpg')
+        img_f = os.path.join(img_root, os.path.basename(txt_f).split(".")[0] + ".jpg")
         if os.path.exists(img_f):
             img = cv2.imread(img_f)
             if os.path.exists(txt_f):
                 with open(txt_f) as f:
                     annos = f.readlines()
                     for ann in annos:
-                        ann = ann.strip().split(' ')
+                        ann = ann.strip().split(" ")
                         if len(ann) == 5:
                             # not include prob
                             category = ann[0]
                             xmin = int(float(ann[1]))
                             ymin = int(float(ann[2]))
                             xmax = int(float(ann[3]))
                             ymax = int(float(ann[4]))
-                            cv2.putText(img, category, (xmin, ymin), cv2.FONT_HERSHEY_COMPLEX, 0.7, (255, 255, 255))
-                            cv2.rectangle(img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1)
+                            cv2.putText(
+                                img,
+                                category,
+                                (xmin, ymin),
+                                cv2.FONT_HERSHEY_COMPLEX,
+                                0.7,
+                                (255, 255, 255),
+                            )
+                            cv2.rectangle(
+                                img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1
+                            )
                         elif len(ann) == 6:
                             # include prob
                             category = ann[0]
                             prob = float(ann[1])
                             xmin = int(float(ann[2]))
                             ymin = int(float(ann[3]))
                             xmax = int(float(ann[4]))
                             ymax = int(float(ann[5]))
-                            cv2.putText(img, '{} {}'.format(category, prob), (xmin, ymin), 
-                            cv2.FONT_HERSHEY_COMPLEX, 0.7, (255, 255, 255))
-                            cv2.rectangle(img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1)
-                cv2.imshow('txt check', img)
+                            cv2.putText(
+                                img,
+                                "{} {}".format(category, prob),
+                                (xmin, ymin),
+                                cv2.FONT_HERSHEY_COMPLEX,
+                                0.7,
+                                (255, 255, 255),
+                            )
+                            cv2.rectangle(
+                                img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1
+                            )
+                cv2.imshow("txt check", img)
                 cv2.waitKey(0)
             else:
-                logging.warning('xxxx image: {} not found.'.format(img_f))
+                logging.warning("xxxx image: {} not found.".format(img_f))
 
 
 if __name__ == "__main__":
     vis_det_txt(sys.argv[1], sys.argv[2])
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/view_voc.py` & `alfred-py-3.0.7/alfred/modules/data/view_voc.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,78 +37,113 @@
 import cv2
 from alfred.utils.log import logger as logging
 
 
 def get_and_check(root, name, length):
     vars = root.findall(name)
     if len(vars) == 0:
-        raise NotImplementedError('Can not find %s in %s.' % (name, root.tag))
+        raise NotImplementedError("Can not find %s in %s." % (name, root.tag))
     if length > 0 and len(vars) != length:
-        raise NotImplementedError('The size of %s is supposed to be %d, but is %d.' % (name, length, len(vars)))
+        raise NotImplementedError(
+            "The size of %s is supposed to be %d, but is %d."
+            % (name, length, len(vars))
+        )
     if length == 1:
         vars = vars[0]
     return vars
 
 
 def get(root, name):
     vars = root.findall(name)
     return vars
 
 
 def vis_voc(img_root, label_root, label_major=True):
-    logging.info('img root: {}, label root: {}'.format(img_root, label_root))
+    logging.info("img root: {}, label root: {}".format(img_root, label_root))
     # auto detection .jpg or .png images
     if label_major:
-        logging.info('label major will using xmls to found images... it might cause no image found')
-        xml_files = glob(os.path.join(label_root, '*.xml'))
+        logging.info(
+            "label major will using xmls to found images... it might cause no image found"
+        )
+        xml_files = glob(os.path.join(label_root, "*.xml"))
         for xml in xml_files:
             if os.path.exists(xml):
-                img_f = os.path.join(img_root, os.path.basename(xml).split('.')[0] + '.jpg')
+                img_f = os.path.join(
+                    img_root, os.path.basename(xml).split(".")[0] + ".jpg"
+                )
                 if not os.path.exists(img_f):
-                    logging.info('switch to png format')
-                    img_f = os.path.join(img_root, os.path.basename(xml).split('.')[0] + '.png')
+                    logging.info("switch to png format")
+                    img_f = os.path.join(
+                        img_root, os.path.basename(xml).split(".")[0] + ".png"
+                    )
                 img = cv2.imread(img_f)
                 if os.path.exists(img_f):
                     tree = ET.parse(xml)
                     root = tree.getroot()
-                    for obj in get(root, 'object'):
-                        category = get_and_check(obj, 'name', 1).text
-                        bndbox = get_and_check(obj, 'bndbox', 1)
-                        xmin = int(float(get_and_check(bndbox, 'xmin', 1).text))
-                        ymin = int(float(get_and_check(bndbox, 'ymin', 1).text))
-                        xmax = int(float(get_and_check(bndbox, 'xmax', 1).text))
-                        ymax = int(float(get_and_check(bndbox, 'ymax', 1).text))
-
-                        cv2.putText(img, category, (xmin, ymin), cv2.FONT_HERSHEY_COMPLEX, 0.7, (255, 255, 255))
-                        cv2.rectangle(img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1)
-                    cv2.imshow('voc check', img)
+                    for obj in get(root, "object"):
+                        category = get_and_check(obj, "name", 1).text
+                        bndbox = get_and_check(obj, "bndbox", 1)
+                        xmin = int(float(get_and_check(bndbox, "xmin", 1).text))
+                        ymin = int(float(get_and_check(bndbox, "ymin", 1).text))
+                        xmax = int(float(get_and_check(bndbox, "xmax", 1).text))
+                        ymax = int(float(get_and_check(bndbox, "ymax", 1).text))
+
+                        cv2.putText(
+                            img,
+                            category,
+                            (xmin, ymin),
+                            cv2.FONT_HERSHEY_COMPLEX,
+                            0.7,
+                            (255, 255, 255),
+                        )
+                        cv2.rectangle(
+                            img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1
+                        )
+                    cv2.imshow("voc check", img)
                     cv2.waitKey(0)
                 else:
-                    logging.warning('xxxx image: {} for label: {} not found.'.format(img_f, xml))
+                    logging.warning(
+                        "xxxx image: {} for label: {} not found.".format(img_f, xml)
+                    )
     else:
-        img_files = glob(os.path.join(img_root, '*.[jp][pn]g'))
+        img_files = glob(os.path.join(img_root, "*.[jp][pn]g"))
         for img_f in img_files:
             if os.path.exists(img_f):
                 img = cv2.imread(img_f)
-                label_path = os.path.join(label_root, os.path.basename(img_f).split('.')[0] + '.xml')
+                label_path = os.path.join(
+                    label_root, os.path.basename(img_f).split(".")[0] + ".xml"
+                )
                 if os.path.exists(label_path):
                     #
                     tree = ET.parse(label_path)
                     root = tree.getroot()
-                    for obj in get(root, 'object'):
-                        category = get_and_check(obj, 'name', 1).text
-                        bndbox = get_and_check(obj, 'bndbox', 1)
-                        xmin = int(float(get_and_check(bndbox, 'xmin', 1).text))
-                        ymin = int(float(get_and_check(bndbox, 'ymin', 1).text))
-                        xmax = int(float(get_and_check(bndbox, 'xmax', 1).text))
-                        ymax = int(float(get_and_check(bndbox, 'ymax', 1).text))
-
-                        cv2.putText(img, category, (xmin, ymin), cv2.FONT_HERSHEY_COMPLEX, 0.7, (255, 255, 255))
-                        cv2.rectangle(img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1)
-                    cv2.imshow('voc check', img)
+                    for obj in get(root, "object"):
+                        category = get_and_check(obj, "name", 1).text
+                        bndbox = get_and_check(obj, "bndbox", 1)
+                        xmin = int(float(get_and_check(bndbox, "xmin", 1).text))
+                        ymin = int(float(get_and_check(bndbox, "ymin", 1).text))
+                        xmax = int(float(get_and_check(bndbox, "xmax", 1).text))
+                        ymax = int(float(get_and_check(bndbox, "ymax", 1).text))
+
+                        cv2.putText(
+                            img,
+                            category,
+                            (xmin, ymin),
+                            cv2.FONT_HERSHEY_COMPLEX,
+                            0.7,
+                            (255, 255, 255),
+                        )
+                        cv2.rectangle(
+                            img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1
+                        )
+                    cv2.imshow("voc check", img)
                     cv2.waitKey(0)
                 else:
-                    logging.warning('xxxx image: {} according label: {} not found.'.format(img_f, label_path))
+                    logging.warning(
+                        "xxxx image: {} according label: {} not found.".format(
+                            img_f, label_path
+                        )
+                    )
 
 
 if __name__ == "__main__":
     vis_voc(sys.argv[1], sys.argv[2])
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/view_yolo.py` & `alfred-py-3.0.7/alfred/modules/data/view_yolo.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,44 +34,53 @@
 import os
 import sys
 import cv2
 from alfred.utils.log import logger as logging
 
 
 def vis_det_yolo(img_root, label_root):
-    logging.info('img root: {}, label root: {}'.format(img_root, label_root))
+    logging.info("img root: {}, label root: {}".format(img_root, label_root))
     # auto detection .jpg or .png images
-    txt_files = glob(os.path.join(label_root, '*.txt'))
+    txt_files = glob(os.path.join(label_root, "*.txt"))
     for txt_f in txt_files:
         txt_root, txt_ext = os.path.splitext(txt_f)
-        img_f = os.path.join(img_root, os.path.basename(txt_root) + '.jpg')
+        img_f = os.path.join(img_root, os.path.basename(txt_root) + ".jpg")
         # img_f = os.path.join(img_root, os.path.basename(txt_f).split('.')[0] + '.jpg')
         if os.path.exists(img_f):
             img = cv2.imread(img_f)
             h, w, _ = img.shape
             if os.path.exists(txt_f):
                 with open(txt_f) as f:
-                    annos = f.readlines() 
+                    annos = f.readlines()
                     for ann in annos:
-                        ann = ann.strip().split(' ')
+                        ann = ann.strip().split(" ")
                         category = ann[0]
                         x = float(ann[1]) * w
                         y = float(ann[2]) * h
                         bw = float(ann[3]) * w
                         bh = float(ann[4]) * h
-                        xmin = int(x - bw/2)
-                        ymin = int(y - bh/2)
-                        xmax = int(x + bw/2)
-                        ymax = int(y + bh/2)
+                        xmin = int(x - bw / 2)
+                        ymin = int(y - bh / 2)
+                        xmax = int(x + bw / 2)
+                        ymax = int(y + bh / 2)
                         print(xmin, ymin, xmax, ymax, category)
-                        cv2.putText(img, category, (xmin, ymin), cv2.FONT_HERSHEY_COMPLEX, 0.7, (255, 255, 255))
-                        cv2.rectangle(img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1)
-                cv2.imshow('yolo check', img)
+                        cv2.putText(
+                            img,
+                            category,
+                            (xmin, ymin),
+                            cv2.FONT_HERSHEY_COMPLEX,
+                            0.7,
+                            (255, 255, 255),
+                        )
+                        cv2.rectangle(
+                            img, (xmin, ymin), (xmax, ymax), (0, 255, 0), 2, 1
+                        )
+                cv2.imshow("yolo check", img)
                 ch = cv2.waitKey(0)
                 if ch == 27:
                     exit()
             else:
-                logging.warning('xxxx image: {} not found.'.format(img_f))
+                logging.warning("xxxx image: {} not found.".format(img_f))
 
 
 if __name__ == "__main__":
     vis_det_txt(sys.argv[1], sys.argv[2])
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/voc2coco.py` & `alfred-py-3.0.7/alfred/modules/data/voc2coco.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/data/voc2yolo.py` & `alfred-py-3.0.7/alfred/modules/data/voc2yolo.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,62 +3,65 @@
 import os
 from os import listdir, getcwd
 from os.path import join
 import sys
 import glob
 
 
-
 def convert(size, box):
-    dw = 1./(size[0])
-    dh = 1./(size[1])
-    x = (box[0] + box[1])/2.0 - 1
-    y = (box[2] + box[3])/2.0 - 1
+    dw = 1.0 / (size[0])
+    dh = 1.0 / (size[1])
+    x = (box[0] + box[1]) / 2.0 - 1
+    y = (box[2] + box[3]) / 2.0 - 1
     w = box[1] - box[0]
     h = box[3] - box[2]
-    x = x*dw
-    w = w*dw
-    y = y*dh
-    h = h*dh
+    x = x * dw
+    w = w * dw
+    y = y * dh
+    h = h * dh
     return (x, y, w, h)
 
 
 def convert_annotation(xml_f, target_dir, classes_names):
-    f_name = os.path.basename(xml_f).split('.')[0] + '.txt'
-    out_file = open(os.path.join(target_dir, f_name), 'w')
+    f_name = os.path.basename(xml_f).split(".")[0] + ".txt"
+    out_file = open(os.path.join(target_dir, f_name), "w")
 
     tree = ET.parse(xml_f)
     root = tree.getroot()
-    size = root.find('size')
-    w = int(size.find('width').text)
-    h = int(size.find('height').text)
-
-    for obj in root.iter('object'):
-        difficult = obj.find('difficult').text
-        cls = obj.find('name').text
+    size = root.find("size")
+    w = int(size.find("width").text)
+    h = int(size.find("height").text)
+
+    for obj in root.iter("object"):
+        difficult = obj.find("difficult").text
+        cls = obj.find("name").text
         if cls not in classes_names or int(difficult) == 1:
             continue
         cls_id = classes_names.index(cls)
-        xmlbox = obj.find('bndbox')
-        b = (float(xmlbox.find('xmin').text), float(xmlbox.find('xmax').text), float(
-            xmlbox.find('ymin').text), float(xmlbox.find('ymax').text))
+        xmlbox = obj.find("bndbox")
+        b = (
+            float(xmlbox.find("xmin").text),
+            float(xmlbox.find("xmax").text),
+            float(xmlbox.find("ymin").text),
+            float(xmlbox.find("ymax").text),
+        )
         bb = convert((w, h), b)
-        out_file.write(str(cls_id) + " " +
-                       " ".join([str(a) for a in bb]) + '\n')
-
+        out_file.write(str(cls_id) + " " + " ".join([str(a) for a in bb]) + "\n")
 
 
 def voc2yolo(img_dir, xml_dir, class_txt):
     classes_names = None
     if class_txt:
-        classes_names = [i.strip() for i in open(class_txt, 'r').readlines()]
+        classes_names = [i.strip() for i in open(class_txt, "r").readlines()]
 
-    labels_target = os.path.join(os.path.dirname(xml_dir.rstrip('/')), 'yolo_converted_from_voc')
-    print('labels dir to save: {}'.format(labels_target))
+    labels_target = os.path.join(
+        os.path.dirname(xml_dir.rstrip("/")), "yolo_converted_from_voc"
+    )
+    print("labels dir to save: {}".format(labels_target))
     if not os.path.exists(labels_target):
         os.makedirs(labels_target)
 
-    xmls = glob.glob(os.path.join(xml_dir, '*.xml'))
+    xmls = glob.glob(os.path.join(xml_dir, "*.xml"))
     for xml in xmls:
         convert_annotation(xml, labels_target, classes_names)
-    print('Done!')
-    print('class name order used is: ', classes_names)
+    print("Done!")
+    print("class name order used is: ", classes_names)
```

### Comparing `alfred-py-3.0.6/alfred/modules/data/yolo2voc.py` & `alfred-py-3.0.7/alfred/modules/data/yolo2voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 """
 
 Converting standared Yolo format to VOC format
 here
 
 """
 
@@ -37,15 +35,15 @@
 import xml.etree.cElementTree as ET
 from PIL import Image
 import sys
 import glob
 
 
 CLASS_MAPPING = {
-    '0': 'name'
+    "0": "name"
     # Add your remaining classes here.
 }
 
 
 def create_root(file_prefix, width, height):
     root = ET.Element("annotations")
     ET.SubElement(root, "filename").text = "{}.jpg".format(file_prefix)
@@ -79,20 +77,19 @@
     tree.write("{}/{}.xml".format(des_dir, file_prefix))
 
 
 def read_file(file_path, des_dir, img_dir, classes_names):
     file_prefix = os.path.basename(file_path).split(".txt")[0]
     image_file_name = "{}.jpg".format(file_prefix)
     img_p = os.path.join(img_dir, image_file_name)
-    assert os.path.exists(
-        img_p), 'make sure all images under: {}'.format(img_dir)
+    assert os.path.exists(img_p), "make sure all images under: {}".format(img_dir)
     img = Image.open(img_p)
 
     w, h = img.size
-    with open(file_path, 'r') as file:
+    with open(file_path, "r") as file:
         lines = file.readlines()
         voc_labels = []
         for line in lines:
             voc = []
             line = line.strip()
             data = line.split()
             # voc.append(CLASS_MAPPING.get(data[0]))
@@ -100,35 +97,35 @@
                 voc.append(classes_names[int(data[0])])
             else:
                 voc.append(data[0])
             bbox_width = float(data[3]) * w
             bbox_height = float(data[4]) * h
             cx = float(data[1]) * w
             cy = float(data[2]) * h
-            x = cx - bbox_width/2
-            y = cy - bbox_height/2
+            x = cx - bbox_width / 2
+            y = cy - bbox_height / 2
             voc.append(x)
             voc.append(y)
             voc.append(x + (bbox_width))
             voc.append(y + (bbox_height))
             voc_labels.append(voc)
         create_file(file_prefix, w, h, voc_labels, des_dir)
     print("Processing complete for file: {}".format(file_path))
 
 
 def yolo2voc(img_dir, txt_dir, class_txt):
     # TODO: need apply a map to mapping yolo label back
     classes_names = None
     if class_txt:
-        classes_names = [i.strip() for i in open(class_txt, 'r').readlines()]
-    des_d = 'Annotations_yolo_converted_for_voc'
-    des_d = os.path.join(os.path.dirname(txt_dir.rstrip('/')), des_d)
-    print('VOC Annotations will saved into: {}'.format(des_d))
+        classes_names = [i.strip() for i in open(class_txt, "r").readlines()]
+    des_d = "Annotations_yolo_converted_for_voc"
+    des_d = os.path.join(os.path.dirname(txt_dir.rstrip("/")), des_d)
+    print("VOC Annotations will saved into: {}".format(des_d))
     os.makedirs(des_d, exist_ok=True)
-    txts = glob.glob(os.path.join(txt_dir.rstrip('/'), '*.txt'))
-    print('found {} text files in yolo format.'.format(len(txts)))
+    txts = glob.glob(os.path.join(txt_dir.rstrip("/"), "*.txt"))
+    print("found {} text files in yolo format.".format(len(txts)))
     for filename in txts:
         read_file(filename, des_d, img_dir, classes_names)
 
 
 if __name__ == "__main__":
     yolo2voc(sys.argv[1], sys.argv[2], None)
```

### Comparing `alfred-py-3.0.6/alfred/modules/dltool/cal_anchors.py` & `alfred-py-3.0.7/alfred/modules/dltool/cal_anchors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 from glob import glob
 import os
 import xml.etree.ElementTree as ET
 
 
 class KmeansYolo:
-
-    def __init__(self, ann_dir, cluster_number, ann_format='voc'):
-        assert ann_format.lower() == 'voc' or ann_format.lower() == 'yolo', 'only support voc or yolo format now.'
+    def __init__(self, ann_dir, cluster_number, ann_format="voc"):
+        assert (
+            ann_format.lower() == "voc" or ann_format.lower() == "yolo"
+        ), "only support voc or yolo format now."
         self.cluster_number = cluster_number
         self.ann_dir = ann_dir
         self.ann_format = ann_format.lower()
-        print('KMeans clustering on: {} clusters.'.format(cluster_number))
+        print("KMeans clustering on: {} clusters.".format(cluster_number))
 
     def iou(self, boxes, clusters):  # 1 box -> k clusters
         n = boxes.shape[0]
         k = self.cluster_number
 
         box_area = boxes[:, 0] * boxes[:, 1]
         box_area = box_area.repeat(k)
@@ -42,99 +43,103 @@
         return accuracy
 
     def kmeans(self, boxes, k, dist=np.median):
         box_number = boxes.shape[0]
         distances = np.empty((box_number, k))
         last_nearest = np.zeros((box_number,))
         np.random.seed()
-        clusters = boxes[np.random.choice(
-            box_number, k, replace=False)]  # init k clusters
+        clusters = boxes[
+            np.random.choice(box_number, k, replace=False)
+        ]  # init k clusters
         while True:
-
             distances = 1 - self.iou(boxes, clusters)
 
             current_nearest = np.argmin(distances, axis=1)
             if (last_nearest == current_nearest).all():
                 break  # clusters won't change
             for cluster in range(k):
                 clusters[cluster] = dist(  # update clusters
-                    boxes[current_nearest == cluster], axis=0)
+                    boxes[current_nearest == cluster], axis=0
+                )
 
             last_nearest = current_nearest
 
         return clusters
 
     def result2txt(self, data):
-        f = open("yolo_anchors.txt", 'w')
+        f = open("yolo_anchors.txt", "w")
         row = np.shape(data)[0]
         for i in range(row):
             if i == 0:
                 x_y = "%d,%d" % (data[i][0], data[i][1])
             else:
                 x_y = ", %d,%d" % (data[i][0], data[i][1])
             f.write(x_y)
         f.close()
 
     def _load_yolo_boxes(self, ann_files):
-        assert isinstance(ann_files, list), 'ann_files must be a list'
+        assert isinstance(ann_files, list), "ann_files must be a list"
         dataSet = []
         for f in ann_files:
-            lines = open(f, 'r').readlines()
+            lines = open(f, "r").readlines()
             infos = [i.strip() for i in lines]
             for line in infos:
                 width = int(line.split(" ")[3])
                 height = int(line.split(",")[4])
                 dataSet.append([width, height])
         return dataSet
-    
+
     def _load_voc_boxes(self, ann_files):
-        assert isinstance(ann_files, list), 'ann_files must be a list'
+        assert isinstance(ann_files, list), "ann_files must be a list"
         dataSet = []
         for f in ann_files:
             tree = ET.parse(f)
             root = tree.getroot()
             # size = root.find('size')
             # im_w = int(size.find('width').text)
             # im_h = int(size.find('height').text)
 
-            for obj in root.iter('object'):
-                xmlbox = obj.find('bndbox')
-               
-                w = float(xmlbox.find('xmax').text) - float(xmlbox.find('xmin').text)
-                h = float(xmlbox.find('ymax').text) - float(xmlbox.find('ymin').text)
+            for obj in root.iter("object"):
+                xmlbox = obj.find("bndbox")
+
+                w = float(xmlbox.find("xmax").text) - float(xmlbox.find("xmin").text)
+                h = float(xmlbox.find("ymax").text) - float(xmlbox.find("ymin").text)
                 dataSet.append([w, h])
         return dataSet
 
     def txt2boxes(self):
         files = None
         dataSet = None
-        if self.ann_format == 'yolo':
-            files = glob(os.path.join(self.ann_dir, '*.txt'))
+        if self.ann_format == "yolo":
+            files = glob(os.path.join(self.ann_dir, "*.txt"))
             dataSet = self._load_yolo_boxes(files)
-            print('[WARN] yolo format anchor calculation **only** support relative anchor (same as YoloV5 format)' +
-            'if you want using it in YoloV3, you gonna need x image wh.')
-        elif self.ann_format == 'voc':
-            files = glob(os.path.join(self.ann_dir, '*.xml'))
+            print(
+                "[WARN] yolo format anchor calculation **only** support relative anchor (same as YoloV5 format)"
+                + "if you want using it in YoloV3, you gonna need x image wh."
+            )
+        elif self.ann_format == "voc":
+            files = glob(os.path.join(self.ann_dir, "*.xml"))
             dataSet = self._load_voc_boxes(files)
-        print('annotation format: {}, all: {} annos.'.format(self.ann_format, len(files)))
-        print('all boxes num: {}'.format(len(dataSet)))
+        print(
+            "annotation format: {}, all: {} annos.".format(self.ann_format, len(files))
+        )
+        print("all boxes num: {}".format(len(dataSet)))
         result = np.array(dataSet)
         return result
 
     def txt2clusters(self):
         all_boxes = self.txt2boxes()
-        print('clustering for anchors....')
+        print("clustering for anchors....")
         result = self.kmeans(all_boxes, k=self.cluster_number)
         result = result[np.lexsort(result.T[0, None])]
         self.result2txt(result)
         print("K anchors:\n {}".format(result))
-        print("Accuracy: {:.2f}%".format(
-            self.avg_iou(all_boxes, result) * 100))
+        print("Accuracy: {:.2f}%".format(self.avg_iou(all_boxes, result) * 100))
 
 
 if __name__ == "__main__":
     cluster_number = 9
     filename = "2012_train.txt"
     # Row format: image_file_path box1 box2 ... boxN;
     # Box format: x_min,y_min,x_max,y_max,class_id (no space).
     kmeans = KmeansYolo(cluster_number, filename)
-    kmeans.txt2clusters()
+    kmeans.txt2clusters()
```

### Comparing `alfred-py-3.0.6/alfred/modules/scrap/__init__.py` & `alfred-py-3.0.7/alfred/modules/scrap/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/scrap/image_scraper.py` & `alfred-py-3.0.7/alfred/modules/scrap/image_scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,36 +27,49 @@
 import os
 import argparse
 import random
 from colorama import Fore, Back, Style
 
 
 class ImageScraper(object):
-
     def __init__(self):
         pass
 
     @staticmethod
     def save_image(image_data, save_prefix, save_dir, index):
         if not os.path.exists(save_dir):
             os.mkdir(save_dir)
         if save_prefix:
             if index:
-                save_file = os.path.join(save_dir, save_prefix + '_' + str(index) + '.jpg')
+                save_file = os.path.join(
+                    save_dir, save_prefix + "_" + str(index) + ".jpg"
+                )
             else:
-                file_name = ''.join(random.sample('AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789', 16))
-                save_file = os.path.join(save_dir, save_prefix + '_' + file_name + '.jpg')
+                file_name = "".join(
+                    random.sample(
+                        "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789",
+                        16,
+                    )
+                )
+                save_file = os.path.join(
+                    save_dir, save_prefix + "_" + file_name + ".jpg"
+                )
         else:
             if index:
-                save_file = os.path.join(save_dir, '_' + str(index) + '.jpg')
+                save_file = os.path.join(save_dir, "_" + str(index) + ".jpg")
             else:
-                file_name = ''.join(random.sample('AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789', 16))
-                save_file = os.path.join(save_dir, '_' + file_name + '.jpg')
-        with open(save_file, 'wb') as f:
-            print('-- image saved into {}'.format(os.path.basename(save_file)))
+                file_name = "".join(
+                    random.sample(
+                        "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789",
+                        16,
+                    )
+                )
+                save_file = os.path.join(save_dir, "_" + file_name + ".jpg")
+        with open(save_file, "wb") as f:
+            print("-- image saved into {}".format(os.path.basename(save_file)))
             f.write(image_data)
 
     @staticmethod
     def decode_url(url):
         url = url.replace("_z2C$q", ":")
         url = url.replace("_z&e3B", ".")
         url = url.replace("AzdH3F", "/")
@@ -64,36 +77,56 @@
         out_table = "abcdefghijklmnopqrstuvw1234567890"
         trans_table = str.maketrans(in_table, out_table)
         url = url.translate(trans_table)
         return url
 
     def scrap(self, query_words, save_dir=None, max_count=5000):
         print(Fore.BLUE)
-        print('-- scrap images of: ' + Fore.YELLOW + Style.BRIGHT + ' '.join(query_words) + Style.RESET_ALL)
+        print(
+            "-- scrap images of: "
+            + Fore.YELLOW
+            + Style.BRIGHT
+            + " ".join(query_words)
+            + Style.RESET_ALL
+        )
         if save_dir:
             root_path = save_dir
         else:
             root_path = os.getcwd()
         for k, query_word in enumerate(query_words):
-            url_pattern = "https://image.baidu.com/search/acjson?tn=resultjson_com&ipn=rj&" \
-                          "ct=201326592&fp=result&queryWord={word}&cl=2&lm=-1&ie=utf-8&oe=utf-8&st=-1&ic=0" \
-                          "&word={word}&face=0&istype=2nc=1&pn={pn}&rn=60"
-            urls = (url_pattern.format(word=query_word, pn=p) for p in range(0, max_count, 30))
+            url_pattern = (
+                "https://image.baidu.com/search/acjson?tn=resultjson_com&ipn=rj&"
+                "ct=201326592&fp=result&queryWord={word}&cl=2&lm=-1&ie=utf-8&oe=utf-8&st=-1&ic=0"
+                "&word={word}&face=0&istype=2nc=1&pn={pn}&rn=60"
+            )
+            urls = (
+                url_pattern.format(word=query_word, pn=p)
+                for p in range(0, max_count, 30)
+            )
             for i_u, url in enumerate(urls):
                 try:
                     html = requests.get(url).text
                     image_urls = re.findall('"objURL":"(.*?)",', html, re.S)
                     for i, image_url in enumerate(image_urls):
                         try:
                             image_url = self.decode_url(image_url)
-                            print('-- decoding url.. : {}'.format(image_url))
-                            print('-- solving %d image' % i)
-                            image = requests.get(image_url, stream=False, timeout=10).content
-                            save_dir = os.path.join(os.path.abspath(root_path), query_words[k])
-                            self.save_image(image, query_word.replace(' ', ''), save_dir, str(i_u) + str(i))
+                            print("-- decoding url.. : {}".format(image_url))
+                            print("-- solving %d image" % i)
+                            image = requests.get(
+                                image_url, stream=False, timeout=10
+                            ).content
+                            save_dir = os.path.join(
+                                os.path.abspath(root_path), query_words[k]
+                            )
+                            self.save_image(
+                                image,
+                                query_word.replace(" ", ""),
+                                save_dir,
+                                str(i_u) + str(i),
+                            )
                         except requests.exceptions.ConnectionError:
-                            print('-- url: %s can not found image.' % image_url)
+                            print("-- url: %s can not found image." % image_url)
                             continue
                 except Exception as e:
                     print(e)
-                    print('-- pass this url.')
-                    pass
+                    print("-- pass this url.")
+                    pass
```

### Comparing `alfred-py-3.0.6/alfred/modules/scrap/scraper_images.py` & `alfred-py-3.0.7/alfred/modules/scrap/scraper_images.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,26 +37,34 @@
 
 
 def save_image(image_data, save_prefix, save_dir, index):
     if not os.path.exists(save_dir):
         os.mkdir(save_dir)
     if save_prefix:
         if index:
-            save_file = os.path.join(save_dir, save_prefix + '_' + str(index) + '.jpg')
+            save_file = os.path.join(save_dir, save_prefix + "_" + str(index) + ".jpg")
         else:
-            file_name = ''.join(random.sample('AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789', 16))
-            save_file = os.path.join(save_dir, save_prefix + '_' + file_name + '.jpg')
+            file_name = "".join(
+                random.sample(
+                    "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789", 16
+                )
+            )
+            save_file = os.path.join(save_dir, save_prefix + "_" + file_name + ".jpg")
     else:
         if index:
-            save_file = os.path.join(save_dir, '_' + str(index) + '.jpg')
+            save_file = os.path.join(save_dir, "_" + str(index) + ".jpg")
         else:
-            file_name = ''.join(random.sample('AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789', 16))
-            save_file = os.path.join(save_dir, '_' + file_name + '.jpg')
-    with open(save_file, 'wb') as f:
-        print('\n--- image saved into {}'.format(os.path.basename(save_file)))
+            file_name = "".join(
+                random.sample(
+                    "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz0123456789", 16
+                )
+            )
+            save_file = os.path.join(save_dir, "_" + file_name + ".jpg")
+    with open(save_file, "wb") as f:
+        print("\n--- image saved into {}".format(os.path.basename(save_file)))
         f.write(image_data)
 
 
 def decode_url(url):
     url = url.replace("_z2C$q", ":")
     url = url.replace("_z&e3B", ".")
     url = url.replace("AzdH3F", "/")
@@ -67,59 +75,73 @@
     return url
 
 
 def get_images_and_save(query_words, root_path, max_number):
     print(query_words)
     print(root_path)
     for k, query_word in enumerate(query_words):
-        url_pattern = "https://image.baidu.com/search/acjson?tn=resultjson_com&ipn=rj&" \
-                      "ct=201326592&fp=result&queryWord={word}&cl=2&lm=-1&ie=utf-8&oe=utf-8&st=-1&ic=0" \
-                      "&word={word}&face=0&istype=2nc=1&pn={pn}&rn=60"
-        urls = (url_pattern.format(word=query_word, pn=p) for p in range(0, max_number, 30))
+        url_pattern = (
+            "https://image.baidu.com/search/acjson?tn=resultjson_com&ipn=rj&"
+            "ct=201326592&fp=result&queryWord={word}&cl=2&lm=-1&ie=utf-8&oe=utf-8&st=-1&ic=0"
+            "&word={word}&face=0&istype=2nc=1&pn={pn}&rn=60"
+        )
+        urls = (
+            url_pattern.format(word=query_word, pn=p) for p in range(0, max_number, 30)
+        )
         for i_u, url in enumerate(urls):
             try:
                 print(url)
                 html = requests.get(url).text
                 image_urls = re.findall('"objURL":"(.*?)",', html, re.S)
                 for i, image_url in enumerate(image_urls):
                     try:
-                        print('[INFO] decoding url..')
+                        print("[INFO] decoding url..")
                         image_url = decode_url(image_url)
                         print(image_url)
-                        print('[INFO] solving %d image' % i)
-                        image = requests.get(image_url, stream=False, timeout=10).content
-                        save_dir = os.path.join(os.path.abspath(root_path), query_words[k])
-                        save_image(image, query_word.replace(' ', ''), save_dir, str(i_u)+str(i))
+                        print("[INFO] solving %d image" % i)
+                        image = requests.get(
+                            image_url, stream=False, timeout=10
+                        ).content
+                        save_dir = os.path.join(
+                            os.path.abspath(root_path), query_words[k]
+                        )
+                        save_image(
+                            image,
+                            query_word.replace(" ", ""),
+                            save_dir,
+                            str(i_u) + str(i),
+                        )
                     except requests.exceptions.ConnectionError:
-                        print('[INFO] url: %s can not found image.' % image_url)
+                        print("[INFO] url: %s can not found image." % image_url)
                         continue
             except Exception as e:
                 print(e)
-                print('[ERROR] pass this url.')
+                print("[ERROR] pass this url.")
                 pass
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description='scraper images, scrap any image from Baidu.')
+    parser = argparse.ArgumentParser(
+        description="scraper images, scrap any image from Baidu."
+    )
 
-    help_ = 'set your query words in a list'
-    parser.add_argument('-q', '--query', nargs='+', help=help_)
+    help_ = "set your query words in a list"
+    parser.add_argument("-q", "--query", nargs="+", help=help_)
 
-    help_ = 'set save root dir'
-    parser.add_argument('-d', '--dir', default='./', help=help_)
+    help_ = "set save root dir"
+    parser.add_argument("-d", "--dir", default="./", help=help_)
 
-    help_ = 'max download image number, default is 80000'
-    parser.add_argument('-m', '--max', type=int, default=80000, help=help_)
+    help_ = "max download image number, default is 80000"
+    parser.add_argument("-m", "--max", type=int, default=80000, help=help_)
 
     args_ = parser.parse_args()
     return args_
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     args = parse_args()
     queries = args.query
     save_root_dir = args.dir
     max_num = args.max
     if not os.path.exists(os.path.abspath(save_root_dir)):
         os.mkdir(os.path.abspath(save_root_dir))
     get_images_and_save(queries, save_root_dir, max_num)
-
```

### Comparing `alfred-py-3.0.6/alfred/modules/text/__init__.py` & `alfred-py-3.0.7/alfred/modules/text/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/vision/__init__.py` & `alfred-py-3.0.7/alfred/modules/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/modules/vision/face_extractor.py` & `alfred-py-3.0.7/alfred/modules/vision/face_extractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,58 +22,61 @@
 # under the License.
 #
 """
 This file using for extracting faces of all images
 
 """
 import glob
+
 try:
     import dlib
 except ImportError:
-    print('You have not installed dlib, install from https://github.com/davisking/dlib')
-    print('see you later.')
+    print("You have not installed dlib, install from https://github.com/davisking/dlib")
+    print("see you later.")
     exit(0)
 import os
 import cv2
 import numpy as np
 from loguru import logger
 
 
 class FaceExtractor(object):
-
-    def __init__(self, predictor_path='shape_predictor_68_face_landmarks.dat'):
+    def __init__(self, predictor_path="shape_predictor_68_face_landmarks.dat"):
         self.detector = dlib.get_frontal_face_detector()
         self.predictor_path = predictor_path
         self.predictor = dlib.shape_predictor(predictor_path)
 
-
     def get_faces_list(self, img, landmark=False):
         """
         get faces and locations
         """
-        assert isinstance(img, np.ndarray), 'img should be numpy array (cv2 frame)'
+        assert isinstance(img, np.ndarray), "img should be numpy array (cv2 frame)"
         if landmark:
             if os.path.exists(self.predictor_path):
                 predictor = dlib.shape_predictor(self.predictor_path)
             else:
-                logger.error('Could not found model file {}, you should download '
-                'dlib landmark model: http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2'.format(self.predictor_path))
+                logger.error(
+                    "Could not found model file {}, you should download "
+                    "dlib landmark model: http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2".format(
+                        self.predictor_path
+                    )
+                )
                 exit(0)
         dets = self.detector(img, 1)
         all_faces = []
         locations = []
         landmarks = []
         for i, d in enumerate(dets):
             # get the face crop
             x = int(d.left())
             y = int(d.top())
             w = int(d.width())
             h = int(d.height())
 
-            face_patch = np.array(img)[y: y + h, x: x + w, 0:3]
+            face_patch = np.array(img)[y : y + h, x : x + w, 0:3]
 
             if landmark:
                 shape = predictor(img, d)
                 landmarks.append(shape)
             locations.append([x, y, w, h])
             all_faces.append(face_patch)
         if landmark:
@@ -85,40 +88,41 @@
         """
         get all faces from img_d
         :param img_d:
         :return:
         """
 
         all_images = []
-        for e in ['png', 'jpg', 'jpeg']:
-            all_images.extend(glob.glob(os.path.join(img_d, '*.{}'.format(e))))
-        print('Found all {} images under {}'.format(len(all_images), img_d))
+        for e in ["png", "jpg", "jpeg"]:
+            all_images.extend(glob.glob(os.path.join(img_d, "*.{}".format(e))))
+        print("Found all {} images under {}".format(len(all_images), img_d))
 
         s_d = os.path.dirname(img_d) + "_faces"
         if not os.path.exists(s_d):
             os.makedirs(s_d)
         for img_f in all_images:
             img = cv2.imread(img_f, cv2.COLOR_BGR2RGB)
 
             dets = self.detector(img, 1)
-            print('=> get {} faces in {}'.format(len(dets), img_f))
-            print('=> saving faces...')
+            print("=> get {} faces in {}".format(len(dets), img_f))
+            print("=> saving faces...")
             for i, d in enumerate(dets):
-                save_face_f = os.path.join(s_d, os.path.basename(img_f).split('.')[0]
-                                           + '_face_{}.png'.format(i))
+                save_face_f = os.path.join(
+                    s_d,
+                    os.path.basename(img_f).split(".")[0] + "_face_{}.png".format(i),
+                )
 
                 # get the face crop
                 x = int(d.left())
                 y = int(d.top())
                 w = int(d.width())
                 h = int(d.height())
 
-                face_patch = np.array(img)[y: y + h, x: x + w, 0:3]
+                face_patch = np.array(img)[y : y + h, x : x + w, 0:3]
                 # print(face_patch.shape)
                 img = cv2.rectangle(img, (x, y), (x + w, y + h), (0, 0, 255), 2)
 
                 # cv2.imshow('tt', img)
                 # cv2.waitKey(0)
                 cv2.imwrite(save_face_f, face_patch)
-        print('Done!')
+        print("Done!")
         # cv2.waitKey(0)
-
```

### Comparing `alfred-py-3.0.6/alfred/modules/vision/to_video.py` & `alfred-py-3.0.7/alfred/modules/vision/to_video.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,50 +38,58 @@
 
 
 class VideoCombiner(object):
     def __init__(self, img_dir):
         self.img_dir = img_dir
 
         if not os.path.exists(self.img_dir):
-            print(Fore.RED + '=> Error: ' + '{} not exist.'.format(self.img_dir))
+            print(Fore.RED + "=> Error: " + "{} not exist.".format(self.img_dir))
             exit(0)
 
         self._get_video_shape()
 
     def _get_video_shape(self):
-        self.all_images = [os.path.join(self.img_dir, i) for i in os.listdir(self.img_dir)]
+        self.all_images = [
+            os.path.join(self.img_dir, i) for i in os.listdir(self.img_dir)
+        ]
 
         # this sorted method seems has problem
         # self.all_images.sort(key=lambda f: int(''.join(filter(str.isdigit, f))))
         self.all_images = natsorted(self.all_images)
-        for item in self.all_images[:int(len(self.all_images) // 3)]:
+        for item in self.all_images[: int(len(self.all_images) // 3)]:
             print(item)
         # order the images order.
 
         sample_img = np.random.choice(self.all_images)
         if os.path.exists(sample_img):
             img = cv2.imread(sample_img)
             self.video_shape = img.shape
         else:
-            print(Fore.RED + '=> Error: ' + '{} not found or open failed, try again.'.format(sample_img))
+            print(
+                Fore.RED
+                + "=> Error: "
+                + "{} not found or open failed, try again.".format(sample_img)
+            )
             exit(0)
 
-    def combine(self, target_file='combined.mp4'):
+    def combine(self, target_file="combined.mp4"):
         size = (self.video_shape[1], self.video_shape[0])
-        print('=> target video frame size: ', size)
-        print('=> all {} frames to solve.'.format(len(self.all_images)))
-        target_f = 'combined_{}.mp4'.format(os.path.basename(self.img_dir))
-        video_writer = cv2.VideoWriter(target_f, cv2.VideoWriter_fourcc(*'DIVX'), 26, size)
+        print("=> target video frame size: ", size)
+        print("=> all {} frames to solve.".format(len(self.all_images)))
+        target_f = "combined_{}.mp4".format(os.path.basename(self.img_dir))
+        video_writer = cv2.VideoWriter(
+            target_f, cv2.VideoWriter_fourcc(*"DIVX"), 26, size
+        )
         i = 0
-        print('=> Solving, be patient.')
+        print("=> Solving, be patient.")
         for img in self.all_images:
             img = cv2.imread(img, cv2.COLOR_BGR2RGB)
             i += 1
             # print('=> Solving: ', i)
             video_writer.write(img)
         video_writer.release()
-        print('Done!')
+        print("Done!")
 
 
 # d = sys.argv[1]
 # combiner = VideoCombiner(d)
-# combiner.combine()
+# combiner.combine()
```

### Comparing `alfred-py-3.0.6/alfred/modules/vision/video_extractor.py` & `alfred-py-3.0.7/alfred/modules/vision/video_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import os
 import sys
+
 try:
     import cv2
 except ImportError:
-    print('you are not install opencv-python, using pip install opencv-python install it.')
+    print(
+        "you are not install opencv-python, using pip install opencv-python install it."
+    )
 from colorama import Fore, Back, Style
 
 
 class VideoExtractor(object):
-
-    def __init__(self, jump_frames=6, save_format='frame_%06d.jpg'):
+    def __init__(self, jump_frames=6, save_format="frame_%06d.jpg"):
         """
         we set frames to jump, etc, using jump_frames=6
         will save one frame per 6 frames jumped
         :param jump_frames:
         :param save_format: this is the frames save format
         users can decide what's the format is: frame_0000004.jpg
         """
@@ -48,27 +50,39 @@
         else:
             self.jump_frames = 6
         self.save_format = save_format
 
     def extract(self, video_f):
         if os.path.exists(video_f) and os.path.isfile(video_f):
             cap = cv2.VideoCapture(video_f)
-            f_n = os.path.basename(video_f).split('.')[0]
+            f_n = os.path.basename(video_f).split(".")[0]
 
-            save_dir = os.path.join(os.path.dirname(video_f), os.path.basename(video_f).split('.')[0])
+            save_dir = os.path.join(
+                os.path.dirname(video_f), os.path.basename(video_f).split(".")[0]
+            )
             if not os.path.exists(save_dir):
                 os.makedirs(save_dir)
 
             res = True
             while res:
                 res, image = cap.read()
                 self.current_frame += 1
                 if self.current_frame % self.jump_frames == 0:
-                    print('Read frame: {} jump frames: {}'.format(self.current_frame, self.jump_frames))
-                    cv2.imwrite(os.path.join(save_dir, f_n + '_' + self.save_format % self.current_save_frame), image)
+                    print(
+                        "Read frame: {} jump frames: {}".format(
+                            self.current_frame, self.jump_frames
+                        )
+                    )
+                    cv2.imwrite(
+                        os.path.join(
+                            save_dir,
+                            f_n + "_" + self.save_format % self.current_save_frame,
+                        ),
+                        image,
+                    )
                     self.current_save_frame += 1
 
             print(Fore.GREEN + Style.BRIGHT)
-            print('Success!')
+            print("Success!")
         else:
             print(Fore.RED + Style.BRIGHT)
-            print('Error! ' + Style.RESET_ALL + '{} not exist.'.format(video_f))
+            print("Error! " + Style.RESET_ALL + "{} not exist.".format(video_f))
```

### Comparing `alfred-py-3.0.6/alfred/modules/vision/video_reducer.py` & `alfred-py-3.0.7/alfred/modules/vision/video_reducer.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import sys
 import cv2
 from colorama import Fore, Back, Style
 from alfred.utils.log import logger as logging
 
 
 class VideoReducer(object):
-
     def __init__(self, jump_frames=6):
         """
         we set frames to jump, etc, using jump_frames=6
         will save one frame per 6 frames jumped
         :param jump_frames:
         :param save_format: this is the frames save format
         users can decide what's the format is: frame_0000004.jpg
@@ -44,30 +43,43 @@
         if jump_frames:
             self.jump_frames = int(jump_frames)
         else:
             self.jump_frames = 6
 
     def act(self, video_f):
         """
-        reduce the video frame by drop frames 
-        
+        reduce the video frame by drop frames
+
         """
         if os.path.exists(video_f) and os.path.isfile(video_f):
-            logging.info('start to reduce file: {}'.format(video_f))
+            logging.info("start to reduce file: {}".format(video_f))
             cap = cv2.VideoCapture(video_f)
-            target_f = os.path.join(os.path.dirname(video_f), os.path.basename(video_f).split('.')[0] + '_reduced.mp4')
+            target_f = os.path.join(
+                os.path.dirname(video_f),
+                os.path.basename(video_f).split(".")[0] + "_reduced.mp4",
+            )
             size = (int(cap.get(3)), int(cap.get(4)))
-            logging.info('video size: {}, will support reduce size in the future.'.format(size))
-            video_writer = cv2.VideoWriter(target_f, cv2.VideoWriter_fourcc(*'DIVX'), 24, size)
+            logging.info(
+                "video size: {}, will support reduce size in the future.".format(size)
+            )
+            video_writer = cv2.VideoWriter(
+                target_f, cv2.VideoWriter_fourcc(*"DIVX"), 24, size
+            )
             res = True
             while res:
                 res, image = cap.read()
                 self.current_frame += 1
-                if (self.current_frame % self.jump_frames == 0) or self.current_frame < 15:
-                    print('Read frame: {} jump frames: {}'.format(self.current_frame, self.jump_frames))
+                if (
+                    self.current_frame % self.jump_frames == 0
+                ) or self.current_frame < 15:
+                    print(
+                        "Read frame: {} jump frames: {}".format(
+                            self.current_frame, self.jump_frames
+                        )
+                    )
                     self.current_save_frame += 1
                     video_writer.write(image)
             video_writer.release()
-            logging.info('reduced video file has been saved into: {}'.format(target_f))
+            logging.info("reduced video file has been saved into: {}".format(target_f))
         else:
             print(Fore.RED + Style.BRIGHT)
-            print('Error! ' + Style.RESET_ALL + '{} not exist.'.format(video_f))
+            print("Error! " + Style.RESET_ALL + "{} not exist.".format(video_f))
```

### Comparing `alfred-py-3.0.6/alfred/modules/vision/vis_kit.py` & `alfred-py-3.0.7/alfred/modules/vision/vis_kit.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 import matplotlib.patheffects as patheffects
 
 
 def draw_box_without_score(img, boxes, classes=None, is_show=False):
     """
     Draw boxes on image, the box mostly are annotations, not the model predict box
     """
-    assert isinstance(boxes,
-                      np.ndarray), 'boxes must nump array, with shape of (None, 5)\nevery element contains (x1,y1,x2,y2, label)'
+    assert isinstance(
+        boxes, np.ndarray
+    ), "boxes must nump array, with shape of (None, 5)\nevery element contains (x1,y1,x2,y2, label)"
     if classes:
         pass
     else:
         height = img.shape[0]
         width = img.shape[1]
 
         font = cv2.QT_FONT_NORMAL
@@ -63,46 +64,71 @@
             y1 = int(boxes[i, 2])
             x1 = int(boxes[i, 3])
             y2 = int(boxes[i, 4])
             x2 = int(boxes[i, 5])
 
             cv2.rectangle(img, (x1, y1), (x2, y2), unique_color, line_thickness)
 
-            text_label = '{}'.format(cls)
-            (ret_val, base_line) = cv2.getTextSize(text_label, font, font_scale, font_thickness)
+            text_label = "{}".format(cls)
+            (ret_val, base_line) = cv2.getTextSize(
+                text_label, font, font_scale, font_thickness
+            )
             text_org = (x1, y1 - 0)
 
-            cv2.rectangle(img, (text_org[0] - 5, text_org[1] + base_line + 2),
-                          (text_org[0] + ret_val[0] + 5, text_org[1] - ret_val[1] - 2), unique_color, line_thickness)
+            cv2.rectangle(
+                img,
+                (text_org[0] - 5, text_org[1] + base_line + 2),
+                (text_org[0] + ret_val[0] + 5, text_org[1] - ret_val[1] - 2),
+                unique_color,
+                line_thickness,
+            )
             # this rectangle for fill text rect
-            cv2.rectangle(img, (text_org[0] - 5, text_org[1] + base_line + 2),
-                          (text_org[0] + ret_val[0] + 4, text_org[1] - ret_val[1] - 2),
-                          unique_color, -1)
-            cv2.putText(img, text_label, text_org, font, font_scale, (255, 255, 255), font_thickness)
+            cv2.rectangle(
+                img,
+                (text_org[0] - 5, text_org[1] + base_line + 2),
+                (text_org[0] + ret_val[0] + 4, text_org[1] - ret_val[1] - 2),
+                unique_color,
+                -1,
+            )
+            cv2.putText(
+                img,
+                text_label,
+                text_org,
+                font,
+                font_scale,
+                (255, 255, 255),
+                font_thickness,
+            )
         if is_show:
-            cv2.imshow('image', img)
+            cv2.imshow("image", img)
             cv2.waitKey(0)
         return img
 
 
-def visualize_det_cv2(img, detections, classes=None, thresh=0.6, is_show=False, background_id=-1):
+def visualize_det_cv2(
+    img, detections, classes=None, thresh=0.6, is_show=False, background_id=-1
+):
     """
     visualize detection on image using cv2, this is the standard way to visualize detections
     :param img:
     :param detections: ssd detections, numpy.array([[id, score, x1, y1, x2, y2]...])
             each row is one object
     :param classes:
     :param thresh:
     :param is_show:
     :param background_id: -1
     :return:
     """
-    assert classes, 'from visualize_det_cv2, classes must be provided, each class in a list with' \
-                    'certain order.'
-    assert isinstance(img, np.ndarray), 'from visualize_det_cv2, img must be a numpy array object.'
+    assert classes, (
+        "from visualize_det_cv2, classes must be provided, each class in a list with"
+        "certain order."
+    )
+    assert isinstance(
+        img, np.ndarray
+    ), "from visualize_det_cv2, img must be a numpy array object."
 
     height = img.shape[0]
     width = img.shape[1]
 
     font = cv2.QT_FONT_NORMAL
     font_scale = 0.4
     font_thickness = 1
@@ -124,73 +150,112 @@
                 y1 = int(detections[i, 2])
                 x1 = int(detections[i, 3])
                 y2 = int(detections[i, 4])
                 x2 = int(detections[i, 5])
 
                 cv2.rectangle(img, (x1, y1), (x2, y2), unique_color, line_thickness)
 
-                text_label = '{} {:.2f}'.format(classes[cls_id], score)
-                (ret_val, base_line) = cv2.getTextSize(text_label, font, font_scale, font_thickness)
+                text_label = "{} {:.2f}".format(classes[cls_id], score)
+                (ret_val, base_line) = cv2.getTextSize(
+                    text_label, font, font_scale, font_thickness
+                )
                 text_org = (x1, y1 - 0)
 
-                cv2.rectangle(img, (text_org[0] - 5, text_org[1] + base_line + 2),
-                              (text_org[0] + ret_val[0] + 5, text_org[1] - ret_val[1] - 2), unique_color,
-                              line_thickness)
+                cv2.rectangle(
+                    img,
+                    (text_org[0] - 5, text_org[1] + base_line + 2),
+                    (text_org[0] + ret_val[0] + 5, text_org[1] - ret_val[1] - 2),
+                    unique_color,
+                    line_thickness,
+                )
                 # this rectangle for fill text rect
-                cv2.rectangle(img, (text_org[0] - 5, text_org[1] + base_line + 2),
-                              (text_org[0] + ret_val[0] + 4, text_org[1] - ret_val[1] - 2),
-                              unique_color, -1)
-                cv2.putText(img, text_label, text_org, font, font_scale, (255, 255, 255), font_thickness)
+                cv2.rectangle(
+                    img,
+                    (text_org[0] - 5, text_org[1] + base_line + 2),
+                    (text_org[0] + ret_val[0] + 4, text_org[1] - ret_val[1] - 2),
+                    unique_color,
+                    -1,
+                )
+                cv2.putText(
+                    img,
+                    text_label,
+                    text_org,
+                    font,
+                    font_scale,
+                    (255, 255, 255),
+                    font_thickness,
+                )
     if is_show:
-        cv2.imshow('image', img)
+        cv2.imshow("image", img)
         cv2.waitKey(0)
     return img
 
 
-def visualize_det_mask_cv2(img, detections, masks, classes=None, is_show=False, background_id=-1, is_video=False):
+def visualize_det_mask_cv2(
+    img,
+    detections,
+    masks,
+    classes=None,
+    is_show=False,
+    background_id=-1,
+    is_video=False,
+):
     """
     this method using for display detections and masks on image
     :param img:
     :param detections: numpy.array([[id, score, x1, y1, x2, y2]...])
             each row is one object. contains id and score in the first 2 rows
     :param masks: numpy.array([[mask_width, mask_height], ...], every element is an
     one chanel mask of on object
     :param classes: classes names in a list with certain order
     :param is_show: to show if it is video
     :param background_id
     :param is_video
     :return:
     """
-    assert isinstance(img, np.ndarray) and isinstance(detections, np.ndarray) and isinstance(masks, np.ndarray), \
-        'images and detections and masks must be numpy array'
-    assert detections.shape[0] == masks.shape[-1], 'detections nums and masks nums are not equal'
-    assert is_show != is_video, 'you can not set is_show and is_video at the same time.'
+    assert (
+        isinstance(img, np.ndarray)
+        and isinstance(detections, np.ndarray)
+        and isinstance(masks, np.ndarray)
+    ), "images and detections and masks must be numpy array"
+    assert (
+        detections.shape[0] == masks.shape[-1]
+    ), "detections nums and masks nums are not equal"
+    assert is_show != is_video, "you can not set is_show and is_video at the same time."
     # draw detections first
     img = visualize_det_cv2(img, detections, classes=classes, is_show=False)
 
     masked_image = img
-    print('masked image shape: ', masked_image.shape)
+    print("masked image shape: ", masked_image.shape)
     num_instances = detections.shape[0]
     for i in range(num_instances):
         cls_id = int(detections[i, 0])
         if cls_id != background_id:
             unique_color = _create_unique_color_uchar(cls_id)
             mask = masks[:, :, i]
             masked_image = _apply_mask2(masked_image, mask, unique_color)
     # masked_image = masked_image.astype(int)
     if is_video:
-        cv2.imshow('image', masked_image)
+        cv2.imshow("image", masked_image)
         cv2.waitKey(1)
     elif is_show:
-        cv2.imshow('image', masked_image)
+        cv2.imshow("image", masked_image)
         cv2.waitKey(0)
     return masked_image
 
 
-def draw_masks(img, masks, cls_color_list, is_show=False, background_id=-1, is_video=False, convert_bgr=False):
+def draw_masks(
+    img,
+    masks,
+    cls_color_list,
+    is_show=False,
+    background_id=-1,
+    is_video=False,
+    convert_bgr=False,
+):
     """
     draw masks pure on an image, the mask format is something like this:
     [[[1], [1], [1], .., [2]],
      [[1], [1], [1], .., [2]],
      [[1], [1], [1], .., [2]]]
     every pixel in image is a class
 
@@ -207,41 +272,41 @@
     :return:
     """
     n, h, w, c = masks.shape
 
     mask_flatten = masks[0].flatten()
     mask_color = np.array(list(map(lambda i: cls_color_list[i], mask_flatten)))
     # reshape to normal image shape,
-    mask_color = np.reshape(mask_color, (h, w, 3)).astype('float32')
+    mask_color = np.reshape(mask_color, (h, w, 3)).astype("float32")
 
     # add this mask on img
     # img = cv2.add(img, mask_color)
     if convert_bgr:
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
     img = cv2.addWeighted(img, 0.6, mask_color, 0.4, 0)
     if is_show:
-        cv2.imshow('img', img)
-        cv2.imwrite('test_res.jpg', img)
+        cv2.imshow("img", img)
+        cv2.imwrite("test_res.jpg", img)
         cv2.waitKey(0)
     return img
 
 
 def _apply_mask2(image, mask, color, alpha=0.5):
     for c in range(3):
-        image[:, :, c] = np.where(mask == 1, image[:, :, c] * (1 - alpha) + alpha * color[c],
-                                  image[:, :, c])
+        image[:, :, c] = np.where(
+            mask == 1, image[:, :, c] * (1 - alpha) + alpha * color[c], image[:, :, c]
+        )
     return image
 
 
 def create_unique_color_float(tag, hue_step=0.41, alpha=0.7):
-    h, v = (tag * hue_step) % 1, 1. - (int(tag * hue_step) % 4) / 5.
-    r, g, b = colorsys.hsv_to_rgb(h, 1., v)
+    h, v = (tag * hue_step) % 1, 1.0 - (int(tag * hue_step) % 4) / 5.0
+    r, g, b = colorsys.hsv_to_rgb(h, 1.0, v)
     return r, g, b, alpha
 
 
 def create_unique_color_uchar(tag, hue_step=0.41, alpha=0.7):
     r, g, b, a = create_unique_color_float(tag, hue_step, alpha)
     return int(255 * r), int(255 * g), int(255 * b), int(255 * a)
 
 
 # ----------------------- 3D drawing functionality ----------------------
-
```

### Comparing `alfred-py-3.0.6/alfred/protos/labelmap_pb2.py` & `alfred-py-3.0.7/alfred/protos/labelmap_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,133 +22,190 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: labelmap.proto
 
 import sys
-_b=sys.version_info[0]<3 and (lambda x:x) or (lambda x:x.encode('latin1'))
+
+_b = sys.version_info[0] < 3 and (lambda x: x) or (lambda x: x.encode("latin1"))
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='labelmap.proto',
-  package='',
-  syntax='proto2',
-  serialized_options=None,
-  serialized_pb=_b('\n\x0elabelmap.proto\"M\n\x0cLabelMapItem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\x05\x12\n\n\x02id\x18\x04 \x01(\x05\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t\"\'\n\x08LabelMap\x12\x1b\n\x04item\x18\x01 \x03(\x0b\x32\r.LabelMapItem')
+    name="labelmap.proto",
+    package="",
+    syntax="proto2",
+    serialized_options=None,
+    serialized_pb=_b(
+        '\n\x0elabelmap.proto"M\n\x0cLabelMapItem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\x05\x12\n\n\x02id\x18\x04 \x01(\x05\x12\x14\n\x0c\x64isplay_name\x18\x03 \x01(\t"\'\n\x08LabelMap\x12\x1b\n\x04item\x18\x01 \x03(\x0b\x32\r.LabelMapItem'
+    ),
 )
 
 
-
-
 _LABELMAPITEM = _descriptor.Descriptor(
-  name='LabelMapItem',
-  full_name='LabelMapItem',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='name', full_name='LabelMapItem.name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='label', full_name='LabelMapItem.label', index=1,
-      number=2, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='id', full_name='LabelMapItem.id', index=2,
-      number=4, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='display_name', full_name='LabelMapItem.display_name', index=3,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=18,
-  serialized_end=95,
+    name="LabelMapItem",
+    full_name="LabelMapItem",
+    filename=None,
+    file=DESCRIPTOR,
+    containing_type=None,
+    fields=[
+        _descriptor.FieldDescriptor(
+            name="name",
+            full_name="LabelMapItem.name",
+            index=0,
+            number=1,
+            type=9,
+            cpp_type=9,
+            label=1,
+            has_default_value=False,
+            default_value=_b("").decode("utf-8"),
+            message_type=None,
+            enum_type=None,
+            containing_type=None,
+            is_extension=False,
+            extension_scope=None,
+            serialized_options=None,
+            file=DESCRIPTOR,
+        ),
+        _descriptor.FieldDescriptor(
+            name="label",
+            full_name="LabelMapItem.label",
+            index=1,
+            number=2,
+            type=5,
+            cpp_type=1,
+            label=1,
+            has_default_value=False,
+            default_value=0,
+            message_type=None,
+            enum_type=None,
+            containing_type=None,
+            is_extension=False,
+            extension_scope=None,
+            serialized_options=None,
+            file=DESCRIPTOR,
+        ),
+        _descriptor.FieldDescriptor(
+            name="id",
+            full_name="LabelMapItem.id",
+            index=2,
+            number=4,
+            type=5,
+            cpp_type=1,
+            label=1,
+            has_default_value=False,
+            default_value=0,
+            message_type=None,
+            enum_type=None,
+            containing_type=None,
+            is_extension=False,
+            extension_scope=None,
+            serialized_options=None,
+            file=DESCRIPTOR,
+        ),
+        _descriptor.FieldDescriptor(
+            name="display_name",
+            full_name="LabelMapItem.display_name",
+            index=3,
+            number=3,
+            type=9,
+            cpp_type=9,
+            label=1,
+            has_default_value=False,
+            default_value=_b("").decode("utf-8"),
+            message_type=None,
+            enum_type=None,
+            containing_type=None,
+            is_extension=False,
+            extension_scope=None,
+            serialized_options=None,
+            file=DESCRIPTOR,
+        ),
+    ],
+    extensions=[],
+    nested_types=[],
+    enum_types=[],
+    serialized_options=None,
+    is_extendable=False,
+    syntax="proto2",
+    extension_ranges=[],
+    oneofs=[],
+    serialized_start=18,
+    serialized_end=95,
 )
 
 
 _LABELMAP = _descriptor.Descriptor(
-  name='LabelMap',
-  full_name='LabelMap',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='item', full_name='LabelMap.item', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=97,
-  serialized_end=136,
+    name="LabelMap",
+    full_name="LabelMap",
+    filename=None,
+    file=DESCRIPTOR,
+    containing_type=None,
+    fields=[
+        _descriptor.FieldDescriptor(
+            name="item",
+            full_name="LabelMap.item",
+            index=0,
+            number=1,
+            type=11,
+            cpp_type=10,
+            label=3,
+            has_default_value=False,
+            default_value=[],
+            message_type=None,
+            enum_type=None,
+            containing_type=None,
+            is_extension=False,
+            extension_scope=None,
+            serialized_options=None,
+            file=DESCRIPTOR,
+        ),
+    ],
+    extensions=[],
+    nested_types=[],
+    enum_types=[],
+    serialized_options=None,
+    is_extendable=False,
+    syntax="proto2",
+    extension_ranges=[],
+    oneofs=[],
+    serialized_start=97,
+    serialized_end=136,
 )
 
-_LABELMAP.fields_by_name['item'].message_type = _LABELMAPITEM
-DESCRIPTOR.message_types_by_name['LabelMapItem'] = _LABELMAPITEM
-DESCRIPTOR.message_types_by_name['LabelMap'] = _LABELMAP
+_LABELMAP.fields_by_name["item"].message_type = _LABELMAPITEM
+DESCRIPTOR.message_types_by_name["LabelMapItem"] = _LABELMAPITEM
+DESCRIPTOR.message_types_by_name["LabelMap"] = _LABELMAP
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-LabelMapItem = _reflection.GeneratedProtocolMessageType('LabelMapItem', (_message.Message,), {
-  'DESCRIPTOR' : _LABELMAPITEM,
-  '__module__' : 'labelmap_pb2'
-  # @@protoc_insertion_point(class_scope:LabelMapItem)
-  })
+LabelMapItem = _reflection.GeneratedProtocolMessageType(
+    "LabelMapItem",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _LABELMAPITEM,
+        "__module__": "labelmap_pb2"
+        # @@protoc_insertion_point(class_scope:LabelMapItem)
+    },
+)
 _sym_db.RegisterMessage(LabelMapItem)
 
-LabelMap = _reflection.GeneratedProtocolMessageType('LabelMap', (_message.Message,), {
-  'DESCRIPTOR' : _LABELMAP,
-  '__module__' : 'labelmap_pb2'
-  # @@protoc_insertion_point(class_scope:LabelMap)
-  })
+LabelMap = _reflection.GeneratedProtocolMessageType(
+    "LabelMap",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _LABELMAP,
+        "__module__": "labelmap_pb2"
+        # @@protoc_insertion_point(class_scope:LabelMap)
+    },
+)
 _sym_db.RegisterMessage(LabelMap)
 
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `alfred-py-3.0.6/alfred/siren/handler.py` & `alfred-py-3.0.7/alfred/siren/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,24 +57,22 @@
         if log_level == "info":
             logger.remove(handler_id=None)
 
     def request_uranus_token(self):
         data = {"user_acc": self.user_acc, "user_password": self.user_password}
         # data = {"user_acc": 'jintian', "user_password": '1195889656'}
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
-        rep = requests.post(
-            url=self.uranus_login_url, headers=headers, data=data
-        )
+        rep = requests.post(url=self.uranus_login_url, headers=headers, data=data)
         print(data)
         rep = json.loads(rep.text)
         print(rep)
         if rep["status"] == "error":
             pass
         else:
-            token = rep['data']["token"]
+            token = rep["data"]["token"]
             with open(global_config.token_config_f, "wb") as f:
                 pickle.dump(token, f)
                 logger.info(f"requested uranus token for robot: {token}")
 
     def _connect(self):
         self.client = mqtt_client.Client(self.client_id)
         self.client.username_pw_set(self.user_acc, self.user_password)
```

### Comparing `alfred-py-3.0.6/alfred/siren/models.py` & `alfred-py-3.0.7/alfred/siren/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 """
 
 contains all models used in Siren chatbot API
 
 """
 import json
 import jsons
@@ -45,40 +43,37 @@
 class MessageOriginality:
     Original = "Original"
     Reply = "Reply"
     Forward = "Forward"
 
 
 class PresenceSession:
-
     def __init__(self) -> None:
         self.id = None
         self.user_id = None
         self.presence = None
         self.last_presence = None
 
 
 class BaseMessage:
-
     def __init__(self) -> None:
         self.id = None
         self.type: MessageType = MessageType.ChatText
         self.fromId = None
         self.fromName = None
 
 
 class PresenceMessage(BaseMessage):
-
     def __init__(self) -> None:
         super().__init__()
 
         self.presenceType: PresenceType = PresenceType.Available
 
-class ChatMessage(BaseMessage):
 
+class ChatMessage(BaseMessage):
     def __init__(self) -> None:
         super().__init__()
 
         self.toId = None
         self.toName = None
         self.text = None
         self.attachment = None
@@ -92,73 +87,66 @@
         self.sendTime = None
         self.longitude = None
         self.latitude = None
 
 
 @dataclass
 class Invitation:
-
     def __init__(self) -> None:
         self.id = None
         self.from_id = None
         self.to_id = None
         self.state = None
         self.sent_date = None
 
 
 class Room:
-
     def __init__(self) -> None:
         self.id = None
         self.name = None
         self.avatar = None
         self.is_group = None
 
 
 class RoomMembership:
-
     def __init__(self) -> None:
         self.room_id = None
         self.user_id = None
         self.role = None
 
 
 @dataclass
 class InvitationMessage:
-
     def __init__(self) -> None:
         self.id = None
         self.type: MessageType = MessageType.EventInvitationRequest
         self.invitationMessageType: InvitationMessageType = InvitationMessageType.INFO
         self.text = None
         self.sendTime = None
         self.fromId = None
         self.toId = None
         self.fromName = None
         self.fromAvatar = None
 
 
 @dataclass
 class ContactChat:
-
     def __init__(self) -> None:
         self.firstName = None
         self.lastName = None
         self.id = None
         self.avatar = None
         self.roomId = None
         self.presence: PresenceType = PresenceType.Available
         self.isGroup = None
 
     def toJSON(self):
-        return json.dumps(self, default=lambda o: o.__dict__,
-                          sort_keys=True, indent=4)
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
 
 
 @dataclass
 class User:
-
     def __init__(self) -> None:
         self.user_addr = None
         self.user_acc = None
         self.user_sign = None
         self.user_nick_name = None
```

### Comparing `alfred-py-3.0.6/alfred/siren/topicgen.py` & `alfred-py-3.0.7/alfred/siren/topicgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-
 def get_events_topic(cid):
-    return "events/" + cid;
+    return "events/" + cid
+
 
 def get_presence_topic(cid):
     return "presence/" + cid
 
+
 def get_personal_events_topic(cid):
     return "personalevents/" + cid
 
+
 def get_chatting_topic(cid):
     return "messages/" + cid
 
+
 def get_file_chatting_topic(cid):
     return "filemessages/" + cid
 
+
 def get_archives_rooms_topic(cid):
     return "archivesrooms/" + cid
 
+
 def get_archives_messages_topic(cid):
     return "archivesmessages/" + cid
 
+
 def get_archives_myid_topic(cid):
     return "archivesmyid/" + cid
```

### Comparing `alfred-py-3.0.6/alfred/tests.py` & `alfred-py-3.0.7/alfred/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,31 @@
 import torch
 from dl.torch.common import print_tensor
 
 from varname import varname
 
 
 def a_func(num):
-    print(varname() + ': ' + str(num))
+    print(varname() + ": " + str(num))
 
 
 def clothes(func):
     def wear():
-        print('Buy clothes!{}'.format(func.__name__))
+        print("Buy clothes!{}".format(func.__name__))
         return func()
+
     return wear
 
 
 @clothes
 def body():
-    print('The body feels could!')
+    print("The body feels could!")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     v = a_func(1098)
 
     # welcome('')
     # logging.info('hi hiu')
     # logging.error('ops')
 
     # a = cv2.imread('/home/jintian/Pictures/1.jpeg')
```

### Comparing `alfred-py-3.0.6/alfred/utils/__init__.py` & `alfred-py-3.0.7/alfred/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/utils/base_config.py` & `alfred-py-3.0.7/alfred/utils/base_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-
 import importlib
 from yacs.config import CfgNode as CN
 import argparse
 
 
 class Config:
     @classmethod
     def load_from_args(cls):
         parser = argparse.ArgumentParser()
-        parser.add_argument('--cfg', type=str, default='config/base.yml')
+        parser.add_argument("--cfg", type=str, default="config/base.yml")
         parser.add_argument("opts", default=None, nargs=argparse.REMAINDER)
         args = parser.parse_args()
         return cls.load(filename=args.cfg, opts=args.opts)
 
     @classmethod
     def load(cls, filename=None, opts=[]) -> CN:
         cfg = CN()
@@ -31,19 +30,19 @@
 
     @staticmethod
     def parse(cfg):
         pass
 
     @staticmethod
     def print(cfg):
-        print('[Info] --------------')
-        print('[Info] Configuration:')
-        print('[Info] --------------')
+        print("[Info] --------------")
+        print("[Info] Configuration:")
+        print("[Info] --------------")
         print(cfg)
 
 
 def load_object(module_name, module_args):
-    module_path = '.'.join(module_name.split('.')[:-1])
+    module_path = ".".join(module_name.split(".")[:-1])
     module = importlib.import_module(module_path)
-    name = module_name.split('.')[-1]
+    name = module_name.split(".")[-1]
     obj = getattr(module, name)(**module_args)
     return obj
```

### Comparing `alfred-py-3.0.6/alfred/utils/communicate.py` & `alfred-py-3.0.7/alfred/utils/communicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         self._connect()
 
     def _connect(self):
         if self.is_server:
             self.socket.bind((self.ip, self.port))
             self.socket.listen(3)
             self.conn, addr = self.socket.accept()
-            print('Server is ready. ', addr)
+            print("Server is ready. ", addr)
         else:
             self.socket.connect((self.ip, self.port))
 
     def send(self, data):
         """
         send any type of data, it might be List, NDArray, etc
         """
         if not self.is_server:
             self.socket.send(data)
         else:
-            print('server can not send data for now.')
+            print("server can not send data for now.")
 
     def did_received_data(self, func):
         self.did_received_data_func = func
 
     def receive(self):
         data = self.conn.recv(self.MAX_BUFFER_SIZE)
         a = np.frombuffer(data, dtype=np.float32)
```

### Comparing `alfred-py-3.0.6/alfred/utils/cv_wrapper.py` & `alfred-py-3.0.7/alfred/utils/cv_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 """
 import cv2
 from PIL import Image, ImageFont, ImageDraw
 import os
 import numpy as np
 
 
-font_f = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "fonts/FZSSJW.TTF")
+font_f = os.path.join(
+    os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "fonts/FZSSJW.TTF"
+)
+
 
 def put_cn_txt_on_img(img, txt, ori, font_scale, color):
     """
     put Chinese text on image
     """
     img_PIL = Image.fromarray(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
-    assert os.path.exists(font_f), '{} not found'.format(font_f)
+    assert os.path.exists(font_f), "{} not found".format(font_f)
     font = ImageFont.truetype(font_f, 25)
-    fillColor = color #(255,0,0)
-    position = ori #(100,100)
+    fillColor = color  # (255,0,0)
+    position = ori  # (100,100)
     draw = ImageDraw.Draw(img_PIL)
     draw.text(position, txt, font=font, fill=fillColor)
     img = cv2.cvtColor(np.asarray(img_PIL), cv2.COLOR_RGB2BGR)
-    return img
+    return img
```

### Comparing `alfred-py-3.0.6/alfred/utils/file_io.py` & `alfred-py-3.0.7/alfred/utils/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import IO, Any, Dict, List, MutableMapping, Optional
 from urllib.parse import urlparse
 import portalocker
 import logging
 import shutil
 from typing import Callable, Optional
 from urllib import request
+
 try:
     import cv2 as cv
 except ImportError as e:
     cv = None
 
 try:
     import cv2 as cv
@@ -563,15 +564,15 @@
 
 
 class SourceIter:
     def __init__(self, src, exit_auto=True):
         self.src = src
         self.srcs = []
         self.crt_index = 0
-        self.crt_filename = ''
+        self.crt_filename = ""
         self.video_mode = False
         self.webcam_mode = False
         self.cap = None
         self.ok = True
         self.exit_auto = exit_auto
 
     def __len__(self):
@@ -591,32 +592,33 @@
                 else:
                     self.ok = False
             else:
                 return frame
         else:
             if self.crt_index < len(self.srcs):
                 p = self.srcs[self.crt_index]
+                self.crt_filename = os.path.basename(p)
                 self.crt_index += 1
                 self.crt_filename = os.path.basename(p)
                 return p
             else:
                 if self.exit_auto:
                     print("Seems iteration done. bye~")
                     exit(0)
                 else:
                     self.ok = False
                 # raise StopIteration
 
 
 class ImageSourceIter(SourceIter):
-    def __init__(self, src, exit_auto=True):
+    def __init__(self, src, exit_auto=True, save_res_video=False):
         super(ImageSourceIter, self).__init__(src, exit_auto)
 
         self._index_sources()
-        self.is_written = False
+        self.is_written = save_res_video
         self.save_f = None
         assert len(self.srcs) > 0, "srcs indexed empty: {}".format(self.srcs)
         self.lens = len(self.srcs)
         if self.video_mode and not self.webcam_mode:
             self.is_save_video_called = False
             fourcc = cv.VideoWriter_fourcc(*"XVID")
             self.video_width = int(self.cap.get(cv.CAP_PROP_FRAME_WIDTH) + 0.5)
@@ -624,15 +626,15 @@
             self.video_height = int(self.cap.get(cv.CAP_PROP_FRAME_HEIGHT) + 0.5)
             if self.video_mode:
                 self.filename = os.path.basename(src).split(".")[0]
                 self.save_f = os.path.join(
                     os.path.dirname(src), self.filename + "_result.mp4"
                 )
                 self.lens = self.video_frame_count
-            else:
+            elif self.webcam_mode:
                 os.makedirs("results", exist_ok=True)
                 self.save_f = os.path.join("results/webcam_result.mp4")
             self.video_writter = cv.VideoWriter(
                 self.save_f, fourcc, 25.0, (self.video_width, self.video_height)
             )
 
     def get_specific_frames(self, frame_indexes, verbose=True):
@@ -714,44 +716,67 @@
         if self.video_mode:
             self.cap.release()
             if not self.webcam_mode:
                 self.video_writter.release()
             if self.is_written and self.is_save_video_called:
                 print("your wrote video result file should saved into: ", self.save_f)
             else:
-                if self.save_f and os.path.exists(self.save_f):
-                    # clean up remove saved file.
-                    os.remove(self.save_f)
+                if self.save_f is not None:
+                    pass
+                    # if os.path.exists(self.save_f):
+                    #     # clean up remove saved file.
+                    #     os.remove(self.save_f)
+
+    def clear_early_quit(self):
+        if self.video_mode:
+            self.cap.release()
+            if not self.webcam_mode:
+                self.video_writter.release()
+            if self.is_written and self.is_save_video_called:
+                print("your wrote video result file should saved into: ", self.save_f)
+            else:
+                if self.save_f is not None:
+                    if os.path.exists(self.save_f):
+                        # clean up remove saved file.
+                        os.remove(self.save_f)
 
     def waitKey(self):
         if self.video_mode:
-            cv.waitKey(1)
+            if cv.waitKey(1) > 0:
+                print("key pressed, exit show..")
+                self.ok = False
+                self.clear_early_quit()
+                # exit(0)
         else:
             cv.waitKey(0)
     
     def show(self, winname, img):
         cv.imshow(winname, img)
 
+    def show(self, winname, mat):
+        cv.imshow(winname, mat)
+
 
 def next_item(iter):
     itm = next(iter)
     if isinstance(itm, str):
         itm = cv.imread(itm)
     return itm
 
+
 class ImageSourceIterAsync(SourceIter):
     """
     reading frames in threads if on video mode
     using queue to to contains readed frames
     """
 
     def __init__(self, src, exit_auto=True):
         super(ImageSourceIter, self).__init__(src, exit_auto)
         import cv2 as cv
-        
+
         self._index_sources()
         self.is_written = False
         self.save_f = None
         assert len(self.srcs) > 0, "srcs indexed empty: {}".format(self.srcs)
         self.lens = len(self.srcs)
         if self.video_mode and not self.webcam_mode:
             self.is_save_video_called = False
@@ -859,8 +884,8 @@
                     os.remove(self.save_f)
 
 
 def get_next_frame(iter):
     itm = next(iter)
     if os.path.isfile(itm):
         itm = cv.imread(itm)
-    return itm
+    return itm
```

### Comparing `alfred-py-3.0.6/alfred/utils/image_convertor.py` & `alfred-py-3.0.7/alfred/utils/image_convertor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
         new_image = new_image[:, :, [2, 1, 0, 3]]
     new_image = Image.fromarray(new_image)
     return new_image
 
 
 def pil2cv(pil_image):
     new_image = cv2.cvtColor(np.array(pil_image), cv2.COLOR_RGB2BGR)
-    return new_image
+    return new_image
```

### Comparing `alfred-py-3.0.6/alfred/utils/log.py` & `alfred-py-3.0.7/alfred/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         format="<lvl>{level}</lvl> {time:MM-DD HH:mm:ss} {file}:{line} - {message}",
     )
 
 
 def formatter(record):
     # package_name = get_package_name()
     filename = record["file"].name
-    if len(record['file'].name) > 17:
-        filename = record["file"].name[:12] + '..' + record["file"].name[-3:]
+    if len(record["file"].name) > 17:
+        filename = record["file"].name[:12] + ".." + record["file"].name[-3:]
     record["extra"].update(filename=filename)
     return "{time:HH:mm:ss MM.DD} <lvl>{level}</lvl> {extra[filename]}:{line}]: {message}\n{exception}"
 
 
 logger.remove()  # Remove the pre-configured handler
 logger.start(
     sys.stderr,
```

### Comparing `alfred-py-3.0.6/alfred/utils/mana.py` & `alfred-py-3.0.7/alfred/utils/mana.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,21 +25,30 @@
 Utils using in MANA universe
 
 such as print welcome message
 """
 from colorama import Fore, Back, Style
 
 
-welcome_msg = '''
+welcome_msg = """
     __  ______    _   _____    ___    ____
    /  |/  /   |  / | / /   |  /   |  /  _/
   / /|_/ / /| | /  |/ / /| | / /| |  / /  
  / /  / / ___ |/ /|  / ___ |/ ___ |_/ /   
 /_/  /_/_/  |_/_/ |_/_/  |_/_/  |_/___/    http://manaai.cn
-'''
+"""
+
 
 def welcome(ori_git_url):
-    print(Fore.YELLOW + Style.BRIGHT + 'Welcome to MANA AI platform!' + Style.RESET_ALL)
+    print(Fore.YELLOW + Style.BRIGHT + "Welcome to MANA AI platform!" + Style.RESET_ALL)
     print(Fore.BLUE + Style.BRIGHT + welcome_msg + Style.RESET_ALL)
-    print(Style.BRIGHT + "once you saw this msg, indicates you were back supported by our team!" + Style.RESET_ALL)
-    print('the latest updates of our codes always at: {} or {}'.format(ori_git_url, 'http://manaai.cn'))
-    print('NOTE: Our codes distributed from anywhere else were not supported!')
+    print(
+        Style.BRIGHT
+        + "once you saw this msg, indicates you were back supported by our team!"
+        + Style.RESET_ALL
+    )
+    print(
+        "the latest updates of our codes always at: {} or {}".format(
+            ori_git_url, "http://manaai.cn"
+        )
+    )
+    print("NOTE: Our codes distributed from anywhere else were not supported!")
```

### Comparing `alfred-py-3.0.6/alfred/utils/math_utils.py` & `alfred-py-3.0.7/alfred/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/utils/pprint.py` & `alfred-py-3.0.7/alfred/utils/pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pprint import pprint, pformat
 
+
 def _highlight(code, filename):
     try:
         import pygments
     except ImportError:
         return code
 
     from pygments.lexers import Python3Lexer, YamlLexer
```

### Comparing `alfred-py-3.0.6/alfred/utils/timer.py` & `alfred-py-3.0.7/alfred/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 
 class Timer(object):
     """A simple timer."""
 
     def __init__(self, name: str):
         self.name = name
-        self.total_time = 0.
+        self.total_time = 0.0
         self.calls = 0
-        self.start_time = 0.
-        self.diff = 0.
-        self.average_time = 0.
+        self.start_time = 0.0
+        self.diff = 0.0
+        self.average_time = 0.0
 
     def tic(self):
         # using time.time instead of time.clock because time time.clock
         # does not normalize for multithreading
         self.start_time = time.perf_counter()
 
     def toc(self, average=True):
@@ -33,40 +33,39 @@
         self.average_time = self.total_time / self.calls
         if average:
             return self.average_time
         else:
             return self.diff
 
     def clear(self):
-        self.total_time = 0.
+        self.total_time = 0.0
         self.calls = 0
-        self.start_time = 0.
-        self.diff = 0.
-        self.average_time = 0.
+        self.start_time = 0.0
+        self.diff = 0.0
+        self.average_time = 0.0
 
 
 class TimerManager(ABC):
-
     def __init__(self, timer_names: Union[List[str], str]):
         self.timer_names = timer_names
         self.tpls = []
 
         if isinstance(self.timer_names, list):
             for tn in self.timer_names:
                 setattr(self, tn, Timer(tn))
                 self.tpls.append(tn)
 
     def collect_avg(self):
         for tn in self.timer_names:
             obj = getattr(self, tn)
-            print(f'{obj.name}: {obj.average_time*1000:.3f}ms')
-        print('')
+            print(f"{obj.name}: {obj.average_time*1000:.3f}ms")
+        print("")
 
 
-'''
+"""
 
 timers = create_some_timers(['det', 'mesh', 'reg'])
 
 timers.det.tic()
 ...
 timers.det.toc()
 
@@ -74,15 +73,15 @@
 timers.mesh.tic()
 ...
 timers.mesh.toc()
 
 
 timers.collect_avg()
 
-'''
+"""
 
 
 class ATimer:
     records = {}
     tmp = None
 
     @classmethod
@@ -93,35 +92,39 @@
     def toc(cls):
         res = (time.time() - cls.tmp) * 1000
         cls.tmp = None
         return res
 
     @classmethod
     def report(cls):
-        header = ['', 'Time(ms)']
+        header = ["", "Time(ms)"]
         contents = []
         for key, val in cls.records.items():
             contents.append(
-                ['{:20s}'.format(key), '{:.2f}'.format(sum(val)/len(val))])
-        print(tabulate.tabulate(contents, header, tablefmt='fancy_grid'))
+                ["{:20s}".format(key), "{:.2f}".format(sum(val) / len(val))]
+            )
+        print(tabulate.tabulate(contents, header, tablefmt="fancy_grid"))
 
     def __init__(self, name, silent=False):
         self.name = name
         self.silent = silent
         if name not in ATimer.records.keys():
             ATimer.records[name] = []
 
     def __enter__(self):
         self.start = time.time()
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         end = time.time()
-        ATimer.records[self.name].append((end-self.start)*1000)
+        ATimer.records[self.name].append((end - self.start) * 1000)
         if not self.silent:
-            t = (end - self.start)*1000
+            t = (end - self.start) * 1000
             if t > 1000:
-                print('-> [{:20s}]: {:5.1f}s'.format(self.name, t/1000))
-            elif t > 1e3*60*60:
-                print('-> [{:20s}]: {:5.1f}min'.format(self.name, t/1e3/60))
+                print("-> [{:20s}]: {:5.1f}s".format(self.name, t / 1000))
+            elif t > 1e3 * 60 * 60:
+                print("-> [{:20s}]: {:5.1f}min".format(self.name, t / 1e3 / 60))
             else:
-                print('-> [{:20s}]: {:5.1f}ms'.format(self.name,
-                      (end-self.start)*1000))
+                print(
+                    "-> [{:20s}]: {:5.1f}ms".format(
+                        self.name, (end - self.start) * 1000
+                    )
+                )
```

### Comparing `alfred-py-3.0.6/alfred/version.py` & `alfred-py-3.0.7/alfred/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Lucas Jin. All rights reserved.
 from datetime import datetime
 
 major_num = 2
 
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 short_version = __version__
 
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split("."):
         if x.isdigit():
```

### Comparing `alfred-py-3.0.6/alfred/vis/__init__.py` & `alfred-py-3.0.7/alfred/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/image/__init__.py` & `alfred-py-3.0.7/alfred/vis/image/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/image/common.py` & `alfred-py-3.0.7/alfred/vis/image/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,35 +33,56 @@
 from .get_dataset_color_map import create_cityscapes_label_colormap
 
 
 class Colors:
     # Ultralytics color palette https://ultralytics.com/
     def __init__(self):
         # hex = matplotlib.colors.TABLEAU_COLORS.values()
-        hex = ('FF3838', 'FF9D97', 'FF701F', 'FFB21D', 'CFD231', '48F90A', '92CC17', '3DDB86', '1A9334', '00D4BB',
-               '2C99A8', '00C2FF', '344593', '6473FF', '0018EC', '8438FF', '520085', 'CB38FF', 'FF95C8', 'FF37C7')
-        self.palette = [self.hex2rgb('#' + c) for c in hex]
+        hex = (
+            "FF3838",
+            "FF9D97",
+            "FF701F",
+            "FFB21D",
+            "CFD231",
+            "48F90A",
+            "92CC17",
+            "3DDB86",
+            "1A9334",
+            "00D4BB",
+            "2C99A8",
+            "00C2FF",
+            "344593",
+            "6473FF",
+            "0018EC",
+            "8438FF",
+            "520085",
+            "CB38FF",
+            "FF95C8",
+            "FF37C7",
+        )
+        self.palette = [self.hex2rgb("#" + c) for c in hex]
         self.n = len(self.palette)
 
     def __call__(self, i, bgr=False):
         c = self.palette[int(i) % self.n]
         return (c[2], c[1], c[0]) if bgr else c
 
     @staticmethod
     def hex2rgb(h):  # rgb order (PIL)
-        return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
+        return tuple(int(h[1 + i : 1 + i + 2], 16) for i in (0, 2, 4))
 
 
 colors = Colors()  # create instance for 'from utils.plots import colors'
 global_random_choices_for_u = [np.random.randint(len(light_colors)) for i in range(200)]
 dynamic_cls_name_color_map = dict()
 
+
 def create_unique_color_float(tag, hue_step=0.41, alpha=0.7):
-    h, v = (tag * hue_step) % 1, 1. - (int(tag * hue_step) % 4) / 5.
-    r, g, b = colorsys.hsv_to_rgb(h, 1., v)
+    h, v = (tag * hue_step) % 1, 1.0 - (int(tag * hue_step) % 4) / 5.0
+    r, g, b = colorsys.hsv_to_rgb(h, 1.0, v)
     return r, g, b, alpha
 
 
 def create_unique_color_uchar(tag, hue_step=0.41, alpha=0.7):
     r, g, b, a = create_unique_color_float(tag, hue_step, alpha)
     return int(255 * r), int(255 * g), int(255 * b), int(255 * a)
 
@@ -81,89 +102,92 @@
     if dark:
         idx = idx % len(dark_colors)
         return dark_colors[idx]
     else:
         idx = idx % len(light_colors)
         return light_colors[idx]
 
+
 def get_unique_color_by_id3(idx, dark=False):
     color_idx = global_random_choices_for_u[idx]
     if dark:
         idx = idx % len(dark_colors)
         return dark_colors[color_idx]
     else:
         idx = idx % len(light_colors)
         return light_colors[color_idx]
 
+
 def get_unique_color_by_id_with_dataset(idx):
     colors = create_cityscapes_label_colormap()
     idx = idx % len(colors)
     return colors[idx]
 
 
 """
 we need some help functions to draw doted rectangle in opencv
 """
 
 
-def _drawline(img, pt1, pt2, color, thickness=1, style='dotted', gap=20):
-    dist = ((pt1[0]-pt2[0])**2+(pt1[1]-pt2[1])**2)**.5
+def _drawline(img, pt1, pt2, color, thickness=1, style="dotted", gap=20):
+    dist = ((pt1[0] - pt2[0]) ** 2 + (pt1[1] - pt2[1]) ** 2) ** 0.5
     pts = []
     for i in np.arange(0, dist, gap):
-        r = i/dist
-        x = int((pt1[0]*(1-r)+pt2[0]*r)+.5)
-        y = int((pt1[1]*(1-r)+pt2[1]*r)+.5)
+        r = i / dist
+        x = int((pt1[0] * (1 - r) + pt2[0] * r) + 0.5)
+        y = int((pt1[1] * (1 - r) + pt2[1] * r) + 0.5)
         p = (x, y)
         pts.append(p)
 
-    if style == 'dotted':
+    if style == "dotted":
         for p in pts:
             cv2.circle(img, p, thickness, color, -1)
-    elif style == 'dashed':
+    elif style == "dashed":
         s = pts[0]
         e = pts[0]
         i = 0
         for p in pts:
             s = e
             e = p
             if i % 2 == 1:
                 cv2.line(img, s, e, color, thickness)
             i += 1
     else:
-        ValueError('style can only be dotted or dashed for now!')
+        ValueError("style can only be dotted or dashed for now!")
 
 
-def _drawpoly(img, pts, color, thickness=1, style='dotted',):
+def _drawpoly(
+    img,
+    pts,
+    color,
+    thickness=1,
+    style="dotted",
+):
     s = pts[0]
     e = pts[0]
     pts.append(pts.pop(0))
     for p in pts:
         s = e
         e = p
         _drawline(img, s, e, color, thickness, style, gap=6)
 
 
-def draw_rect_with_style(img, pt1, pt2, color, thickness=1, style='dotted'):
+def draw_rect_with_style(img, pt1, pt2, color, thickness=1, style="dotted"):
     pts = [pt1, (pt2[0], pt1[1]), pt2, (pt1[0], pt2[1])]
     _drawpoly(img, pts, color, thickness, style)
     return img
 
 
-def put_txt_with_newline(image, multi_line_txt, pt, font, font_scale, color, thickness, line_type):
+def put_txt_with_newline(
+    image, multi_line_txt, pt, font, font_scale, color, thickness, line_type
+):
     text_size, _ = cv2.getTextSize(multi_line_txt, font, font_scale, thickness)
     line_height = text_size[1] + 5
     x, y0 = pt
     for i, line in enumerate(multi_line_txt.split("\n")):
         y = y0 + i * line_height
-        cv2.putText(image,
-                    line,
-                    (x, y),
-                    font,
-                    font_scale,
-                    color,
-                    thickness,
-                    line_type)
+        cv2.putText(image, line, (x, y), font, font_scale, color, thickness, line_type)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     c = create_unique_color_uchar(1)
     print(c)
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/constants.py` & `alfred-py-3.0.7/alfred/vis/image/constants.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/image/det.py` & `alfred-py-3.0.7/alfred/vis/image/det.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,25 +524,27 @@
 
     if class_names is None or len(class_names) == 0:
         class_names = coco_label_map_list[1:]
     else:
         if cls_ids is None:
             # not class id, using default name, assue only 1 class
             if class_names is None:
-                class_names = ['object']
+                class_names = ["object"]
             if class_names[0] not in dynamic_cls_name_color_map.keys():
-                dynamic_cls_name_color_map[class_names[0]] = colors(np.random.choice(global_random_choices_for_u))
+                dynamic_cls_name_color_map[class_names[0]] = colors(
+                    np.random.choice(global_random_choices_for_u)
+                )
             force_color = [dynamic_cls_name_color_map[class_names[0]]]
             # class_names.insert(0, 'none')
-    
+
     for i in range(n_boxes):
         if cls_ids is not None:
             cls_id = int(cls_ids[i])
         else:
-            cls_id = 0 # fake id, assume just one class
+            cls_id = 0  # fake id, assume just one class
         if cls_id != background_id:
             if scores is not None:
                 if scores[i] > thresh:
                     if force_color:
                         if random:
                             unique_color = force_color[np.random.randint(100)]
                         else:
@@ -616,25 +618,37 @@
                     )
                     # txt_bottom_left = (x1+4, y1-4)
                     delta = 4
                     txt_bottom_left = (x1, y1 - delta)  # make text a little higher
                     if transparent:
                         cv2.rectangle(
                             img_mask,
-                            (txt_bottom_left[0], txt_bottom_left[1] - ret_val[1] - delta),
-                            (txt_bottom_left[0] + ret_val[0], txt_bottom_left[1] + delta),
+                            (
+                                txt_bottom_left[0],
+                                txt_bottom_left[1] - ret_val[1] - delta,
+                            ),
+                            (
+                                txt_bottom_left[0] + ret_val[0],
+                                txt_bottom_left[1] + delta,
+                            ),
                             unique_color,
                             -1,
                             cv2.LINE_AA,
                         )
                     else:
                         cv2.rectangle(
                             img,
-                            (txt_bottom_left[0], txt_bottom_left[1] - ret_val[1] - delta),
-                            (txt_bottom_left[0] + ret_val[0], txt_bottom_left[1] + delta),
+                            (
+                                txt_bottom_left[0],
+                                txt_bottom_left[1] - ret_val[1] - delta,
+                            ),
+                            (
+                                txt_bottom_left[0] + ret_val[0],
+                                txt_bottom_left[1] + delta,
+                            ),
                             unique_color,
                             -1,
                             cv2.LINE_AA,
                         )
                     cv2.putText(
                         img,
                         text_label,
@@ -698,17 +712,17 @@
                             cv2.LINE_AA,
                         )
 
                 if class_names:
                     text_label = "{}".format(class_names[cls_id])
                 else:
                     text_label = "{}".format(cls_id)
-                
+
                 if track_ids:
-                    text_label += ' ID: {}'.format(track_ids[i])
+                    text_label += " ID: {}".format(track_ids[i])
 
                 (ret_val, _) = cv2.getTextSize(
                     text_label, font, font_scale, font_thickness
                 )
                 txt_bottom_left = (x1 + 4, y1 - 4)
                 if transparent:
                     cv2.rectangle(
@@ -924,26 +938,22 @@
             ]
         ).reshape((4, 4))
         # print('start draw...')
         for i in range(4):
             x = np.append(
                 box_3d[
                     0,
-                    face_idx[
-                        i,
-                    ],
+                    face_idx[i,],
                 ],
                 box_3d[0, face_idx[i, 0]],
             )
             y = np.append(
                 box_3d[
                     1,
-                    face_idx[
-                        i,
-                    ],
+                    face_idx[i,],
                 ],
                 box_3d[1, face_idx[i, 0]],
             )
             # print('x: ', x)
             # print('y: ', y)
             # cv2.line(img, (point_1_, point_1_), (point_2_, point_2_), color, 1)
             pts = np.vstack((x, y)).T
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/face.py` & `alfred-py-3.0.7/alfred/vis/image/face.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,8 +26,7 @@
             right_bottom = (right, bottom)
             left_bottom = (left, bottom)
             cv2.line(img, left_top, right_top, line_color, 1, cv2.LINE_AA)
             cv2.line(img, right_top, right_bottom, line_color, 1, cv2.LINE_AA)
             cv2.line(img, right_bottom, left_bottom, line_color, 1, cv2.LINE_AA)
             cv2.line(img, left_bottom, left_top, line_color, 1, cv2.LINE_AA)
     return img
-
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/get_dataset_color_map.py` & `alfred-py-3.0.7/alfred/vis/image/get_dataset_color_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,364 +34,372 @@
 
 * PASCAL VOC 2012 (http://host.robots.ox.ac.uk/pascal/VOC/).
 """
 
 import numpy as np
 
 # Dataset names.
-_ADE20K = 'ade20k'
-_CITYSCAPES = 'cityscapes'
-_MAPILLARY_VISTAS = 'mapillary_vistas'
-_PASCAL = 'pascal'
+_ADE20K = "ade20k"
+_CITYSCAPES = "cityscapes"
+_MAPILLARY_VISTAS = "mapillary_vistas"
+_PASCAL = "pascal"
 
 # Max number of entries in the colormap for each dataset.
 _DATASET_MAX_ENTRIES = {
     _ADE20K: 151,
     _CITYSCAPES: 19,
     _MAPILLARY_VISTAS: 66,
     _PASCAL: 256,
 }
 
 
 def create_coco_stuff_colormap():
-    return np.asarray([
-        [201, 189, 129],
-        [165, 42, 42],
-        [41, 191, 255],  # sky
-        [81,  0, 81],  # drivable_area
-        [0, 163, 65],  # trees
-        [153, 153, 153],  # pole 5
-        [244, 35, 232],
-        [6, 166, 0],  # 7 cross walk
-        [0,  0, 142],
-        [140, 140, 200],
-        [220, 220,  0],
-        [18, 122, 201],
-        [250, 170, 30],  # 12 trafficlight
-        [230, 150, 140],
-        [220, 20, 60],  # 14 pedestrian
-        [255, 79, 161],
-        [255,  0,  0],  # rider
-        [150, 100, 100],
-        [70, 70, 70],
-        [150, 120, 90],
-        [220, 20, 60],
-        [255, 132, 0],  # guard rail
-        [255, 255, 255],  # lane_broken_white
-        [255, 255, 0],  # lane 23
-        [200, 128, 128],
-        [255, 255, 255],
-        [0,  0, 70],  # 26 truck
-        [251, 255, 0],  # lane solid white
-        [70, 130, 180],
-        [0, 218, 230],  # vehicle_construction_vehicle 29
-        [255, 112, 10],  # cone 30
-        [149, 0, 255],  # stop lane 31
-        [0, 170, 30],
-        [255, 255, 128],
-        [250, 0, 30],
-        [0, 255, 255],
-        [220, 220, 220],
-        [170, 170, 170],
-        [0,  0, 142],
-        [100, 170, 30],
-        [40, 40, 40],
-        [0, 162, 255],  # 41
-        [170, 170, 170],
-        [0, 0, 142],
-        [170, 170, 170],
-        [210, 170, 100],
-        [153, 153, 153],
-        [128, 128, 128],
-        [0, 0, 142],
-        [250, 170, 30],
-        [192, 192, 192],
-        [220, 220, 0],
-        [180, 165, 180],
-        [119, 11, 32],
-        [0, 0, 142],
-        [0, 60, 100],
-        [13, 181, 136],  # vehicle_other 56
-        [0, 0, 90],
-        [0, 0, 230],
-        [0, 80, 100],
-        [128, 64, 64],
-        [0, 0, 110],
-        [0, 0, 70],
-        [0, 0, 192],
-        [32, 32, 32],
-        [0, 0, 0],
-        [0, 0, 0],
-    ])
+    return np.asarray(
+        [
+            [201, 189, 129],
+            [165, 42, 42],
+            [41, 191, 255],  # sky
+            [81, 0, 81],  # drivable_area
+            [0, 163, 65],  # trees
+            [153, 153, 153],  # pole 5
+            [244, 35, 232],
+            [6, 166, 0],  # 7 cross walk
+            [0, 0, 142],
+            [140, 140, 200],
+            [220, 220, 0],
+            [18, 122, 201],
+            [250, 170, 30],  # 12 trafficlight
+            [230, 150, 140],
+            [220, 20, 60],  # 14 pedestrian
+            [255, 79, 161],
+            [255, 0, 0],  # rider
+            [150, 100, 100],
+            [70, 70, 70],
+            [150, 120, 90],
+            [220, 20, 60],
+            [255, 132, 0],  # guard rail
+            [255, 255, 255],  # lane_broken_white
+            [255, 255, 0],  # lane 23
+            [200, 128, 128],
+            [255, 255, 255],
+            [0, 0, 70],  # 26 truck
+            [251, 255, 0],  # lane solid white
+            [70, 130, 180],
+            [0, 218, 230],  # vehicle_construction_vehicle 29
+            [255, 112, 10],  # cone 30
+            [149, 0, 255],  # stop lane 31
+            [0, 170, 30],
+            [255, 255, 128],
+            [250, 0, 30],
+            [0, 255, 255],
+            [220, 220, 220],
+            [170, 170, 170],
+            [0, 0, 142],
+            [100, 170, 30],
+            [40, 40, 40],
+            [0, 162, 255],  # 41
+            [170, 170, 170],
+            [0, 0, 142],
+            [170, 170, 170],
+            [210, 170, 100],
+            [153, 153, 153],
+            [128, 128, 128],
+            [0, 0, 142],
+            [250, 170, 30],
+            [192, 192, 192],
+            [220, 220, 0],
+            [180, 165, 180],
+            [119, 11, 32],
+            [0, 0, 142],
+            [0, 60, 100],
+            [13, 181, 136],  # vehicle_other 56
+            [0, 0, 90],
+            [0, 0, 230],
+            [0, 80, 100],
+            [128, 64, 64],
+            [0, 0, 110],
+            [0, 0, 70],
+            [0, 0, 192],
+            [32, 32, 32],
+            [0, 0, 0],
+            [0, 0, 0],
+        ]
+    )
 
 
 def create_ade20k_label_colormap():
     """Creates a label colormap used in ADE20K segmentation benchmark.
 
     Returns:
       A colormap for visualizing segmentation results.
     """
-    return np.asarray([
-        [0, 0, 0],
-        [120, 120, 120],
-        [180, 120, 120],
-        [6, 230, 230],
-        [80, 50, 50],
-        [4, 200, 3],
-        [120, 120, 80],
-        [140, 140, 140],
-        [204, 5, 255],
-        [230, 230, 230],
-        [4, 250, 7],
-        [224, 5, 255],
-        [235, 255, 7],
-        [150, 5, 61],
-        [120, 120, 70],
-        [8, 255, 51],
-        [255, 6, 82],
-        [143, 255, 140],
-        [204, 255, 4],
-        [255, 51, 7],
-        [204, 70, 3],
-        [0, 102, 200],
-        [61, 230, 250],
-        [255, 6, 51],
-        [11, 102, 255],
-        [255, 7, 71],
-        [255, 9, 224],
-        [9, 7, 230],
-        [220, 220, 220],
-        [255, 9, 92],
-        [112, 9, 255],
-        [8, 255, 214],
-        [7, 255, 224],
-        [255, 184, 6],
-        [10, 255, 71],
-        [255, 41, 10],
-        [7, 255, 255],
-        [224, 255, 8],
-        [102, 8, 255],
-        [255, 61, 6],
-        [255, 194, 7],
-        [255, 122, 8],
-        [0, 255, 20],
-        [255, 8, 41],
-        [255, 5, 153],
-        [6, 51, 255],
-        [235, 12, 255],
-        [160, 150, 20],
-        [0, 163, 255],
-        [140, 140, 140],
-        [250, 10, 15],
-        [20, 255, 0],
-        [31, 255, 0],
-        [255, 31, 0],
-        [255, 224, 0],
-        [153, 255, 0],
-        [0, 0, 255],
-        [255, 71, 0],
-        [0, 235, 255],
-        [0, 173, 255],
-        [31, 0, 255],
-        [11, 200, 200],
-        [255, 82, 0],
-        [0, 255, 245],
-        [0, 61, 255],
-        [0, 255, 112],
-        [0, 255, 133],
-        [255, 0, 0],
-        [255, 163, 0],
-        [255, 102, 0],
-        [194, 255, 0],
-        [0, 143, 255],
-        [51, 255, 0],
-        [0, 82, 255],
-        [0, 255, 41],
-        [0, 255, 173],
-        [10, 0, 255],
-        [173, 255, 0],
-        [0, 255, 153],
-        [255, 92, 0],
-        [255, 0, 255],
-        [255, 0, 245],
-        [255, 0, 102],
-        [255, 173, 0],
-        [255, 0, 20],
-        [255, 184, 184],
-        [0, 31, 255],
-        [0, 255, 61],
-        [0, 71, 255],
-        [255, 0, 204],
-        [0, 255, 194],
-        [0, 255, 82],
-        [0, 10, 255],
-        [0, 112, 255],
-        [51, 0, 255],
-        [0, 194, 255],
-        [0, 122, 255],
-        [0, 255, 163],
-        [255, 153, 0],
-        [0, 255, 10],
-        [255, 112, 0],
-        [143, 255, 0],
-        [82, 0, 255],
-        [163, 255, 0],
-        [255, 235, 0],
-        [8, 184, 170],
-        [133, 0, 255],
-        [0, 255, 92],
-        [184, 0, 255],
-        [255, 0, 31],
-        [0, 184, 255],
-        [0, 214, 255],
-        [255, 0, 112],
-        [92, 255, 0],
-        [0, 224, 255],
-        [112, 224, 255],
-        [70, 184, 160],
-        [163, 0, 255],
-        [153, 0, 255],
-        [71, 255, 0],
-        [255, 0, 163],
-        [255, 204, 0],
-        [255, 0, 143],
-        [0, 255, 235],
-        [133, 255, 0],
-        [255, 0, 235],
-        [245, 0, 255],
-        [255, 0, 122],
-        [255, 245, 0],
-        [10, 190, 212],
-        [214, 255, 0],
-        [0, 204, 255],
-        [20, 0, 255],
-        [255, 255, 0],
-        [0, 153, 255],
-        [0, 41, 255],
-        [0, 255, 204],
-        [41, 0, 255],
-        [41, 255, 0],
-        [173, 0, 255],
-        [0, 245, 255],
-        [71, 0, 255],
-        [122, 0, 255],
-        [0, 255, 184],
-        [0, 92, 255],
-        [184, 255, 0],
-        [0, 133, 255],
-        [255, 214, 0],
-        [25, 194, 194],
-        [102, 255, 0],
-        [92, 0, 255],
-    ])
+    return np.asarray(
+        [
+            [0, 0, 0],
+            [120, 120, 120],
+            [180, 120, 120],
+            [6, 230, 230],
+            [80, 50, 50],
+            [4, 200, 3],
+            [120, 120, 80],
+            [140, 140, 140],
+            [204, 5, 255],
+            [230, 230, 230],
+            [4, 250, 7],
+            [224, 5, 255],
+            [235, 255, 7],
+            [150, 5, 61],
+            [120, 120, 70],
+            [8, 255, 51],
+            [255, 6, 82],
+            [143, 255, 140],
+            [204, 255, 4],
+            [255, 51, 7],
+            [204, 70, 3],
+            [0, 102, 200],
+            [61, 230, 250],
+            [255, 6, 51],
+            [11, 102, 255],
+            [255, 7, 71],
+            [255, 9, 224],
+            [9, 7, 230],
+            [220, 220, 220],
+            [255, 9, 92],
+            [112, 9, 255],
+            [8, 255, 214],
+            [7, 255, 224],
+            [255, 184, 6],
+            [10, 255, 71],
+            [255, 41, 10],
+            [7, 255, 255],
+            [224, 255, 8],
+            [102, 8, 255],
+            [255, 61, 6],
+            [255, 194, 7],
+            [255, 122, 8],
+            [0, 255, 20],
+            [255, 8, 41],
+            [255, 5, 153],
+            [6, 51, 255],
+            [235, 12, 255],
+            [160, 150, 20],
+            [0, 163, 255],
+            [140, 140, 140],
+            [250, 10, 15],
+            [20, 255, 0],
+            [31, 255, 0],
+            [255, 31, 0],
+            [255, 224, 0],
+            [153, 255, 0],
+            [0, 0, 255],
+            [255, 71, 0],
+            [0, 235, 255],
+            [0, 173, 255],
+            [31, 0, 255],
+            [11, 200, 200],
+            [255, 82, 0],
+            [0, 255, 245],
+            [0, 61, 255],
+            [0, 255, 112],
+            [0, 255, 133],
+            [255, 0, 0],
+            [255, 163, 0],
+            [255, 102, 0],
+            [194, 255, 0],
+            [0, 143, 255],
+            [51, 255, 0],
+            [0, 82, 255],
+            [0, 255, 41],
+            [0, 255, 173],
+            [10, 0, 255],
+            [173, 255, 0],
+            [0, 255, 153],
+            [255, 92, 0],
+            [255, 0, 255],
+            [255, 0, 245],
+            [255, 0, 102],
+            [255, 173, 0],
+            [255, 0, 20],
+            [255, 184, 184],
+            [0, 31, 255],
+            [0, 255, 61],
+            [0, 71, 255],
+            [255, 0, 204],
+            [0, 255, 194],
+            [0, 255, 82],
+            [0, 10, 255],
+            [0, 112, 255],
+            [51, 0, 255],
+            [0, 194, 255],
+            [0, 122, 255],
+            [0, 255, 163],
+            [255, 153, 0],
+            [0, 255, 10],
+            [255, 112, 0],
+            [143, 255, 0],
+            [82, 0, 255],
+            [163, 255, 0],
+            [255, 235, 0],
+            [8, 184, 170],
+            [133, 0, 255],
+            [0, 255, 92],
+            [184, 0, 255],
+            [255, 0, 31],
+            [0, 184, 255],
+            [0, 214, 255],
+            [255, 0, 112],
+            [92, 255, 0],
+            [0, 224, 255],
+            [112, 224, 255],
+            [70, 184, 160],
+            [163, 0, 255],
+            [153, 0, 255],
+            [71, 255, 0],
+            [255, 0, 163],
+            [255, 204, 0],
+            [255, 0, 143],
+            [0, 255, 235],
+            [133, 255, 0],
+            [255, 0, 235],
+            [245, 0, 255],
+            [255, 0, 122],
+            [255, 245, 0],
+            [10, 190, 212],
+            [214, 255, 0],
+            [0, 204, 255],
+            [20, 0, 255],
+            [255, 255, 0],
+            [0, 153, 255],
+            [0, 41, 255],
+            [0, 255, 204],
+            [41, 0, 255],
+            [41, 255, 0],
+            [173, 0, 255],
+            [0, 245, 255],
+            [71, 0, 255],
+            [122, 0, 255],
+            [0, 255, 184],
+            [0, 92, 255],
+            [184, 255, 0],
+            [0, 133, 255],
+            [255, 214, 0],
+            [25, 194, 194],
+            [102, 255, 0],
+            [92, 0, 255],
+        ]
+    )
 
 
 def create_cityscapes_label_colormap():
     """Creates a label colormap used in CITYSCAPES segmentation benchmark.
 
     Returns:
       A colormap for visualizing segmentation results.
     """
-    return np.asarray([
-        [128, 64, 128],
-        [244, 35, 232],
-        [70, 70, 70],
-        [102, 102, 156],
-        [190, 153, 153],
-        [153, 153, 153],
-        [250, 170, 30],
-        [220, 220, 0],
-        [107, 142, 35],
-        [152, 251, 152],
-        [70, 130, 180],
-        [220, 20, 60],
-        [255, 0, 0],
-        [0, 0, 142],
-        [0, 0, 70],
-        [0, 60, 100],
-        [0, 80, 100],
-        [0, 0, 230],
-        [119, 11, 32],
-    ])
+    return np.asarray(
+        [
+            [128, 64, 128],
+            [244, 35, 232],
+            [70, 70, 70],
+            [102, 102, 156],
+            [190, 153, 153],
+            [153, 153, 153],
+            [250, 170, 30],
+            [220, 220, 0],
+            [107, 142, 35],
+            [152, 251, 152],
+            [70, 130, 180],
+            [220, 20, 60],
+            [255, 0, 0],
+            [0, 0, 142],
+            [0, 0, 70],
+            [0, 60, 100],
+            [0, 80, 100],
+            [0, 0, 230],
+            [119, 11, 32],
+        ]
+    )
 
 
 def create_mapillary_vistas_label_colormap():
     """Creates a label colormap used in Mapillary Vistas segmentation benchmark.
 
     Returns:
       A colormap for visualizing segmentation results.
     """
-    return np.asarray([
-        [165, 42, 42],
-        [0, 192, 0],
-        [196, 196, 196],
-        [190, 153, 153],
-        [180, 165, 180],
-        [102, 102, 156],
-        [102, 102, 156],
-        [128, 64, 255],
-        [140, 140, 200],
-        [170, 170, 170],
-        [250, 170, 160],
-        [96, 96, 96],
-        [230, 150, 140],
-        [128, 64, 128],
-        [110, 110, 110],
-        [244, 35, 232],
-        [150, 100, 100],
-        [70, 70, 70],
-        [150, 120, 90],
-        [220, 20, 60],
-        [255, 0, 0],
-        [255, 0, 0],
-        [255, 0, 0],
-        [200, 128, 128],
-        [255, 255, 255],
-        [64, 170, 64],
-        [128, 64, 64],
-        [70, 130, 180],
-        [255, 255, 255],
-        [152, 251, 152],
-        [107, 142, 35],
-        [0, 170, 30],
-        [255, 255, 128],
-        [250, 0, 30],
-        [0, 0, 0],
-        [220, 220, 220],
-        [170, 170, 170],
-        [222, 40, 40],
-        [100, 170, 30],
-        [40, 40, 40],
-        [33, 33, 33],
-        [170, 170, 170],
-        [0, 0, 142],
-        [170, 170, 170],
-        [210, 170, 100],
-        [153, 153, 153],
-        [128, 128, 128],
-        [0, 0, 142],
-        [250, 170, 30],
-        [192, 192, 192],
-        [220, 220, 0],
-        [180, 165, 180],
-        [119, 11, 32],
-        [0, 0, 142],
-        [0, 60, 100],
-        [0, 0, 142],
-        [0, 0, 90],
-        [0, 0, 230],
-        [0, 80, 100],
-        [128, 64, 64],
-        [0, 0, 110],
-        [0, 0, 70],
-        [0, 0, 192],
-        [32, 32, 32],
-        [0, 0, 0],
-        [0, 0, 0],
-    ])
+    return np.asarray(
+        [
+            [165, 42, 42],
+            [0, 192, 0],
+            [196, 196, 196],
+            [190, 153, 153],
+            [180, 165, 180],
+            [102, 102, 156],
+            [102, 102, 156],
+            [128, 64, 255],
+            [140, 140, 200],
+            [170, 170, 170],
+            [250, 170, 160],
+            [96, 96, 96],
+            [230, 150, 140],
+            [128, 64, 128],
+            [110, 110, 110],
+            [244, 35, 232],
+            [150, 100, 100],
+            [70, 70, 70],
+            [150, 120, 90],
+            [220, 20, 60],
+            [255, 0, 0],
+            [255, 0, 0],
+            [255, 0, 0],
+            [200, 128, 128],
+            [255, 255, 255],
+            [64, 170, 64],
+            [128, 64, 64],
+            [70, 130, 180],
+            [255, 255, 255],
+            [152, 251, 152],
+            [107, 142, 35],
+            [0, 170, 30],
+            [255, 255, 128],
+            [250, 0, 30],
+            [0, 0, 0],
+            [220, 220, 220],
+            [170, 170, 170],
+            [222, 40, 40],
+            [100, 170, 30],
+            [40, 40, 40],
+            [33, 33, 33],
+            [170, 170, 170],
+            [0, 0, 142],
+            [170, 170, 170],
+            [210, 170, 100],
+            [153, 153, 153],
+            [128, 128, 128],
+            [0, 0, 142],
+            [250, 170, 30],
+            [192, 192, 192],
+            [220, 220, 0],
+            [180, 165, 180],
+            [119, 11, 32],
+            [0, 0, 142],
+            [0, 60, 100],
+            [0, 0, 142],
+            [0, 0, 90],
+            [0, 0, 230],
+            [0, 80, 100],
+            [128, 64, 64],
+            [0, 0, 110],
+            [0, 0, 70],
+            [0, 0, 192],
+            [32, 32, 32],
+            [0, 0, 0],
+            [0, 0, 0],
+        ]
+    )
 
 
 def create_pascal_label_colormap():
     """Creates a label colormap used in PASCAL VOC segmentation benchmark.
 
     Returns:
       A colormap for visualizing segmentation results.
@@ -453,15 +461,15 @@
     elif dataset == _CITYSCAPES:
         return create_cityscapes_label_colormap()
     elif dataset == _MAPILLARY_VISTAS:
         return create_mapillary_vistas_label_colormap()
     elif dataset == _PASCAL:
         return create_pascal_label_colormap()
     else:
-        raise ValueError('Unsupported dataset.')
+        raise ValueError("Unsupported dataset.")
 
 
 def label_to_color_image(label, dataset=_PASCAL):
     """Adds color defined by the dataset colormap to the label.
 
     Args:
       label: A 2D array with integer type, storing the segmentation label.
@@ -473,14 +481,14 @@
         to the dataset color map.
 
     Raises:
       ValueError: If label is not of rank 2 or its value is larger than color
         map maximum entry.
     """
     if label.ndim != 2:
-        raise ValueError('Expect 2-D input label')
+        raise ValueError("Expect 2-D input label")
 
     if np.max(label) >= _DATASET_MAX_ENTRIES[dataset]:
-        raise ValueError('label value too large.')
+        raise ValueError("label value too large.")
 
     colormap = create_label_colormap(dataset)
     return colormap[label]
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/mask.py` & `alfred-py-3.0.7/alfred/vis/image/mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         mask = masks[i]
 
         cls_color = get_unique_color_by_id(label)
         # only get RGB
         instance_color = get_unique_color_by_id(i)[:-1]
         # now adding masks to image, and colorize it
         if score >= score_thresh:
-
             x1 = int(box[0])
             y1 = int(box[1])
             x2 = int(box[2])
             y2 = int(box[3])
 
             if draw_box:
                 image = draw_one_bbox(image, box, cls_color, 1)
@@ -194,15 +193,14 @@
         mask = masks[i]
 
         cls_color = get_unique_color_by_id(label)
         # only get RGB
         instance_color = get_unique_color_by_id(i)[:-1]
         # now adding masks to image, and colorize it
         if score >= score_thresh:
-
             x1 = int(box[0])
             y1 = int(box[1])
             x2 = int(box[2])
             y2 = int(box[3])
 
             if draw_box:
                 image = draw_one_bbox(image, box, cls_color, 1)
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose.py` & `alfred-py-3.0.7/alfred/vis/image/pose.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose_dataset_info.py` & `alfred-py-3.0.7/alfred/vis/image/pose_dataset_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         self.upper_body_ids = []
         self.lower_body_ids = []
 
         self.flip_index_name = []
         self.flip_pairs_name = []
 
         for kid in self.keypoint_info.keys():
-
             keypoint_name = self.keypoint_info[kid]["name"]
             self.keypoint_id2name[kid] = keypoint_name
             self.keypoint_name2id[keypoint_name] = kid
             self.pose_kpt_color.append(
                 self.keypoint_info[kid].get("color", [255, 128, 0])
             )
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose_datasets/animalpose.py` & `alfred-py-3.0.7/alfred/vis/image/pose_datasets/mpii.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,137 @@
 dataset_info = dict(
-    dataset_name='animalpose',
+    dataset_name="mpii",
     paper_info=dict(
-        author='Cao, Jinkun and Tang, Hongyang and Fang, Hao-Shu and '
-        'Shen, Xiaoyong and Lu, Cewu and Tai, Yu-Wing',
-        title='Cross-Domain Adaptation for Animal Pose Estimation',
-        container='The IEEE International Conference on '
-        'Computer Vision (ICCV)',
-        year='2019',
-        homepage='https://sites.google.com/view/animal-pose/',
+        author="Mykhaylo Andriluka and Leonid Pishchulin and "
+        "Peter Gehler and Schiele, Bernt",
+        title="2D Human Pose Estimation: New Benchmark and "
+        "State of the Art Analysis",
+        container="IEEE Conference on Computer Vision and "
+        "Pattern Recognition (CVPR)",
+        year="2014",
+        homepage="http://human-pose.mpi-inf.mpg.de/",
     ),
     keypoint_info={
-        0:
-        dict(
-            name='L_Eye', id=0, color=[0, 255, 0], type='upper', swap='R_Eye'),
-        1:
-        dict(
-            name='R_Eye',
-            id=1,
-            color=[255, 128, 0],
-            type='upper',
-            swap='L_Eye'),
-        2:
-        dict(
-            name='L_EarBase',
-            id=2,
-            color=[0, 255, 0],
-            type='upper',
-            swap='R_EarBase'),
-        3:
-        dict(
-            name='R_EarBase',
-            id=3,
-            color=[255, 128, 0],
-            type='upper',
-            swap='L_EarBase'),
-        4:
-        dict(name='Nose', id=4, color=[51, 153, 255], type='upper', swap=''),
-        5:
-        dict(name='Throat', id=5, color=[51, 153, 255], type='upper', swap=''),
-        6:
-        dict(
-            name='TailBase', id=6, color=[51, 153, 255], type='lower',
-            swap=''),
-        7:
-        dict(
-            name='Withers', id=7, color=[51, 153, 255], type='upper', swap=''),
-        8:
-        dict(
-            name='L_F_Elbow',
-            id=8,
-            color=[0, 255, 0],
-            type='upper',
-            swap='R_F_Elbow'),
-        9:
-        dict(
-            name='R_F_Elbow',
-            id=9,
-            color=[255, 128, 0],
-            type='upper',
-            swap='L_F_Elbow'),
-        10:
-        dict(
-            name='L_B_Elbow',
+        0: dict(
+            name="right_ankle",
+            id=0,
+            color=[255, 128, 0],
+            type="lower",
+            swap="left_ankle",
+        ),
+        1: dict(
+            name="right_knee", id=1, color=[255, 128, 0], type="lower", swap="left_knee"
+        ),
+        2: dict(
+            name="right_hip", id=2, color=[255, 128, 0], type="lower", swap="left_hip"
+        ),
+        3: dict(
+            name="left_hip", id=3, color=[0, 255, 0], type="lower", swap="right_hip"
+        ),
+        4: dict(
+            name="left_knee", id=4, color=[0, 255, 0], type="lower", swap="right_knee"
+        ),
+        5: dict(
+            name="left_ankle", id=5, color=[0, 255, 0], type="lower", swap="right_ankle"
+        ),
+        6: dict(name="pelvis", id=6, color=[51, 153, 255], type="lower", swap=""),
+        7: dict(name="thorax", id=7, color=[51, 153, 255], type="upper", swap=""),
+        8: dict(name="upper_neck", id=8, color=[51, 153, 255], type="upper", swap=""),
+        9: dict(name="head_top", id=9, color=[51, 153, 255], type="upper", swap=""),
+        10: dict(
+            name="right_wrist",
             id=10,
-            color=[0, 255, 0],
-            type='lower',
-            swap='R_B_Elbow'),
-        11:
-        dict(
-            name='R_B_Elbow',
+            color=[255, 128, 0],
+            type="upper",
+            swap="left_wrist",
+        ),
+        11: dict(
+            name="right_elbow",
             id=11,
             color=[255, 128, 0],
-            type='lower',
-            swap='L_B_Elbow'),
-        12:
-        dict(
-            name='L_F_Knee',
+            type="upper",
+            swap="left_elbow",
+        ),
+        12: dict(
+            name="right_shoulder",
             id=12,
-            color=[0, 255, 0],
-            type='upper',
-            swap='R_F_Knee'),
-        13:
-        dict(
-            name='R_F_Knee',
-            id=13,
             color=[255, 128, 0],
-            type='upper',
-            swap='L_F_Knee'),
-        14:
-        dict(
-            name='L_B_Knee',
+            type="upper",
+            swap="left_shoulder",
+        ),
+        13: dict(
+            name="left_shoulder",
+            id=13,
+            color=[0, 255, 0],
+            type="upper",
+            swap="right_shoulder",
+        ),
+        14: dict(
+            name="left_elbow",
             id=14,
             color=[0, 255, 0],
-            type='lower',
-            swap='R_B_Knee'),
-        15:
-        dict(
-            name='R_B_Knee',
+            type="upper",
+            swap="right_elbow",
+        ),
+        15: dict(
+            name="left_wrist",
             id=15,
-            color=[255, 128, 0],
-            type='lower',
-            swap='L_B_Knee'),
-        16:
-        dict(
-            name='L_F_Paw',
-            id=16,
             color=[0, 255, 0],
-            type='upper',
-            swap='R_F_Paw'),
-        17:
-        dict(
-            name='R_F_Paw',
-            id=17,
-            color=[255, 128, 0],
-            type='upper',
-            swap='L_F_Paw'),
-        18:
-        dict(
-            name='L_B_Paw',
-            id=18,
-            color=[0, 255, 0],
-            type='lower',
-            swap='R_B_Paw'),
-        19:
-        dict(
-            name='R_B_Paw',
-            id=19,
-            color=[255, 128, 0],
-            type='lower',
-            swap='L_B_Paw')
+            type="upper",
+            swap="right_wrist",
+        ),
     },
     skeleton_info={
-        0: dict(link=('L_Eye', 'R_Eye'), id=0, color=[51, 153, 255]),
-        1: dict(link=('L_Eye', 'L_EarBase'), id=1, color=[0, 255, 0]),
-        2: dict(link=('R_Eye', 'R_EarBase'), id=2, color=[255, 128, 0]),
-        3: dict(link=('L_Eye', 'Nose'), id=3, color=[0, 255, 0]),
-        4: dict(link=('R_Eye', 'Nose'), id=4, color=[255, 128, 0]),
-        5: dict(link=('Nose', 'Throat'), id=5, color=[51, 153, 255]),
-        6: dict(link=('Throat', 'Withers'), id=6, color=[51, 153, 255]),
-        7: dict(link=('TailBase', 'Withers'), id=7, color=[51, 153, 255]),
-        8: dict(link=('Throat', 'L_F_Elbow'), id=8, color=[0, 255, 0]),
-        9: dict(link=('L_F_Elbow', 'L_F_Knee'), id=9, color=[0, 255, 0]),
-        10: dict(link=('L_F_Knee', 'L_F_Paw'), id=10, color=[0, 255, 0]),
-        11: dict(link=('Throat', 'R_F_Elbow'), id=11, color=[255, 128, 0]),
-        12: dict(link=('R_F_Elbow', 'R_F_Knee'), id=12, color=[255, 128, 0]),
-        13: dict(link=('R_F_Knee', 'R_F_Paw'), id=13, color=[255, 128, 0]),
-        14: dict(link=('TailBase', 'L_B_Elbow'), id=14, color=[0, 255, 0]),
-        15: dict(link=('L_B_Elbow', 'L_B_Knee'), id=15, color=[0, 255, 0]),
-        16: dict(link=('L_B_Knee', 'L_B_Paw'), id=16, color=[0, 255, 0]),
-        17: dict(link=('TailBase', 'R_B_Elbow'), id=17, color=[255, 128, 0]),
-        18: dict(link=('R_B_Elbow', 'R_B_Knee'), id=18, color=[255, 128, 0]),
-        19: dict(link=('R_B_Knee', 'R_B_Paw'), id=19, color=[255, 128, 0])
+        0: dict(link=("right_ankle", "right_knee"), id=0, color=[255, 128, 0]),
+        1: dict(link=("right_knee", "right_hip"), id=1, color=[255, 128, 0]),
+        2: dict(link=("right_hip", "pelvis"), id=2, color=[255, 128, 0]),
+        3: dict(link=("pelvis", "left_hip"), id=3, color=[0, 255, 0]),
+        4: dict(link=("left_hip", "left_knee"), id=4, color=[0, 255, 0]),
+        5: dict(link=("left_knee", "left_ankle"), id=5, color=[0, 255, 0]),
+        6: dict(link=("pelvis", "thorax"), id=6, color=[51, 153, 255]),
+        7: dict(link=("thorax", "upper_neck"), id=7, color=[51, 153, 255]),
+        8: dict(link=("upper_neck", "head_top"), id=8, color=[51, 153, 255]),
+        9: dict(link=("upper_neck", "right_shoulder"), id=9, color=[255, 128, 0]),
+        10: dict(link=("right_shoulder", "right_elbow"), id=10, color=[255, 128, 0]),
+        11: dict(link=("right_elbow", "right_wrist"), id=11, color=[255, 128, 0]),
+        12: dict(link=("upper_neck", "left_shoulder"), id=12, color=[0, 255, 0]),
+        13: dict(link=("left_shoulder", "left_elbow"), id=13, color=[0, 255, 0]),
+        14: dict(link=("left_elbow", "left_wrist"), id=14, color=[0, 255, 0]),
     },
     joint_weights=[
-        1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1., 1.2, 1.2, 1.2, 1.2,
-        1.5, 1.5, 1.5, 1.5
+        1.5,
+        1.2,
+        1.0,
+        1.0,
+        1.2,
+        1.5,
+        1.0,
+        1.0,
+        1.0,
+        1.0,
+        1.5,
+        1.2,
+        1.0,
+        1.0,
+        1.2,
+        1.5,
     ],
-
-    # Note: The original paper did not provide enough information about
-    # the sigmas. We modified from 'https://github.com/cocodataset/'
-    # 'cocoapi/blob/master/PythonAPI/pycocotools/cocoeval.py#L523'
+    # Adapted from COCO dataset.
     sigmas=[
-        0.025, 0.025, 0.026, 0.035, 0.035, 0.10, 0.10, 0.10, 0.107, 0.107,
-        0.107, 0.107, 0.087, 0.087, 0.087, 0.087, 0.089, 0.089, 0.089, 0.089
-    ])
+        0.089,
+        0.083,
+        0.107,
+        0.107,
+        0.083,
+        0.089,
+        0.026,
+        0.026,
+        0.026,
+        0.026,
+        0.062,
+        0.072,
+        0.179,
+        0.179,
+        0.072,
+        0.062,
+    ],
+)
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose_datasets/coco_wholebody_hand.py` & `alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco_wholebody_hand.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,85 @@
 dataset_info = dict(
-    dataset_name='coco_wholebody_hand',
+    dataset_name="coco_wholebody_hand",
     paper_info=dict(
-        author='Jin, Sheng and Xu, Lumin and Xu, Jin and '
-        'Wang, Can and Liu, Wentao and '
-        'Qian, Chen and Ouyang, Wanli and Luo, Ping',
-        title='Whole-Body Human Pose Estimation in the Wild',
-        container='Proceedings of the European '
-        'Conference on Computer Vision (ECCV)',
-        year='2020',
-        homepage='https://github.com/jin-s13/COCO-WholeBody/',
+        author="Jin, Sheng and Xu, Lumin and Xu, Jin and "
+        "Wang, Can and Liu, Wentao and "
+        "Qian, Chen and Ouyang, Wanli and Luo, Ping",
+        title="Whole-Body Human Pose Estimation in the Wild",
+        container="Proceedings of the European " "Conference on Computer Vision (ECCV)",
+        year="2020",
+        homepage="https://github.com/jin-s13/COCO-WholeBody/",
     ),
     keypoint_info={
-        0:
-        dict(name='wrist', id=0, color=[255, 255, 255], type='', swap=''),
-        1:
-        dict(name='thumb1', id=1, color=[255, 128, 0], type='', swap=''),
-        2:
-        dict(name='thumb2', id=2, color=[255, 128, 0], type='', swap=''),
-        3:
-        dict(name='thumb3', id=3, color=[255, 128, 0], type='', swap=''),
-        4:
-        dict(name='thumb4', id=4, color=[255, 128, 0], type='', swap=''),
-        5:
-        dict(
-            name='forefinger1', id=5, color=[255, 153, 255], type='', swap=''),
-        6:
-        dict(
-            name='forefinger2', id=6, color=[255, 153, 255], type='', swap=''),
-        7:
-        dict(
-            name='forefinger3', id=7, color=[255, 153, 255], type='', swap=''),
-        8:
-        dict(
-            name='forefinger4', id=8, color=[255, 153, 255], type='', swap=''),
-        9:
-        dict(
-            name='middle_finger1',
-            id=9,
-            color=[102, 178, 255],
-            type='',
-            swap=''),
-        10:
-        dict(
-            name='middle_finger2',
-            id=10,
-            color=[102, 178, 255],
-            type='',
-            swap=''),
-        11:
-        dict(
-            name='middle_finger3',
-            id=11,
-            color=[102, 178, 255],
-            type='',
-            swap=''),
-        12:
-        dict(
-            name='middle_finger4',
-            id=12,
-            color=[102, 178, 255],
-            type='',
-            swap=''),
-        13:
-        dict(
-            name='ring_finger1', id=13, color=[255, 51, 51], type='', swap=''),
-        14:
-        dict(
-            name='ring_finger2', id=14, color=[255, 51, 51], type='', swap=''),
-        15:
-        dict(
-            name='ring_finger3', id=15, color=[255, 51, 51], type='', swap=''),
-        16:
-        dict(
-            name='ring_finger4', id=16, color=[255, 51, 51], type='', swap=''),
-        17:
-        dict(name='pinky_finger1', id=17, color=[0, 255, 0], type='', swap=''),
-        18:
-        dict(name='pinky_finger2', id=18, color=[0, 255, 0], type='', swap=''),
-        19:
-        dict(name='pinky_finger3', id=19, color=[0, 255, 0], type='', swap=''),
-        20:
-        dict(name='pinky_finger4', id=20, color=[0, 255, 0], type='', swap='')
+        0: dict(name="wrist", id=0, color=[255, 255, 255], type="", swap=""),
+        1: dict(name="thumb1", id=1, color=[255, 128, 0], type="", swap=""),
+        2: dict(name="thumb2", id=2, color=[255, 128, 0], type="", swap=""),
+        3: dict(name="thumb3", id=3, color=[255, 128, 0], type="", swap=""),
+        4: dict(name="thumb4", id=4, color=[255, 128, 0], type="", swap=""),
+        5: dict(name="forefinger1", id=5, color=[255, 153, 255], type="", swap=""),
+        6: dict(name="forefinger2", id=6, color=[255, 153, 255], type="", swap=""),
+        7: dict(name="forefinger3", id=7, color=[255, 153, 255], type="", swap=""),
+        8: dict(name="forefinger4", id=8, color=[255, 153, 255], type="", swap=""),
+        9: dict(name="middle_finger1", id=9, color=[102, 178, 255], type="", swap=""),
+        10: dict(name="middle_finger2", id=10, color=[102, 178, 255], type="", swap=""),
+        11: dict(name="middle_finger3", id=11, color=[102, 178, 255], type="", swap=""),
+        12: dict(name="middle_finger4", id=12, color=[102, 178, 255], type="", swap=""),
+        13: dict(name="ring_finger1", id=13, color=[255, 51, 51], type="", swap=""),
+        14: dict(name="ring_finger2", id=14, color=[255, 51, 51], type="", swap=""),
+        15: dict(name="ring_finger3", id=15, color=[255, 51, 51], type="", swap=""),
+        16: dict(name="ring_finger4", id=16, color=[255, 51, 51], type="", swap=""),
+        17: dict(name="pinky_finger1", id=17, color=[0, 255, 0], type="", swap=""),
+        18: dict(name="pinky_finger2", id=18, color=[0, 255, 0], type="", swap=""),
+        19: dict(name="pinky_finger3", id=19, color=[0, 255, 0], type="", swap=""),
+        20: dict(name="pinky_finger4", id=20, color=[0, 255, 0], type="", swap=""),
     },
     skeleton_info={
-        0:
-        dict(link=('wrist', 'thumb1'), id=0, color=[255, 128, 0]),
-        1:
-        dict(link=('thumb1', 'thumb2'), id=1, color=[255, 128, 0]),
-        2:
-        dict(link=('thumb2', 'thumb3'), id=2, color=[255, 128, 0]),
-        3:
-        dict(link=('thumb3', 'thumb4'), id=3, color=[255, 128, 0]),
-        4:
-        dict(link=('wrist', 'forefinger1'), id=4, color=[255, 153, 255]),
-        5:
-        dict(link=('forefinger1', 'forefinger2'), id=5, color=[255, 153, 255]),
-        6:
-        dict(link=('forefinger2', 'forefinger3'), id=6, color=[255, 153, 255]),
-        7:
-        dict(link=('forefinger3', 'forefinger4'), id=7, color=[255, 153, 255]),
-        8:
-        dict(link=('wrist', 'middle_finger1'), id=8, color=[102, 178, 255]),
-        9:
-        dict(
-            link=('middle_finger1', 'middle_finger2'),
-            id=9,
-            color=[102, 178, 255]),
-        10:
-        dict(
-            link=('middle_finger2', 'middle_finger3'),
-            id=10,
-            color=[102, 178, 255]),
-        11:
-        dict(
-            link=('middle_finger3', 'middle_finger4'),
-            id=11,
-            color=[102, 178, 255]),
-        12:
-        dict(link=('wrist', 'ring_finger1'), id=12, color=[255, 51, 51]),
-        13:
-        dict(
-            link=('ring_finger1', 'ring_finger2'), id=13, color=[255, 51, 51]),
-        14:
-        dict(
-            link=('ring_finger2', 'ring_finger3'), id=14, color=[255, 51, 51]),
-        15:
-        dict(
-            link=('ring_finger3', 'ring_finger4'), id=15, color=[255, 51, 51]),
-        16:
-        dict(link=('wrist', 'pinky_finger1'), id=16, color=[0, 255, 0]),
-        17:
-        dict(
-            link=('pinky_finger1', 'pinky_finger2'), id=17, color=[0, 255, 0]),
-        18:
-        dict(
-            link=('pinky_finger2', 'pinky_finger3'), id=18, color=[0, 255, 0]),
-        19:
-        dict(
-            link=('pinky_finger3', 'pinky_finger4'), id=19, color=[0, 255, 0])
+        0: dict(link=("wrist", "thumb1"), id=0, color=[255, 128, 0]),
+        1: dict(link=("thumb1", "thumb2"), id=1, color=[255, 128, 0]),
+        2: dict(link=("thumb2", "thumb3"), id=2, color=[255, 128, 0]),
+        3: dict(link=("thumb3", "thumb4"), id=3, color=[255, 128, 0]),
+        4: dict(link=("wrist", "forefinger1"), id=4, color=[255, 153, 255]),
+        5: dict(link=("forefinger1", "forefinger2"), id=5, color=[255, 153, 255]),
+        6: dict(link=("forefinger2", "forefinger3"), id=6, color=[255, 153, 255]),
+        7: dict(link=("forefinger3", "forefinger4"), id=7, color=[255, 153, 255]),
+        8: dict(link=("wrist", "middle_finger1"), id=8, color=[102, 178, 255]),
+        9: dict(link=("middle_finger1", "middle_finger2"), id=9, color=[102, 178, 255]),
+        10: dict(
+            link=("middle_finger2", "middle_finger3"), id=10, color=[102, 178, 255]
+        ),
+        11: dict(
+            link=("middle_finger3", "middle_finger4"), id=11, color=[102, 178, 255]
+        ),
+        12: dict(link=("wrist", "ring_finger1"), id=12, color=[255, 51, 51]),
+        13: dict(link=("ring_finger1", "ring_finger2"), id=13, color=[255, 51, 51]),
+        14: dict(link=("ring_finger2", "ring_finger3"), id=14, color=[255, 51, 51]),
+        15: dict(link=("ring_finger3", "ring_finger4"), id=15, color=[255, 51, 51]),
+        16: dict(link=("wrist", "pinky_finger1"), id=16, color=[0, 255, 0]),
+        17: dict(link=("pinky_finger1", "pinky_finger2"), id=17, color=[0, 255, 0]),
+        18: dict(link=("pinky_finger2", "pinky_finger3"), id=18, color=[0, 255, 0]),
+        19: dict(link=("pinky_finger3", "pinky_finger4"), id=19, color=[0, 255, 0]),
     },
-    joint_weights=[1.] * 21,
+    joint_weights=[1.0] * 21,
     sigmas=[
-        0.029, 0.022, 0.035, 0.037, 0.047, 0.026, 0.025, 0.024, 0.035, 0.018,
-        0.024, 0.022, 0.026, 0.017, 0.021, 0.021, 0.032, 0.02, 0.019, 0.022,
-        0.031
-    ])
+        0.029,
+        0.022,
+        0.035,
+        0.037,
+        0.047,
+        0.026,
+        0.025,
+        0.024,
+        0.035,
+        0.018,
+        0.024,
+        0.022,
+        0.026,
+        0.017,
+        0.021,
+        0.021,
+        0.032,
+        0.02,
+        0.019,
+        0.022,
+        0.031,
+    ],
+)
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose_datasets/mpii.py` & `alfred-py-3.0.7/alfred/vis/image/pose_datasets/coco.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,155 +1,151 @@
 dataset_info = dict(
-    dataset_name='mpii',
+    dataset_name="coco",
     paper_info=dict(
-        author='Mykhaylo Andriluka and Leonid Pishchulin and '
-        'Peter Gehler and Schiele, Bernt',
-        title='2D Human Pose Estimation: New Benchmark and '
-        'State of the Art Analysis',
-        container='IEEE Conference on Computer Vision and '
-        'Pattern Recognition (CVPR)',
-        year='2014',
-        homepage='http://human-pose.mpi-inf.mpg.de/',
+        author="Lin, Tsung-Yi and Maire, Michael and "
+        "Belongie, Serge and Hays, James and "
+        "Perona, Pietro and Ramanan, Deva and "
+        r"Doll{\'a}r, Piotr and Zitnick, C Lawrence",
+        title="Microsoft coco: Common objects in context",
+        container="European conference on computer vision",
+        year="2014",
+        homepage="http://cocodataset.org/",
     ),
     keypoint_info={
-        0:
-        dict(
-            name='right_ankle',
-            id=0,
-            color=[255, 128, 0],
-            type='lower',
-            swap='left_ankle'),
-        1:
-        dict(
-            name='right_knee',
-            id=1,
-            color=[255, 128, 0],
-            type='lower',
-            swap='left_knee'),
-        2:
-        dict(
-            name='right_hip',
-            id=2,
-            color=[255, 128, 0],
-            type='lower',
-            swap='left_hip'),
-        3:
-        dict(
-            name='left_hip',
-            id=3,
-            color=[0, 255, 0],
-            type='lower',
-            swap='right_hip'),
-        4:
-        dict(
-            name='left_knee',
-            id=4,
-            color=[0, 255, 0],
-            type='lower',
-            swap='right_knee'),
-        5:
-        dict(
-            name='left_ankle',
+        0: dict(name="nose", id=0, color=[51, 153, 255], type="upper", swap=""),
+        1: dict(
+            name="left_eye", id=1, color=[51, 153, 255], type="upper", swap="right_eye"
+        ),
+        2: dict(
+            name="right_eye", id=2, color=[51, 153, 255], type="upper", swap="left_eye"
+        ),
+        3: dict(
+            name="left_ear", id=3, color=[51, 153, 255], type="upper", swap="right_ear"
+        ),
+        4: dict(
+            name="right_ear", id=4, color=[51, 153, 255], type="upper", swap="left_ear"
+        ),
+        5: dict(
+            name="left_shoulder",
             id=5,
             color=[0, 255, 0],
-            type='lower',
-            swap='right_ankle'),
-        6:
-        dict(name='pelvis', id=6, color=[51, 153, 255], type='lower', swap=''),
-        7:
-        dict(name='thorax', id=7, color=[51, 153, 255], type='upper', swap=''),
-        8:
-        dict(
-            name='upper_neck',
+            type="upper",
+            swap="right_shoulder",
+        ),
+        6: dict(
+            name="right_shoulder",
+            id=6,
+            color=[255, 128, 0],
+            type="upper",
+            swap="left_shoulder",
+        ),
+        7: dict(
+            name="left_elbow", id=7, color=[0, 255, 0], type="upper", swap="right_elbow"
+        ),
+        8: dict(
+            name="right_elbow",
             id=8,
-            color=[51, 153, 255],
-            type='upper',
-            swap=''),
-        9:
-        dict(
-            name='head_top', id=9, color=[51, 153, 255], type='upper',
-            swap=''),
-        10:
-        dict(
-            name='right_wrist',
-            id=10,
             color=[255, 128, 0],
-            type='upper',
-            swap='left_wrist'),
-        11:
-        dict(
-            name='right_elbow',
-            id=11,
-            color=[255, 128, 0],
-            type='upper',
-            swap='left_elbow'),
-        12:
-        dict(
-            name='right_shoulder',
-            id=12,
+            type="upper",
+            swap="left_elbow",
+        ),
+        9: dict(
+            name="left_wrist", id=9, color=[0, 255, 0], type="upper", swap="right_wrist"
+        ),
+        10: dict(
+            name="right_wrist",
+            id=10,
             color=[255, 128, 0],
-            type='upper',
-            swap='left_shoulder'),
-        13:
-        dict(
-            name='left_shoulder',
-            id=13,
-            color=[0, 255, 0],
-            type='upper',
-            swap='right_shoulder'),
-        14:
-        dict(
-            name='left_elbow',
+            type="upper",
+            swap="left_wrist",
+        ),
+        11: dict(
+            name="left_hip", id=11, color=[0, 255, 0], type="lower", swap="right_hip"
+        ),
+        12: dict(
+            name="right_hip", id=12, color=[255, 128, 0], type="lower", swap="left_hip"
+        ),
+        13: dict(
+            name="left_knee", id=13, color=[0, 255, 0], type="lower", swap="right_knee"
+        ),
+        14: dict(
+            name="right_knee",
             id=14,
-            color=[0, 255, 0],
-            type='upper',
-            swap='right_elbow'),
-        15:
-        dict(
-            name='left_wrist',
+            color=[255, 128, 0],
+            type="lower",
+            swap="left_knee",
+        ),
+        15: dict(
+            name="left_ankle",
             id=15,
             color=[0, 255, 0],
-            type='upper',
-            swap='right_wrist')
+            type="lower",
+            swap="right_ankle",
+        ),
+        16: dict(
+            name="right_ankle",
+            id=16,
+            color=[255, 128, 0],
+            type="lower",
+            swap="left_ankle",
+        ),
     },
     skeleton_info={
-        0:
-        dict(link=('right_ankle', 'right_knee'), id=0, color=[255, 128, 0]),
-        1:
-        dict(link=('right_knee', 'right_hip'), id=1, color=[255, 128, 0]),
-        2:
-        dict(link=('right_hip', 'pelvis'), id=2, color=[255, 128, 0]),
-        3:
-        dict(link=('pelvis', 'left_hip'), id=3, color=[0, 255, 0]),
-        4:
-        dict(link=('left_hip', 'left_knee'), id=4, color=[0, 255, 0]),
-        5:
-        dict(link=('left_knee', 'left_ankle'), id=5, color=[0, 255, 0]),
-        6:
-        dict(link=('pelvis', 'thorax'), id=6, color=[51, 153, 255]),
-        7:
-        dict(link=('thorax', 'upper_neck'), id=7, color=[51, 153, 255]),
-        8:
-        dict(link=('upper_neck', 'head_top'), id=8, color=[51, 153, 255]),
-        9:
-        dict(link=('upper_neck', 'right_shoulder'), id=9, color=[255, 128, 0]),
-        10:
-        dict(
-            link=('right_shoulder', 'right_elbow'), id=10, color=[255, 128,
-                                                                  0]),
-        11:
-        dict(link=('right_elbow', 'right_wrist'), id=11, color=[255, 128, 0]),
-        12:
-        dict(link=('upper_neck', 'left_shoulder'), id=12, color=[0, 255, 0]),
-        13:
-        dict(link=('left_shoulder', 'left_elbow'), id=13, color=[0, 255, 0]),
-        14:
-        dict(link=('left_elbow', 'left_wrist'), id=14, color=[0, 255, 0])
+        0: dict(link=("left_ankle", "left_knee"), id=0, color=[0, 255, 0]),
+        1: dict(link=("left_knee", "left_hip"), id=1, color=[0, 255, 0]),
+        2: dict(link=("right_ankle", "right_knee"), id=2, color=[255, 128, 0]),
+        3: dict(link=("right_knee", "right_hip"), id=3, color=[255, 128, 0]),
+        4: dict(link=("left_hip", "right_hip"), id=4, color=[51, 153, 255]),
+        5: dict(link=("left_shoulder", "left_hip"), id=5, color=[51, 153, 255]),
+        6: dict(link=("right_shoulder", "right_hip"), id=6, color=[51, 153, 255]),
+        7: dict(link=("left_shoulder", "right_shoulder"), id=7, color=[51, 153, 255]),
+        8: dict(link=("left_shoulder", "left_elbow"), id=8, color=[0, 255, 0]),
+        9: dict(link=("right_shoulder", "right_elbow"), id=9, color=[255, 128, 0]),
+        10: dict(link=("left_elbow", "left_wrist"), id=10, color=[0, 255, 0]),
+        11: dict(link=("right_elbow", "right_wrist"), id=11, color=[255, 128, 0]),
+        12: dict(link=("left_eye", "right_eye"), id=12, color=[51, 153, 255]),
+        13: dict(link=("nose", "left_eye"), id=13, color=[51, 153, 255]),
+        14: dict(link=("nose", "right_eye"), id=14, color=[51, 153, 255]),
+        15: dict(link=("left_eye", "left_ear"), id=15, color=[51, 153, 255]),
+        16: dict(link=("right_eye", "right_ear"), id=16, color=[51, 153, 255]),
+        17: dict(link=("left_ear", "left_shoulder"), id=17, color=[51, 153, 255]),
+        18: dict(link=("right_ear", "right_shoulder"), id=18, color=[51, 153, 255]),
     },
     joint_weights=[
-        1.5, 1.2, 1., 1., 1.2, 1.5, 1., 1., 1., 1., 1.5, 1.2, 1., 1., 1.2, 1.5
+        1.0,
+        1.0,
+        1.0,
+        1.0,
+        1.0,
+        1.0,
+        1.0,
+        1.2,
+        1.2,
+        1.5,
+        1.5,
+        1.0,
+        1.0,
+        1.2,
+        1.2,
+        1.5,
+        1.5,
     ],
-    # Adapted from COCO dataset.
     sigmas=[
-        0.089, 0.083, 0.107, 0.107, 0.083, 0.089, 0.026, 0.026, 0.026, 0.026,
-        0.062, 0.072, 0.179, 0.179, 0.072, 0.062
-    ])
+        0.026,
+        0.025,
+        0.025,
+        0.035,
+        0.035,
+        0.079,
+        0.079,
+        0.072,
+        0.072,
+        0.062,
+        0.062,
+        0.107,
+        0.107,
+        0.087,
+        0.087,
+        0.089,
+        0.089,
+    ],
+)
```

### Comparing `alfred-py-3.0.6/alfred/vis/image/pose_hand.py` & `alfred-py-3.0.7/alfred/vis/image/pose_hand.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/image/seg.py` & `alfred-py-3.0.7/alfred/vis/image/seg.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,40 +30,50 @@
 import numpy as np
 import cv2
 from .get_dataset_color_map import label_to_color_image
 from .get_dataset_color_map import _ADE20K, _CITYSCAPES, _MAPILLARY_VISTAS, _PASCAL
 
 from .mask import label2color_mask
 
-def vis_semantic_seg(img, seg, alpha=0.7, override_colormap=None, color_suite='cityscapes', is_show=False):
-    mask_color = label2color_mask(seg, override_id_clr_map=override_colormap, color_suit=color_suite)
+
+def vis_semantic_seg(
+    img, seg, alpha=0.7, override_colormap=None, color_suite="cityscapes", is_show=False
+):
+    mask_color = label2color_mask(
+        seg, override_id_clr_map=override_colormap, color_suit=color_suite
+    )
     img_shape = img.shape
     mask_shape = mask_color.shape
     if img_shape != mask_shape:
         # resize mask to img shape
         mask_color = cv2.resize(mask_color, (img.shape[1], img.shape[0]))
 
     res = cv2.addWeighted(img, 0.5, mask_color, alpha, 0.4)
     if is_show:
-        cv2.imshow('result', res)
+        cv2.imshow("result", res)
         cv2.waitKey(0)
     return res, mask_color
 
 
 def draw_seg_by_dataset(img, seg, dataset, alpha=0.7, is_show=False, bgr_in=False):
-    assert dataset in [_PASCAL, _CITYSCAPES, _MAPILLARY_VISTAS, _ADE20K], 'dataset not support yet.'
+    assert dataset in [
+        _PASCAL,
+        _CITYSCAPES,
+        _MAPILLARY_VISTAS,
+        _ADE20K,
+    ], "dataset not support yet."
     img = np.asarray(img, dtype=np.uint8)
     if bgr_in:
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
     mask_color = np.asarray(label_to_color_image(seg, dataset), dtype=np.uint8)
     img_shape = img.shape
     mask_shape = mask_color.shape
     if img_shape != mask_shape:
         # resize mask to img shape
         mask_color = cv2.resize(mask_color, (img.shape[1], img.shape[0]))
 
     res = cv2.addWeighted(img, 0.3, mask_color, alpha, 0.6)
     if is_show:
-        cv2.imshow('result', res)
+        cv2.imshow("result", res)
         cv2.waitKey(0)
     return res, mask_color
```

### Comparing `alfred-py-3.0.6/alfred/vis/mesh3d/o3dsocket.py` & `alfred-py-3.0.7/alfred/vis/mesh3d/o3dsocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from traceback import print_tb
 import open3d as o3d
 from .o3dwrapper import Vector3dVector, create_mesh, load_mesh
 from .utils import Timer
 from .utils import BaseSocket, log
 import json
 import numpy as np
@@ -25,101 +24,94 @@
 
 
 class VisOpen3DSocket(BaseSocket):
     def __init__(self, cfg=None) -> None:
         if cfg is None:
             crt_dir = os.path.dirname(__file__)
             cfg = DefaultConfig.load(
-                filename=os.path.join(crt_dir, 'default_viscfg.yml'))
+                filename=os.path.join(crt_dir, "default_viscfg.yml")
+            )
         # output
         host = cfg.host
         port = cfg.port
 
         self.write = cfg.write
         self.out = cfg.out
         self.cfg = cfg
         if self.write:
-            print('[Info] capture the screen to {}'.format(self.out))
+            print("[Info] capture the screen to {}".format(self.out))
             os.makedirs(self.out, exist_ok=True)
         # scene
         vis = o3d.visualization.VisualizerWithKeyCallback()
-        vis.register_key_callback(ord('A'), o3d_callback_rotate)
-        vis.create_window(window_name='Visualizer',
-                          width=cfg.width, height=cfg.height)
+        vis.register_key_callback(ord("A"), o3d_callback_rotate)
+        vis.create_window(window_name="Visualizer", width=cfg.width, height=cfg.height)
         self.vis = vis
         # load the scene
         for sc in cfg.scene:
-            key = sc['module']
-            mesh_args = sc['args']
+            key = sc["module"]
+            mesh_args = sc["args"]
             mesh = load_object(key, mesh_args)
             self.vis.add_geometry(mesh)
 
         for key, val in cfg.extra.items():
             mesh = load_mesh(val["path"])
-            trans = np.array(val['transform']).reshape(4, 4)
+            trans = np.array(val["transform"]).reshape(4, 4)
             mesh.transform(trans)
             self.vis.add_geometry(mesh)
         # create vis => update => super() init
         super().__init__(host, port, debug=cfg.debug)
         self.block = cfg.block
         if os.path.exists(cfg.body_model_template):
             body_template = o3d.io.read_triangle_mesh(cfg.body_model_template)
             self.body_template = body_template
         else:
             self.body_template = None
-        self.body_model = load_object(
-            cfg.body_model.module, cfg.body_model.args)
+        self.body_model = load_object(cfg.body_model.module, cfg.body_model.args)
         zero_params = self.body_model.init_params(1)
         self.max_human = cfg.max_human
         self.track = cfg.track
         self.filter = cfg.filter
         self.camera_pose = cfg.camera.camera_pose
         self.init_camera(cfg.camera.camera_pose)
-        self.zero_vertices = Vector3dVector(
-            np.zeros((self.body_model.nVertices, 3)))
+        self.zero_vertices = Vector3dVector(np.zeros((self.body_model.nVertices, 3)))
 
         self.vertices, self.meshes = [], []
         for i in range(self.max_human):
             self.add_human(zero_params)
 
         self.count = 0
         self.previous = {}
         self.critrange = CritRange(**cfg.range)
         self.new_frames = cfg.new_frames
 
     def add_human(self, zero_params):
         vertices = self.body_model(
-            return_verts=True, return_tensor=False, **zero_params)[0]
+            return_verts=True, return_tensor=False, **zero_params
+        )[0]
         self.vertices.append(vertices)
         if self.body_template is None:  # create template
             mesh = create_mesh(
-                vertices=vertices, faces=self.body_model.faces, colors=self.body_model.color)
+                vertices=vertices,
+                faces=self.body_model.faces,
+                colors=self.body_model.color,
+            )
         else:
             mesh = copy.deepcopy(self.body_template)
         self.meshes.append(mesh)
         self.vis.add_geometry(mesh)
         self.init_camera(self.camera_pose)
 
     @staticmethod
     def set_camera(cfg, camera_pose):
-        theta, phi = np.deg2rad(-(cfg.camera.theta + 90)
-                                ), np.deg2rad(cfg.camera.phi)
+        theta, phi = np.deg2rad(-(cfg.camera.theta + 90)), np.deg2rad(cfg.camera.phi)
         theta = theta + np.pi
         st, ct = np.sin(theta), np.cos(theta)
         sp, cp = np.sin(phi), np.cos(phi)
-        rot_x = np.array([
-            [1., 0., 0.],
-            [0., ct, -st],
-            [0, st, ct]
-        ])
-        rot_z = np.array([
-            [cp, -sp, 0],
-            [sp, cp, 0.],
-            [0., 0., 1.]
-        ])
+        rot_x = np.array([[1.0, 0.0, 0.0], [0.0, ct, -st], [0, st, ct]])
+        rot_z = np.array([[cp, -sp, 0], [sp, cp, 0.0], [0.0, 0.0, 1.0]])
         camera_pose[:3, :3] = rot_x @ rot_z
         return camera_pose
 
     def init_camera(self, camera_pose):
         ctr = self.vis.get_view_control()
         init_param = ctr.convert_to_pinhole_camera_parameters()
         # init_param.intrinsic.set_intrinsics(init_param.intrinsic.width, init_param.intrinsic.height, fx, fy, cx, cy)
@@ -130,98 +122,99 @@
         ctr = self.vis.get_view_control()
         init_param = ctr.convert_to_pinhole_camera_parameters()
         return np.array(init_param.extrinsic)
 
     def filter_human(self, datas):
         datas_new = []
         for data in datas:
-            kpts3d = np.array(data['keypoints3d'])
-            data['keypoints3d'] = kpts3d
-            pid = data['id']
+            kpts3d = np.array(data["keypoints3d"])
+            data["keypoints3d"] = kpts3d
+            pid = data["id"]
             if pid not in self.previous.keys():
                 if not self.critrange(kpts3d):
                     continue
                 self.previous[pid] = 0
             self.previous[pid] += 1
             if self.previous[pid] > self.new_frames:
                 datas_new.append(data)
         return datas_new
 
     def main(self, datas):
         if self.debug:
-            log('[Info] Load data {}'.format(self.count))
+            log("[Info] Load data {}".format(self.count))
         if isinstance(datas, str):
             datas = json.loads(datas)
         print(datas)
         for data in datas:
             for key in data.keys():
-                if key == 'id':
+                if key == "id":
                     continue
                 data[key] = np.array(data[key])
-            if 'keypoints3d' not in data.keys() and self.filter:
-                data['keypoints3d'] = self.body_model(
-                    return_verts=False, return_tensor=False, **data)[0]
+            if "keypoints3d" not in data.keys() and self.filter:
+                data["keypoints3d"] = self.body_model(
+                    return_verts=False, return_tensor=False, **data
+                )[0]
         if self.filter:
             datas = self.filter_human(datas)
-        with Timer('forward'):
+        with Timer("forward"):
             params = []
             for i, data in enumerate(datas):
                 if i >= len(self.meshes):
-                    print('[Error] the number of human exceeds!')
+                    print("[Error] the number of human exceeds!")
                     self.add_human(data)
-                if 'vertices' in data.keys():
-                    vertices = data['vertices']
+                if "vertices" in data.keys():
+                    vertices = data["vertices"]
                     self.vertices[i] = Vector3dVector(vertices)
                 else:
                     params.append(data)
             if len(params) > 0:
-                params = self.body_model.merge_params(
-                    params, share_shape=False)
+                params = self.body_model.merge_params(params, share_shape=False)
                 vertices = self.body_model(
-                    return_verts=True, return_tensor=False, **params)
+                    return_verts=True, return_tensor=False, **params
+                )
                 for i in range(vertices.shape[0]):
                     self.vertices[i] = Vector3dVector(vertices[i])
             for i in range(len(datas), len(self.meshes)):
                 self.vertices[i] = self.zero_vertices
         # Open3D will lock the thread here
-        with Timer('set vertices'):
+        with Timer("set vertices"):
             for i in range(len(self.vertices)):
                 self.meshes[i].vertices = self.vertices[i]
                 if i < len(datas) and self.track:
-                    col = get_rgb_01(datas[i]['id'])
+                    col = get_rgb_01(datas[i]["id"])
                     self.meshes[i].paint_uniform_color(col)
-        print('verts done.')
+        print("verts done.")
 
     def o3dcallback(self):
         if rotate:
-            self.cfg.camera.phi += np.pi/10
+            self.cfg.camera.phi += np.pi / 10
             camera_pose = self.set_camera(self.cfg, self.get_camera())
             self.init_camera(camera_pose)
 
     def update(self):
         if self.disconnect and not self.block:
             self.previous.clear()
         if not self.queue.empty():
             if self.debug:
-                log('Update' + str(self.queue.qsize()))
+                log("Update" + str(self.queue.qsize()))
             datas = self.queue.get()
             if not self.block:
                 while self.queue.qsize() > 0:
                     datas = self.queue.get()
             self.main(datas)
-            with Timer('update geometry'):
+            with Timer("update geometry"):
                 for mesh in self.meshes:
                     mesh.compute_triangle_normals()
                     self.vis.update_geometry(mesh)
                 self.o3dcallback()
                 self.vis.poll_events()
                 self.vis.update_renderer()
             if self.write:
-                outname = join(self.out, '{:06d}.jpg'.format(self.count))
-                with Timer('capture'):
+                outname = join(self.out, "{:06d}.jpg".format(self.count))
+                with Timer("capture"):
                     self.vis.capture_screen_image(outname)
             self.count += 1
         else:
-            with Timer('update renderer', True):
+            with Timer("update renderer", True):
                 self.o3dcallback()
                 self.vis.poll_events()
                 self.vis.update_renderer()
```

### Comparing `alfred-py-3.0.6/alfred/vis/mesh3d/skelmodel.py` & `alfred-py-3.0.7/alfred/vis/mesh3d/skelmodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,144 +1,161 @@
-
 import numpy as np
 import cv2
 from os.path import join
 import os
 from .o3d_visconfig import CONFIG
 from alfred.utils.log import logger
 
 
 def calTransformation(v_i, v_j, r, adaptr=False, ratio=10):
-    """ from to vertices to T
+    """from to vertices to T
 
     Arguments:
         v_i {} -- [description]
         v_j {[type]} -- [description]
     """
     xaxis = np.array([1, 0, 0])
-    v = (v_i + v_j)/2
-    direc = (v_i - v_j)
+    v = (v_i + v_j) / 2
+    direc = v_i - v_j
     length = np.linalg.norm(direc)
-    direc = direc/length
+    direc = direc / length
     rotdir = np.cross(xaxis, direc)
     if np.linalg.norm(rotdir) > 1e-3:
-        rotdir = rotdir/np.linalg.norm(rotdir)
+        rotdir = rotdir / np.linalg.norm(rotdir)
         rotdir = rotdir * np.arccos(np.dot(direc, xaxis))
         rotmat, _ = cv2.Rodrigues(rotdir)
     else:
         rotmat = np.eye(3)
     # set the minimal radius for the finger and face
-    shrink = min(max(length/ratio, 0.005), 0.05)
-    eigval = np.array([[length/2/r, 0, 0], [0, shrink, 0], [0, 0, shrink]])
+    shrink = min(max(length / ratio, 0.005), 0.05)
+    eigval = np.array([[length / 2 / r, 0, 0], [0, shrink, 0], [0, 0, shrink]])
     T = np.eye(4)
     T[:3, :3] = rotmat @ eigval @ rotmat.T
     T[:3, 3] = v
     return T, r, length
 
 
 class SkelModel:
-    def __init__(self, nJoints=None, kintree=None, body_type=None, joint_radius=0.02, res=20, **kwargs) -> None:
+    def __init__(
+        self,
+        nJoints=None,
+        kintree=None,
+        body_type=None,
+        joint_radius=0.02,
+        res=20,
+        **kwargs,
+    ) -> None:
         if nJoints is not None:
             self.nJoints = nJoints
             self.kintree = kintree
         else:
             config = CONFIG[body_type]
-            self.nJoints = config['nJoints']
-            self.kintree = config['kintree']
+            self.nJoints = config["nJoints"]
+            self.kintree = config["kintree"]
         self.body_type = body_type
-        self.device = 'none'
+        self.device = "none"
         cur_dir = os.path.dirname(__file__)
         faces = np.loadtxt(
-            join(cur_dir, 'assets', 'sphere_faces_{}.txt'.format(res)), dtype=np.int)
+            join(cur_dir, "assets", "sphere_faces_{}.txt".format(res)), dtype=np.int
+        )
         self.vertices = np.loadtxt(
-            join(cur_dir, 'assets', 'sphere_vertices_{}.txt'.format(res)))
+            join(cur_dir, "assets", "sphere_vertices_{}.txt".format(res))
+        )
         # compose faces
         faces_all = []
         for nj in range(self.nJoints):
-            faces_all.append(faces + nj*self.vertices.shape[0])
+            faces_all.append(faces + nj * self.vertices.shape[0])
         for nk in range(len(self.kintree)):
-            faces_all.append(faces + self.nJoints *
-                             self.vertices.shape[0] + nk*self.vertices.shape[0])
+            faces_all.append(
+                faces
+                + self.nJoints * self.vertices.shape[0]
+                + nk * self.vertices.shape[0]
+            )
         self.faces = np.vstack(faces_all)
         self.color = None
-        self.nVertices = self.vertices.shape[0] * self.nJoints + \
-            self.vertices.shape[0] * len(self.kintree)
+        self.nVertices = self.vertices.shape[0] * self.nJoints + self.vertices.shape[
+            0
+        ] * len(self.kintree)
         self.joint_radius = joint_radius
 
-    def __call__(self, keypoints3d, id=0, return_verts=True, return_tensor=False, **kwargs):
+    def __call__(
+        self, keypoints3d, id=0, return_verts=True, return_tensor=False, **kwargs
+    ):
         if len(keypoints3d.shape) == 2:
             keypoints3d = keypoints3d[None]
         if not return_verts:
             return keypoints3d
         if keypoints3d.shape[-1] == 3:  # add confidence
-            keypoints3d = np.dstack((keypoints3d, np.ones(
-                (keypoints3d.shape[0], keypoints3d.shape[1], 1))))
+            keypoints3d = np.dstack(
+                (keypoints3d, np.ones((keypoints3d.shape[0], keypoints3d.shape[1], 1)))
+            )
         r = self.joint_radius
         if keypoints3d.shape[0] > 15 and keypoints3d.shape[0] != self.nJoints:
-            logger.warning(f'keypoint3d shape not equal to nJoints: {keypoints3d.shape[0]} vs {self.nJoints}')
+            logger.warning(
+                f"keypoint3d shape not equal to nJoints: {keypoints3d.shape[0]} vs {self.nJoints}"
+            )
         # joints
         min_conf = 0.1
         verts_final = []
         for nper in range(keypoints3d.shape[0]):
             vertices_all = []
             kpts3d = keypoints3d[nper]
             # limb
             closet_joints = []
             for nk, (i, j) in enumerate(self.kintree):
                 if kpts3d[i][-1] < min_conf or kpts3d[j][-1] < min_conf:
-                    vertices_all.append(self.vertices*0.001)
+                    vertices_all.append(self.vertices * 0.001)
                     continue
-                T, _, length = calTransformation(
-                    kpts3d[i, :3], kpts3d[j, :3], r=1)
+                T, _, length = calTransformation(kpts3d[i, :3], kpts3d[j, :3], r=1)
                 if length > 2:  # large than 2 meter
-                    vertices_all.append(self.vertices*0.001)
+                    vertices_all.append(self.vertices * 0.001)
                     continue
                 if length < self.joint_radius * 5:
                     closet_joints.append(i)
                     closet_joints.append(j)
                 vertices = self.vertices @ T[:3, :3].T + T[:3, 3:].T
                 vertices_all.append(vertices)
             for nj in range(self.nJoints):
-                if self.body_type in ['bodyhand', 'bodyhandface'] and nj > 25:
+                if self.body_type in ["bodyhand", "bodyhandface"] and nj > 25:
                     r_ = r / 2
                 else:
                     r_ = r
                 if kpts3d[nj, -1] < min_conf:
-                    vertices_all.append(self.vertices*0.001)
+                    vertices_all.append(self.vertices * 0.001)
                     continue
-                vertices_all.append(self.vertices*r_ + kpts3d[nj:nj+1, :3])
+                vertices_all.append(self.vertices * r_ + kpts3d[nj : nj + 1, :3])
             vertices = np.vstack(vertices_all)
             verts_final.append(vertices)
         verts_final = np.stack(verts_final)
         return verts_final
 
     def to(self, none):
         pass
 
     def merge_params(self, params, share_shape=False):
-        keypoints = np.stack([param['keypoints3d'] for param in params])
-        return {'keypoints3d': keypoints, 'id': [0]}
+        keypoints = np.stack([param["keypoints3d"] for param in params])
+        return {"keypoints3d": keypoints, "id": [0]}
 
     def init_params(self, nFrames):
-        return {'keypoints3d': np.zeros((self.nJoints, 4))}
+        return {"keypoints3d": np.zeros((self.nJoints, 4))}
 
 
 class SMPLSKEL:
     def __init__(self, model_type, gender, body_type) -> None:
         from ..smplmodel import load_model
+
         config = CONFIG[body_type]
-        self.smpl_model = load_model(
-            gender, model_type=model_type, skel_type=body_type)
-        self.body_model = SkelModel(config['nJoints'], config['kintree'])
+        self.smpl_model = load_model(gender, model_type=model_type, skel_type=body_type)
+        self.body_model = SkelModel(config["nJoints"], config["kintree"])
 
     def __call__(self, return_verts=True, **kwargs):
-        keypoints3d = self.smpl_model(
-            return_verts=False, return_tensor=False, **kwargs)
+        keypoints3d = self.smpl_model(return_verts=False, return_tensor=False, **kwargs)
         if not return_verts:
             return keypoints3d
         else:
             verts = self.body_model(
-                return_verts=True, return_tensor=False, keypoints3d=keypoints3d[0])
+                return_verts=True, return_tensor=False, keypoints3d=keypoints3d[0]
+            )
             return verts
 
     def init_params(self, nFrames):
         return np.zeros((self.body_model.nJoints, 4))
```

### Comparing `alfred-py-3.0.6/alfred/vis/mesh3d/utils.py` & `alfred-py-3.0.7/alfred/vis/renders/render_p3d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,312 +1,261 @@
-import time
-import tabulate
-import socket
-import time
-from threading import Thread
-from queue import Queue
-import cv2
-import numpy as np
+# -*- coding: utf-8 -*-
+# brought from https://github.com/mkocabas/VIBE/blob/master/lib/utils/renderer.py
+import sys
 import os
+import json
+from typing import Tuple
+from pytorch3d.renderer.cameras import PerspectiveCameras
+import torch
+from torch import nn
+import pickle
+
+# Data structures and functions for rendering
+from pytorch3d.structures import Meshes, join_meshes_as_scene
+from pytorch3d.renderer import (
+    look_at_view_transform,
+    FoVPerspectiveCameras,
+    FoVOrthographicCameras,
+    OpenGLPerspectiveCameras,
+    PointLights,
+    DirectionalLights,
+    Materials,
+    RasterizationSettings,
+    MeshRenderer,
+    MeshRasterizer,
+    SoftPhongShader,
+    TexturesUV,
+    TexturesVertex,
+)
 
+# from pytorch3d.io.mesh
+from pytorch3d.io import IO
+import numpy as np
 
-def log(x):
-    from datetime import datetime
-    time_now = datetime.now().strftime("%m-%d-%H:%M:%S.%f ")
-    print(time_now + x)
-
-
-def myarray2string(array, separator=', ', fmt='%.3f', indent=8):
-    assert len(array.shape) == 2, 'Only support MxN matrix, {}'.format(
-        array.shape)
-    blank = ' ' * indent
-    res = ['[']
-    for i in range(array.shape[0]):
-        res.append(
-            blank + '  ' + '[{}]'.format(separator.join([fmt % (d) for d in array[i]])))
-        if i != array.shape[0] - 1:
-            res[-1] += ', '
-    res.append(blank + ']')
-    return '\r\n'.join(res)
-
-
-def write_common_results(dumpname=None, results=[], keys=[], fmt='%2.3f'):
-    format_out = {'float_kind': lambda x: fmt % x}
-    out_text = []
-    out_text.append('[\n')
-    for idata, data in enumerate(results):
-        out_text.append('    {\n')
-        output = {}
-        output['id'] = data['id']
-        for key in keys:
-            if key not in data.keys():
-                continue
-            # BUG: This function will failed if the rows of the data[key] is too large
-            # output[key] = np.array2string(data[key], max_line_width=1000, separator=', ', formatter=format_out)
-            output[key] = myarray2string(data[key], separator=', ', fmt=fmt)
-        for key in output.keys():
-            out_text.append('        \"{}\": {}'.format(key, output[key]))
-            if key != keys[-1]:
-                out_text.append(',\n')
-            else:
-                out_text.append('\n')
-        out_text.append('    }')
-        if idata != len(results) - 1:
-            out_text.append(',\n')
-        else:
-            out_text.append('\n')
-    out_text.append(']\n')
-    if dumpname is not None:
-        os.makedirs(os.path.dirname(dumpname), exist_ok=True)
-        with open(dumpname, 'w') as f:
-            f.writelines(out_text)
-    else:
-        return ''.join(out_text)
-
-
-def encode_detect(data):
-    res = write_common_results(None, data, ['keypoints3d'])
-    res = res.replace('\r', '').replace('\n', '').replace(' ', '')
-    return res.encode('ascii')
-
-
-def encode_smpl(data):
-    res = write_common_results(
-        None, data, ['poses', 'shapes', 'expression', 'Rh', 'Th'])
-    res = res.replace('\r', '').replace('\n', '').replace(' ', '')
-    return res.encode('ascii')
-
-
-def encode_image(image):
-    fourcc = [int(cv2.IMWRITE_JPEG_QUALITY), 90]
-    result, img_encode = cv2.imencode('.jpg', image, fourcc)
-    data = np.array(img_encode)
-    stringData = data.tostring()
-    return stringData
-
-
-class BaseSocketClient:
-    def __init__(self, host, port) -> None:
-        if host == 'auto':
-            host = socket.gethostname()
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.connect((host, port))
-        self.s = s
-
-    def send(self, data):
-        val = encode_detect(data)
-        self.s.send(bytes('{}\n'.format(len(val)), 'ascii'))
-        self.s.sendall(val)
-
-    def send_smpl(self, data):
-        val = encode_smpl(data)
-        self.s.send(bytes('{}\n'.format(len(val)), 'ascii'))
-        self.s.sendall(val)
-
-    def close(self):
-        self.s.close()
-
-
-class BaseSocket:
-    def __init__(self, host, port, debug=False) -> None:
-        # 创建 socket 对象
-        print('[Info] server start')
-        serversocket = socket.socket(
-            socket.AF_INET, socket.SOCK_STREAM)
-        serversocket.bind((host, port))
-        serversocket.listen(1)
-        self.serversocket = serversocket
-        self.queue = Queue()
-        self.t = Thread(target=self.run)
-        self.t.start()
-        self.debug = debug
-        self.disconnect = False
-
-    @staticmethod
-    def recvLine(sock):
-        flag = True
-        result = b''
-        while not result.endswith(b'\n'):
-            res = sock.recv(1)
-            if not res:
-                flag = False
-                break
-            result += res
-        return flag, result.strip().decode('ascii')
-
-    @staticmethod
-    def recvAll(sock, l):
-        l = int(l)
-        result = b''
-        while (len(result) < l):
-            t = sock.recv(l - len(result))
-            result += t
-        return result.decode('ascii')
-
-    def run(self):
-        while True:
-            clientsocket, addr = self.serversocket.accept()
-            print("[Info] Connect: %s" % str(addr))
-            self.disconnect = False
-            while True:
-                flag, l = self.recvLine(clientsocket)
-                if not flag:
-                    print("[Info] Disonnect: %s" % str(addr))
-                    self.disconnect = True
-                    break
-                data = self.recvAll(clientsocket, l)
-                if self.debug:
-                    log('[Info] Recv data')
-                self.queue.put(data)
-            clientsocket.close()
-
-    def update(self):
-        time.sleep(1)
-        while not self.queue.empty():
-            log('update')
-            data = self.queue.get()
-            self.main(data)
-
-    def main(self, datas):
-        print(datas)
-
-    def __del__(self):
-        self.serversocket.close()
-        self.t.join()
-
-
-class Timer:
-    records = {}
-    tmp = None
-
-    @classmethod
-    def tic(cls):
-        cls.tmp = time.time()
-
-    @classmethod
-    def toc(cls):
-        res = (time.time() - cls.tmp) * 1000
-        cls.tmp = None
-        return res
-
-    @classmethod
-    def report(cls):
-        header = ['', 'Time(ms)']
-        contents = []
-        for key, val in cls.records.items():
-            contents.append(
-                ['{:20s}'.format(key), '{:.2f}'.format(sum(val)/len(val))])
-        print(tabulate.tabulate(contents, header, tablefmt='fancy_grid'))
-
-    def __init__(self, name, silent=False):
-        self.name = name
-        self.silent = silent
-        if name not in Timer.records.keys():
-            Timer.records[name] = []
-
-    def __enter__(self):
-        self.start = time.time()
-
-    def __exit__(self, exc_type, exc_value, exc_tb):
-        end = time.time()
-        Timer.records[self.name].append((end-self.start)*1000)
-        if not self.silent:
-            t = (end - self.start)*1000
-            if t > 1000:
-                print('-> [{:20s}]: {:5.1f}s'.format(self.name, t/1000))
-            elif t > 1e3*60*60:
-                print('-> [{:20s}]: {:5.1f}min'.format(self.name, t/1e3/60))
-            else:
-                print('-> [{:20s}]: {:5.1f}ms'.format(self.name,
-                      (end-self.start)*1000))
+
+"""
+source code adopt from ROMP
+edited by alfred-py
+"""
 
 
-'''
-Color utils
-'''
-
-
-def generate_colorbar(N=20, cmap='jet'):
-    bar = ((np.arange(N)/(N-1))*255).astype(np.uint8).reshape(-1, 1)
-    colorbar = cv2.applyColorMap(bar, cv2.COLORMAP_JET).squeeze()
-    if False:
-        colorbar = np.clip(colorbar + 64, 0, 255)
-    import random
-    random.seed(666)
-    index = [i for i in range(N)]
-    random.shuffle(index)
-    rgb = colorbar[index, :]
-    rgb = rgb.tolist()
-    return rgb
-
-
-colors_bar_rgb = generate_colorbar(cmap='hsv')
-
-colors_table = {
-    'b': [0.65098039, 0.74117647, 0.85882353],
-    '_pink': [.9, .7, .7],
-    '_mint': [166/255.,  229/255.,  204/255.],
-    '_mint2': [202/255.,  229/255.,  223/255.],
-    '_green': [153/255.,  216/255.,  201/255.],
-    '_green2': [171/255.,  221/255.,  164/255.],
-    'r': [251/255.,  128/255.,  114/255.],
-    '_orange': [253/255.,  174/255.,  97/255.],
-    'y': [250/255.,  230/255.,  154/255.],
-    '_r': [255/255, 0, 0],
-    'g': [0, 255/255, 0],
-    '_b': [0, 0, 255/255],
-    'k': [0, 0, 0],
-    '_y': [255/255, 255/255, 0],
-    'purple': [128/255, 0, 128/255],
-    'smap_b': [51/255, 153/255, 255/255],
-    'smap_r': [255/255, 51/255, 153/255],
-    'smap_b': [51/255, 255/255, 153/255],
+colors = {
+    "pink": [0.7, 0.7, 0.9],
+    "neutral": [0.9, 0.9, 0.8],
+    "capsule": [0.7, 0.75, 0.5],
+    "yellow": [0.5, 0.7, 0.75],
 }
 
 
-def get_rgb(index):
-    if isinstance(index, int):
-        if index == -1:
-            return (255, 255, 255)
-        if index < -1:
-            return (0, 0, 0)
-        col = colors_bar_rgb[index % len(colors_bar_rgb)]
-    else:
-        col = colors_table.get(index, (1, 0, 0))
-        col = tuple([int(c*255) for c in col[::-1]])
-    return col
-
-
-def get_rgb_01(index):
-    col = get_rgb(index)
-    return [i*1./255 for i in col[:3]]
-
-
-class BaseCrit:
-    def __init__(self, min_conf, min_joints=3) -> None:
-        self.min_conf = min_conf
-        self.min_joints = min_joints
-        self.name = self.__class__.__name__
-
-    def __call__(self, keypoints3d, **kwargs):
-        # keypoints3d: (N, 4)
-        conf = keypoints3d[..., -1]
-        conf[conf < self.min_conf] = 0
-        idx = keypoints3d[..., -1] > self.min_conf
-        return len(idx) > self.min_joints
-
-
-class CritRange(BaseCrit):
-    def __init__(self, minr, maxr, rate_inlier, min_conf) -> None:
-        super().__init__(min_conf)
-        self.min = minr
-        self.max = maxr
-        self.rate = rate_inlier
-
-    def __call__(self, keypoints3d, **kwargs):
-        idx = keypoints3d[..., -1] > self.min_conf
-        k3d = keypoints3d[idx, :3]
-        crit = (k3d[:, 0] > self.min[0]) & (k3d[:, 0] < self.max[0]) &\
-            (k3d[:, 1] > self.min[1]) & (k3d[:, 1] < self.max[1]) &\
-            (k3d[:, 2] > self.min[2]) & (k3d[:, 2] < self.max[2])
-        self.log = '{}: {}'.format(self.name, k3d)
-        return crit.sum()/crit.shape[0] > self.rate
+def get_projection_matrix_for_weak_perspective_camera(s_x, s_y, t_x, t_y):
+    P = torch.eye(4)
+    P[0, 0] = s_x
+    P[1, 1] = s_y
+    P[0, 3] = t_x * s_x
+    P[1, 3] = -t_y * s_y
+    P[2, 2] = -1
+    print(P)
+    return P[:-1, :-1], P[:, -1][:-1]
+
+
+class Renderer(nn.Module):
+    def __init__(
+        self,
+        faces,
+        resolution=(512, 512),
+        perps=True,
+        R=None,
+        T=None,
+        use_gpu=False,
+    ):
+        super(Renderer, self).__init__()
+        self.name = "pytorch3d"
+        self.perps = perps
+        if use_gpu:
+            self.device = torch.device("cuda")
+            print("visualize in gpu mode")
+        else:
+            self.device = torch.device("cpu")
+            print("visualize in cpu mode")
+
+        if isinstance(faces, np.ndarray):
+            faces = torch.from_numpy(faces.astype(np.float))
+            faces.to(self.device)
+        self.faces = faces.unsqueeze(0).to(self.device)  # add a BatchSize dim
+        self.default_color = torch.as_tensor(colors["neutral"]).unsqueeze(0)
+        print("default color: ", self.default_color.shape)
+        self.save_io = IO()
+
+        if R is None:
+            self.default_R = torch.Tensor(
+                [[[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]]
+            )
+        if T is None:
+            self.default_T = torch.Tensor([[0.0, 0.0, 0.0]])
+        self.fov = 60
+
+        if self.perps:
+            # self.cameras = FoVPerspectiveCameras(zfar=1000,
+            #     R=self.default_R, T=self.default_T, fov=60, device=self.device
+            # )
+            self.cameras = PerspectiveCameras(
+                focal_length=5000,
+                R=self.default_R,
+                T=self.default_T,
+                device=self.device,
+            )
+            self.lights = PointLights(
+                ambient_color=((0.56, 0.56, 0.56),),
+                location=torch.Tensor([[0.0, 0.0, 0.0]]),
+                device=self.device,
+            )
+        else:
+            self.cameras = FoVOrthographicCameras(
+                R=self.default_R,
+                T=self.default_T,
+                znear=0.0,
+                zfar=100.0,
+                max_y=1.0,
+                min_y=-1.0,
+                max_x=1.0,
+                min_x=-1.0,
+                device=self.device,
+            )
+            self.lights = DirectionalLights(
+                direction=torch.Tensor([[0.0, 1.0, 0.0]]), device=self.device
+            )
+
+        # Define the settings for rasterization and shading. Here we set the output image to be of size
+        # 512x512. As we are rendering images for visualization purposes only we will set faces_per_pixel=1
+        # and blur_radius=0.0.
+        raster_settings = RasterizationSettings(
+            image_size=(resolution[0], resolution[1]),
+            blur_radius=0.0,
+            faces_per_pixel=1,
+        )
+        print("resolution: ", resolution)
+
+        # Create a Phong renderer by composing a rasterizer and a shader. The textured Phong shader will
+        # interpolate the texture uv coordinates for each vertex, sample from a texture image and
+        # apply the Phong lighting model
+        self.renderer = MeshRenderer(
+            rasterizer=MeshRasterizer(
+                cameras=self.cameras, raster_settings=raster_settings
+            ),
+            shader=SoftPhongShader(
+                device=self.device, cameras=self.cameras, lights=self.lights
+            ),
+        )
+
+    # def render(self, img, verts, cam, angle=None, axis=None, mesh_filename=None, color=[1.0, 1.0, 0.9], rotate=False):
+    def render(
+        self,
+        img,
+        verts,
+        faces=None,
+        color=None,
+        camera_t=torch.zeros([1, 3, 3], dtype=torch.float32),
+        camera_rot=torch.zeros([1, 3, 3], dtype=torch.float32),
+        focal_length=1000,
+        merge_meshes=True,
+        cam=None,
+        mesh_filename=None,
+        **kwargs,
+    ):
+        assert (
+            len(verts.shape) >= 2
+        ), f"The input verts of visualizer is bounded to be 3-dims (Nx6890 x3) tensor, but got: {verts.shape}"
+        if isinstance(verts, np.ndarray):
+            verts = torch.from_numpy(verts)
+        if len(verts.shape) == 2:
+            verts = verts.unsqueeze(0)
+        if faces is None:
+            faces = self.faces
+
+        BS = verts.shape[0]
+        if verts.shape[0] != faces.shape[0]:
+            faces = faces.repeat(BS, 1, 1).to(self.device)
+
+        verts = verts.to(self.device)
+
+        if (
+            isinstance(color, np.ndarray)
+            or isinstance(color, tuple)
+            or isinstance(color, list)
+        ):
+            # color = torch.from_numpy(np.array(color)).to(self.device).unsqueeze(1)
+            color = torch.from_numpy(np.array(color)).to(self.device).unsqueeze(0)
+        elif color is None:
+            color = self.default_color
+
+        verts = verts.to(self.device)
+        verts = verts.float()
+        verts_rgb = torch.ones_like(verts)
+        verts_rgb[:, :] = color
+        textures = TexturesVertex(verts_features=verts_rgb)
+        verts[:, :, :2] *= -1
+        meshes = Meshes(verts, faces, textures)
+        if merge_meshes:
+            meshes = join_meshes_as_scene(meshes)
+        if mesh_filename is not None:
+            self.save_io.save_mesh(meshes, mesh_filename)
+        if camera_t is not None:
+            # cam = cam.float()
+            # print(cam)
+            cam = torch.as_tensor(camera_t).to(self.device)
+            if self.perps:
+                T = cam
+                T = T.unsqueeze(0).repeat(BS, 1)
+                print(T)
+                # new_cam = FoVPerspectiveCameras(zfar=1000, znear=0.05,
+                #     R=self.default_R, T=T, fov=self.fov, device=self.device)
+                new_cam = PerspectiveCameras(
+                    focal_length=focal_length, R=self.default_R, T=T, device=self.device
+                )
+            else:
+                R, T, xyz_ranges = cam
+                new_cam = FoVOrthographicCameras(
+                    R=R, T=self.default_T, **xyz_ranges, device=self.device
+                )
+            images = self.renderer(meshes, cameras=new_cam)
+        else:
+            images = self.renderer(meshes)
+        print(images)
+        images[..., :-1] *= 255
+        images = images[..., :-1].cpu().numpy()
+        print(images)
+        if images.shape[-1] > 3:
+            images = images[..., :-1]
+        return images
+
+
+def get_renderer(test=False, **kwargs):
+    renderer = Renderer(**kwargs)
+    if test:
+        import cv2
+
+        dist = 1 / np.tan(np.radians(args().FOV / 2.0))
+        print("dist:", dist)
+        model = pickle.load(
+            open(
+                os.path.join(args().smpl_model_path, "smpl", "SMPL_NEUTRAL.pkl"), "rb"
+            ),
+            encoding="latin1",
+        )
+        np_v_template = (
+            torch.from_numpy(np.array(model["v_template"])).cuda().float()[None]
+        )
+        face = torch.from_numpy(model["f"].astype(np.int32)).cuda()[None]
+        np_v_template = np_v_template.repeat(2, 1, 1)
+        np_v_template[1] += 0.3
+        np_v_template[:, :, 2] += dist
+        face = face.repeat(2, 1, 1)
+        result = renderer(np_v_template, face).cpu().numpy()
+        for ri in range(len(result)):
+            cv2.imwrite(
+                "test{}.png".format(ri), (result[ri, :, :, :3] * 255).astype(np.uint8)
+            )
+    return renderer
+
+
+if __name__ == "__main__":
+    get_renderer(test=True, perps=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alfred-py-3.0.6/alfred/vis/pointcloud/__init__.py` & `alfred-py-3.0.7/alfred/vis/pointcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `alfred-py-3.0.6/alfred/vis/pointcloud/pointcloud_vis.py` & `alfred-py-3.0.7/alfred/vis/pointcloud/pointcloud_vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 showing 3d point cloud using open3d
 """
 import numpy as np
 import cv2
 import matplotlib.pyplot as plt
 
 from alfred.fusion.common import compute_3d_box_lidar_coords
+
 try:
     from open3d import *
     import open3d as o3d
 except ImportError:
-    print('importing 3d_vis in alfred-py need open3d installed.')
+    print("importing 3d_vis in alfred-py need open3d installed.")
     exit(0)
 
 
 def draw_pointclouds_boxes_o3d(pointcloud, boxes_3d, line_color=[0, 1, 0]):
     """
     draw boxes3d on pointcloud, a typical boxes_3d format:
     [[4.481686, 5.147319, -1.0229858, 1.5728549, 3.646751, 1.5121397, 1.5486346],
@@ -51,23 +52,35 @@
     pcs = np.array(pointcloud[:, :3])
     pcobj = o3d.geometry.PointCloud()
     pcobj.points = o3d.utility.Vector3dVector(pcs)
     geometries.append(pcobj)
 
     # append boxes to geometries
     for p in boxes_3d:
-        xyz = np.array([p[: 3]])
-        hwl = np.array([p[3: 6]])
+        xyz = np.array([p[:3]])
+        hwl = np.array([p[3:6]])
         r_y = [p[6]]
         pts3d = compute_3d_box_lidar_coords(
-            xyz, hwl, angles=r_y, origin=(0.5, 0.5, 0.5), axis=2)
+            xyz, hwl, angles=r_y, origin=(0.5, 0.5, 0.5), axis=2
+        )
 
-        lines = [[0, 1], [1, 2], [2, 3], [3, 0],
-                 [4, 5], [5, 6], [6, 7], [7, 4],
-                 [0, 4], [1, 5], [2, 6], [3, 7]]
+        lines = [
+            [0, 1],
+            [1, 2],
+            [2, 3],
+            [3, 0],
+            [4, 5],
+            [5, 6],
+            [6, 7],
+            [7, 4],
+            [0, 4],
+            [1, 5],
+            [2, 6],
+            [3, 7],
+        ]
         colors = [line_color for i in range(len(lines))]
         line_set = o3d.geometry.LineSet()
         line_set.points = o3d.utility.Vector3dVector(pts3d[0])
         line_set.lines = o3d.utility.Vector2iVector(lines)
         line_set.colors = o3d.utility.Vector3dVector(colors)
         geometries.append(line_set)
 
@@ -114,25 +127,27 @@
     line_set = LineSet()
     line_set.points = Vector3dVector(points)
     line_set.lines = Vector2iVector(lines)
     line_set.colors = Vector3dVector(colors)
     draw_pcs_open3d([point_cloud, line_set])
     ```
     """
+
     def capture_depth(vis):
         depth = vis.capture_depth_float_buffer()
         plt.imshow(np.asarray(depth))
         plt.show()
         return False
 
     def capture_image(vis):
         image = vis.capture_screen_float_buffer()
         plt.imshow(np.asarray(image))
         plt.show()
         return False
+
     vis = o3d.visualization.Visualizer()
     vis.create_window()
     for g in geometries:
         vis.add_geometry(g)
     opt = vis.get_render_option()
     opt.background_color = np.asarray([255, 255, 255])
     opt.point_size = 2
```

### Comparing `alfred-py-3.0.6/alfred/vis/renders/render_prd.py` & `alfred-py-3.0.7/alfred/vis/renders/render_prd.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,33 @@
 import numpy as np
 import cv2
 import trimesh
 
 
 # autopep8: off
 os_name = platform.platform().lower()
-if 'centos' in os_name or 'windows' in os_name or 'tlinux' in os_name:
-    os.environ['PYOPENGL_PLATFORM'] = 'egl'
-elif 'debian' in os_name or 'ubuntu' in os_name:
-    os.environ['PYOPENGL_PLATFORM'] = 'osmesa'
-print(os.environ['PYOPENGL_PLATFORM'])
+if "centos" in os_name or "windows" in os_name or "tlinux" in os_name:
+    os.environ["PYOPENGL_PLATFORM"] = "egl"
+elif "debian" in os_name or "ubuntu" in os_name:
+    os.environ["PYOPENGL_PLATFORM"] = "osmesa"
+print(os.environ["PYOPENGL_PLATFORM"])
 
 import pyrender
 from pyrender.constants import RenderFlags
 from pyrender.constants import DEFAULT_Z_NEAR
+
 # autopep8: on
 
 
 class WeakPerspectiveCamera(pyrender.Camera):
-    def __init__(self,
-                 scale,
-                 translation,
-                 znear=DEFAULT_Z_NEAR,
-                 zfar=None,
-                 name=None):
+    def __init__(self, scale, translation, znear=DEFAULT_Z_NEAR, zfar=None, name=None):
         super(WeakPerspectiveCamera, self).__init__(
-            znear=znear, zfar=zfar, name=name,
+            znear=znear,
+            zfar=zfar,
+            name=name,
         )
         self.scale = scale
         self.translation = translation
 
     def get_projection_matrix(self, width=None, height=None):
         P = np.eye(4)
         P[0, 0] = self.scale[0]
@@ -41,70 +39,76 @@
         P[0, 3] = self.translation[0] * self.scale[0]
         P[1, 3] = -self.translation[1] * self.scale[1]
         P[2, 2] = -1
         return P
 
 
 class Renderer:
-    def __init__(self, smpl_faces, resolution=(224, 224), orig_img=False, wireframe=False, use_gpu=True):
+    def __init__(
+        self,
+        smpl_faces,
+        resolution=(224, 224),
+        orig_img=False,
+        wireframe=False,
+        use_gpu=True,
+    ):
         """
         resolution is: h, w
         """
-        self.name = 'pyrender'
+        self.name = "pyrender"
         self.resolution = resolution
         self.faces = smpl_faces
         self.orig_img = orig_img
         self.wireframe = wireframe
         self.renderer = pyrender.OffscreenRenderer(
             viewport_width=self.resolution[1],
             viewport_height=self.resolution[0],
             point_size=1.0,
         )
         # set the scene
         self.scene = pyrender.Scene(
-            bg_color=[0.0, 0.0, 0.0, 0.0], ambient_light=(0.3, 0.3, 0.3))
+            bg_color=[0.0, 0.0, 0.0, 0.0], ambient_light=(0.3, 0.3, 0.3)
+        )
 
         # light = pyrender.PointLight(color=[1.0, 1.0, 1.0], intensity=0.8)
         light = pyrender.DirectionalLight(color=[1.0, 1.0, 1.0], intensity=0.8)
 
         light_pose = np.eye(4)
         light_pose[:3, 3] = [0, -1, 1]
         self.scene.add(light, pose=light_pose)
 
         light_pose[:3, 3] = [0, 1, 1]
         self.scene.add(light, pose=light_pose)
 
         light_pose[:3, 3] = [1, 1, 2]
         self.scene.add(light, pose=light_pose)
-        print('render initiated.')
+        print("render initiated.")
 
     def render(
         self,
         img,
         verts,
         cam,
         angle=None,
         axis=None,
         mesh_filename=None,
         color=[1.0, 1.0, 0.9],
         rotate=False,
     ):
         mesh = trimesh.Trimesh(vertices=verts, faces=self.faces, process=False)
 
-        Rx = trimesh.transformations.rotation_matrix(
-            math.radians(180), [1, 0, 0])
+        Rx = trimesh.transformations.rotation_matrix(math.radians(180), [1, 0, 0])
         mesh.apply_transform(Rx)
-        
+
         if rotate:
             rot = trimesh.transformations.rotation_matrix(np.radians(60), [0, 1, 0])
             mesh.apply_transform(rot)
 
         if angle and axis:
-            R = trimesh.transformations.rotation_matrix(
-                math.radians(angle), axis)
+            R = trimesh.transformations.rotation_matrix(math.radians(angle), axis)
             mesh.apply_transform(R)
 
         if mesh_filename is not None:
             mesh.export(mesh_filename)
 
         sx, sy, tx, ty = cam
 
@@ -119,15 +123,15 @@
             wireframe=True,
             roughnessFactor=1.0,
             emissiveFactor=(0.1, 0.1, 0.1),
             baseColorFactor=(color[0], color[1], color[2], 1.0),
         )
 
         mesh = pyrender.Mesh.from_trimesh(mesh, material=material)
-        mesh_node = self.scene.add(mesh, 'mesh')
+        mesh_node = self.scene.add(mesh, "mesh")
 
         camera_pose = np.eye(4)
         cam_node = self.scene.add(camera, pose=camera_pose)
 
         if self.wireframe:
             render_flags = RenderFlags.RGBA | RenderFlags.ALL_WIREFRAME
         else:
@@ -136,14 +140,14 @@
 
         if rgb.shape[-1] == 4:
             valid_mask = (rgb[:, :, -1] > 0)[:, :, np.newaxis]
             output_img = rgb[:, :, :-1] * valid_mask + (1 - valid_mask) * img
             image = output_img.astype(np.uint8)
         else:
             # rgb could be 3 channel output
-            valid_mask = (rgb > 0)
+            valid_mask = rgb > 0
             output_img = rgb * valid_mask + (1 - valid_mask) * img
             image = output_img.astype(np.uint8)
 
         self.scene.remove_node(mesh_node)
         self.scene.remove_node(cam_node)
         return image
```

### Comparing `alfred-py-3.0.6/alfred_py.egg-info/PKG-INFO` & `alfred-py-3.0.7/alfred_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-py
-Version: 3.0.6
+Version: 3.0.7
 Summary: Alfred is a DeepLearning utility library.
 Home-page: https://github.com/jinfagang/alfred
 Author: Lucas Jin
 Author-email: jinfagang19@163.com
 License: GPL-3.0
 Keywords: deep learning,script helper,tools
 Platform: any
```

### Comparing `alfred-py-3.0.6/alfred_py.egg-info/SOURCES.txt` & `alfred-py-3.0.7/alfred_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 alfred/utils/cv_wrapper.py
 alfred/utils/file_io.py
 alfred/utils/image_convertor.py
 alfred/utils/log.py
 alfred/utils/mana.py
 alfred/utils/math_utils.py
 alfred/utils/pprint.py
+alfred/utils/progress.py
 alfred/utils/timer.py
 alfred/vis/__init__.py
 alfred/vis/image/__init__.py
 alfred/vis/image/common.py
 alfred/vis/image/constants.py
 alfred/vis/image/det.py
 alfred/vis/image/face.py
```

### Comparing `alfred-py-3.0.6/setup.py` & `alfred-py-3.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,113 +27,125 @@
 """
 from setuptools import setup, find_packages
 from setuptools import setup, Extension
 import io
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
-with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with io.open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-version_file = 'alfred/version.py'
+version_file = "alfred/version.py"
 
 
 def get_version():
-    with open(version_file, 'r') as f:
-        exec(compile(f.read(), version_file, 'exec'))
-    return locals()['__version__']
-
-
-setup(name='alfred-py',
-      version=get_version(),
-      keywords=['deep learning', 'script helper', 'tools'],
-      description='Alfred is a DeepLearning utility library.',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      license='GPL-3.0',
-      classifiers=[
-          # Operation system
-          "Operating System :: OS Independent",
-          # How mature is this project? Common values are
-          #   3 - Alpha
-          #   4 - Beta
-          #   5 - Production/Stable
-          "Development Status :: 4 - Beta",
-          # Indicate who your project is intended for
-          "Intended Audience :: Developers",
-          # Topics
-          "Topic :: Education",
-          "Topic :: Scientific/Engineering",
-          "Topic :: Scientific/Engineering :: Artificial Intelligence",
-          "Topic :: Scientific/Engineering :: Image Recognition",
-          # Pick your license as you wish
-          "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-          # Specify the Python versions you support here. In particular, ensure
-          # that you indicate whether you support Python 2, Python 3 or both.
-          "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.6",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
-      ],
-      find_packages='',
-      packages=[
-          'alfred',
-          'alfred.dl',
-          'alfred.dl.inference',
-          'alfred.dl.data',
-          'alfred.dl.data.common',
-          'alfred.dl.data.meta',
-          'alfred.dl.torch',
-          'alfred.dl.torch.train',
-          'alfred.dl.torch.distribute',
-          'alfred.dl.torch.runner',
-          'alfred.dl.torch.nn',
-          'alfred.dl.torch.nn.modules',
-          'alfred.dl.torch.ops',
-          'alfred.dl.metrics',
-          'alfred.dl.tf',
-          'alfred.dl.evaluator',
-          'alfred.vis',
-          'alfred.modules',
-          'alfred.modules.scrap',
-          'alfred.modules.text',
-          'alfred.modules.vision',
-          'alfred.modules.data',
-          'alfred.modules.dltool',
-          'alfred.modules.cabinet',
-          'alfred.modules.cabinet.mdparse',
-          'alfred.modules.cabinet.mdparse.formatters',
-          'alfred.modules.cabinet.mdparse.transformers',
-          'alfred.modules.cabinet.mdparse.transformers.html',
-          'alfred.modules.cabinet.mdparse.transformers.md',
-          'alfred.modules',
-          'alfred.fusion',
-          'alfred.vis.image',
-          'alfred.vis.image.pose_datasets',
-          'alfred.vis.pointcloud',
-          'alfred.vis.renders',
-          'alfred.vis.mesh3d',
-          'alfred.utils',
-          'alfred.siren',
-          'alfred.protos',
-          'alfred.deploy.tensorrt'
-      ],
-      # package_dir={'alfred': 'alfred'},
-      entry_points={
-          'console_scripts': [
-              'alfred = alfred.alfred:main'
-          ]
-      },
-      include_package_data=True,
-      author="Lucas Jin",
-      author_email="jinfagang19@163.com",
-      url='https://github.com/jinfagang/alfred',
-      platforms='any',
-      install_requires=['colorama', 'natsort', 'requests', 'regex',
-                        'funcy', 'pascal-voc-writer', 'markdown',
-                        'future', 'deprecated', 'loguru',
-                        'pyquaternion', 'jsons', 'natsort', 'loguru',
-                        'pascal_voc_writer', 'funcy', 'gtrending', 'xdg',
-                        'portalocker']
-      )
+    with open(version_file, "r") as f:
+        exec(compile(f.read(), version_file, "exec"))
+    return locals()["__version__"]
+
+
+setup(
+    name="alfred-py",
+    version=get_version(),
+    keywords=["deep learning", "script helper", "tools"],
+    description="Alfred is a DeepLearning utility library.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license="GPL-3.0",
+    classifiers=[
+        # Operation system
+        "Operating System :: OS Independent",
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 4 - Beta",
+        # Indicate who your project is intended for
+        "Intended Audience :: Developers",
+        # Topics
+        "Topic :: Education",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Image Recognition",
+        # Pick your license as you wish
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+    ],
+    find_packages="",
+    packages=[
+        "alfred",
+        "alfred.dl",
+        "alfred.dl.inference",
+        "alfred.dl.data",
+        "alfred.dl.data.common",
+        "alfred.dl.data.meta",
+        "alfred.dl.torch",
+        "alfred.dl.torch.train",
+        "alfred.dl.torch.distribute",
+        "alfred.dl.torch.runner",
+        "alfred.dl.torch.nn",
+        "alfred.dl.torch.nn.modules",
+        "alfred.dl.torch.ops",
+        "alfred.dl.metrics",
+        "alfred.dl.tf",
+        "alfred.dl.evaluator",
+        "alfred.vis",
+        "alfred.modules",
+        "alfred.modules.scrap",
+        "alfred.modules.text",
+        "alfred.modules.vision",
+        "alfred.modules.data",
+        "alfred.modules.dltool",
+        "alfred.modules.cabinet",
+        "alfred.modules.cabinet.mdparse",
+        "alfred.modules.cabinet.mdparse.formatters",
+        "alfred.modules.cabinet.mdparse.transformers",
+        "alfred.modules.cabinet.mdparse.transformers.html",
+        "alfred.modules.cabinet.mdparse.transformers.md",
+        "alfred.modules",
+        "alfred.fusion",
+        "alfred.vis.image",
+        "alfred.vis.image.pose_datasets",
+        "alfred.vis.pointcloud",
+        "alfred.vis.renders",
+        "alfred.vis.mesh3d",
+        "alfred.utils",
+        "alfred.siren",
+        "alfred.protos",
+        "alfred.deploy.tensorrt",
+    ],
+    # package_dir={'alfred': 'alfred'},
+    entry_points={"console_scripts": ["alfred = alfred.alfred:main"]},
+    include_package_data=True,
+    author="Lucas Jin",
+    author_email="jinfagang19@163.com",
+    url="https://github.com/jinfagang/alfred",
+    platforms="any",
+    install_requires=[
+        "colorama",
+        "natsort",
+        "requests",
+        "regex",
+        "funcy",
+        "pascal-voc-writer",
+        "markdown",
+        "future",
+        "deprecated",
+        "loguru",
+        "pyquaternion",
+        "jsons",
+        "natsort",
+        "loguru",
+        "pascal_voc_writer",
+        "funcy",
+        "gtrending",
+        "xdg",
+        "portalocker",
+    ],
+)
```

