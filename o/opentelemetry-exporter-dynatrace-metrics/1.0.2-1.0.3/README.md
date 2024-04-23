# Comparing `tmp/opentelemetry-exporter-dynatrace-metrics-1.0.2.tar.gz` & `tmp/opentelemetry-exporter-dynatrace-metrics-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry-exporter-dynatrace-metrics-1.0.2.tar", last modified: Mon Dec  5 11:43:52 2022, max compression
+gzip compressed data, was "opentelemetry-exporter-dynatrace-metrics-1.0.3.tar", last modified: Tue Apr 23 13:52:50 2024, max compression
```

## Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2.tar` & `opentelemetry-exporter-dynatrace-metrics-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.693036 opentelemetry-exporter-dynatrace-metrics-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2022-12-05 11:43:52.693036 opentelemetry-exporter-dynatrace-metrics-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-05 11:43:52.693036 opentelemetry-exporter-dynatrace-metrics-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.689036 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-05 11:43:52.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 11:43:52.693036 opentelemetry-exporter-dynatrace-metrics-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    31689 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/test/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2022-12-05 11:43:45.000000 opentelemetry-exporter-dynatrace-metrics-1.0.2/test/test_histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-23 13:52:50.834138 opentelemetry-exporter-dynatrace-metrics-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 13:52:50.834138 opentelemetry-exporter-dynatrace-metrics-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 13:52:50.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:52:50.830138 opentelemetry-exporter-dynatrace-metrics-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    31689 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/test/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-23 13:52:42.000000 opentelemetry-exporter-dynatrace-metrics-1.0.3/test/test_histogram_utils.py
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/LICENSE` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/PKG-INFO` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-dynatrace-metrics
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dynatrace Metric Exporter for OpenTelemetry
 Home-page: https://github.com/dynatrace-oss/opentelemetry-metric-python/
 Author: Dynatrace
 Author-email: opensource@dynatrace.com
 License: Apache-2.0
 Project-URL: Dynatrace, https://www.dynatrace.com/
 Project-URL: Source, https://github.com/dynatrace-oss/opentelemetry-metric-python/
 Project-URL: Download, https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/#files
-Description: # Dynatrace OpenTelemetry Metrics Exporter for Python
+Description: # Dynatrace
+        
+        [Dynatrace](https://www.dynatrace.com/integrations/opentelemetry) supports native
+        OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+        All signals can be sent directly to Dynatrace via **OTLP protobuf over HTTP**
+        using the built-in OTLP/HTTP Exporter available in the OpenTelemetry Python SDK.
+        More information on configuring your Python applications to use the OTLP exporter can be found in the
+        [Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/otel-wt-python).
+        
+        ## Dynatrace OpenTelemetry Metrics Exporter for Python
+        ![Static Badge](https://img.shields.io/badge/status-deprecated-orange)
+        
+        > **Warning**
+        > Dynatrace supports native OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+        > Therefore, the proprietary Dynatrace OpenTelemetry metrics exporter is deprecated in favor of exporting via OTLP/HTTP.
+        >
+        > The exporter is still available but after the end of 2023, no support, updates, or compatibility with newer OTel versions will be provided.
+        >
+        > Please refer to the [migration guide](https://www.dynatrace.com/support/help/shortlink/migrating-dynatrace-metrics-exporter-otlp-exporter#migrate-applications) for instructions on how to migrate to the OTLP HTTP exporter, as well as reasoning and benefits for this transition.
+        >
+        > For an example on how to configure the OTLP exporter in a Python application, check out the [Python integration walk-through](https://www.dynatrace.com/support/help/shortlink/otel-wt-python) page in the Dynatrace documentation.
         
         This exporter allows exporting metrics created using the [OpenTelemetry SDK for Python](https://github.com/open-telemetry/opentelemetry-python)
         directly to [Dynatrace](https://www.dynatrace.com).
         
         **It was built against OpenTelemetry SDK version `1.12.0` and should work with any `1.12+` version.**
         
         More information on exporting OpenTelemetry metrics to Dynatrace can be found in the
         [Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/opentelemetry-metrics).
         
-        ## Getting started
+        ### Getting started
         
-        ### Installation
+        #### Installation
         
         To install the [latest version from PyPI](https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/) run:
         
         ```shell
         pip install opentelemetry-exporter-dynatrace-metrics
         ```
         
-        ### Usage
-        
-        The general setup of OpenTelemetry Python is explained in the official [Getting Started Guide](https://open-telemetry.github.io/opentelemetry-python/getting-started.html#add-metrics).
+        #### Usage
         
         ```python
+        from opentelemetry import metrics
+        from opentelemetry.sdk.metrics import MeterProvider
+        from dynatrace.opentelemetry.metrics.export import (
+            configure_dynatrace_metrics_export
+        )
+        
+        
         # setup metrics export pipeline
         metrics.set_meter_provider(MeterProvider(
             # configure Exporter/MetricReader combination with a 5000ms export
             # interval, endpoint url and API token.
             metric_readers=[
                 configure_dynatrace_metrics_export(
                     export_interval_millis=5000,
@@ -54,113 +79,115 @@
             description="Description of MyCounter",
             unit="1"
         )
         
         counter.add(25, {"dimension-1": "value-1"})
         ```
         
-        ### Example
+        #### Example
         
         To run the [example](example/basic_example.py), clone this repository and change to the `opentelemetry-metric-python` folder, then run:
         
         ```shell
         pip install .           # install the Dynatrace exporter
+        pip install psutil      # this package is used by the example to read CPU/Memory usage
         export LOGLEVEL=DEBUG   # (optional) Set the log level to debug to see more output (default is INFO)
         python example/basic_example.py
         ```
         
         A more complete setup routine can be found [here](example/install_and_run.sh), including installing inside a virtual environment and getting required packages.
         If you just want to see it in action, it should be sufficient to run [`example/install_and_run.sh`](example/install_and_run.sh) from the root folder.
         This script will install Python, set up a virtual environment, pull in all the required packages and run the [example](example/basic_example.py).
         
         The example also offers a simple CLI. Run `python example/basic_example.py -h` to get more information.
         
-        ### Configuration
+        #### Configuration
         
         The exporter allows for configuring the following settings by passing them to the constructor:
         
-        #### Dynatrace API Endpoint
+        ##### Dynatrace API Endpoint
         
         The endpoint to which the metrics are sent is specified using the `endpoint_url` parameter.
         
         Given an environment ID `myenv123` on Dynatrace SaaS, the [metrics ingest endpoint](https://www.dynatrace.com/support/help/dynatrace-api/environment-api/metric-v2/post-ingest-metrics/) would be `https://myenv123.live.dynatrace.com/api/v2/metrics/ingest`.
         
         If a OneAgent is installed on the host, it can provide a local endpoint for providing metrics directly without the need for an API token.
         This feature is currently in an Early Adopter phase and has to be enabled as described in the [OneAgent metric API documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/local-api/).
         Using the local API endpoint, the host ID and host name context are automatically added to each metric as dimensions.
         The default metric API endpoint exposed by the OneAgent is `http://localhost:14499/metrics/ingest`.
         If no endpoint is set and a OneAgent is running on the host, metrics will be exported to it automatically using the OneAgent with no endpoint or API token configuration required.
         
-        #### Dynatrace API Token
+        ##### Dynatrace API Token
         
         The Dynatrace API token to be used by the exporter is specified using the `api_token` parameter and could, for example, be read from an environment variable.
         
         Creating an API token for your Dynatrace environment is described in the [Dynatrace API documentation](https://www.dynatrace.com/support/help/dynatrace-api/basics/dynatrace-api-authentication/).
         The permission required for sending metrics is `Ingest metrics` (`metrics.ingest`) and it is recommended to limit scope to only this permission.
         
-        #### Metric Key Prefix
+        ##### Metric Key Prefix
         
         The `prefix` parameter specifies an optional prefix, which is prepended to each metric key, separated by a dot (`<prefix>.<name>`).
         
-        #### Default Dimensions
+        ##### Default Dimensions
         
         The `default_dimensions` parameter can be used to optionally specify a list of key/value pairs, which will be added as additional dimensions to all data points.
         Dimension keys are unique, and labels on instruments will overwrite the default dimensions if key collisions appear.
         
-        #### Export Dynatrace Metadata
+        ##### Export Dynatrace Metadata
         
         If running on a host with a running OneAgent, setting the `export_dynatrace_metadata` option to `True` will export metadata collected by the OneAgent to the Dynatrace endpoint.
         If no Dynatrace API endpoint is set, the default exporter endpoint will be the OneAgent endpoint, and this option will be set automatically.
         Therefore, if no endpoint is specified, a OneAgent is assumed to be running and used as the export endpoint for all metric lines, including metadata.
         More information on the underlying Dynatrace metadata feature that is used by the exporter can be found in the
         [Dynatrace documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/enrich-metrics/).
         
-        ##### Dimensions precedence
+        ###### Dimensions precedence
         
         When specifying default dimensions, attributes and Dynatrace metadata enrichment, the precedence of dimensions with the same key is as follows:
         Default dimensions are overwritten by attributes passed to instruments, which in turn are overwritten by the Dynatrace metadata dimensions (even though the likeliness of a collision here is very low, since the Dynatrace metadata only contains [Dynatrace reserved dimensions](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/metric-ingestion-protocol/#syntax) starting with `dt.*`).
         
-        ## Development
+        ### Development
         
-        ### Requirements
+        #### Requirements
         
-        Just [`tox`](https://pypi.org/project/tox/).
+        Just [`tox`](https://pypi.org/project/tox/). Make sure to `pip install` the `requirements-dev.txt` to get the relevant packages. 
         
-        ### Running tests and lint
+        #### Running tests and lint
         
         * Test all supported python versions: `tox`
         * Test all supported python versions in parallel: `tox -p`
         * A particular python version: `tox -e 38`
         * Current python version: `tox -e py`
         * Lint: `tox -e lint`
         
-        ## Limitations
+        ### Limitations
         
-        ### Typed attributes support
+        #### Typed attributes support
         
         The OpenTelemetry Metrics API for Python supports the concept
         of [Attributes]( https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/common/common.md#attributes).
         These attributes consist of key-value pairs, where the keys are strings and the
         values are either primitive types or arrays of uniform primitive types.
         
         At the moment, this exporter **only supports attributes with string key and
         value type**.
         This means that if attributes of any other type are used, they will be 
         **ignored** and **only** the string-valued attributes are going to be sent to
         Dynatrace.
         
-        ### Histogram
+        #### Histogram
         
         OpenTelemetry Histograms are exported to Dynatrace as statistical summaries
         consisting of a minimum and maximum value, the total sum of all values, and the
         count of the values summarized. If the min and max values are not directly
         available on the metric data point, estimations based on the boundaries of the
         first and last buckets containing values are used.
+        
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/README.md` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,57 @@
-# Dynatrace OpenTelemetry Metrics Exporter for Python
+# Dynatrace
+
+[Dynatrace](https://www.dynatrace.com/integrations/opentelemetry) supports native
+OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+All signals can be sent directly to Dynatrace via **OTLP protobuf over HTTP**
+using the built-in OTLP/HTTP Exporter available in the OpenTelemetry Python SDK.
+More information on configuring your Python applications to use the OTLP exporter can be found in the
+[Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/otel-wt-python).
+
+## Dynatrace OpenTelemetry Metrics Exporter for Python
+![Static Badge](https://img.shields.io/badge/status-deprecated-orange)
+
+> **Warning**
+> Dynatrace supports native OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+> Therefore, the proprietary Dynatrace OpenTelemetry metrics exporter is deprecated in favor of exporting via OTLP/HTTP.
+>
+> The exporter is still available but after the end of 2023, no support, updates, or compatibility with newer OTel versions will be provided.
+>
+> Please refer to the [migration guide](https://www.dynatrace.com/support/help/shortlink/migrating-dynatrace-metrics-exporter-otlp-exporter#migrate-applications) for instructions on how to migrate to the OTLP HTTP exporter, as well as reasoning and benefits for this transition.
+>
+> For an example on how to configure the OTLP exporter in a Python application, check out the [Python integration walk-through](https://www.dynatrace.com/support/help/shortlink/otel-wt-python) page in the Dynatrace documentation.
 
 This exporter allows exporting metrics created using the [OpenTelemetry SDK for Python](https://github.com/open-telemetry/opentelemetry-python)
 directly to [Dynatrace](https://www.dynatrace.com).
 
 **It was built against OpenTelemetry SDK version `1.12.0` and should work with any `1.12+` version.**
 
 More information on exporting OpenTelemetry metrics to Dynatrace can be found in the
 [Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/opentelemetry-metrics).
 
-## Getting started
+### Getting started
 
-### Installation
+#### Installation
 
 To install the [latest version from PyPI](https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/) run:
 
 ```shell
 pip install opentelemetry-exporter-dynatrace-metrics
 ```
 
-### Usage
-
-The general setup of OpenTelemetry Python is explained in the official [Getting Started Guide](https://open-telemetry.github.io/opentelemetry-python/getting-started.html#add-metrics).
+#### Usage
 
 ```python
+from opentelemetry import metrics
+from opentelemetry.sdk.metrics import MeterProvider
+from dynatrace.opentelemetry.metrics.export import (
+    configure_dynatrace_metrics_export
+)
+
+
 # setup metrics export pipeline
 metrics.set_meter_provider(MeterProvider(
     # configure Exporter/MetricReader combination with a 5000ms export
     # interval, endpoint url and API token.
     metric_readers=[
         configure_dynatrace_metrics_export(
             export_interval_millis=5000,
@@ -43,104 +68,105 @@
     description="Description of MyCounter",
     unit="1"
 )
 
 counter.add(25, {"dimension-1": "value-1"})
 ```
 
-### Example
+#### Example
 
 To run the [example](example/basic_example.py), clone this repository and change to the `opentelemetry-metric-python` folder, then run:
 
 ```shell
 pip install .           # install the Dynatrace exporter
+pip install psutil      # this package is used by the example to read CPU/Memory usage
 export LOGLEVEL=DEBUG   # (optional) Set the log level to debug to see more output (default is INFO)
 python example/basic_example.py
 ```
 
 A more complete setup routine can be found [here](example/install_and_run.sh), including installing inside a virtual environment and getting required packages.
 If you just want to see it in action, it should be sufficient to run [`example/install_and_run.sh`](example/install_and_run.sh) from the root folder.
 This script will install Python, set up a virtual environment, pull in all the required packages and run the [example](example/basic_example.py).
 
 The example also offers a simple CLI. Run `python example/basic_example.py -h` to get more information.
 
-### Configuration
+#### Configuration
 
 The exporter allows for configuring the following settings by passing them to the constructor:
 
-#### Dynatrace API Endpoint
+##### Dynatrace API Endpoint
 
 The endpoint to which the metrics are sent is specified using the `endpoint_url` parameter.
 
 Given an environment ID `myenv123` on Dynatrace SaaS, the [metrics ingest endpoint](https://www.dynatrace.com/support/help/dynatrace-api/environment-api/metric-v2/post-ingest-metrics/) would be `https://myenv123.live.dynatrace.com/api/v2/metrics/ingest`.
 
 If a OneAgent is installed on the host, it can provide a local endpoint for providing metrics directly without the need for an API token.
 This feature is currently in an Early Adopter phase and has to be enabled as described in the [OneAgent metric API documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/local-api/).
 Using the local API endpoint, the host ID and host name context are automatically added to each metric as dimensions.
 The default metric API endpoint exposed by the OneAgent is `http://localhost:14499/metrics/ingest`.
 If no endpoint is set and a OneAgent is running on the host, metrics will be exported to it automatically using the OneAgent with no endpoint or API token configuration required.
 
-#### Dynatrace API Token
+##### Dynatrace API Token
 
 The Dynatrace API token to be used by the exporter is specified using the `api_token` parameter and could, for example, be read from an environment variable.
 
 Creating an API token for your Dynatrace environment is described in the [Dynatrace API documentation](https://www.dynatrace.com/support/help/dynatrace-api/basics/dynatrace-api-authentication/).
 The permission required for sending metrics is `Ingest metrics` (`metrics.ingest`) and it is recommended to limit scope to only this permission.
 
-#### Metric Key Prefix
+##### Metric Key Prefix
 
 The `prefix` parameter specifies an optional prefix, which is prepended to each metric key, separated by a dot (`<prefix>.<name>`).
 
-#### Default Dimensions
+##### Default Dimensions
 
 The `default_dimensions` parameter can be used to optionally specify a list of key/value pairs, which will be added as additional dimensions to all data points.
 Dimension keys are unique, and labels on instruments will overwrite the default dimensions if key collisions appear.
 
-#### Export Dynatrace Metadata
+##### Export Dynatrace Metadata
 
 If running on a host with a running OneAgent, setting the `export_dynatrace_metadata` option to `True` will export metadata collected by the OneAgent to the Dynatrace endpoint.
 If no Dynatrace API endpoint is set, the default exporter endpoint will be the OneAgent endpoint, and this option will be set automatically.
 Therefore, if no endpoint is specified, a OneAgent is assumed to be running and used as the export endpoint for all metric lines, including metadata.
 More information on the underlying Dynatrace metadata feature that is used by the exporter can be found in the
 [Dynatrace documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/enrich-metrics/).
 
-##### Dimensions precedence
+###### Dimensions precedence
 
 When specifying default dimensions, attributes and Dynatrace metadata enrichment, the precedence of dimensions with the same key is as follows:
 Default dimensions are overwritten by attributes passed to instruments, which in turn are overwritten by the Dynatrace metadata dimensions (even though the likeliness of a collision here is very low, since the Dynatrace metadata only contains [Dynatrace reserved dimensions](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/metric-ingestion-protocol/#syntax) starting with `dt.*`).
 
-## Development
+### Development
 
-### Requirements
+#### Requirements
 
-Just [`tox`](https://pypi.org/project/tox/).
+Just [`tox`](https://pypi.org/project/tox/). Make sure to `pip install` the `requirements-dev.txt` to get the relevant packages. 
 
-### Running tests and lint
+#### Running tests and lint
 
 * Test all supported python versions: `tox`
 * Test all supported python versions in parallel: `tox -p`
 * A particular python version: `tox -e 38`
 * Current python version: `tox -e py`
 * Lint: `tox -e lint`
 
-## Limitations
+### Limitations
 
-### Typed attributes support
+#### Typed attributes support
 
 The OpenTelemetry Metrics API for Python supports the concept
 of [Attributes]( https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/common/common.md#attributes).
 These attributes consist of key-value pairs, where the keys are strings and the
 values are either primitive types or arrays of uniform primitive types.
 
 At the moment, this exporter **only supports attributes with string key and
 value type**.
 This means that if attributes of any other type are used, they will be 
 **ignored** and **only** the string-valued attributes are going to be sent to
 Dynatrace.
 
-### Histogram
+#### Histogram
 
 OpenTelemetry Histograms are exported to Dynatrace as statistical summaries
 consisting of a minimum and maximum value, the total sum of all values, and the
 count of the values summarized. If the min and max values are not directly
 available on the metric data point, estimations based on the boundaries of the
-first and last buckets containing values are used.
+first and last buckets containing values are used.
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/setup.cfg` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 project_urls = 
 	Dynatrace = https://www.dynatrace.com/
 	Source = https://github.com/dynatrace-oss/opentelemetry-metric-python/
 	Download = https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/#files
 license = Apache-2.0
 platforms = any
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 7 - Inactive
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/__init__.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     _DynatraceMetricsExporter,
 )
 from opentelemetry.sdk.metrics.export import (
     PeriodicExportingMetricReader,
     MetricReader,
 )
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 
 def configure_dynatrace_metrics_export(
     endpoint_url: Optional[str] = None,
     api_token: Optional[str] = None,
     prefix: Optional[str] = None,
     default_dimensions: Optional[Mapping[str, str]] = None,
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_exporter.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_factory.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_factory.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/dynatrace/opentelemetry/metrics/export/_histogram_utils.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/dynatrace/opentelemetry/metrics/export/_histogram_utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/PKG-INFO` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 Metadata-Version: 2.1
 Name: opentelemetry-exporter-dynatrace-metrics
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dynatrace Metric Exporter for OpenTelemetry
 Home-page: https://github.com/dynatrace-oss/opentelemetry-metric-python/
 Author: Dynatrace
 Author-email: opensource@dynatrace.com
 License: Apache-2.0
 Project-URL: Dynatrace, https://www.dynatrace.com/
 Project-URL: Source, https://github.com/dynatrace-oss/opentelemetry-metric-python/
 Project-URL: Download, https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/#files
-Description: # Dynatrace OpenTelemetry Metrics Exporter for Python
+Description: # Dynatrace
+        
+        [Dynatrace](https://www.dynatrace.com/integrations/opentelemetry) supports native
+        OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+        All signals can be sent directly to Dynatrace via **OTLP protobuf over HTTP**
+        using the built-in OTLP/HTTP Exporter available in the OpenTelemetry Python SDK.
+        More information on configuring your Python applications to use the OTLP exporter can be found in the
+        [Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/otel-wt-python).
+        
+        ## Dynatrace OpenTelemetry Metrics Exporter for Python
+        ![Static Badge](https://img.shields.io/badge/status-deprecated-orange)
+        
+        > **Warning**
+        > Dynatrace supports native OpenTelemetry protocol (OTLP) ingest for traces, metrics and logs.
+        > Therefore, the proprietary Dynatrace OpenTelemetry metrics exporter is deprecated in favor of exporting via OTLP/HTTP.
+        >
+        > The exporter is still available but after the end of 2023, no support, updates, or compatibility with newer OTel versions will be provided.
+        >
+        > Please refer to the [migration guide](https://www.dynatrace.com/support/help/shortlink/migrating-dynatrace-metrics-exporter-otlp-exporter#migrate-applications) for instructions on how to migrate to the OTLP HTTP exporter, as well as reasoning and benefits for this transition.
+        >
+        > For an example on how to configure the OTLP exporter in a Python application, check out the [Python integration walk-through](https://www.dynatrace.com/support/help/shortlink/otel-wt-python) page in the Dynatrace documentation.
         
         This exporter allows exporting metrics created using the [OpenTelemetry SDK for Python](https://github.com/open-telemetry/opentelemetry-python)
         directly to [Dynatrace](https://www.dynatrace.com).
         
         **It was built against OpenTelemetry SDK version `1.12.0` and should work with any `1.12+` version.**
         
         More information on exporting OpenTelemetry metrics to Dynatrace can be found in the
         [Dynatrace documentation](https://www.dynatrace.com/support/help/shortlink/opentelemetry-metrics).
         
-        ## Getting started
+        ### Getting started
         
-        ### Installation
+        #### Installation
         
         To install the [latest version from PyPI](https://pypi.org/project/opentelemetry-exporter-dynatrace-metrics/) run:
         
         ```shell
         pip install opentelemetry-exporter-dynatrace-metrics
         ```
         
-        ### Usage
-        
-        The general setup of OpenTelemetry Python is explained in the official [Getting Started Guide](https://open-telemetry.github.io/opentelemetry-python/getting-started.html#add-metrics).
+        #### Usage
         
         ```python
+        from opentelemetry import metrics
+        from opentelemetry.sdk.metrics import MeterProvider
+        from dynatrace.opentelemetry.metrics.export import (
+            configure_dynatrace_metrics_export
+        )
+        
+        
         # setup metrics export pipeline
         metrics.set_meter_provider(MeterProvider(
             # configure Exporter/MetricReader combination with a 5000ms export
             # interval, endpoint url and API token.
             metric_readers=[
                 configure_dynatrace_metrics_export(
                     export_interval_millis=5000,
@@ -54,113 +79,115 @@
             description="Description of MyCounter",
             unit="1"
         )
         
         counter.add(25, {"dimension-1": "value-1"})
         ```
         
-        ### Example
+        #### Example
         
         To run the [example](example/basic_example.py), clone this repository and change to the `opentelemetry-metric-python` folder, then run:
         
         ```shell
         pip install .           # install the Dynatrace exporter
+        pip install psutil      # this package is used by the example to read CPU/Memory usage
         export LOGLEVEL=DEBUG   # (optional) Set the log level to debug to see more output (default is INFO)
         python example/basic_example.py
         ```
         
         A more complete setup routine can be found [here](example/install_and_run.sh), including installing inside a virtual environment and getting required packages.
         If you just want to see it in action, it should be sufficient to run [`example/install_and_run.sh`](example/install_and_run.sh) from the root folder.
         This script will install Python, set up a virtual environment, pull in all the required packages and run the [example](example/basic_example.py).
         
         The example also offers a simple CLI. Run `python example/basic_example.py -h` to get more information.
         
-        ### Configuration
+        #### Configuration
         
         The exporter allows for configuring the following settings by passing them to the constructor:
         
-        #### Dynatrace API Endpoint
+        ##### Dynatrace API Endpoint
         
         The endpoint to which the metrics are sent is specified using the `endpoint_url` parameter.
         
         Given an environment ID `myenv123` on Dynatrace SaaS, the [metrics ingest endpoint](https://www.dynatrace.com/support/help/dynatrace-api/environment-api/metric-v2/post-ingest-metrics/) would be `https://myenv123.live.dynatrace.com/api/v2/metrics/ingest`.
         
         If a OneAgent is installed on the host, it can provide a local endpoint for providing metrics directly without the need for an API token.
         This feature is currently in an Early Adopter phase and has to be enabled as described in the [OneAgent metric API documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/local-api/).
         Using the local API endpoint, the host ID and host name context are automatically added to each metric as dimensions.
         The default metric API endpoint exposed by the OneAgent is `http://localhost:14499/metrics/ingest`.
         If no endpoint is set and a OneAgent is running on the host, metrics will be exported to it automatically using the OneAgent with no endpoint or API token configuration required.
         
-        #### Dynatrace API Token
+        ##### Dynatrace API Token
         
         The Dynatrace API token to be used by the exporter is specified using the `api_token` parameter and could, for example, be read from an environment variable.
         
         Creating an API token for your Dynatrace environment is described in the [Dynatrace API documentation](https://www.dynatrace.com/support/help/dynatrace-api/basics/dynatrace-api-authentication/).
         The permission required for sending metrics is `Ingest metrics` (`metrics.ingest`) and it is recommended to limit scope to only this permission.
         
-        #### Metric Key Prefix
+        ##### Metric Key Prefix
         
         The `prefix` parameter specifies an optional prefix, which is prepended to each metric key, separated by a dot (`<prefix>.<name>`).
         
-        #### Default Dimensions
+        ##### Default Dimensions
         
         The `default_dimensions` parameter can be used to optionally specify a list of key/value pairs, which will be added as additional dimensions to all data points.
         Dimension keys are unique, and labels on instruments will overwrite the default dimensions if key collisions appear.
         
-        #### Export Dynatrace Metadata
+        ##### Export Dynatrace Metadata
         
         If running on a host with a running OneAgent, setting the `export_dynatrace_metadata` option to `True` will export metadata collected by the OneAgent to the Dynatrace endpoint.
         If no Dynatrace API endpoint is set, the default exporter endpoint will be the OneAgent endpoint, and this option will be set automatically.
         Therefore, if no endpoint is specified, a OneAgent is assumed to be running and used as the export endpoint for all metric lines, including metadata.
         More information on the underlying Dynatrace metadata feature that is used by the exporter can be found in the
         [Dynatrace documentation](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/ingestion-methods/enrich-metrics/).
         
-        ##### Dimensions precedence
+        ###### Dimensions precedence
         
         When specifying default dimensions, attributes and Dynatrace metadata enrichment, the precedence of dimensions with the same key is as follows:
         Default dimensions are overwritten by attributes passed to instruments, which in turn are overwritten by the Dynatrace metadata dimensions (even though the likeliness of a collision here is very low, since the Dynatrace metadata only contains [Dynatrace reserved dimensions](https://www.dynatrace.com/support/help/how-to-use-dynatrace/metrics/metric-ingestion/metric-ingestion-protocol/#syntax) starting with `dt.*`).
         
-        ## Development
+        ### Development
         
-        ### Requirements
+        #### Requirements
         
-        Just [`tox`](https://pypi.org/project/tox/).
+        Just [`tox`](https://pypi.org/project/tox/). Make sure to `pip install` the `requirements-dev.txt` to get the relevant packages. 
         
-        ### Running tests and lint
+        #### Running tests and lint
         
         * Test all supported python versions: `tox`
         * Test all supported python versions in parallel: `tox -p`
         * A particular python version: `tox -e 38`
         * Current python version: `tox -e py`
         * Lint: `tox -e lint`
         
-        ## Limitations
+        ### Limitations
         
-        ### Typed attributes support
+        #### Typed attributes support
         
         The OpenTelemetry Metrics API for Python supports the concept
         of [Attributes]( https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/common/common.md#attributes).
         These attributes consist of key-value pairs, where the keys are strings and the
         values are either primitive types or arrays of uniform primitive types.
         
         At the moment, this exporter **only supports attributes with string key and
         value type**.
         This means that if attributes of any other type are used, they will be 
         **ignored** and **only** the string-valued attributes are going to be sent to
         Dynatrace.
         
-        ### Histogram
+        #### Histogram
         
         OpenTelemetry Histograms are exported to Dynatrace as statistical summaries
         consisting of a minimum and maximum value, the total sum of all values, and the
         count of the values summarized. If the min and max values are not directly
         available on the metric data point, estimations based on the boundaries of the
         first and last buckets containing values are used.
+        
 Platform: any
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/src/opentelemetry_exporter_dynatrace_metrics.egg-info/SOURCES.txt` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/src/opentelemetry_exporter_dynatrace_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/test/test_exporter.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/test/test_exporter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry-exporter-dynatrace-metrics-1.0.2/test/test_histogram_utils.py` & `opentelemetry-exporter-dynatrace-metrics-1.0.3/test/test_histogram_utils.py`

 * *Files identical despite different names*

