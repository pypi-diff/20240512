# Comparing `tmp/syntrac_sdk-0.0.6.tar.gz` & `tmp/syntrac_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.6.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.7.tar", max compression
```

## Comparing `syntrac_sdk-0.0.6.tar` & `syntrac_sdk-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0      395 2024-05-08 11:06:52.376394 syntrac_sdk-0.0.6/README.md
--rw-r--r--   0        0        0     2072 2024-05-08 11:06:52.396781 syntrac_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7767 2024-05-08 11:06:52.378540 syntrac_sdk-0.0.6/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-05-08 11:06:52.380801 syntrac_sdk-0.0.6/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-05-08 11:06:52.381123 syntrac_sdk-0.0.6/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11612 2024-05-08 11:06:52.381461 syntrac_sdk-0.0.6/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0    16396 2024-05-08 11:06:52.382016 syntrac_sdk-0.0.6/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4393 2024-05-08 11:06:52.382247 syntrac_sdk-0.0.6/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-05-08 11:06:52.382367 syntrac_sdk-0.0.6/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-05-08 11:06:52.382541 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-05-08 11:06:52.382761 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3362 2024-05-08 11:06:52.383012 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2109 2024-05-08 11:06:52.383285 syntrac_sdk-0.0.6/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-05-08 11:06:52.383564 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-05-08 11:06:52.383907 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      225 2024-05-08 11:06:52.384152 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2024-05-08 11:06:52.384368 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0     9686 2024-05-08 11:06:52.384690 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-05-08 11:06:52.385135 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0      152 2024-05-08 11:06:52.385435 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__init__.py
--rw-r--r--   0        0        0      514 2024-05-08 11:06:52.385695 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9274 2024-05-08 11:06:52.385838 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     4571 2024-05-08 11:06:52.386119 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1345 2024-05-08 11:06:52.386260 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
--rw-r--r--   0        0        0     5583 2024-05-08 11:06:52.386400 syntrac_sdk-0.0.6/syntrac/sdk/prompts/client.py
--rw-r--r--   0        0        0     1558 2024-05-08 11:06:52.386523 syntrac_sdk-0.0.6/syntrac/sdk/prompts/model.py
--rw-r--r--   0        0        0      408 2024-05-08 11:06:52.386661 syntrac_sdk-0.0.6/syntrac/sdk/prompts/registry.py
--rw-r--r--   0        0        0     2424 2024-05-08 11:06:52.386791 syntrac_sdk-0.0.6/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-05-08 11:06:52.387182 syntrac_sdk-0.0.6/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      248 2024-05-08 11:06:52.387397 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      559 2024-05-08 11:06:52.387697 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-05-08 11:06:52.387835 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-05-08 11:06:52.388017 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0      818 2024-05-08 11:06:52.388350 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
--rw-r--r--   0        0        0    29511 2024-05-08 11:06:52.388737 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-05-08 11:06:52.388857 syntrac_sdk-0.0.6/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0      297 2024-05-08 11:06:52.389080 syntrac_sdk-0.0.6/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0      322 2024-05-08 11:06:52.389300 syntrac_sdk-0.0.6/syntrac/sdk/tracing/context_passing.py
--rw-r--r--   0        0        0    23992 2024-05-08 11:06:52.389629 syntrac_sdk-0.0.6/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      604 2024-05-08 11:06:52.389828 syntrac_sdk-0.0.6/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     1487 2024-05-08 11:06:52.390133 syntrac_sdk-0.0.6/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-05-08 11:06:52.390363 syntrac_sdk-0.0.6/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-05-08 11:06:52.390578 syntrac_sdk-0.0.6/syntrac/sdk/version.py
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-05-12 08:53:28.807631 syntrac_sdk-0.0.7/README.md
+-rw-r--r--   0        0        0     2072 2024-05-12 08:53:28.826929 syntrac_sdk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-12 08:53:28.809045 syntrac_sdk-0.0.7/syntrac/sdk/.DS_Store
+-rw-r--r--   0        0        0     6417 2024-05-12 08:53:28.809158 syntrac_sdk-0.0.7/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-12 08:53:28.811132 syntrac_sdk-0.0.7/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-05-12 08:53:28.811456 syntrac_sdk-0.0.7/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2024-05-12 08:53:28.811804 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-12 08:53:28.812218 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3126 2024-05-12 08:53:28.812507 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc
+-rw-r--r--   0        0        0    10195 2024-05-12 08:53:28.812742 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     9276 2024-05-12 08:53:28.812912 syntrac_sdk-0.0.7/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1571 2024-05-12 08:53:28.813245 syntrac_sdk-0.0.7/syntrac/sdk/decorators/helper.py
+-rw-r--r--   0        0        0     7917 2024-05-12 08:53:28.813556 syntrac_sdk-0.0.7/syntrac/sdk/decorators/task.py
+-rw-r--r--   0        0        0     7099 2024-05-12 08:53:28.813851 syntrac_sdk-0.0.7/syntrac/sdk/decorators/workflow.py
+-rw-r--r--   0        0        0     2650 2024-05-12 08:53:28.814088 syntrac_sdk-0.0.7/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-05-12 08:53:28.814201 syntrac_sdk-0.0.7/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:53:28.814430 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-12 08:53:28.814791 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3362 2024-05-12 08:53:28.815016 syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2024-05-12 08:53:28.815255 syntrac_sdk-0.0.7/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-05-12 08:53:28.815524 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-05-12 08:53:28.815836 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2024-05-12 08:53:28.816064 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2024-05-12 08:53:28.816261 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0     9686 2024-05-12 08:53:28.816578 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-05-12 08:53:28.816734 syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0     2424 2024-05-12 08:53:28.816862 syntrac_sdk-0.0.7/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-05-12 08:53:28.817160 syntrac_sdk-0.0.7/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      302 2024-05-12 08:53:28.817385 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-12 08:53:28.817703 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-05-12 08:53:28.818120 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     4806 2024-05-12 08:53:28.818307 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-05-12 08:53:28.818516 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0      818 2024-05-12 08:53:28.818774 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
+-rw-r--r--   0        0        0     2748 2024-05-12 08:53:28.818912 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0    27029 2024-05-12 08:53:28.819384 syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-05-12 08:53:28.819525 syntrac_sdk-0.0.7/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0     2509 2024-05-12 08:53:28.819650 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context.py
+-rw-r--r--   0        0        0      297 2024-05-12 08:53:28.819915 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0      322 2024-05-12 08:53:28.820140 syntrac_sdk-0.0.7/syntrac/sdk/tracing/context_passing.py
+-rw-r--r--   0        0        0     1880 2024-05-12 08:53:28.820252 syntrac_sdk-0.0.7/syntrac/sdk/tracing/span_from_context.py
+-rw-r--r--   0        0        0    22217 2024-05-12 08:53:28.820606 syntrac_sdk-0.0.7/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      878 2024-05-12 08:53:28.820842 syntrac_sdk-0.0.7/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2024-05-12 08:53:28.821058 syntrac_sdk-0.0.7/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-05-12 08:53:28.821348 syntrac_sdk-0.0.7/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-05-12 08:53:28.821473 syntrac_sdk-0.0.7/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.7/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.6/pyproject.toml` & `syntrac_sdk-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-sdk"
-version = "0.0.6"
+version = "0.0.7"
 description = "Syntrac Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac"
 documentation = "https://syntrac.com/docs/openllmetry"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -29,15 +29,15 @@
   opentelemetry-instrumentation-urllib3 = "0.44b0"
   syntrac-opentelemetry-semantic-conventions-ai = "0.0.1"
   syntrac-opentelemetry-instrumentation-openai = "0.0.2"
   syntrac-opentelemetry-instrumentation-anthropic = "0.0.2"
   syntrac-opentelemetry-instrumentation-cohere = "0.0.2"
   syntrac-opentelemetry-instrumentation-pinecone = "0.0.2"
   syntrac-opentelemetry-instrumentation-qdrant = "0.0.2"
-  syntrac-opentelemetry-instrumentation-langchain = "0.0.3"
+  syntrac-opentelemetry-instrumentation-langchain = "0.0.4"
   syntrac-opentelemetry-instrumentation-chromadb = "0.0.2"
   syntrac-opentelemetry-instrumentation-transformers = "0.0.2"
   syntrac-opentelemetry-instrumentation-llamaindex = "0.0.2"
   syntrac-opentelemetry-instrumentation-haystack = "0.0.2"
   syntrac-opentelemetry-instrumentation-bedrock = "0.0.2"
   syntrac-opentelemetry-instrumentation-replicate = "0.0.2"
   syntrac-opentelemetry-instrumentation-vertexai = "0.0.2"
```

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.7/syntrac/sdk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 import os
 import sys
-from deprecated import deprecated
-import requests
-from pathlib import Path
 
 from typing import Optional, Set
 from colorama import Fore
+from opentelemetry import trace
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import SpanExporter
 from opentelemetry.sdk.metrics.export import MetricExporter
 from opentelemetry.sdk.resources import SERVICE_NAME
 from opentelemetry.propagators.textmap import TextMapPropagator
 from opentelemetry.util.re import parse_env_headers
+from syntrac_opentelemetry.semconv.ai import SpanAttributes
 
 from syntrac.sdk.metrics.metrics import MetricsWrapper
 from syntrac.sdk.telemetry import Telemetry
 from syntrac.sdk.instruments import Instruments
 from syntrac.sdk.config import (
     is_content_tracing_enabled,
     is_tracing_enabled,
     is_metrics_enabled,
 )
 from syntrac.sdk.fetcher import Fetcher
 from syntrac.sdk.tracing.tracing import (
     TracerWrapper,
+)
+from syntrac.sdk.tracing.context import (
     set_association_properties,
-    set_correlation_id,
 )
 from typing import Dict
 
 
 class Syntrac:
-    AUTO_CREATED_KEY_PATH = str(
-        Path.home() / ".cache" / "syntrac" / "auto_created_key"
-    )
-    AUTO_CREATED_URL = str(Path.home() / ".cache" / "syntrac" / "auto_created_url")
-
     __tracer_wrapper: TracerWrapper
     __fetcher: Fetcher
 
     @staticmethod
     def init(
         app_name: Optional[str] = sys.argv[0],
         api_endpoint: str = "https://analytics-api.syntrac.dev",
-        api_key: str = None,
+        api_key: Optional[str] = None,
         headers: Dict[str, str] = {},
         disable_batch=False,
-        exporter: SpanExporter = None,
-        metrics_exporter: MetricExporter = None,
+        exporter: Optional[SpanExporter] = None,
+        metrics_exporter: Optional[MetricExporter] = None,
         metrics_headers: Dict[str, str] = {},
-        processor: SpanProcessor = None,
-        propagator: TextMapPropagator = None,
+        processor: Optional[SpanProcessor] = None,
+        propagator: Optional[TextMapPropagator] = None,
         syntrac_sync_enabled: bool = True,
         resource_attributes: dict = {},
         instruments: Optional[Set[Instruments]] = None,
     ) -> None:
         Telemetry()
 
         api_endpoint = os.getenv("SYNTRAC_BASE_URL") or api_endpoint
         api_key = os.getenv("SYNTRAC_API_KEY") or api_key
 
         if (
             syntrac_sync_enabled
-            and api_endpoint.find("syntrac.com") != -1
             and api_key
             and not exporter
             and not processor
         ):
             Syntrac.__fetcher = Fetcher(base_url=api_endpoint, api_key=api_key)
-            Syntrac.__fetcher.run()
-            print(
-                Fore.GREEN + "Syntrac syncing configuration and prompts" + Fore.RESET
-            )
 
         if not is_tracing_enabled():
             print(Fore.YELLOW + "Tracing is disabled" + Fore.RESET)
             return
 
         enable_content_tracing = is_content_tracing_enabled()
 
@@ -83,62 +73,14 @@
             print(Fore.GREEN + "Syntrac exporting traces to a custom exporter")
 
         headers = os.getenv("SYNTRAC_HEADERS") or headers
 
         if isinstance(headers, str):
             headers = parse_env_headers(headers)
 
-        # auto-create a dashboard on Syntrac if no export endpoint is provided
-        if (
-            not exporter
-            and not processor
-            and api_endpoint == "https://analytics-api.syntrac.dev"
-            and not api_key
-        ):
-            if not Telemetry().feature_enabled("auto_create_dashboard"):
-                print(
-                    Fore.RED
-                    + "Error: Missing Syntrac API key,"
-                    + " go to https://analytics-api.syntrac.dev/settings/api-keys to create one"
-                )
-                print("Set the SYNTRAC_API_KEY environment variable to the key")
-                print(Fore.RESET)
-                return
-
-            headers = None  # disable headers if we're auto-creating a dashboard
-            if not os.path.exists(
-                Syntrac.AUTO_CREATED_KEY_PATH
-            ) or not os.path.exists(Syntrac.AUTO_CREATED_URL):
-                os.makedirs(
-                    os.path.dirname(Syntrac.AUTO_CREATED_KEY_PATH), exist_ok=True
-                )
-                os.makedirs(os.path.dirname(Syntrac.AUTO_CREATED_URL), exist_ok=True)
-
-                print(
-                    Fore.YELLOW
-                    + "No Syntrac API key provided, auto-creating a dashboard on Syntrac",
-                )
-                res = requests.post(
-                    "https://analytics-api.syntrac.dev/api/registration/auto-create"
-                ).json()
-                access_url = f"https://analytics-api.syntrac.dev/trace?skt={res['uiAccessKey']}"
-                api_key = res["apiKey"]
-
-                print(Fore.YELLOW + "SYNTRAC_API_KEY=", api_key)
-
-                open(Syntrac.AUTO_CREATED_KEY_PATH, "w").write(api_key)
-                open(Syntrac.AUTO_CREATED_URL, "w").write(access_url)
-            else:
-                api_key = open("/tmp/syntrac_key.txt").read()
-                access_url = open("/tmp/syntrac_url.txt").read()
-
-            print(
-                Fore.GREEN + f"\nGo to {access_url} to see a live dashboard\n",
-            )
-
         if not exporter and not processor and headers:
             print(
                 Fore.GREEN
                 + f"Syntrac exporting traces to {api_endpoint}, authenticating with custom headers"
             )
 
         if api_key and not exporter and not processor and not headers:
@@ -179,37 +121,71 @@
 
         MetricsWrapper.set_static_params(
             resource_attributes, metrics_endpoint, metrics_headers
         )
         Syntrac.__metrics_wrapper = MetricsWrapper(exporter=metrics_exporter)
 
     @staticmethod
-    @deprecated(version="0.0.62", reason="Use set_association_properties instead")
-    def set_correlation_id(correlation_id: str) -> None:
-        set_correlation_id(correlation_id)
-
     def set_association_properties(properties: dict) -> None:
         set_association_properties(properties)
 
+    @staticmethod
     def report_score(
-        association_property_name: str,
-        association_property_id: str,
+        id: Optional[str],
         score: float,
     ):
+        """Apply score to all llm steps belongs to action
+        id: action_id or unique id linked by associate_trace method
+        """
         if not Syntrac.__fetcher:
             print(
                 Fore.RED
                 + "Error: Cannot report score. Missing Syntrac API key,"
                 + " go to https://app.syntrac.com/settings/api-keys to create one"
             )
             print("Set the SYNTRAC_API_KEY environment variable to the key")
             print(Fore.RESET)
             return
 
-        Syntrac.__fetcher.post(
-            "score",
+        Syntrac.__fetcher.patch(
+            f"actions/{id}/score",
             {
-                "entity_name": f"syntrac.association.properties.{association_property_name}",
-                "entity_id": association_property_id,
                 "score": score,
             },
         )
+
+    @staticmethod
+    def associate_trace(id: str, span_id: Optional[str]):
+        """Associate trace and space with a unique id
+        id: unique id linked with trace
+        span_id: unique id linked with span
+        """
+        span = trace.get_current_span()
+        span.set_attribute(
+          f"{SpanAttributes.SYNTRAC_ASSOCIATION_PROPERTIES}.trace_alias",
+          id
+        )
+        if span_id:
+            span.set_attribute(
+              f"{SpanAttributes.SYNTRAC_ASSOCIATION_PROPERTIES}.span_alias",
+              span_id
+            )
+
+    @staticmethod
+    def update_span(id: str, body: Dict[str, str]):
+        """Update span value with data if processed asynchronously
+        id: span_id or unique id linked with span
+        """
+        if not Syntrac.__fetcher:
+            print(
+                Fore.RED
+                + "Error: Cannot report score. Missing Syntrac API key,"
+                + " go to https://app.syntrac.com/settings/api-keys to create one"
+            )
+            print("Set the SYNTRAC_API_KEY environment variable to the key")
+            print(Fore.RESET)
+            return
+
+        Syntrac.__fetcher.patch(
+            f"steps/{id}",
+            body,
+        )
```

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.7/syntrac/sdk/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.7/syntrac/sdk/otlp/json/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.5"
+__version__ = "0.0.7"
```

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.7/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.7/syntrac/sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,33 @@
 magic:    0xa70d0d0a
-moddate:  0x060a0966 (Sun Mar 31 07:00:22 2024 UTC)
-files sz: 23992
+moddate:  0x61f43e66 (Sat May 11 04:30:25 2024 UTC)
+files sz: 22217
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 12
+   stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       016c035a04640064026c056d065a060100640064036c076d085a08010064
-      0064046c096d0a5a0a0100640064056c0b6d0c5a0c0100640064066c0d6d
-      0e5a0e6d0f5a0f0100640064076c106d115a110100640064086c126d135a
-      130100640064096c146d155a156d165a166d175a1701006400640a6c186d
-      195a196d1a5a1a01006400640b6c1b6d1c5a1c6d1d5a1d6d1e5a1e010064
-      00640c6c1f6d205a2001006400640d6c216d225a2201006400640e6c236d
-      245a2401006400640f6c256d265a260100640064106c276d285a28010064
-      0064116c296d2a5a2a6d2b5a2b6d2c5a2c010064125a2d64135a2e020047
-      00641484006415652fa6030000ab0300000000000000005a306416653164
-      1764016604641884045a3264196533641764016604641a84045a34641b65
-      31641764016604641c84045a35641d6531641e6536641f65316420653164
-      21653364176401660c642284045a37641765386602642384045a39642465
-      316425652a65316531660219000000000000000000641765156606642684
-      045a3a6427650c6417650e6604642884045a3b642984005a3c642a84005a
-      3d642b84005a3e642c84005a3f642d84005a40642e84005a41642f84005a
-      42643084005a43643184005a44643284005a45643384005a46643484005a
-      47643584005a48643684005a49643784005a4a643884005a4b643984005a
-      4c643a84005a4d643b84005a4e64015300
+      0064046c096d0a5a0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d
+      0f5a0f6d105a100100640064066c116d125a120100640064076c136d145a
+      146d155a150100640064086c166d175a170100640064096c186d195a1901
+      006400640a6c1a6d1b5a1b6d1c5a1c6d1d5a1d01006400640b6c1e6d1f5a
+      1f6d205a2001006400640c6c216d225a2201006400640d6c236d245a2401
+      006400640e6c256d265a2601006400640f6c276d285a280100640064106c
+      296d2a5a2a0100640064116c2b6d2c5a2c6d2d5a2d0100640064126c2e6d
+      2f5a2f6d305a30010064135a3164145a32020047006415840064166533a6
+      030000ab0300000000000000005a34641765356602641884045a36641965
+      37641a650e653765376602190000000000000000006417651b6606641b84
+      045a38641c6512641765146604641d84045a39641e84005a3a641f84005a
+      3b642084005a3c642184005a3d642284005a3e642384005a3f642484005a
+      40642584005a41642684005a42642784005a43642884005a44642984005a
+      45642a84005a46642b84005a47642c84005a48642d84005a49642e84005a
+      4a642f84005a4b643084005a4c64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (atexit)
                  8 STORE_NAME               0 (atexit)
    
@@ -66,495 +64,503 @@
                 60 LOAD_CONST               4 (('OTLPSpanExporter',))
                 62 IMPORT_NAME              9 (syntrac.sdk.otlp.json.trace_exporter)
                 64 IMPORT_FROM             10 (OTLPSpanExporter)
                 66 STORE_NAME              10 (OTLPSpanExporter)
                 68 POP_TOP
    
     12          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               5 (('Resource',))
-                74 IMPORT_NAME             11 (opentelemetry.sdk.resources)
-                76 IMPORT_FROM             12 (Resource)
-                78 STORE_NAME              12 (Resource)
-                80 POP_TOP
-   
-    13          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               6 (('TracerProvider', 'SpanProcessor'))
-                86 IMPORT_NAME             13 (opentelemetry.sdk.trace)
-                88 IMPORT_FROM             14 (TracerProvider)
-                90 STORE_NAME              14 (TracerProvider)
-                92 IMPORT_FROM             15 (SpanProcessor)
-                94 STORE_NAME              15 (SpanProcessor)
+                72 LOAD_CONST               5 (('Any', 'Callable', 'Dict', 'Optional', 'Set'))
+                74 IMPORT_NAME             11 (typing)
+                76 IMPORT_FROM             12 (Any)
+                78 STORE_NAME              12 (Any)
+                80 IMPORT_FROM             13 (Callable)
+                82 STORE_NAME              13 (Callable)
+                84 IMPORT_FROM             14 (Dict)
+                86 STORE_NAME              14 (Dict)
+                88 IMPORT_FROM             15 (Optional)
+                90 STORE_NAME              15 (Optional)
+                92 IMPORT_FROM             16 (Set)
+                94 STORE_NAME              16 (Set)
                 96 POP_TOP
    
-    14          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               7 (('TextMapPropagator',))
-               102 IMPORT_NAME             16 (opentelemetry.propagators.textmap)
-               104 IMPORT_FROM             17 (TextMapPropagator)
-               106 STORE_NAME              17 (TextMapPropagator)
+    13          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               6 (('Resource',))
+               102 IMPORT_NAME             17 (opentelemetry.sdk.resources)
+               104 IMPORT_FROM             18 (Resource)
+               106 STORE_NAME              18 (Resource)
                108 POP_TOP
    
-    15         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               8 (('set_global_textmap',))
-               114 IMPORT_NAME             18 (opentelemetry.propagate)
-               116 IMPORT_FROM             19 (set_global_textmap)
-               118 STORE_NAME              19 (set_global_textmap)
-               120 POP_TOP
-   
-    16         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST               9 (('SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor'))
-               126 IMPORT_NAME             20 (opentelemetry.sdk.trace.export)
-               128 IMPORT_FROM             21 (SpanExporter)
-               130 STORE_NAME              21 (SpanExporter)
-               132 IMPORT_FROM             22 (SimpleSpanProcessor)
-               134 STORE_NAME              22 (SimpleSpanProcessor)
-               136 IMPORT_FROM             23 (BatchSpanProcessor)
-               138 STORE_NAME              23 (BatchSpanProcessor)
-               140 POP_TOP
-   
-    21         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              10 (('get_tracer_provider', 'ProxyTracerProvider'))
-               146 IMPORT_NAME             24 (opentelemetry.trace)
-               148 IMPORT_FROM             25 (get_tracer_provider)
-               150 STORE_NAME              25 (get_tracer_provider)
-               152 IMPORT_FROM             26 (ProxyTracerProvider)
-               154 STORE_NAME              26 (ProxyTracerProvider)
-               156 POP_TOP
-   
-    22         158 LOAD_CONST               0 (0)
-               160 LOAD_CONST              11 (('get_value', 'attach', 'set_value'))
-               162 IMPORT_NAME             27 (opentelemetry.context)
-               164 IMPORT_FROM             28 (get_value)
-               166 STORE_NAME              28 (get_value)
-               168 IMPORT_FROM             29 (attach)
-               170 STORE_NAME              29 (attach)
-               172 IMPORT_FROM             30 (set_value)
-               174 STORE_NAME              30 (set_value)
-               176 POP_TOP
-   
-    24         178 LOAD_CONST               0 (0)
-               180 LOAD_CONST              12 (('SpanAttributes',))
-               182 IMPORT_NAME             31 (syntrac_opentelemetry.semconv.ai)
-               184 IMPORT_FROM             32 (SpanAttributes)
-               186 STORE_NAME              32 (SpanAttributes)
-               188 POP_TOP
-   
-    25         190 LOAD_CONST               0 (0)
-               192 LOAD_CONST              13 (('Telemetry',))
-               194 IMPORT_NAME             33 (syntrac.sdk)
-               196 IMPORT_FROM             34 (Telemetry)
-               198 STORE_NAME              34 (Telemetry)
-               200 POP_TOP
-   
-    26         202 LOAD_CONST               0 (0)
-               204 LOAD_CONST              14 (('Instruments',))
-               206 IMPORT_NAME             35 (syntrac.sdk.instruments)
-               208 IMPORT_FROM             36 (Instruments)
-               210 STORE_NAME              36 (Instruments)
-               212 POP_TOP
-   
-    27         214 LOAD_CONST               0 (0)
-               216 LOAD_CONST              15 (('ContentAllowList',))
-               218 IMPORT_NAME             37 (syntrac.sdk.tracing.content_allow_list)
-               220 IMPORT_FROM             38 (ContentAllowList)
-               222 STORE_NAME              38 (ContentAllowList)
-               224 POP_TOP
-   
-    28         226 LOAD_CONST               0 (0)
-               228 LOAD_CONST              16 (('is_notebook',))
-               230 IMPORT_NAME             39 (syntrac.sdk.utils)
-               232 IMPORT_FROM             40 (is_notebook)
-               234 STORE_NAME              40 (is_notebook)
-               236 POP_TOP
-   
-    29         238 LOAD_CONST               0 (0)
-               240 LOAD_CONST              17 (('Dict', 'Optional', 'Set'))
-               242 IMPORT_NAME             41 (typing)
-               244 IMPORT_FROM             42 (Dict)
-               246 STORE_NAME              42 (Dict)
-               248 IMPORT_FROM             43 (Optional)
-               250 STORE_NAME              43 (Optional)
-               252 IMPORT_FROM             44 (Set)
-               254 STORE_NAME              44 (Set)
-               256 POP_TOP
-   
-    31         258 LOAD_CONST              18 ('syntrac.tracer')
-               260 STORE_NAME              45 (TRACER_NAME)
-   
-    32         262 LOAD_CONST              19 ('\n    iam.cloud.ibm.com,\n    dataplatform.cloud.ibm.com,\n    ml.cloud.ibm.com,\n    api.openai.com,\n    openai.azure.com,\n    api.anthropic.com,\n    api.cohere.ai,\n    pinecone.io,\n    syntrac.com,\n    posthog.com,\n    bedrock-runtime,\n    googleapis.com,\n    githubusercontent.com')
-               264 STORE_NAME              46 (EXCLUDED_URLS)
-   
-    48         266 PUSH_NULL
-               268 LOAD_BUILD_CLASS
-               270 LOAD_CONST              20 (<code object TracerWrapper, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 48>)
-               272 MAKE_FUNCTION            0
-               274 LOAD_CONST              21 ('TracerWrapper')
-               276 LOAD_NAME               47 (object)
-               278 PRECALL                  3
-               282 CALL                     3
-               292 STORE_NAME              48 (TracerWrapper)
-   
-   353         294 LOAD_CONST              22 ('correlation_id')
-               296 LOAD_NAME               49 (str)
-               298 LOAD_CONST              23 ('return')
-               300 LOAD_CONST               1 (None)
-               302 BUILD_TUPLE              4
-               304 LOAD_CONST              24 (<code object set_correlation_id, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 353>)
-               306 MAKE_FUNCTION            4 (annotations)
-               308 STORE_NAME              50 (set_correlation_id)
-   
-   357         310 LOAD_CONST              25 ('properties')
-               312 LOAD_NAME               51 (dict)
-               314 LOAD_CONST              23 ('return')
-               316 LOAD_CONST               1 (None)
-               318 BUILD_TUPLE              4
-               320 LOAD_CONST              26 (<code object set_association_properties, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 357>)
+    14         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               7 (('TracerProvider', 'SpanProcessor'))
+               114 IMPORT_NAME             19 (opentelemetry.sdk.trace)
+               116 IMPORT_FROM             20 (TracerProvider)
+               118 STORE_NAME              20 (TracerProvider)
+               120 IMPORT_FROM             21 (SpanProcessor)
+               122 STORE_NAME              21 (SpanProcessor)
+               124 POP_TOP
+   
+    15         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST               8 (('TextMapPropagator',))
+               130 IMPORT_NAME             22 (opentelemetry.propagators.textmap)
+               132 IMPORT_FROM             23 (TextMapPropagator)
+               134 STORE_NAME              23 (TextMapPropagator)
+               136 POP_TOP
+   
+    16         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST               9 (('set_global_textmap',))
+               142 IMPORT_NAME             24 (opentelemetry.propagate)
+               144 IMPORT_FROM             25 (set_global_textmap)
+               146 STORE_NAME              25 (set_global_textmap)
+               148 POP_TOP
+   
+    17         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST              10 (('SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor'))
+               154 IMPORT_NAME             26 (opentelemetry.sdk.trace.export)
+               156 IMPORT_FROM             27 (SpanExporter)
+               158 STORE_NAME              27 (SpanExporter)
+               160 IMPORT_FROM             28 (SimpleSpanProcessor)
+               162 STORE_NAME              28 (SimpleSpanProcessor)
+               164 IMPORT_FROM             29 (BatchSpanProcessor)
+               166 STORE_NAME              29 (BatchSpanProcessor)
+               168 POP_TOP
+   
+    22         170 LOAD_CONST               0 (0)
+               172 LOAD_CONST              11 (('get_tracer_provider', 'ProxyTracerProvider'))
+               174 IMPORT_NAME             30 (opentelemetry.trace)
+               176 IMPORT_FROM             31 (get_tracer_provider)
+               178 STORE_NAME              31 (get_tracer_provider)
+               180 IMPORT_FROM             32 (ProxyTracerProvider)
+               182 STORE_NAME              32 (ProxyTracerProvider)
+               184 POP_TOP
+   
+    24         186 LOAD_CONST               0 (0)
+               188 LOAD_CONST              12 (('SpanAttributes',))
+               190 IMPORT_NAME             33 (syntrac_opentelemetry.semconv.ai)
+               192 IMPORT_FROM             34 (SpanAttributes)
+               194 STORE_NAME              34 (SpanAttributes)
+               196 POP_TOP
+   
+    25         198 LOAD_CONST               0 (0)
+               200 LOAD_CONST              13 (('Telemetry',))
+               202 IMPORT_NAME             35 (syntrac.sdk)
+               204 IMPORT_FROM             36 (Telemetry)
+               206 STORE_NAME              36 (Telemetry)
+               208 POP_TOP
+   
+    26         210 LOAD_CONST               0 (0)
+               212 LOAD_CONST              14 (('Instruments',))
+               214 IMPORT_NAME             37 (syntrac.sdk.instruments)
+               216 IMPORT_FROM             38 (Instruments)
+               218 STORE_NAME              38 (Instruments)
+               220 POP_TOP
+   
+    27         222 LOAD_CONST               0 (0)
+               224 LOAD_CONST              15 (('ContentAllowList',))
+               226 IMPORT_NAME             39 (syntrac.sdk.tracing.content_allow_list)
+               228 IMPORT_FROM             40 (ContentAllowList)
+               230 STORE_NAME              40 (ContentAllowList)
+               232 POP_TOP
+   
+    28         234 LOAD_CONST               0 (0)
+               236 LOAD_CONST              16 (('is_notebook',))
+               238 IMPORT_NAME             41 (syntrac.sdk.utils)
+               240 IMPORT_FROM             42 (is_notebook)
+               242 STORE_NAME              42 (is_notebook)
+               244 POP_TOP
+   
+    29         246 LOAD_CONST               0 (0)
+               248 LOAD_CONST              17 (('set_override_enable_context_tracing', 'get_association_properties'))
+               250 IMPORT_NAME             43 (syntrac.sdk.tracing.context)
+               252 IMPORT_FROM             44 (set_override_enable_context_tracing)
+               254 STORE_NAME              44 (set_override_enable_context_tracing)
+               256 IMPORT_FROM             45 (get_association_properties)
+               258 STORE_NAME              45 (get_association_properties)
+               260 POP_TOP
+   
+    30         262 LOAD_CONST               0 (0)
+               264 LOAD_CONST              18 (('set_workflow_name_from_context', 'set_prompt_attributes_from_context'))
+               266 IMPORT_NAME             46 (syntrac.sdk.tracing.span_from_context)
+               268 IMPORT_FROM             47 (set_workflow_name_from_context)
+               270 STORE_NAME              47 (set_workflow_name_from_context)
+               272 IMPORT_FROM             48 (set_prompt_attributes_from_context)
+               274 STORE_NAME              48 (set_prompt_attributes_from_context)
+               276 POP_TOP
+   
+    32         278 LOAD_CONST              19 ('syntrac.tracer')
+               280 STORE_NAME              49 (TRACER_NAME)
+   
+    33         282 LOAD_CONST              20 ('\n    iam.cloud.ibm.com,\n    dataplatform.cloud.ibm.com,\n    ml.cloud.ibm.com,\n    api.openai.com,\n    openai.azure.com,\n    api.anthropic.com,\n    api.cohere.ai,\n    pinecone.io,\n    syntrac.com,\n    posthog.com,\n    bedrock-runtime,\n    googleapis.com,\n    githubusercontent.com')
+               284 STORE_NAME              50 (EXCLUDED_URLS)
+   
+    49         286 PUSH_NULL
+               288 LOAD_BUILD_CLASS
+               290 LOAD_CONST              21 (<code object TracerWrapper, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 49>)
+               292 MAKE_FUNCTION            0
+               294 LOAD_CONST              22 ('TracerWrapper')
+               296 LOAD_NAME               51 (object)
+               298 PRECALL                  3
+               302 CALL                     3
+               312 STORE_NAME              52 (TracerWrapper)
+   
+   332         314 LOAD_CONST              23 ('return')
+               316 LOAD_NAME               53 (bool)
+               318 BUILD_TUPLE              2
+               320 LOAD_CONST              24 (<code object is_llm_span, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 332>)
                322 MAKE_FUNCTION            4 (annotations)
-               324 STORE_NAME              52 (set_association_properties)
+               324 STORE_NAME              54 (is_llm_span)
    
-   361         326 LOAD_CONST              27 ('workflow_name')
-               328 LOAD_NAME               49 (str)
-               330 LOAD_CONST              23 ('return')
-               332 LOAD_CONST               1 (None)
-               334 BUILD_TUPLE              4
-               336 LOAD_CONST              28 (<code object set_workflow_name, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 361>)
-               338 MAKE_FUNCTION            4 (annotations)
-               340 STORE_NAME              53 (set_workflow_name)
-   
-   365         342 LOAD_CONST              29 ('key')
-   
-   366         344 LOAD_NAME               49 (str)
-   
-   365         346 LOAD_CONST              30 ('version')
-   
-   367         348 LOAD_NAME               54 (int)
-   
-   365         350 LOAD_CONST              31 ('version_name')
-   
-   368         352 LOAD_NAME               49 (str)
-   
-   365         354 LOAD_CONST              32 ('version_hash')
-   
-   369         356 LOAD_NAME               49 (str)
-   
-   365         358 LOAD_CONST              33 ('template_variables')
-   
-   370         360 LOAD_NAME               51 (dict)
-   
-   365         362 LOAD_CONST              23 ('return')
-   
-   371         364 LOAD_CONST               1 (None)
-   
-   365         366 BUILD_TUPLE             12
-               368 LOAD_CONST              34 (<code object set_prompt_tracing_context, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 365>)
-               370 MAKE_FUNCTION            4 (annotations)
-               372 STORE_NAME              55 (set_prompt_tracing_context)
-   
-   379         374 LOAD_CONST              23 ('return')
-               376 LOAD_NAME               56 (bool)
-               378 BUILD_TUPLE              2
-               380 LOAD_CONST              35 (<code object is_llm_span, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 379>)
-               382 MAKE_FUNCTION            4 (annotations)
-               384 STORE_NAME              57 (is_llm_span)
-   
-   383         386 LOAD_CONST              36 ('api_endpoint')
-               388 LOAD_NAME               49 (str)
-               390 LOAD_CONST              37 ('headers')
-               392 LOAD_NAME               42 (Dict)
-               394 LOAD_NAME               49 (str)
-               396 LOAD_NAME               49 (str)
-               398 BUILD_TUPLE              2
-               400 BINARY_SUBSCR
-               410 LOAD_CONST              23 ('return')
-               412 LOAD_NAME               21 (SpanExporter)
-               414 BUILD_TUPLE              6
-               416 LOAD_CONST              38 (<code object init_spans_exporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 383>)
-               418 MAKE_FUNCTION            4 (annotations)
-               420 STORE_NAME              58 (init_spans_exporter)
-   
-   387         422 LOAD_CONST              39 ('resource')
-               424 LOAD_NAME               12 (Resource)
-               426 LOAD_CONST              23 ('return')
-               428 LOAD_NAME               14 (TracerProvider)
-               430 BUILD_TUPLE              4
-               432 LOAD_CONST              40 (<code object init_tracer_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 387>)
-               434 MAKE_FUNCTION            4 (annotations)
-               436 STORE_NAME              59 (init_tracer_provider)
+   336         326 LOAD_CONST              25 ('api_endpoint')
+               328 LOAD_NAME               55 (str)
+               330 LOAD_CONST              26 ('headers')
+               332 LOAD_NAME               14 (Dict)
+               334 LOAD_NAME               55 (str)
+               336 LOAD_NAME               55 (str)
+               338 BUILD_TUPLE              2
+               340 BINARY_SUBSCR
+               350 LOAD_CONST              23 ('return')
+               352 LOAD_NAME               27 (SpanExporter)
+               354 BUILD_TUPLE              6
+               356 LOAD_CONST              27 (<code object init_spans_exporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 336>)
+               358 MAKE_FUNCTION            4 (annotations)
+               360 STORE_NAME              56 (init_spans_exporter)
+   
+   340         362 LOAD_CONST              28 ('resource')
+               364 LOAD_NAME               18 (Resource)
+               366 LOAD_CONST              23 ('return')
+               368 LOAD_NAME               20 (TracerProvider)
+               370 BUILD_TUPLE              4
+               372 LOAD_CONST              29 (<code object init_tracer_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 340>)
+               374 MAKE_FUNCTION            4 (annotations)
+               376 STORE_NAME              57 (init_tracer_provider)
+   
+   358         378 LOAD_CONST              30 (<code object init_instrumentations, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 358>)
+               380 MAKE_FUNCTION            0
+               382 STORE_NAME              58 (init_instrumentations)
+   
+   379         384 LOAD_CONST              31 (<code object init_openai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 379>)
+               386 MAKE_FUNCTION            0
+               388 STORE_NAME              59 (init_openai_instrumentor)
+   
+   390         390 LOAD_CONST              32 (<code object init_anthropic_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 390>)
+               392 MAKE_FUNCTION            0
+               394 STORE_NAME              60 (init_anthropic_instrumentor)
+   
+   401         396 LOAD_CONST              33 (<code object init_cohere_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 401>)
+               398 MAKE_FUNCTION            0
+               400 STORE_NAME              61 (init_cohere_instrumentor)
+   
+   412         402 LOAD_CONST              34 (<code object init_pinecone_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 412>)
+               404 MAKE_FUNCTION            0
+               406 STORE_NAME              62 (init_pinecone_instrumentor)
+   
+   423         408 LOAD_CONST              35 (<code object init_qdrant_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 423>)
+               410 MAKE_FUNCTION            0
+               412 STORE_NAME              63 (init_qdrant_instrumentor)
+   
+   433         414 LOAD_CONST              36 (<code object init_chroma_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 433>)
+               416 MAKE_FUNCTION            0
+               418 STORE_NAME              64 (init_chroma_instrumentor)
+   
+   444         420 LOAD_CONST              37 (<code object init_haystack_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 444>)
+               422 MAKE_FUNCTION            0
+               424 STORE_NAME              65 (init_haystack_instrumentor)
+   
+   455         426 LOAD_CONST              38 (<code object init_langchain_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 455>)
+               428 MAKE_FUNCTION            0
+               430 STORE_NAME              66 (init_langchain_instrumentor)
+   
+   466         432 LOAD_CONST              39 (<code object init_transformers_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 466>)
+               434 MAKE_FUNCTION            0
+               436 STORE_NAME              67 (init_transformers_instrumentor)
    
-   405         438 LOAD_CONST              41 (<code object init_instrumentations, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 405>)
+   477         438 LOAD_CONST              40 (<code object init_llama_index_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 477>)
                440 MAKE_FUNCTION            0
-               442 STORE_NAME              60 (init_instrumentations)
+               442 STORE_NAME              68 (init_llama_index_instrumentor)
    
-   426         444 LOAD_CONST              42 (<code object init_openai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 426>)
+   488         444 LOAD_CONST              41 (<code object init_requests_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 488>)
                446 MAKE_FUNCTION            0
-               448 STORE_NAME              61 (init_openai_instrumentor)
+               448 STORE_NAME              69 (init_requests_instrumentor)
    
-   437         450 LOAD_CONST              43 (<code object init_anthropic_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 437>)
+   498         450 LOAD_CONST              42 (<code object init_urllib3_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 498>)
                452 MAKE_FUNCTION            0
-               454 STORE_NAME              62 (init_anthropic_instrumentor)
+               454 STORE_NAME              70 (init_urllib3_instrumentor)
    
-   448         456 LOAD_CONST              44 (<code object init_cohere_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 448>)
+   508         456 LOAD_CONST              43 (<code object init_pymysql_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 508>)
                458 MAKE_FUNCTION            0
-               460 STORE_NAME              63 (init_cohere_instrumentor)
+               460 STORE_NAME              71 (init_pymysql_instrumentor)
    
-   459         462 LOAD_CONST              45 (<code object init_pinecone_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 459>)
+   518         462 LOAD_CONST              44 (<code object init_bedrock_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 518>)
                464 MAKE_FUNCTION            0
-               466 STORE_NAME              64 (init_pinecone_instrumentor)
+               466 STORE_NAME              72 (init_bedrock_instrumentor)
    
-   470         468 LOAD_CONST              46 (<code object init_qdrant_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 470>)
+   528         468 LOAD_CONST              45 (<code object init_replicate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 528>)
                470 MAKE_FUNCTION            0
-               472 STORE_NAME              65 (init_qdrant_instrumentor)
+               472 STORE_NAME              73 (init_replicate_instrumentor)
    
-   480         474 LOAD_CONST              47 (<code object init_chroma_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 480>)
+   539         474 LOAD_CONST              46 (<code object init_vertexai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 539>)
                476 MAKE_FUNCTION            0
-               478 STORE_NAME              66 (init_chroma_instrumentor)
+               478 STORE_NAME              74 (init_vertexai_instrumentor)
    
-   491         480 LOAD_CONST              48 (<code object init_haystack_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 491>)
+   550         480 LOAD_CONST              47 (<code object init_watsonx_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 550>)
                482 MAKE_FUNCTION            0
-               484 STORE_NAME              67 (init_haystack_instrumentor)
+               484 STORE_NAME              75 (init_watsonx_instrumentor)
    
-   502         486 LOAD_CONST              49 (<code object init_langchain_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 502>)
+   561         486 LOAD_CONST              48 (<code object init_weaviate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 561>)
                488 MAKE_FUNCTION            0
-               490 STORE_NAME              68 (init_langchain_instrumentor)
-   
-   513         492 LOAD_CONST              50 (<code object init_transformers_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 513>)
-               494 MAKE_FUNCTION            0
-               496 STORE_NAME              69 (init_transformers_instrumentor)
-   
-   524         498 LOAD_CONST              51 (<code object init_llama_index_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 524>)
-               500 MAKE_FUNCTION            0
-               502 STORE_NAME              70 (init_llama_index_instrumentor)
-   
-   535         504 LOAD_CONST              52 (<code object init_requests_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 535>)
-               506 MAKE_FUNCTION            0
-               508 STORE_NAME              71 (init_requests_instrumentor)
-   
-   545         510 LOAD_CONST              53 (<code object init_urllib3_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 545>)
-               512 MAKE_FUNCTION            0
-               514 STORE_NAME              72 (init_urllib3_instrumentor)
-   
-   555         516 LOAD_CONST              54 (<code object init_pymysql_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 555>)
-               518 MAKE_FUNCTION            0
-               520 STORE_NAME              73 (init_pymysql_instrumentor)
-   
-   565         522 LOAD_CONST              55 (<code object init_bedrock_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 565>)
-               524 MAKE_FUNCTION            0
-               526 STORE_NAME              74 (init_bedrock_instrumentor)
-   
-   575         528 LOAD_CONST              56 (<code object init_replicate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 575>)
-               530 MAKE_FUNCTION            0
-               532 STORE_NAME              75 (init_replicate_instrumentor)
-   
-   586         534 LOAD_CONST              57 (<code object init_vertexai_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 586>)
-               536 MAKE_FUNCTION            0
-               538 STORE_NAME              76 (init_vertexai_instrumentor)
-   
-   597         540 LOAD_CONST              58 (<code object init_watsonx_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 597>)
-               542 MAKE_FUNCTION            0
-               544 STORE_NAME              77 (init_watsonx_instrumentor)
-   
-   608         546 LOAD_CONST              59 (<code object init_weaviate_instrumentor, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 608>)
-               548 MAKE_FUNCTION            0
-               550 STORE_NAME              78 (init_weaviate_instrumentor)
-               552 LOAD_CONST               1 (None)
-               554 RETURN_VALUE
+               490 STORE_NAME              76 (init_weaviate_instrumentor)
+               492 LOAD_CONST               1 (None)
+               494 RETURN_VALUE
    consts
       0
       None
       ('Fore',)
       ('trace',)
       ('OTLPSpanExporter',)
+      ('Any', 'Callable', 'Dict', 'Optional', 'Set')
       ('Resource',)
       ('TracerProvider', 'SpanProcessor')
       ('TextMapPropagator',)
       ('set_global_textmap',)
       ('SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor')
       ('get_tracer_provider', 'ProxyTracerProvider')
-      ('get_value', 'attach', 'set_value')
       ('SpanAttributes',)
       ('Telemetry',)
       ('Instruments',)
       ('ContentAllowList',)
       ('is_notebook',)
-      ('Dict', 'Optional', 'Set')
+      ('set_override_enable_context_tracing', 'get_association_properties')
+      ('set_workflow_name_from_context', 'set_prompt_attributes_from_context')
       'syntrac.tracer'
       '\n    iam.cloud.ibm.com,\n    dataplatform.cloud.ibm.com,\n    ml.cloud.ibm.com,\n    api.openai.com,\n    openai.azure.com,\n    api.anthropic.com,\n    api.cohere.ai,\n    pinecone.io,\n    syntrac.com,\n    posthog.com,\n    bedrock-runtime,\n    googleapis.com,\n    githubusercontent.com'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x8700970065005a0164005a02550069005a036504650564013c00000064
-            025a066507650564033c00000064045a086509650564053c00000069005a
-            0a650b65096509660219000000000000000000650564063c000000090009
-            0009000900090064146408650c6409650d640a650e640b650f6510651119
-            00000000000000000019000000000000000000640c6400660a8800660164
-            0d840d5a12640e84005a13640f84005a1465156401650464036507640565
-            096406650b65096509660219000000000000000000640c6404660a641084
-            04a6000000ab0000000000000000005a166517640c6507660264118404a6
-            000000ab0000000000000000005a18641284005a19641384005a1a880078
-            015a1b5300
+            025a066507650564033c00000064045a086509650a190000000000000000
+            00650564053c00000069005a0b650c650a650a6602190000000000000000
+            00650564063c000000650d650564073c000000650e650564083c00000065
+            0f650564093c00000064045a106509651119000000000000000000650564
+            0a3c00000065126505640b3c00000065136505640c3c0000000900090009
+            0009000900641a640e6509650f19000000000000000000640f6509651419
+            000000000000000000641065096512190000000000000000006411650965
+            156516190000000000000000001900000000000000000064126400660a88
+            0066016413840d5a17641484005a18641584005a19651a64016504640365
+            076405650a6406650c650a650a6602190000000000000000006412640466
+            0a64168404a6000000ab0000000000000000005a1b651c64126507660264
+            178404a6000000ab0000000000000000005a1d641884005a1e641984005a
+            1f880078015a205300
                        0 MAKE_CELL                0 (__class__)
          
-          48           2 RESUME                   0
+          49           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('TracerWrapper')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-          49          14 BUILD_MAP                0
+          50          14 BUILD_MAP                0
                       16 STORE_NAME               3 (resource_attributes)
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_NAME                5 (__annotations__)
                       22 LOAD_CONST               1 ('resource_attributes')
                       24 STORE_SUBSCR
          
-          50          28 LOAD_CONST               2 (True)
+          51          28 LOAD_CONST               2 (True)
                       30 STORE_NAME               6 (enable_content_tracing)
                       32 LOAD_NAME                7 (bool)
                       34 LOAD_NAME                5 (__annotations__)
                       36 LOAD_CONST               3 ('enable_content_tracing')
                       38 STORE_SUBSCR
          
-          51          42 LOAD_CONST               4 (None)
+          52          42 LOAD_CONST               4 (None)
                       44 STORE_NAME               8 (endpoint)
-                      46 LOAD_NAME                9 (str)
-                      48 LOAD_NAME                5 (__annotations__)
-                      50 LOAD_CONST               5 ('endpoint')
-                      52 STORE_SUBSCR
+                      46 LOAD_NAME                9 (Optional)
+                      48 LOAD_NAME               10 (str)
+                      50 BINARY_SUBSCR
+                      60 LOAD_NAME                5 (__annotations__)
+                      62 LOAD_CONST               5 ('endpoint')
+                      64 STORE_SUBSCR
          
-          52          56 BUILD_MAP                0
-                      58 STORE_NAME              10 (headers)
-                      60 LOAD_NAME               11 (Dict)
-                      62 LOAD_NAME                9 (str)
-                      64 LOAD_NAME                9 (str)
-                      66 BUILD_TUPLE              2
-                      68 BINARY_SUBSCR
-                      78 LOAD_NAME                5 (__annotations__)
-                      80 LOAD_CONST               6 ('headers')
-                      82 STORE_SUBSCR
+          53          68 BUILD_MAP                0
+                      70 STORE_NAME              11 (headers)
+                      72 LOAD_NAME               12 (Dict)
+                      74 LOAD_NAME               10 (str)
+                      76 LOAD_NAME               10 (str)
+                      78 BUILD_TUPLE              2
+                      80 BINARY_SUBSCR
+                      90 LOAD_NAME                5 (__annotations__)
+                      92 LOAD_CONST               6 ('headers')
+                      94 STORE_SUBSCR
          
-          56          86 NOP
+          54          98 LOAD_NAME               13 (Resource)
+                     100 LOAD_NAME                5 (__annotations__)
+                     102 LOAD_CONST               7 ('_TracerWrapper__resource')
+                     104 STORE_SUBSCR
          
-          57          88 NOP
+          55         108 LOAD_NAME               14 (TracerProvider)
+                     110 LOAD_NAME                5 (__annotations__)
+                     112 LOAD_CONST               8 ('_TracerWrapper__tracer_provider')
+                     114 STORE_SUBSCR
          
-          58          90 NOP
+          56         118 LOAD_NAME               15 (SpanProcessor)
+                     120 LOAD_NAME                5 (__annotations__)
+                     122 LOAD_CONST               9 ('_TracerWrapper__spans_processor')
+                     124 STORE_SUBSCR
          
-          59          92 NOP
+          57         128 LOAD_CONST               4 (None)
+                     130 STORE_NAME              16 (_TracerWrapper__spans_processor_original_on_start)
+                     132 LOAD_NAME                9 (Optional)
+                     134 LOAD_NAME               17 (Callable)
+                     136 BINARY_SUBSCR
+                     146 LOAD_NAME                5 (__annotations__)
+                     148 LOAD_CONST              10 ('_TracerWrapper__spans_processor_original_on_start')
+                     150 STORE_SUBSCR
          
-          60          94 NOP
+          58         154 LOAD_NAME               18 (SpanExporter)
+                     156 LOAD_NAME                5 (__annotations__)
+                     158 LOAD_CONST              11 ('_TracerWrapper__spans_exporter')
+                     160 STORE_SUBSCR
          
-          54          96 LOAD_CONST              20 ((False, None, None, None, None))
-                      98 LOAD_CONST               8 ('processor')
+          59         164 LOAD_NAME               19 (ContentAllowList)
+                     166 LOAD_NAME                5 (__annotations__)
+                     168 LOAD_CONST              12 ('_TracerWrapper__content_allow_list')
+                     170 STORE_SUBSCR
          
-          57         100 LOAD_NAME               12 (SpanProcessor)
+          63         174 NOP
          
-          54         102 LOAD_CONST               9 ('propagator')
+          64         176 NOP
          
-          58         104 LOAD_NAME               13 (TextMapPropagator)
+          65         178 NOP
          
-          54         106 LOAD_CONST              10 ('exporter')
+          66         180 NOP
          
-          59         108 LOAD_NAME               14 (SpanExporter)
+          67         182 NOP
          
-          54         110 LOAD_CONST              11 ('instruments')
+          61         184 LOAD_CONST              26 ((False, None, None, None, None))
+                     186 LOAD_CONST              14 ('processor')
          
-          60         112 LOAD_NAME               15 (Optional)
-                     114 LOAD_NAME               16 (Set)
-                     116 LOAD_NAME               17 (Instruments)
-                     118 BINARY_SUBSCR
-                     128 BINARY_SUBSCR
+          64         188 LOAD_NAME                9 (Optional)
+                     190 LOAD_NAME               15 (SpanProcessor)
+                     192 BINARY_SUBSCR
          
-          54         138 LOAD_CONST              12 ('return')
+          61         202 LOAD_CONST              15 ('propagator')
          
-          61         140 LOAD_CONST               0 ('TracerWrapper')
+          65         204 LOAD_NAME                9 (Optional)
+                     206 LOAD_NAME               20 (TextMapPropagator)
+                     208 BINARY_SUBSCR
          
-          54         142 BUILD_TUPLE             10
-                     144 LOAD_CLOSURE             0 (__class__)
-                     146 BUILD_TUPLE              1
-                     148 LOAD_CONST              13 (<code object __new__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 54>)
-                     150 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                     152 STORE_NAME              18 (__new__)
+          61         218 LOAD_CONST              16 ('exporter')
          
-         266         154 LOAD_CONST              14 (<code object exit_handler, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 266>)
-                     156 MAKE_FUNCTION            0
-                     158 STORE_NAME              19 (exit_handler)
+          66         220 LOAD_NAME                9 (Optional)
+                     222 LOAD_NAME               18 (SpanExporter)
+                     224 BINARY_SUBSCR
          
-         269         160 LOAD_CONST              15 (<code object _span_processor_on_start, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 269>)
-                     162 MAKE_FUNCTION            0
-                     164 STORE_NAME              20 (_span_processor_on_start)
+          61         234 LOAD_CONST              17 ('instruments')
          
-         319         166 LOAD_NAME               21 (staticmethod)
+          67         236 LOAD_NAME                9 (Optional)
+                     238 LOAD_NAME               21 (Set)
+                     240 LOAD_NAME               22 (Instruments)
+                     242 BINARY_SUBSCR
+                     252 BINARY_SUBSCR
          
-         320         168 LOAD_CONST               1 ('resource_attributes')
+          61         262 LOAD_CONST              18 ('return')
          
-         321         170 LOAD_NAME                4 (dict)
+          68         264 LOAD_CONST               0 ('TracerWrapper')
          
-         320         172 LOAD_CONST               3 ('enable_content_tracing')
+          61         266 BUILD_TUPLE             10
+                     268 LOAD_CLOSURE             0 (__class__)
+                     270 BUILD_TUPLE              1
+                     272 LOAD_CONST              19 (<code object __new__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 61>)
+                     274 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                     276 STORE_NAME              23 (__new__)
          
-         322         174 LOAD_NAME                7 (bool)
+         273         278 LOAD_CONST              20 (<code object exit_handler, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 273>)
+                     280 MAKE_FUNCTION            0
+                     282 STORE_NAME              24 (exit_handler)
          
-         320         176 LOAD_CONST               5 ('endpoint')
+         276         284 LOAD_CONST              21 (<code object _span_processor_on_start, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 276>)
+                     286 MAKE_FUNCTION            0
+                     288 STORE_NAME              25 (_span_processor_on_start)
          
-         323         178 LOAD_NAME                9 (str)
+         298         290 LOAD_NAME               26 (staticmethod)
          
-         320         180 LOAD_CONST               6 ('headers')
+         299         292 LOAD_CONST               1 ('resource_attributes')
          
-         324         182 LOAD_NAME               11 (Dict)
-                     184 LOAD_NAME                9 (str)
-                     186 LOAD_NAME                9 (str)
-                     188 BUILD_TUPLE              2
-                     190 BINARY_SUBSCR
+         300         294 LOAD_NAME                4 (dict)
          
-         320         200 LOAD_CONST              12 ('return')
+         299         296 LOAD_CONST               3 ('enable_content_tracing')
          
-         325         202 LOAD_CONST               4 (None)
+         301         298 LOAD_NAME                7 (bool)
          
-         320         204 BUILD_TUPLE             10
-                     206 LOAD_CONST              16 (<code object set_static_params, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 319>)
-                     208 MAKE_FUNCTION            4 (annotations)
+         299         300 LOAD_CONST               5 ('endpoint')
          
-         319         210 PRECALL                  0
-                     214 CALL                     0
+         302         302 LOAD_NAME               10 (str)
          
-         320         224 STORE_NAME              22 (set_static_params)
+         299         304 LOAD_CONST               6 ('headers')
          
-         331         226 LOAD_NAME               23 (classmethod)
+         303         306 LOAD_NAME               12 (Dict)
+                     308 LOAD_NAME               10 (str)
+                     310 LOAD_NAME               10 (str)
+                     312 BUILD_TUPLE              2
+                     314 BINARY_SUBSCR
          
-         332         228 LOAD_CONST              12 ('return')
-                     230 LOAD_NAME                7 (bool)
-                     232 BUILD_TUPLE              2
-                     234 LOAD_CONST              17 (<code object verify_initialized, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 331>)
-                     236 MAKE_FUNCTION            4 (annotations)
+         299         324 LOAD_CONST              18 ('return')
          
-         331         238 PRECALL                  0
-                     242 CALL                     0
+         304         326 LOAD_CONST               4 (None)
+         
+         299         328 BUILD_TUPLE             10
+                     330 LOAD_CONST              22 (<code object set_static_params, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 298>)
+                     332 MAKE_FUNCTION            4 (annotations)
+         
+         298         334 PRECALL                  0
+                     338 CALL                     0
+         
+         299         348 STORE_NAME              27 (set_static_params)
+         
+         310         350 LOAD_NAME               28 (classmethod)
          
-         332         252 STORE_NAME              24 (verify_initialized)
+         311         352 LOAD_CONST              18 ('return')
+                     354 LOAD_NAME                7 (bool)
+                     356 BUILD_TUPLE              2
+                     358 LOAD_CONST              23 (<code object verify_initialized, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 310>)
+                     360 MAKE_FUNCTION            4 (annotations)
          
-         346         254 LOAD_CONST              18 (<code object flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 346>)
-                     256 MAKE_FUNCTION            0
-                     258 STORE_NAME              25 (flush)
-         
-         349         260 LOAD_CONST              19 (<code object get_tracer, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 349>)
-                     262 MAKE_FUNCTION            0
-                     264 STORE_NAME              26 (get_tracer)
-                     266 LOAD_CLOSURE             0 (__class__)
-                     268 COPY                     1
-                     270 STORE_NAME              27 (__classcell__)
-                     272 RETURN_VALUE
+         310         362 PRECALL                  0
+                     366 CALL                     0
+         
+         311         376 STORE_NAME              29 (verify_initialized)
+         
+         325         378 LOAD_CONST              24 (<code object flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 325>)
+                     380 MAKE_FUNCTION            0
+                     382 STORE_NAME              30 (flush)
+         
+         328         384 LOAD_CONST              25 (<code object get_tracer, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py", line 328>)
+                     386 MAKE_FUNCTION            0
+                     388 STORE_NAME              31 (get_tracer)
+                     390 LOAD_CLOSURE             0 (__class__)
+                     392 COPY                     1
+                     394 STORE_NAME              32 (__classcell__)
+                     396 RETURN_VALUE
          consts
             'TracerWrapper'
             'resource_attributes'
             True
             'enable_content_tracing'
             None
             'endpoint'
             'headers'
+            '_TracerWrapper__resource'
+            '_TracerWrapper__tracer_provider'
+            '_TracerWrapper__spans_processor'
+            '_TracerWrapper__spans_processor_original_on_start'
+            '_TracerWrapper__spans_exporter'
+            '_TracerWrapper__content_allow_list'
             False
             'processor'
             'propagator'
             'exporter'
             'instruments'
             'return'
             code
@@ -702,870 +708,870 @@
                   200000000000000000a6010000ab0100000000000000000100747f000000
                   00000000000000a6000000ab0000000000000000007c065f400000000000
                   0000007483000000000000000000006a4200000000000000007c066a4300
                   00000000000000a6010000ab01000000000000000001007c006a04000000
                   00000000005300
                              0 COPY_FREE_VARS           1
                
-                54           2 RESUME                   0
+                61           2 RESUME                   0
                
-                62           4 LOAD_GLOBAL              1 (NULL + hasattr)
+                69           4 LOAD_GLOBAL              1 (NULL + hasattr)
                             16 LOAD_FAST                0 (cls)
                             18 LOAD_CONST               1 ('instance')
                             20 PRECALL                  2
                             24 CALL                     2
                             34 EXTENDED_ARG             8
                             36 POP_JUMP_FORWARD_IF_TRUE  2077 (to 4192)
                
-                63          38 LOAD_GLOBAL              3 (NULL + super)
+                70          38 LOAD_GLOBAL              3 (NULL + super)
                             50 LOAD_GLOBAL              4 (TracerWrapper)
                             62 LOAD_FAST                0 (cls)
                             64 PRECALL                  2
                             68 CALL                     2
                             78 LOAD_METHOD              3 (__new__)
                            100 LOAD_FAST                0 (cls)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 COPY                     1
                            118 STORE_FAST               6 (obj)
                            120 LOAD_FAST                0 (cls)
                            122 STORE_ATTR               4 (instance)
                
-                64         132 LOAD_GLOBAL              4 (TracerWrapper)
+                71         132 LOAD_GLOBAL              4 (TracerWrapper)
                            144 LOAD_ATTR                5 (endpoint)
                            154 POP_JUMP_FORWARD_IF_TRUE     2 (to 160)
                
-                65         156 LOAD_FAST                6 (obj)
+                72         156 LOAD_FAST                6 (obj)
                            158 RETURN_VALUE
                
-                67     >>  160 LOAD_GLOBAL             13 (NULL + Resource)
+                74     >>  160 LOAD_GLOBAL             13 (NULL + Resource)
                            172 LOAD_GLOBAL              4 (TracerWrapper)
                            184 LOAD_ATTR                7 (resource_attributes)
                            194 KW_NAMES                 2
                            196 PRECALL                  1
                            200 CALL                     1
                            210 LOAD_FAST                6 (obj)
                            212 STORE_ATTR               8 (_TracerWrapper__resource)
                
-                68         222 LOAD_GLOBAL             19 (NULL + init_tracer_provider)
+                75         222 LOAD_GLOBAL             19 (NULL + init_tracer_provider)
                
-                69         234 LOAD_FAST                6 (obj)
+                76         234 LOAD_FAST                6 (obj)
                            236 LOAD_ATTR                8 (_TracerWrapper__resource)
                
-                68         246 KW_NAMES                 3
+                75         246 KW_NAMES                 3
                            248 PRECALL                  1
                            252 CALL                     1
                            262 LOAD_FAST                6 (obj)
                            264 STORE_ATTR              10 (_TracerWrapper__tracer_provider)
                
-                71         274 LOAD_FAST                2 (processor)
+                78         274 LOAD_FAST                2 (processor)
                            276 POP_JUMP_FORWARD_IF_FALSE    56 (to 390)
                
-                72         278 LOAD_GLOBAL             23 (NULL + Telemetry)
+                79         278 LOAD_GLOBAL             23 (NULL + Telemetry)
                            290 PRECALL                  0
                            294 CALL                     0
                            304 LOAD_METHOD             12 (capture)
                            326 LOAD_CONST               4 ('tracer:init')
                            328 LOAD_CONST               5 ('processor')
                            330 LOAD_CONST               6 ('custom')
                            332 BUILD_MAP                1
                            334 PRECALL                  2
                            338 CALL                     2
                            348 POP_TOP
                
-                73         350 LOAD_FAST                2 (processor)
+                80         350 LOAD_FAST                2 (processor)
                            352 LOAD_FAST                6 (obj)
                            354 STORE_ATTR              13 (_TracerWrapper__spans_processor)
                
-                74         364 LOAD_FAST                2 (processor)
+                81         364 LOAD_FAST                2 (processor)
                            366 LOAD_ATTR               14 (on_start)
                            376 LOAD_FAST                6 (obj)
                            378 STORE_ATTR              15 (_TracerWrapper__spans_processor_original_on_start)
                            388 JUMP_FORWARD           214 (to 818)
                
-                76     >>  390 LOAD_FAST                4 (exporter)
+                83     >>  390 LOAD_FAST                4 (exporter)
                            392 POP_JUMP_FORWARD_IF_FALSE    42 (to 478)
                
-                77         394 LOAD_GLOBAL             23 (NULL + Telemetry)
+                84         394 LOAD_GLOBAL             23 (NULL + Telemetry)
                            406 PRECALL                  0
                            410 CALL                     0
                            420 LOAD_METHOD             12 (capture)
                
-                78         442 LOAD_CONST               4 ('tracer:init')
+                85         442 LOAD_CONST               4 ('tracer:init')
                
-                80         444 LOAD_CONST               6 ('custom')
+                87         444 LOAD_CONST               6 ('custom')
                
-                81         446 LOAD_FAST                1 (disable_batch)
+                88         446 LOAD_FAST                1 (disable_batch)
                            448 POP_JUMP_FORWARD_IF_FALSE     2 (to 454)
                            450 LOAD_CONST               7 ('simple')
                            452 JUMP_FORWARD             1 (to 456)
                        >>  454 LOAD_CONST               8 ('batch')
                
-                79     >>  456 LOAD_CONST               9 (('exporter', 'processor'))
+                86     >>  456 LOAD_CONST               9 (('exporter', 'processor'))
                            458 BUILD_CONST_KEY_MAP      2
                
-                77         460 PRECALL                  2
+                84         460 PRECALL                  2
                            464 CALL                     2
                            474 POP_TOP
                            476 JUMP_FORWARD            51 (to 580)
                
-                85     >>  478 LOAD_GLOBAL             23 (NULL + Telemetry)
+                92     >>  478 LOAD_GLOBAL             23 (NULL + Telemetry)
                            490 PRECALL                  0
                            494 CALL                     0
                            504 LOAD_METHOD             12 (capture)
                
-                86         526 LOAD_CONST               4 ('tracer:init')
+                93         526 LOAD_CONST               4 ('tracer:init')
                
-                88         528 LOAD_GLOBAL              4 (TracerWrapper)
+                95         528 LOAD_GLOBAL              4 (TracerWrapper)
                            540 LOAD_ATTR                5 (endpoint)
                
-                89         550 LOAD_FAST                1 (disable_batch)
+                96         550 LOAD_FAST                1 (disable_batch)
                            552 POP_JUMP_FORWARD_IF_FALSE     2 (to 558)
                            554 LOAD_CONST               7 ('simple')
                            556 JUMP_FORWARD             1 (to 560)
                        >>  558 LOAD_CONST               8 ('batch')
                
-                87     >>  560 LOAD_CONST               9 (('exporter', 'processor'))
+                94     >>  560 LOAD_CONST               9 (('exporter', 'processor'))
                            562 BUILD_CONST_KEY_MAP      2
                
-                85         564 PRECALL                  2
+                92         564 PRECALL                  2
                            568 CALL                     2
                            578 POP_TOP
                
-                95     >>  580 LOAD_FAST                4 (exporter)
+               102     >>  580 LOAD_FAST                4 (exporter)
                
-                94         582 POP_JUMP_FORWARD_IF_FALSE     2 (to 588)
+               101         582 POP_JUMP_FORWARD_IF_FALSE     2 (to 588)
                            584 LOAD_FAST                4 (exporter)
                            586 JUMP_FORWARD            35 (to 658)
                
-                96     >>  588 LOAD_GLOBAL             33 (NULL + init_spans_exporter)
+               103     >>  588 LOAD_GLOBAL             33 (NULL + init_spans_exporter)
                
-                97         600 LOAD_GLOBAL              4 (TracerWrapper)
+               104         600 LOAD_GLOBAL              4 (TracerWrapper)
                            612 LOAD_ATTR                5 (endpoint)
                            622 LOAD_GLOBAL              4 (TracerWrapper)
                            634 LOAD_ATTR               17 (headers)
                
-                96         644 PRECALL                  2
+               103         644 PRECALL                  2
                            648 CALL                     2
                
-                93     >>  658 LOAD_FAST                6 (obj)
+               100     >>  658 LOAD_FAST                6 (obj)
                            660 STORE_ATTR              18 (_TracerWrapper__spans_exporter)
                
-               100         670 LOAD_FAST                1 (disable_batch)
+               107         670 LOAD_FAST                1 (disable_batch)
                            672 POP_JUMP_FORWARD_IF_TRUE    14 (to 702)
                            674 LOAD_GLOBAL             39 (NULL + is_notebook)
                            686 PRECALL                  0
                            690 CALL                     0
                            700 POP_JUMP_FORWARD_IF_FALSE    26 (to 754)
                
-               101     >>  702 LOAD_GLOBAL             41 (NULL + SimpleSpanProcessor)
+               108     >>  702 LOAD_GLOBAL             41 (NULL + SimpleSpanProcessor)
                
-               102         714 LOAD_FAST                6 (obj)
+               109         714 LOAD_FAST                6 (obj)
                            716 LOAD_ATTR               18 (_TracerWrapper__spans_exporter)
                
-               101         726 PRECALL                  1
+               108         726 PRECALL                  1
                            730 CALL                     1
                            740 LOAD_FAST                6 (obj)
                            742 STORE_ATTR              13 (_TracerWrapper__spans_processor)
                            752 JUMP_FORWARD            25 (to 804)
                
-               105     >>  754 LOAD_GLOBAL             43 (NULL + BatchSpanProcessor)
+               112     >>  754 LOAD_GLOBAL             43 (NULL + BatchSpanProcessor)
                
-               106         766 LOAD_FAST                6 (obj)
+               113         766 LOAD_FAST                6 (obj)
                            768 LOAD_ATTR               18 (_TracerWrapper__spans_exporter)
                
-               105         778 PRECALL                  1
+               112         778 PRECALL                  1
                            782 CALL                     1
                            792 LOAD_FAST                6 (obj)
                            794 STORE_ATTR              13 (_TracerWrapper__spans_processor)
                
-               108     >>  804 LOAD_CONST               0 (None)
+               115     >>  804 LOAD_CONST               0 (None)
                            806 LOAD_FAST                6 (obj)
                            808 STORE_ATTR              15 (_TracerWrapper__spans_processor_original_on_start)
                
-               110     >>  818 LOAD_FAST                6 (obj)
+               117     >>  818 LOAD_FAST                6 (obj)
                            820 LOAD_ATTR               22 (_span_processor_on_start)
                            830 LOAD_FAST                6 (obj)
                            832 LOAD_ATTR               13 (_TracerWrapper__spans_processor)
                            842 STORE_ATTR              14 (on_start)
                
-               111         852 LOAD_FAST                6 (obj)
+               118         852 LOAD_FAST                6 (obj)
                            854 LOAD_ATTR               10 (_TracerWrapper__tracer_provider)
                            864 LOAD_METHOD             23 (add_span_processor)
                            886 LOAD_FAST                6 (obj)
                            888 LOAD_ATTR               13 (_TracerWrapper__spans_processor)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               113         914 LOAD_FAST                3 (propagator)
+               120         914 LOAD_FAST                3 (propagator)
                            916 POP_JUMP_FORWARD_IF_FALSE    15 (to 948)
                
-               114         918 LOAD_GLOBAL             49 (NULL + set_global_textmap)
+               121         918 LOAD_GLOBAL             49 (NULL + set_global_textmap)
                            930 LOAD_FAST                3 (propagator)
                            932 PRECALL                  1
                            936 CALL                     1
                            946 POP_TOP
                
-               116     >>  948 LOAD_CONST              10 (False)
+               123     >>  948 LOAD_CONST              10 (False)
                            950 STORE_FAST               7 (instrument_set)
                
-               117         952 LOAD_FAST                5 (instruments)
+               124         952 LOAD_FAST                5 (instruments)
                            954 POP_JUMP_FORWARD_IF_NOT_NONE    18 (to 992)
                
-               118         956 LOAD_GLOBAL             51 (NULL + init_instrumentations)
+               125         956 LOAD_GLOBAL             51 (NULL + init_instrumentations)
                            968 PRECALL                  0
                            972 CALL                     0
                            982 POP_TOP
                
-               119         984 LOAD_CONST              11 (True)
+               126         984 LOAD_CONST              11 (True)
                            986 STORE_FAST               7 (instrument_set)
                            988 EXTENDED_ARG             5
                            990 JUMP_FORWARD          1501 (to 3994)
                
-               121     >>  992 LOAD_FAST                5 (instruments)
+               128     >>  992 LOAD_FAST                5 (instruments)
                            994 GET_ITER
                        >>  996 EXTENDED_ARG             5
                            998 FOR_ITER              1497 (to 3994)
                           1000 STORE_FAST               8 (instrument)
                
-               122        1002 LOAD_FAST                8 (instrument)
+               129        1002 LOAD_FAST                8 (instrument)
                           1004 LOAD_GLOBAL             52 (Instruments)
                           1016 LOAD_ATTR               27 (OPENAI)
                           1026 COMPARE_OP               2 (==)
                           1032 POP_JUMP_FORWARD_IF_FALSE    71 (to 1176)
                
-               123        1034 LOAD_GLOBAL             57 (NULL + init_openai_instrumentor)
+               130        1034 LOAD_GLOBAL             57 (NULL + init_openai_instrumentor)
                           1046 PRECALL                  0
                           1050 CALL                     0
                           1060 POP_JUMP_FORWARD_IF_TRUE    54 (to 1170)
                
-               124        1062 LOAD_GLOBAL             59 (NULL + print)
+               131        1062 LOAD_GLOBAL             59 (NULL + print)
                           1074 LOAD_GLOBAL             60 (Fore)
                           1086 LOAD_ATTR               31 (RED)
                           1096 LOAD_CONST              12 ('Warning: OpenAI library does not exist.')
                           1098 BINARY_OP                0 (+)
                           1102 PRECALL                  1
                           1106 CALL                     1
                           1116 POP_TOP
                
-               125        1118 LOAD_GLOBAL             59 (NULL + print)
+               132        1118 LOAD_GLOBAL             59 (NULL + print)
                           1130 LOAD_GLOBAL             60 (Fore)
                           1142 LOAD_ATTR               32 (RESET)
                           1152 PRECALL                  1
                           1156 CALL                     1
                           1166 POP_TOP
                           1168 JUMP_BACKWARD           87 (to 996)
                
-               127     >> 1170 LOAD_CONST              11 (True)
+               134     >> 1170 LOAD_CONST              11 (True)
                           1172 STORE_FAST               7 (instrument_set)
                           1174 JUMP_BACKWARD           90 (to 996)
                
-               128     >> 1176 LOAD_FAST                8 (instrument)
+               135     >> 1176 LOAD_FAST                8 (instrument)
                           1178 LOAD_GLOBAL             52 (Instruments)
                           1190 LOAD_ATTR               33 (ANTHROPIC)
                           1200 COMPARE_OP               2 (==)
                           1206 POP_JUMP_FORWARD_IF_FALSE    71 (to 1350)
                
-               129        1208 LOAD_GLOBAL             69 (NULL + init_anthropic_instrumentor)
+               136        1208 LOAD_GLOBAL             69 (NULL + init_anthropic_instrumentor)
                           1220 PRECALL                  0
                           1224 CALL                     0
                           1234 POP_JUMP_FORWARD_IF_TRUE    54 (to 1344)
                
-               130        1236 LOAD_GLOBAL             59 (NULL + print)
+               137        1236 LOAD_GLOBAL             59 (NULL + print)
                
-               131        1248 LOAD_GLOBAL             60 (Fore)
+               138        1248 LOAD_GLOBAL             60 (Fore)
                           1260 LOAD_ATTR               31 (RED)
                           1270 LOAD_CONST              13 ('Warning: Anthropic library does not exist.')
                           1272 BINARY_OP                0 (+)
                
-               130        1276 PRECALL                  1
+               137        1276 PRECALL                  1
                           1280 CALL                     1
                           1290 POP_TOP
                
-               133        1292 LOAD_GLOBAL             59 (NULL + print)
+               140        1292 LOAD_GLOBAL             59 (NULL + print)
                           1304 LOAD_GLOBAL             60 (Fore)
                           1316 LOAD_ATTR               32 (RESET)
                           1326 PRECALL                  1
                           1330 CALL                     1
                           1340 POP_TOP
                           1342 JUMP_BACKWARD          174 (to 996)
                
-               135     >> 1344 LOAD_CONST              11 (True)
+               142     >> 1344 LOAD_CONST              11 (True)
                           1346 STORE_FAST               7 (instrument_set)
                           1348 JUMP_BACKWARD          177 (to 996)
                
-               136     >> 1350 LOAD_FAST                8 (instrument)
+               143     >> 1350 LOAD_FAST                8 (instrument)
                           1352 LOAD_GLOBAL             52 (Instruments)
                           1364 LOAD_ATTR               35 (COHERE)
                           1374 COMPARE_OP               2 (==)
                           1380 POP_JUMP_FORWARD_IF_FALSE    73 (to 1528)
                
-               137        1382 LOAD_GLOBAL             73 (NULL + init_cohere_instrumentor)
+               144        1382 LOAD_GLOBAL             73 (NULL + init_cohere_instrumentor)
                           1394 PRECALL                  0
                           1398 CALL                     0
                           1408 POP_JUMP_FORWARD_IF_TRUE    55 (to 1520)
                
-               138        1410 LOAD_GLOBAL             59 (NULL + print)
+               145        1410 LOAD_GLOBAL             59 (NULL + print)
                           1422 LOAD_GLOBAL             60 (Fore)
                           1434 LOAD_ATTR               31 (RED)
                           1444 LOAD_CONST              14 ('Warning: Cohere library does not exist.')
                           1446 BINARY_OP                0 (+)
                           1450 PRECALL                  1
                           1454 CALL                     1
                           1464 POP_TOP
                
-               139        1466 LOAD_GLOBAL             59 (NULL + print)
+               146        1466 LOAD_GLOBAL             59 (NULL + print)
                           1478 LOAD_GLOBAL             60 (Fore)
                           1490 LOAD_ATTR               32 (RESET)
                           1500 PRECALL                  1
                           1504 CALL                     1
                           1514 POP_TOP
                           1516 EXTENDED_ARG             1
                           1518 JUMP_BACKWARD          262 (to 996)
                
-               141     >> 1520 LOAD_CONST              11 (True)
+               148     >> 1520 LOAD_CONST              11 (True)
                           1522 STORE_FAST               7 (instrument_set)
                           1524 EXTENDED_ARG             1
                           1526 JUMP_BACKWARD          266 (to 996)
                
-               142     >> 1528 LOAD_FAST                8 (instrument)
+               149     >> 1528 LOAD_FAST                8 (instrument)
                           1530 LOAD_GLOBAL             52 (Instruments)
                           1542 LOAD_ATTR               37 (PINECONE)
                           1552 COMPARE_OP               2 (==)
                           1558 POP_JUMP_FORWARD_IF_FALSE    73 (to 1706)
                
-               143        1560 LOAD_GLOBAL             77 (NULL + init_pinecone_instrumentor)
+               150        1560 LOAD_GLOBAL             77 (NULL + init_pinecone_instrumentor)
                           1572 PRECALL                  0
                           1576 CALL                     0
                           1586 POP_JUMP_FORWARD_IF_TRUE    55 (to 1698)
                
-               144        1588 LOAD_GLOBAL             59 (NULL + print)
+               151        1588 LOAD_GLOBAL             59 (NULL + print)
                
-               145        1600 LOAD_GLOBAL             60 (Fore)
+               152        1600 LOAD_GLOBAL             60 (Fore)
                           1612 LOAD_ATTR               31 (RED)
                           1622 LOAD_CONST              15 ('Warning: Pinecone library does not exist.')
                           1624 BINARY_OP                0 (+)
                
-               144        1628 PRECALL                  1
+               151        1628 PRECALL                  1
                           1632 CALL                     1
                           1642 POP_TOP
                
-               147        1644 LOAD_GLOBAL             59 (NULL + print)
+               154        1644 LOAD_GLOBAL             59 (NULL + print)
                           1656 LOAD_GLOBAL             60 (Fore)
                           1668 LOAD_ATTR               32 (RESET)
                           1678 PRECALL                  1
                           1682 CALL                     1
                           1692 POP_TOP
                           1694 EXTENDED_ARG             1
                           1696 JUMP_BACKWARD          351 (to 996)
                
-               149     >> 1698 LOAD_CONST              11 (True)
+               156     >> 1698 LOAD_CONST              11 (True)
                           1700 STORE_FAST               7 (instrument_set)
                           1702 EXTENDED_ARG             1
                           1704 JUMP_BACKWARD          355 (to 996)
                
-               150     >> 1706 LOAD_FAST                8 (instrument)
+               157     >> 1706 LOAD_FAST                8 (instrument)
                           1708 LOAD_GLOBAL             52 (Instruments)
                           1720 LOAD_ATTR               39 (CHROMA)
                           1730 COMPARE_OP               2 (==)
                           1736 POP_JUMP_FORWARD_IF_FALSE    73 (to 1884)
                
-               151        1738 LOAD_GLOBAL             81 (NULL + init_chroma_instrumentor)
+               158        1738 LOAD_GLOBAL             81 (NULL + init_chroma_instrumentor)
                           1750 PRECALL                  0
                           1754 CALL                     0
                           1764 POP_JUMP_FORWARD_IF_TRUE    55 (to 1876)
                
-               152        1766 LOAD_GLOBAL             59 (NULL + print)
+               159        1766 LOAD_GLOBAL             59 (NULL + print)
                           1778 LOAD_GLOBAL             60 (Fore)
                           1790 LOAD_ATTR               31 (RED)
                           1800 LOAD_CONST              16 ('Warning: Chroma library does not exist.')
                           1802 BINARY_OP                0 (+)
                           1806 PRECALL                  1
                           1810 CALL                     1
                           1820 POP_TOP
                
-               153        1822 LOAD_GLOBAL             59 (NULL + print)
+               160        1822 LOAD_GLOBAL             59 (NULL + print)
                           1834 LOAD_GLOBAL             60 (Fore)
                           1846 LOAD_ATTR               32 (RESET)
                           1856 PRECALL                  1
                           1860 CALL                     1
                           1870 POP_TOP
                           1872 EXTENDED_ARG             1
                           1874 JUMP_BACKWARD          440 (to 996)
                
-               155     >> 1876 LOAD_CONST              11 (True)
+               162     >> 1876 LOAD_CONST              11 (True)
                           1878 STORE_FAST               7 (instrument_set)
                           1880 EXTENDED_ARG             1
                           1882 JUMP_BACKWARD          444 (to 996)
                
-               156     >> 1884 LOAD_FAST                8 (instrument)
+               163     >> 1884 LOAD_FAST                8 (instrument)
                           1886 LOAD_GLOBAL             52 (Instruments)
                           1898 LOAD_ATTR               41 (LANGCHAIN)
                           1908 COMPARE_OP               2 (==)
                           1914 POP_JUMP_FORWARD_IF_FALSE    73 (to 2062)
                
-               157        1916 LOAD_GLOBAL             85 (NULL + init_langchain_instrumentor)
+               164        1916 LOAD_GLOBAL             85 (NULL + init_langchain_instrumentor)
                           1928 PRECALL                  0
                           1932 CALL                     0
                           1942 POP_JUMP_FORWARD_IF_TRUE    55 (to 2054)
                
-               158        1944 LOAD_GLOBAL             59 (NULL + print)
+               165        1944 LOAD_GLOBAL             59 (NULL + print)
                
-               159        1956 LOAD_GLOBAL             60 (Fore)
+               166        1956 LOAD_GLOBAL             60 (Fore)
                           1968 LOAD_ATTR               31 (RED)
                           1978 LOAD_CONST              17 ('Warning: LangChain library does not exist.')
                           1980 BINARY_OP                0 (+)
                
-               158        1984 PRECALL                  1
+               165        1984 PRECALL                  1
                           1988 CALL                     1
                           1998 POP_TOP
                
-               161        2000 LOAD_GLOBAL             59 (NULL + print)
+               168        2000 LOAD_GLOBAL             59 (NULL + print)
                           2012 LOAD_GLOBAL             60 (Fore)
                           2024 LOAD_ATTR               32 (RESET)
                           2034 PRECALL                  1
                           2038 CALL                     1
                           2048 POP_TOP
                           2050 EXTENDED_ARG             2
                           2052 JUMP_BACKWARD          529 (to 996)
                
-               163     >> 2054 LOAD_CONST              11 (True)
+               170     >> 2054 LOAD_CONST              11 (True)
                           2056 STORE_FAST               7 (instrument_set)
                           2058 EXTENDED_ARG             2
                           2060 JUMP_BACKWARD          533 (to 996)
                
-               164     >> 2062 LOAD_FAST                8 (instrument)
+               171     >> 2062 LOAD_FAST                8 (instrument)
                           2064 LOAD_GLOBAL             52 (Instruments)
                           2076 LOAD_ATTR               43 (LLAMA_INDEX)
                           2086 COMPARE_OP               2 (==)
                           2092 POP_JUMP_FORWARD_IF_FALSE    73 (to 2240)
                
-               165        2094 LOAD_GLOBAL             89 (NULL + init_llama_index_instrumentor)
+               172        2094 LOAD_GLOBAL             89 (NULL + init_llama_index_instrumentor)
                           2106 PRECALL                  0
                           2110 CALL                     0
                           2120 POP_JUMP_FORWARD_IF_TRUE    55 (to 2232)
                
-               166        2122 LOAD_GLOBAL             59 (NULL + print)
+               173        2122 LOAD_GLOBAL             59 (NULL + print)
                
-               167        2134 LOAD_GLOBAL             60 (Fore)
+               174        2134 LOAD_GLOBAL             60 (Fore)
                           2146 LOAD_ATTR               31 (RED)
                           2156 LOAD_CONST              18 ('Warning: LlamaIndex library does not exist.')
                           2158 BINARY_OP                0 (+)
                
-               166        2162 PRECALL                  1
+               173        2162 PRECALL                  1
                           2166 CALL                     1
                           2176 POP_TOP
                
-               169        2178 LOAD_GLOBAL             59 (NULL + print)
+               176        2178 LOAD_GLOBAL             59 (NULL + print)
                           2190 LOAD_GLOBAL             60 (Fore)
                           2202 LOAD_ATTR               32 (RESET)
                           2212 PRECALL                  1
                           2216 CALL                     1
                           2226 POP_TOP
                           2228 EXTENDED_ARG             2
                           2230 JUMP_BACKWARD          618 (to 996)
                
-               171     >> 2232 LOAD_CONST              11 (True)
+               178     >> 2232 LOAD_CONST              11 (True)
                           2234 STORE_FAST               7 (instrument_set)
                           2236 EXTENDED_ARG             2
                           2238 JUMP_BACKWARD          622 (to 996)
                
-               172     >> 2240 LOAD_FAST                8 (instrument)
+               179     >> 2240 LOAD_FAST                8 (instrument)
                           2242 LOAD_GLOBAL             52 (Instruments)
                           2254 LOAD_ATTR               45 (TRANSFORMERS)
                           2264 COMPARE_OP               2 (==)
                           2270 POP_JUMP_FORWARD_IF_FALSE    73 (to 2418)
                
-               173        2272 LOAD_GLOBAL             93 (NULL + init_transformers_instrumentor)
+               180        2272 LOAD_GLOBAL             93 (NULL + init_transformers_instrumentor)
                           2284 PRECALL                  0
                           2288 CALL                     0
                           2298 POP_JUMP_FORWARD_IF_TRUE    55 (to 2410)
                
-               174        2300 LOAD_GLOBAL             59 (NULL + print)
+               181        2300 LOAD_GLOBAL             59 (NULL + print)
                
-               175        2312 LOAD_GLOBAL             60 (Fore)
+               182        2312 LOAD_GLOBAL             60 (Fore)
                           2324 LOAD_ATTR               31 (RED)
                
-               176        2334 LOAD_CONST              19 ('Warning: Transformers library does not exist.')
+               183        2334 LOAD_CONST              19 ('Warning: Transformers library does not exist.')
                
-               175        2336 BINARY_OP                0 (+)
+               182        2336 BINARY_OP                0 (+)
                
-               174        2340 PRECALL                  1
+               181        2340 PRECALL                  1
                           2344 CALL                     1
                           2354 POP_TOP
                
-               178        2356 LOAD_GLOBAL             59 (NULL + print)
+               185        2356 LOAD_GLOBAL             59 (NULL + print)
                           2368 LOAD_GLOBAL             60 (Fore)
                           2380 LOAD_ATTR               32 (RESET)
                           2390 PRECALL                  1
                           2394 CALL                     1
                           2404 POP_TOP
                           2406 EXTENDED_ARG             2
                           2408 JUMP_BACKWARD          707 (to 996)
                
-               180     >> 2410 LOAD_CONST              11 (True)
+               187     >> 2410 LOAD_CONST              11 (True)
                           2412 STORE_FAST               7 (instrument_set)
                           2414 EXTENDED_ARG             2
                           2416 JUMP_BACKWARD          711 (to 996)
                
-               181     >> 2418 LOAD_FAST                8 (instrument)
+               188     >> 2418 LOAD_FAST                8 (instrument)
                           2420 LOAD_GLOBAL             52 (Instruments)
                           2432 LOAD_ATTR               47 (REQUESTS)
                           2442 COMPARE_OP               2 (==)
                           2448 POP_JUMP_FORWARD_IF_FALSE    73 (to 2596)
                
-               182        2450 LOAD_GLOBAL             97 (NULL + init_requests_instrumentor)
+               189        2450 LOAD_GLOBAL             97 (NULL + init_requests_instrumentor)
                           2462 PRECALL                  0
                           2466 CALL                     0
                           2476 POP_JUMP_FORWARD_IF_TRUE    55 (to 2588)
                
-               183        2478 LOAD_GLOBAL             59 (NULL + print)
+               190        2478 LOAD_GLOBAL             59 (NULL + print)
                
-               184        2490 LOAD_GLOBAL             60 (Fore)
+               191        2490 LOAD_GLOBAL             60 (Fore)
                           2502 LOAD_ATTR               31 (RED)
                           2512 LOAD_CONST              20 ('Warning: Requests library does not exist.')
                           2514 BINARY_OP                0 (+)
                
-               183        2518 PRECALL                  1
+               190        2518 PRECALL                  1
                           2522 CALL                     1
                           2532 POP_TOP
                
-               186        2534 LOAD_GLOBAL             59 (NULL + print)
+               193        2534 LOAD_GLOBAL             59 (NULL + print)
                           2546 LOAD_GLOBAL             60 (Fore)
                           2558 LOAD_ATTR               32 (RESET)
                           2568 PRECALL                  1
                           2572 CALL                     1
                           2582 POP_TOP
                           2584 EXTENDED_ARG             3
                           2586 JUMP_BACKWARD          796 (to 996)
                
-               188     >> 2588 LOAD_CONST              11 (True)
+               195     >> 2588 LOAD_CONST              11 (True)
                           2590 STORE_FAST               7 (instrument_set)
                           2592 EXTENDED_ARG             3
                           2594 JUMP_BACKWARD          800 (to 996)
                
-               189     >> 2596 LOAD_FAST                8 (instrument)
+               196     >> 2596 LOAD_FAST                8 (instrument)
                           2598 LOAD_GLOBAL             52 (Instruments)
                           2610 LOAD_ATTR               49 (URLLIB3)
                           2620 COMPARE_OP               2 (==)
                           2626 POP_JUMP_FORWARD_IF_FALSE    73 (to 2774)
                
-               190        2628 LOAD_GLOBAL            101 (NULL + init_urllib3_instrumentor)
+               197        2628 LOAD_GLOBAL            101 (NULL + init_urllib3_instrumentor)
                           2640 PRECALL                  0
                           2644 CALL                     0
                           2654 POP_JUMP_FORWARD_IF_TRUE    55 (to 2766)
                
-               191        2656 LOAD_GLOBAL             59 (NULL + print)
+               198        2656 LOAD_GLOBAL             59 (NULL + print)
                           2668 LOAD_GLOBAL             60 (Fore)
                           2680 LOAD_ATTR               31 (RED)
                           2690 LOAD_CONST              21 ('Warning: urllib3 library does not exist.')
                           2692 BINARY_OP                0 (+)
                           2696 PRECALL                  1
                           2700 CALL                     1
                           2710 POP_TOP
                
-               192        2712 LOAD_GLOBAL             59 (NULL + print)
+               199        2712 LOAD_GLOBAL             59 (NULL + print)
                           2724 LOAD_GLOBAL             60 (Fore)
                           2736 LOAD_ATTR               32 (RESET)
                           2746 PRECALL                  1
                           2750 CALL                     1
                           2760 POP_TOP
                           2762 EXTENDED_ARG             3
                           2764 JUMP_BACKWARD          885 (to 996)
                
-               194     >> 2766 LOAD_CONST              11 (True)
+               201     >> 2766 LOAD_CONST              11 (True)
                           2768 STORE_FAST               7 (instrument_set)
                           2770 EXTENDED_ARG             3
                           2772 JUMP_BACKWARD          889 (to 996)
                
-               195     >> 2774 LOAD_FAST                8 (instrument)
+               202     >> 2774 LOAD_FAST                8 (instrument)
                           2776 LOAD_GLOBAL             52 (Instruments)
                           2788 LOAD_ATTR               51 (PYMYSQL)
                           2798 COMPARE_OP               2 (==)
                           2804 POP_JUMP_FORWARD_IF_FALSE    73 (to 2952)
                
-               196        2806 LOAD_GLOBAL            105 (NULL + init_pymysql_instrumentor)
+               203        2806 LOAD_GLOBAL            105 (NULL + init_pymysql_instrumentor)
                           2818 PRECALL                  0
                           2822 CALL                     0
                           2832 POP_JUMP_FORWARD_IF_TRUE    55 (to 2944)
                
-               197        2834 LOAD_GLOBAL             59 (NULL + print)
+               204        2834 LOAD_GLOBAL             59 (NULL + print)
                           2846 LOAD_GLOBAL             60 (Fore)
                           2858 LOAD_ATTR               31 (RED)
                           2868 LOAD_CONST              22 ('Warning: PyMySQL library does not exist.')
                           2870 BINARY_OP                0 (+)
                           2874 PRECALL                  1
                           2878 CALL                     1
                           2888 POP_TOP
                
-               198        2890 LOAD_GLOBAL             59 (NULL + print)
+               205        2890 LOAD_GLOBAL             59 (NULL + print)
                           2902 LOAD_GLOBAL             60 (Fore)
                           2914 LOAD_ATTR               32 (RESET)
                           2924 PRECALL                  1
                           2928 CALL                     1
                           2938 POP_TOP
                           2940 EXTENDED_ARG             3
                           2942 JUMP_BACKWARD          974 (to 996)
                
-               200     >> 2944 LOAD_CONST              11 (True)
+               207     >> 2944 LOAD_CONST              11 (True)
                           2946 STORE_FAST               7 (instrument_set)
                           2948 EXTENDED_ARG             3
                           2950 JUMP_BACKWARD          978 (to 996)
                
-               201     >> 2952 LOAD_FAST                8 (instrument)
+               208     >> 2952 LOAD_FAST                8 (instrument)
                           2954 LOAD_GLOBAL             52 (Instruments)
                           2966 LOAD_ATTR               53 (BEDROCK)
                           2976 COMPARE_OP               2 (==)
                           2982 POP_JUMP_FORWARD_IF_FALSE    73 (to 3130)
                
-               202        2984 LOAD_GLOBAL            109 (NULL + init_bedrock_instrumentor)
+               209        2984 LOAD_GLOBAL            109 (NULL + init_bedrock_instrumentor)
                           2996 PRECALL                  0
                           3000 CALL                     0
                           3010 POP_JUMP_FORWARD_IF_TRUE    55 (to 3122)
                
-               203        3012 LOAD_GLOBAL             59 (NULL + print)
+               210        3012 LOAD_GLOBAL             59 (NULL + print)
                           3024 LOAD_GLOBAL             60 (Fore)
                           3036 LOAD_ATTR               31 (RED)
                           3046 LOAD_CONST              23 ('Warning: Bedrock library does not exist.')
                           3048 BINARY_OP                0 (+)
                           3052 PRECALL                  1
                           3056 CALL                     1
                           3066 POP_TOP
                
-               204        3068 LOAD_GLOBAL             59 (NULL + print)
+               211        3068 LOAD_GLOBAL             59 (NULL + print)
                           3080 LOAD_GLOBAL             60 (Fore)
                           3092 LOAD_ATTR               32 (RESET)
                           3102 PRECALL                  1
                           3106 CALL                     1
                           3116 POP_TOP
                           3118 EXTENDED_ARG             4
                           3120 JUMP_BACKWARD         1063 (to 996)
                
-               206     >> 3122 LOAD_CONST              11 (True)
+               213     >> 3122 LOAD_CONST              11 (True)
                           3124 STORE_FAST               7 (instrument_set)
                           3126 EXTENDED_ARG             4
                           3128 JUMP_BACKWARD         1067 (to 996)
                
-               207     >> 3130 LOAD_FAST                8 (instrument)
+               214     >> 3130 LOAD_FAST                8 (instrument)
                           3132 LOAD_GLOBAL             52 (Instruments)
                           3144 LOAD_ATTR               55 (REPLICATE)
                           3154 COMPARE_OP               2 (==)
                           3160 POP_JUMP_FORWARD_IF_FALSE    73 (to 3308)
                
-               208        3162 LOAD_GLOBAL            113 (NULL + init_replicate_instrumentor)
+               215        3162 LOAD_GLOBAL            113 (NULL + init_replicate_instrumentor)
                           3174 PRECALL                  0
                           3178 CALL                     0
                           3188 POP_JUMP_FORWARD_IF_TRUE    55 (to 3300)
                
-               209        3190 LOAD_GLOBAL             59 (NULL + print)
+               216        3190 LOAD_GLOBAL             59 (NULL + print)
                
-               210        3202 LOAD_GLOBAL             60 (Fore)
+               217        3202 LOAD_GLOBAL             60 (Fore)
                           3214 LOAD_ATTR               31 (RED)
                           3224 LOAD_CONST              24 ('Warning: Replicate library does not exist.')
                           3226 BINARY_OP                0 (+)
                
-               209        3230 PRECALL                  1
+               216        3230 PRECALL                  1
                           3234 CALL                     1
                           3244 POP_TOP
                
-               212        3246 LOAD_GLOBAL             59 (NULL + print)
+               219        3246 LOAD_GLOBAL             59 (NULL + print)
                           3258 LOAD_GLOBAL             60 (Fore)
                           3270 LOAD_ATTR               32 (RESET)
                           3280 PRECALL                  1
                           3284 CALL                     1
                           3294 POP_TOP
                           3296 EXTENDED_ARG             4
                           3298 JUMP_BACKWARD         1152 (to 996)
                
-               214     >> 3300 LOAD_CONST              11 (True)
+               221     >> 3300 LOAD_CONST              11 (True)
                           3302 STORE_FAST               7 (instrument_set)
                           3304 EXTENDED_ARG             4
                           3306 JUMP_BACKWARD         1156 (to 996)
                
-               215     >> 3308 LOAD_FAST                8 (instrument)
+               222     >> 3308 LOAD_FAST                8 (instrument)
                           3310 LOAD_GLOBAL             52 (Instruments)
                           3322 LOAD_ATTR               57 (VERTEXAI)
                           3332 COMPARE_OP               2 (==)
                           3338 POP_JUMP_FORWARD_IF_FALSE    73 (to 3486)
                
-               216        3340 LOAD_GLOBAL            117 (NULL + init_vertexai_instrumentor)
+               223        3340 LOAD_GLOBAL            117 (NULL + init_vertexai_instrumentor)
                           3352 PRECALL                  0
                           3356 CALL                     0
                           3366 POP_JUMP_FORWARD_IF_TRUE    55 (to 3478)
                
-               217        3368 LOAD_GLOBAL             59 (NULL + print)
+               224        3368 LOAD_GLOBAL             59 (NULL + print)
                
-               218        3380 LOAD_GLOBAL             60 (Fore)
+               225        3380 LOAD_GLOBAL             60 (Fore)
                           3392 LOAD_ATTR               31 (RED)
                           3402 LOAD_CONST              25 ('Warning: Vertex AI library does not exist.')
                           3404 BINARY_OP                0 (+)
                
-               217        3408 PRECALL                  1
+               224        3408 PRECALL                  1
                           3412 CALL                     1
                           3422 POP_TOP
                
-               220        3424 LOAD_GLOBAL             59 (NULL + print)
+               227        3424 LOAD_GLOBAL             59 (NULL + print)
                           3436 LOAD_GLOBAL             60 (Fore)
                           3448 LOAD_ATTR               32 (RESET)
                           3458 PRECALL                  1
                           3462 CALL                     1
                           3472 POP_TOP
                           3474 EXTENDED_ARG             4
                           3476 JUMP_BACKWARD         1241 (to 996)
                
-               222     >> 3478 LOAD_CONST              11 (True)
+               229     >> 3478 LOAD_CONST              11 (True)
                           3480 STORE_FAST               7 (instrument_set)
                           3482 EXTENDED_ARG             4
                           3484 JUMP_BACKWARD         1245 (to 996)
                
-               223     >> 3486 LOAD_FAST                8 (instrument)
+               230     >> 3486 LOAD_FAST                8 (instrument)
                           3488 LOAD_GLOBAL             52 (Instruments)
                           3500 LOAD_ATTR               59 (WATSONX)
                           3510 COMPARE_OP               2 (==)
                           3516 POP_JUMP_FORWARD_IF_FALSE    73 (to 3664)
                
-               224        3518 LOAD_GLOBAL            121 (NULL + init_watsonx_instrumentor)
+               231        3518 LOAD_GLOBAL            121 (NULL + init_watsonx_instrumentor)
                           3530 PRECALL                  0
                           3534 CALL                     0
                           3544 POP_JUMP_FORWARD_IF_TRUE    55 (to 3656)
                
-               225        3546 LOAD_GLOBAL             59 (NULL + print)
+               232        3546 LOAD_GLOBAL             59 (NULL + print)
                           3558 LOAD_GLOBAL             60 (Fore)
                           3570 LOAD_ATTR               31 (RED)
                           3580 LOAD_CONST              26 ('Warning: Watsonx library does not exist.')
                           3582 BINARY_OP                0 (+)
                           3586 PRECALL                  1
                           3590 CALL                     1
                           3600 POP_TOP
                
-               226        3602 LOAD_GLOBAL             59 (NULL + print)
+               233        3602 LOAD_GLOBAL             59 (NULL + print)
                           3614 LOAD_GLOBAL             60 (Fore)
                           3626 LOAD_ATTR               32 (RESET)
                           3636 PRECALL                  1
                           3640 CALL                     1
                           3650 POP_TOP
                           3652 EXTENDED_ARG             5
                           3654 JUMP_BACKWARD         1330 (to 996)
                
-               228     >> 3656 LOAD_CONST              11 (True)
+               235     >> 3656 LOAD_CONST              11 (True)
                           3658 STORE_FAST               7 (instrument_set)
                           3660 EXTENDED_ARG             5
                           3662 JUMP_BACKWARD         1334 (to 996)
                
-               229     >> 3664 LOAD_FAST                8 (instrument)
+               236     >> 3664 LOAD_FAST                8 (instrument)
                           3666 LOAD_GLOBAL             52 (Instruments)
                           3678 LOAD_ATTR               61 (WEAVIATE)
                           3688 COMPARE_OP               2 (==)
                           3694 POP_JUMP_FORWARD_IF_FALSE    73 (to 3842)
                
-               230        3696 LOAD_GLOBAL            125 (NULL + init_weaviate_instrumentor)
+               237        3696 LOAD_GLOBAL            125 (NULL + init_weaviate_instrumentor)
                           3708 PRECALL                  0
                           3712 CALL                     0
                           3722 POP_JUMP_FORWARD_IF_TRUE    55 (to 3834)
                
-               231        3724 LOAD_GLOBAL             59 (NULL + print)
+               238        3724 LOAD_GLOBAL             59 (NULL + print)
                
-               232        3736 LOAD_GLOBAL             60 (Fore)
+               239        3736 LOAD_GLOBAL             60 (Fore)
                           3748 LOAD_ATTR               31 (RED)
                           3758 LOAD_CONST              27 ('Warning: Weaviate library does not exist.')
                           3760 BINARY_OP                0 (+)
                
-               231        3764 PRECALL                  1
+               238        3764 PRECALL                  1
                           3768 CALL                     1
                           3778 POP_TOP
                
-               234        3780 LOAD_GLOBAL             59 (NULL + print)
+               241        3780 LOAD_GLOBAL             59 (NULL + print)
                           3792 LOAD_GLOBAL             60 (Fore)
                           3804 LOAD_ATTR               32 (RESET)
                           3814 PRECALL                  1
                           3818 CALL                     1
                           3828 POP_TOP
                           3830 EXTENDED_ARG             5
                           3832 JUMP_BACKWARD         1419 (to 996)
                
-               236     >> 3834 LOAD_CONST              11 (True)
+               243     >> 3834 LOAD_CONST              11 (True)
                           3836 STORE_FAST               7 (instrument_set)
                           3838 EXTENDED_ARG             5
                           3840 JUMP_BACKWARD         1423 (to 996)
                
-               239     >> 3842 LOAD_GLOBAL             59 (NULL + print)
+               246     >> 3842 LOAD_GLOBAL             59 (NULL + print)
                
-               240        3854 LOAD_GLOBAL             60 (Fore)
+               247        3854 LOAD_GLOBAL             60 (Fore)
                           3866 LOAD_ATTR               31 (RED)
                
-               241        3876 LOAD_CONST              28 ('Warning: ')
+               248        3876 LOAD_CONST              28 ('Warning: ')
                
-               240        3878 BINARY_OP                0 (+)
+               247        3878 BINARY_OP                0 (+)
                
-               242        3882 LOAD_FAST                8 (instrument)
+               249        3882 LOAD_FAST                8 (instrument)
                
-               240        3884 BINARY_OP                0 (+)
+               247        3884 BINARY_OP                0 (+)
                
-               243        3888 LOAD_CONST              29 (' instrumentation does not exist.')
+               250        3888 LOAD_CONST              29 (' instrumentation does not exist.')
                
-               240        3890 BINARY_OP                0 (+)
+               247        3890 BINARY_OP                0 (+)
                
-               239        3894 PRECALL                  1
+               246        3894 PRECALL                  1
                           3898 CALL                     1
                           3908 POP_TOP
                
-               245        3910 LOAD_GLOBAL             59 (NULL + print)
+               252        3910 LOAD_GLOBAL             59 (NULL + print)
                
-               246        3922 LOAD_CONST              30 ('Usage:\nfrom syntrac.sdk.instruments import Instruments\nSyntrac.init(app_name="...", instruments=set([Instruments.OPENAI]))')
+               253        3922 LOAD_CONST              30 ('Usage:\nfrom syntrac.sdk.instruments import Instruments\nSyntrac.init(app_name="...", instruments=set([Instruments.OPENAI]))')
                
-               245        3924 PRECALL                  1
+               252        3924 PRECALL                  1
                           3928 CALL                     1
                           3938 POP_TOP
                
-               250        3940 LOAD_GLOBAL             59 (NULL + print)
+               257        3940 LOAD_GLOBAL             59 (NULL + print)
                           3952 LOAD_GLOBAL             60 (Fore)
                           3964 LOAD_ATTR               32 (RESET)
                           3974 PRECALL                  1
                           3978 CALL                     1
                           3988 POP_TOP
                           3990 EXTENDED_ARG             5
                           3992 JUMP_BACKWARD         1499 (to 996)
                
-               252     >> 3994 LOAD_FAST                7 (instrument_set)
+               259     >> 3994 LOAD_FAST                7 (instrument_set)
                           3996 POP_JUMP_FORWARD_IF_TRUE    53 (to 4104)
                
-               253        3998 LOAD_GLOBAL             59 (NULL + print)
+               260        3998 LOAD_GLOBAL             59 (NULL + print)
                
-               254        4010 LOAD_GLOBAL             60 (Fore)
+               261        4010 LOAD_GLOBAL             60 (Fore)
                           4022 LOAD_ATTR               31 (RED)
                           4032 LOAD_CONST              31 ("Warning: No valid instruments set. Remove 'instrument' argument to use all instruments, or set a valid instrument.")
                           4034 BINARY_OP                0 (+)
                
-               253        4038 PRECALL                  1
+               260        4038 PRECALL                  1
                           4042 CALL                     1
                           4052 POP_TOP
                
-               257        4054 LOAD_GLOBAL             59 (NULL + print)
+               264        4054 LOAD_GLOBAL             59 (NULL + print)
                           4066 LOAD_GLOBAL             60 (Fore)
                           4078 LOAD_ATTR               32 (RESET)
                           4088 PRECALL                  1
                           4092 CALL                     1
                           4102 POP_TOP
                
-               259     >> 4104 LOAD_GLOBAL            127 (NULL + ContentAllowList)
+               266     >> 4104 LOAD_GLOBAL            127 (NULL + ContentAllowList)
                           4116 PRECALL                  0
                           4120 CALL                     0
                           4130 LOAD_FAST                6 (obj)
                           4132 STORE_ATTR              64 (_TracerWrapper__content_allow_list)
                
-               262        4142 LOAD_GLOBAL            131 (NULL + atexit)
+               269        4142 LOAD_GLOBAL            131 (NULL + atexit)
                           4154 LOAD_ATTR               66 (register)
                           4164 LOAD_FAST                6 (obj)
                           4166 LOAD_ATTR               67 (exit_handler)
                           4176 PRECALL                  1
                           4180 CALL                     1
                           4190 POP_TOP
                
-               264     >> 4192 LOAD_FAST                0 (cls)
+               271     >> 4192 LOAD_FAST                0 (cls)
                           4194 LOAD_ATTR                4 (instance)
                           4204 RETURN_VALUE
                consts
                   None
                   'instance'
                   ('attributes',)
                   ('resource',)
@@ -1599,15 +1605,15 @@
                   "Warning: No valid instruments set. Remove 'instrument' argument to use all instruments, or set a valid instrument."
                names      ('hasattr', 'super', 'TracerWrapper', '__new__', 'instance', 'endpoint', 'Resource', 'resource_attributes', '_TracerWrapper__resource', 'init_tracer_provider', '_TracerWrapper__tracer_provider', 'Telemetry', 'capture', '_TracerWrapper__spans_processor', 'on_start', '_TracerWrapper__spans_processor_original_on_start', 'init_spans_exporter', 'headers', '_TracerWrapper__spans_exporter', 'is_notebook', 'SimpleSpanProcessor', 'BatchSpanProcessor', '_span_processor_on_start', 'add_span_processor', 'set_global_textmap', 'init_instrumentations', 'Instruments', 'OPENAI', 'init_openai_instrumentor', 'print', 'Fore', 'RED', 'RESET', 'ANTHROPIC', 'init_anthropic_instrumentor', 'COHERE', 'init_cohere_instrumentor', 'PINECONE', 'init_pinecone_instrumentor', 'CHROMA', 'init_chroma_instrumentor', 'LANGCHAIN', 'init_langchain_instrumentor', 'LLAMA_INDEX', 'init_llama_index_instrumentor', 'TRANSFORMERS', 'init_transformers_instrumentor', 'REQUESTS', 'init_requests_instrumentor', 'URLLIB3', 'init_urllib3_instrumentor', 'PYMYSQL', 'init_pymysql_instrumentor', 'BEDROCK', 'init_bedrock_instrumentor', 'REPLICATE', 'init_replicate_instrumentor', 'VERTEXAI', 'init_vertexai_instrumentor', 'WATSONX', 'init_watsonx_instrumentor', 'WEAVIATE', 'init_weaviate_instrumentor', 'ContentAllowList', '_TracerWrapper__content_allow_list', 'atexit', 'register', 'exit_handler')
                varnames   ('cls', 'disable_batch', 'processor', 'propagator', 'exporter', 'instruments', 'obj', 'instrument_set', 'instrument')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       '__new__'
-               firstlineno 54
+               firstlineno 61
                lnotab
                   0x040822015e01180104023e010c010cff1c03040148010e011a02040130
                   01020202010afe04fe12083001020216010afe04fe100a02ff06020c012c
                   ff0efd0c0720010c010cff1c040c010cff1a030e0222013e0204011e0204
                   0104011c0108020a0120011c0138013402060120011c010c011cff100334
                   02060120011c0138013602080120011c010c011cff10033602080120011c
                   0138013602080120011c010c011cff10033602080120011c010c011cff10
@@ -1621,374 +1627,196 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               266           0 RESUME                   0
+               273           0 RESUME                   0
                
-               267           2 LOAD_FAST                0 (self)
+               274           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (flush)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('flush',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       'exit_handler'
-               firstlineno 266
+               firstlineno 273
                lnotab 0x0201
             code
                argcount  : 3
-               nlocals   : 13
+               nlocals   : 6
                stacksize : 6
                flags     : 3
                code
-                  0x97007401000000000000000000006401a6010000ab0100000000000000
-                  007d037c0381207c01a00100000000000000000000000000000000000000
-                  007404000000000000000000006a0300000000000000007c03a6020000ab
-                  02000000000000000001007401000000000000000000006402a6010000ab
-                  0100000000000000007d047c0481207c01a0010000000000000000000000
-                  0000000000000000007404000000000000000000006a0400000000000000
-                  007c04a6020000ab02000000000000000001007401000000000000000000
-                  006403a6010000ab0100000000000000007d057c05819b7c05a005000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  0044005d2a5c0200007d067d077c01a00100000000000000000000000000
-                  000000000000007404000000000000000000006a0600000000000000009b
-                  0064047c069b009d037c07a6020000ab02000000000000000001008c2b7c
-                  006a07000000000000000073557c006a080000000000000000a009000000
-                  00000000000000000000000000000000007c05a6010000ab010000000000
-                  000000721e74150000000000000000000074170000000000000000000064
-                  056406a6020000ab020000000000000000a6010000ab0100000000000000
-                  0001006e1d74150000000000000000000074170000000000000000000064
-                  056407a6020000ab020000000000000000a6010000ab0100000000000000
-                  0001007419000000000000000000007c01a6010000ab0100000000000000
-                  0072e07401000000000000000000006408a6010000ab0100000000000000
-                  007d087c0881167c01a00100000000000000000000000000000000000000
-                  0064097c08a6020000ab0200000000000000000100740100000000000000
-                  000000640aa6010000ab0100000000000000007d097c0981167c01a00100
-                  00000000000000000000000000000000000000640b7c09a6020000ab0200
-                  000000000000000100740100000000000000000000640ca6010000ab0100
-                  000000000000007d0a7c0a81167c01a00100000000000000000000000000
-                  00000000000000640d7c0aa6020000ab0200000000000000000100740100
-                  000000000000000000640ea6010000ab0100000000000000007d0b7c0b81
-                  167c01a0010000000000000000000000000000000000000000640f7c0ba6
-                  020000ab02000000000000000001007401000000000000000000006410a6
-                  010000ab0100000000000000007d0c7c0b81337c0ca00500000000000000
-                  00000000000000000000000000a6000000ab00000000000000000044005d
-                  1e5c0200007d067d077c01a0010000000000000000000000000000000000
-                  00000064117c069b009d027c07a6020000ab02000000000000000001008c
-                  1f7c006a0d000000000000000072187c00a00d0000000000000000000000
-                  0000000000000000007c017c02a6020000ab020000000000000000010064
-                  00530064005300
-               269           0 RESUME                   0
+                  0x97007401000000000000000000007c01a6010000ab0100000000000000
+                  000100740300000000000000000000a6000000ab0000000000000000007d
+                  037c03817f7c03a0020000000000000000000000000000000000000000a6
+                  000000ab00000000000000000044005d2a5c0200007d047d057c01a00300
+                  000000000000000000000000000000000000007408000000000000000000
+                  006a0500000000000000009b0064017c049b009d037c05a6020000ab0200
+                  0000000000000001008c2b7c006a06000000000000000073397c006a0700
+                  00000000000000a00800000000000000000000000000000000000000007c
+                  03a6010000ab010000000000000000721074130000000000000000000064
+                  02a6010000ab01000000000000000001006e0f7413000000000000000000
+                  006403a6010000ab01000000000000000001007415000000000000000000
+                  007c01a6010000ab01000000000000000001007c006a0b00000000000000
+                  0072187c00a00b00000000000000000000000000000000000000007c017c
+                  02a6020000ab02000000000000000001006400530064005300
+               276           0 RESUME                   0
                
-               270           2 LOAD_GLOBAL              1 (NULL + get_value)
-                            14 LOAD_CONST               1 ('workflow_name')
+               277           2 LOAD_GLOBAL              1 (NULL + set_workflow_name_from_context)
+                            14 LOAD_FAST                1 (span)
                             16 PRECALL                  1
                             20 CALL                     1
-                            30 STORE_FAST               3 (workflow_name)
-               
-               271          32 LOAD_FAST                3 (workflow_name)
-                            34 POP_JUMP_FORWARD_IF_NONE    32 (to 100)
-               
-               272          36 LOAD_FAST                1 (span)
-                            38 LOAD_METHOD              1 (set_attribute)
-                            60 LOAD_GLOBAL              4 (SpanAttributes)
-                            72 LOAD_ATTR                3 (SYNTRAC_WORKFLOW_NAME)
-                            82 LOAD_FAST                3 (workflow_name)
-                            84 PRECALL                  2
-                            88 CALL                     2
-                            98 POP_TOP
-               
-               274     >>  100 LOAD_GLOBAL              1 (NULL + get_value)
-                           112 LOAD_CONST               2 ('correlation_id')
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 STORE_FAST               4 (correlation_id)
-               
-               275         130 LOAD_FAST                4 (correlation_id)
-                           132 POP_JUMP_FORWARD_IF_NONE    32 (to 198)
-               
-               276         134 LOAD_FAST                1 (span)
-                           136 LOAD_METHOD              1 (set_attribute)
-                           158 LOAD_GLOBAL              4 (SpanAttributes)
-                           170 LOAD_ATTR                4 (SYNTRAC_CORRELATION_ID)
-                           180 LOAD_FAST                4 (correlation_id)
-                           182 PRECALL                  2
-                           186 CALL                     2
-                           196 POP_TOP
-               
-               278     >>  198 LOAD_GLOBAL              1 (NULL + get_value)
-                           210 LOAD_CONST               3 ('association_properties')
-                           212 PRECALL                  1
-                           216 CALL                     1
-                           226 STORE_FAST               5 (association_properties)
-               
-               279         228 LOAD_FAST                5 (association_properties)
-                           230 POP_JUMP_FORWARD_IF_NONE   155 (to 542)
-               
-               280         232 LOAD_FAST                5 (association_properties)
-                           234 LOAD_METHOD              5 (items)
-                           256 PRECALL                  0
-                           260 CALL                     0
-                           270 GET_ITER
-                       >>  272 FOR_ITER                42 (to 358)
-                           274 UNPACK_SEQUENCE          2
-                           278 STORE_FAST               6 (key)
-                           280 STORE_FAST               7 (value)
-               
-               281         282 LOAD_FAST                1 (span)
-                           284 LOAD_METHOD              1 (set_attribute)
-               
-               282         306 LOAD_GLOBAL              4 (SpanAttributes)
-                           318 LOAD_ATTR                6 (SYNTRAC_ASSOCIATION_PROPERTIES)
-                           328 FORMAT_VALUE             0
-                           330 LOAD_CONST               4 ('.')
-                           332 LOAD_FAST                6 (key)
-                           334 FORMAT_VALUE             0
-                           336 BUILD_STRING             3
-                           338 LOAD_FAST                7 (value)
-               
-               281         340 PRECALL                  2
-                           344 CALL                     2
-                           354 POP_TOP
-                           356 JUMP_BACKWARD           43 (to 272)
-               
-               285     >>  358 LOAD_FAST                0 (self)
-                           360 LOAD_ATTR                7 (enable_content_tracing)
-                           370 POP_JUMP_FORWARD_IF_TRUE    85 (to 542)
-               
-               286         372 LOAD_FAST                0 (self)
-                           374 LOAD_ATTR                8 (_TracerWrapper__content_allow_list)
-                           384 LOAD_METHOD              9 (is_allowed)
-                           406 LOAD_FAST                5 (association_properties)
-                           408 PRECALL                  1
-                           412 CALL                     1
-                           422 POP_JUMP_FORWARD_IF_FALSE    30 (to 484)
-               
-               287         424 LOAD_GLOBAL             21 (NULL + attach)
-                           436 LOAD_GLOBAL             23 (NULL + set_value)
-                           448 LOAD_CONST               5 ('override_enable_content_tracing')
-                           450 LOAD_CONST               6 (True)
-                           452 PRECALL                  2
-                           456 CALL                     2
-                           466 PRECALL                  1
-                           470 CALL                     1
-                           480 POP_TOP
-                           482 JUMP_FORWARD            29 (to 542)
-               
-               289     >>  484 LOAD_GLOBAL             21 (NULL + attach)
-                           496 LOAD_GLOBAL             23 (NULL + set_value)
-                           508 LOAD_CONST               5 ('override_enable_content_tracing')
-                           510 LOAD_CONST               7 (False)
-                           512 PRECALL                  2
-                           516 CALL                     2
-                           526 PRECALL                  1
-                           530 CALL                     1
-                           540 POP_TOP
-               
-               291     >>  542 LOAD_GLOBAL             25 (NULL + is_llm_span)
-                           554 LOAD_FAST                1 (span)
-                           556 PRECALL                  1
-                           560 CALL                     1
-                           570 POP_JUMP_FORWARD_IF_FALSE   224 (to 1020)
-               
-               292         572 LOAD_GLOBAL              1 (NULL + get_value)
-                           584 LOAD_CONST               8 ('prompt_key')
-                           586 PRECALL                  1
-                           590 CALL                     1
-                           600 STORE_FAST               8 (prompt_key)
-               
-               293         602 LOAD_FAST                8 (prompt_key)
-                           604 POP_JUMP_FORWARD_IF_NONE    22 (to 650)
-               
-               294         606 LOAD_FAST                1 (span)
-                           608 LOAD_METHOD              1 (set_attribute)
-                           630 LOAD_CONST               9 ('syntrac.prompt.key')
-                           632 LOAD_FAST                8 (prompt_key)
-                           634 PRECALL                  2
-                           638 CALL                     2
-                           648 POP_TOP
-               
-               296     >>  650 LOAD_GLOBAL              1 (NULL + get_value)
-                           662 LOAD_CONST              10 ('prompt_version')
-                           664 PRECALL                  1
-                           668 CALL                     1
-                           678 STORE_FAST               9 (prompt_version)
-               
-               297         680 LOAD_FAST                9 (prompt_version)
-                           682 POP_JUMP_FORWARD_IF_NONE    22 (to 728)
-               
-               298         684 LOAD_FAST                1 (span)
-                           686 LOAD_METHOD              1 (set_attribute)
-                           708 LOAD_CONST              11 ('syntrac.prompt.version')
-                           710 LOAD_FAST                9 (prompt_version)
-                           712 PRECALL                  2
-                           716 CALL                     2
-                           726 POP_TOP
-               
-               300     >>  728 LOAD_GLOBAL              1 (NULL + get_value)
-                           740 LOAD_CONST              12 ('prompt_version_name')
-                           742 PRECALL                  1
-                           746 CALL                     1
-                           756 STORE_FAST              10 (prompt_version_name)
-               
-               301         758 LOAD_FAST               10 (prompt_version_name)
-                           760 POP_JUMP_FORWARD_IF_NONE    22 (to 806)
-               
-               302         762 LOAD_FAST                1 (span)
-                           764 LOAD_METHOD              1 (set_attribute)
-                           786 LOAD_CONST              13 ('syntrac.prompt.version_name')
-                           788 LOAD_FAST               10 (prompt_version_name)
-                           790 PRECALL                  2
-                           794 CALL                     2
-                           804 POP_TOP
-               
-               304     >>  806 LOAD_GLOBAL              1 (NULL + get_value)
-                           818 LOAD_CONST              14 ('prompt_version_hash')
-                           820 PRECALL                  1
-                           824 CALL                     1
-                           834 STORE_FAST              11 (prompt_version_hash)
-               
-               305         836 LOAD_FAST               11 (prompt_version_hash)
-                           838 POP_JUMP_FORWARD_IF_NONE    22 (to 884)
-               
-               306         840 LOAD_FAST                1 (span)
-                           842 LOAD_METHOD              1 (set_attribute)
-                           864 LOAD_CONST              15 ('syntrac.prompt.version_hash')
-                           866 LOAD_FAST               11 (prompt_version_hash)
-                           868 PRECALL                  2
-                           872 CALL                     2
-                           882 POP_TOP
-               
-               308     >>  884 LOAD_GLOBAL              1 (NULL + get_value)
-                           896 LOAD_CONST              16 ('prompt_template_variables')
-                           898 PRECALL                  1
-                           902 CALL                     1
-                           912 STORE_FAST              12 (prompt_template_variables)
-               
-               309         914 LOAD_FAST               11 (prompt_version_hash)
-                           916 POP_JUMP_FORWARD_IF_NONE    51 (to 1020)
+                            30 POP_TOP
                
-               310         918 LOAD_FAST               12 (prompt_template_variables)
-                           920 LOAD_METHOD              5 (items)
-                           942 PRECALL                  0
-                           946 CALL                     0
-                           956 GET_ITER
-                       >>  958 FOR_ITER                30 (to 1020)
-                           960 UNPACK_SEQUENCE          2
-                           964 STORE_FAST               6 (key)
-                           966 STORE_FAST               7 (value)
-               
-               311         968 LOAD_FAST                1 (span)
-                           970 LOAD_METHOD              1 (set_attribute)
-               
-               312         992 LOAD_CONST              17 ('syntrac.prompt.template_variables.')
-                           994 LOAD_FAST                6 (key)
-                           996 FORMAT_VALUE             0
-                           998 BUILD_STRING             2
-                          1000 LOAD_FAST                7 (value)
-               
-               311        1002 PRECALL                  2
-                          1006 CALL                     2
-                          1016 POP_TOP
-                          1018 JUMP_BACKWARD           31 (to 958)
-               
-               316     >> 1020 LOAD_FAST                0 (self)
-                          1022 LOAD_ATTR               13 (_TracerWrapper__spans_processor_original_on_start)
-                          1032 POP_JUMP_FORWARD_IF_FALSE    24 (to 1082)
-               
-               317        1034 LOAD_FAST                0 (self)
-                          1036 LOAD_METHOD             13 (_TracerWrapper__spans_processor_original_on_start)
-                          1058 LOAD_FAST                1 (span)
-                          1060 LOAD_FAST                2 (parent_context)
-                          1062 PRECALL                  2
-                          1066 CALL                     2
-                          1076 POP_TOP
-                          1078 LOAD_CONST               0 (None)
-                          1080 RETURN_VALUE
+               279          32 LOAD_GLOBAL              3 (NULL + get_association_properties)
+                            44 PRECALL                  0
+                            48 CALL                     0
+                            58 STORE_FAST               3 (association_properties)
+               
+               280          60 LOAD_FAST                3 (association_properties)
+                            62 POP_JUMP_FORWARD_IF_NONE   127 (to 318)
+               
+               281          64 LOAD_FAST                3 (association_properties)
+                            66 LOAD_METHOD              2 (items)
+                            88 PRECALL                  0
+                            92 CALL                     0
+                           102 GET_ITER
+                       >>  104 FOR_ITER                42 (to 190)
+                           106 UNPACK_SEQUENCE          2
+                           110 STORE_FAST               4 (key)
+                           112 STORE_FAST               5 (value)
+               
+               282         114 LOAD_FAST                1 (span)
+                           116 LOAD_METHOD              3 (set_attribute)
+               
+               283         138 LOAD_GLOBAL              8 (SpanAttributes)
+                           150 LOAD_ATTR                5 (SYNTRAC_ASSOCIATION_PROPERTIES)
+                           160 FORMAT_VALUE             0
+                           162 LOAD_CONST               1 ('.')
+                           164 LOAD_FAST                4 (key)
+                           166 FORMAT_VALUE             0
+                           168 BUILD_STRING             3
+                           170 LOAD_FAST                5 (value)
+               
+               282         172 PRECALL                  2
+                           176 CALL                     2
+                           186 POP_TOP
+                           188 JUMP_BACKWARD           43 (to 104)
+               
+               286     >>  190 LOAD_FAST                0 (self)
+                           192 LOAD_ATTR                6 (enable_content_tracing)
+                           202 POP_JUMP_FORWARD_IF_TRUE    57 (to 318)
+               
+               287         204 LOAD_FAST                0 (self)
+                           206 LOAD_ATTR                7 (_TracerWrapper__content_allow_list)
+                           216 LOAD_METHOD              8 (is_allowed)
+                           238 LOAD_FAST                3 (association_properties)
+                           240 PRECALL                  1
+                           244 CALL                     1
+                           254 POP_JUMP_FORWARD_IF_FALSE    16 (to 288)
+               
+               288         256 LOAD_GLOBAL             19 (NULL + set_override_enable_context_tracing)
+                           268 LOAD_CONST               2 (True)
+                           270 PRECALL                  1
+                           274 CALL                     1
+                           284 POP_TOP
+                           286 JUMP_FORWARD            15 (to 318)
+               
+               290     >>  288 LOAD_GLOBAL             19 (NULL + set_override_enable_context_tracing)
+                           300 LOAD_CONST               3 (False)
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 POP_TOP
+               
+               292     >>  318 LOAD_GLOBAL             21 (NULL + set_prompt_attributes_from_context)
+                           330 LOAD_FAST                1 (span)
+                           332 PRECALL                  1
+                           336 CALL                     1
+                           346 POP_TOP
+               
+               295         348 LOAD_FAST                0 (self)
+                           350 LOAD_ATTR               11 (_TracerWrapper__spans_processor_original_on_start)
+                           360 POP_JUMP_FORWARD_IF_FALSE    24 (to 410)
+               
+               296         362 LOAD_FAST                0 (self)
+                           364 LOAD_METHOD             11 (_TracerWrapper__spans_processor_original_on_start)
+                           386 LOAD_FAST                1 (span)
+                           388 LOAD_FAST                2 (parent_context)
+                           390 PRECALL                  2
+                           394 CALL                     2
+                           404 POP_TOP
+                           406 LOAD_CONST               0 (None)
+                           408 RETURN_VALUE
                
-               316     >> 1082 LOAD_CONST               0 (None)
-                          1084 RETURN_VALUE
+               295     >>  410 LOAD_CONST               0 (None)
+                           412 RETURN_VALUE
                consts
                   None
-                  'workflow_name'
-                  'correlation_id'
-                  'association_properties'
                   '.'
-                  'override_enable_content_tracing'
                   True
                   False
-                  'prompt_key'
-                  'syntrac.prompt.key'
-                  'prompt_version'
-                  'syntrac.prompt.version'
-                  'prompt_version_name'
-                  'syntrac.prompt.version_name'
-                  'prompt_version_hash'
-                  'syntrac.prompt.version_hash'
-                  'prompt_template_variables'
-                  'syntrac.prompt.template_variables.'
-               names      ('get_value', 'set_attribute', 'SpanAttributes', 'SYNTRAC_WORKFLOW_NAME', 'SYNTRAC_CORRELATION_ID', 'items', 'SYNTRAC_ASSOCIATION_PROPERTIES', 'enable_content_tracing', '_TracerWrapper__content_allow_list', 'is_allowed', 'attach', 'set_value', 'is_llm_span', '_TracerWrapper__spans_processor_original_on_start')
-               varnames   ('self', 'span', 'parent_context', 'workflow_name', 'correlation_id', 'association_properties', 'key', 'value', 'prompt_key', 'prompt_version', 'prompt_version_name', 'prompt_version_hash', 'prompt_template_variables')
+               names      ('set_workflow_name_from_context', 'get_association_properties', 'items', 'set_attribute', 'SpanAttributes', 'SYNTRAC_ASSOCIATION_PROPERTIES', 'enable_content_tracing', '_TracerWrapper__content_allow_list', 'is_allowed', 'set_override_enable_context_tracing', 'set_prompt_attributes_from_context', '_TracerWrapper__spans_processor_original_on_start')
+               varnames   ('self', 'span', 'parent_context', 'association_properties', 'key', 'value')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       '_span_processor_on_start'
-               firstlineno 269
+               firstlineno 276
                lnotab
-                  0x02011e01040140021e01040140021e0104013201180122ff12040e0134
-                  013c023a021e011e0104012c021e0104012c021e0104012c021e0104012c
-                  021e010401320118010aff12050e0130ff
+                  0x02011e021c0104013201180122ff12040e01340120021e021e030e0130
+                  ff
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 2
                flags     : 3
                code
                   0x97007c007400000000000000000000005f0100000000000000007c0174
                   00000000000000000000005f0200000000000000007c0274000000000000
                   00000000005f0300000000000000007c037400000000000000000000005f
                   04000000000000000064005300
-               319           0 RESUME                   0
+               298           0 RESUME                   0
                
-               326           2 LOAD_FAST                0 (resource_attributes)
+               305           2 LOAD_FAST                0 (resource_attributes)
                              4 LOAD_GLOBAL              0 (TracerWrapper)
                             16 STORE_ATTR               1 (resource_attributes)
                
-               327          26 LOAD_FAST                1 (enable_content_tracing)
+               306          26 LOAD_FAST                1 (enable_content_tracing)
                             28 LOAD_GLOBAL              0 (TracerWrapper)
                             40 STORE_ATTR               2 (enable_content_tracing)
                
-               328          50 LOAD_FAST                2 (endpoint)
+               307          50 LOAD_FAST                2 (endpoint)
                             52 LOAD_GLOBAL              0 (TracerWrapper)
                             64 STORE_ATTR               3 (endpoint)
                
-               329          74 LOAD_FAST                3 (headers)
+               308          74 LOAD_FAST                3 (headers)
                             76 LOAD_GLOBAL              0 (TracerWrapper)
                             88 STORE_ATTR               4 (headers)
                             98 LOAD_CONST               0 (None)
                            100 RETURN_VALUE
                consts
                   None
                names      ('TracerWrapper', 'resource_attributes', 'enable_content_tracing', 'endpoint', 'headers')
                varnames   ('resource_attributes', 'enable_content_tracing', 'endpoint', 'headers')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       'set_static_params'
-               firstlineno 319
+               firstlineno 298
                lnotab 0x0207180118011801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
@@ -1997,64 +1825,64 @@
                   006403a6010000ab01000000000000000070016404a00300000000000000
                   00000000000000000000000000a6000000ab00000000000000000064056b
                   0200000000720264065300740900000000000000000000740a0000000000
                   00000000006a06000000000000000064077a000000a6010000ab01000000
                   00000000000100740900000000000000000000740a000000000000000000
                   006a070000000000000000a6010000ab0100000000000000000100640653
                   00
-               331           0 RESUME                   0
+               310           0 RESUME                   0
                
-               333           2 LOAD_GLOBAL              1 (NULL + hasattr)
+               312           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('instance')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE     2 (to 38)
                
-               334          34 LOAD_CONST               2 (True)
+               313          34 LOAD_CONST               2 (True)
                             36 RETURN_VALUE
                
-               336     >>   38 LOAD_GLOBAL              3 (NULL + os)
+               315     >>   38 LOAD_GLOBAL              3 (NULL + os)
                             50 LOAD_ATTR                2 (getenv)
                             60 LOAD_CONST               3 ('SYNTRAC_SUPPRESS_WARNINGS')
                             62 PRECALL                  1
                             66 CALL                     1
                             76 JUMP_IF_TRUE_OR_POP      1 (to 80)
                             78 LOAD_CONST               4 ('false')
                        >>   80 LOAD_METHOD              3 (lower)
                            102 PRECALL                  0
                            106 CALL                     0
                            116 LOAD_CONST               5 ('true')
                            118 COMPARE_OP               2 (==)
                            124 POP_JUMP_FORWARD_IF_FALSE     2 (to 130)
                
-               337         126 LOAD_CONST               6 (False)
+               316         126 LOAD_CONST               6 (False)
                            128 RETURN_VALUE
                
-               339     >>  130 LOAD_GLOBAL              9 (NULL + print)
+               318     >>  130 LOAD_GLOBAL              9 (NULL + print)
                
-               340         142 LOAD_GLOBAL             10 (Fore)
+               319         142 LOAD_GLOBAL             10 (Fore)
                            154 LOAD_ATTR                6 (RED)
                
-               341         164 LOAD_CONST               7 ('Warning: Syntrac not initialized, make sure you call Syntrac.init()')
+               320         164 LOAD_CONST               7 ('Warning: Syntrac not initialized, make sure you call Syntrac.init()')
                
-               340         166 BINARY_OP                0 (+)
+               319         166 BINARY_OP                0 (+)
                
-               339         170 PRECALL                  1
+               318         170 PRECALL                  1
                            174 CALL                     1
                            184 POP_TOP
                
-               343         186 LOAD_GLOBAL              9 (NULL + print)
+               322         186 LOAD_GLOBAL              9 (NULL + print)
                            198 LOAD_GLOBAL             10 (Fore)
                            210 LOAD_ATTR                7 (RESET)
                            220 PRECALL                  1
                            224 CALL                     1
                            234 POP_TOP
                
-               344         236 LOAD_CONST               6 (False)
+               323         236 LOAD_CONST               6 (False)
                            238 RETURN_VALUE
                consts
                   None
                   'instance'
                   True
                   'SYNTRAC_SUPPRESS_WARNINGS'
                   'false'
@@ -2063,27 +1891,27 @@
                   'Warning: Syntrac not initialized, make sure you call Syntrac.init()'
                names      ('hasattr', 'os', 'getenv', 'lower', 'print', 'Fore', 'RED', 'RESET')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       'verify_initialized'
-               firstlineno 331
+               firstlineno 310
                lnotab 0x020220010402580104020c01160102ff04ff10043201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-               346           0 RESUME                   0
+               325           0 RESUME                   0
                
-               347           2 LOAD_FAST                0 (self)
+               326           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_TracerWrapper__spans_processor)
                             14 LOAD_METHOD              1 (force_flush)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 POP_TOP
                             52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
@@ -2091,261 +1919,71 @@
                   None
                names      ('_TracerWrapper__spans_processor', 'force_flush')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       'flush'
-               firstlineno 346
+               firstlineno 325
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000740400000000000000000000a6010000ab010000000000
                   0000005300
-               349           0 RESUME                   0
+               328           0 RESUME                   0
                
-               350           2 LOAD_FAST                0 (self)
+               329           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_TracerWrapper__tracer_provider)
                             14 LOAD_METHOD              1 (get_tracer)
                             36 LOAD_GLOBAL              4 (TRACER_NAME)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 RETURN_VALUE
                consts
                   None
                names      ('_TracerWrapper__tracer_provider', 'get_tracer', 'TRACER_NAME')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
                name       'get_tracer'
-               firstlineno 349
+               firstlineno 328
                lnotab 0x0201
             (False, None, None, None, None)
-         names      ('__name__', '__module__', '__qualname__', 'resource_attributes', 'dict', '__annotations__', 'enable_content_tracing', 'bool', 'endpoint', 'str', 'headers', 'Dict', 'SpanProcessor', 'TextMapPropagator', 'SpanExporter', 'Optional', 'Set', 'Instruments', '__new__', 'exit_handler', '_span_processor_on_start', 'staticmethod', 'set_static_params', 'classmethod', 'verify_initialized', 'flush', 'get_tracer', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'resource_attributes', 'dict', '__annotations__', 'enable_content_tracing', 'bool', 'endpoint', 'Optional', 'str', 'headers', 'Dict', 'Resource', 'TracerProvider', 'SpanProcessor', '_TracerWrapper__spans_processor_original_on_start', 'Callable', 'SpanExporter', 'ContentAllowList', 'TextMapPropagator', 'Set', 'Instruments', '__new__', 'exit_handler', '_span_processor_on_start', 'staticmethod', 'set_static_params', 'classmethod', 'verify_initialized', 'flush', 'get_tracer', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'TracerWrapper'
-         firstlineno 48
+         firstlineno 49
          lnotab
-            0x0e010e010e010e011e04020102010201020102fa040302fd020402fc02
-            0502fb02061afa020702f90c7f0055060306320201020102ff020202fe02
-            0302fd020412fc020502fb06ff0e01020b02010aff0e01020e0603
+            0x0e010e010e011a011e010a010a010a011a010a010a0402010201020102
+            0102fa04030efd02040efc02050efb02061afa020702f90c7f0055060306
+            160201020102ff020202fe020302fd020412fc020502fb06ff0e01020b02
+            010aff0e01020e0603
       'TracerWrapper'
-      'correlation_id'
       'return'
       code
          argcount  : 1
          nlocals   : 1
-         stacksize : 6
-         flags     : 3
-         code
-            0x970074010000000000000000000074030000000000000000000064017c
-            00a6020000ab020000000000000000a6010000ab01000000000000000001
-            0064005300
-         353           0 RESUME                   0
-         
-         354           2 LOAD_GLOBAL              1 (NULL + attach)
-                      14 LOAD_GLOBAL              3 (NULL + set_value)
-                      26 LOAD_CONST               1 ('correlation_id')
-                      28 LOAD_FAST                0 (correlation_id)
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 PRECALL                  1
-                      48 CALL                     1
-                      58 POP_TOP
-                      60 LOAD_CONST               0 (None)
-                      62 RETURN_VALUE
-         consts
-            None
-            'correlation_id'
-         names      ('attach', 'set_value')
-         varnames   ('correlation_id',)
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
-         name       'set_correlation_id'
-         firstlineno 353
-         lnotab 0x0201
-      'properties'
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 6
-         flags     : 3
-         code
-            0x970074010000000000000000000074030000000000000000000064017c
-            00a6020000ab020000000000000000a6010000ab01000000000000000001
-            0064005300
-         357           0 RESUME                   0
-         
-         358           2 LOAD_GLOBAL              1 (NULL + attach)
-                      14 LOAD_GLOBAL              3 (NULL + set_value)
-                      26 LOAD_CONST               1 ('association_properties')
-                      28 LOAD_FAST                0 (properties)
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 PRECALL                  1
-                      48 CALL                     1
-                      58 POP_TOP
-                      60 LOAD_CONST               0 (None)
-                      62 RETURN_VALUE
-         consts
-            None
-            'association_properties'
-         names      ('attach', 'set_value')
-         varnames   ('properties',)
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
-         name       'set_association_properties'
-         firstlineno 357
-         lnotab 0x0201
-      'workflow_name'
-      code
-         argcount  : 1
-         nlocals   : 1
-         stacksize : 6
-         flags     : 3
-         code
-            0x970074010000000000000000000074030000000000000000000064017c
-            00a6020000ab020000000000000000a6010000ab01000000000000000001
-            0064005300
-         361           0 RESUME                   0
-         
-         362           2 LOAD_GLOBAL              1 (NULL + attach)
-                      14 LOAD_GLOBAL              3 (NULL + set_value)
-                      26 LOAD_CONST               1 ('workflow_name')
-                      28 LOAD_FAST                0 (workflow_name)
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 PRECALL                  1
-                      48 CALL                     1
-                      58 POP_TOP
-                      60 LOAD_CONST               0 (None)
-                      62 RETURN_VALUE
-         consts
-            None
-            'workflow_name'
-         names      ('attach', 'set_value')
-         varnames   ('workflow_name',)
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
-         name       'set_workflow_name'
-         firstlineno 361
-         lnotab 0x0201
-      'key'
-      'version'
-      'version_name'
-      'version_hash'
-      'template_variables'
-      code
-         argcount  : 5
-         nlocals   : 5
-         stacksize : 6
-         flags     : 3
-         code
-            0x970074010000000000000000000074030000000000000000000064017c
-            00a6020000ab020000000000000000a6010000ab01000000000000000001
-            0074010000000000000000000074030000000000000000000064027c01a6
-            020000ab020000000000000000a6010000ab010000000000000000010074
-            010000000000000000000074030000000000000000000064037c02a60200
-            00ab020000000000000000a6010000ab0100000000000000000100740100
-            00000000000000000074030000000000000000000064047c03a6020000ab
-            020000000000000000a6010000ab01000000000000000001007401000000
-            0000000000000074030000000000000000000064057c04a6020000ab0200
-            00000000000000a6010000ab010000000000000000010064005300
-         365           0 RESUME                   0
-         
-         372           2 LOAD_GLOBAL              1 (NULL + attach)
-                      14 LOAD_GLOBAL              3 (NULL + set_value)
-                      26 LOAD_CONST               1 ('prompt_key')
-                      28 LOAD_FAST                0 (key)
-                      30 PRECALL                  2
-                      34 CALL                     2
-                      44 PRECALL                  1
-                      48 CALL                     1
-                      58 POP_TOP
-         
-         373          60 LOAD_GLOBAL              1 (NULL + attach)
-                      72 LOAD_GLOBAL              3 (NULL + set_value)
-                      84 LOAD_CONST               2 ('prompt_version')
-                      86 LOAD_FAST                1 (version)
-                      88 PRECALL                  2
-                      92 CALL                     2
-                     102 PRECALL                  1
-                     106 CALL                     1
-                     116 POP_TOP
-         
-         374         118 LOAD_GLOBAL              1 (NULL + attach)
-                     130 LOAD_GLOBAL              3 (NULL + set_value)
-                     142 LOAD_CONST               3 ('prompt_version_name')
-                     144 LOAD_FAST                2 (version_name)
-                     146 PRECALL                  2
-                     150 CALL                     2
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 POP_TOP
-         
-         375         176 LOAD_GLOBAL              1 (NULL + attach)
-                     188 LOAD_GLOBAL              3 (NULL + set_value)
-                     200 LOAD_CONST               4 ('prompt_version_hash')
-                     202 LOAD_FAST                3 (version_hash)
-                     204 PRECALL                  2
-                     208 CALL                     2
-                     218 PRECALL                  1
-                     222 CALL                     1
-                     232 POP_TOP
-         
-         376         234 LOAD_GLOBAL              1 (NULL + attach)
-                     246 LOAD_GLOBAL              3 (NULL + set_value)
-                     258 LOAD_CONST               5 ('prompt_template_variables')
-                     260 LOAD_FAST                4 (template_variables)
-                     262 PRECALL                  2
-                     266 CALL                     2
-                     276 PRECALL                  1
-                     280 CALL                     1
-                     290 POP_TOP
-                     292 LOAD_CONST               0 (None)
-                     294 RETURN_VALUE
-         consts
-            None
-            'prompt_key'
-            'prompt_version'
-            'prompt_version_name'
-            'prompt_version_hash'
-            'prompt_template_variables'
-         names      ('attach', 'set_value')
-         varnames   ('key', 'version', 'version_name', 'version_hash', 'template_variables')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
-         name       'set_prompt_tracing_context'
-         firstlineno 365
-         lnotab 0x02073a013a013a013a01
-      code
-         argcount  : 1
-         nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             000000000000007404000000000000000000006a030000000000000000a6
             010000ab010000000000000000640075015300
-         379           0 RESUME                   0
+         332           0 RESUME                   0
          
-         380           2 LOAD_FAST                0 (span)
+         333           2 LOAD_FAST                0 (span)
                        4 LOAD_ATTR                0 (attributes)
                       14 LOAD_METHOD              1 (get)
                       36 LOAD_GLOBAL              4 (SpanAttributes)
                       48 LOAD_ATTR                3 (LLM_REQUEST_TYPE)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 LOAD_CONST               0 (None)
@@ -2355,29 +1993,29 @@
             None
          names      ('attributes', 'get', 'SpanAttributes', 'LLM_REQUEST_TYPE')
          varnames   ('span',)
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'is_llm_span'
-         firstlineno 379
+         firstlineno 332
          lnotab 0x0201
       'api_endpoint'
       'headers'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c009b0064019d027c01ac02a60200
             00ab0200000000000000005300
-         383           0 RESUME                   0
+         336           0 RESUME                   0
          
-         384           2 LOAD_GLOBAL              1 (NULL + OTLPSpanExporter)
+         337           2 LOAD_GLOBAL              1 (NULL + OTLPSpanExporter)
                       14 LOAD_FAST                0 (api_endpoint)
                       16 FORMAT_VALUE             0
                       18 LOAD_CONST               1 ('/v1/traces')
                       20 BUILD_STRING             2
                       22 LOAD_FAST                1 (headers)
                       24 KW_NAMES                 2
                       26 PRECALL                  2
@@ -2389,15 +2027,15 @@
             ('endpoint', 'headers')
          names      ('OTLPSpanExporter',)
          varnames   ('api_endpoint', 'headers')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_spans_exporter'
-         firstlineno 383
+         firstlineno 336
          lnotab 0x0201
       'resource'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
@@ -2406,82 +2044,82 @@
             0000007d027403000000000000000000007c027404000000000000000000
             00a6020000ab02000000000000000072257407000000000000000000007c
             00ac01a6010000ab0100000000000000007d017409000000000000000000
             006a0500000000000000007c01a6010000ab01000000000000000001006e
             28740d000000000000000000007c026402a6020000ab0200000000000000
             007316740f000000000000000000006a0800000000000000006403a60100
             00ab0100000000000000000100640053007c027d017c015300
-         387           0 RESUME                   0
+         340           0 RESUME                   0
          
-         388           2 LOAD_CONST               0 (None)
+         341           2 LOAD_CONST               0 (None)
                        4 STORE_FAST               1 (provider)
          
-         389           6 LOAD_GLOBAL              1 (NULL + get_tracer_provider)
+         342           6 LOAD_GLOBAL              1 (NULL + get_tracer_provider)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_FAST               2 (default_provider)
          
-         391          34 LOAD_GLOBAL              3 (NULL + isinstance)
+         344          34 LOAD_GLOBAL              3 (NULL + isinstance)
                       46 LOAD_FAST                2 (default_provider)
                       48 LOAD_GLOBAL              4 (ProxyTracerProvider)
                       60 PRECALL                  2
                       64 CALL                     2
                       74 POP_JUMP_FORWARD_IF_FALSE    37 (to 150)
          
-         392          76 LOAD_GLOBAL              7 (NULL + TracerProvider)
+         345          76 LOAD_GLOBAL              7 (NULL + TracerProvider)
                       88 LOAD_FAST                0 (resource)
                       90 KW_NAMES                 1
                       92 PRECALL                  1
                       96 CALL                     1
                      106 STORE_FAST               1 (provider)
          
-         393         108 LOAD_GLOBAL              9 (NULL + trace)
+         346         108 LOAD_GLOBAL              9 (NULL + trace)
                      120 LOAD_ATTR                5 (set_tracer_provider)
                      130 LOAD_FAST                1 (provider)
                      132 PRECALL                  1
                      136 CALL                     1
                      146 POP_TOP
                      148 JUMP_FORWARD            40 (to 230)
          
-         394     >>  150 LOAD_GLOBAL             13 (NULL + hasattr)
+         347     >>  150 LOAD_GLOBAL             13 (NULL + hasattr)
                      162 LOAD_FAST                2 (default_provider)
                      164 LOAD_CONST               2 ('add_span_processor')
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_JUMP_FORWARD_IF_TRUE    22 (to 226)
          
-         395         182 LOAD_GLOBAL             15 (NULL + logging)
+         348         182 LOAD_GLOBAL             15 (NULL + logging)
                      194 LOAD_ATTR                8 (error)
          
-         396         204 LOAD_CONST               3 ("Cannot add span processor to the default provider since it doesn't support it")
+         349         204 LOAD_CONST               3 ("Cannot add span processor to the default provider since it doesn't support it")
          
-         395         206 PRECALL                  1
+         348         206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         398         222 LOAD_CONST               0 (None)
+         351         222 LOAD_CONST               0 (None)
                      224 RETURN_VALUE
          
-         400     >>  226 LOAD_FAST                2 (default_provider)
+         353     >>  226 LOAD_FAST                2 (default_provider)
                      228 STORE_FAST               1 (provider)
          
-         402     >>  230 LOAD_FAST                1 (provider)
+         355     >>  230 LOAD_FAST                1 (provider)
                      232 RETURN_VALUE
          consts
             None
             ('resource',)
             'add_span_processor'
             "Cannot add span processor to the default provider since it doesn't support it"
          names      ('get_tracer_provider', 'isinstance', 'ProxyTracerProvider', 'TracerProvider', 'trace', 'set_tracer_provider', 'hasattr', 'logging', 'error')
          varnames   ('resource', 'provider', 'default_provider')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_tracer_provider'
-         firstlineno 387
+         firstlineno 340
          lnotab 0x020104011c022a0120012a012001160102ff100304020402
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
@@ -2499,116 +2137,116 @@
             000000000000000100741900000000000000000000a6000000ab00000000
             00000000000100741b00000000000000000000a6000000ab000000000000
             0000000100741d00000000000000000000a6000000ab0000000000000000
             000100741f00000000000000000000a6000000ab00000000000000000001
             00742100000000000000000000a6000000ab000000000000000000010074
             2300000000000000000000a6000000ab0000000000000000000100640053
             00
-         405           0 RESUME                   0
+         358           0 RESUME                   0
          
-         406           2 LOAD_GLOBAL              1 (NULL + init_openai_instrumentor)
+         359           2 LOAD_GLOBAL              1 (NULL + init_openai_instrumentor)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
          
-         407          30 LOAD_GLOBAL              3 (NULL + init_anthropic_instrumentor)
+         360          30 LOAD_GLOBAL              3 (NULL + init_anthropic_instrumentor)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 POP_TOP
          
-         408          58 LOAD_GLOBAL              5 (NULL + init_cohere_instrumentor)
+         361          58 LOAD_GLOBAL              5 (NULL + init_cohere_instrumentor)
                       70 PRECALL                  0
                       74 CALL                     0
                       84 POP_TOP
          
-         409          86 LOAD_GLOBAL              7 (NULL + init_pinecone_instrumentor)
+         362          86 LOAD_GLOBAL              7 (NULL + init_pinecone_instrumentor)
                       98 PRECALL                  0
                      102 CALL                     0
                      112 POP_TOP
          
-         410         114 LOAD_GLOBAL              9 (NULL + init_qdrant_instrumentor)
+         363         114 LOAD_GLOBAL              9 (NULL + init_qdrant_instrumentor)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 POP_TOP
          
-         411         142 LOAD_GLOBAL             11 (NULL + init_chroma_instrumentor)
+         364         142 LOAD_GLOBAL             11 (NULL + init_chroma_instrumentor)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 POP_TOP
          
-         412         170 LOAD_GLOBAL             13 (NULL + init_haystack_instrumentor)
+         365         170 LOAD_GLOBAL             13 (NULL + init_haystack_instrumentor)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-         413         198 LOAD_GLOBAL             15 (NULL + init_langchain_instrumentor)
+         366         198 LOAD_GLOBAL             15 (NULL + init_langchain_instrumentor)
                      210 PRECALL                  0
                      214 CALL                     0
                      224 POP_TOP
          
-         414         226 LOAD_GLOBAL             17 (NULL + init_llama_index_instrumentor)
+         367         226 LOAD_GLOBAL             17 (NULL + init_llama_index_instrumentor)
                      238 PRECALL                  0
                      242 CALL                     0
                      252 POP_TOP
          
-         415         254 LOAD_GLOBAL             19 (NULL + init_transformers_instrumentor)
+         368         254 LOAD_GLOBAL             19 (NULL + init_transformers_instrumentor)
                      266 PRECALL                  0
                      270 CALL                     0
                      280 POP_TOP
          
-         416         282 LOAD_GLOBAL             21 (NULL + init_requests_instrumentor)
+         369         282 LOAD_GLOBAL             21 (NULL + init_requests_instrumentor)
                      294 PRECALL                  0
                      298 CALL                     0
                      308 POP_TOP
          
-         417         310 LOAD_GLOBAL             23 (NULL + init_urllib3_instrumentor)
+         370         310 LOAD_GLOBAL             23 (NULL + init_urllib3_instrumentor)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 POP_TOP
          
-         418         338 LOAD_GLOBAL             25 (NULL + init_pymysql_instrumentor)
+         371         338 LOAD_GLOBAL             25 (NULL + init_pymysql_instrumentor)
                      350 PRECALL                  0
                      354 CALL                     0
                      364 POP_TOP
          
-         419         366 LOAD_GLOBAL             27 (NULL + init_bedrock_instrumentor)
+         372         366 LOAD_GLOBAL             27 (NULL + init_bedrock_instrumentor)
                      378 PRECALL                  0
                      382 CALL                     0
                      392 POP_TOP
          
-         420         394 LOAD_GLOBAL             29 (NULL + init_replicate_instrumentor)
+         373         394 LOAD_GLOBAL             29 (NULL + init_replicate_instrumentor)
                      406 PRECALL                  0
                      410 CALL                     0
                      420 POP_TOP
          
-         421         422 LOAD_GLOBAL             31 (NULL + init_vertexai_instrumentor)
+         374         422 LOAD_GLOBAL             31 (NULL + init_vertexai_instrumentor)
                      434 PRECALL                  0
                      438 CALL                     0
                      448 POP_TOP
          
-         422         450 LOAD_GLOBAL             33 (NULL + init_watsonx_instrumentor)
+         375         450 LOAD_GLOBAL             33 (NULL + init_watsonx_instrumentor)
                      462 PRECALL                  0
                      466 CALL                     0
                      476 POP_TOP
          
-         423         478 LOAD_GLOBAL             35 (NULL + init_weaviate_instrumentor)
+         376         478 LOAD_GLOBAL             35 (NULL + init_weaviate_instrumentor)
                      490 PRECALL                  0
                      494 CALL                     0
                      504 POP_TOP
                      506 LOAD_CONST               0 (None)
                      508 RETURN_VALUE
          consts
             None
          names      ('init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_llama_index_instrumentor', 'init_transformers_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_instrumentations'
-         firstlineno 405
+         firstlineno 358
          lnotab
             0x02011c011c011c011c011c011c011c011c011c011c011c011c011c011c
             011c011c011c01
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
@@ -2618,59 +2256,59 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814e740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c006405ac
             06a6010000ab0100000000000000007d017c016a07000000000000000073
             147c01a0080000000000000000000000000000000000000000a6000000ab
             000000000000000000010064055300
-         426           0 RESUME                   0
+         379           0 RESUME                   0
          
-         427           2 LOAD_GLOBAL              0 (importlib)
+         380           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('openai')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    78 (to 220)
          
-         428          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         381          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:openai:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         429         130 LOAD_CONST               3 (0)
+         382         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('OpenAIInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.openai)
                      136 IMPORT_FROM              6 (OpenAIInstrumentor)
                      138 STORE_FAST               0 (OpenAIInstrumentor)
                      140 POP_TOP
          
-         431         142 PUSH_NULL
+         384         142 PUSH_NULL
                      144 LOAD_FAST                0 (OpenAIInstrumentor)
                      146 LOAD_CONST               5 (True)
                      148 KW_NAMES                 6
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               1 (instrumentor)
          
-         432         166 LOAD_FAST                1 (instrumentor)
+         385         166 LOAD_FAST                1 (instrumentor)
                      168 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      178 POP_JUMP_FORWARD_IF_TRUE    20 (to 220)
          
-         433         180 LOAD_FAST                1 (instrumentor)
+         386         180 LOAD_FAST                1 (instrumentor)
                      182 LOAD_METHOD              8 (instrument)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 POP_TOP
          
-         434     >>  220 LOAD_CONST               5 (True)
+         387     >>  220 LOAD_CONST               5 (True)
                      222 RETURN_VALUE
          consts
             None
             'openai'
             'instrumentation:openai:init'
             0
             ('OpenAIInstrumentor',)
@@ -2678,15 +2316,15 @@
             ('enrich_assistant',)
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.openai', 'OpenAIInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('OpenAIInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_openai_instrumentor'
-         firstlineno 426
+         firstlineno 379
          lnotab 0x02013e0142010c0218010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2694,72 +2332,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         437           0 RESUME                   0
+         390           0 RESUME                   0
          
-         438           2 LOAD_GLOBAL              0 (importlib)
+         391           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('anthropic')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         439          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         392          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:anthropic:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         440         130 LOAD_CONST               3 (0)
+         393         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('AnthropicInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.anthropic)
                      136 IMPORT_FROM              6 (AnthropicInstrumentor)
                      138 STORE_FAST               0 (AnthropicInstrumentor)
                      140 POP_TOP
          
-         442         142 PUSH_NULL
+         395         142 PUSH_NULL
                      144 LOAD_FAST                0 (AnthropicInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         443         162 LOAD_FAST                1 (instrumentor)
+         396         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         444         176 LOAD_FAST                1 (instrumentor)
+         397         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         445     >>  216 LOAD_CONST               5 (True)
+         398     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'anthropic'
             'instrumentation:anthropic:init'
             0
             ('AnthropicInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.anthropic', 'AnthropicInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('AnthropicInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_anthropic_instrumentor'
-         firstlineno 437
+         firstlineno 390
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2767,72 +2405,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         448           0 RESUME                   0
+         401           0 RESUME                   0
          
-         449           2 LOAD_GLOBAL              0 (importlib)
+         402           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('cohere')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         450          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         403          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:cohere:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         451         130 LOAD_CONST               3 (0)
+         404         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('CohereInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.cohere)
                      136 IMPORT_FROM              6 (CohereInstrumentor)
                      138 STORE_FAST               0 (CohereInstrumentor)
                      140 POP_TOP
          
-         453         142 PUSH_NULL
+         406         142 PUSH_NULL
                      144 LOAD_FAST                0 (CohereInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         454         162 LOAD_FAST                1 (instrumentor)
+         407         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         455         176 LOAD_FAST                1 (instrumentor)
+         408         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         456     >>  216 LOAD_CONST               5 (True)
+         409     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'cohere'
             'instrumentation:cohere:init'
             0
             ('CohereInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.cohere', 'CohereInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('CohereInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_cohere_instrumentor'
-         firstlineno 448
+         firstlineno 401
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2840,72 +2478,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         459           0 RESUME                   0
+         412           0 RESUME                   0
          
-         460           2 LOAD_GLOBAL              0 (importlib)
+         413           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('pinecone')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         461          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         414          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:pinecone:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         462         130 LOAD_CONST               3 (0)
+         415         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('PineconeInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.pinecone)
                      136 IMPORT_FROM              6 (PineconeInstrumentor)
                      138 STORE_FAST               0 (PineconeInstrumentor)
                      140 POP_TOP
          
-         464         142 PUSH_NULL
+         417         142 PUSH_NULL
                      144 LOAD_FAST                0 (PineconeInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         465         162 LOAD_FAST                1 (instrumentor)
+         418         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         466         176 LOAD_FAST                1 (instrumentor)
+         419         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         467     >>  216 LOAD_CONST               5 (True)
+         420     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'pinecone'
             'instrumentation:pinecone:init'
             0
             ('PineconeInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.pinecone', 'PineconeInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('PineconeInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_pinecone_instrumentor'
-         firstlineno 459
+         firstlineno 412
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2913,76 +2551,76 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814e740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073187c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             00000000000100640053006400530064005300
-         470           0 RESUME                   0
+         423           0 RESUME                   0
          
-         471           2 LOAD_GLOBAL              0 (importlib)
+         424           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('qdrant_client')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    78 (to 220)
          
-         472          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         425          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:qdrant:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         473         130 LOAD_CONST               3 (0)
+         426         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('QdrantInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.qdrant)
                      136 IMPORT_FROM              6 (QdrantInstrumentor)
                      138 STORE_FAST               0 (QdrantInstrumentor)
                      140 POP_TOP
          
-         475         142 PUSH_NULL
+         428         142 PUSH_NULL
                      144 LOAD_FAST                0 (QdrantInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         476         162 LOAD_FAST                1 (instrumentor)
+         429         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    24 (to 224)
          
-         477         176 LOAD_FAST                1 (instrumentor)
+         430         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
                      216 LOAD_CONST               0 (None)
                      218 RETURN_VALUE
          
-         471     >>  220 LOAD_CONST               0 (None)
+         424     >>  220 LOAD_CONST               0 (None)
                      222 RETURN_VALUE
          
-         476     >>  224 LOAD_CONST               0 (None)
+         429     >>  224 LOAD_CONST               0 (None)
                      226 RETURN_VALUE
          consts
             None
             'qdrant_client'
             'instrumentation:qdrant:init'
             0
             ('QdrantInstrumentor',)
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.qdrant', 'QdrantInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('QdrantInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_qdrant_instrumentor'
-         firstlineno 470
+         firstlineno 423
          lnotab 0x02013e0142010c0214010e012cfa0405
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -2990,72 +2628,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         480           0 RESUME                   0
+         433           0 RESUME                   0
          
-         481           2 LOAD_GLOBAL              0 (importlib)
+         434           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('chromadb')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         482          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         435          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:chromadb:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         483         130 LOAD_CONST               3 (0)
+         436         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('ChromaInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.chromadb)
                      136 IMPORT_FROM              6 (ChromaInstrumentor)
                      138 STORE_FAST               0 (ChromaInstrumentor)
                      140 POP_TOP
          
-         485         142 PUSH_NULL
+         438         142 PUSH_NULL
                      144 LOAD_FAST                0 (ChromaInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         486         162 LOAD_FAST                1 (instrumentor)
+         439         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         487         176 LOAD_FAST                1 (instrumentor)
+         440         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         488     >>  216 LOAD_CONST               5 (True)
+         441     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'chromadb'
             'instrumentation:chromadb:init'
             0
             ('ChromaInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.chromadb', 'ChromaInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('ChromaInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_chroma_instrumentor'
-         firstlineno 480
+         firstlineno 433
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3063,72 +2701,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         491           0 RESUME                   0
+         444           0 RESUME                   0
          
-         492           2 LOAD_GLOBAL              0 (importlib)
+         445           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('haystack')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         493          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         446          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:haystack:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         494         130 LOAD_CONST               3 (0)
+         447         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('HaystackInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.haystack)
                      136 IMPORT_FROM              6 (HaystackInstrumentor)
                      138 STORE_FAST               0 (HaystackInstrumentor)
                      140 POP_TOP
          
-         496         142 PUSH_NULL
+         449         142 PUSH_NULL
                      144 LOAD_FAST                0 (HaystackInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         497         162 LOAD_FAST                1 (instrumentor)
+         450         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         498         176 LOAD_FAST                1 (instrumentor)
+         451         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         499     >>  216 LOAD_CONST               5 (True)
+         452     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'haystack'
             'instrumentation:haystack:init'
             0
             ('HaystackInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.haystack', 'HaystackInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('HaystackInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_haystack_instrumentor'
-         firstlineno 491
+         firstlineno 444
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3136,72 +2774,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         502           0 RESUME                   0
+         455           0 RESUME                   0
          
-         503           2 LOAD_GLOBAL              0 (importlib)
+         456           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('langchain')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         504          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         457          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:langchain:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         505         130 LOAD_CONST               3 (0)
+         458         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('LangchainInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.langchain)
                      136 IMPORT_FROM              6 (LangchainInstrumentor)
                      138 STORE_FAST               0 (LangchainInstrumentor)
                      140 POP_TOP
          
-         507         142 PUSH_NULL
+         460         142 PUSH_NULL
                      144 LOAD_FAST                0 (LangchainInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         508         162 LOAD_FAST                1 (instrumentor)
+         461         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         509         176 LOAD_FAST                1 (instrumentor)
+         462         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         510     >>  216 LOAD_CONST               5 (True)
+         463     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'langchain'
             'instrumentation:langchain:init'
             0
             ('LangchainInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.langchain', 'LangchainInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('LangchainInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_langchain_instrumentor'
-         firstlineno 502
+         firstlineno 455
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3209,72 +2847,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         513           0 RESUME                   0
+         466           0 RESUME                   0
          
-         514           2 LOAD_GLOBAL              0 (importlib)
+         467           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('transformers')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         515          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         468          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:transformers:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         516         130 LOAD_CONST               3 (0)
+         469         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('TransformersInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.transformers)
                      136 IMPORT_FROM              6 (TransformersInstrumentor)
                      138 STORE_FAST               0 (TransformersInstrumentor)
                      140 POP_TOP
          
-         518         142 PUSH_NULL
+         471         142 PUSH_NULL
                      144 LOAD_FAST                0 (TransformersInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         519         162 LOAD_FAST                1 (instrumentor)
+         472         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         520         176 LOAD_FAST                1 (instrumentor)
+         473         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         521     >>  216 LOAD_CONST               5 (True)
+         474     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'transformers'
             'instrumentation:transformers:init'
             0
             ('TransformersInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.transformers', 'TransformersInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('TransformersInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_transformers_instrumentor'
-         firstlineno 513
+         firstlineno 466
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3282,322 +2920,322 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         524           0 RESUME                   0
+         477           0 RESUME                   0
          
-         525           2 LOAD_GLOBAL              0 (importlib)
+         478           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('llama_index')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         526          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         479          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:llamaindex:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         527         130 LOAD_CONST               3 (0)
+         480         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('LlamaIndexInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.llamaindex)
                      136 IMPORT_FROM              6 (LlamaIndexInstrumentor)
                      138 STORE_FAST               0 (LlamaIndexInstrumentor)
                      140 POP_TOP
          
-         529         142 PUSH_NULL
+         482         142 PUSH_NULL
                      144 LOAD_FAST                0 (LlamaIndexInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         530         162 LOAD_FAST                1 (instrumentor)
+         483         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         531         176 LOAD_FAST                1 (instrumentor)
+         484         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         532     >>  216 LOAD_CONST               5 (True)
+         485     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'llama_index'
             'instrumentation:llamaindex:init'
             0
             ('LlamaIndexInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.llamaindex', 'LlamaIndexInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('LlamaIndexInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_llama_index_instrumentor'
-         firstlineno 524
+         firstlineno 477
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             0000008132640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a050000000000000000731b7c01a0060000000000
             000000000000000000000000000000740e00000000000000000000ac04a6
             010000ab010000000000000000010064055300
-         535           0 RESUME                   0
+         488           0 RESUME                   0
          
-         536           2 LOAD_GLOBAL              0 (importlib)
+         489           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('requests')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    50 (to 164)
          
-         537          64 LOAD_CONST               2 (0)
+         490          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('RequestsInstrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.requests)
                       70 IMPORT_FROM              4 (RequestsInstrumentor)
                       72 STORE_FAST               0 (RequestsInstrumentor)
                       74 POP_TOP
          
-         539          76 PUSH_NULL
+         492          76 PUSH_NULL
                       78 LOAD_FAST                0 (RequestsInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         540          96 LOAD_FAST                1 (instrumentor)
+         493          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    27 (to 164)
          
-         541         110 LOAD_FAST                1 (instrumentor)
+         494         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 LOAD_GLOBAL             14 (EXCLUDED_URLS)
                      146 KW_NAMES                 4
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         542     >>  164 LOAD_CONST               5 (True)
+         495     >>  164 LOAD_CONST               5 (True)
                      166 RETURN_VALUE
          consts
             None
             'requests'
             0
             ('RequestsInstrumentor',)
             ('excluded_urls',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.requests', 'RequestsInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument', 'EXCLUDED_URLS')
          varnames   ('RequestsInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_requests_instrumentor'
-         firstlineno 535
+         firstlineno 488
          lnotab 0x02013e010c0214010e013601
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             0000008132640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a050000000000000000731b7c01a0060000000000
             000000000000000000000000000000740e00000000000000000000ac04a6
             010000ab010000000000000000010064055300
-         545           0 RESUME                   0
+         498           0 RESUME                   0
          
-         546           2 LOAD_GLOBAL              0 (importlib)
+         499           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('urllib3')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    50 (to 164)
          
-         547          64 LOAD_CONST               2 (0)
+         500          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('URLLib3Instrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.urllib3)
                       70 IMPORT_FROM              4 (URLLib3Instrumentor)
                       72 STORE_FAST               0 (URLLib3Instrumentor)
                       74 POP_TOP
          
-         549          76 PUSH_NULL
+         502          76 PUSH_NULL
                       78 LOAD_FAST                0 (URLLib3Instrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         550          96 LOAD_FAST                1 (instrumentor)
+         503          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    27 (to 164)
          
-         551         110 LOAD_FAST                1 (instrumentor)
+         504         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 LOAD_GLOBAL             14 (EXCLUDED_URLS)
                      146 KW_NAMES                 4
                      148 PRECALL                  1
                      152 CALL                     1
                      162 POP_TOP
          
-         552     >>  164 LOAD_CONST               5 (True)
+         505     >>  164 LOAD_CONST               5 (True)
                      166 RETURN_VALUE
          consts
             None
             'urllib3'
             0
             ('URLLib3Instrumentor',)
             ('excluded_urls',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.urllib3', 'URLLib3Instrumentor', 'is_instrumented_by_opentelemetry', 'instrument', 'EXCLUDED_URLS')
          varnames   ('URLLib3Instrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_urllib3_instrumentor'
-         firstlineno 545
+         firstlineno 498
          lnotab 0x02013e010c0214010e013601
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             000000812b640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a05000000000000000073147c01a0060000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             0064045300
-         555           0 RESUME                   0
+         508           0 RESUME                   0
          
-         556           2 LOAD_GLOBAL              0 (importlib)
+         509           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('sqlalchemy')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    43 (to 150)
          
-         557          64 LOAD_CONST               2 (0)
+         510          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('SQLAlchemyInstrumentor',))
                       68 IMPORT_NAME              3 (opentelemetry.instrumentation.sqlalchemy)
                       70 IMPORT_FROM              4 (SQLAlchemyInstrumentor)
                       72 STORE_FAST               0 (SQLAlchemyInstrumentor)
                       74 POP_TOP
          
-         559          76 PUSH_NULL
+         512          76 PUSH_NULL
                       78 LOAD_FAST                0 (SQLAlchemyInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         560          96 LOAD_FAST                1 (instrumentor)
+         513          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    20 (to 150)
          
-         561         110 LOAD_FAST                1 (instrumentor)
+         514         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 POP_TOP
          
-         562     >>  150 LOAD_CONST               4 (True)
+         515     >>  150 LOAD_CONST               4 (True)
                      152 RETURN_VALUE
          consts
             None
             'sqlalchemy'
             0
             ('SQLAlchemyInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'opentelemetry.instrumentation.sqlalchemy', 'SQLAlchemyInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('SQLAlchemyInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_pymysql_instrumentor'
-         firstlineno 555
+         firstlineno 508
          lnotab 0x02013e010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000006401a6010000ab010000000000
             000000812b640264036c036d047d00010002007c00a6000000ab00000000
             00000000007d017c016a05000000000000000073147c01a0060000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             0064045300
-         565           0 RESUME                   0
+         518           0 RESUME                   0
          
-         566           2 LOAD_GLOBAL              0 (importlib)
+         519           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('boto3')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    43 (to 150)
          
-         567          64 LOAD_CONST               2 (0)
+         520          64 LOAD_CONST               2 (0)
                       66 LOAD_CONST               3 (('BedrockInstrumentor',))
                       68 IMPORT_NAME              3 (syntrac_opentelemetry.instrumentation.bedrock)
                       70 IMPORT_FROM              4 (BedrockInstrumentor)
                       72 STORE_FAST               0 (BedrockInstrumentor)
                       74 POP_TOP
          
-         569          76 PUSH_NULL
+         522          76 PUSH_NULL
                       78 LOAD_FAST                0 (BedrockInstrumentor)
                       80 PRECALL                  0
                       84 CALL                     0
                       94 STORE_FAST               1 (instrumentor)
          
-         570          96 LOAD_FAST                1 (instrumentor)
+         523          96 LOAD_FAST                1 (instrumentor)
                       98 LOAD_ATTR                5 (is_instrumented_by_opentelemetry)
                      108 POP_JUMP_FORWARD_IF_TRUE    20 (to 150)
          
-         571         110 LOAD_FAST                1 (instrumentor)
+         524         110 LOAD_FAST                1 (instrumentor)
                      112 LOAD_METHOD              6 (instrument)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 POP_TOP
          
-         572     >>  150 LOAD_CONST               4 (True)
+         525     >>  150 LOAD_CONST               4 (True)
                      152 RETURN_VALUE
          consts
             None
             'boto3'
             0
             ('BedrockInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'syntrac_opentelemetry.instrumentation.bedrock', 'BedrockInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('BedrockInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_bedrock_instrumentor'
-         firstlineno 565
+         firstlineno 518
          lnotab 0x02013e010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3605,72 +3243,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         575           0 RESUME                   0
+         528           0 RESUME                   0
          
-         576           2 LOAD_GLOBAL              0 (importlib)
+         529           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('replicate')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         577          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         530          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:replicate:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         578         130 LOAD_CONST               3 (0)
+         531         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('ReplicateInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.replicate)
                      136 IMPORT_FROM              6 (ReplicateInstrumentor)
                      138 STORE_FAST               0 (ReplicateInstrumentor)
                      140 POP_TOP
          
-         580         142 PUSH_NULL
+         533         142 PUSH_NULL
                      144 LOAD_FAST                0 (ReplicateInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         581         162 LOAD_FAST                1 (instrumentor)
+         534         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         582         176 LOAD_FAST                1 (instrumentor)
+         535         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         583     >>  216 LOAD_CONST               5 (True)
+         536     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'replicate'
             'instrumentation:replicate:init'
             0
             ('ReplicateInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.replicate', 'ReplicateInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('ReplicateInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_replicate_instrumentor'
-         firstlineno 575
+         firstlineno 528
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3678,72 +3316,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         586           0 RESUME                   0
+         539           0 RESUME                   0
          
-         587           2 LOAD_GLOBAL              0 (importlib)
+         540           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('vertexai')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         588          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         541          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:vertexai:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         589         130 LOAD_CONST               3 (0)
+         542         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('VertexAIInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.vertexai)
                      136 IMPORT_FROM              6 (VertexAIInstrumentor)
                      138 STORE_FAST               0 (VertexAIInstrumentor)
                      140 POP_TOP
          
-         591         142 PUSH_NULL
+         544         142 PUSH_NULL
                      144 LOAD_FAST                0 (VertexAIInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         592         162 LOAD_FAST                1 (instrumentor)
+         545         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         593         176 LOAD_FAST                1 (instrumentor)
+         546         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         594     >>  216 LOAD_CONST               5 (True)
+         547     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'vertexai'
             'instrumentation:vertexai:init'
             0
             ('VertexAIInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.vertexai', 'VertexAIInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('VertexAIInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_vertexai_instrumentor'
-         firstlineno 586
+         firstlineno 539
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3751,72 +3389,72 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         597           0 RESUME                   0
+         550           0 RESUME                   0
          
-         598           2 LOAD_GLOBAL              0 (importlib)
+         551           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('ibm_watson_machine_learning')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         599          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         552          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:watsonx:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         600         130 LOAD_CONST               3 (0)
+         553         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('WatsonxInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.watsonx)
                      136 IMPORT_FROM              6 (WatsonxInstrumentor)
                      138 STORE_FAST               0 (WatsonxInstrumentor)
                      140 POP_TOP
          
-         602         142 PUSH_NULL
+         555         142 PUSH_NULL
                      144 LOAD_FAST                0 (WatsonxInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         603         162 LOAD_FAST                1 (instrumentor)
+         556         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         604         176 LOAD_FAST                1 (instrumentor)
+         557         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         605     >>  216 LOAD_CONST               5 (True)
+         558     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'ibm_watson_machine_learning'
             'instrumentation:watsonx:init'
             0
             ('WatsonxInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.watsonx', 'WatsonxInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('WatsonxInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_watsonx_instrumentor'
-         firstlineno 597
+         firstlineno 550
          lnotab 0x02013e0142010c0214010e012801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
@@ -3824,79 +3462,78 @@
             00000000000000000000000000000000006401a6010000ab010000000000
             000000814c740700000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006402a6010000ab
             0100000000000000000100640364046c056d067d00010002007c00a60000
             00ab0000000000000000007d017c016a07000000000000000073147c01a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000010064055300
-         608           0 RESUME                   0
+         561           0 RESUME                   0
          
-         609           2 LOAD_GLOBAL              0 (importlib)
+         562           2 LOAD_GLOBAL              0 (importlib)
                       14 LOAD_ATTR                1 (util)
                       24 LOAD_METHOD              2 (find_spec)
                       46 LOAD_CONST               1 ('weaviate')
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_NONE    76 (to 216)
          
-         610          64 LOAD_GLOBAL              7 (NULL + Telemetry)
+         563          64 LOAD_GLOBAL              7 (NULL + Telemetry)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 LOAD_METHOD              4 (capture)
                      112 LOAD_CONST               2 ('instrumentation:weaviate:init')
                      114 PRECALL                  1
                      118 CALL                     1
                      128 POP_TOP
          
-         611         130 LOAD_CONST               3 (0)
+         564         130 LOAD_CONST               3 (0)
                      132 LOAD_CONST               4 (('WeaviateInstrumentor',))
                      134 IMPORT_NAME              5 (syntrac_opentelemetry.instrumentation.weaviate)
                      136 IMPORT_FROM              6 (WeaviateInstrumentor)
                      138 STORE_FAST               0 (WeaviateInstrumentor)
                      140 POP_TOP
          
-         613         142 PUSH_NULL
+         566         142 PUSH_NULL
                      144 LOAD_FAST                0 (WeaviateInstrumentor)
                      146 PRECALL                  0
                      150 CALL                     0
                      160 STORE_FAST               1 (instrumentor)
          
-         614         162 LOAD_FAST                1 (instrumentor)
+         567         162 LOAD_FAST                1 (instrumentor)
                      164 LOAD_ATTR                7 (is_instrumented_by_opentelemetry)
                      174 POP_JUMP_FORWARD_IF_TRUE    20 (to 216)
          
-         615         176 LOAD_FAST                1 (instrumentor)
+         568         176 LOAD_FAST                1 (instrumentor)
                      178 LOAD_METHOD              8 (instrument)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_TOP
          
-         616     >>  216 LOAD_CONST               5 (True)
+         569     >>  216 LOAD_CONST               5 (True)
                      218 RETURN_VALUE
          consts
             None
             'weaviate'
             'instrumentation:weaviate:init'
             0
             ('WeaviateInstrumentor',)
             True
          names      ('importlib', 'util', 'find_spec', 'Telemetry', 'capture', 'syntrac_opentelemetry.instrumentation.weaviate', 'WeaviateInstrumentor', 'is_instrumented_by_opentelemetry', 'instrument')
          varnames   ('WeaviateInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_weaviate_instrumentor'
-         firstlineno 608
+         firstlineno 561
          lnotab 0x02013e0142010c0214010e012801
-   names      ('atexit', 'logging', 'os', 'importlib.util', 'importlib', 'colorama', 'Fore', 'opentelemetry', 'trace', 'syntrac.sdk.otlp.json.trace_exporter', 'OTLPSpanExporter', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.trace', 'TracerProvider', 'SpanProcessor', 'opentelemetry.propagators.textmap', 'TextMapPropagator', 'opentelemetry.propagate', 'set_global_textmap', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor', 'opentelemetry.trace', 'get_tracer_provider', 'ProxyTracerProvider', 'opentelemetry.context', 'get_value', 'attach', 'set_value', 'syntrac_opentelemetry.semconv.ai', 'SpanAttributes', 'syntrac.sdk', 'Telemetry', 'syntrac.sdk.instruments', 'Instruments', 'syntrac.sdk.tracing.content_allow_list', 'ContentAllowList', 'syntrac.sdk.utils', 'is_notebook', 'typing', 'Dict', 'Optional', 'Set', 'TRACER_NAME', 'EXCLUDED_URLS', 'object', 'TracerWrapper', 'str', 'set_correlation_id', 'dict', 'set_association_properties', 'set_workflow_name', 'int', 'set_prompt_tracing_context', 'bool', 'is_llm_span', 'init_spans_exporter', 'init_tracer_provider', 'init_instrumentations', 'init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_transformers_instrumentor', 'init_llama_index_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
+   names      ('atexit', 'logging', 'os', 'importlib.util', 'importlib', 'colorama', 'Fore', 'opentelemetry', 'trace', 'syntrac.sdk.otlp.json.trace_exporter', 'OTLPSpanExporter', 'typing', 'Any', 'Callable', 'Dict', 'Optional', 'Set', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.trace', 'TracerProvider', 'SpanProcessor', 'opentelemetry.propagators.textmap', 'TextMapPropagator', 'opentelemetry.propagate', 'set_global_textmap', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor', 'opentelemetry.trace', 'get_tracer_provider', 'ProxyTracerProvider', 'syntrac_opentelemetry.semconv.ai', 'SpanAttributes', 'syntrac.sdk', 'Telemetry', 'syntrac.sdk.instruments', 'Instruments', 'syntrac.sdk.tracing.content_allow_list', 'ContentAllowList', 'syntrac.sdk.utils', 'is_notebook', 'syntrac.sdk.tracing.context', 'set_override_enable_context_tracing', 'get_association_properties', 'syntrac.sdk.tracing.span_from_context', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'TRACER_NAME', 'EXCLUDED_URLS', 'object', 'TracerWrapper', 'bool', 'is_llm_span', 'str', 'init_spans_exporter', 'init_tracer_provider', 'init_instrumentations', 'init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_transformers_instrumentor', 'init_llama_index_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010801080108030c010c010c030c0110010c010c01140510
-      0114020c010c010c010c010c011402040104101c7f007f00331004100410
-      04020102ff020202fe020302fd020402fc020502fb020602fa080e0c0424
+      0x00ff020108010801080108030c010c010c031c010c0110010c010c0114
+      0510020c010c010c010c010c0110011002040104101c7f007f001d0c0424
       0410120615060b060b060b060b060a060b060b060b060b060b060a060a06
       0a060a060b060b060b
```

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.7/syntrac/sdk/tracing/tracing.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 
 
 from colorama import Fore
 from opentelemetry import trace
 from syntrac.sdk.otlp.json.trace_exporter import (
     OTLPSpanExporter
 )
+from typing import Any, Callable, Dict, Optional, Set
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider, SpanProcessor
 from opentelemetry.propagators.textmap import TextMapPropagator
 from opentelemetry.propagate import set_global_textmap
 from opentelemetry.sdk.trace.export import (
     SpanExporter,
     SimpleSpanProcessor,
     BatchSpanProcessor,
 )
 from opentelemetry.trace import get_tracer_provider, ProxyTracerProvider
-from opentelemetry.context import get_value, attach, set_value
 
 from syntrac_opentelemetry.semconv.ai import SpanAttributes
 from syntrac.sdk import Telemetry
 from syntrac.sdk.instruments import Instruments
 from syntrac.sdk.tracing.content_allow_list import ContentAllowList
 from syntrac.sdk.utils import is_notebook
-from typing import Dict, Optional, Set
+from syntrac.sdk.tracing.context import set_override_enable_context_tracing, get_association_properties
+from syntrac.sdk.tracing.span_from_context import set_workflow_name_from_context, set_prompt_attributes_from_context
 
 TRACER_NAME = "syntrac.tracer"
 EXCLUDED_URLS = """
     iam.cloud.ibm.com,
     dataplatform.cloud.ibm.com,
     ml.cloud.ibm.com,
     api.openai.com,
@@ -44,37 +45,43 @@
     googleapis.com,
     githubusercontent.com"""
 
 
 class TracerWrapper(object):
     resource_attributes: dict = {}
     enable_content_tracing: bool = True
-    endpoint: str = None
+    endpoint: Optional[str] = None
     headers: Dict[str, str] = {}
+    __resource: Resource
+    __tracer_provider: TracerProvider
+    __spans_processor: SpanProcessor
+    __spans_processor_original_on_start: Optional[Callable] = None
+    __spans_exporter: SpanExporter
+    __content_allow_list: ContentAllowList
 
     def __new__(
         cls,
         disable_batch=False,
-        processor: SpanProcessor = None,
-        propagator: TextMapPropagator = None,
-        exporter: SpanExporter = None,
+        processor: Optional[SpanProcessor] = None,
+        propagator: Optional[TextMapPropagator] = None,
+        exporter: Optional[SpanExporter] = None,
         instruments: Optional[Set[Instruments]] = None,
     ) -> "TracerWrapper":
         if not hasattr(cls, "instance"):
             obj = cls.instance = super(TracerWrapper, cls).__new__(cls)
             if not TracerWrapper.endpoint:
                 return obj
 
             obj.__resource = Resource(attributes=TracerWrapper.resource_attributes)
-            obj.__tracer_provider: TracerProvider = init_tracer_provider(
+            obj.__tracer_provider = init_tracer_provider(
                 resource=obj.__resource
             )
             if processor:
                 Telemetry().capture("tracer:init", {"processor": "custom"})
-                obj.__spans_processor: SpanProcessor = processor
+                obj.__spans_processor = processor
                 obj.__spans_processor_original_on_start = processor.on_start
             else:
                 if exporter:
                     Telemetry().capture(
                         "tracer:init",
                         {
                             "exporter": "custom",
@@ -86,27 +93,27 @@
                         "tracer:init",
                         {
                             "exporter": TracerWrapper.endpoint,
                             "processor": "simple" if disable_batch else "batch",
                         },
                     )
 
-                obj.__spans_exporter: SpanExporter = (
+                obj.__spans_exporter = (
                     exporter
                     if exporter
                     else init_spans_exporter(
                         TracerWrapper.endpoint, TracerWrapper.headers
                     )
                 )
                 if disable_batch or is_notebook():
-                    obj.__spans_processor: SpanProcessor = SimpleSpanProcessor(
+                    obj.__spans_processor = SimpleSpanProcessor(
                         obj.__spans_exporter
                     )
                 else:
-                    obj.__spans_processor: SpanProcessor = BatchSpanProcessor(
+                    obj.__spans_processor = BatchSpanProcessor(
                         obj.__spans_exporter
                     )
                 obj.__spans_processor_original_on_start = None
 
             obj.__spans_processor.on_start = obj._span_processor_on_start
             obj.__tracer_provider.add_span_processor(obj.__spans_processor)
 
@@ -263,58 +270,30 @@
 
         return cls.instance
 
     def exit_handler(self):
         self.flush()
 
     def _span_processor_on_start(self, span, parent_context):
-        workflow_name = get_value("workflow_name")
-        if workflow_name is not None:
-            span.set_attribute(SpanAttributes.SYNTRAC_WORKFLOW_NAME, workflow_name)
-
-        correlation_id = get_value("correlation_id")
-        if correlation_id is not None:
-            span.set_attribute(SpanAttributes.SYNTRAC_CORRELATION_ID, correlation_id)
+        set_workflow_name_from_context(span)
 
-        association_properties = get_value("association_properties")
+        association_properties: Any = get_association_properties()
         if association_properties is not None:
             for key, value in association_properties.items():
                 span.set_attribute(
                     f"{SpanAttributes.SYNTRAC_ASSOCIATION_PROPERTIES}.{key}", value
                 )
 
             if not self.enable_content_tracing:
                 if self.__content_allow_list.is_allowed(association_properties):
-                    attach(set_value("override_enable_content_tracing", True))
+                    set_override_enable_context_tracing(True)
                 else:
-                    attach(set_value("override_enable_content_tracing", False))
+                    set_override_enable_context_tracing(False)
 
-        if is_llm_span(span):
-            prompt_key = get_value("prompt_key")
-            if prompt_key is not None:
-                span.set_attribute("syntrac.prompt.key", prompt_key)
-
-            prompt_version = get_value("prompt_version")
-            if prompt_version is not None:
-                span.set_attribute("syntrac.prompt.version", prompt_version)
-
-            prompt_version_name = get_value("prompt_version_name")
-            if prompt_version_name is not None:
-                span.set_attribute("syntrac.prompt.version_name", prompt_version_name)
-
-            prompt_version_hash = get_value("prompt_version_hash")
-            if prompt_version_hash is not None:
-                span.set_attribute("syntrac.prompt.version_hash", prompt_version_hash)
-
-            prompt_template_variables = get_value("prompt_template_variables")
-            if prompt_version_hash is not None:
-                for key, value in prompt_template_variables.items():
-                    span.set_attribute(
-                        f"syntrac.prompt.template_variables.{key}", value
-                    )
+        set_prompt_attributes_from_context(span)
 
         # Call original on_start method if it exists in custom processor
         if self.__spans_processor_original_on_start:
             self.__spans_processor_original_on_start(span, parent_context)
 
     @staticmethod
     def set_static_params(
@@ -346,50 +325,24 @@
     def flush(self):
         self.__spans_processor.force_flush()
 
     def get_tracer(self):
         return self.__tracer_provider.get_tracer(TRACER_NAME)
 
 
-def set_correlation_id(correlation_id: str) -> None:
-    attach(set_value("correlation_id", correlation_id))
-
-
-def set_association_properties(properties: dict) -> None:
-    attach(set_value("association_properties", properties))
-
-
-def set_workflow_name(workflow_name: str) -> None:
-    attach(set_value("workflow_name", workflow_name))
-
-
-def set_prompt_tracing_context(
-    key: str,
-    version: int,
-    version_name: str,
-    version_hash: str,
-    template_variables: dict,
-) -> None:
-    attach(set_value("prompt_key", key))
-    attach(set_value("prompt_version", version))
-    attach(set_value("prompt_version_name", version_name))
-    attach(set_value("prompt_version_hash", version_hash))
-    attach(set_value("prompt_template_variables", template_variables))
-
-
 def is_llm_span(span) -> bool:
     return span.attributes.get(SpanAttributes.LLM_REQUEST_TYPE) is not None
 
 
 def init_spans_exporter(api_endpoint: str, headers: Dict[str, str]) -> SpanExporter:
     return OTLPSpanExporter(endpoint=f"{api_endpoint}/v1/traces", headers=headers)
 
 
 def init_tracer_provider(resource: Resource) -> TracerProvider:
-    provider: TracerProvider = None
+    provider: Optional[TracerProvider] = None
     default_provider: TracerProvider = get_tracer_provider()
 
     if isinstance(default_provider, ProxyTracerProvider):
         provider = TracerProvider(resource=resource)
         trace.set_tracer_provider(provider)
     elif not hasattr(default_provider, "add_span_processor"):
         logging.error(
```

### Comparing `syntrac_sdk-0.0.6/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.7/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.6/PKG-INFO` & `syntrac_sdk-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Syntrac Software Development Kit (SDK) for Python
 Home-page: https://github.com/syntracAI/syntrac
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,15 +25,15 @@
 Requires-Dist: posthog (>=3.0.2,<4.0.0)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: syntrac-opentelemetry-instrumentation-anthropic (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-bedrock (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-chromadb (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-cohere (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-haystack (==0.0.2)
-Requires-Dist: syntrac-opentelemetry-instrumentation-langchain (==0.0.3)
+Requires-Dist: syntrac-opentelemetry-instrumentation-langchain (==0.0.4)
 Requires-Dist: syntrac-opentelemetry-instrumentation-llamaindex (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-openai (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-pinecone (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-qdrant (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-replicate (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-transformers (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-vertexai (==0.0.2)
```

