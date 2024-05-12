# Comparing `tmp/python-amazon-sp-api-1.5.1.tar.gz` & `tmp/python-amazon-sp-api-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-sp-api-1.5.1.tar", last modified: Tue Apr 30 10:08:36 2024, max compression
+gzip compressed data, was "python-amazon-sp-api-1.5.2.tar", last modified: Sun May 12 08:10:45 2024, max compression
```

## Comparing `python-amazon-sp-api-1.5.1.tar` & `python-amazon-sp-api-1.5.2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.511584 python-amazon-sp-api-1.5.1/make_endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/make_endpoint/make_endpoint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.511584 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-30 10:08:36.000000 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-30 10:08:36.000000 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:08:36.000000 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 10:08:36.000000 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 10:08:36.000000 python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.511584 python-amazon-sp-api-1.5.1/sp_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.511584 python-amazon-sp-api-1.5.1/sp_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/aplus_content/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/aplus_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/aplus_content/aplus_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/application_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/application_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/application_management/application_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/authorization/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/catalog/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/catalog_items/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/catalog_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/catalog_items/catalog_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/data_kiosk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/data_kiosk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/data_kiosk/data_kiosk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/fba_inbound_eligibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fba_inbound_eligibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/fba_small_and_light/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fba_small_and_light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fba_small_and_light/fba_small_and_light.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/feeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/feeds/feeds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/finances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/finances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/finances/finances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_inbound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66400 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_inbound/fulfillment_inbound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_outbound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28743 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_outbound/fulfillment_outbound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/inventories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/inventories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/inventories/inventories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.515584 python-amazon-sp-api-1.5.1/sp_api/api/listings_items/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/listings_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/listings_items/listings_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/listings_restrictions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/listings_restrictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/listings_restrictions/listings_restrictions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/merchant_fulfillment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/merchant_fulfillment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/merchant_fulfillment/merchant_fulfillment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/messaging/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/notifications/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/orders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/orders/orders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/product_fees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/product_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/product_fees/product_fees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/product_type_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/product_type_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/product_type_definitions/product_type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/products/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/products/products.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/products/products_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/replenishment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/replenishment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/replenishment/replenishment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/reports/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/sales/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/sales/sales.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/sellers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/sellers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/sellers/sellers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/services/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.519584 python-amazon-sp-api-1.5.1/sp_api/api/shipping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14506 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/shipping/shipping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/solicitations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/solicitations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/solicitations/solicitations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/supply_sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/supply_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/supply_sources/supply_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/tokens/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/upload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/upload/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_orders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_payments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_shipping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28770 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_invoices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_invoices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_invoices/vendor_invoices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_orders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_orders/vendor_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_shipments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_shipments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_shipments/vendor_shipments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.523584 python-amazon-sp-api-1.5.1/sp_api/api/vendor_transaction_status/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_transaction_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/api/vendor_transaction_status/vendor_transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.527584 python-amazon-sp-api-1.5.1/sp_api/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.527584 python-amazon-sp-api-1.5.1/sp_api/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/ApiResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/InventoryEnums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/feedTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/fulfillment_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/identifiersType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/included_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/inegibility_reasons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/processing_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/reportTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/report_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/sales_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/base/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.527584 python-amazon-sp-api-1.5.1/sp_api/util/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/util/key_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/util/load_all_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/util/load_date_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/sp_api/util/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.527584 python-amazon-sp-api-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/finances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/finances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/finances/test_finances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/notifications/test_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/orders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/orders/test_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/product_fees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/product_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/product_fees/product_fees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/reports/test_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/api/sellers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/sellers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/api/sellers/test_sellers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:36.531584 python-amazon-sp-api-1.5.1/tests/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/client/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/client/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/client/test_credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-30 10:08:26.000000 python-amazon-sp-api-1.5.1/tests/client/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/make_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/make_endpoint/make_endpoint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-12 08:10:45.000000 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-12 08:10:45.000000 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:10:45.000000 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 08:10:45.000000 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 08:10:45.000000 python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/sp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/sp_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/sp_api/api/aplus_content/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/aplus_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/aplus_content/aplus_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.791972 python-amazon-sp-api-1.5.2/sp_api/api/application_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/application_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/application_management/application_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/authorization/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/catalog/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/catalog_items/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/catalog_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/catalog_items/catalog_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/data_kiosk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/data_kiosk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/data_kiosk/data_kiosk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/fba_inbound_eligibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fba_inbound_eligibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/fba_small_and_light/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fba_small_and_light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fba_small_and_light/fba_small_and_light.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/feeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/feeds/feeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/finances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/finances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/finances/finances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_inbound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_inbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66400 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_inbound/fulfillment_inbound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_outbound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_outbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28743 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_outbound/fulfillment_outbound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.795973 python-amazon-sp-api-1.5.2/sp_api/api/inventories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/inventories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/inventories/inventories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/listings_items/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/listings_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/listings_items/listings_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/listings_restrictions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/listings_restrictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/listings_restrictions/listings_restrictions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/merchant_fulfillment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/merchant_fulfillment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/merchant_fulfillment/merchant_fulfillment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/messaging/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/notifications/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/orders/orders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/product_fees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/product_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/product_fees/product_fees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/product_type_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/product_type_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/product_type_definitions/product_type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/products/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/products/products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/products/products_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/replenishment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/replenishment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/replenishment/replenishment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.799973 python-amazon-sp-api-1.5.2/sp_api/api/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/reports/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/sales/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/sales/sales.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/sellers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/sellers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/sellers/sellers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/services/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/shipping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14506 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/shipping/shipping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/solicitations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/solicitations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/solicitations/solicitations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/supply_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/supply_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/supply_sources/supply_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/tokens/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/upload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.803973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_payments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_shipping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28770 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_invoices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_invoices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_invoices/vendor_invoices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_orders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_orders/vendor_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_shipments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_shipments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_shipments/vendor_shipments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/api/vendor_transaction_status/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_transaction_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/api/vendor_transaction_status/vendor_transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.807973 python-amazon-sp-api-1.5.2/sp_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.811973 python-amazon-sp-api-1.5.2/sp_api/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/ApiResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/InventoryEnums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/feedTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/fulfillment_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/identifiersType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/included_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/inegibility_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/reportTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/report_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/sales_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/base/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.811973 python-amazon-sp-api-1.5.2/sp_api/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/util/key_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/util/load_all_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/util/load_date_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/sp_api/util/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.811973 python-amazon-sp-api-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.811973 python-amazon-sp-api-1.5.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.811973 python-amazon-sp-api-1.5.2/tests/api/finances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/finances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/finances/test_finances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/api/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/notifications/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/orders/test_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/api/product_fees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/product_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/product_fees/product_fees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/api/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/reports/test_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/api/sellers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/sellers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/api/sellers/test_sellers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:45.815973 python-amazon-sp-api-1.5.2/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/client/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/client/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/client/test_credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-12 08:10:37.000000 python-amazon-sp-api-1.5.2/tests/client/test_helpers.py
```

### Comparing `python-amazon-sp-api-1.5.1/LICENSE` & `python-amazon-sp-api-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/PKG-INFO` & `python-amazon-sp-api-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-sp-api
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python wrapper for the Amazon Selling-Partner API
 Home-page: https://github.com/saleweaver/python-amazon-sp-api
 Author: Michael
 Author-email: info@saleweaver.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `python-amazon-sp-api-1.5.1/README.md` & `python-amazon-sp-api-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/make_endpoint/make_endpoint` & `python-amazon-sp-api-1.5.2/make_endpoint/make_endpoint`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/PKG-INFO` & `python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-sp-api
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python wrapper for the Amazon Selling-Partner API
 Home-page: https://github.com/saleweaver/python-amazon-sp-api
 Author: Michael
 Author-email: info@saleweaver.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `python-amazon-sp-api-1.5.1/python_amazon_sp_api.egg-info/SOURCES.txt` & `python-amazon-sp-api-1.5.2/python_amazon_sp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/setup.py` & `python-amazon-sp-api-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/__init__.py` & `python-amazon-sp-api-1.5.2/sp_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/aplus_content/aplus_content.py` & `python-amazon-sp-api-1.5.2/sp_api/api/aplus_content/aplus_content.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/application_management/application_management.py` & `python-amazon-sp-api-1.5.2/sp_api/api/application_management/application_management.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/authorization/authorization.py` & `python-amazon-sp-api-1.5.2/sp_api/api/authorization/authorization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/catalog/catalog.py` & `python-amazon-sp-api-1.5.2/sp_api/api/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/catalog_items/catalog_items.py` & `python-amazon-sp-api-1.5.2/sp_api/api/catalog_items/catalog_items.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/data_kiosk/data_kiosk.py` & `python-amazon-sp-api-1.5.2/sp_api/api/data_kiosk/data_kiosk.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py` & `python-amazon-sp-api-1.5.2/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/fba_small_and_light/fba_small_and_light.py` & `python-amazon-sp-api-1.5.2/sp_api/api/fba_small_and_light/fba_small_and_light.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/feeds/feeds.py` & `python-amazon-sp-api-1.5.2/sp_api/api/feeds/feeds.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/finances/finances.py` & `python-amazon-sp-api-1.5.2/sp_api/api/finances/finances.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_inbound/fulfillment_inbound.py` & `python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_inbound/fulfillment_inbound.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/fulfillment_outbound/fulfillment_outbound.py` & `python-amazon-sp-api-1.5.2/sp_api/api/fulfillment_outbound/fulfillment_outbound.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/inventories/inventories.py` & `python-amazon-sp-api-1.5.2/sp_api/api/inventories/inventories.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/listings_items/listings_items.py` & `python-amazon-sp-api-1.5.2/sp_api/api/listings_items/listings_items.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/listings_restrictions/listings_restrictions.py` & `python-amazon-sp-api-1.5.2/sp_api/api/listings_restrictions/listings_restrictions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/merchant_fulfillment/merchant_fulfillment.py` & `python-amazon-sp-api-1.5.2/sp_api/api/merchant_fulfillment/merchant_fulfillment.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/messaging/messaging.py` & `python-amazon-sp-api-1.5.2/sp_api/api/messaging/messaging.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/notifications/notifications.py` & `python-amazon-sp-api-1.5.2/sp_api/api/notifications/notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/orders/orders.py` & `python-amazon-sp-api-1.5.2/sp_api/api/orders/orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/product_fees/product_fees.py` & `python-amazon-sp-api-1.5.2/sp_api/api/product_fees/product_fees.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/product_type_definitions/product_type_definitions.py` & `python-amazon-sp-api-1.5.2/sp_api/api/product_type_definitions/product_type_definitions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/products/products.py` & `python-amazon-sp-api-1.5.2/sp_api/api/products/products.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/products/products_definitions.py` & `python-amazon-sp-api-1.5.2/sp_api/api/products/products_definitions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/replenishment/replenishment.py` & `python-amazon-sp-api-1.5.2/sp_api/api/replenishment/replenishment.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/reports/reports.py` & `python-amazon-sp-api-1.5.2/sp_api/api/reports/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/sales/sales.py` & `python-amazon-sp-api-1.5.2/sp_api/api/sales/sales.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/sellers/sellers.py` & `python-amazon-sp-api-1.5.2/sp_api/api/sellers/sellers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/services/services.py` & `python-amazon-sp-api-1.5.2/sp_api/api/services/services.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/shipping/shipping.py` & `python-amazon-sp-api-1.5.2/sp_api/api/shipping/shipping.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/solicitations/solicitations.py` & `python-amazon-sp-api-1.5.2/sp_api/api/solicitations/solicitations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/supply_sources/supply_sources.py` & `python-amazon-sp-api-1.5.2/sp_api/api/supply_sources/supply_sources.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/tokens/tokens.py` & `python-amazon-sp-api-1.5.2/sp_api/api/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/upload/upload.py` & `python-amazon-sp-api-1.5.2/sp_api/api/upload/upload.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_invoices/vendor_invoices.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_invoices/vendor_invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_orders/vendor_orders.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_orders/vendor_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_shipments/vendor_shipments.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_shipments/vendor_shipments.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/api/vendor_transaction_status/vendor_transaction_status.py` & `python-amazon-sp-api-1.5.2/sp_api/api/vendor_transaction_status/vendor_transaction_status.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/auth/access_token_client.py` & `python-amazon-sp-api-1.5.2/sp_api/auth/access_token_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/ApiResponse.py` & `python-amazon-sp-api-1.5.2/sp_api/base/ApiResponse.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/__init__.py` & `python-amazon-sp-api-1.5.2/sp_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/client.py` & `python-amazon-sp-api-1.5.2/sp_api/base/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,29 @@
 from .exceptions import get_exception_for_code, MissingScopeException
 from .marketplaces import Marketplaces
 from sp_api.base.credential_provider import CredentialProvider
 
 log = logging.getLogger(__name__)
 
 
+def show_donation_message():
+    import os
+    if os.environ.get('ENV_DISABLE_DONATION_MSG'):
+        return
+    print("🌟 Thank you for using python-amazon-sp-api! 🌟")
+    print("This tool helps developers and businesses connect seamlessly with Amazon's vast marketplace,")
+    print("enabling powerful automations and data management.")
+    print("If you appreciate this project and find it useful, please consider supporting its continued development:")
+    print(" - 🙌 GitHub Sponsors: https://github.com/sponsors/saleweaver")
+    print(" - 🌐 BTC Address: bc1q6uqgczasmnvnc5upumarugw2mksnwneg0f65ws")
+    print(" - 🌐 ETH Address: 0xf59534F7a7F5410DBCD0c779Ac3bB6503bd32Ae5")
+    print("\nYour support helps keep the project alive and evolving, and is greatly appreciated!")
+    print("\nTo disable this donation message, set the ENV_DISABLE_DONATION_MSG=1 environment variable.")
+
+
 class Client(BaseClient):
     grantless_scope: str = ''
     keep_restricted_data_token: bool = False
     version = None
 
     def __init__(
             self,
@@ -121,14 +136,15 @@
                 js = js[0]
 
         error = js.get('errors', None)
 
         if error:
             exception = get_exception_for_code(res.status_code)
             raise exception(error, headers=res.headers)
+        show_donation_message()
         return ApiResponse(**js, headers=res.headers)
 
     def _add_marketplaces(self, data):
         POST = ['marketplaceIds', 'MarketplaceIds']
         GET = ['MarketplaceId', 'MarketplaceIds', 'marketplace_ids', 'marketplaceIds']
 
         if self.method == 'POST':
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/credential_provider.py` & `python-amazon-sp-api-1.5.2/sp_api/base/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/exceptions.py` & `python-amazon-sp-api-1.5.2/sp_api/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/feedTypes.py` & `python-amazon-sp-api-1.5.2/sp_api/base/feedTypes.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/helpers.py` & `python-amazon-sp-api-1.5.2/sp_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/identifiersType.py` & `python-amazon-sp-api-1.5.2/sp_api/base/identifiersType.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/included_data.py` & `python-amazon-sp-api-1.5.2/sp_api/base/included_data.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/inegibility_reasons.py` & `python-amazon-sp-api-1.5.2/sp_api/base/inegibility_reasons.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/marketplaces.py` & `python-amazon-sp-api-1.5.2/sp_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/notifications.py` & `python-amazon-sp-api-1.5.2/sp_api/base/notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/base/reportTypes.py` & `python-amazon-sp-api-1.5.2/sp_api/base/reportTypes.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/util/key_maker.py` & `python-amazon-sp-api-1.5.2/sp_api/util/key_maker.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/util/load_all_pages.py` & `python-amazon-sp-api-1.5.2/sp_api/util/load_all_pages.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/util/load_date_bound.py` & `python-amazon-sp-api-1.5.2/sp_api/util/load_date_bound.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/sp_api/util/retry.py` & `python-amazon-sp-api-1.5.2/sp_api/util/retry.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/api/finances/test_finances.py` & `python-amazon-sp-api-1.5.2/tests/api/finances/test_finances.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/api/notifications/test_notifications.py` & `python-amazon-sp-api-1.5.2/tests/api/notifications/test_notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/api/orders/test_orders.py` & `python-amazon-sp-api-1.5.2/tests/api/orders/test_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/api/product_fees/product_fees.py` & `python-amazon-sp-api-1.5.2/tests/api/product_fees/product_fees.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/api/reports/test_reports.py` & `python-amazon-sp-api-1.5.2/tests/api/reports/test_reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/client/test_auth.py` & `python-amazon-sp-api-1.5.2/tests/client/test_auth.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/client/test_base.py` & `python-amazon-sp-api-1.5.2/tests/client/test_base.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/client/test_credential_provider.py` & `python-amazon-sp-api-1.5.2/tests/client/test_credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-1.5.1/tests/client/test_helpers.py` & `python-amazon-sp-api-1.5.2/tests/client/test_helpers.py`

 * *Files identical despite different names*

