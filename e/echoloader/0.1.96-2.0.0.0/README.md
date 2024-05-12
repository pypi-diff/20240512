# Comparing `tmp/echoloader-0.1.96.tar.gz` & `tmp/echoloader-2.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoloader-0.1.96.tar", max compression
+gzip compressed data, was "echoloader-2.0.0.0.tar", max compression
```

## Comparing `echoloader-0.1.96.tar` & `echoloader-2.0.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       24 2024-04-19 14:36:43.618282 echoloader-0.1.96/echoloader/__init__.py
--rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-0.1.96/echoloader/__main__.py
--rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-0.1.96/echoloader/config.py
--rw-r--r--   0        0        0     1856 2024-02-13 06:10:05.802876 echoloader-0.1.96/echoloader/dimse/__init__.py
--rw-r--r--   0        0        0     3125 2024-02-13 06:10:05.804882 echoloader-0.1.96/echoloader/dimse/dimse.py
--rw-r--r--   0        0        0      882 2024-02-13 06:10:05.805881 echoloader-0.1.96/echoloader/dimse/fs.py
--rw-r--r--   0        0        0      367 2024-02-13 06:10:05.807885 echoloader-0.1.96/echoloader/dimse/store.py
--rw-r--r--   0        0        0     2141 2024-02-13 06:10:05.808881 echoloader-0.1.96/echoloader/dimse/tls.py
--rw-r--r--   0        0        0    11166 2024-02-13 06:10:05.810887 echoloader-0.1.96/echoloader/lib/hl7.py
--rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-0.1.96/echoloader/login.py
--rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-0.1.96/echoloader/qt.py
--rw-r--r--   0        0        0    17177 2024-04-19 06:41:21.735964 echoloader-0.1.96/echoloader/results_sync/__init__.py
--rw-r--r--   0        0        0     2937 2024-02-13 06:10:05.818041 echoloader-0.1.96/echoloader/results_sync/hl7_sync.py
--rw-r--r--   0        0        0     4724 2024-03-23 07:31:12.577918 echoloader-0.1.96/echoloader/sync.py
--rw-r--r--   0        0        0    41608 2024-04-19 14:36:43.619293 echoloader-0.1.96/echoloader/watcher.py
--rw-r--r--   0        0        0      849 2024-04-19 14:36:43.624300 echoloader-0.1.96/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 echoloader-0.1.96/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-05-12 10:16:33.095644 echoloader-2.0.0.0/echoloader/__init__.py
+-rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-2.0.0.0/echoloader/__main__.py
+-rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-2.0.0.0/echoloader/config.py
+-rw-r--r--   0        0        0     1892 2024-05-10 04:56:58.818889 echoloader-2.0.0.0/echoloader/dimse/__init__.py
+-rw-r--r--   0        0        0     3355 2024-05-10 04:56:58.822043 echoloader-2.0.0.0/echoloader/dimse/dimse.py
+-rw-r--r--   0        0        0      882 2024-05-08 09:01:09.949355 echoloader-2.0.0.0/echoloader/dimse/fs.py
+-rw-r--r--   0        0        0      367 2024-05-08 09:01:09.951380 echoloader-2.0.0.0/echoloader/dimse/store.py
+-rw-r--r--   0        0        0     2141 2024-05-08 09:01:09.953390 echoloader-2.0.0.0/echoloader/dimse/tls.py
+-rw-r--r--   0        0        0    11327 2024-05-10 04:56:58.824282 echoloader-2.0.0.0/echoloader/lib/hl7.py
+-rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-2.0.0.0/echoloader/login.py
+-rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-2.0.0.0/echoloader/qt.py
+-rw-r--r--   0        0        0    19592 2024-05-10 18:02:00.449867 echoloader-2.0.0.0/echoloader/results_sync/__init__.py
+-rw-r--r--   0        0        0     2946 2024-05-10 04:56:58.829317 echoloader-2.0.0.0/echoloader/results_sync/hl7_sync.py
+-rw-r--r--   0        0        0     3284 2024-05-10 04:56:58.831350 echoloader-2.0.0.0/echoloader/results_sync/pdf_sc.py
+-rw-r--r--   0        0        0     4724 2024-05-08 09:01:09.970144 echoloader-2.0.0.0/echoloader/sync.py
+-rw-r--r--   0        0        0    42125 2024-05-10 04:56:58.833507 echoloader-2.0.0.0/echoloader/watcher.py
+-rw-r--r--   0        0        0      871 2024-05-12 10:16:33.100658 echoloader-2.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 echoloader-2.0.0.0/PKG-INFO
```

### Comparing `echoloader-0.1.96/echoloader/config.py` & `echoloader-2.0.0.0/echoloader/config.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/dimse/__init__.py` & `echoloader-2.0.0.0/echoloader/dimse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def detail_to_destination(sync_details, **kwargs):
     details = sync_details.split('&')
     parts = details[0].split(':')
     sync_destination = {
         'id': str(uuid.uuid4()),
         'sync_modalities': details[1].split(',') if len(details) > 1 else kwargs.get('sync_modalities', ['SR']),
         'sync_source': 'ECHOLOADER',
+        'sync_event': 'REAL_TIME',
     }
     if len(parts) == 1:
         sync_destination['path'] = parts[0]
     elif len(parts) > 2:
         sync_destination['host'] = parts[0]
         sync_destination['port'] = parts[1]
         sync_destination['remote_ae_title'] = parts[2]
```

### Comparing `echoloader-0.1.96/echoloader/dimse/dimse.py` & `echoloader-2.0.0.0/echoloader/dimse/dimse.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,15 +55,20 @@
                 cx._as_scp = True
 
             status = assoc.send_c_store(ds)
 
             # Check the status of the storage request
             if status:
                 # If the storage request succeeded this will be 0x0000
+                if status.Status == 0x0000:
+                    logger.debug('C-STORE completed successfully')
+                    return
+
                 logger.debug(f'C-STORE request status: 0x{status.Status:04x}')
+                raise ValueError(f'C-STORE failed with status 0x{status.Status:04x}')
             else:
                 raise ValueError('Connection timed out, was aborted or received invalid response')
         finally:
             # Release the association
             assoc.release()
 
     def __str__(self):
```

### Comparing `echoloader-0.1.96/echoloader/dimse/fs.py` & `echoloader-2.0.0.0/echoloader/dimse/fs.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/dimse/tls.py` & `echoloader-2.0.0.0/echoloader/dimse/tls.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/lib/hl7.py` & `echoloader-2.0.0.0/echoloader/lib/hl7.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         vendor_config = self.vendor_config
 
         logger.debug("HL7 generation started")
 
         is_invalid_report_doc = not report_doc_encoded
         is_invalid_measurements = not measurements or len(measurements) == 0
 
-        if report_type in ["PDF", "DOCX"] and is_invalid_report_doc:
+        if report_type in ["PDF", "DOCX", "RTF"] and is_invalid_report_doc:
             logger.warning("Failed to generate HL7 - Report DOC is invalid")
             return False
 
         if report_type == "TEXT" and is_invalid_measurements:
             logger.warning("Failed to generate HL7 - Invalid measurements")
             return False
 
@@ -118,29 +118,31 @@
         message.obr.obr_22 = pd_formatted  # Approved Date & Time
         message.obr.obr_24 = ""  # Modality
         # https://hl7-definition.caristix.com/v2/HL7v2.5/Tables/0123
         message.obr.obr_25 = "R"  # Result status - F - Final, R - store, but not verified, etc..,
         message.obr.obr_31 = ""  # Study desc
 
         obx_index = 1
-        is_doc_requested = report_type in ["ALL", "PDF", "DOCX"]
+        is_doc_requested = report_type in ["ALL", "PDF", "DOCX", "RTF"]
 
         if not is_invalid_report_doc and is_doc_requested:
             logger.debug("Embedding Report PDF into OBX")
 
             obx = Segment("OBX")
             obx.obx_1 = str(obx_index)  # Observation Set ID
             obx.obx_2 = "ED"  # Observation Set ID
             obx.obx_3.obx_3_1 = ""  # Observation Identifier
             obx.obx_3.obx_3_2 = ""  # Study desc
 
             if vendor_config.get("report_pdf_format", "SIMPLE") == "SIMPLE":
                 obx.obx_5 = report_doc_encoded  # Observation result
             else:
-                obx.obx_5 = f"{'docx' if report_type == 'DOCX' else 'pdf'}^TEXT^^Base64^{report_doc_encoded}"
+                obx_report_type = report_type.lower()
+                obx_report_type = "pdf" if obx_report_type not in ["docx", "rtf"] else obx_report_type
+                obx.obx_5 = f"{obx_report_type}^TEXT^^Base64^{report_doc_encoded}"
 
             # Observation result status https://hl7-definition.caristix.com/v2/HL7v2.5/Tables/0085
             obx.obx_11 = report_status
             obx.obx_14 = study_dt  # Observation Date & Time
             obx.obx_19 = pd_formatted
 
             message.add(obx)
@@ -245,15 +247,15 @@
                 logger.error(f'Failed to send HL7(SFTP): {self.msg_control_id}, {vendor_config.get("host")}, ex: {ex}')
 
         elif vendor_config.get("transfer_mode") == "FILE":
             hl7_string = self.message.to_er7()
 
             try:
                 full_path = os.path.join(vendor_config.get("root_path"), f"{self.msg_control_id}.hl7")
-                file = open(full_path, "a")
-                file.write(hl7_string)
-                file.close()
+                with open(full_path, "a") as file:
+                    file.write(hl7_string)
+                    file.close()
 
                 logger.info(f'HL7(File) was written successfully.. ID: {self.msg_control_id}, File: {full_path}')
 
             except Exception as ex:
                 logger.error(f'Failed to write HL7. ID: {self.msg_control_id}, {vendor_config.get("host")}, ex: {ex}')
```

### Comparing `echoloader-0.1.96/echoloader/login.py` & `echoloader-2.0.0.0/echoloader/login.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/qt.py` & `echoloader-2.0.0.0/echoloader/qt.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/results_sync/__init__.py` & `echoloader-2.0.0.0/echoloader/results_sync/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 import datetime
 import io
 import logging
 from collections import defaultdict
 from functools import cached_property
 
+import numpy as np
 import requests
 from dateutil import parser
+from fitz import fitz
 from pydicom import dcmread
 from pydicom.uid import generate_uid
 
 from echoloader.dimse import destination_to_store
 from echoloader.login import unpack
 from echoloader.results_sync.hl7_sync import Hl7Sync
+from echoloader.results_sync.pdf_sc import generate_pdf_sc
 
 logger = logging.getLogger('echolog')
 
 RESULT_FETCH_RETRIES = 3
 
 
+def apply_overwrites(overwrites, ds, modality):
+    for o in overwrites:
+        m, rest = o.split(':', 1)
+        if m == modality:
+            k, v = rest.split('=', 1)
+            if k.endswith('UID'):
+                v = generate_uid(prefix=v)
+            setattr(ds, k, v)
+
+
 class ResultsSync:
     def __init__(self, study, args, **kwargs):
         self.study = study
         self.args = args
         self.sid = str(study.get('id'))
 
         self.protocol = kwargs.get('protocol', {})
@@ -33,14 +46,15 @@
         self.api_url = kwargs.get('api_url', '')
         self.headers = kwargs.get('headers', {})
         self.db_mods = kwargs.get('mods', {})
         self.params = kwargs.get('params', {})
         self.ds_retrieve_func = kwargs.get('ds_retrieve_func')
         self.pdf_retrieve_func = kwargs.get('pdf_retrieve_func')
         self.audit_func = kwargs.get('audit_func')
+        self.overwrite_tags = args.get('overwrite_tags', [])
 
         self.sr_params = {}
         self.doc_params = {}
         self.pdf_params = {}
         self.ps_params = {}
         self.sc_params = {}
         self.sync_status_success = defaultdict(list)
@@ -66,26 +80,29 @@
         if args.get('sync_edited_status'):
             self.sr_params['edited_status'] = True
         if args.get('sync_annotations'):
             self.sr_params['annotations'] = True
 
         self.doc_params['dicom_encapsulated_pdf'] = True
         self.by_measurement = args.get('sync_by_measurement', False)
+        self.sync_pdf_as_sc = args.get('sync_pdf_as_sc', False)
         self.sync_generate_uid = args.get('sync_generate_uid', False)
         self.hl7_config = self.dicom_router_config.get('hl7_config', {})
 
         self.grouped_ms = None
         self.sync_destinations = kwargs.get('sync_destinations', {})
 
     def find_realtime_destinations(self):
         self.grouped_ms = self.read_grouped_ms(not self.is_echoloader)
 
         # If the number of measurements to sync is greater than 0, sync to all destinations
         if len(self.grouped_ms) > 0:
             logger.debug(f'Found {len(self.grouped_ms)} new measurements for {self.study.get("visit", "")}')
+            if self.is_echoloader:
+                return list(filter(lambda x: x.get('sync_event', 'REAL_TIME') == 'REAL_TIME', self.sync_destinations))
             return self.sync_destinations
 
         logger.info(f'No new measurements for {self.study.get("visit", "")}')
         return []
 
     def find_trigger_destinations(self):
         try:
@@ -180,15 +197,38 @@
                     and m.get('used')
                     and m.get('dicom_id')
                     and m.get('plot_obj')):
                 k = (m['dicom_id'], m['frame'], *([m['id']] if self.by_measurement else []))
                 grouped_ms[k].append(m['id'])
         return grouped_ms
 
-    def sync_sc_ps(self, func):
+    def sync_sc(self, func):
+        for ms in self.grouped_ms.values():
+            yield func(ms)
+
+        if self.sync_pdf_as_sc and len(self.grouped_ms) > 0:
+            pdf_data = self.pdf()
+
+            if not pdf_data:
+                logger.error(f'Failed to fetch PDF for {self.study.get("visit", "")}')
+                return
+
+            doc_pdf = fitz.open(stream=pdf_data, filetype="pdf")
+            for i, page in enumerate(doc_pdf):
+                pixmap = page.get_pixmap()
+                pdf_page = pixmap.samples
+                image_array = (np.frombuffer(pdf_page, dtype=np.uint8)
+                               .reshape(pixmap.h, pixmap.w, len(pdf_page) // (pixmap.h * pixmap.w)))
+
+                ds = generate_pdf_sc(image_array, self.study, i)
+                yield func([], ds=ds)
+
+            doc_pdf.close()
+
+    def sync_ps(self, func):
         for ms in self.grouped_ms.values():
             yield func(ms)
 
     def ds(self):
         ds = self.dicoms
         for k, d in ds.items():
             if (not self.is_echoloader or (self.is_echoloader and d['last_update'] > self.last_sync)) and not d.get(
@@ -207,44 +247,67 @@
 
     def ps(self, ms):
         return {
             'url': f'{self.api_url}/dicom/ps',
             'params': {**self.params, **self.ps_params, 'measurements': ms},
         }
 
-    def sc(self, ms):
+    def sc(self, ms, ds=None):
         return {
+            'ds': ds,
             'url': f'{self.api_url}/dicom/sc',
             'params': {**self.params, **self.sc_params, 'measurements': ms},
         }
 
     def doc(self):
         return {
             'url': f'{self.api_url}/study/pdf/{self.sid}',
             'params': {**self.params, **self.doc_params},
         }
 
+    def pdf(self):
+        pdf_content = None
+
+        try:
+            if self.is_echoloader:
+                res = requests.get(f"{self.api_url}/study/pdf/{self.study.get('id')}", headers=self.headers,
+                                   params=self.pdf_params)
+                pdf_content = res.content if res.status_code == 200 else None
+                if res.status_code != 200:
+                    logger.error(f'Failed to fetch from {res.url} - {res.status_code}')
+            elif self.pdf_retrieve_func:
+                pdf_content = self.pdf_retrieve_func(self.pdf_params)
+
+            return pdf_content
+        except Exception as exc:
+            logger.error(f'Failed to fetch PDF due to {exc}')
+            return None
+
     def retrieve_ds(self, req_obj, modality):
+        if req_obj.get('ds'):
+            return req_obj.get('ds')
+
+        url = req_obj.get('url')
         if self.is_echoloader:
-            req = requests.get(req_obj.get('url'), headers=self.headers, params=req_obj.get('params'))
-            url = req.url
+            req = requests.get(url, headers=self.headers, params=req_obj.get('params'))
             try:
                 bs = unpack(req)
             except Exception as exc:
                 logger.error(f'Failed to fetch {url} due to {exc}')
                 raise exc
             ds = dcmread(io.BytesIO(bs))
-            if self.sync_generate_uid:
-                ds.SOPInstanceUID = generate_uid(
-                    prefix='1.2.826.0.1.3680043.10.918.', entropy_srcs=[f"{self.last_sync}{url}"])
-            return ds
+        elif self.ds_retrieve_func:
+            ds = self.ds_retrieve_func(modality, req_obj)
         else:
-            if self.ds_retrieve_func:
-                return self.ds_retrieve_func(modality, req_obj)
             return None
+        if self.sync_generate_uid:
+            ds.SOPInstanceUID = generate_uid(
+                prefix='1.2.826.0.1.3680043.10.918.', entropy_srcs=[f"{self.last_sync}{url}"])
+        apply_overwrites(self.overwrite_tags, ds, modality)
+        return ds
 
     def get_sync_summary(self, destination):
         return str(destination_to_store(destination))
 
     def update_sync_status(self, sync_destination, sync_status, error_summary):
         if self.is_echoloader:
             sync_log_id = sync_destination.get('sync_log_id')
@@ -301,16 +364,16 @@
                 self.audit_func(sync_log)
 
     def sync_study(self, destinations):
         modalities = [modality for destination in destinations for modality in destination.get('sync_modalities', [])]
         dimse_connections = [destination_to_store(sync_destination) for sync_destination in destinations]
 
         options = {
-            'PS': lambda: self.sync_sc_ps(self.ps),
-            'SC': lambda: self.sync_sc_ps(self.sc),
+            'PS': lambda: self.sync_ps(self.ps),
+            'SC': lambda: self.sync_sc(self.sc),
             'DS': lambda: self.ds(),
             'SR': lambda: [self.sr()],
             'DOC': lambda: [self.doc()],
         }
 
         for modality in list(dict.fromkeys(modalities)):
             for req_obj in options[modality]():
```

### Comparing `echoloader-0.1.96/echoloader/results_sync/hl7_sync.py` & `echoloader-2.0.0.0/echoloader/results_sync/hl7_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 }
         return measurements
 
     def pdf(self, report_type):
         pdf_content = None
 
         try:
-            if report_type == 'DOCX':
+            if report_type in ['DOCX', 'RTF']:
                 self.pdf_params['report_type'] = report_type
 
             if self.is_echoloader:
                 res = requests.get(f"{self.api_url}/study/pdf/{self.study.get('id')}", headers=self.headers,
                                    params=self.pdf_params)
                 pdf_content = res.content if res.status_code == 200 else None
                 if res.status_code != 200:
```

### Comparing `echoloader-0.1.96/echoloader/sync.py` & `echoloader-2.0.0.0/echoloader/sync.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.96/echoloader/watcher.py` & `echoloader-2.0.0.0/echoloader/watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,16 +836,28 @@
     parser.add_argument(
         '--sync-generate-uid',
         help='Generate a random SOPInstanceUID instead of using the deterministic UID from the backend',
         default=False,
         action='store_true',
     )
     parser.add_argument(
+        '--sync-pdf-as-sc',
+        help='Send PDF report pages as Secondary Captures',
+        default=False,
+        action='store_true',
+    )
+    parser.add_argument(
+        '--overwrite-tags',
+        help='Tags to override for specific output modalities, in the format MODALITY:TAG=VALUE',
+        nargs='*',
+        default=[],
+    )
+    parser.add_argument(
         '-v',
-        default='1.4.6',
+        default='2.0.0',
         help='Version of API to use',
     )
     parser.add_argument(
         '-y',
         default=False,
         action='store_true',
         help='Answer yes to all prompts',
@@ -895,18 +907,22 @@
         '--log',
         help='File for logs',
     )
     parser.add_argument(
         '--filter',
         help='Inclusive filter for DS files to process',
         default=[
-            'getattr(ds, "Modality", None) == "US"',  # Only accept ultrasound modalities
-            'getattr(ds, "Manufacturer", None) != "Us2.ai"',  # Filter recursive cases
-            'getattr(ds, "SequenceOfUltrasoundRegions", [])',  # Ensure ultrasound regions exists
-            'getattr(ds.SequenceOfUltrasoundRegions[0], "PhysicalDeltaX", 0)',  # Ensure we have scale
+            # Only accept ultrasound modalities
+            'getattr(ds, "Modality", None) in ["US", "SR"]',
+            # Filter recursive cases
+            'getattr(ds, "Manufacturer", None) != "Us2.ai"',
+            # Ensure ultrasound regions exists
+            'getattr(ds, "Modality", None) == "SR" or getattr(ds, "SequenceOfUltrasoundRegions", [])',
+            # Ensure we have scale
+            'getattr(ds, "Modality", None) == "SR" or getattr(ds.SequenceOfUltrasoundRegions[0], "PhysicalDeltaX", 0)',
         ],
         nargs='+',
     )
     parser.add_argument(
         '--src-glob',
         help='glob expression to apply on src directory',
         default='*',
```

### Comparing `echoloader-0.1.96/pyproject.toml` & `echoloader-2.0.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echoloader"
-version = "0.1.96"
+version = "2.0.0.0"
 description = ""
 authors = ["mathias <mathias@us2.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 requests = "^2.27.1"
 watchdog = "^2.1.7"
@@ -18,14 +18,15 @@
 imageio-ffmpeg = "0.4.9"
 av = "10.0.0"
 python-dateutil = "^2.8.2"
 pathy = "^0.10.2"
 pysftp = "^0.2.9"
 hl7apy = "^1.3.4"
 boto3 = "^1.28.62"
+pymupdf = "^1.24.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `echoloader-0.1.96/PKG-INFO` & `echoloader-2.0.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoloader
-Version: 0.1.96
+Version: 2.0.0.0
 Summary: 
 Author: mathias
 Author-email: mathias@us2.ai
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: av (==10.0.0)
@@ -12,14 +12,15 @@
 Requires-Dist: hl7apy (>=1.3.4,<2.0.0)
 Requires-Dist: imageio (==2.31.4)
 Requires-Dist: imageio-ffmpeg (==0.4.9)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: opencv-python-headless (>=4.5.5.64,<5.0.0.0)
 Requires-Dist: pathy (>=0.10.2,<0.11.0)
 Requires-Dist: pydicom (>=2.3.0,<3.0.0)
+Requires-Dist: pymupdf (>=1.24.2,<2.0.0)
 Requires-Dist: pynetdicom (>=2.0.2,<3.0.0)
 Requires-Dist: pysftp (>=0.2.9,<0.3.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-gdcm (>=3.0.12,<4.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: watchdog (>=2.1.7,<3.0.0)
```

