# Comparing `tmp/telemetrix_uno_r4-1.1.0.tar.gz` & `tmp/telemetrix_uno_r4-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetrix_uno_r4-1.1.0.tar", last modified: Tue Mar 12 19:52:46 2024, max compression
+gzip compressed data, was "telemetrix_uno_r4-1.1.1.tar", last modified: Sat May 11 22:23:40 2024, max compression
```

## Comparing `telemetrix_uno_r4-1.1.0.tar` & `telemetrix_uno_r4-1.1.1.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.272080 telemetrix_uno_r4-1.1.0/
--rw-r--r--   0 afy       (1000) afy       (1000)     2394 2024-03-12 19:52:46.272080 telemetrix_uno_r4-1.1.0/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)     1724 2023-09-16 23:18:19.000000 telemetrix_uno_r4-1.1.0/README.md
--rw-rw-r--   0 afy       (1000) afy       (1000)      894 2024-03-12 19:46:10.000000 telemetrix_uno_r4-1.1.0/pyproject.toml
--rw-rw-r--   0 afy       (1000) afy       (1000)       38 2024-03-12 19:52:46.272080 telemetrix_uno_r4-1.1.0/setup.cfg
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/__init__.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/__init__.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     4156 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    91324 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/telemetrix_uno_r4_minima.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     4152 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_aio_serial.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    91499 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_uno_r4_minima_aio.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2985 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1931 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3194 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3334 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2680 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2091 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2583 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3112 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2278 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1850 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2665 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3478 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_spi_adxl345_accelerometer.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.264079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2505 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1739 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3052 2024-01-11 21:20:00.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2891 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2679 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1734 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2349 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2805 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1904 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1451 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2470 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3158 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_spi_adxl345_accelerometer.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.264079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2945 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2068 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3392 2024-01-11 21:27:03.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3079 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2810 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2419 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2695 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3222 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2370 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1614 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_scroll_message.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2814 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3619 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_spi_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1962 2023-09-16 23:06:16.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wwb_servo.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.264079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2963 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1998 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3255 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3257 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2703 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2269 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2606 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3150 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2341 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1614 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_scroll_message.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1873 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2688 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3473 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_spi_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2465 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_using_class.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2991 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1967 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3244 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3055 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2686 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2216 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2589 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3118 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2348 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1503 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_scroll_message.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1856 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2671 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3484 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_spi_adxl345_accelerometer.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2528 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1722 2024-03-02 19:05:19.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3073 2024-03-12 19:00:04.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2914 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2702 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1757 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2372 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2828 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1929 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1329 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_scroll_message.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1475 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2493 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3181 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_spi_adxl345_accelerometer.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2511 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_analog_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1703 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_blink.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3058 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_dht.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2613 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2685 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input_pullup.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1740 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_fade.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2355 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_hc-sr04_distance_sensor.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2811 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_i2c_adxl345_accelerometer.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1938 2024-02-16 16:15:08.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_loop_back.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1295 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_scroll_message.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     1457 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_servo.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2476 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_sonar_disable.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3164 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_spi_adxl345_accelerometer.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     4309 2024-03-12 19:46:10.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    94594 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/telemetrix_uno_r4_wifi.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     4305 2024-03-12 19:46:10.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2665 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_ble.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_serial.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2559 2024-03-12 19:16:01.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_socket.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    96889 2024-03-12 19:42:03.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_uno_r4_wifi_aio.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/
--rw-r--r--   0 afy       (1000) afy       (1000)     2394 2024-03-12 19:52:46.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)     7773 2024-03-12 19:52:46.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/SOURCES.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)        1 2024-03-12 19:52:46.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/dependency_links.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)       15 2024-03-12 19:52:46.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/requires.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)       44 2024-03-12 19:52:46.000000 telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/top_level.txt
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.260079 telemetrix_uno_r4-1.1.0/venv/
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-03-12 19:52:46.268080 telemetrix_uno_r4-1.1.0/venv/bin/
--rw-rw-r--   0 afy       (1000) afy       (1000)     1176 2023-08-01 17:08:20.000000 telemetrix_uno_r4-1.1.0/venv/bin/activate_this.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/
+-rw-r--r--   0 afy       (1000) afy       (1000)     2394 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1724 2023-09-16 23:18:19.000000 telemetrix_uno_r4-1.1.1/README.md
+-rw-rw-r--   0 afy       (1000) afy       (1000)      894 2024-05-11 21:28:49.000000 telemetrix_uno_r4-1.1.1/pyproject.toml
+-rw-rw-r--   0 afy       (1000) afy       (1000)       38 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/setup.cfg
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/__init__.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/__init__.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4157 2024-05-11 21:28:49.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    91373 2024-05-11 21:54:24.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/telemetrix_uno_r4_minima.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.004566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4152 2024-05-11 21:28:49.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_aio_serial.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    91548 2024-05-11 21:54:24.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_uno_r4_minima_aio.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.004566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2985 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1931 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3194 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3334 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2680 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2091 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2583 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3112 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2278 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1850 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2665 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3478 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_spi_adxl345_accelerometer.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.004566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2505 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1739 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3052 2024-01-11 21:20:00.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2891 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2679 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1734 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2349 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2805 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1904 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1451 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2470 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3158 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_spi_adxl345_accelerometer.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.008566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2945 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2068 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3392 2024-01-11 21:27:03.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3079 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2810 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2419 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2695 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3222 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2370 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1614 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_scroll_message.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2814 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3619 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_spi_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1962 2023-09-16 23:06:16.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wwb_servo.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.008566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2963 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1998 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3255 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3257 2024-03-19 22:21:25.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2703 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2269 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2606 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3150 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2341 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1614 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_scroll_message.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1873 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2688 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3473 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_spi_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2465 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_using_class.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.008566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2991 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1967 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3244 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3055 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2686 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2216 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2589 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3118 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2348 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1503 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_scroll_message.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1856 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2671 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3484 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_spi_adxl345_accelerometer.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.008566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2528 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1722 2024-03-02 19:05:19.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3073 2024-03-12 19:00:04.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2914 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2702 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1757 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2372 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2828 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1929 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1329 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_scroll_message.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1475 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2493 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3181 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_spi_adxl345_accelerometer.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2511 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_analog_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1703 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_blink.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3058 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_dht.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2613 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2685 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input_pullup.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1740 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_fade.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2355 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_hc-sr04_distance_sensor.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2811 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_i2c_adxl345_accelerometer.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1938 2024-02-16 16:15:08.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_loop_back.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1295 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_scroll_message.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1457 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_servo.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2476 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_sonar_disable.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3164 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_spi_adxl345_accelerometer.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4309 2024-05-11 21:28:50.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    94647 2024-05-11 21:54:24.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/telemetrix_uno_r4_wifi.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4305 2024-05-11 21:28:49.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2665 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_ble.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2023-08-10 23:36:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_serial.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2559 2024-03-12 19:16:01.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_socket.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    96934 2024-05-11 21:45:56.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_uno_r4_wifi_aio.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/
+-rw-r--r--   0 afy       (1000) afy       (1000)     2394 2024-05-11 22:23:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)     7773 2024-05-11 22:23:40.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/SOURCES.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)        1 2024-05-11 22:23:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/dependency_links.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)       15 2024-05-11 22:23:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/requires.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)       44 2024-05-11 22:23:39.000000 telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/top_level.txt
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.000565 telemetrix_uno_r4-1.1.1/venv/
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2024-05-11 22:23:40.012566 telemetrix_uno_r4-1.1.1/venv/bin/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1176 2023-08-01 17:08:20.000000 telemetrix_uno_r4-1.1.1/venv/bin/activate_this.py
```

### Comparing `telemetrix_uno_r4-1.1.0/PKG-INFO` & `telemetrix_uno_r4-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemetrix_uno_r4
-Version: 1.1.0
+Version: 1.1.1
 Summary: Telemetrix Clients Supporting The Arduino Uno R4 Minima and Wifi
 Author-email: Alan Yorinks <MisterYsLab@gmail.com>
 License: AGPL-3.0-or-later
 Keywords: telemetrix,Arduino,R4,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `telemetrix_uno_r4-1.1.0/README.md` & `telemetrix_uno_r4-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/pyproject.toml` & `telemetrix_uno_r4-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [project]
 name = "telemetrix_uno_r4"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Alan Yorinks", email="MisterYsLab@gmail.com" },
 ]
 description = "Telemetrix Clients Supporting The Arduino Uno R4 Minima and Wifi"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "AGPL-3.0-or-later"}
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/private_constants.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/private_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     STEPPER_TARGET_POSITION = 16
     STEPPER_CURRENT_POSITION = 17
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     DEBUG_PRINT = 99
 
-    TELEMETRIX_VERSION = "1.00"
+    TELEMETRIX_VERSION = "1.1.1"
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/telemetrix_uno_r4_minima.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima/telemetrix_uno_r4_minima.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- Copyright (c) 2023 Alan Yorinks All rights reserved.
+ Copyright (c) 2023, 2024 Alan Yorinks All rights reserved.
 
  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU AFFERO GENERAL PUBLIC LICENSE
  Version 3 as published by the Free Software Foundation; either
  or (at your option) any later version.
  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -245,15 +245,15 @@
         #                      'motion_complete_callback': None,
         #                      'acceleration_callback': None}
         #
         # # build a list of stepper motor info items
         # self.stepper_info_list = []
         # # a list of dictionaries to hold stepper information
         # for motor in range(self.max_number_of_steppers):
-        #     self.stepper_info_list.append(self.stepper_info)
+        #     self.stepper_info_list.append(self.stepper_info.copy())
 
         self.the_reporter_thread.start()
         self.the_data_receive_thread.start()
 
         print(f"telemetrix_uno_r4_minima:  Version"
               f" {PrivateConstants.TELEMETRIX_VERSION}\n\n"
               f"Copyright (c) 2023 Alan Yorinks All Rights Reserved.\n")
@@ -533,16 +533,16 @@
        :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
 
         self._i2c_read_request(address, register, number_of_bytes,
                                callback=callback, i2c_port=i2c_port,
                                write_register=write_register)
 
@@ -572,16 +572,16 @@
        :param write_register: If True, the register is written before read
                               Else, the write is suppressed
 
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
 
         self._i2c_read_request(address, register, number_of_bytes,
                                stop_transmission=False,
                                callback=callback, i2c_port=i2c_port,
                                write_register=write_register)
@@ -940,15 +940,15 @@
                            NOTE: You must specify the chips select pins here!
 
 
         command message: [command, [cs pins...]]
         """
 
         if self.reported_features & PrivateConstants.SPI_FEATURE:
-            if type(chip_select_list) != list:
+            if type(chip_select_list) is not list:
                 if self.shutdown_on_exception:
                     self.shutdown()
                 raise RuntimeError('chip_select_list must be in the form of a list')
             if not chip_select_list:
                 if self.shutdown_on_exception:
                     self.shutdown()
                 raise RuntimeError('Chip select pins were not specified')
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/private_constants.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/private_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     STEPPER_CURRENT_POSITION = 17
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
 
     DEBUG_PRINT = 99
 
-    TELEMETRIX_AIO_VERSION = "1.0.0"
+    TELEMETRIX_AIO_VERSION = "1.1.1"
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_aio_serial.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_aio_serial.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_uno_r4_minima_aio.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/minima/telemetrix_uno_r4_minima_aio/telemetrix_uno_r4_minima_aio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- Copyright (c) 2023 Alan Yorinks All rights reserved.
+ Copyright (c) 2023, 2024 Alan Yorinks All rights reserved.
 
  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU AFFERO GENERAL PUBLIC LICENSE
  Version 3 as published by the Free Software Foundation; either
  or (at your option) any later version.
  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -249,15 +249,15 @@
         #                      'motion_complete_callback': None,
         #                      'acceleration_callback': None}
         #
         # # build a list of stepper motor info items
         # self.stepper_info_list = []
         # # a list of dictionaries to hold stepper information
         # for motor in range(self.max_number_of_steppers):
-        #     self.stepper_info_list.append(self.stepper_info)
+        #     self.stepper_info_list.append(self.stepper_info.copy())
 
         print(f'telemetrix_uno_r4_minima_aio Version:'
               f' {PrivateConstants.TELEMETRIX_AIO_VERSION}')
         print(f'Copyright (c) 2023 Alan Yorinks All rights reserved.\n')
 
         if autostart:
             self.loop.run_until_complete(self.start_aio())
@@ -488,16 +488,16 @@
         :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
         if not callback:
             if self.shutdown_on_exception:
                 await self.shutdown()
             raise RuntimeError('i2c_read: A Callback must be specified')
 
@@ -529,16 +529,16 @@
 
         :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
         if not callback:
             if self.shutdown_on_exception:
                 await self.shutdown()
             raise RuntimeError(
                 'i2c_read_restart_transmission: A Callback must be specified')
@@ -925,15 +925,15 @@
                            NOTE: You must specify the chips select pins here!
 
 
         command message: [command, number of cs pins, [cs pins...]]
         """
         if self.reported_features & PrivateConstants.SPI_FEATURE:
 
-            if type(chip_select_list) != list:
+            if type(chip_select_list) is not list:
                 if self.shutdown_on_exception:
                     await self.shutdown()
                 raise RuntimeError('chip_select_list must be in the form of a list')
             if not chip_select_list:
                 if self.shutdown_on_exception:
                     await self.shutdown()
                 raise RuntimeError('Chip select pins were not specified')
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/asyncio/msa_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_minima_examples/threaded/mst_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_minima_examples/threaded/mst_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_scroll_message.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_scroll_message.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wba_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wwb_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/BLE/wwb_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_scroll_message.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_scroll_message.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_using_class.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/WIFI/wwa_using_class.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_scroll_message.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_scroll_message.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/asyncio/usbSerial/wsa_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_scroll_message.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_scroll_message.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/WIFI/wwt_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_analog_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_analog_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_blink.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_blink.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_dht.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_dht.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input_pullup.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_digital_input_pullup.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_fade.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_fade.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_hc-sr04_distance_sensor.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_hc-sr04_distance_sensor.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_i2c_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_i2c_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_loop_back.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_loop_back.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_scroll_message.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_scroll_message.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_servo.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_servo.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_sonar_disable.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_sonar_disable.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_spi_adxl345_accelerometer.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/r4_wifi_examples/threaded/usbSerial/wst_spi_adxl345_accelerometer.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/private_constants.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/private_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     STEPPER_TARGET_POSITION = 16
     STEPPER_CURRENT_POSITION = 17
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     DEBUG_PRINT = 99
 
-    TELEMETRIX_VERSION = "1.1.0"
+    TELEMETRIX_VERSION = "1.1.1"
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/telemetrix_uno_r4_wifi.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi/telemetrix_uno_r4_wifi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- Copyright (c) 2023 Alan Yorinks All rights reserved.
+ Copyright (c) 2023, 2024 Alan Yorinks All rights reserved.
 
  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU AFFERO GENERAL PUBLIC LICENSE
  Version 3 as published by the Free Software Foundation; either
  or (at your option) any later version.
  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -273,15 +273,15 @@
         #                      'motion_complete_callback': None,
         #                      'acceleration_callback': None}
         #
         # # build a list of stepper motor info items
         # self.stepper_info_list = []
         # # a list of dictionaries to hold stepper information
         # for motor in range(self.max_number_of_steppers):
-        #     self.stepper_info_list.append(self.stepper_info)
+        #     self.stepper_info_list.append(self.stepper_info.copy())
 
         self.the_reporter_thread.start()
         self.the_data_receive_thread.start()
 
         print(f"telemetrix_uno_r4_wifi:  Version"
               f" {PrivateConstants.TELEMETRIX_VERSION}\n\n"
               f"Copyright (c) 2023 Alan Yorinks All Rights Reserved.\n")
@@ -569,16 +569,16 @@
        :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
 
         self._i2c_read_request(address, register, number_of_bytes,
                                callback=callback, i2c_port=i2c_port,
                                write_register=write_register)
 
@@ -608,16 +608,16 @@
        :param write_register: If True, the register is written before read
                               Else, the write is suppressed
 
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
 
         self._i2c_read_request(address, register, number_of_bytes,
                                stop_transmission=False,
                                callback=callback, i2c_port=i2c_port,
                                write_register=write_register)
@@ -976,15 +976,15 @@
                            NOTE: You must specify the chips select pins here!
 
 
         command message: [command, [cs pins...]]
         """
 
         if self.reported_features & PrivateConstants.SPI_FEATURE:
-            if type(chip_select_list) != list:
+            if type(chip_select_list) is not list:
                 if self.shutdown_on_exception:
                     self.shutdown()
                 raise RuntimeError('chip_select_list must be in the form of a list')
             if not chip_select_list:
                 if self.shutdown_on_exception:
                     self.shutdown()
                 raise RuntimeError('Chip select pins were not specified')
@@ -2445,14 +2445,15 @@
     #     num_steps = int.from_bytes(steps, byteorder='big', signed=True)
     #
     #     cb_list = [PrivateConstants.STEPPER_DISTANCE_TO_GO, report[0], num_steps,
     #                time.time()]
     #
     #     cb(cb_list)
     #
+
     def _stepper_target_position_report(self, report):
         return  # for now
     #     """
     #     Report stepper target position to go.
     #
     #     :param report: data[0] = motor_id, data[1] = target position MSB,
     #                    data[2] = target position byte MSB+1
@@ -2473,14 +2474,15 @@
     #     target_position = int.from_bytes(target, byteorder='big', signed=True)
     #
     #     cb_list = [PrivateConstants.STEPPER_TARGET_POSITION, report[0], target_position,
     #                time.time()]
     #
     #     cb(cb_list)
     #
+
     def _stepper_current_position_report(self, report):
         return  # for now
     #     """
     #     Report stepper current position.
     #
     #     :param report: data[0] = motor_id, data[1] = current position MSB,
     #                    data[2] = current position byte MSB+1
@@ -2501,14 +2503,15 @@
     #     current_position = int.from_bytes(position, byteorder='big', signed=True)
     #
     #     cb_list = [PrivateConstants.STEPPER_CURRENT_POSITION, report[0], current_position,
     #                time.time()]
     #
     #     cb(cb_list)
     #
+
     def _stepper_is_running_report(self, report):
         return  # for now
     #     """
     #     Report if the motor is currently running
     #
     #     :param report: data[0] = motor_id, True if motor is running or False if it is not.
     #
@@ -2519,14 +2522,15 @@
     #     # get callback
     #     cb = self.stepper_info_list[report[0]]['is_running_callback']
     #
     #     cb_list = [PrivateConstants.STEPPER_RUNNING_REPORT, report[0], time.time()]
     #
     #     cb(cb_list)
     #
+
     def _stepper_run_complete_report(self, report):
         return  # for now
     #     """
     #     The motor completed it motion
     #
     #     :param report: data[0] = motor_id
     #
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/private_constants.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/private_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     STEPPER_TARGET_POSITION = 16
     STEPPER_CURRENT_POSITION = 17
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     DEBUG_PRINT = 99
 
-    TELEMETRIX_VERSION = "1.1.0"
+    TELEMETRIX_VERSION = "1.1.1"
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_ble.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_ble.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_serial.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_serial.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_socket.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_aio_socket.py`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_uno_r4_wifi_aio.py` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4/wifi/telemetrix_uno_r4_wifi_aio/telemetrix_uno_r4_wifi_aio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
- Copyright (c) 2023 Alan Yorinks All rights reserved.
+ Copyright (c) 2023, 2024 Alan Yorinks All rights reserved.
 
  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU AFFERO GENERAL PUBLIC LICENSE
  Version 3 as published by the Free Software Foundation; either
  or (at your option) any later version.
  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -282,15 +282,15 @@
         #                      'motion_complete_callback': None,
         #                      'acceleration_callback': None}
         #
         # # build a list of stepper motor info items
         # self.stepper_info_list = []
         # # a list of dictionaries to hold stepper information
         # for motor in range(self.max_number_of_steppers):
-        #     self.stepper_info_list.append(self.stepper_info)
+        #     self.stepper_info_list.append(self.stepper_info.copy())
 
         print(f'telemetrix_uno_r4_wifi_aio Version:'
               f' {PrivateConstants.TELEMETRIX_VERSION}')
         print(f'Copyright (c) 2023 Alan Yorinks All rights reserved.\n')
 
         if autostart:
             self.loop.run_until_complete(self.start_aio())
@@ -541,16 +541,16 @@
         :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
         if not callback:
             if self.shutdown_on_exception:
                 await self.shutdown()
             raise RuntimeError('i2c_read: A Callback must be specified')
 
@@ -582,16 +582,16 @@
 
         :param write_register: If True, the register is written
                                        before read
                               Else, the write is suppressed
 
         callback returns a data list:
 
-        [I2C_READ_REPORT, address, register, count of data bytes,
-         data bytes, time-stamp]
+        [I2C_READ_REPORT, i2c_port, number of bytes read, address, register,
+           bytes read..., time-stamp]
 
         """
         if not callback:
             if self.shutdown_on_exception:
                 await self.shutdown()
             raise RuntimeError(
                 'i2c_read_restart_transmission: A Callback must be specified')
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/PKG-INFO` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemetrix_uno_r4
-Version: 1.1.0
+Version: 1.1.1
 Summary: Telemetrix Clients Supporting The Arduino Uno R4 Minima and Wifi
 Author-email: Alan Yorinks <MisterYsLab@gmail.com>
 License: AGPL-3.0-or-later
 Keywords: telemetrix,Arduino,R4,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `telemetrix_uno_r4-1.1.0/telemetrix_uno_r4.egg-info/SOURCES.txt` & `telemetrix_uno_r4-1.1.1/telemetrix_uno_r4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telemetrix_uno_r4-1.1.0/venv/bin/activate_this.py` & `telemetrix_uno_r4-1.1.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

