# Comparing `tmp/gaea_operator-1.2.0.dev6-py3-none-any.whl.zip` & `tmp/gaea_operator-1.2.0.dev7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,113 +1,135 @@
-Zip file size: 147631 bytes, number of entries: 111
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/__init__.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/components/__init__.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/components/eval/__init__.py
--rw-r--r--  2.0 unx     4169 b- defN 24-Apr-22 03:05 gaea_operator/components/eval/ocrnet.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-22 03:05 gaea_operator/components/eval/ppyoloe_plus.py
--rw-r--r--  2.0 unx     4153 b- defN 24-Apr-22 03:05 gaea_operator/components/eval/resnet.py
--rw-r--r--  2.0 unx     3102 b- defN 24-Apr-22 03:05 gaea_operator/components/inference/__init__.py
--rw-r--r--  2.0 unx     4357 b- defN 24-Apr-22 03:05 gaea_operator/components/inference/inference.py
--rw-r--r--  2.0 unx     3550 b- defN 24-Apr-22 03:05 gaea_operator/components/package/__init__.py
--rw-r--r--  2.0 unx     8422 b- defN 24-Apr-22 03:05 gaea_operator/components/package/package.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/components/train/__init__.py
--rw-r--r--  2.0 unx     7519 b- defN 24-Apr-22 03:05 gaea_operator/components/train/ocrnet.py
--rw-r--r--  2.0 unx     8365 b- defN 24-Apr-22 03:05 gaea_operator/components/train/ppyoloe_plus.py
--rw-r--r--  2.0 unx     7390 b- defN 24-Apr-22 03:05 gaea_operator/components/train/resnet.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/components/transform/__init__.py
--rw-r--r--  2.0 unx     6236 b- defN 24-Apr-22 03:05 gaea_operator/components/transform/ocrnet.py
--rw-r--r--  2.0 unx     6078 b- defN 24-Apr-22 03:05 gaea_operator/components/transform/ppyoloe_plus.py
--rw-r--r--  2.0 unx     6214 b- defN 24-Apr-22 03:05 gaea_operator/components/transform/resnet.py
--rw-r--r--  2.0 unx     3557 b- defN 24-Apr-22 03:05 gaea_operator/components/transform_eval/__init__.py
--rw-r--r--  2.0 unx     8001 b- defN 24-Apr-22 03:05 gaea_operator/components/transform_eval/transform_eval.py
--rw-r--r--  2.0 unx      505 b- defN 24-Apr-22 03:05 gaea_operator/config/__init__.py
--rw-r--r--  2.0 unx     4883 b- defN 24-Apr-22 03:05 gaea_operator/config/config.py
--rw-r--r--  2.0 unx    14051 b- defN 24-Apr-22 03:05 gaea_operator/config/generate_transform_config.py
--rw-r--r--  2.0 unx    14835 b- defN 24-Apr-22 03:05 gaea_operator/config/modify_package_files.py
--rw-r--r--  2.0 unx     3642 b- defN 24-Apr-22 03:05 gaea_operator/config/update_parse.py
--rw-r--r--  2.0 unx    16721 b- defN 24-Apr-22 03:05 gaea_operator/config/update_pbtxt.py
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/ocrnet/__init__.py
--rw-r--r--  2.0 unx     5599 b- defN 24-Apr-22 03:05 gaea_operator/config/ocrnet/ocrnet_config.py
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/ocrnet/template/__init__.py
--rw-r--r--  2.0 unx     8809 b- defN 24-Apr-22 03:05 gaea_operator/config/ocrnet/template/modify_train_parameter.py
--rwxr-xr-x  2.0 unx     1467 b- defN 24-Apr-22 03:05 gaea_operator/config/ocrnet/template/parameter.yaml
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/__init__.py
--rw-r--r--  2.0 unx     4058 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/ppyoloeplus_config.py
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/template/__init__.py
--rw-r--r--  2.0 unx    12621 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/template/modify_train_parameter.py
--rw-r--r--  2.0 unx     4583 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/template/parameter.yaml
--rw-r--r--  2.0 unx     4666 b- defN 24-Apr-22 03:05 gaea_operator/config/ppyoloe_plus/template/parameter_c.yaml
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/resnet/__init__.py
--rw-r--r--  2.0 unx     4283 b- defN 24-Apr-22 03:05 gaea_operator/config/resnet/resnet_config.py
--rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 03:05 gaea_operator/config/resnet/template/__init__.py
--rw-r--r--  2.0 unx    11498 b- defN 24-Apr-22 03:05 gaea_operator/config/resnet/template/modify_train_parameter.py
--rw-r--r--  2.0 unx     2315 b- defN 24-Apr-22 03:05 gaea_operator/config/resnet/template/parameter.yaml
--rw-r--r--  2.0 unx      370 b- defN 24-Apr-22 03:05 gaea_operator/dataset/__init__.py
--rw-r--r--  2.0 unx     4259 b- defN 24-Apr-22 03:05 gaea_operator/dataset/cityscape_dataset.py
--rw-r--r--  2.0 unx     6508 b- defN 24-Apr-22 03:05 gaea_operator/dataset/coco_dataset.py
--rw-r--r--  2.0 unx     7314 b- defN 24-Apr-22 03:05 gaea_operator/dataset/dataset.py
--rw-r--r--  2.0 unx     4297 b- defN 24-Apr-22 03:05 gaea_operator/dataset/imagenet_dataset.py
--rw-r--r--  2.0 unx      584 b- defN 24-Apr-22 03:05 gaea_operator/metric/__init__.py
--rw-r--r--  2.0 unx     5740 b- defN 24-Apr-22 03:05 gaea_operator/metric/metric.py
--rw-r--r--  2.0 unx      433 b- defN 24-Apr-22 03:05 gaea_operator/metric/analysis/__init__.py
--rw-r--r--  2.0 unx    18968 b- defN 24-Apr-22 03:05 gaea_operator/metric/analysis/eval_metric_analysis.py
--rw-r--r--  2.0 unx     7907 b- defN 24-Apr-22 03:05 gaea_operator/metric/analysis/inference_metric_analysis.py
--rw-r--r--  2.0 unx    11706 b- defN 24-Apr-22 03:05 gaea_operator/metric/analysis/label_statistics_metric_analysis.py
--rw-r--r--  2.0 unx      792 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/__init__.py
--rw-r--r--  2.0 unx     3195 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/check.py
--rw-r--r--  2.0 unx     1923 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/metric.py
--rw-r--r--  2.0 unx      779 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/__init__.py
--rw-r--r--  2.0 unx     6960 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/accuracy.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/average_precision.py
--rw-r--r--  2.0 unx     5264 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/bbox_confusion_matrix.py
--rw-r--r--  2.0 unx     3939 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/confusion_matrix.py
--rw-r--r--  2.0 unx    20678 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/mean_ap.py
--rw-r--r--  2.0 unx     6128 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/mean_iou.py
--rw-r--r--  2.0 unx    19509 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/precision_recall_curve.py
--rw-r--r--  2.0 unx    11970 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/image/precision_recall_f1score.py
--rw-r--r--  2.0 unx      289 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/tabular/__init__.py
--rw-r--r--  2.0 unx     1207 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/tabular/count_statistic.py
--rw-r--r--  2.0 unx     2241 b- defN 24-Apr-22 03:05 gaea_operator/metric/operator/tabular/histogram_statistic.py
--rw-r--r--  2.0 unx     4864 b- defN 24-Apr-22 03:05 gaea_operator/metric/schema/object_detection.yaml
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/metric/types/__init__.py
--rw-r--r--  2.0 unx     1173 b- defN 24-Apr-22 03:05 gaea_operator/metric/types/image_classification_metric.py
--rw-r--r--  2.0 unx     4874 b- defN 24-Apr-22 03:05 gaea_operator/metric/types/metric.py
--rw-r--r--  2.0 unx     2362 b- defN 24-Apr-22 03:05 gaea_operator/metric/types/object_detection_metric.py
--rw-r--r--  2.0 unx     1244 b- defN 24-Apr-22 03:05 gaea_operator/metric/types/semantic_segmentation_metric.py
--rw-r--r--  2.0 unx      214 b- defN 24-Apr-22 03:05 gaea_operator/model/__init__.py
--rw-r--r--  2.0 unx     1436 b- defN 24-Apr-22 03:05 gaea_operator/model/model.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/__init__.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ocrnet_pipeline/__init__.py
--rw-r--r--  2.0 unx    12009 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py
--rw-r--r--  2.0 unx     1051 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml
--rw-r--r--  2.0 unx     1119 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ocrnet_pipeline/transform_parameter.yaml
--rw-r--r--  2.0 unx     1326 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ppyoloe_plus_pipeline/train_parameter.yaml
--rw-r--r--  2.0 unx     1815 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/ppyoloe_plus_pipeline/transform_parameter.yaml
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/resnet_pipeline/__init__.py
--rw-r--r--  2.0 unx    12187 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py
--rw-r--r--  2.0 unx     1271 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/resnet_pipeline/train_parameter.yaml
--rw-r--r--  2.0 unx     1121 b- defN 24-Apr-22 03:05 gaea_operator/pipelines/resnet_pipeline/transform_parameter.yaml
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-22 03:05 gaea_operator/trainer/__init__.py
--rw-r--r--  2.0 unx     5406 b- defN 24-Apr-22 03:05 gaea_operator/trainer/trainer.py
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-22 03:05 gaea_operator/transform/__init__.py
--rw-r--r--  2.0 unx     3307 b- defN 24-Apr-22 03:05 gaea_operator/transform/cvt_copy_model.py
--rw-r--r--  2.0 unx      776 b- defN 24-Apr-22 03:05 gaea_operator/transform/transform.py
--rw-r--r--  2.0 unx     1788 b- defN 24-Apr-22 03:05 gaea_operator/utils/__init__.py
--rw-r--r--  2.0 unx     5557 b- defN 24-Apr-22 03:05 gaea_operator/utils/accelerator.py
--rw-r--r--  2.0 unx     2887 b- defN 24-Apr-22 03:05 gaea_operator/utils/compress.py
--rw-r--r--  2.0 unx      426 b- defN 24-Apr-22 03:05 gaea_operator/utils/consts.py
--rw-r--r--  2.0 unx     1948 b- defN 24-Apr-22 03:05 gaea_operator/utils/file.py
--rw-r--r--  2.0 unx     1533 b- defN 24-Apr-22 03:05 gaea_operator/utils/import_module.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-22 03:05 gaea_operator/utils/model_template.py
--rw-r--r--  2.0 unx     1680 b- defN 24-Apr-22 03:05 gaea_operator/utils/registry.py
--rw-r--r--  2.0 unx     1000 b- defN 24-Apr-22 03:05 gaea_operator/utils/tensor.py
--rw-r--r--  2.0 unx      301 b- defN 24-Apr-22 03:05 gaea_operator/utils/time.py
--rw-r--r--  2.0 unx     4864 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.data/data/yaml/object_detection.yaml
--rw-r--r--  2.0 unx     4583 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.data/data/yaml/parameter.yaml
--rw-r--r--  2.0 unx     4666 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.data/data/yaml/parameter_c.yaml
--rw-r--r--  2.0 unx     1326 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.data/data/yaml/train_parameter.yaml
--rw-r--r--  2.0 unx     1815 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.data/data/yaml/transform_parameter.yaml
--rw-r--r--  2.0 unx     2173 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11343 b- defN 24-Apr-22 03:05 gaea_operator-1.2.0.dev6.dist-info/RECORD
-111 files, 469939 bytes uncompressed, 128993 bytes compressed:  72.6%
+Zip file size: 184965 bytes, number of entries: 133
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/components/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/__init__.py
+-rw-r--r--  2.0 unx     4731 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/codetr.py
+-rw-r--r--  2.0 unx     4597 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/convnext.py
+-rw-r--r--  2.0 unx     4169 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/ocrnet.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/ppyoloe_plus.py
+-rw-r--r--  2.0 unx     4153 b- defN 24-Apr-22 09:09 gaea_operator/components/eval/resnet.py
+-rw-r--r--  2.0 unx     3102 b- defN 24-Apr-22 09:09 gaea_operator/components/inference/__init__.py
+-rw-r--r--  2.0 unx     4357 b- defN 24-Apr-22 09:09 gaea_operator/components/inference/inference.py
+-rw-r--r--  2.0 unx     3550 b- defN 24-Apr-22 09:09 gaea_operator/components/package/__init__.py
+-rw-r--r--  2.0 unx     8422 b- defN 24-Apr-22 09:09 gaea_operator/components/package/package.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/components/train/__init__.py
+-rw-r--r--  2.0 unx     8618 b- defN 24-Apr-22 09:09 gaea_operator/components/train/codetr.py
+-rw-r--r--  2.0 unx     7854 b- defN 24-Apr-22 09:09 gaea_operator/components/train/convnext.py
+-rw-r--r--  2.0 unx     7519 b- defN 24-Apr-22 09:09 gaea_operator/components/train/ocrnet.py
+-rw-r--r--  2.0 unx     8365 b- defN 24-Apr-22 09:09 gaea_operator/components/train/ppyoloe_plus.py
+-rw-r--r--  2.0 unx     7390 b- defN 24-Apr-22 09:09 gaea_operator/components/train/resnet.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/__init__.py
+-rw-r--r--  2.0 unx     6209 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/codetr.py
+-rw-r--r--  2.0 unx     6219 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/convnext.py
+-rw-r--r--  2.0 unx     6236 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/ocrnet.py
+-rw-r--r--  2.0 unx     6078 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/ppyoloe_plus.py
+-rw-r--r--  2.0 unx     6214 b- defN 24-Apr-22 09:09 gaea_operator/components/transform/resnet.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-Apr-22 09:09 gaea_operator/components/transform_eval/__init__.py
+-rw-r--r--  2.0 unx     8001 b- defN 24-Apr-22 09:09 gaea_operator/components/transform_eval/transform_eval.py
+-rw-r--r--  2.0 unx      690 b- defN 24-Apr-22 09:09 gaea_operator/config/__init__.py
+-rw-r--r--  2.0 unx     4964 b- defN 24-Apr-22 09:09 gaea_operator/config/config.py
+-rw-r--r--  2.0 unx    14830 b- defN 24-Apr-22 09:09 gaea_operator/config/generate_transform_config.py
+-rw-r--r--  2.0 unx    14835 b- defN 24-Apr-22 09:09 gaea_operator/config/modify_package_files.py
+-rw-r--r--  2.0 unx     3642 b- defN 24-Apr-22 09:09 gaea_operator/config/update_parse.py
+-rw-r--r--  2.0 unx    16721 b- defN 24-Apr-22 09:09 gaea_operator/config/update_pbtxt.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/__init__.py
+-rw-r--r--  2.0 unx     5352 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/codetr_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/template/__init__.py
+-rw-r--r--  2.0 unx      590 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/template/deploy_parameter.yaml
+-rw-r--r--  2.0 unx    14292 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/template/modify_parameter.py
+-rw-r--r--  2.0 unx    13658 b- defN 24-Apr-22 09:09 gaea_operator/config/codetr/template/train_parameter.yaml
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/convnext/__init__.py
+-rw-r--r--  2.0 unx     3999 b- defN 24-Apr-22 09:09 gaea_operator/config/convnext/convnext_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/convnext/template/__init__.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-22 09:09 gaea_operator/config/convnext/template/modify_train_parameter.py
+-rw-r--r--  2.0 unx     1356 b- defN 24-Apr-22 09:09 gaea_operator/config/convnext/template/parameter.yaml
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/ocrnet/__init__.py
+-rw-r--r--  2.0 unx     5599 b- defN 24-Apr-22 09:09 gaea_operator/config/ocrnet/ocrnet_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/ocrnet/template/__init__.py
+-rw-r--r--  2.0 unx     8809 b- defN 24-Apr-22 09:09 gaea_operator/config/ocrnet/template/modify_train_parameter.py
+-rwxr-xr-x  2.0 unx     1467 b- defN 24-Apr-22 09:09 gaea_operator/config/ocrnet/template/parameter.yaml
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/__init__.py
+-rw-r--r--  2.0 unx     4058 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/ppyoloeplus_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/template/__init__.py
+-rw-r--r--  2.0 unx    12621 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/template/modify_train_parameter.py
+-rw-r--r--  2.0 unx     4583 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/template/parameter.yaml
+-rw-r--r--  2.0 unx     4666 b- defN 24-Apr-22 09:09 gaea_operator/config/ppyoloe_plus/template/parameter_c.yaml
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/resnet/__init__.py
+-rw-r--r--  2.0 unx     4283 b- defN 24-Apr-22 09:09 gaea_operator/config/resnet/resnet_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-22 09:09 gaea_operator/config/resnet/template/__init__.py
+-rw-r--r--  2.0 unx    11498 b- defN 24-Apr-22 09:09 gaea_operator/config/resnet/template/modify_train_parameter.py
+-rw-r--r--  2.0 unx     2315 b- defN 24-Apr-22 09:09 gaea_operator/config/resnet/template/parameter.yaml
+-rw-r--r--  2.0 unx      370 b- defN 24-Apr-22 09:09 gaea_operator/dataset/__init__.py
+-rw-r--r--  2.0 unx     4259 b- defN 24-Apr-22 09:09 gaea_operator/dataset/cityscape_dataset.py
+-rw-r--r--  2.0 unx     6521 b- defN 24-Apr-22 09:09 gaea_operator/dataset/coco_dataset.py
+-rw-r--r--  2.0 unx     7314 b- defN 24-Apr-22 09:09 gaea_operator/dataset/dataset.py
+-rw-r--r--  2.0 unx     4311 b- defN 24-Apr-22 09:09 gaea_operator/dataset/imagenet_dataset.py
+-rw-r--r--  2.0 unx      584 b- defN 24-Apr-22 09:09 gaea_operator/metric/__init__.py
+-rw-r--r--  2.0 unx     5740 b- defN 24-Apr-22 09:09 gaea_operator/metric/metric.py
+-rw-r--r--  2.0 unx      433 b- defN 24-Apr-22 09:09 gaea_operator/metric/analysis/__init__.py
+-rw-r--r--  2.0 unx    18968 b- defN 24-Apr-22 09:09 gaea_operator/metric/analysis/eval_metric_analysis.py
+-rw-r--r--  2.0 unx     7907 b- defN 24-Apr-22 09:09 gaea_operator/metric/analysis/inference_metric_analysis.py
+-rw-r--r--  2.0 unx    11706 b- defN 24-Apr-22 09:09 gaea_operator/metric/analysis/label_statistics_metric_analysis.py
+-rw-r--r--  2.0 unx      792 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/__init__.py
+-rw-r--r--  2.0 unx     3195 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/check.py
+-rw-r--r--  2.0 unx     1923 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/metric.py
+-rw-r--r--  2.0 unx      779 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/__init__.py
+-rw-r--r--  2.0 unx     6960 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/accuracy.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/average_precision.py
+-rw-r--r--  2.0 unx     5264 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/bbox_confusion_matrix.py
+-rw-r--r--  2.0 unx     3939 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/confusion_matrix.py
+-rw-r--r--  2.0 unx    20678 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/mean_ap.py
+-rw-r--r--  2.0 unx     6128 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/mean_iou.py
+-rw-r--r--  2.0 unx    19509 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/precision_recall_curve.py
+-rw-r--r--  2.0 unx    11970 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/image/precision_recall_f1score.py
+-rw-r--r--  2.0 unx      289 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/tabular/__init__.py
+-rw-r--r--  2.0 unx     1207 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/tabular/count_statistic.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-Apr-22 09:09 gaea_operator/metric/operator/tabular/histogram_statistic.py
+-rw-r--r--  2.0 unx     4864 b- defN 24-Apr-22 09:09 gaea_operator/metric/schema/object_detection.yaml
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/metric/types/__init__.py
+-rw-r--r--  2.0 unx     1173 b- defN 24-Apr-22 09:09 gaea_operator/metric/types/image_classification_metric.py
+-rw-r--r--  2.0 unx     4874 b- defN 24-Apr-22 09:09 gaea_operator/metric/types/metric.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-Apr-22 09:09 gaea_operator/metric/types/object_detection_metric.py
+-rw-r--r--  2.0 unx     1244 b- defN 24-Apr-22 09:09 gaea_operator/metric/types/semantic_segmentation_metric.py
+-rw-r--r--  2.0 unx      214 b- defN 24-Apr-22 09:09 gaea_operator/model/__init__.py
+-rw-r--r--  2.0 unx     1436 b- defN 24-Apr-22 09:09 gaea_operator/model/model.py
+-rw-r--r--  2.0 unx      446 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/codetr_pipeline/__init__.py
+-rw-r--r--  2.0 unx    12171 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/codetr_pipeline/codetr_pipeline.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/convnext_pipeline/__init__.py
+-rw-r--r--  2.0 unx    11860 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/convnext_pipeline/convnext_pipeline.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ocrnet_pipeline/__init__.py
+-rw-r--r--  2.0 unx    12008 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py
+-rw-r--r--  2.0 unx     1051 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml
+-rw-r--r--  2.0 unx     1119 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ocrnet_pipeline/transform_parameter.yaml
+-rw-r--r--  2.0 unx     1326 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ppyoloe_plus_pipeline/train_parameter.yaml
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/ppyoloe_plus_pipeline/transform_parameter.yaml
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/resnet_pipeline/__init__.py
+-rw-r--r--  2.0 unx    12187 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py
+-rw-r--r--  2.0 unx     1271 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/resnet_pipeline/train_parameter.yaml
+-rw-r--r--  2.0 unx     1121 b- defN 24-Apr-22 09:09 gaea_operator/pipelines/resnet_pipeline/transform_parameter.yaml
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-22 09:09 gaea_operator/trainer/__init__.py
+-rw-r--r--  2.0 unx     6818 b- defN 24-Apr-22 09:09 gaea_operator/trainer/trainer.py
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-22 09:09 gaea_operator/transform/__init__.py
+-rw-r--r--  2.0 unx     3307 b- defN 24-Apr-22 09:09 gaea_operator/transform/cvt_copy_model.py
+-rw-r--r--  2.0 unx      776 b- defN 24-Apr-22 09:09 gaea_operator/transform/transform.py
+-rw-r--r--  2.0 unx     1866 b- defN 24-Apr-22 09:09 gaea_operator/utils/__init__.py
+-rw-r--r--  2.0 unx     5557 b- defN 24-Apr-22 09:09 gaea_operator/utils/accelerator.py
+-rw-r--r--  2.0 unx     2887 b- defN 24-Apr-22 09:09 gaea_operator/utils/compress.py
+-rw-r--r--  2.0 unx      532 b- defN 24-Apr-22 09:09 gaea_operator/utils/consts.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-22 09:09 gaea_operator/utils/file.py
+-rw-r--r--  2.0 unx     1533 b- defN 24-Apr-22 09:09 gaea_operator/utils/import_module.py
+-rw-r--r--  2.0 unx    10020 b- defN 24-Apr-22 09:09 gaea_operator/utils/model_template.py
+-rw-r--r--  2.0 unx     1680 b- defN 24-Apr-22 09:09 gaea_operator/utils/registry.py
+-rw-r--r--  2.0 unx     1000 b- defN 24-Apr-22 09:09 gaea_operator/utils/tensor.py
+-rw-r--r--  2.0 unx      301 b- defN 24-Apr-22 09:09 gaea_operator/utils/time.py
+-rw-r--r--  2.0 unx      590 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/deploy_parameter.yaml
+-rw-r--r--  2.0 unx     4864 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/object_detection.yaml
+-rw-r--r--  2.0 unx     1356 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/parameter.yaml
+-rw-r--r--  2.0 unx     4666 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/parameter_c.yaml
+-rw-r--r--  2.0 unx    13658 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/train_parameter.yaml
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.data/data/yaml/transform_parameter.yaml
+-rw-r--r--  2.0 unx     2173 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13690 b- defN 24-Apr-22 09:09 gaea_operator-1.2.0.dev7.dist-info/RECORD
+133 files, 594788 bytes uncompressed, 162465 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -3,14 +3,20 @@
 
 Filename: gaea_operator/components/__init__.py
 Comment: 
 
 Filename: gaea_operator/components/eval/__init__.py
 Comment: 
 
+Filename: gaea_operator/components/eval/codetr.py
+Comment: 
+
+Filename: gaea_operator/components/eval/convnext.py
+Comment: 
+
 Filename: gaea_operator/components/eval/ocrnet.py
 Comment: 
 
 Filename: gaea_operator/components/eval/ppyoloe_plus.py
 Comment: 
 
 Filename: gaea_operator/components/eval/resnet.py
@@ -27,26 +33,38 @@
 
 Filename: gaea_operator/components/package/package.py
 Comment: 
 
 Filename: gaea_operator/components/train/__init__.py
 Comment: 
 
+Filename: gaea_operator/components/train/codetr.py
+Comment: 
+
+Filename: gaea_operator/components/train/convnext.py
+Comment: 
+
 Filename: gaea_operator/components/train/ocrnet.py
 Comment: 
 
 Filename: gaea_operator/components/train/ppyoloe_plus.py
 Comment: 
 
 Filename: gaea_operator/components/train/resnet.py
 Comment: 
 
 Filename: gaea_operator/components/transform/__init__.py
 Comment: 
 
+Filename: gaea_operator/components/transform/codetr.py
+Comment: 
+
+Filename: gaea_operator/components/transform/convnext.py
+Comment: 
+
 Filename: gaea_operator/components/transform/ocrnet.py
 Comment: 
 
 Filename: gaea_operator/components/transform/ppyoloe_plus.py
 Comment: 
 
 Filename: gaea_operator/components/transform/resnet.py
@@ -72,14 +90,47 @@
 
 Filename: gaea_operator/config/update_parse.py
 Comment: 
 
 Filename: gaea_operator/config/update_pbtxt.py
 Comment: 
 
+Filename: gaea_operator/config/codetr/__init__.py
+Comment: 
+
+Filename: gaea_operator/config/codetr/codetr_config.py
+Comment: 
+
+Filename: gaea_operator/config/codetr/template/__init__.py
+Comment: 
+
+Filename: gaea_operator/config/codetr/template/deploy_parameter.yaml
+Comment: 
+
+Filename: gaea_operator/config/codetr/template/modify_parameter.py
+Comment: 
+
+Filename: gaea_operator/config/codetr/template/train_parameter.yaml
+Comment: 
+
+Filename: gaea_operator/config/convnext/__init__.py
+Comment: 
+
+Filename: gaea_operator/config/convnext/convnext_config.py
+Comment: 
+
+Filename: gaea_operator/config/convnext/template/__init__.py
+Comment: 
+
+Filename: gaea_operator/config/convnext/template/modify_train_parameter.py
+Comment: 
+
+Filename: gaea_operator/config/convnext/template/parameter.yaml
+Comment: 
+
 Filename: gaea_operator/config/ocrnet/__init__.py
 Comment: 
 
 Filename: gaea_operator/config/ocrnet/ocrnet_config.py
 Comment: 
 
 Filename: gaea_operator/config/ocrnet/template/__init__.py
@@ -225,14 +276,26 @@
 
 Filename: gaea_operator/model/model.py
 Comment: 
 
 Filename: gaea_operator/pipelines/__init__.py
 Comment: 
 
+Filename: gaea_operator/pipelines/codetr_pipeline/__init__.py
+Comment: 
+
+Filename: gaea_operator/pipelines/codetr_pipeline/codetr_pipeline.py
+Comment: 
+
+Filename: gaea_operator/pipelines/convnext_pipeline/__init__.py
+Comment: 
+
+Filename: gaea_operator/pipelines/convnext_pipeline/convnext_pipeline.py
+Comment: 
+
 Filename: gaea_operator/pipelines/ocrnet_pipeline/__init__.py
 Comment: 
 
 Filename: gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py
 Comment: 
 
 Filename: gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml
@@ -300,35 +363,38 @@
 
 Filename: gaea_operator/utils/tensor.py
 Comment: 
 
 Filename: gaea_operator/utils/time.py
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.data/data/yaml/object_detection.yaml
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/deploy_parameter.yaml
+Comment: 
+
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/object_detection.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.data/data/yaml/parameter.yaml
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.data/data/yaml/parameter_c.yaml
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/parameter_c.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.data/data/yaml/train_parameter.yaml
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/train_parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.data/data/yaml/transform_parameter.yaml
+Filename: gaea_operator-1.2.0.dev7.data/data/yaml/transform_parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.dist-info/METADATA
+Filename: gaea_operator-1.2.0.dev7.dist-info/METADATA
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.dist-info/WHEEL
+Filename: gaea_operator-1.2.0.dev7.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.dist-info/top_level.txt
+Filename: gaea_operator-1.2.0.dev7.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev6.dist-info/RECORD
+Filename: gaea_operator-1.2.0.dev7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaea_operator/config/__init__.py

```diff
@@ -5,12 +5,15 @@
 # @Author  : yanxiaodong
 # @File    : __init__.py.py
 """
 from gaea_operator.config.config import Config
 from gaea_operator.config.ppyoloe_plus.ppyoloeplus_config import PPYOLOEPLUSMConfig
 from gaea_operator.config.resnet.resnet_config import ResNetConfig
 from gaea_operator.config.ocrnet.ocrnet_config import OCRNetConfig
+from gaea_operator.config.convnext.convnext_config import ConvNextConfig
+from gaea_operator.config.codetr.codetr_config import CoDETRConfig
 
 __all__ = ["PPYOLOEPLUSMConfig",
            "Config",
            "ResNetConfig",
-           "OCRNetConfig"]
+           "OCRNetConfig",
+           "ConvNextConfig", "CoDETRConfig"]
```

## gaea_operator/config/config.py

```diff
@@ -110,18 +110,20 @@
             advanced_parameters[KEY_EVAL_HEIGHT] = height
 
         input_size = InputSize(width=int(advanced_parameters[KEY_EVAL_WIDTH]),
                                height=int(advanced_parameters[KEY_EVAL_HEIGHT]))
 
         meta_data = ModelMetadata(**self._metadata)
         meta_data.inputSize = input_size
-        meta_data.maxBoxNum = int(advanced_parameters[KEY_MAX_BOX_NUM])
+        maxBoxNum = int(advanced_parameters[KEY_MAX_BOX_NUM]) \
+                                if KEY_MAX_BOX_NUM in advanced_parameters else 1
+        meta_data.maxBoxNum = maxBoxNum
         advanced_parameters = {
             'inferenceMaxBatchSize': int(advanced_parameters[KEY_MAX_BATCH_SIZE]),
-            'maxBoxNum': int(advanced_parameters[KEY_MAX_BOX_NUM]),
+            'maxBoxNum': maxBoxNum,
             'evalWidth': int(advanced_parameters[KEY_EVAL_WIDTH]),
             'evalHeight': int(advanced_parameters[KEY_EVAL_HEIGHT])}
 
         if meta_data.algorithmParameters is None:
             meta_data.algorithmParameters = advanced_parameters
         else:
             meta_data.algorithmParameters.update(advanced_parameters)
```

## gaea_operator/config/generate_transform_config.py

```diff
@@ -19,15 +19,16 @@
 MODEL_NAME_DICT = {"ppyoloe": ["image", "scale_factor"],
                    "change-ppyoloe": ["image", "tmp_image", "scale_factor"],
                    "vit-base": ["x"],
                    "resnet": ["x"],
                    "ocrnet": ["x"],
                    "maskformer": ["x"],
                    "change-ocrnet": ["x", "tmp_image"],
-                   "co-detr": ["x"]
+                   "convnext": ["input"], 
+                   "codetr": ["input"]
                    }
 
 KEY_SOURCE_FRAMEWORK = 'source_framework'
 KEY_ACCELERATOR = 'accelerator'
 KEY_MODEL_TYPE = 'model_type'
 KEY_EVAL_WIDTH = 'eval_width'
 KEY_EVAL_HEIGHT = 'eval_height'
@@ -83,32 +84,35 @@
     batch = -1 if max_batch_size > 1 else 1
     input_shape = {}
     if '_' in model_name:
         model_name = model_name[: -2]
         bcelogger.info('modify model name -> {}'.format(model_name))
 
     if model_name not in MODEL_NAME_DICT.keys():
-        raise ValueError("model name not in model list")
-        return
+        raise ValueError("model name:{} not in model list".format(model_name))
     if "ppyoloe" in model_name:
         input_shape = {"image": [batch, 3, height, width], "scale_factor": [batch, 2]}
         if "change" in model_name:
             input_shape["tmp_image"] = [batch, 3, height, width]
     elif "vit-base" in model_name or "resnet" in model_name:
         input_shape["x"] = [batch, 3, height, width]
     elif "maskformer" in model_name or \
             "ocrnet" in model_name:
         bcelogger.warning("maskformer and ocrnet not support batchsize > 1")
         batch = 1
         input_shape['x'] = [batch, 3, height, width]
         if "change" in model_name:
             input_shape['x'] = [batch, 6, height, width]
+    elif "convnext" in model_name:
+        input_shape['input'] = [batch, 3, height, width]
+    elif "codetr" in model_name:
+        input_shape['input'] = [1, 3, height, width]
+        bcelogger.warning("codetr not support batchsize > 1")
     else:
         raise ValueError("model name not in model list")
-        return
     return input_shape
 
 
 def _trans_shape(input_shape: dict) -> dict:
     """
     trans shape 
     """
@@ -272,17 +276,26 @@
                 start_param += name
                 start_param += ":"
                 start_param += shape
                 start_param += ","
             start_param = start_param[:-1]
             cmd += start_param + " "
         if min_batch == max_batch:
-            cmd = f" --workspace=2048 --{advanced_parameters[KEY_PRECISION]}"
+            cmd = f" --workspace=12288"
+        else:
+            cmd += f" --workspace=12288"
+        if KEY_PRECISION not in advanced_parameters or \
+            advanced_parameters[KEY_PRECISION].lower() in ["fp32", "float32"]:
+            pass
         else:
-            cmd += f" --workspace=2048 --{advanced_parameters[KEY_PRECISION]}"
+            if KEY_PRECISION in advanced_parameters:
+                cmd += f" --{advanced_parameters[KEY_PRECISION]}"
+        model_type = advanced_parameters[KEY_MODEL_TYPE].lower()
+        if model_type in ['codetr']:
+            cmd += f" --staticPlugins=/usr/src/tensorrt/plugins/libmmdeploy_tensorrt_ops.so"
         bcelogger.info(f"OnnxToTensorrt cmd = {cmd}")
 
         OnnxToTensorrtParam["cmd"] = cmd
 
         pipeline_cfg.append(OnnxToTensorrtParam)
     # bitmain
     else:
@@ -315,14 +328,16 @@
     """
     yaml_data = metadata
     model_input_name = ['x']
     if 'ppyoloe' in model_name:
         model_input_name = ['image']
     if 'change' in model_name:
         model_input_name.append('tmp_image')
+    if 'convnext' in model_name or 'codetr' in model_name:
+        model_input_name = ['input']
 
     if 'artifact' in yaml_data and 'metadata' in yaml_data['artifact'] \
             and 'algorithmParameters' in yaml_data['artifact']['metadata']:
         alg_param = yaml_data['artifact']['metadata']['algorithmParameters']
     elif 'algorithmParameters' in yaml_data:
         alg_param = yaml_data['algorithmParameters']
     else:
@@ -341,16 +356,16 @@
 
 def generate_transform_config(advanced_parameters: dict, config_name: str, metadata: Dict):
     """
     Create a config file for the specific model
     """
     model_name = advanced_parameters[KEY_MODEL_TYPE].lower()
     mean, std = get_mean_std(metadata, model_name)
-    input_shape = gen_input_shape(model_name, int(advanced_parameters[KEY_EVAL_HEIGHT]), \
-                                  int(advanced_parameters[KEY_EVAL_WIDTH]), \
+    input_shape = gen_input_shape(model_name, int(advanced_parameters[KEY_EVAL_WIDTH]), \
+                                  int(advanced_parameters[KEY_EVAL_HEIGHT]), \
                                   int(advanced_parameters[KEY_MAX_BATCH_SIZE]))
 
     bcelogger.info(str(input_shape))
     norm, transpose = get_norm_transpose(advanced_parameters[KEY_ACCELERATOR])
 
     create_common_config(advanced_parameters,
                          input_shape=input_shape,
```

## gaea_operator/dataset/coco_dataset.py

```diff
@@ -70,15 +70,15 @@
 
         raw_data_list = []
         for file in annotation_file_list:
             json_data = json.load(open(file, "r"))
             images = json_data["images"]
 
             bcelogger.info(f"Parse annotation file {file}, image num is {len(images)}")
-
+            
             for img in images:
                 img["file_name"] = self._file_name_cvt_abs(img["file_name"], file, base_uri, 2, work_dir)
                 self.image_set.add(img["file_name"])
 
             raw_data_list.append(json_data)
 
         return raw_data_list
@@ -100,15 +100,15 @@
         with open(file_path, "w") as fp:
             json.dump(raw_data, fp, separators=(",", ":"))
 
     def _coco_data_raw_concat(self, raw_data: List[Dict]):
         cat_name2id = self._category_valid(raw_data)
 
         raw_data_coco = {"images": [], "annotations": [], "categories": []}
-        max_ann_id = 1
+        max_ann_id = -1
         new_im_id = 1
 
         categories = []
         for cat in raw_data[0]["categories"]:
             cat["id"] = int(cat["id"])
             categories.append(cat)
         raw_data_coco["categories"] = categories
```

## gaea_operator/dataset/imagenet_dataset.py

```diff
@@ -72,15 +72,15 @@
         label_name2id = self._category_valid(label_list)
 
         raw_data_imagenet = []
 
         for idx, data in enumerate(raw_data):
             old2new_cat_id = {}
             for inner_idx, label in enumerate(label_list[idx]):
-                label_name, label_id = label.split(" ")[0], label.split(" ")[1]
+                label_name, label_id = label.strip().split(" ")[0], label.strip().split(" ")[1]
                 if label_id != label_name2id[label_name]:
                     old2new_cat_id[label_id] = label_name2id[label_name]
             for item in data:
                 img_file, label_id = item.strip("\"").rsplit(" ", 1)
                 label_id = int(label_id)
                 if label_id in old2new_cat_id:
                     label_id = old2new_cat_id[label_id]
@@ -106,9 +106,8 @@
                 for inner_idx, label in enumerate(label_list[idx]):
                     if label != label_list[0][inner_idx]:
                         raise ValueError(f"The labels name is not equal, please check {label_list}")
             self.labels = [{"id": str(name.split(" ")[1]), "name": name.split(" ")[0]} for name in label_list[0]]
             bcelogger.info(f"The labels is {self.labels}")
             return {name.split(" ")[0]: name.split(" ")[1] for name in label_list[0]}
         else:
-            raise ValueError(f"The number of labels is not equal, please check {label_list}")
-
+            raise ValueError(f"The number of labels is not equal, please check {label_list}")
```

## gaea_operator/pipelines/__init__.py

```diff
@@ -1,7 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-# @Time    : 2024/4/18
-# @Author  : yanxiaodong
-# @File    : __init__.py.py
+__init__.py
 """
+
+from gaea_operator.pipelines.ocrnet_pipeline.ocrnet_pipeline import pipeline as ocrnet_pipeline
+from gaea_operator.pipelines.ppyoloe_plus_pipeline.ppyoloe_plus_pipeline import pipeline as ppyoloe_plus_pipeline
+from gaea_operator.pipelines.resnet_pipeline.resnet_pipeline import pipeline as resnet_pipeline
+
+ppls = [ocrnet_pipeline(), ppyoloe_plus_pipeline(), resnet_pipeline()]
```

## gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py

```diff
@@ -12,15 +12,14 @@
 from gaea_operator.utils import DEFAULT_TRAIN_CONFIG_FILE_NAME, \
     DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME, \
     ModelTemplate
 from gaea_operator.components.transform_eval import transform_eval_step
 from gaea_operator.components.package import package_step
 from gaea_operator.components.inference import inference_step
 
-
 @Pipeline(
     name="ocrnet",
     cache_options=CacheOptions(enable=False),
 )
 def pipeline(accelerator: str = "T4",
              extra_fs_name: str = "vistudio",
              extra_fs_mount_path: str = "/home/paddleflow/storage/mnt/fs-root-vistudio",
```

## gaea_operator/trainer/trainer.py

```diff
@@ -11,15 +11,16 @@
 import time
 import threading
 
 from gaea_tracker import ExperimentTracker
 
 from gaea_operator.metric.types.metric import LOSS_METRIC_NAME
 from gaea_operator.metric import get_score_from_metric_raw
-from gaea_operator.utils import read_file, DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME, DEFAULT_TRAIN_CONFIG_FILE_NAME
+from gaea_operator.utils import read_file, DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME, DEFAULT_TRAIN_CONFIG_FILE_NAME, \
+    DEFAULT_PYTORCH_MODEL_FILE_NAME, DEFAULT_DEPLOY_CONFIG_FILE_NAME
 
 
 class Trainer(object):
     """
     Trainer class for different framework.
     """
     framework_paddlepaddle = "PaddlePaddle"
@@ -51,14 +52,29 @@
             bcelogger.error(f"PaddleDetection training failed: {e}")
             raise e
         finally:
             self.training_exit_flag = True
             if self.thread is not None:
                 self.thread.join()
 
+    def pytorch_launch(self):
+        """
+        Launch the Pytorch training process.
+        """
+        from torch.distributed.run import main
+        try:
+            main()
+        except Exception as e:
+            bcelogger.error(f"Pytorch launch training failed: {e}")
+            raise e
+        finally:
+            self.training_exit_flag = True
+            if self.thread is not None:
+                self.thread.join()
+
     def paddledet_export(self, model_dir: str):
         """
         Export the model to static.
         """
         from paddledet.tools import export_model
         weights = os.path.join(model_dir, DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME)
         export_model.main(weights=weights, output_dir=model_dir)
@@ -79,14 +95,32 @@
         from paddleseg.tools import export_model
         weights = os.path.join(model_dir, DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME)
         config = os.path.join(model_dir, DEFAULT_TRAIN_CONFIG_FILE_NAME)
         bcelogger.info('cofnig: {} model_path: {} save_dir: {} input_shape: {}'.format(config, 
                                                                                    weights, model_dir, input_shape))
         export_model.main(config=config, model_path=weights, save_dir=model_dir, input_shape=input_shape)
 
+    def convnext_export(self, model_dir: str):
+        """
+        Export the model to onnx."""
+        config = os.path.join(model_dir, DEFAULT_TRAIN_CONFIG_FILE_NAME)
+        weights = os.path.join(model_dir, DEFAULT_PYTORCH_MODEL_FILE_NAME)
+        from convnext.tools import export_model
+        export_model.main(config_file=config, weight_path=weights, output_dir=model_dir)
+
+    def codetr_export(self, model_dir: str):
+        """
+        Export the model to onnx."""
+        train_cfg = os.path.join(model_dir, DEFAULT_TRAIN_CONFIG_FILE_NAME)
+        deploy_cfg = os.path.join(model_dir, DEFAULT_DEPLOY_CONFIG_FILE_NAME)
+        weights = os.path.join(model_dir, DEFAULT_PYTORCH_MODEL_FILE_NAME)
+        from mmdet.tools.codetr_torch2onnx import torch2onnx
+        torch2onnx(model_dir, 'best_model.onnx', deploy_cfg, train_cfg, weights, 
+                    device='cpu', run_mode='predict_out')
+
     @classmethod
     def _framework_check(cls, framework: str):
         frameworks = [cls.framework_paddlepaddle, cls.framework_pytorch]
         bcelogger.info(f"framework: {framework}")
 
         assert framework in frameworks, f"framework must be one of {frameworks}, but get framework {framework}"
```

## gaea_operator/utils/__init__.py

```diff
@@ -6,15 +6,17 @@
 # @File    : __init__.py.py
 """
 from .consts import DEFAULT_TRAIN_CONFIG_FILE_NAME, \
     DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME, \
     DEFAULT_TRANSFORM_CONFIG_FILE_NAME, \
     DEFAULT_META_FILE_NAME, \
     DEFAULT_METRIC_FILE_NAME, \
-    DEFAULT_TRITON_CONFIG_FILE_NAME
+    DEFAULT_TRITON_CONFIG_FILE_NAME, \
+    DEFAULT_PYTORCH_MODEL_FILE_NAME, \
+    DEFAULT_DEPLOY_CONFIG_FILE_NAME
 from .file import find_upper_level_folder, \
     write_file, \
     read_file, \
     read_yaml_file, \
     write_yaml_file, \
     find_dir
 from .compress import get_filepaths_in_archive
```

## gaea_operator/utils/consts.py

```diff
@@ -3,11 +3,13 @@
 """
 # @Time    : 2024/3/8
 # @Author  : yanxiaodong
 # @File    : consts.py
 """
 DEFAULT_TRAIN_CONFIG_FILE_NAME = "train_config.yaml"
 DEFAULT_TRANSFORM_CONFIG_FILE_NAME = "transform_config.yaml"
+DEFAULT_DEPLOY_CONFIG_FILE_NAME = "deploy_config.yaml"
 DEFAULT_META_FILE_NAME = "meta.yaml"
 DEFAULT_METRIC_FILE_NAME = "metric.json"
 DEFAULT_PADDLEPADDLE_MODEL_FILE_NAME = "best_model.pdparams"
-DEFAULT_TRITON_CONFIG_FILE_NAME = "config.pbtxt"
+DEFAULT_TRITON_CONFIG_FILE_NAME = "config.pbtxt"
+DEFAULT_PYTORCH_MODEL_FILE_NAME = "best_model.pth"
```

## gaea_operator/utils/file.py

```diff
@@ -43,17 +43,20 @@
         yaml.dump(obj, f, allow_unicode=True, sort_keys=False)
 
 
 def read_file(input_dir: str, file_name: str = "response.json"):
     """
     Read the response list from a file.
     """
-    with open(os.path.join(input_dir, file_name), "r") as f:
+    file_path = os.path.join(input_dir, file_name)
+    if not os.path.exists(file_path):
+        raise FileNotFoundError(f"File {file_path} does not exist.")
+    data = None
+    with open(file_path, "r", encoding='utf-8') as f:
         data = json.load(f)
-
     return data
 
 
 def read_yaml_file(input_dir: str, file_name: str = "response.yaml"):
     """
     Read the response list from a file.
     """
```

## gaea_operator/utils/model_template.py

```diff
@@ -13,14 +13,16 @@
 class ModelTemplate(metaclass=ABCMeta):
     """
     Algorithm class
     """
     PPYOLOE_PLUS_NAME = 'ppyoloe_plus'
     RESNET_NAME = 'resnet'
     OCRNET_NAME = 'ocrnet'
+    CONVNEXT_NAME = 'convnext'
+    CODETR_NAME = 'codetr'
 
     def __init__(self, model_store_name: str):
         model_store = parse_modelstore_name(model_store_name)
         self.workspace_id = model_store.workspace_id
         self.model_store_name = model_store.local_name
 
     @abstractmethod
@@ -180,19 +182,110 @@
         """
         model_name = ModelName(workspace_id=self.workspace_id,
                                model_store_name=self.model_store_name,
                                local_name="ocrnet-ensemble")
         return model_name.get_name()
 
 
+class ConvNextTemplate(ModelTemplate):
+    """
+    ResNet Algorithm class
+    """
+    def __init__(self, model_store_name):
+        super(ConvNextTemplate, self).__init__(model_store_name=model_store_name)
+
+    def suggest_template_preprocess(self):
+        """
+        Get template name for preprocess
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="convnext-preprocess")
+        return model_name.get_name()
+
+    def suggest_template_postprocess(self):
+        """
+        Get template name for postprocess
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="convnext-postprocess")
+        return model_name.get_name()
+
+    def suggest_template_model(self):
+        """
+        Get template name for model
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="convnext-model")
+        return model_name.get_name()
+
+    def suggest_template_ensemble(self):
+        """
+        Get template name for ensemble
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="convnext-ensemble")
+        return model_name.get_name()
+
+
+class CoDETRTemplate(ModelTemplate):
+    """
+    ResNet Algorithm class
+    """
+    def __init__(self, model_store_name):
+        super(CoDETRTemplate, self).__init__(model_store_name=model_store_name)
+
+    def suggest_template_preprocess(self):
+        """
+        Get template name for preprocess
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="codetr-preprocess")
+        return model_name.get_name()
+
+    def suggest_template_postprocess(self):
+        """
+        Get template name for postprocess
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="codetr-postprocess")
+        return model_name.get_name()
+
+    def suggest_template_model(self):
+        """
+        Get template name for model
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="codetr-model")
+        return model_name.get_name()
+
+    def suggest_template_ensemble(self):
+        """
+        Get template name for ensemble
+        """
+        model_name = ModelName(workspace_id=self.workspace_id,
+                               model_store_name=self.model_store_name,
+                               local_name="codetr-ensemble")
+        return model_name.get_name()
+
 def get_model_template(name: str, model_store_name: str):
     """
     Get algorithm class by name
     """
     if name == ModelTemplate.PPYOLOE_PLUS_NAME:
         return PPYOLOEPLUSTemplate(model_store_name=model_store_name)
     elif name == ModelTemplate.RESNET_NAME:
         return ResNetTemplate(model_store_name=model_store_name)
     elif name == ModelTemplate.OCRNET_NAME:
         return OCRNetTemplate(model_store_name=model_store_name)
+    elif name == ModelTemplate.CONVNEXT_NAME:
+        return ConvNextTemplate(model_store_name=model_store_name)
+    elif name == ModelTemplate.CODETR_NAME:
+        return CoDETRTemplate(model_store_name=model_store_name)
     else:
         raise NotImplementedError(f'Algorithm {name} not supported')
```

## Comparing `gaea_operator-1.2.0.dev6.data/data/yaml/object_detection.yaml` & `gaea_operator-1.2.0.dev7.data/data/yaml/object_detection.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev6.data/data/yaml/parameter.yaml` & `gaea_operator-1.2.0.dev7.data/data/yaml/parameter_c.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 metric: COCO
-num_classes: 8
+num_classes: 39
 
 TrainDataset:
     name: COCODataSet
     image_dir: ''
     anno_path: train.json
     dataset_dir: dataset
     allow_empty: true
@@ -22,60 +22,59 @@
     dataset_dir: dataset # if set, anno_path will be 'dataset_dir/anno_path'
 
 use_gpu: true
 use_xpu: false
 log_iter: 100
 save_dir: output
 # make sure snap_epoch <= epoch
-snapshot_epoch: 5
+snapshot_epoch: 20
 print_flops: false
 
 # Exporting the model
 export:
   post_process: True  # Whether post-processing is included in the network when export model.
   nms: True           # Whether NMS is included in the network when export model.
   benchmark: False    # It is used to testing model performance, if set `True`, post-process and NMS will not be exported.
   fuse_conv_bn: False
 
 # 1. PARAMETER: epoch
 epoch: 10
 
 LearningRate:
   # 2. PARAMETER: base_lr
-  base_lr: 0.001
+  base_lr: 0.000125
   schedulers:
     - name: CosineDecay
-      # make sure >= epoch
-      max_epochs: 96
+      max_epochs: 150
     - name: LinearWarmup
       start_factor: 0.
       epochs: 5
 
 OptimizerBuilder:
   optimizer:
-    momentum: 0.9
-    type: Momentum
+    type: AdamW
+    weight_decay: 0.0001
   regularizer:
     factor: 0.0005
     type: L2
 
-architecture: YOLOv3
+architecture: YOLOv3SixChannel
 norm_type: sync_bn
 use_ema: true
 ema_decay: 0.9998
 ema_black_list: ['proj_conv.weight']
 custom_black_list: ['reduce_mean']
 
-YOLOv3:
-  backbone: CSPResNet
+YOLOv3SixChannel:
+  backbone: CSPResNetSix
   neck: CustomCSPPAN
   yolo_head: PPYOLOEHead
   post_process: ~
 
-CSPResNet:
+CSPResNetSix:
   layers: [3, 6, 6, 3]
   channels: [64, 128, 256, 512, 1024]
   return_idx: [1, 2, 3]
   use_large_stem: True
   use_alpha: True
 
 CustomCSPPAN:
@@ -107,58 +106,71 @@
     score_threshold: 0.01
     nms_threshold: 0.7
 
 # 3. PARAMETER: worker_num
 worker_num: 2
 
 # 4. PARAMETER: eval_height
-eval_height: &eval_height 544
+eval_height: &eval_height 320
 
 # 5. PARAMETER: eval_width
-eval_width: &eval_width 960
+eval_width: &eval_width 320
 
 eval_size: &eval_size [*eval_height, *eval_width]
 
 TrainReader:
   sample_transforms:
-    - Decode: {}
-    - RandomDistort: {}
-    - RandomExpand: {fill_value: [123.675, 116.28, 103.53]}
-    - RandomCrop: {}
-    - RandomFlip: {}
+    - DecodePair: {suffix: "_template.jpg"}
+    - RandomDistortPair: {}
+    - RandomExpandPair: {fill_value: [123.675, 116.28, 103.53]}
+    - RandomCropPair: {}
+    - RandomFlipPair: {}
   batch_transforms:
-    - BatchRandomResize: {target_size: [[224, 640], [256, 672], [288, 704], [320, 736], [352,768], [384,800], [416, 832], [448, 864], [480, 896], [512, 928], [544, 960], [576, 992], [608, 1024], [640, 1056], [672, 1088]], random_size: True, random_interp: True, keep_ratio: False}
-    - NormalizeImage: {mean: [0., 0., 0.], std: [1., 1., 1.], norm_type: none}
-    - Permute: {}
-    - PadGT: {}
+    - BatchRandomResizePair: {
+        target_size: [192, 224, 256, 288, 320, 352, 384, 416, 448],
+        random_size: True, 
+        random_interp: True, 
+        keep_ratio: False
+      }
+    - NormalizeImagePair: {
+        mean: [0., 0., 0.], 
+        std: [1., 1., 1.], 
+        norm_type: none
+      }
+    - PermutePair: {}
+    - PadGTPair: {}
   # 6. PARAMETER: batch_size
-  batch_size: 8
+  batch_size: 24
   allow_empty: true
   shuffle: true
   drop_last: false
-  use_shared_memory: true # /dev/shm only 64MB, turn on if > 1GB
+  use_shared_memory: true
   collate_batch: true
 
 EvalReader:
   sample_transforms:
-    - Decode: {}
-    - Resize: {target_size: *eval_size, keep_ratio: False, interp: 2}
-    - NormalizeImage: {mean: [0., 0., 0.], std: [1., 1., 1.], norm_type: none}
-    - Permute: {}
-  batch_size: 4
+    - DecodePair: {suffix: "_template.jpg"}
+    - ResizePair: {target_size: *eval_size, keep_ratio: False, interp: 2}
+    - NormalizeImagePair: {
+        mean: [0., 0., 0.], 
+        std: [1., 1., 1.], 
+        norm_type: none
+      }
+    - PermutePair: {}
+  batch_size: 16
   allow_empty: true
 
 TestReader:
   inputs_def:
     image_shape: [3, *eval_height, *eval_width]
   sample_transforms:
-    - Decode: {}
-    - Resize: {target_size: *eval_size, keep_ratio: False, interp: 2}
-    - NormalizeImage: {mean: [0., 0., 0.], std: [1., 1., 1.], norm_type: none}
-    - Permute: {}
+    - DecodePair: {suffix: "_template.jpg"}
+    - ResizePair: {target_size: *eval_size, keep_ratio: False, interp: 2}
+    - NormalizeImagePair: {mean: [0., 0., 0.], std: [1., 1., 1.], norm_type: none}
+    - PermutePair: {}
   batch_size: 1
 
 weights: output/ppyoloe_model_weights/model_final
 
 # 7. PARAMETER: pretrain_weights
 # s: https://bj.bcebos.com/v1/paddledet/models/pretrained/ppyoloe_crn_s_obj365_pretrained.pdparams
 # m: https://bj.bcebos.com/v1/paddledet/models/pretrained/ppyoloe_crn_m_obj365_pretrained.pdparams
```

## Comparing `gaea_operator-1.2.0.dev6.data/data/yaml/transform_parameter.yaml` & `gaea_operator-1.2.0.dev7.data/data/yaml/transform_parameter.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev6.dist-info/METADATA` & `gaea_operator-1.2.0.dev7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-operator
-Version: 1.2.0.dev6
+Version: 1.2.0.dev7
 Summary: A common operator library to help with training neural networks.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_operator-1.2.0.dev6.dist-info/RECORD` & `gaea_operator-1.2.0.dev7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 gaea_operator/__init__.py,sha256=ByRuPwRErAhcYsPdR2RnVWtm35lq8yW-pzKVQkMlzIU,131
 gaea_operator/components/__init__.py,sha256=ByRuPwRErAhcYsPdR2RnVWtm35lq8yW-pzKVQkMlzIU,131
 gaea_operator/components/eval/__init__.py,sha256=I_nhvM_IU3swPZsE4m9lKQj50PABhRHZTVkiDjYZK5s,131
+gaea_operator/components/eval/codetr.py,sha256=GjstYt8BVRET_ZOmHoD9fWPYZd4zYDDIt0KVa1bclXc,4731
+gaea_operator/components/eval/convnext.py,sha256=bCEPip34Ah71qn6T6hsWHoJ2ZFlhilfAshoSXIrHduw,4597
 gaea_operator/components/eval/ocrnet.py,sha256=MO5F_bFFGFcYrZ2fG0eequzlTJxO_paPJCTh9gvjCpE,4169
 gaea_operator/components/eval/ppyoloe_plus.py,sha256=IXw89UF6Dp4gzAuhL0jHZZmmQGHFDpk_rhIyo7g9ygQ,4268
 gaea_operator/components/eval/resnet.py,sha256=ZxVF6RtFbqOEL0sM1sIMFOCbTIRZD3FQm2k43otT2ak,4153
 gaea_operator/components/inference/__init__.py,sha256=2aksz2GZp7BM51TKl-8KpAWpZoSSSMzEqOtSls7bd-E,3102
 gaea_operator/components/inference/inference.py,sha256=lwQV4nW-M9AD9quwlrVYoYk7towBR70erxv1xrMIVRE,4357
 gaea_operator/components/package/__init__.py,sha256=KxEJhC3kcIqj6Q7G_BCGCudrVvVkDnrRkkoJCXM6-Q8,3550
 gaea_operator/components/package/package.py,sha256=rnzZbpfzEANTZmetsGP89V70yoO14u26Z3Dr-PqTuEA,8422
 gaea_operator/components/train/__init__.py,sha256=I_nhvM_IU3swPZsE4m9lKQj50PABhRHZTVkiDjYZK5s,131
+gaea_operator/components/train/codetr.py,sha256=jARDcx2O5xwRhy5MrTsKnf0Jb4zEu5Vr0xeViQodml4,8618
+gaea_operator/components/train/convnext.py,sha256=8Vg0B6Gw7EDP50QbylHtnse1Uv9EaRNLfb8Lilwbm6Q,7854
 gaea_operator/components/train/ocrnet.py,sha256=N3JcXdhCaWuO1PDCXgA_8dyA04LBeFDrez3Y9spujkM,7519
 gaea_operator/components/train/ppyoloe_plus.py,sha256=pJ7XuhRhpYQnL1IRkwzxrtWYI8-EgS8LnwZY6a9w0XU,8365
 gaea_operator/components/train/resnet.py,sha256=1AsZtSTZyCA965Dasw9Ti9VHK_55mO1BRSyBE7MAHNc,7390
 gaea_operator/components/transform/__init__.py,sha256=I_nhvM_IU3swPZsE4m9lKQj50PABhRHZTVkiDjYZK5s,131
+gaea_operator/components/transform/codetr.py,sha256=SIsNh2TPVSjdppngl8w4rI3AnLbxQQZMWpPGTx3ZBNE,6209
+gaea_operator/components/transform/convnext.py,sha256=TBAFZVSYJSj0sztX-Gmuo5PDNFOp0TVrzaenydFXUxk,6219
 gaea_operator/components/transform/ocrnet.py,sha256=i75STCEued24oL7F0SmEbMBK7ESFry1eRIBMMupsUzc,6236
 gaea_operator/components/transform/ppyoloe_plus.py,sha256=WzwLtmTyvhd6iINlmXoh1zEX20RQahB2v9qZT3PsmU0,6078
 gaea_operator/components/transform/resnet.py,sha256=-FHg9_M5Sdt46U6HxfjSqHOUFA8jc6c0O6qgg7fk7aM,6214
 gaea_operator/components/transform_eval/__init__.py,sha256=VV2mbByhDQmiNkRPPQf8EgLqbTSXvwAJUqUylJT01tQ,3557
 gaea_operator/components/transform_eval/transform_eval.py,sha256=aaxyrom38RccFE8B7gNgxEs9E-bBUrFUH6dw2PpOBK4,8001
-gaea_operator/config/__init__.py,sha256=b283tp9PPcPViZMKzZPXa95bSNQQQHSHoP724eR8MdI,505
-gaea_operator/config/config.py,sha256=npxGcoNgTIU-pKnWpgqZBWLfWZm3GiYNTqhY3zeG_p0,4883
-gaea_operator/config/generate_transform_config.py,sha256=sYOyvd3lZ8j9gPXandrXmlGegq4KqSkoc4oku02vQMA,14051
+gaea_operator/config/__init__.py,sha256=cnMSFVbTClrj3AvCW8bEQhFsi_Ok7QWy3Vzdzm0g8WI,690
+gaea_operator/config/config.py,sha256=bVLmNPzB-xMJPupe_I97tAhSiL9NPSwj5dKN1pWC99A,4964
+gaea_operator/config/generate_transform_config.py,sha256=MHz6CmyQDJgaD5n7E9YeGH1OcYDztNfqxL7gPAMUfEI,14830
 gaea_operator/config/modify_package_files.py,sha256=iZAmxnNPdH0cHuEFJUTnzf0rM54rPFfyI7ZDJaUe1zU,14835
 gaea_operator/config/update_parse.py,sha256=JrqELK2dgIWCrtVz8gI6A6rH_5QbqZOHDNCDujnMqxs,3642
 gaea_operator/config/update_pbtxt.py,sha256=w3A5CRbnK1B4vKyUA8Qk2EDWLAqatM3ZkOw9Jxj1v9Q,16721
+gaea_operator/config/codetr/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
+gaea_operator/config/codetr/codetr_config.py,sha256=zBh6oToBVf-9Mf05qxTocZPBVBlTwnCxCh2M6DARVbU,5352
+gaea_operator/config/codetr/template/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
+gaea_operator/config/codetr/template/deploy_parameter.yaml,sha256=9HpozKsKup6_yGb_Snwbq03FB7uIIKi1A6JWd4VZJDg,590
+gaea_operator/config/codetr/template/modify_parameter.py,sha256=UFi79Oh463-LznIoFDDNDz2lNGQUzGbK2ghCi8Ohoiw,14292
+gaea_operator/config/codetr/template/train_parameter.yaml,sha256=eKcMU4LV7F7dwOP7APoWzksfRXo6PgfPwy0WAw2D-0k,13658
+gaea_operator/config/convnext/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
+gaea_operator/config/convnext/convnext_config.py,sha256=rfsR2UDJDqh1CZC4GjrKMOD5l4c1aa8n6GLCzUVRUSo,3999
+gaea_operator/config/convnext/template/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
+gaea_operator/config/convnext/template/modify_train_parameter.py,sha256=TngknRxSURmxiZId_gLGGIWW5tEet3pvygt9ZH_Qa54,3964
+gaea_operator/config/convnext/template/parameter.yaml,sha256=dWrkeBo22rDKrfNj7N-1pfhssst5XDfELGNtSki8Db0,1356
 gaea_operator/config/ocrnet/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
 gaea_operator/config/ocrnet/ocrnet_config.py,sha256=FbS-W3ljAbE-ZRkBCONC5mSowk87QVOMxN9PUV6AAww,5599
 gaea_operator/config/ocrnet/template/__init__.py,sha256=lX4deGvIgAQ1fTcskBUDqRfnOlOabgQjZXGwOJCVCkU,130
 gaea_operator/config/ocrnet/template/modify_train_parameter.py,sha256=p21spoGEwZHPfQL94HFAL5947UXU1OEQHQ2x_Z6J-xI,8809
 gaea_operator/config/ocrnet/template/parameter.yaml,sha256=CbogpeuW_OZJLgF0AbxsFjFJzZ-_RF3s9NCnGojGB9o,1467
 gaea_operator/config/ppyoloe_plus/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
 gaea_operator/config/ppyoloe_plus/ppyoloeplus_config.py,sha256=t1jN8ti8hpMM-l1U2Ukl8AS8xZsyKQh2pE5wNE1ew2U,4058
@@ -38,17 +55,17 @@
 gaea_operator/config/resnet/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
 gaea_operator/config/resnet/resnet_config.py,sha256=oJcrEEsIOe8waeijGNit9B215bNULXYw_xO9AIn6k9U,4283
 gaea_operator/config/resnet/template/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
 gaea_operator/config/resnet/template/modify_train_parameter.py,sha256=TbSV1IvnYIDS2m1uixHbJst4rA4BzzynbprqaLcSrwA,11498
 gaea_operator/config/resnet/template/parameter.yaml,sha256=c1lyNOcU63Ekb1gW86ZiHfwIOnrGJhLqOiyXEsLq9yU,2315
 gaea_operator/dataset/__init__.py,sha256=bV9qDmmiN73ZFRAUfOAAuUGv3C38Dejhv7gE0Y9Dx5k,370
 gaea_operator/dataset/cityscape_dataset.py,sha256=nxAllGXO40Fpqvm0RpQoS9whStodLp0ZpXTBhgjFXoM,4259
-gaea_operator/dataset/coco_dataset.py,sha256=YQMRb6Oe9yH75x3EpIV9wx8NiabDx0spPIHB8Ox8O28,6508
+gaea_operator/dataset/coco_dataset.py,sha256=8ZGuwXcotDHl4gSCYhp3k59haS-0D-gwBJhoZi2aBQk,6521
 gaea_operator/dataset/dataset.py,sha256=FEnDgbyS3bzx_XxLYnoEb-TXL3QB3NMNfbeByBhUmRA,7314
-gaea_operator/dataset/imagenet_dataset.py,sha256=TAfVBn6RtfdOpXP_2wr2hL4SRTwLAdCSKPV0Nm4kswY,4297
+gaea_operator/dataset/imagenet_dataset.py,sha256=xL35XeFBvZKrTRjmncUtKLTxFtbtfc5KFuMq4j701bg,4311
 gaea_operator/metric/__init__.py,sha256=fk0G_Cw3od-yzlYq5l48xDslTmqLFddrWoXOi3xqI48,584
 gaea_operator/metric/metric.py,sha256=p6KtrpC0muO0BPAdxePf3-17K5yRI6P5f9YhfncYhIo,5740
 gaea_operator/metric/analysis/__init__.py,sha256=kEv9_MuQOFC83fCprxY19T7omFNXa9dAuxstXlsEsX8,433
 gaea_operator/metric/analysis/eval_metric_analysis.py,sha256=LI84GVQICAdeliKo2JGNmAcp4caK3aObNR72lyMqQkc,18968
 gaea_operator/metric/analysis/inference_metric_analysis.py,sha256=oxXltL3ySZHvT0Ay1LjSo0sgxJb0emjE-gq7ClaJxHI,7907
 gaea_operator/metric/analysis/label_statistics_metric_analysis.py,sha256=93j10RML9xkGAu2fDQokIzl-0DYprLiVtnhdiThYRmQ,11706
 gaea_operator/metric/operator/__init__.py,sha256=Tz9wUArWR7NZvW1X9OwIGn7yTIELiwFFYszRXhQnAyY,792
@@ -70,42 +87,47 @@
 gaea_operator/metric/types/__init__.py,sha256=x5whaLpvnYR6XL2VB8IbYJ12jtYW7_zUnWks_JZY1A8,131
 gaea_operator/metric/types/image_classification_metric.py,sha256=Q-XVRRogS43yhuN0MHQY6viu-k9_r6ADK_Df2tBjPkU,1173
 gaea_operator/metric/types/metric.py,sha256=H1KHU_Kf3yxXd4pvrxY2d75tBNkQ0vEQ526A6tg3AnI,4874
 gaea_operator/metric/types/object_detection_metric.py,sha256=fS5aJZ8lHxRAcs69bfgVlvRijsbAAjuWSg2ZtuVtKA0,2362
 gaea_operator/metric/types/semantic_segmentation_metric.py,sha256=RVOUp2x8QGKwf3EepvBR-yaLvEj0OF6uM0aC0Ah-ASQ,1244
 gaea_operator/model/__init__.py,sha256=EssP2HXBMWO-4iXPbWjscBrXxSojJBOOHV3p-ioV6tA,214
 gaea_operator/model/model.py,sha256=pNswhABsGB5HHeExA4fOHH4ob2uRPqs97sCzRGPQwIo,1436
-gaea_operator/pipelines/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
+gaea_operator/pipelines/__init__.py,sha256=nEQqKhehDzCqqnUpUAI9VkgSQM3bnFVNeE1S7-SW_gk,446
+gaea_operator/pipelines/codetr_pipeline/__init__.py,sha256=1lMjOt9_9c8pQcVCxYDTt5cq9bvl4jS1yrAjTvc5ZVI,131
+gaea_operator/pipelines/codetr_pipeline/codetr_pipeline.py,sha256=_zPFyH6mQfoedqr4i1PQkTUnajUWm8F7VRpmCFlhL1w,12171
+gaea_operator/pipelines/convnext_pipeline/__init__.py,sha256=1lMjOt9_9c8pQcVCxYDTt5cq9bvl4jS1yrAjTvc5ZVI,131
+gaea_operator/pipelines/convnext_pipeline/convnext_pipeline.py,sha256=90xcgVCn-iaBw6Id9_xiybAk6hhNo0GzaRauLYCiQic,11860
 gaea_operator/pipelines/ocrnet_pipeline/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
-gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py,sha256=7g8pjtZ0sKPgA3NY3jG36RFFVNZGPB1w3PNxnEgu-jk,12009
+gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py,sha256=cpxfX6VLc3MSnE4gfZmqPJArdnMhakMhhPHujZB6fBo,12008
 gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml,sha256=-9TJKBJuH8fA-Ftb-zarkuixRYCaDRd7pog6SilDrWk,1051
 gaea_operator/pipelines/ocrnet_pipeline/transform_parameter.yaml,sha256=TdQFxYG4tE0TnasDO_4nfJji1pCbMxRu9j0WtkOrYp8,1119
 gaea_operator/pipelines/ppyoloe_plus_pipeline/train_parameter.yaml,sha256=uDAljU4wltJi_TcK19ZF7eFVjck_Clju82c6yjOpmS8,1326
 gaea_operator/pipelines/ppyoloe_plus_pipeline/transform_parameter.yaml,sha256=j1am43Egq5r5ZPAq8SwQtXGexoGKDoieI07uUE0KJ4s,1815
 gaea_operator/pipelines/resnet_pipeline/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
 gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py,sha256=CFLBY_PY1LKVzWnPwq-Un-L-D1rYwmRGpkkF-nNLurw,12187
 gaea_operator/pipelines/resnet_pipeline/train_parameter.yaml,sha256=kVRkIx_DvDle-02D3YoWpVhJ8rkbXOiuBWSCF-YDCfY,1271
 gaea_operator/pipelines/resnet_pipeline/transform_parameter.yaml,sha256=luJ-ZjerE13jXu4e7igHrrtR8_k8UYSCTxiyQbS7VhE,1121
 gaea_operator/trainer/__init__.py,sha256=Kpisv4LZyJQy6vEce-8g3HS8bo8y6rwk8K3pEaF0na0,181
-gaea_operator/trainer/trainer.py,sha256=s0P1HZejcAtksmcIKuoUdHbK8oxGeEGNnpYfQW4fxr0,5406
+gaea_operator/trainer/trainer.py,sha256=MkEwTykpnDCgxUZXez0VhqYMfAgtwoyS1gX_ftKcn1Y,6818
 gaea_operator/transform/__init__.py,sha256=1NtMabt2_F9fVeLuAM7g3i0yIac_4RP0lHMZzdyDDcY,187
 gaea_operator/transform/cvt_copy_model.py,sha256=jSWWgt2RT9ULPLNyOxypmpNuQ1kWH0gw2XNe6OLE7Sw,3307
 gaea_operator/transform/transform.py,sha256=kDZ4m4QUPbuDYSwT6lKFH7T0GEADNL3f6T-L4IUjG0g,776
-gaea_operator/utils/__init__.py,sha256=DmxN4SMbqaCs_ZHTJBF9eMitaXKLIi1Qm6TKHT_NY0Q,1788
+gaea_operator/utils/__init__.py,sha256=D-yoYbeA55UWfi_om1EWgDRkbWYiOoBMj3ALNPGvfhI,1866
 gaea_operator/utils/accelerator.py,sha256=pSxy9v9IS1xWQ_utJWQ4ljX80-rrRxnHoSBFmDZLAuY,5557
 gaea_operator/utils/compress.py,sha256=rnM_Wv_UrP9LB30xeu6f5Zch3QFH-pHGcReC8PTYjZk,2887
-gaea_operator/utils/consts.py,sha256=0TsyISenFn_x8eRNIH1fdXPLw8zSac-IAfiCxKbhySw,426
-gaea_operator/utils/file.py,sha256=9g9fFq8aw4t0I8D3wkN9Bao3tfaN3X3itZmO4LF6MsU,1948
+gaea_operator/utils/consts.py,sha256=qP2cVRQ9oDS946cpFBx75DXGzRDsoB9ZRHBkn45WIPw,532
+gaea_operator/utils/file.py,sha256=vwWaBAo9FVDbcEQUxiHwIDgvKEg-r5IoQLeSV-hPkY0,2114
 gaea_operator/utils/import_module.py,sha256=W1mKFqBClRsYm9MNqParN-03PUFIwgMJJAgSAvD9m38,1533
-gaea_operator/utils/model_template.py,sha256=n9vvjumL9wtqTHmyvLsdZdewyH1sksqGY6APmnIGG7Y,6613
+gaea_operator/utils/model_template.py,sha256=lzBEQJV_5mu7QbexszNsLjFBgC34okGsLfMz1n83IFc,10020
 gaea_operator/utils/registry.py,sha256=QchfsCrwhk3i8gmtS16PAF4029TcdOdEeWUdo1ruAps,1680
 gaea_operator/utils/tensor.py,sha256=BLnnyKz79hOqZy-L7IeA4ffDX5DoWP9NvLzStdI6C8w,1000
 gaea_operator/utils/time.py,sha256=xNKc-rzCCwhh-hNlNO05J_TA6rCMKMepuZ3qzvcScLs,301
-gaea_operator-1.2.0.dev6.data/data/yaml/object_detection.yaml,sha256=2V6AJBVa1nAE9FAosyz4z4Qv0ebw1IumYoRPUWo3Ebg,4864
-gaea_operator-1.2.0.dev6.data/data/yaml/parameter.yaml,sha256=cliceLv-V-sYmwEzbXyylbXR4MElQZQ9yrAmg6CIohM,4583
-gaea_operator-1.2.0.dev6.data/data/yaml/parameter_c.yaml,sha256=KVxZIotf24fk_SAI1v-CHNMC2ouG_lpMY0l_CtSXoRM,4666
-gaea_operator-1.2.0.dev6.data/data/yaml/train_parameter.yaml,sha256=uDAljU4wltJi_TcK19ZF7eFVjck_Clju82c6yjOpmS8,1326
-gaea_operator-1.2.0.dev6.data/data/yaml/transform_parameter.yaml,sha256=j1am43Egq5r5ZPAq8SwQtXGexoGKDoieI07uUE0KJ4s,1815
-gaea_operator-1.2.0.dev6.dist-info/METADATA,sha256=8mMEBLjPrDGliNtmgty2iiW407eBG2y-tnDBDh_5KZg,2173
-gaea_operator-1.2.0.dev6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gaea_operator-1.2.0.dev6.dist-info/top_level.txt,sha256=1-ONMzqexKnQ2qOurelrROodwfO1B8jTzpzbERvNycY,14
-gaea_operator-1.2.0.dev6.dist-info/RECORD,,
+gaea_operator-1.2.0.dev7.data/data/yaml/deploy_parameter.yaml,sha256=9HpozKsKup6_yGb_Snwbq03FB7uIIKi1A6JWd4VZJDg,590
+gaea_operator-1.2.0.dev7.data/data/yaml/object_detection.yaml,sha256=2V6AJBVa1nAE9FAosyz4z4Qv0ebw1IumYoRPUWo3Ebg,4864
+gaea_operator-1.2.0.dev7.data/data/yaml/parameter.yaml,sha256=dWrkeBo22rDKrfNj7N-1pfhssst5XDfELGNtSki8Db0,1356
+gaea_operator-1.2.0.dev7.data/data/yaml/parameter_c.yaml,sha256=KVxZIotf24fk_SAI1v-CHNMC2ouG_lpMY0l_CtSXoRM,4666
+gaea_operator-1.2.0.dev7.data/data/yaml/train_parameter.yaml,sha256=eKcMU4LV7F7dwOP7APoWzksfRXo6PgfPwy0WAw2D-0k,13658
+gaea_operator-1.2.0.dev7.data/data/yaml/transform_parameter.yaml,sha256=j1am43Egq5r5ZPAq8SwQtXGexoGKDoieI07uUE0KJ4s,1815
+gaea_operator-1.2.0.dev7.dist-info/METADATA,sha256=k00luO5Mo8aWASVUxlG1X0Divioi0Oa1AzkG3VlxO1E,2173
+gaea_operator-1.2.0.dev7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gaea_operator-1.2.0.dev7.dist-info/top_level.txt,sha256=1-ONMzqexKnQ2qOurelrROodwfO1B8jTzpzbERvNycY,14
+gaea_operator-1.2.0.dev7.dist-info/RECORD,,
```

