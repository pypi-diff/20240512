# Comparing `tmp/fim-utils-1.7.0b1.tar.gz` & `tmp/fim-utils-1.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim-utils-1.7.0b1.tar", last modified: Sat May 11 02:54:36 2024, max compression
+gzip compressed data, was "fim-utils-1.7.0b2.tar", last modified: Sun May 12 19:25:26 2024, max compression
```

## Comparing `fim-utils-1.7.0b1.tar` & `fim-utils-1.7.0b2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.7.0b1/.gitignore
--rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.7.0b1/LICENSE
--rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.7.0b1/MANIFEST.in
--rw-r--r--   0        0        0     8671 2024-05-11 02:27:13.133092 fim-utils-1.7.0b1/README.md
--rw-r--r--   0        0        0      158 2024-05-11 02:47:18.942023 fim-utils-1.7.0b1/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.7.0b1/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.7.0b1/fimutil/al2s/al2s.conf.template
--rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.7.0b1/fimutil/al2s/al2s_api.py
--rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.7.0b1/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.7.0b1/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.7.0b1/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    21817 2024-05-10 08:58:33.558511 fim-utils-1.7.0b1/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.7.0b1/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.7.0b1/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.7.0b1/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3478 2024-05-10 17:29:54.447929 fim-utils-1.7.0b1/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.7.0b1/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.7.0b1/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    25789 2024-05-11 02:02:54.660722 fim-utils-1.7.0b1/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.7.0b1/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.7.0b1/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.7.0b1/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.7.0b1/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1998 2024-05-10 21:42:05.649139 fim-utils-1.7.0b1/fimutil/ralph/p4_switch.py
--rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.7.0b1/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     8381 2024-05-10 20:05:45.369295 fim-utils-1.7.0b1/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.7.0b1/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    11349 2024-05-11 02:27:13.139125 fim-utils-1.7.0b1/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.7.0b1/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.7.0b1/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.7.0b1/fimutil/utilities/scan_al2s.py
--rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.7.0b1/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.7.0b1/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.7.0b1/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1032 2024-05-10 20:47:11.260720 fim-utils-1.7.0b1/pyproject.toml
--rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.7.0b1/setup.py
--rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.7.0b1/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.7.0b1/test/netam_test.py
--rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.7.0b1/test/ralph_test.py
--rw-r--r--   0        0        0     9397 1970-01-01 00:00:00.000000 fim-utils-1.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.7.0b2/.gitignore
+-rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.7.0b2/LICENSE
+-rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.7.0b2/MANIFEST.in
+-rw-r--r--   0        0        0     8671 2024-05-11 02:27:13.133092 fim-utils-1.7.0b2/README.md
+-rw-r--r--   0        0        0      158 2024-05-12 19:19:59.482720 fim-utils-1.7.0b2/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.7.0b2/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.7.0b2/fimutil/al2s/al2s.conf.template
+-rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.7.0b2/fimutil/al2s/al2s_api.py
+-rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.7.0b2/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.7.0b2/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.7.0b2/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    21817 2024-05-10 08:58:33.558511 fim-utils-1.7.0b2/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.7.0b2/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.7.0b2/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.7.0b2/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3478 2024-05-10 17:29:54.447929 fim-utils-1.7.0b2/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.7.0b2/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.7.0b2/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    25892 2024-05-12 19:22:30.018036 fim-utils-1.7.0b2/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.7.0b2/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.7.0b2/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.7.0b2/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.7.0b2/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1974 2024-05-12 17:01:53.392063 fim-utils-1.7.0b2/fimutil/ralph/p4_switch.py
+-rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.7.0b2/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     8381 2024-05-10 20:05:45.369295 fim-utils-1.7.0b2/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.7.0b2/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    11349 2024-05-11 02:27:13.139125 fim-utils-1.7.0b2/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.7.0b2/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.7.0b2/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.7.0b2/fimutil/utilities/scan_al2s.py
+-rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.7.0b2/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.7.0b2/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.7.0b2/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1032 2024-05-12 19:19:31.473571 fim-utils-1.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.7.0b2/setup.py
+-rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.7.0b2/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.7.0b2/test/netam_test.py
+-rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.7.0b2/test/ralph_test.py
+-rw-r--r--   0        0        0     9397 1970-01-01 00:00:00.000000 fim-utils-1.7.0b2/PKG-INFO
```

### Comparing `fim-utils-1.7.0b1/.gitignore` & `fim-utils-1.7.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/LICENSE` & `fim-utils-1.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/README.md` & `fim-utils-1.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/al2s/al2s_api.py` & `fim-utils-1.7.0b2/fimutil/al2s/al2s_api.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/al2s/arm.py` & `fim-utils-1.7.0b2/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/al2s/cloud_cfg.py` & `fim-utils-1.7.0b2/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/netam/arm.py` & `fim-utils-1.7.0b2/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/netam/nso.py` & `fim-utils-1.7.0b2/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/netam/sr_pce.py` & `fim-utils-1.7.0b2/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/asset.py` & `fim-utils-1.7.0b2/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/dp_switch.py` & `fim-utils-1.7.0b2/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/ethernetport.py` & `fim-utils-1.7.0b2/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/fim_helper.py` & `fim-utils-1.7.0b2/fimutil/ralph/fim_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,22 +500,23 @@
     # create p4 switch with interfaces and links back to dataplane switch ports
     logging.debug('Adding p4 switch')
     if site.p4_switch is None:
         logging.info(f'P4 Switch was not detected/catalogued')
         return topo
 
     # this prefers an IP address, but uses S/N if IP is None (like in GENI racks)
-    logging.info(f'Adding P4 switch {site.name}')
+    logging.debug(f'Adding P4 switch {site.name}')
 
     p4_name = p4_switch_name_id(real_switch_site.lower(),
                                 site.p4_switch.fields['IP'] if site.p4_switch.fields['IP'] else site.p4_switch.fields['SN'])
-
+    logging.info(f'Adding P4 switch {p4_name}')
     p4 = topo.add_node(name=p4_name[0],
                        node_id=p4_name[1],
-                       site=site.name, ntype=NodeType.Switch, stitch_node=True)
+                       site=site.name, ntype=NodeType.Switch, stitch_node=False,
+                       capacities=Capacities(unit=1))
 
     p4_service_type = ServiceType.MPLS
     p4_ns = p4.add_network_service(name=p4.name + '-ns', node_id=p4.node_id + '-ns',
                                    nstype=p4_service_type, stitch_node=False)
 
     dp_to_p4_ports = []
```

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/fpga.py` & `fim-utils-1.7.0b2/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/gpu.py` & `fim-utils-1.7.0b2/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/model.py` & `fim-utils-1.7.0b2/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/nvme.py` & `fim-utils-1.7.0b2/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/p4_switch.py` & `fim-utils-1.7.0b2/fimutil/ralph/p4_switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pyjq
 import logging
-from typing import List
 
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.asset import RalphAsset, RalphAssetType, RalphAssetMimatch
 from fimutil.ralph.model import SimpleModel
 from fimutil.ralph.ethernetport import EthernetPort
```

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/ralph_uri.py` & `fim-utils-1.7.0b2/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/site.py` & `fim-utils-1.7.0b2/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/storage.py` & `fim-utils-1.7.0b2/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/ralph/worker_node.py` & `fim-utils-1.7.0b2/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/utilities/generate_instance_flavors.py` & `fim-utils-1.7.0b2/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/utilities/scan_al2s.py` & `fim-utils-1.7.0b2/fimutil/utilities/scan_al2s.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/utilities/scan_net.py` & `fim-utils-1.7.0b2/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/utilities/scan_site.py` & `fim-utils-1.7.0b2/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/fimutil/utilities/scan_worker.py` & `fim-utils-1.7.0b2/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/pyproject.toml` & `fim-utils-1.7.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License",
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent"]
 dynamic = ["version", "description"]
 requires-python = '>=3.9'
 dependencies = [
-	"fabric_fim >= 1.7.0b1",
+	"fabric_fim >= 1.7.0b2",
     "pyjq == 2.6.0",
 	"jsonpath_ng == 1.5.3",
 	]
 
 [tool.flit.module]
 name = "fimutil"
```

### Comparing `fim-utils-1.7.0b1/setup.py` & `fim-utils-1.7.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/test/al2s_test.py` & `fim-utils-1.7.0b2/test/al2s_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/test/netam_test.py` & `fim-utils-1.7.0b2/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b1/PKG-INFO` & `fim-utils-1.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.7.0b1
+Version: 1.7.0b2
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Dist: fabric_fim >= 1.7.0b1
+Requires-Dist: fabric_fim >= 1.7.0b2
 Requires-Dist: pyjq == 2.6.0
 Requires-Dist: jsonpath_ng == 1.5.3
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flit ; extra == "test"
 Project-URL: Home, https://github.com/fabric-testbed/information-model-utils
 Provides-Extra: test
```

