# Comparing `tmp/onnxscript-0.1.0.dev20240510.tar.gz` & `tmp/onnxscript-0.1.0.dev20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240510.tar", last modified: Fri May 10 00:01:42 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240511.tar", last modified: Sat May 11 00:01:45 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240510.tar` & `onnxscript-0.1.0.dev20240511.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.576414 onnxscript-0.1.0.dev20240510/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-10 00:01:42.576414 onnxscript-0.1.0.dev20240510/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.508414 onnxscript-0.1.0.dev20240510/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.512414 onnxscript-0.1.0.dev20240510/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.516414 onnxscript-0.1.0.dev20240510/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.516414 onnxscript-0.1.0.dev20240510/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.516414 onnxscript-0.1.0.dev20240510/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.496413 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.516414 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.540414 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.496413 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.496413 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.540414 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.544414 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.544414 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.548414 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.556414 onnxscript-0.1.0.dev20240510/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2619 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    92963 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20889 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/_type_casting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    55917 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.556414 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.564414 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.568414 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.572414 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6718 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.572414 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.572414 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/bfloat16_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.572414 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.572414 onnxscript-0.1.0.dev20240510/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.576414 onnxscript-0.1.0.dev20240510/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 00:01:42.576414 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-10 00:01:42.000000 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-10 00:01:42.000000 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-10 00:01:42.000000 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-10 00:01:42.000000 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-10 00:01:42.000000 onnxscript-0.1.0.dev20240510/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-10 00:01:42.576414 onnxscript-0.1.0.dev20240510/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-10 00:00:57.000000 onnxscript-0.1.0.dev20240510/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.681226 onnxscript-0.1.0.dev20240511/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.685226 onnxscript-0.1.0.dev20240511/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.685226 onnxscript-0.1.0.dev20240511/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.685226 onnxscript-0.1.0.dev20240511/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.689226 onnxscript-0.1.0.dev20240511/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.673225 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.689226 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.709227 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.673225 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.673225 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.709227 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.709227 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.713227 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.717228 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.721228 onnxscript-0.1.0.dev20240511/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2702 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    92963 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20889 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/_type_casting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58627 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.721228 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.733229 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.737229 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.741229 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6735 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26344 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.741229 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.741229 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/bfloat16_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5171 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40099 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-11 00:01:45.000000 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-11 00:01:45.000000 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-11 00:01:45.000000 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-11 00:01:45.000000 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-11 00:01:45.000000 onnxscript-0.1.0.dev20240511/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-11 00:01:45.745229 onnxscript-0.1.0.dev20240511/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-11 00:00:59.000000 onnxscript-0.1.0.dev20240511/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240510/LICENSE` & `onnxscript-0.1.0.dev20240511/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/PKG-INFO` & `onnxscript-0.1.0.dev20240511/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240510
+Version: 0.1.0.dev20240511
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b4dd7774f166e46984aebc6d3626cd5edae3dcd5
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/32bcd064d0fd94ee40e358b419589388d7ffe360
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240510/README.md` & `onnxscript-0.1.0.dev20240511/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240511/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240511/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240511/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240511/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240511/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240511/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     # Enums
     "AttributeType",
     "DataType",
     # Types
     "OperatorIdentifier",
     # Protobuf compatible types
     "TensorProtoTensor",
+    # Conversion functions
+    "from_proto",
+    "to_proto",
 ]
 
 from onnxscript.ir import serde
 from onnxscript.ir._core import (
     Attr,
     AttrFloat32,
     AttrFloat32s,
@@ -122,8 +125,8 @@
     ShapeProtocol,
     SparseTensorProtocol,
     SymbolicDimProtocol,
     TensorProtocol,
     TypeProtocol,
     ValueProtocol,
 )
-from onnxscript.ir.serde import TensorProtoTensor
+from onnxscript.ir.serde import TensorProtoTensor, from_proto, to_proto
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/_type_casting.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240511/onnxscript/ir/serde.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 
 from __future__ import annotations
 
 __all__ = [
     # Tensors
     "TensorProtoTensor",
     # Deserialization
+    "from_proto",
     "deserialize_attribute",
     "deserialize_function",
     "deserialize_graph",
     "deserialize_model",
     "deserialize_node",
     "deserialize_opset_import",
     "deserialize_tensor",
     "deserialize_type_proto_for_shape",
     "deserialize_type_proto_for_type",
     "deserialize_value_info_proto",
     # Serialization
+    "to_proto",
     "serialize_attribute_into",
     "serialize_attribute",
     "serialize_dimension_into",
     "serialize_function_into",
     "serialize_function",
     "serialize_graph_into",
     "serialize_graph",
@@ -85,14 +87,83 @@
 def _unflatten_complex(
     array: npt.NDArray[np.float32 | np.float64],
 ) -> npt.NDArray[np.complex64 | np.complex128]:
     """Convert the real representation of a complex dtype to the complex dtype."""
     return array[::2] + 1j * array[1::2]
 
 
+def from_proto(
+    proto: onnx.ModelProto
+    | onnx.GraphProto
+    | onnx.NodeProto
+    | onnx.TensorProto
+    | onnx.AttributeProto
+    | onnx.ValueInfoProto
+    | onnx.TypeProto,
+) -> Any:
+    """Deserialize an ONNX proto message to an IR object."""
+    if isinstance(proto, onnx.ModelProto):
+        return deserialize_model(proto)
+    if isinstance(proto, onnx.GraphProto):
+        return deserialize_graph(proto)
+    if isinstance(proto, onnx.NodeProto):
+        return deserialize_node(proto)
+    if isinstance(proto, onnx.TensorProto):
+        return deserialize_tensor(proto)
+    if isinstance(proto, onnx.AttributeProto):
+        return deserialize_attribute(proto)
+    if isinstance(proto, onnx.ValueInfoProto):
+        return deserialize_value_info_proto(proto, None)
+    if isinstance(proto, onnx.TypeProto):
+        return _core.TypeAndShape(
+            deserialize_type_proto_for_type(proto),
+            deserialize_type_proto_for_shape(proto),
+        )
+    raise NotImplementedError(
+        f"Deserialization of {type(proto)} in from_proto is not implemented. "
+        "Use a specific ir.serde.deserialize* function instead."
+    )
+
+
+def to_proto(
+    ir_object: _protocols.ModelProtocol
+    | _protocols.GraphProtocol
+    | _protocols.NodeProtocol
+    | _protocols.ValueProtocol
+    | _protocols.AttributeProtocol
+    | _protocols.ReferenceAttributeProtocol
+    | _protocols.TensorProtocol
+    | onnx.TypeProto
+    | _protocols.GraphViewProtocol,
+) -> Any:
+    """Serialize an IR object to a proto."""
+    if isinstance(ir_object, _protocols.ModelProtocol):
+        return serialize_model(ir_object)
+    if isinstance(ir_object, _protocols.GraphProtocol):
+        return serialize_graph(ir_object)
+    if isinstance(ir_object, _protocols.NodeProtocol):
+        return serialize_node(ir_object)
+    if isinstance(ir_object, _protocols.TensorProtocol):
+        return serialize_tensor(ir_object)
+    if isinstance(ir_object, _protocols.ValueProtocol):
+        return serialize_value(ir_object)
+    if isinstance(ir_object, _protocols.AttributeProtocol):
+        return serialize_attribute(ir_object)
+    if isinstance(ir_object, _protocols.ReferenceAttributeProtocol):
+        return serialize_reference_attribute_into(onnx.AttributeProto(), ir_object)
+    if isinstance(ir_object, _protocols.TypeProtocol):
+        return serialize_type_into(onnx.TypeProto(), ir_object)
+    if isinstance(ir_object, _protocols.GraphViewProtocol):
+        return serialize_graph(ir_object)
+    raise NotImplementedError(
+        f"Serialization of {type(ir_object)} in to_proto is not implemented. "
+        "Use a specific ir.serde.serialize* function instead."
+    )
+
+
 class TensorProtoTensor(_core.TensorBase):  # pylint: disable=too-many-ancestors
     """A tensor initialized from a tensor proto."""
 
     def __init__(self, proto: onnx.TensorProto) -> None:
         self._proto = proto
         self._metadata_props: dict[str, str] | None = deserialize_metadata_props(
             proto.metadata_props
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240511/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/main.py` & `onnxscript-0.1.0.dev20240511/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240511/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240511/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 # condition to check if we need to replace the pattern
-def check_if_not_need_reshape(input_a, input_b, shape_c, **_) -> bool:
+def check_if_not_need_reshape(context, input_a, input_b, shape_c, **_) -> bool:
     """If matmul broadcasting is enough, then we don't need the reshapes.
 
     To validate this, we need to check the following:
     1. Input shapes check: input_a and input_b should be broadcastable
     2. Output shape check: shape_c should be the same as the output shape from the matmul(input_a, input_b)
 
     If the above are true, then we don't need the reshapes.
@@ -122,15 +122,15 @@
             broadcast_matmul_output_shape,
         )
         return False
 
     return True
 
 
-def two_reshapes_matmul_reshape_pattern(input_a, input_b, shape_a, shape_b, shape_c):
+def two_reshapes_matmul_reshape_pattern(op, input_a, input_b, shape_a, shape_b, shape_c):
     # TODO: Modified from `value_ints` to `value` to match pattern in benchmark models.
     # This implementation misses pattern of Constants with `value_ints` attribute.
     # See more at https://github.com/microsoft/onnx-rewriter/issues/191.
     # A better solution is to improve pattern matching and avoid depending on writing
     # Constants in pattern. See https://github.com/microsoft/onnx-rewriter/issues/192.
     reshape_a = op.Reshape(input_a, shape_a)
     reshape_b = op.Reshape(input_b, shape_b)
@@ -138,15 +138,15 @@
     return op.Reshape(matmul, shape_c)
 
 
 def matmul(op, input_a, input_b, **_):
     return op.MatMul(input_a, input_b)
 
 
-def one_reshape_matmul_reshape_pattern(input_a, input_b, shape_a, shape_c):
+def one_reshape_matmul_reshape_pattern(op, input_a, input_b, shape_a, shape_c):
     reshape_a = op.Reshape(input_a, shape_a)
     matmul = op.MatMul(reshape_a, input_b)
     return op.Reshape(matmul, shape_c)
 
 
 # Register the rewrite rules
 two_reshapes_matmul_reshape_rule = pattern.RewriteRule(
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from onnxscript import ir
 from onnxscript.rewriter import pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
-def cast_constant_of_shape(shape, scalar, dtype):
+def cast_constant_of_shape(op, shape, scalar, dtype):
     constant = op.ConstantOfShape(shape, value=scalar)
     return op.Cast(constant, to=dtype)
 
 
 def fused_cast_constant_of_shape(op, shape: ir.Value, scalar: ir.Attr, dtype: ir.Attr, **_):
     # Cast scalar (a TensorProto attribute) to the specified dtype
     scalar_value = scalar.value.numpy().item()
     cast_value = onnx.helper.make_tensor("value", dtype.value, (1,), [scalar_value])
     return op.ConstantOfShape(shape, value=cast_value)
 
 
-def cast_constant_of_shape_without_value(shape, dtype):
+def cast_constant_of_shape_without_value(op, shape, dtype):
     constant = op.ConstantOfShape(shape)
     return op.Cast(constant, to=dtype)
 
 
 def fused_cast_constant_of_shape_without_value(op, shape, dtype, **_):
     zero = onnx.helper.make_tensor("value", dtype.value, (1,), [0])
     return op.ConstantOfShape(shape, value=zero)
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from onnxscript.rewriter import pattern
 from onnxscript.rewriter.broadcast_to_matmul import check_if_not_need_reshape
 
 op = pattern.onnxop
 
 
 # Pattern to match against
-def reshape_gemm_reshape_pattern(input_a, input_b, input_c, shape_a, shape_c):
+def reshape_gemm_reshape_pattern(op, input_a, input_b, input_c, shape_a, shape_c):
     reshape_a = op.Reshape(input_a, shape_a)
     # TODO: Temporary workaround to support benchmodels.
     # Tracked by https://github.com/microsoft/onnx-rewriter/issues/197.
     gemm = op.Gemm(reshape_a, input_b, input_c, alpha=1.0, beta=1.0)
     return op.Reshape(gemm, shape_c)
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/generic_pattern.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,184 +9,142 @@
 import onnxscript.rewriter.pattern as orp
 from onnxscript import ir
 
 
 class PatternMatchResult:
     """Stores information about a match if a match was successful.
 
-    * pattern: the instance of :class:`GenericPattern` which found this result
-    * model_nodes: matched nodes coming from the model
-    * pattern_nodes: corresponding nodes coming from the pattern
-    * pattern_input_names: input names of the pattern
-    * pattern_ouptut_names: output names of the pattern
+    * pattern: the GraphPattern which found this result
+    * model_nodes: the graph nodes that matched the pattern
+    * matched_pattern_to_model_value: a mapping from ValuePattern to ir.Value
     * kwargs: additional attributes the user may add through the method
         :meth:`PatternMatchResult.add_kwargs`
-
-    The class creates one attributes `matched_pattern_to_model_name`,
-    which maps every result name from the pattern to the corresponding
-    result name in the model.
     """
 
     def __init__(
         self,
-        pattern: GenericPattern,
+        pattern: orp.GraphPattern,
         model_nodes: Sequence[ir.Node],
-        pattern_nodes: Sequence[ir.Node],
-        pattern_inputs: Sequence[ir.Value],
-        pattern_outputs: Sequence[ir.Value],
     ):
+        pattern_nodes: list[orp.NodePattern] = list(pattern)
         assert len(model_nodes) == len(pattern_nodes)
         self.pattern = pattern
         self.model_nodes = model_nodes
-        self.pattern_nodes = pattern_nodes
-        self.pattern_inputs = pattern_inputs
-        self.pattern_outputs = pattern_outputs
         self.kwargs: dict[str, Any] = {}
+        self.matched_pattern_to_model_value: dict[orp.ValuePattern, ir.Value] = {}
 
-        matched_pattern_to_model_value: dict[str, ir.Value] = {}
-        for gn, pn in zip(model_nodes, pattern_nodes):
+        for graph_node, pattern_node in zip(model_nodes, pattern_nodes):
             assert (
-                gn.op_type == pn.op_type
-            ), f"Unexpected type mismatch {gn.op_type!r} != {pn.op_type!r}"
-            assert len(gn.inputs) == len(
-                pn.inputs
-            ), f"Unexpected number of inputs for type {gn.op_type}"
-            for a, b in zip(gn.inputs, pn.inputs):
+                graph_node.op_identifier() == pattern_node.op_identifier()
+            ), f"Unexpected type mismatch {graph_node.op_identifier()!r} != {pattern_node.op_identifier()!r}"
+            assert len(graph_node.inputs) == len(
+                pattern_node.inputs
+            ), f"Unexpected number of inputs for type {graph_node.op_identifier()}"
+            for a, b in zip(graph_node.inputs, pattern_node.inputs):
                 if b is None:
                     # optional input or not an interesting input
                     continue
-                b_name = b.name
-                assert b_name is not None
-                if b_name in matched_pattern_to_model_value:
-                    assert matched_pattern_to_model_value[b_name] == a, (
-                        f"Ambiguities, pattern input '{b_name}' means "
-                        f"'{a!r}' or '{matched_pattern_to_model_value[b_name]}'"
-                    )
-                else:
-                    matched_pattern_to_model_value[b_name] = a
-
-            assert len(gn.outputs) == len(
-                pn.outputs
-            ), f"Unexpected number of outputs for type {gn.op_type}"
-            for a, b in zip(gn.outputs, pn.outputs):
-                b_name = b.name
-                assert b_name is not None
-                if b_name in matched_pattern_to_model_value:
-                    assert matched_pattern_to_model_value[b_name] == a, (
-                        f"Ambiguities, pattern output {b_name!r} means "
-                        f"{a!r} or {matched_pattern_to_model_value[b_name]}"
-                    )
-                else:
-                    matched_pattern_to_model_value[b_name] = a
+                self._bind(b, a)
 
-        self.matched_pattern_to_model_value = matched_pattern_to_model_value
+            assert len(graph_node.outputs) == len(
+                pattern_node.outputs
+            ), f"Unexpected number of outputs for type {graph_node.op_identifier()}"
+            for a, b in zip(graph_node.outputs, pattern_node.outputs):
+                self._bind(b, a)
+
+    def _bind(self, value_pattern: orp.ValuePattern, value: ir.Value) -> None:
+        map = self.matched_pattern_to_model_value
+        if value_pattern in map:
+            assert map[value_pattern] == value, (
+                f"Ambiguities, pattern output {value_pattern!r} means "
+                f"{value!r} or {map[value_pattern]}"
+            )
+        else:
+            map[value_pattern] = value
 
     def add_kwargs(self, name: str, value: Any):
         """Adds an attribute, it can be done when the match is being validated,
         this attribute can be used when building the replacement nodes.
         """
         self.kwargs[name] = value
 
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__name__}([{self.pattern.__class__.__name__}], "
-            f"... {len(self.model_nodes)} nodes ..., {self.pattern_inputs}, "
-            f"{self.pattern_outputs})"
+            f"PatternMatchResult: {len(self.model_nodes)} nodes ..., {self.pattern.inputs}, "
+            f"{self.pattern.outputs})"
         )
 
 
 def _to_match_result(pmr: PatternMatchResult) -> orp.MatchResult:
     """Converts a PatternMatchResult into a MatchResult.
 
     TODO: This is a temporary hack until MatchResult and PatternMatchResult are unified.
     """
     result = orp.MatchResult(success=True)
     result.nodes.extend(pmr.model_nodes)
     for var, val in pmr.matched_pattern_to_model_value.items():
-        result.bind(var, val)
-    result.outputs.extend(
-        [pmr.matched_pattern_to_model_value[v.name] for v in pmr.pattern_outputs]
-    )
+        if var.name is not None:
+            result.bind(var.name, val)
+    result.outputs.extend([pmr.matched_pattern_to_model_value[v] for v in pmr.pattern.outputs])
     return result
 
 
-class GenericRewriteRule(orp.RewriteRule):
-    """
-    Defines a rewriting rule.
-
-        pattern: a pattern defines by :class:`GenericPattern`.
-    """
+def _value_to_str(value: ir.Value | orp.ValuePattern) -> str:
+    return value.name if value.name is not None else "anonymous:" + str(id(value))
 
-    def __init__(self, pattern: GenericPattern):
-        self.pattern = pattern
-        self.verbose: int = 0  # TODO: remove this
-
-    def matches(self, node: ir.Node, model: ir.Model) -> orp.MatchResult:
-        del model
-        del node
-        raise RuntimeError(f"This pattern {self} is meant to replace not to only match.")
 
-    def try_rewrite(
-        self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
-    ) -> orp.ReplacementSubgraph | None:
-        """See :meth:`RewriteRule.try_rewrite`."""
-
-        pattern_match_result = self.pattern.match(model.graph, node)
-        if pattern_match_result:
-            match_result = _to_match_result(pattern_match_result)
-            context = None  # TODO: create a context
-            if not self.pattern.validate_mapping(context, **match_result.bindings):
-                pattern_match_result._hint(
-                    "validate_mapping", "The pattern was rejected by the validation function."
-                )
-                return None
+def _opt_value_to_str(value: ir.Value | orp.ValuePattern | None) -> str:
+    return _value_to_str(value) if value is not None else "None"
 
-            return self.pattern.apply(model, match_result, verbose=self.verbose)
-        return None
 
-    def count_matches(self, model: ir.Model, *, commute: bool = False) -> int:
-        """See :meth:`RewriteRule.count_matches`."""
-        raise NotImplementedError("Not supported yet.")
+def _node_to_str(node: ir.Node | orp.NodePattern) -> str:
+    inputs = ", ".join(_opt_value_to_str(input) for input in node.inputs)
+    outputs = ", ".join(_opt_value_to_str(output) for output in node.outputs)
+    op_type = node.op_type
+    domain = str(node.domain)
+    qualified_op = f"{domain}.{op_type}" if domain else op_type
+    return f"{outputs} = {qualified_op}({inputs})"
 
-    def commute(self) -> list[orp.RewriteRule]:
-        """See :meth:`RewriteRule.commute`."""
-        raise RuntimeError("Not supported (yet?). It could lead to many patterns.")
 
-    def apply_to_model(self, model: ir.Model, *, commute: bool = False) -> int:
-        """See :meth:`RewriteRule.apply_to_model`."""
-        return orp.RewriteRuleSet([self], commute=commute).apply_to_model(model)
+# def _pattern_node_to_str(node: orp.NodePattern) -> str:
+#     inputs = ", ".join(_opt_value_to_str(input) for input in node.inputs)
+#     outputs = ", ".join(_opt_value_to_str(output) for output in node.outputs)
+#     return f"{outputs} = {node.op_type}({inputs})"
 
 
-class GenericPattern:
+class GenericPatternMatcher(orp.PatternMatcher):
     """
     Implements a pattern optimization for quick experimentation.
 
     Current limitation:
 
     * The current implementation does match on domain name (easy fix).
     * It does not compares attributes either (easy fix as well).
     """
 
-    def __init__(self, verbose: int = 0):
-        self.verbose = verbose
-        self._cache: dict = {}
+    def __init__(self, pattern: orp.GraphPattern) -> None:
+        super().__init__(pattern)
 
     def enumerate_matches(
-        self, graph: ir.Graph | ir.GraphView, node: ir.Node | None = None
+        self,
+        model: ir.Model,
+        graph_or_function: ir.Graph | ir.Function,
+        node: ir.Node | None = None,
+        verbose: int = 0,
     ) -> Iterator:
         """Enumerates all the matches."""
         if node is None:
             matched = []
-            for node in graph:
-                res = self.match(graph, node)
+            for node in graph_or_function:
+                res = self.match(model, graph_or_function, node, verbose=verbose)
                 if res:
                     matched.append(res)
                     yield res
         else:
-            res = self.match(graph, node)
+            res = self.match(model, graph_or_function, node, verbose=verbose)
             if res:
                 yield res
 
     def none(
         self,
         node: ir.Node | None = None,
         lineno: int | None = None,
@@ -239,37 +197,38 @@
                 if hasattr(self, "_debug"):
                     msg2 = self._debug_print()
                     if msg2:
                         msg2 = f"\n{textwrap.indent(msg2, '    ')}"
                 else:
                     msg2 = ""
                 print(
-                    f"[{self.__class__.__name__}.match] NONE - line: {lineno}:"
+                    f"[{self.__class__.__name__}.match] Match failed at line: {lineno}:"
                     f"{os.path.split(self.__class__.__module__)[-1]}, "
                     f"op_type={node.op_type}{msg}{msg2}"
                 )
+        return None
 
-    def print_match(self, n1: ir.Node, n2: ir.Node) -> str:
-        s1 = f"{n1.op_type}({n1.inputs})"
-        s2 = f"{n2.op_type}({n2.inputs})"
-        return f"match {s1} with {s2} (pattern)"
+    def print_match(self, graph_node: ir.Node, pattern_node: orp.NodePattern) -> str:
+        s1 = _node_to_str(graph_node)
+        s2 = _node_to_str(pattern_node)
+        return f"match {s1} with pattern: {s2}"
 
     def _debug_print(self) -> str:
         if not hasattr(self, "_debug"):
             return ""
 
         def _s(s: str) -> str:
             if len(s) <= 30:
                 return s
             return f"{s[:15]}...{s[-15:]}"
 
         def _p(n: ir.Node, full: bool = False) -> str:
             if full:
                 return str(n)
-            return f"{n.op_type}({', '.join([str(input) for input in n.inputs])})"
+            return _node_to_str(n)
 
         rows = []
         for k, v in sorted(self._debug.items()):
             if k == "stack":
                 rows.append(f"len({k})={len(v)}:{v}")  # type: ignore[arg-type]
                 continue
             if k == "iteration":
@@ -281,14 +240,16 @@
                     rows.append(
                         f"  {_p(pattern_node)} ~ {_p(graph_node)} [{id(pattern_node)}-{id(graph_node)}]"
                     )
                 continue
             if k == "hint":
                 rows.append(f"--hint--: {v[0]}")  # type: ignore[arg-type]
                 for i in v[1:]:
+                    if isinstance(i, str):
+                        rows.append("  " + i)
                     if isinstance(i, ir.Node):
                         rows.append("  " + _p(i, full=True))
                 continue
             if k in {"node", "pattern", "pattern_node", "pattern_nodes"}:
                 continue
             rows.append(f"-- not shown {k}")
 
@@ -296,25 +257,25 @@
 
     def _hint(self, *args: Any) -> None:
         """Add debugging information to help users."""
         self._debug["hint"] = args
 
     def _match_backward(
         self,
-        node: ir.Node,
-        matched: dict[ir.Node, ir.Node],
-        stack: list[ir.Node],
+        starting_node: ir.Node,
+        matched: dict[orp.NodePattern, ir.Node],
+        stack: list[orp.NodePattern],
         graph_node: ir.Node,
-        pattern_node: ir.Node,
+        pattern_node: orp.NodePattern,
     ) -> int | None:
         """
         Matches backward.
 
         Args:
-            node: root node (the node the matched begain with, used only for debugging)
+            starting_node: root node (the node the matched begain with, used only for debugging)
             matched: nodes of the pattern matched as already matched
             stack: next node to look into
             graph_node: node coming from the graph
             pattern_node: node coming from the pattern
 
         Returns:
             number of matched nodes, None or False to indicate a failed match
@@ -327,57 +288,60 @@
             self._hint(
                 "BACKWARD: not the same number of inputs",
                 "-- pattern",
                 pattern_node,
                 "-- model",
                 graph_node,
             )
-            return self.none(node, inspect.currentframe().f_lineno)
-        for i, pi in zip(graph_node.inputs, pattern_node.inputs):
-            ppred = pi.producer()
-            if ppred is None:
-                # ppred is None means the pattern ends here.
+            return self.none(starting_node, inspect.currentframe().f_lineno)
+        for graph_value, pattern_value in zip(graph_node.inputs, pattern_node.inputs):
+            # TODO(rama): Handle constant-pattern
+            pattern_pred = pattern_value.producer()
+            if pattern_pred is None:
+                # pattern_pred is None means the pattern ends here.
                 continue
-            pred = i.producer()
-            if pred is None:
+            graph_pred = graph_value.producer()
+            if graph_pred is None:
                 # No node in the graph.
-                return self.none(node, inspect.currentframe().f_lineno)
-            if pred.op_type != ppred.op_type:
+                return self.none(starting_node, inspect.currentframe().f_lineno)
+            if graph_pred.op_identifier() != pattern_pred.op_identifier():
                 self._hint(
                     "BACKWARD: different node types",
                     "--pattern",
-                    ppred,
+                    _node_to_str(pattern_pred),
                     "-- model",
-                    pred,
+                    _node_to_str(graph_pred),
                 )
-                return self.none(node, inspect.currentframe().f_lineno)
+                return self.none(starting_node, inspect.currentframe().f_lineno)
             # matching backward
-            if ppred not in matched:
+            if pattern_pred not in matched:
                 if self.verbose >= 10:
-                    print(f"[GenericPattern._match_backward] {self.print_match(pred, ppred)}")
-                matched[ppred] = pred
-                stack.append(ppred)
+                    print(
+                        f"[GenericPattern._match_backward] {self.print_match(graph_pred, pattern_pred)}"
+                    )
+                matched[pattern_pred] = graph_pred
+                stack.append(pattern_pred)
                 match_count += 1
         if self.verbose > 5 and match_count > 0:
-            print(f"[GenericPattern._match_backward] add {match_count} nodes")
+            print(f"[GenericPatternMatcher._match_backward] add {match_count} nodes")
         return match_count
 
     def _match_forward(
         self,
-        root_node: ir.Node,
-        matched: dict[ir.Node, ir.Node],
-        stack: list[int],
+        starting_node: ir.Node,
+        matched: dict[orp.NodePattern, ir.Node],
+        stack: list[orp.NodePattern],
         graph_node: ir.Node,
-        pattern_node: ir.Node,
+        pattern_node: orp.NodePattern,
     ) -> int | None:
         """
         Matches forward.
 
         Args:
-            root_node: root node (the node the match begins with, used only for debugging)
+            starting_node: root node (the node the match begins with, used only for debugging)
             matched: nodes of the pattern matched as already matched
             stack: next node to look into
             graph_node: node coming from the graph
             pattern_node: node coming from the pattern
 
         Returns:
             number of matched nodes to continue, None or False to indicate a failed match
@@ -390,41 +354,44 @@
             self._hint(
                 "FORWARD: not the same number of output_names",
                 "-- pattern",
                 pattern_node,
                 "-- model",
                 graph_node,
             )
-            return self.none(root_node, inspect.currentframe().f_lineno)
+            return self.none(starting_node, inspect.currentframe().f_lineno)
 
-        for o, op in zip(graph_node.outputs, pattern_node.outputs):
-            graph_node_users = [user for user, _ in o.uses()]
-            pattern_node_users = [user for user, _ in op.uses()]
+        for graph_output, pattern_output in zip(graph_node.outputs, pattern_node.outputs):
+            graph_node_users = [user for user, _ in graph_output.uses()]
+            pattern_node_users = [user for user, _ in pattern_output.uses()]
             if not pattern_node_users:
                 # The pattern has no node forward, the matching stops.
                 continue
             if len(graph_node_users) < len(pattern_node_users):
                 # Not enough node in the graph to match the pattern. A match is not possible
-                return self.none(root_node, inspect.currentframe().f_lineno)
+                return self.none(starting_node, inspect.currentframe().f_lineno)
 
             # Here comes the fun part, there is the same number of successors or more
             # nodes in the graph to match with the pattern.
             # And we have to handle the nodes already matched as found.
             # Hopefully, there is only one option.
 
             if len(graph_node_users) == len(pattern_node_users) == 1:
                 # Let's deal with the simple case
-                if graph_node_users[0].op_type != pattern_node_users[0].op_type:
-                    return self.none(root_node, inspect.currentframe().f_lineno)
+                if (
+                    graph_node_users[0].op_identifier()
+                    != pattern_node_users[0].op_identifier()
+                ):
+                    return self.none(starting_node, inspect.currentframe().f_lineno)
 
                 node = pattern_node_users[0]
                 if node not in matched:
                     if self.verbose >= 10:
                         print(
-                            f"[GenericPattern._match_forward]{self.print_match(graph_node_users[0], pattern_node_users[0])}"
+                            f"[GenericPatternMatcher._match_forward]{self.print_match(graph_node_users[0], pattern_node_users[0])}"
                         )
                     matched[node] = graph_node_users[0]
                     stack.append(node)
                     match_count += 1
                 continue
 
             # Let's remove the nodes already matched.
@@ -452,32 +419,35 @@
                 continue
             if len(free) < len(pattern_node_users_not_matched):
                 # Not enough successors to match the remaining patterns.
                 return self.none(node, inspect.currentframe().f_lineno)
             if len(pattern_node_users_not_matched) == len(free) == 1:
                 # Only one option again.
                 graph_node = free[0]
-                if pattern_node_users_not_matched[0].op_type != graph_node.op_type:
+                if (
+                    pattern_node_users_not_matched[0].op_identifier()
+                    != graph_node.op_identifier()
+                ):
                     return self.none(node, inspect.currentframe().f_lineno)
 
                 key = pattern_node_users_not_matched[0]
                 if self.verbose >= 10:
                     print(
-                        f"[GenericPattern._match_forward] {self.print_match(graph_node, pattern_node_users_not_matched[0])}"
+                        f"[GenericPatternMatcher._match_forward] {self.print_match(graph_node, pattern_node_users_not_matched[0])}"
                     )
                 matched[key] = graph_node
                 stack.append(key)
                 match_count += 1
                 continue
 
             # And now another fun part, let's try to handle the case when
             # there is only one option, matching on node type only returns one
             # option.
-            expected_op_type = [_.op_type for _ in pattern_node_users_not_matched]
-            got_op_type = [_.op_type for _ in free]
+            expected_op_type = [_.op_identifier() for _ in pattern_node_users_not_matched]
+            got_op_type = [_.op_identifier() for _ in free]
 
             ec = collections.Counter(expected_op_type)
             gc = collections.Counter(got_op_type)
             if len(ec) != len(gc) or set(ec) != set(gc):
                 # unique operator types is different.
                 self._hint(
                     "FORWARD: unique operator types are different",
@@ -494,24 +464,24 @@
             for k, v in ec.items():
                 if gc[k] < v:
                     # Not enough types to match.
                     return self.none(node, inspect.currentframe().f_lineno)
 
             # At this stage, we know matching the types is possible.
             # We first mark whatever is possible.
-            ptype_to_node = {_.op_type: _ for _ in pattern_node_users_not_matched}
-            gtype_to_node = {_.op_type: _ for _ in free}
+            ptype_to_node = {_.op_identifier(): _ for _ in pattern_node_users_not_matched}
+            gtype_to_node = {_.op_identifier(): _ for _ in free}
             missing = []
             for k, v in ec.items():
                 if gc[k] == v == 1:
                     key = id(ptype_to_node[k])
                     if key not in matched:
                         if self.verbose >= 10:
                             print(
-                                f"[GenericPattern._match_forward] match "
+                                f"[GenericPatternMatcher._match_forward] match "
                                 f"{self.print_match(gtype_to_node[k], ptype_to_node[k])}"
                             )
                         matched[key] = gtype_to_node[k]
                         stack.append(key)
                         match_count += 1
                 else:
                     missing.append(k)
@@ -523,92 +493,97 @@
             # 1. make assumptions and continue
             # 2. mark the node as incomplete matching, we could end up stuck anyway.
             raise NotImplementedError(
                 f"There are more than one option, this will be implemented later, "
                 f"ec={ec}, gc={gc}"
             )
         if self.verbose > 5 and match_count > 0:
-            print(f"[GenericPattern._match_forward] add {match_count} nodes")
+            print(f"[GenericPatternMatcher._match_forward] add {match_count} nodes")
         return match_count
 
     def match(
         self,
-        g: ir.Graph | ir.GraphView,
+        model: ir.Model,
+        graph_or_function: ir.Graph | ir.Function,
         node: ir.Node,
-    ) -> PatternMatchResult | None:
+        verbose: int = 0,
+    ) -> orp.MatchResult | None:
+        del model
+        del graph_or_function
+        self.verbose = verbose
         self._debug = {}
 
-        match_pattern: ir.Graph = self._get_match_pattern(g)
-
         # Let's match the last node.
         # Then we need to match successors and predecessors.
-        last_pattern_node = match_pattern[-1]
-        if node.op_type != last_pattern_node.op_type:
-            # The last node does not have the same op_type.
+        last_pattern_node = self.pattern.node(-1)
+        if node.op_identifier() != last_pattern_node.op_identifier():
+            # The last node does not have the same op_identifier().
             return self.none()
 
         if self.verbose > 5:
-            print(f"[GenericPattern.match] starts with {node}")
+            print(
+                f"[GenericPatternMatcher.match] Matching started at node: {_node_to_str(node)}"
+            )
             if self.verbose >= 10:
-                print(f"[GenericPattern.match] match pattern {self!r}")
+                print(f"[GenericPatternMatcher.match] match pattern {self}")
 
-        all_pattern_nodes = set(match_pattern)
-        matched: dict[ir.Node, ir.Node] = {last_pattern_node: node}
-        stack: list[ir.Node] = [last_pattern_node]
+        all_pattern_nodes = set(self.pattern)
+        matched: dict[orp.NodePattern, ir.Node] = {last_pattern_node: node}
+        stack: list[orp.NodePattern] = [last_pattern_node]
         iteration = 0
 
         if self.verbose > 5:
             self._debug = dict(
-                pattern=match_pattern,
+                pattern=self.pattern,
                 matched=matched,
                 stack=stack,
                 iteration=iteration,
                 node=node,
                 pattern_node=last_pattern_node,
-                pattern_nodes=match_pattern,
+                pattern_nodes=self.pattern,
             )
 
-        max_iter = len(match_pattern) * 2
+        max_iter = self.pattern.num_nodes() * 2
         while stack and iteration < max_iter:
             nodes_not_in_pattern = set(matched.keys()) - all_pattern_nodes
             assert not nodes_not_in_pattern, (
                 f"Some nodes are not part of the pattern: {nodes_not_in_pattern}"
                 f"\nall_pattern_nodes={all_pattern_nodes}"
             )
 
             # TODO(justinchuby): Change to a for loop
             iteration += 1
             if self.verbose > 5:
                 print(
-                    f"[GenericPattern.match] iteration={iteration} "
+                    f"[GenericPatternMatcher.match] iteration={iteration} "
                     f"n_matched={len(matched)}, n_stack={len(stack)}, "
-                    f"matched_types={collections.Counter(_.op_type for _ in matched)}"
+                    f"matched_types={collections.Counter(_.op_identifier() for _ in matched)}"
                 )
-            pattern_node_from_stack = stack.pop()
-            pattern_to_graph_node = matched[pattern_node_from_stack]
+            next_pattern_node = stack.pop()
+            next_graph_node = matched[next_pattern_node]
 
             result = self._match_backward(
-                node, matched, stack, pattern_to_graph_node, pattern_node_from_stack
+                node, matched, stack, next_graph_node, next_pattern_node
             )
             if result is None:
                 if self.verbose > 5:
-                    print("[GenericPattern.match] done. backward failed.")
+                    print("[GenericPatternMatcher.match] done. backward failed.")
                 return result
 
             nodes_not_in_pattern = set(matched.keys()) - all_pattern_nodes
             assert (
                 not nodes_not_in_pattern
             ), f"Some nodes are not part of the pattern: {nodes_not_in_pattern}"
 
             result = self._match_forward(
-                node, matched, stack, pattern_to_graph_node, pattern_node_from_stack
+                node, matched, stack, next_graph_node, next_pattern_node
             )
             if result is None:
                 if self.verbose > 5:
-                    print("[GenericPattern.match] done. forward failed.")
+                    print("[GenericPatternMatcher.match] done. forward failed.")
                 return result
 
             nodes_not_in_pattern = set(matched.keys()) - all_pattern_nodes
             assert (
                 not nodes_not_in_pattern
             ), f"Some nodes are not part of the pattern: {nodes_not_in_pattern}"
 
@@ -616,112 +591,27 @@
                 self._debug["iteration"] = iteration
 
         if iteration >= max_iter and stack:
             self._hint("reached {iteration}>={max_iter} iterations")
             return self.none(node, inspect.currentframe().f_lineno)
 
         if self.verbose > 5:
-            print(f"[GenericPattern.match] done. {len(matched)} matched nodes")
+            print(f"[GenericPatternMatcher.match] done. {len(matched)} matched nodes")
 
         # At this point, the pattern is matched but let's make sure.
-        assert len(matched) == len(match_pattern), (
+        assert len(matched) == self.pattern.num_nodes(), (
             f"Number of matched nodes is different, {len(matched)} matched nodes, "
-            f"and {len(match_pattern)} nodes in the pattern, matched is {matched}"
+            f"and {len(self.pattern)} nodes in the pattern, matched is {matched}"
         )
         assert len(stack) == 0, f"There are still {len(stack)} nodes to explore."
 
         # We order the matched nodes in the same order than the pattern
         # to let next functions to be able to build the matching again.
-        matched_nodes = [matched[pattern_node] for pattern_node in match_pattern]
-        return PatternMatchResult(
-            self,
-            matched_nodes,
-            tuple(match_pattern),
-            match_pattern.inputs,
-            match_pattern.outputs,
-        )
-
-    def apply(
-        self,
-        model: ir.Model,
-        match_result: orp.MatchResult,
-        verbose: int = 0,
-    ) -> orp.ReplacementSubgraph | None:
-        x = orp.ReplacementPatternFunction(self.apply_pattern)
-        replacement = x.get_replacement(match_result)
-        # if replacement is not None:
-        #     TODO(Rama)
-        #     assert len(replacement.new_outputs) == len(match_result.pattern_outputs), (
-        #         f"Not the same number of outputs, matched "
-        #         f"outputs={match_result.pattern_outputs}, "
-        #         f"got {replacement.new_outputs} in the applied pattern."
-        #     )
-        return replacement
-
-    def make_rule(self) -> orp.RewriteRule:
-        """Creates the corresponding rule for this pattern."""
-        return GenericRewriteRule(self)
-
-
-class FunctionPattern(GenericPattern):
-    """An instance of GenericPattern taking ir.Function.
-
-    It defines the matching pattern and its replacement.
-
-    Args:
-        match_pattern: the onnx ir function defining the matching pattern
-        apply_pattern: the onnx ir function defining the new pattern
-        validate_mapping: the function used to validate a pattern
-        verbose: in [0, 10], increase the verbosity to understand why a pattern
-            does not match
-
-    """
-
-    def __init__(
-        self,
-        match_pattern: ir.Function,
-        apply_pattern: Callable,
-        validate_mapping: Callable,
-        verbose: int = 0,
-    ):
-        self.match_pattern = match_pattern
-        self.apply_pattern = apply_pattern
-        self.validate_mapping = validate_mapping
-        self.verbose = verbose
-
-    def _get_match_pattern(self, *_, **__):
-        return self.match_pattern
-
-
-def _build_pattern(match_pattern_function: Callable) -> ir.Graph:
-    kwargs = {}
-    args = []
-
-    # There should be a better way.
-    sig = inspect.signature(match_pattern_function)
-    for i, p in enumerate(sig.parameters.values()):
-        if i == 0:
-            continue
-        if p.default is not inspect._empty:
-            # an attribute
-            kwargs[p.name] = p.default
-        else:
-            args.append(p.name)
-
-    assert len(kwargs) == 0, f"Attributes are not supported yet but kwargs={kwargs}"
-
-    inputs = [ir.Input(name=name) for name in args]
-    builder = orp.RewriterContext()
-    outputs = match_pattern_function(builder, *inputs, **kwargs)
-    if isinstance(outputs, ir.Value):
-        outputs = [outputs]
-    # TODO(Rama): Should construct a function!
-    graph = ir.Graph(inputs=inputs, outputs=outputs, nodes=builder.nodes)
-    graph.outputs[:] = outputs
-    return graph
+        matched_nodes = [matched[pattern_node] for pattern_node in self.pattern]
+        return _to_match_result(PatternMatchResult(self.pattern, matched_nodes))
 
 
 def make_pattern_rule(
     match_pattern_function: Callable,
     apply_pattern_function: Callable,
     validate_mapping: Callable | None = None,
     verbose: int = 0,
@@ -739,16 +629,16 @@
             If not specified, it is equivalent to a function that always return True
         verbose: verbosity level
 
     Returns:
         the rewriting rule
     """
 
-    match_pattern_ir = _build_pattern(match_pattern_function)
-
-    pat = FunctionPattern(
-        match_pattern_ir,
+    pattern = orp._to_graph_pattern(match_pattern_function)
+    matcher = GenericPatternMatcher(pattern)
+    return orp.RewriteRule(
+        pattern,
         apply_pattern_function,
-        validate_mapping or (lambda *_, **__: True),
+        validate_mapping,
+        matcher,
         verbose=verbose,
     )
-    return pat.make_rule()
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/no_op.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 op = pattern.onnxop
 
 # TODO: Support 1-D constant tensors
 # https://github.com/microsoft/onnx-rewriter/issues/186
 
 
 # Pattern to match against
-def mul_by_1(x):
+def mul_by_1(op, x):
     return x * 1
 
 
-def add_0(x):
+def add_0(op, x):
     return x + 0
 
 
-def sub_0(x):
+def sub_0(op, x):
     return x - 0
 
 
-def div_by_1(x):
+def div_by_1(op, x):
     return x / 1
 
 
 # Replacement
 def identity(op, x):
     return op.Identity(x)
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
 import logging
 
 from onnxscript.rewriter import pattern
 
-op = pattern.onnxop
-msft_op = pattern.msft_op
 torch_module_op = pattern.torch_module_op
 
 logger = logging.getLogger(__name__)
 
 
 def group_normalization_and_silu_submodule(
+    op,
     input,
     weight,
     bias,
     epsilon,
     groups,
 ):
-    group_norm = msft_op.GroupNorm(
+    group_norm = op.GroupNorm(
         input,
         weight,
         bias,
         activation=0,
         channels_last=1,
         epsilon=epsilon,
         groups=groups,
+        domain="com.microsoft",
     )
     transposed = op.Transpose(group_norm, perm=[0, 3, 1, 2])
-    return torch_module_op.submodule("torch_nn_modules_activation_SiLU")(transposed)
+    return torch_module_op.submodule("torch_nn_modules_activation_SiLU")(
+        transposed
+    )  # TODO(rama)
 
 
 def group_normalization_with_silu(
     op,
     input,
     weight,
     bias,
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import logging
 
 import numpy as np
 import onnx
 
 from onnxscript.rewriter import _ir_utils, pattern
 
-op = pattern.onnxop
-msft_op = pattern.msft_op
 torch_module_op = pattern.torch_module_op
 
 logger = logging.getLogger(__name__)
 
 
 def check_if_simulated_instance_norm_is_used(
+    context,
     input_x,
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
@@ -82,14 +81,15 @@
     if original_input_shape is None or original_input_shape.tolist() != input_x.shape:
         return False
 
     return True
 
 
 def instance_simulates_group_normalization_pattern(
+    op,
     input_x,
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 from onnxscript import ir
 from onnxscript.rewriter import pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
-def softmax_with_fp32_upcast(input, axis):
+def softmax_with_fp32_upcast(op, input, axis):
     upcast = op.Cast(input, to=onnx.TensorProto.FLOAT)
     softmax = op.Softmax(upcast, axis=axis)  # pylint: disable=redefined-outer-name
     return op.Cast(softmax, to=onnx.TensorProto.FLOAT16)
 
 
 def softmax(op, input, axis):
     return op.Softmax(input, axis=axis)
 
 
-def softmax_with_fp32_upcast_without_axis(input):
+def softmax_with_fp32_upcast_without_axis(op, input):
     upcast = op.Cast(input, to=onnx.TensorProto.FLOAT)
     softmax = op.Softmax(upcast)  # pylint: disable=redefined-outer-name
     return op.Cast(softmax, to=onnx.TensorProto.FLOAT16)
 
 
 def softmax_without_axis(op, input):
     return op.Softmax(input)
 
 
-def check_if_fp16_input(input, **_) -> bool:
+def check_if_fp16_input(context, input, **_) -> bool:
     if input is None:
         logger.warning(
             "Cannot perform softmax upcast removal: "
             "cannot retrieve match_bindings for 'input' for dtype validation."
         )
         return False
     return input.dtype == ir.DataType.FLOAT16
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240511/onnxscript/rewriter/pattern.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
+import abc
 import dataclasses
 import inspect
 import itertools
 import math
 from typing import (
     Any,
     Callable,
+    Iterator,
     List,
     MutableSequence,
     Optional,
     Protocol,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
-import onnx
-
 from onnxscript import ir
 from onnxscript.ir import _convenience
 from onnxscript.rewriter import _ir_utils, _tape
 
 T = TypeVar("T")
 
 
@@ -37,34 +37,47 @@
 
     def __init__(self, value: str):
         self._value = value
 
     def matches(self, item: str) -> bool:
         return item == self._value
 
+    def __str__(self) -> str:
+        return self._value
+
 
 class PrefixPattern(Pattern[str]):
     """Matches strings with a given prefix."""
 
     def __init__(self, value: str) -> None:
         self._value = value
 
     def matches(self, value: str) -> bool:
         return value.startswith(self._value)
 
+    def __str__(self) -> str:
+        return f"{self._value}*"
+
 
 class AttrPattern(Pattern[Union[ir.Attr, ir.RefAttr]]):
     """Base class for an attribute pattern. Matches any attribute value by default."""
 
     def __init__(self, name: str | None):
-        self.name = name
+        self._name = name
+
+    @property
+    def name(self) -> str | None:
+        return self._name
 
     def matches(self, attr: ir.Attr | ir.RefAttr) -> bool:
         return True
 
+    def __str__(self) -> str:
+        return self._name if self._name is not None else "anonymous:" + str(id(self))
+
 
 # TODO: Support tensors. Align with usage elsewhere.
 SupportedAttrTypes = Union[
     int,
     float,
     str,
     Sequence[int],
@@ -83,14 +96,17 @@
     def __init__(self, value: SupportedAttrTypes):
         super().__init__(None)
         self._value = value
 
     def matches(self, attr: ir.Attr | ir.RefAttr) -> bool:
         return isinstance(attr, ir.Attr) and attr.value == self._value
 
+    def __str__(self) -> str:
+        return str(self._value)
+
 
 def _to_attr_pattern(value: AttrPattern | ValuePattern | SupportedAttrTypes) -> AttrPattern:
     """Represents promotion of values allowed as keyword-arguments in a pattern-builder call to an AttrPattern."""
     if isinstance(value, AttrPattern):
         return value
     if type(value) == ValuePattern:
         # This is a hack. Currently, when we create pattern-variables, we create them as ValuePattern,
@@ -122,39 +138,45 @@
     Here, `op` is an instance of OpsetPatternBuilder and `op.Matmul` is an instance
     of OpPatternBuilder, and  `op.Matmul(x, y)` is an instance of NodePattern.
 
     (ii) An opset pattern is also matched against the actual opset domain used in the
     input model.
     """
 
-    def __init__(self, domain_pattern: Pattern[str] | str) -> None:
-        if isinstance(domain_pattern, str):
-            domain_pattern = StringConstantPattern(domain_pattern)
-        self.domain_pattern = domain_pattern
+    def __init__(self, domain: Pattern[str] | str) -> None:
+        if isinstance(domain, str):
+            self._domain_name: str | None = domain
+            self._domain_pattern: Pattern[str] = StringConstantPattern(domain)
+        else:
+            self._domain_name = None
+            self._domain_pattern = domain
 
-    @classmethod
-    def domain_prefix(cls, domain: str) -> OpsetPatternBuilder:
-        return cls(PrefixPattern(domain))
+    @property
+    def domain_name(self) -> str | None:
+        return self._domain_name
 
     def matches(self, domain):
-        return self.domain_pattern.matches(domain)
+        return self._domain_pattern.matches(domain)
 
-    def __getattr__(self, name: str) -> OpPatternBuilder:
-        return OpPatternBuilder(self, StringConstantPattern(name))
+    def __getattr__(self, op_name: str) -> OpPatternBuilder:
+        return OpPatternBuilder(self, op_name)
 
     def submodule(self, name: str) -> OpPatternBuilder:
         """This method is used to match against submodule ops with prefix."""
         return OpPatternBuilder(self, PrefixPattern(name))
 
+    def __str__(self) -> str:
+        return str(self._domain_pattern)
+
 
 onnxop = OpsetPatternBuilder("")
 
 msft_op = OpsetPatternBuilder("com.microsoft")
 
-torch_module_op = OpsetPatternBuilder.domain_prefix("pkg.torch")
+torch_module_op = OpsetPatternBuilder(PrefixPattern("pkg.torch"))
 
 
 class OpPatternBuilder:
     """A utility class to build a NodePattern.
 
     It is used primarily to create a NodePattern.
     Example usage:
@@ -165,36 +187,56 @@
     Here, `op` is an instance of OpsetPatternBuilder and `op.Matmul` is an instance
     of OpPatternBuilder, and  `op.Matmul(x, y)` is an instance of NodePattern.
 
     """
 
     def __init__(
         self,
-        opset_pattern: Pattern[str],
-        op_name_pattern: Pattern[str],
+        opset_pattern: OpsetPatternBuilder,
+        op_name: str | Pattern[str],
     ) -> None:
         self.opset_pattern = opset_pattern
-        self.op_name_pattern = op_name_pattern
+        self.op_name = op_name
 
-    def __call__(self, *args, **kwargs):
-        # TODO(rama): Unify with convention used elsewhere.
-        if "_num_outputs" in kwargs:
-            num_outputs = kwargs["_num_outputs"]
-            del kwargs["_num_outputs"]
+    def __call__(
+        self,
+        *args,
+        domain: str | None = None,
+        version: int | None = None,
+        outputs: int | list[str | None] = 1,
+        **kwargs,
+    ):
+        if version is not None:
+            raise ValueError(
+                "The pattern builder does not support 'version' keyword argument. "
+                "Version restrictions should be handled by rewrite rules."
+            )
+        if domain is None:
+            opset_pattern = self.opset_pattern
+        elif isinstance(domain, str):
+            opset_pattern = OpsetPatternBuilder(domain)
         else:
-            num_outputs = 1
+            # TODO(rama): allow OpsetPatternBuilder as domain.
+            raise TypeError("domain must be a string.")
+
+        if isinstance(outputs, int):
+            outputs = [None for _ in range(outputs)]
+        elif not isinstance(outputs, Sequence) or not all(
+            isinstance(x, (str, type(None))) for x in outputs
+        ):
+            raise ValueError("outputs must be an int or a list[str|None].")
         inputs = [_to_value_pattern(x) for x in args]
         attributes = {name: _to_attr_pattern(value) for (name, value) in kwargs.items()}
-        node_pattern = NodePattern(
-            self.opset_pattern, self.op_name_pattern, inputs, attributes
-        )
-        if num_outputs == 1:
-            return NodeOutputPattern(node_pattern, 0)
+        node_pattern = NodePattern(opset_pattern, self.op_name, inputs, attributes, outputs)
+        output_values = node_pattern.outputs
+        # Unpack outputs if there is only one output, the common case.
+        if len(output_values) == 1:
+            return output_values[0]
         else:
-            return [NodeOutputPattern(node_pattern, i) for i in range(num_outputs)]
+            return output_values
 
 
 def _to_value_pattern(
     x: ValuePattern | int | float | None,
 ) -> ValuePattern | None:
     """Promotes an input-value used to construct a NodePattern to a ValuePattern.
 
@@ -239,87 +281,102 @@
             return t2
     The above pattern matches a sequence of two Reshape ops.
     The matched_nodes will contain the two Reshape ops, and the bindings will
     contain the values that are bound to the variables `x`, `shape1`, and `shape2`.
     """
 
     def __init__(self, success: bool) -> None:
-        self.success: bool = success
-        # For a successful match, matched_nodes is a list of values that matched the pattern.
+        self._success: bool = success
+        # For a successful match, _matched_nodes is a list of values that matched the pattern.
         # These include the internal nodes of the pattern that were matched, but not
         # the leaves (sub-trees) that match against the variables in the pattern.
         # These represent the values that will be replaced by the replacement pattern.
-        self.matched_nodes: MutableSequence[ir.Node] = []
+        self._matched_nodes: MutableSequence[ir.Node] = []
         # For a successful match, bindings is a dictionary of mapping pattern-variable-names
         # to values.
         self.bindings: dict[str, Any] = {}
-        self.outputs: MutableSequence[ir.Value] = []
+        self.outputs: list[ir.Value] = []
 
     def __bool__(self):
-        return self.success
+        return self._success
 
     @classmethod
     def FAIL(cls):
         return cls(False)
 
     @property
     def nodes(self) -> MutableSequence[ir.Node]:
-        return self.matched_nodes
+        return self._matched_nodes
 
     def bind(self, var: str, value: Any) -> bool:
         """Binds a pattern variable name to a value from the matched IR.
 
         Returns True if the binding is successful, False otherwise (when the binding is inconsistent).
         """
         if var in self.bindings:
             # TODO(rama): Use appropriate equality-check here.
             if self.bindings[var] == value:
                 return True
-            self.success = False
+            self._success = False
             return False
         self.bindings[var] = value
         return True
 
     def extend(self, other: MatchResult | bool):
-        if not self.success:
+        if not self._success:
             return
         if not other:
-            self.success = False
+            self._success = False
             return
         if isinstance(other, bool):
             return
         for var, val in other.bindings.items():
             if var in self.bindings:
                 # TODO: handle attribute var bindings
                 if self.bindings[var] != val:
-                    self.success = False
+                    self._success = False
                     return
             else:
                 self.bindings[var] = val
-        assert self.matched_nodes is not None, "matched_nodes should not be None."
-        self.matched_nodes.extend(other.matched_nodes)  # type: ignore[attr-defined]
+        assert self._matched_nodes is not None, "_matched_nodes should not be None."
+        self._matched_nodes.extend(other._matched_nodes)  # type: ignore[attr-defined]
 
 
 class ValuePattern:
     """Base class for all patterns that match against IR values.
 
     This is used primarily to provide operator overloadings for arithmetic
     operations, so that we can write patterns like `x + 1` and `1 + x`.
     """
 
     def __init__(self, name: str | None) -> None:
-        self.name = name
+        self._name = name
+        # Note: uses will be computed only when the full graph-pattern is constructed.
+        self._uses: list[tuple[NodePattern, int]] = []
+
+    @property
+    def name(self) -> str | None:
+        return self._name
+
+    def producer(self) -> None | NodePattern:
+        return None
+
+    def uses(self) -> Sequence[tuple[NodePattern, int]]:
+        return self._uses
+
+    def append_use(self, node: NodePattern, index: int):
+        self._uses.append((node, index))
 
     def __repr__(self) -> str:
-        return f"ValuePattern({self.name!r})"
+        return f"ValuePattern({self._name!r})"
 
     def matches(self, value: ir.Value):
         result = MatchResult(success=True)
-        if self.name is not None:
-            result.bind(self.name, value)
+        if self._name is not None:
+            result.bind(self._name, value)
         return result
 
     def commute(self) -> Sequence[ValuePattern]:
         """Return a list of commuted patterns.
 
         This is used to handle commutative operations like addition and multiplication.
         A single pattern is converted into a list of equivalent patterns by swapping
@@ -350,37 +407,95 @@
 
     def __rtruediv__(self, other):
         return onnxop.Div(other, self)
 
     def __pow__(self, other):
         return onnxop.Pow(self, other)
 
+    def __str__(self) -> str:
+        return self._name if self._name is not None else "anonymous:" + str(id(self))
+
 
 class NodePattern:
     """Represents a pattern that matches against a Node.
 
     This differs from a NodeOutputPattern in that it matches against a node (which
     may produce 1 or more outputs), whereas a NodeOutputPattern matches against
     a specific output of a node.
     """
 
     def __init__(
         self,
-        domain: Pattern[str],
-        op: Pattern[str],
+        domain: OpsetPatternBuilder,
+        op: str | Pattern[str],
         inputs: Sequence[int | float | ValuePattern | None],
         attributes: dict[str, AttrPattern],
+        outputs: Sequence[str | None],
     ):
         self.domain = domain
-        self.op = op
+        self.op = StringConstantPattern(op) if isinstance(op, str) else op
         self.inputs = [_to_value_pattern(x) for x in inputs]
         self.attributes = attributes
+        # In the common case, domain and op are constants, which can be used to optimize matching.
+        if isinstance(op, str) and domain.domain_name is not None:
+            # TODO(rama): support overloaded operators.
+            overload = ""
+            self._op_identifier: tuple[str, str, str] | None = (
+                domain.domain_name,
+                op,
+                overload,
+            )
+        else:
+            self._op_identifier = None
+        self.outputs = [NodeOutputPattern(self, i, name) for i, name in enumerate(outputs)]
 
-    def matches_node(self, node: ir.Node) -> MatchResult:
-        """Examine if the IR node matches the self pattern."""
+        # Update uses for inputs.
+        for index, value in enumerate(self.inputs):
+            if value is not None:
+                value.append_use(self, index)
+
+    def __str__(self) -> str:
+        inputs = ", ".join(str(v) for v in self.inputs)
+        outputs = ", ".join(str(v) for v in self.outputs)
+        attributes = ", ".join(f"{k}={v}" for k, v in self.attributes.items())
+        op = str(self.op)
+        domain = str(self.domain)
+        qualified_op = f"{domain}.{op}" if domain else op
+        inputs_and_attributes = f"{inputs}, {attributes}" if attributes else inputs
+        return f"{outputs} = {qualified_op} ({inputs_and_attributes})"
+
+    def op_identifier(self) -> Tuple[str, str, str] | None:
+        return self._op_identifier
+
+    @property
+    def op_type(self) -> str:
+        return str(self.op)
+
+    def matches(self, node: ir.Node) -> bool:
+        """Matches the pattern represented by self against a node.
+
+        This is purely a local node-level match, and does not consider the subgraph rooted at the node.
+        We check the domain, op_type, and attributes of the node, but not the inputs.
+        """
+        if not self.op.matches(node.op_type):
+            return False
+        # TODO(rama): Ensure we handle "" and "onnx.ai" correctly.
+        if not self.domain.matches(node.domain):
+            return False
+
+        # for name, attr_pattern in self.attributes.items():
+        #     attr_value = node.attributes.get(name)
+        #     if attr_value is None:
+        #         return False
+        #     if not attr_pattern.matches(attr_value):
+        #         return False
+        return True
+
+    def matches_subgraph(self, node: ir.Node) -> MatchResult:
+        """Matches the pattern subgraph represented by self against subgraph rooted at node."""
         if not self.domain.matches(node.domain):
             return MatchResult.FAIL()
         if not self.op.matches(node.op_type):
             return MatchResult.FAIL()
         match = MatchResult(success=True)
         # TODO: We should add filtered logging starting from here to emit why
         # matching failed. This should cut a lot of noises compared to logging everything,
@@ -426,65 +541,76 @@
                         yield [pattern, *rest]
 
         inputs = list(enumerate_inputs(list_of_lists, 0))
         if self.domain.matches("") and (self.op.matches("Add") or self.op.matches("Mul")):
             # TODO: handle cases where number of inputs is not 2.
             swapped = [[x[1], x[0]] for x in inputs]
             inputs.extend(swapped)
-        return [NodePattern(self.domain, self.op, input, self.attributes) for input in inputs]
+        outputs = [value.name for value in self.outputs]
+        return [
+            NodePattern(self.domain, self.op, input, self.attributes, outputs)
+            for input in inputs
+        ]
 
 
 class NodeOutputPattern(ValuePattern):
     """Represents a pattern that matches against a specific output of a Node.
 
     This is the primary pattern used to match against computed values, that
     is values computed using a specific op.
     """
 
     def __init__(
-        self, node_pattern: NodePattern, output_index: int, name: str | None = None
+        self, producer: NodePattern, output_index: int, name: str | None = None
     ) -> None:
         super().__init__(name)
-        self.node_pattern = node_pattern
-        self.output_index = output_index
+        self._producer = producer
+        self._output_index = output_index
+
+    @property
+    def output_index(self) -> int:
+        return self._output_index
 
     def matches(self, value: ir.Value):
-        """Match the StaticValueInfo from IR with the `matches_node()` in node pattern."""
+        """Match the StaticValueInfo from IR with the `matches_subgraph()` in node pattern."""
         node = value.producer()
         if node is None:
             return MatchResult.FAIL()
-        if value.index() != self.output_index:
+        if value.index() != self._output_index:
             return MatchResult.FAIL()
-        return self.node_pattern.matches_node(node)
+        return self._producer.matches_subgraph(node)
 
     def commute(self) -> Sequence[ValuePattern]:
         # TODO
         return [
-            NodeOutputPattern(pattern, self.output_index, self.name)
-            for pattern in self.node_pattern.commute()
+            NodeOutputPattern(pattern, self._output_index, self.name)
+            for pattern in self._producer.commute()
         ]
 
+    def producer(self) -> NodePattern:
+        return self._producer
+
 
 Var = ValuePattern
 
 
 class Constant(ValuePattern):
     """Represents a pattern that matches against a scalar constant value."""
 
     def __init__(
         self, value: int | float, rel_tol: float = 1e-5, abs_tol: float = 1e-8
     ) -> None:
         super().__init__(None)
-        self.value = value
-        self.rel_tol = rel_tol
-        self.abs_tol = abs_tol
+        self._value = value
+        self._rel_tol = rel_tol
+        self._abs_tol = abs_tol
 
     def match_scalar(self, scalar_value):
         status = math.isclose(
-            scalar_value, self.value, rel_tol=self.rel_tol, abs_tol=self.abs_tol
+            scalar_value, self._value, rel_tol=self._rel_tol, abs_tol=self._abs_tol
         )
         # Note: If the value is produced by a Constant node, we could include
         # the Constant node in the return_value list. However, we don't do that.
         # Instead, we will rely on DCE to remove the constant node if it is not
         # used elsewhere.
         return MatchResult(success=status)
 
@@ -499,87 +625,145 @@
             return MatchResult.FAIL()
 
         return self.match_scalar(constant_value.item())
 
     def commute(self) -> list[ValuePattern]:
         return [self]
 
+    def __str__(self) -> str:
+        return str(self._value)
+
+
+def _nodes_in_pattern(outputs: Sequence[ValuePattern]) -> list[NodePattern]:
+    """Returns all nodes used in a pattern, given the outputs of the pattern."""
+    node_patterns: list[NodePattern] = []
+
+    def visit(value_patterns: Sequence[ValuePattern | None]) -> None:
+        for value_pattern in value_patterns:
+            if isinstance(value_pattern, NodeOutputPattern):
+                node_pattern = value_pattern.producer()
+                if node_pattern not in node_patterns:
+                    node_patterns.append(node_pattern)
+                    visit(node_pattern.inputs)
+
+    visit(outputs)
+    node_patterns.reverse()
+    return node_patterns
+
 
 class GraphPattern:
     """Represents a pattern that can be matched against a subgraph."""
 
-    def __init__(self, outputs: Sequence[ValuePattern]) -> None:
-        self.outputs = outputs
+    def __init__(
+        self, inputs: Sequence[ValuePattern], outputs: Sequence[ValuePattern]
+    ) -> None:
+        self._inputs = inputs
+        self._outputs = outputs
         if len(outputs) == 0:
             raise ValueError("GraphPattern must have at least one output")
+        self._nodes = _nodes_in_pattern(outputs)
+
         # Check if all outputs are produced by the same node.
         output_node = None
         for i, value_pattern in enumerate(outputs):
             if not isinstance(value_pattern, ValuePattern):
                 raise TypeError(
                     f"Invalid type {type(value_pattern)} for graph pattern output."
                 )
             if not isinstance(value_pattern, NodeOutputPattern) or (
                 value_pattern.output_index != i
             ):
                 output_node = None
             elif i == 0:
-                output_node = value_pattern.node_pattern
-            elif value_pattern.node_pattern is not output_node:
+                output_node = value_pattern.producer()
+            elif value_pattern.producer() is not output_node:
                 output_node = None
         self._output_node = output_node
 
+    def node(self, index: int) -> NodePattern:
+        return self._nodes[index]
+
+    def num_nodes(self) -> int:
+        return len(self._nodes)
+
+    @property
+    def inputs(self) -> Sequence[ValuePattern]:
+        return self._inputs
+
+    @property
+    def outputs(self) -> Sequence[ValuePattern]:
+        return self._outputs
+
+    def __iter__(self) -> Iterator[NodePattern]:
+        return iter(self._nodes)
+
+    def __reversed__(self) -> Iterator[NodePattern]:
+        return reversed(self._nodes)
+
+    @property
+    def has_single_output_node(self) -> bool:
+        return self._output_node is not None
+
     @property
     def num_outputs(self) -> int:
-        return len(self.outputs)
+        return len(self._outputs)
 
-    def matches_node(self, node: ir.Node) -> MatchResult:
+    def matches_subgraph(self, node: ir.Node) -> MatchResult:
         if self._output_node is None:
             return MatchResult.FAIL()
-        return self._output_node.matches_node(node)
+        return self._output_node.matches_subgraph(node)
 
     def commute(self) -> Sequence[GraphPattern]:
         if self._output_node is None:
             raise NotImplementedError(
                 "Cannot commute a graph pattern with multiple output nodes."
             )
         nodes = self._output_node.commute()
         return [
-            GraphPattern([NodeOutputPattern(n, i) for i in range(self.num_outputs)])
+            GraphPattern(
+                self._inputs, [NodeOutputPattern(n, i) for i in range(self.num_outputs)]
+            )
             for n in nodes
         ]
 
+    def __str__(self) -> str:
+        inputs = ", ".join(str(v) for v in self._inputs)
+        outputs = ", ".join(str(v) for v in self._outputs)
+        nodes = "\n   ".join(str(n) for n in self._nodes)
+        return f"pattern ({inputs}) {{\n   {nodes}\n   return {outputs}\n}}"
+
 
 def _to_graph_pattern(pattern_constructor: Callable) -> GraphPattern:
     """Convert a pattern-construction function to a GraphPattern.
 
     A pattern-construction function will return values as below:
     ::
-        def pattern(x: Var, shape1: Var, shape2: Var):
+        def pattern(op, x: Var, shape1: Var, shape2: Var):
             ...
             return outputs
 
     We create a pattern graph by creating pattern-variables for each parameter of the function,
     and calling the function. The returned values are normalized to a list of ValuePatterns,
     which represent the outputs of the pattern graph.
 
     Args:
         pattern_constructor: Callable
 
     Returns:
         GraphPattern: A representation of the pattern that can be matched against a subgraph.
     """
     _pattern_vars = inspect.signature(pattern_constructor).parameters
-    vars = [Var(v) for v in _pattern_vars]
-    pattern_outputs = pattern_constructor(*vars)
+    pattern_inputs = [Var(v) for v in _pattern_vars][1:]  # Skip the first parameter
+    pattern_outputs = pattern_constructor(onnxop, *pattern_inputs)
+    # TODO(rama): classify inputs as value/attribute vars
     # Returned value could be a single ValuePattern or a list of ValuePatterns.
     # Normalize representation to a list of ValuePatterns.
     if isinstance(pattern_outputs, ValuePattern):
         pattern_outputs = [pattern_outputs]
-    return GraphPattern(pattern_outputs)
+    return GraphPattern(pattern_inputs, pattern_outputs)
 
 
 def _valid_to_replace(matched_nodes: Sequence[ir.Node]) -> bool:
     """Check that values computed by the matched_nodes, except for the last one, are used only by the matched_nodes."""
     # * Must check that all values matched by pattern are used only by pattern,
     # except for the value that is replaced.
     # * Must ensure that replacement subgraph does not use any of the deleted
@@ -611,21 +795,22 @@
     def __getattr__(self, op_type: str) -> Any:
         return lambda *args, **kwargs: self._make_node(op_type, args, kwargs)
 
     def _make_node(self, op_type: str, inputs: Sequence[ir.Value], kwargs: dict[str, Any]):
         # TODO(rama): some of the following logic should move into the tape.
         domain = kwargs.pop("domain", "")
         version = kwargs.pop("version", None)
-        self._used_opsets.append((domain, version))
         outputs = kwargs.pop("outputs", 1)
         if isinstance(outputs, Sequence):
             num_outputs = len(outputs)
         else:
             assert isinstance(outputs, int)
             num_outputs = outputs
+
+        self._used_opsets.append((domain, version))
         if num_outputs == 1:
             value = self._tape.op(op_type, inputs=inputs, attributes=kwargs, domain=domain)
             if isinstance(outputs, Sequence):
                 value.name = outputs[0]
             return value
         values = self._tape.op_multi_output(
             op_type, inputs=inputs, attributes=kwargs, domain=domain, num_outputs=num_outputs
@@ -655,14 +840,22 @@
 
     match: MatchResult
     new_outputs: Sequence[ir.Value]
     new_nodes: Sequence[ir.Node]
     used_opsets: UsedOpsets
 
 
+def always_true(*args, **kwargs) -> bool:
+    """A condition function that always returns True.
+
+    This is used when no condition function is provided for a rewrite rule.
+    """
+    return True
+
+
 class ReplacementPatternFunction:
     """The replacement pattern that will replace the targeted pattern.
 
     Attributes:
         function (Callable): The replacement function that will be used to replace the matched pattern.
     """
 
@@ -690,114 +883,149 @@
         elif version is not None and version != imports[domain]:
             raise ValueError(
                 f"Multiple versions of opset {domain} used. "
                 f"Expected version {imports[domain]}, but got {version}."
             )
 
 
+class PatternMatcher(abc.ABC):
+    def __init__(self, pattern: GraphPattern) -> None:
+        self.pattern = pattern
+
+    @abc.abstractmethod
+    def match(
+        self,
+        model: ir.Model,
+        graph_or_function: ir.Graph | ir.Function,
+        node: ir.Node,
+        verbose: int = 0,
+    ) -> MatchResult:
+        pass
+
+    def __str__(self) -> str:
+        return str(self.pattern)
+
+
+class SimplePatternMatcher(PatternMatcher):
+    def __init__(self, pattern: GraphPattern) -> None:
+        assert (
+            pattern.has_single_output_node
+        ), "SimplePatternMatcher only supports patterns with a single output node."
+        super().__init__(pattern)
+
+    def match(
+        self,
+        model: ir.Model,
+        graph_or_function: ir.Graph | ir.Function,
+        node: ir.Node,
+        verbose: int = 0,
+    ) -> MatchResult:
+        # TODO(rama): support verbose
+        del model
+        del graph_or_function
+        if len(node.outputs) != self.pattern.num_outputs:
+            return MatchResult.FAIL()
+        match = self.pattern.matches_subgraph(node)
+        if not match:
+            return MatchResult.FAIL()
+        if not _valid_to_replace(match.nodes):
+            return MatchResult.FAIL()
+        match.outputs.extend(node.outputs)
+        return match
+
+
 class RewriteRule:
     def __init__(
         self,
-        target_pattern: GraphPattern | Callable | None = None,
-        replacement_pattern: ReplacementPatternFunction | Callable | None = None,
+        target_pattern: GraphPattern | Callable,
+        replacement_pattern: ReplacementPatternFunction | Callable,
         condition_function: Callable | None = None,
+        matcher: PatternMatcher | None = None,
+        verbose: int = 0,
     ) -> None:
         """Create a rewrite rule.
 
         Args:
             target_pattern: The pattern function that will be
                 matched against the IR.
             replacement_pattern: The replacement function that
                 will be used to replace the matched pattern.
             condition_function: The condition function that
                 will be used to check if the pattern matches the IR with ir.Values
                 constraints in consideration.
-
+            matcher: The pattern matcher that will be used to match the pattern.
+                If not provided, a default matcher will be used.
+            verbose: The verbosity level of the rule.
         """
-        if target_pattern is None:
-            # NOTE: this is a default-constructor. Caller responsible for filling in the fields.
-            assert replacement_pattern is None
-            assert condition_function is None
-            return
-        elif replacement_pattern is None:
-            raise ValueError(
-                "replacement_pattern must be provided if target_pattern is provided"
-            )
 
         if not isinstance(target_pattern, GraphPattern):
             target_pattern = _to_graph_pattern(target_pattern)
         self._target_pattern = target_pattern
 
         if not isinstance(replacement_pattern, ReplacementPatternFunction):
             replacement_pattern = ReplacementPatternFunction(replacement_pattern)
         self._replacement_pattern = replacement_pattern
-        self._condition_function = condition_function
+        self._condition_function = condition_function or always_true
+        if matcher is None:
+            if target_pattern.has_single_output_node:
+                matcher = SimplePatternMatcher(self._target_pattern)
+            else:
+                import onnxscript.rewriter.generic_pattern as generic_pattern
 
-    def matches(self, node: ir.Node, model: ir.Model) -> MatchResult:
-        """Check if the node from IR matches the pattern."""
-        if len(node.outputs) != self._target_pattern.num_outputs:
-            return MatchResult.FAIL()
-        match = self._target_pattern.matches_node(node)
-        if (
-            self._condition_function is not None
-            and match
-            and not self._condition_function(**match.bindings)
-        ):
-            return MatchResult.FAIL()
-        match.outputs.extend(node.outputs)
-        return match
+                matcher = generic_pattern.GenericPatternMatcher(self._target_pattern)
+        self._matcher = matcher
+        self._verbose = verbose
 
     def try_rewrite(
         self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
     ) -> ReplacementSubgraph | None:
         """If the node matches the pattern, then replace the node with the replacement pattern."""
-        match = self.matches(node, model)
+        match = self._matcher.match(model, graph_or_function, node, verbose=self._verbose)
         if match:
-            assert match.nodes is not None, "Matched values should not be None."
-            if _valid_to_replace(match.nodes):
-                replacement_subgraph = self._replacement_pattern.get_replacement(match)
-                if replacement_subgraph is None:
-                    return None
-                if len(replacement_subgraph.new_outputs) != self._target_pattern.num_outputs:
-                    raise ValueError(
-                        f"Number of outputs from replacement function does not match the number of outputs from the target pattern. "
-                        f"Expected {self._target_pattern.num_outputs}, but got {len(replacement_subgraph.new_outputs)}."
-                    )
-                # TODO(rama): Check/update opset-imports
-                # (i) Following is required by multi-output matcher too; move this.
-                # (ii) Remove the opset imports from deleted nodes?
-                _update_opset_imports(graph_or_function, replacement_subgraph)
-                _update_opset_imports(model.graph, replacement_subgraph)
-                return replacement_subgraph
+            context = None  # TODO(rama)
+            if not self._condition_function(context, **match.bindings):
+                return None
+            replacement_subgraph = self._replacement_pattern.get_replacement(match)
+            if replacement_subgraph is None:
+                return None
+            if len(replacement_subgraph.new_outputs) != self._target_pattern.num_outputs:
+                raise ValueError(
+                    f"Number of outputs from replacement function does not match the number of outputs from the target pattern. "
+                    f"Expected {self._target_pattern.num_outputs}, but got {len(replacement_subgraph.new_outputs)}."
+                )
+            # TODO(rama): Remove the opset imports from deleted nodes?
+            _update_opset_imports(graph_or_function, replacement_subgraph)
+            _update_opset_imports(model.graph, replacement_subgraph)
+            return replacement_subgraph
         return None
 
     def apply_to_model(self, model: ir.Model, *, commute: bool = False):
         # TODO(titaiwang): Why do we need RewriteRuleSet?
         return RewriteRuleSet([self], commute=commute).apply_to_model(model)
 
-    def count_matches(self, model: ir.Model, *, commute: bool = False):
-        return RewriteRuleSet([self], commute=commute).count_matches(model)
-
     def commute(self) -> Sequence[RewriteRule]:
         def replace_pattern(new_pattern):
             """Return a shallow copy of self with node_pattern replaced by new_pattern."""
-            rule = RewriteRule()
-            rule._condition_function = self._condition_function
-            rule._target_pattern = new_pattern
-            rule._replacement_pattern = self._replacement_pattern
-            return rule
+            # TODO(rama): Maybe we should use a better alternative to construct new matcher.
+            matcher_class = type(self._matcher)
+            return RewriteRule(
+                new_pattern,
+                self._replacement_pattern,
+                self._condition_function,
+                matcher_class(new_pattern),
+                self._verbose,
+            )
 
         return [replace_pattern(p) for p in self._target_pattern.commute()]
 
 
 def _apply_delta(
     graph_or_function: ir.Graph | ir.Function,
     node: ir.Node,
-    # TODO(jutinchuby): Use a more descriptive data structure to store deltas
-    delta,
+    delta: ReplacementSubgraph,
 ):
     """Applies delta.
 
     This code is valid is the considered pattern has only one output.
     In case of multi output replacements, there is not need to rename
     the outputs.
 
@@ -809,61 +1037,41 @@
 
     The current implementation insert all the nodes at the same position
     but checks there is not inconsistency. In that case, it fails.
     We could reorder (long) or do more clever changes.
     The reordering would probably happen not very often.
     """
 
-    if isinstance(delta, tuple):
-        # multi-output strategy
-        n_matches, matched_nodes, inserted_nodes = delta
-
-        # TODO(rama): Was "assert i not in to_insert"; seems wrong.
-        # What is this trying to check? Best effort correction below.
-        assert node not in inserted_nodes  # conflicts should avoid that case
-
-        graph_or_function.insert_after(node, inserted_nodes)
-        # TODO: improve this
-        # This is updating the graph/function outputs to use the new outputs
-        for inserted_node in inserted_nodes:
-            for new_output in inserted_node.outputs:
-                if (index := new_output.meta.get(_ir_utils.GRAPH_OUTPUT_META_KEY)) is not None:  # type: ignore[assignment]
-                    graph_or_function.outputs[index] = new_output
-
-        for d in matched_nodes:
-            assert d in graph_or_function
-        graph_or_function.remove(matched_nodes, safe=True)
-    else:
-        assert isinstance(delta, ReplacementSubgraph)
-        # Replace matched nodes with new nodes, matched values with new values
-        old_values = delta.match.outputs
-        new_values = delta.new_outputs
-
-        for old_value, new_value in zip(old_values, new_values):
-            # Propagate relevant info from old value to new value
-            # TODO(Rama): Perhaps we should merge old and new types. As of now, new
-            # values don't have type information. Note that this could be a problem
-            # for semantics-altering rewrite-rules: we should allow users to override
-            # this for such rules.
-            new_value.type = old_value.type
-            new_value.shape = old_value.shape
-            new_value.const_value = old_value.const_value
-            new_value.name = old_value.name
-
-        # Reconnect the users of the deleted node to use the new outputs
-        _convenience.replace_all_uses_with(old_values, new_values)
-        # Update graph/function outputs if the node generates output
-        replacement_mapping = dict(zip(old_values, new_values))
-        for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
-            if graph_or_function_output in replacement_mapping:
-                graph_or_function.outputs[idx] = replacement_mapping[graph_or_function_output]
-
-        # insert new nodes after the index node
-        graph_or_function.insert_after(node, delta.new_nodes)
-        graph_or_function.remove(delta.match.nodes, safe=True)
+    assert isinstance(delta, ReplacementSubgraph)
+    # Replace matched nodes with new nodes, matched values with new values
+    old_values = delta.match.outputs
+    new_values = delta.new_outputs
+
+    for old_value, new_value in zip(old_values, new_values):
+        # Propagate relevant info from old value to new value
+        # TODO(Rama): Perhaps we should merge old and new types. As of now, new
+        # values don't have type information. Note that this could be a problem
+        # for semantics-altering rewrite-rules: we should allow users to override
+        # this for such rules.
+        new_value.type = old_value.type
+        new_value.shape = old_value.shape
+        new_value.const_value = old_value.const_value
+        new_value.name = old_value.name
+
+    # Reconnect the users of the deleted node to use the new outputs
+    _convenience.replace_all_uses_with(old_values, new_values)
+    # Update graph/function outputs if the node generates output
+    replacement_mapping = dict(zip(old_values, new_values))
+    for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
+        if graph_or_function_output in replacement_mapping:
+            graph_or_function.outputs[idx] = replacement_mapping[graph_or_function_output]
+
+    # insert new nodes after the index node
+    graph_or_function.insert_after(node, delta.new_nodes)
+    graph_or_function.remove(delta.match.nodes, safe=True)
 
 
 class RewriteRuleSet:
     def __init__(self, rules: Sequence[RewriteRule], *, commute: bool = False) -> None:
         if commute:
             rules = list(itertools.chain.from_iterable([rule.commute() for rule in rules]))
         self.rules = rules
@@ -889,28 +1097,7 @@
 
     def apply_to_model(self, model: ir.Model) -> int:
         assert isinstance(model, ir.Model)
         count = self._apply_to_graph_or_function(model, model.graph)
         for function in model.functions.values():
             count += self._apply_to_graph_or_function(model, function)
         return count
-
-    def _count_matches_in_graph_or_function(
-        self, model: ir.Model, graph_or_function: ir.Graph | ir.Function
-    ) -> int:
-        count = 0
-        for node in graph_or_function:
-            for rule in self.rules:
-                if rule.matches(node, model):
-                    count += 1
-                    break
-        return count
-
-    def count_matches(self, model: onnx.ModelProto | ir.Model):
-        if isinstance(model, onnx.ModelProto):
-            model = ir.serde.deserialize_model(model)
-        else:
-            assert isinstance(model, ir.Model)
-        count = self._count_matches_in_graph_or_function(model, model.graph)
-        for function in model.functions.values():
-            count += self._count_matches_in_graph_or_function(model, function)
-        return count
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240511/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240511/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240511/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240511/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240511/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript/values.py` & `onnxscript-0.1.0.dev20240511/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240511/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240510
+Version: 0.1.0.dev20240511
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b4dd7774f166e46984aebc6d3626cd5edae3dcd5
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/32bcd064d0fd94ee40e358b419589388d7ffe360
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240510/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240511/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/pyproject.toml` & `onnxscript-0.1.0.dev20240511/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240510/setup.py` & `onnxscript-0.1.0.dev20240511/setup.py`

 * *Files identical despite different names*

