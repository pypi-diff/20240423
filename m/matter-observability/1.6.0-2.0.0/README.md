# Comparing `tmp/matter_observability-1.6.0-py3-none-any.whl.zip` & `tmp/matter_observability-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 11334 bytes, number of entries: 21
+Zip file size: 11298 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_observability/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_observability/__init__.py
--rw-r--r--  2.0 unx      286 b- defN 20-Feb-02 00:00 matter_observability/config.py
+-rw-r--r--  2.0 unx      331 b- defN 20-Feb-02 00:00 matter_observability/config.py
 -rw-r--r--  2.0 unx      132 b- defN 20-Feb-02 00:00 matter_observability/exceptions.py
 -rw-r--r--  2.0 unx      133 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 20-Feb-02 00:00 matter_observability/fastapi/request_id.py
--rw-r--r--  2.0 unx      817 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
+-rw-r--r--  2.0 unx      536 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
 -rw-r--r--  2.0 unx       73 b- defN 20-Feb-02 00:00 matter_observability/logging/__init__.py
--rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/logging/logging_config.py
--rw-r--r--  2.0 unx      316 b- defN 20-Feb-02 00:00 matter_observability/metrics/__init__.py
--rw-r--r--  2.0 unx      867 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
+-rw-r--r--  2.0 unx     2427 b- defN 20-Feb-02 00:00 matter_observability/logging/logging_config.py
+-rw-r--r--  2.0 unx      314 b- defN 20-Feb-02 00:00 matter_observability/metrics/__init__.py
+-rw-r--r--  2.0 unx      868 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
 -rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/metrics/decorators.py
 -rw-r--r--  2.0 unx      473 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_counter.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge.py
 -rw-r--r--  2.0 unx      708 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge_duration.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_metric.py
--rw-r--r--  2.0 unx      903 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
-?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.6.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.6.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.6.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.6.0.dist-info/RECORD
-21 files, 20367 bytes uncompressed, 7968 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx      900 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
+?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-2.0.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-2.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-2.0.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-2.0.0.dist-info/RECORD
+21 files, 20126 bytes uncompressed, 7932 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: matter_observability/metrics/labeled_metric.py
 Comment: 
 
 Filename: matter_observability/metrics/utils.py
 Comment: 
 
-Filename: matter_observability-1.6.0.dist-info/METADATA
+Filename: matter_observability-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_observability-1.6.0.dist-info/WHEEL
+Filename: matter_observability-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_observability-1.6.0.dist-info/licenses/LICENSE
+Filename: matter_observability-2.0.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_observability-1.6.0.dist-info/RECORD
+Filename: matter_observability-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_observability/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.6.0"
+__version__ = "2.0.0"
```

## matter_observability/config.py

```diff
@@ -1,8 +1,8 @@
 import os
 
 
 class Config:
-    ENABLE_METRICS = os.getenv("ENABLE_METRICS", "true").lower() == "true"
+    ENABLE_METRICS = os.getenv("ENABLE_METRICS", "true").lower() == "true"  # Used by prometheus-fastapi-instrumentator
     SERVER_LOG_LEVEL = os.getenv("SERVER_LOG_LEVEL", "info")
     PROMETHEUS_PUSH_GATEWAY_HOST = os.getenv("PROMETHEUS_PUSH_GATEWAY_HOST")
     INSTANCE_NAME = os.getenv("INSTANCE_NAME")
```

## matter_observability/fastapi/utils.py

```diff
@@ -1,23 +1,15 @@
-from starlette_exporter import PrometheusMiddleware, handle_metrics
+from fastapi import FastAPI
+from prometheus_fastapi_instrumentator import Instrumentator
 
-from matter_observability.config import Config
-from matter_observability.exceptions import MisConfigurationError
 from .request_id import process_request_id
 
 
-def configure_middleware(app, skip_paths=None):
+def configure_middleware(app: FastAPI, skip_paths: list[str] | None = None) -> None:
     metrics_path = "/internal/metrics"
+    skip_paths = skip_paths or [metrics_path]
 
     app.middleware("http")(process_request_id)
 
-    if Config.ENABLE_METRICS:
-        if bool(Config.INSTANCE_NAME) is False:
-            raise MisConfigurationError("Environment variable: INSTANCE_NAME is not valid")
-
-        app.add_middleware(
-            PrometheusMiddleware,
-            app_name=Config.INSTANCE_NAME,
-            group_paths=True,
-            skip_paths=[metrics_path] + skip_paths if skip_paths else [metrics_path],
-        )
-        app.add_route(metrics_path, handle_metrics)
+    Instrumentator(excluded_handlers=skip_paths, should_respect_env_var=True, env_var_name="ENABLE_METRICS").instrument(
+        app=app
+    ).expose(app=app, endpoint=metrics_path)
```

## matter_observability/logging/logging_config.py

```diff
@@ -1,10 +1,9 @@
 from matter_observability.config import Config  # pragma: no cover
 
-
 LOGGING_CONFIG_BASIC = {
     "version": 1,
     "formatters": {
         "no_request_id": {
             "format": "[%(asctime)s] [%(levelname)s] [%(name)s] [%(filename)s:%(funcName)s:%(lineno)s] - %(message)s"
         },
     },
```

## matter_observability/metrics/__init__.py

```diff
@@ -1,9 +1,7 @@
 __all__ = []
 
+from .custom_metrics import COUNTER_CUSTOM, GAUGE_CUSTOM, GAUGE_PROCESSING_TIME
+from .decorators import count_occurrence, gauge_value, measure_processing_time
+from .labeled_counter import LabeledCounter
 from .labeled_gauge import LabeledGauge
 from .labeled_gauge_duration import LabeledGaugeDuration
-from .labeled_counter import LabeledCounter
-
-from .custom_metrics import GAUGE_PROCESSING_TIME, GAUGE_CUSTOM, COUNTER_CUSTOM
-
-from .decorators import gauge_value, measure_processing_time, count_occurrence
```

## matter_observability/metrics/custom_metrics.py

```diff
@@ -1,9 +1,10 @@
 import os
-from prometheus_client import Gauge, Counter
+
+from prometheus_client import Counter, Gauge
 
 from matter_observability.config import Config
 
 if os.getenv("INSTANCE_TYPE") == "celery":
     from .utils import REGISTRY
 else:
     from prometheus_client import REGISTRY
```

## matter_observability/metrics/decorators.py

```diff
@@ -1,14 +1,14 @@
 import functools
 from asyncio import iscoroutinefunction
 
+from .custom_metrics import COUNTER_CUSTOM, GAUGE_CUSTOM, GAUGE_PROCESSING_TIME
+from .labeled_counter import LabeledCounter
 from .labeled_gauge import LabeledGauge
 from .labeled_gauge_duration import LabeledGaugeDuration
-from .labeled_counter import LabeledCounter
-from .custom_metrics import GAUGE_CUSTOM, GAUGE_PROCESSING_TIME, COUNTER_CUSTOM
 
 
 def gauge_value(label: str, use_push_gateway: bool = False):
     labeled_gauge = LabeledGauge(use_push_gateway=use_push_gateway, metric=GAUGE_CUSTOM, label=label)
 
     def wrapped(func):
         @functools.wraps(func)
```

## matter_observability/metrics/labeled_counter.py

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
 import logging
 
-from .utils import publish_metrics
 from .labeled_metric import LabeledMetric
+from .utils import publish_metrics
 
 
 class LabeledCounter(LabeledMetric):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     @property
```

## matter_observability/metrics/labeled_gauge_duration.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-import time
 import logging
+import time
 
 from .labeled_gauge import LabeledGauge
 
 
 class LabeledGaugeDuration(LabeledGauge):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

## matter_observability/metrics/utils.py

```diff
@@ -1,11 +1,11 @@
 import logging
 from urllib.error import HTTPError
 
-from prometheus_client import push_to_gateway, CollectorRegistry
+from prometheus_client import CollectorRegistry, push_to_gateway
 
 from matter_observability.config import Config
 from matter_observability.exceptions import MisConfigurationError
 
 REGISTRY = CollectorRegistry()
 job_name = f"batch_{Config.INSTANCE_NAME}"
 
@@ -19,8 +19,8 @@
             push_to_gateway(
                 f"{Config.PROMETHEUS_PUSH_GATEWAY_HOST}:9091",
                 job=job_name,
                 registry=REGISTRY,
                 timeout=1,  # The connection timeout
             )
         except (OSError, HTTPError) as ex:
-            logging.warning(f"Observability: Unable to send metrics to the Push Gateway: {str(ex)}")
+            logging.warning(f"Observability: Unable to send metrics to the Push Gateway: {ex!s}")
```

## Comparing `matter_observability-1.6.0.dist-info/METADATA` & `matter_observability-2.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: matter-observability
-Version: 1.6.0
+Version: 2.0.0
 Summary: A template for Matter's observability library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-observability#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-observability/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-observability
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
```

## Comparing `matter_observability-1.6.0.dist-info/licenses/LICENSE` & `matter_observability-2.0.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_observability-1.6.0.dist-info/RECORD` & `matter_observability-2.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-matter_observability/__about__.py,sha256=FR_H1hPr0f-WoHc77gw_GT5yLHo5uJLy-sppoL-t8lo,134
+matter_observability/__about__.py,sha256=rzZFQ3B-1kwQEv3_mv8w4vo2K16fWbrXEtD739rb_fA,134
 matter_observability/__init__.py,sha256=3w1lcMfVq_KzRTAJVSrwL5vGSnu2BzERE4WFHCGvzFY,112
-matter_observability/config.py,sha256=m55Od1HaB8neBOYLhCJc2uwTSUlXT54JtOR5FzpqEQk,286
+matter_observability/config.py,sha256=UKORWKu3BE9FvzuLYT8HbCAtvwuB5Lxu24ho1ft73fs,331
 matter_observability/exceptions.py,sha256=vc3AZT1ZsrkTgnkeoiOFsAgsSIlCkywHryUnm-APVQo,132
 matter_observability/fastapi/__init__.py,sha256=TBGRRAMg7Q2Ov_a6sUZuWIoH9ITxWF036CYLVn-K25g,133
 matter_observability/fastapi/request_id.py,sha256=frjbfIr6U3J6ElbA5ZDnNFiz7eKerCGStevHHZu78P0,641
-matter_observability/fastapi/utils.py,sha256=7_42_uQDpMliYsSz-K5txWLJMUySmPKThdmS559moKw,817
+matter_observability/fastapi/utils.py,sha256=VOux21KI6HJMZgPDWoozLV7lHiaoh6WHT0LKf6kp6W4,536
 matter_observability/logging/__init__.py,sha256=Xz1akGf5QHmMHjF9PpQ6Ljx8V5VI28N1tjom11jEKnQ,73
-matter_observability/logging/logging_config.py,sha256=9o5_blZVHIuZHE06G-jKpne4pm7Nxx2RskcSV20ISz0,2428
-matter_observability/metrics/__init__.py,sha256=CRAS0OI8AddFdIZFa66JvVam2tTjbfw-CLLEFRiwxnU,316
-matter_observability/metrics/custom_metrics.py,sha256=WWs17yaOu4mN45VDhzo3z4UbRBurWdc7rMlnsTvMGmg,867
-matter_observability/metrics/decorators.py,sha256=DU-3lQZLYjSv_pTf36W_kdAvSZsOBrS61aPN7o8ryeM,2428
-matter_observability/metrics/labeled_counter.py,sha256=9ziI7Xlu1ApKo-eQcEVCSyAId_xvqo8jm6y3yLGT9ak,473
+matter_observability/logging/logging_config.py,sha256=IXpfh1nOqae91nkkBsTXyPGytyAy4Q8p9jU7rXq8vDE,2427
+matter_observability/metrics/__init__.py,sha256=4cDKU2b_q-XNsq3eo06PDasSd3w7CVG4-uAmycOIjvE,314
+matter_observability/metrics/custom_metrics.py,sha256=2DCMSyAwnSf8hfNeRCAKdWLm5BGFp3C0vRQHvNVVCSM,868
+matter_observability/metrics/decorators.py,sha256=LdnXq5dpxrBsjw6iOtFys3DLHmBhSK59FiusIkp8kHM,2428
+matter_observability/metrics/labeled_counter.py,sha256=SO7h6_4MAhO_AzQJOMhl2puB3vBBY6YQeVFhbYlPeH8,473
 matter_observability/metrics/labeled_gauge.py,sha256=MYJRPuqsvrjdBmDIiBaxzA66CUjJVI1KOGvzRRhDas0,489
-matter_observability/metrics/labeled_gauge_duration.py,sha256=-Xaxskzx2NytzBnLtbm6tJWjfHiBuqlNZ1WcG7HW7wA,708
+matter_observability/metrics/labeled_gauge_duration.py,sha256=mXVxqHi5RKL1-e6pC7i8-huopt53D1KfrMRcCEZbe_Y,708
 matter_observability/metrics/labeled_metric.py,sha256=Qn4psWuJJTyALay8-wU0vK2Y0epp25JWPSoZ8BQK8hM,421
-matter_observability/metrics/utils.py,sha256=0UmfcQlxlvOnA-mxaOBYnjSRaUa0EP4UKHVLDQG7VGA,903
-matter_observability-1.6.0.dist-info/METADATA,sha256=WcWK9ZPPkF6iiDy9c4djF5l05dl_qol7_qW2Lob_oXc,5852
-matter_observability-1.6.0.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-matter_observability-1.6.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_observability-1.6.0.dist-info/RECORD,,
+matter_observability/metrics/utils.py,sha256=TjhMxm3hj8PrOpJxuBHkwqexvXDuZPx7Oiul3EDlcUA,900
+matter_observability-2.0.0.dist-info/METADATA,sha256=_4N79vezto2qN2Qm6wftoypU-szhZlQpj8GwkvqRzag,5852
+matter_observability-2.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+matter_observability-2.0.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_observability-2.0.0.dist-info/RECORD,,
```

