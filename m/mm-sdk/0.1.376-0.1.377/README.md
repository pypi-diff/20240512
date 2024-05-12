# Comparing `tmp/mm_sdk-0.1.376.tar.gz` & `tmp/mm_sdk-0.1.377.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_sdk-0.1.376.tar", max compression
+gzip compressed data, was "mm_sdk-0.1.377.tar", max compression
```

## Comparing `mm_sdk-0.1.376.tar` & `mm_sdk-0.1.377.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      943 2024-05-07 12:36:50.652160 mm_sdk-0.1.376/pyproject.toml
--rw-r--r--   0        0        0     1615 2023-09-04 18:13:32.000000 mm_sdk-0.1.376/sdk/__init__.py
--rw-r--r--   0        0        0     3260 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/admitad.py
--rw-r--r--   0        0        0     3235 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/analytics.py
--rw-r--r--   0        0        0      770 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/barcode_recognizer.py
--rw-r--r--   0        0        0      251 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/base.py
--rw-r--r--   0        0        0     3961 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/cash_register.py
--rw-r--r--   0        0        0      644 2023-09-04 18:13:32.000000 mm_sdk-0.1.376/sdk/click_again.py
--rw-r--r--   0        0        0     8565 2023-10-23 08:41:09.000000 mm_sdk-0.1.376/sdk/client.py
--rw-r--r--   0        0        0      714 2023-11-27 11:52:12.000000 mm_sdk-0.1.376/sdk/cryptopro.py
--rw-r--r--   0        0        0     2504 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/elk.py
--rw-r--r--   0        0        0     1661 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/face_detector.py
--rw-r--r--   0        0        0     5064 2024-05-07 12:28:07.000000 mm_sdk-0.1.376/sdk/gift.py
--rw-r--r--   0        0        0    20030 2024-05-07 12:28:07.000000 mm_sdk-0.1.376/sdk/gigtest.py
--rw-r--r--   0        0        0        0 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/mis/__init__.py
--rw-r--r--   0        0        0     3449 2023-11-27 11:52:12.000000 mm_sdk-0.1.376/sdk/mis/client.py
--rw-r--r--   0        0        0     3471 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/mis/crm.py
--rw-r--r--   0        0        0     3322 2023-09-04 18:13:32.000000 mm_sdk-0.1.376/sdk/mis/lab.py
--rw-r--r--   0        0        0     3630 2023-10-23 08:41:09.000000 mm_sdk-0.1.376/sdk/mis/lmk.py
--rw-r--r--   0        0        0     5188 2024-05-07 12:28:07.000000 mm_sdk-0.1.376/sdk/mis/mobil.py
--rw-r--r--   0        0        0      620 2023-11-27 11:52:12.000000 mm_sdk-0.1.376/sdk/mis/samd.py
--rw-r--r--   0        0        0     1295 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/mis/standalone.py
--rw-r--r--   0        0        0      577 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/mis/widgets.py
--rw-r--r--   0        0        0     4158 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/mobile_backend.py
--rw-r--r--   0        0        0      858 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/notemaster.py
--rw-r--r--   0        0        0     2878 2023-06-21 20:04:42.000000 mm_sdk-0.1.376/sdk/notification.py
--rw-r--r--   0        0        0     2607 2024-05-07 12:28:07.000000 mm_sdk-0.1.376/sdk/nsirosminzdrav.py
--rw-r--r--   0        0        0     5311 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/personal.py
--rw-r--r--   0        0        0    17080 2023-10-23 08:41:09.000000 mm_sdk-0.1.376/sdk/pre_record.py
--rw-r--r--   0        0        0     1740 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/prodoctorov.py
--rw-r--r--   0        0        0     1738 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/reestr.py
--rw-r--r--   0        0        0     1343 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/roistat.py
--rw-r--r--   0        0        0     4377 2024-05-07 12:28:07.000000 mm_sdk-0.1.376/sdk/samd.py
--rw-r--r--   0        0        0      961 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/site_mobilmed.py
--rw-r--r--   0        0        0      687 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/sms.py
--rw-r--r--   0        0        0        0 2023-10-23 08:41:09.000000 mm_sdk-0.1.376/sdk/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-10-23 08:41:09.000000 mm_sdk-0.1.376/sdk/utils/django_request_id.py
--rw-r--r--   0        0        0     5349 2022-12-01 10:21:55.000000 mm_sdk-0.1.376/sdk/yandex_courier.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.376/setup.py
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.376/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-05-12 13:18:54.076335 mm_sdk-0.1.377/pyproject.toml
+-rw-r--r--   0        0        0     1615 2023-08-28 20:35:53.000000 mm_sdk-0.1.377/sdk/__init__.py
+-rw-r--r--   0        0        0     3260 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/admitad.py
+-rw-r--r--   0        0        0     3235 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/analytics.py
+-rw-r--r--   0        0        0      770 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/barcode_recognizer.py
+-rw-r--r--   0        0        0      251 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/base.py
+-rw-r--r--   0        0        0     3961 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/cash_register.py
+-rw-r--r--   0        0        0      644 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/click_again.py
+-rw-r--r--   0        0        0     8565 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/client.py
+-rw-r--r--   0        0        0      714 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/cryptopro.py
+-rw-r--r--   0        0        0     2504 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/elk.py
+-rw-r--r--   0        0        0     1661 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/face_detector.py
+-rw-r--r--   0        0        0     4533 2024-05-12 13:13:31.000000 mm_sdk-0.1.377/sdk/gift.py
+-rw-r--r--   0        0        0    20030 2024-04-04 11:55:45.000000 mm_sdk-0.1.377/sdk/gigtest.py
+-rw-r--r--   0        0        0        0 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/mis/__init__.py
+-rw-r--r--   0        0        0     3449 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/mis/client.py
+-rw-r--r--   0        0        0     3471 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/mis/crm.py
+-rw-r--r--   0        0        0     3322 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/mis/lab.py
+-rw-r--r--   0        0        0     3630 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/mis/lmk.py
+-rw-r--r--   0        0        0     5188 2024-03-03 21:11:34.000000 mm_sdk-0.1.377/sdk/mis/mobil.py
+-rw-r--r--   0        0        0      620 2024-02-06 16:30:14.000000 mm_sdk-0.1.377/sdk/mis/samd.py
+-rw-r--r--   0        0        0     1295 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/mis/standalone.py
+-rw-r--r--   0        0        0      577 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/mis/widgets.py
+-rw-r--r--   0        0        0     4158 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/mobile_backend.py
+-rw-r--r--   0        0        0      858 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/notemaster.py
+-rw-r--r--   0        0        0     2878 2023-07-10 15:32:19.000000 mm_sdk-0.1.377/sdk/notification.py
+-rw-r--r--   0        0        0     2607 2024-04-04 12:17:02.000000 mm_sdk-0.1.377/sdk/nsirosminzdrav.py
+-rw-r--r--   0        0        0     5311 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/personal.py
+-rw-r--r--   0        0        0    17080 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/pre_record.py
+-rw-r--r--   0        0        0     1740 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/prodoctorov.py
+-rw-r--r--   0        0        0     1738 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/reestr.py
+-rw-r--r--   0        0        0     1343 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/roistat.py
+-rw-r--r--   0        0        0     4377 2024-05-12 13:13:31.000000 mm_sdk-0.1.377/sdk/samd.py
+-rw-r--r--   0        0        0      961 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/site_mobilmed.py
+-rw-r--r--   0        0        0      687 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/sms.py
+-rw-r--r--   0        0        0        0 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-11-02 10:40:21.000000 mm_sdk-0.1.377/sdk/utils/django_request_id.py
+-rw-r--r--   0        0        0     5349 2023-01-25 15:18:03.000000 mm_sdk-0.1.377/sdk/yandex_courier.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 mm_sdk-0.1.377/setup.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 mm_sdk-0.1.377/PKG-INFO
```

### Comparing `mm_sdk-0.1.376/pyproject.toml` & `mm_sdk-0.1.377/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mm-sdk"
-version = "0.1.376"
+version = "0.1.377"
 description = ""
 authors = ["dyus <dyuuus@gmail.com>"]
 packages = [
     { include = "sdk" },
 ]
 
 [build-system]
```

### Comparing `mm_sdk-0.1.376/sdk/__init__.py` & `mm_sdk-0.1.377/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/admitad.py` & `mm_sdk-0.1.377/sdk/admitad.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/analytics.py` & `mm_sdk-0.1.377/sdk/analytics.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/barcode_recognizer.py` & `mm_sdk-0.1.377/sdk/barcode_recognizer.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/cash_register.py` & `mm_sdk-0.1.377/sdk/cash_register.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/click_again.py` & `mm_sdk-0.1.377/sdk/click_again.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/client.py` & `mm_sdk-0.1.377/sdk/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/cryptopro.py` & `mm_sdk-0.1.377/sdk/cryptopro.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/elk.py` & `mm_sdk-0.1.377/sdk/elk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/face_detector.py` & `mm_sdk-0.1.377/sdk/face_detector.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/gift.py` & `mm_sdk-0.1.377/sdk/gift.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,18 @@
     percent = "percent"
 
 
 class GiftCodesRequest(BaseModel):
     code: str = None
     not_expired: bool = True
     is_promo: bool = True
-    support_percent_amount: bool = Field(
-        description="Флаг включающий работу с процентными промокодами", default=False
-    )
 
 
 class GiftCodeRequest(BaseModel):
     code: str
-    support_percent_amount: bool = Field(
-        description="Флаг включающий работу с процентными промокодами", default=False
-    )
 
 
 class GenerateCodeRequest(BaseModel):
     amount: int
     amount_type: AmountType
 
     class Config:
@@ -53,17 +47,14 @@
         description="Идентификатор заявки/предварительной записи связанной с заявкой. Без него промокод арендуется на краткое время"
     )
     source: str = Field(description="Источник, может быть любым текстом")
     cost: Optional[int] = Field(description="Цена без применения промокодов")
     visit_at: Optional[datetime.date] = Field(
         description="Нужна для проверки действителен, ли промокод на дату визита"
     )
-    support_percent_amount: bool = Field(
-        description="Флаг включающий работу с процентными промокодами", default=False
-    )
 
     class Config:
         use_enum_values = True
 
 
 class UnUseCode(BaseModel):
     code: str
```

### Comparing `mm_sdk-0.1.376/sdk/gigtest.py` & `mm_sdk-0.1.377/sdk/gigtest.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/client.py` & `mm_sdk-0.1.377/sdk/mis/client.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/crm.py` & `mm_sdk-0.1.377/sdk/mis/crm.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/lab.py` & `mm_sdk-0.1.377/sdk/mis/lab.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/lmk.py` & `mm_sdk-0.1.377/sdk/mis/lmk.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/mobil.py` & `mm_sdk-0.1.377/sdk/mis/mobil.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/samd.py` & `mm_sdk-0.1.377/sdk/mis/samd.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/standalone.py` & `mm_sdk-0.1.377/sdk/mis/standalone.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mis/widgets.py` & `mm_sdk-0.1.377/sdk/mis/widgets.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/mobile_backend.py` & `mm_sdk-0.1.377/sdk/mobile_backend.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/notemaster.py` & `mm_sdk-0.1.377/sdk/notemaster.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/notification.py` & `mm_sdk-0.1.377/sdk/notification.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/nsirosminzdrav.py` & `mm_sdk-0.1.377/sdk/nsirosminzdrav.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/personal.py` & `mm_sdk-0.1.377/sdk/personal.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/pre_record.py` & `mm_sdk-0.1.377/sdk/pre_record.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/prodoctorov.py` & `mm_sdk-0.1.377/sdk/prodoctorov.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/reestr.py` & `mm_sdk-0.1.377/sdk/reestr.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/roistat.py` & `mm_sdk-0.1.377/sdk/roistat.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/samd.py` & `mm_sdk-0.1.377/sdk/samd.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/site_mobilmed.py` & `mm_sdk-0.1.377/sdk/site_mobilmed.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/sms.py` & `mm_sdk-0.1.377/sdk/sms.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/sdk/yandex_courier.py` & `mm_sdk-0.1.377/sdk/yandex_courier.py`

 * *Files identical despite different names*

### Comparing `mm_sdk-0.1.376/setup.py` & `mm_sdk-0.1.377/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0', 'pydantic>=1.7.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mm-sdk',
-    'version': '0.1.376',
+    'version': '0.1.377',
     'description': '',
     'long_description': 'None',
     'author': 'dyus',
     'author_email': 'dyuuus@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mm_sdk-0.1.376/PKG-INFO` & `mm_sdk-0.1.377/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mm-sdk
-Version: 0.1.376
+Version: 0.1.377
 Summary: 
 Author: dyus
 Author-email: dyuuus@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

