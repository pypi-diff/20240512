# Comparing `tmp/ecuapassdocs-0.75.tar.gz` & `tmp/ecuapassdocs-0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.75.tar", last modified: Fri May 10 13:10:20 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.76.tar", last modified: Sun May 12 12:33:18 2024, max compression
```

## Comparing `ecuapassdocs-0.75.tar` & `ecuapassdocs-0.76.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.75/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.475325 ecuapassdocs-0.75/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.479325 ecuapassdocs-0.75/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3202 2024-04-25 03:25:15.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18145 2024-05-06 01:21:28.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9947 2024-05-08 05:43:09.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    20527 2024-05-08 05:40:58.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    25562 2024-04-12 15:14:37.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1850 2024-04-12 15:43:23.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1709 2024-04-12 15:43:35.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9777 2024-05-10 05:33:15.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/info/old-utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.479325 ecuapassdocs-0.75/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.487325 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.487325 ecuapassdocs-0.75/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.491325 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.499325 ecuapassdocs-0.75/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-08 13:54:13.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/join.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18782 2024-05-08 13:57:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.475325 ecuapassdocs-0.75/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1424 2024-05-10 13:10:17.000000 ecuapassdocs-0.75/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.476425 ecuapassdocs-0.76/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-12 12:33:18.476425 ecuapassdocs-0.76/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.76/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.448424 ecuapassdocs-0.76/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.452424 ecuapassdocs-0.76/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3415 2024-05-10 22:36:24.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18145 2024-05-06 01:21:28.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     8258 2024-05-12 11:58:35.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    20528 2024-05-12 11:51:17.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    25576 2024-05-10 22:34:00.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2187 2024-05-10 22:50:32.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2065 2024-05-10 22:37:13.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    11223 2024-05-12 11:42:43.000000 ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/info/old-utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.76/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.452424 ecuapassdocs-0.76/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.460425 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.460425 ecuapassdocs-0.76/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.464425 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.472425 ecuapassdocs-0.76/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15815 2024-05-11 02:21:09.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/join.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18780 2024-05-12 00:44:17.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.76/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.476425 ecuapassdocs-0.76/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.76/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-12 12:33:18.448424 ecuapassdocs-0.76/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-12 12:33:18.000000 ecuapassdocs-0.76/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-05-12 12:33:18.000000 ecuapassdocs-0.76/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-12 12:33:18.000000 ecuapassdocs-0.76/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-12 12:33:18.000000 ecuapassdocs-0.76/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-12 12:33:18.000000 ecuapassdocs-0.76/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-12 12:33:18.476425 ecuapassdocs-0.76/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1473 2024-05-12 12:33:16.000000 ecuapassdocs-0.76/setup.py
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,37 +5,40 @@
 #-- Class containing data for filling Ecuapass document
 #-----------------------------------------------------------
 class EcuData:
 	temporalDir = None
 
 	empresas = { 
 		"BYZA": {
-			'id'     : "BYZA",
-			"nombre" : "Grupo BYZA S.A.S.",
+			'id'       : "BYZA",
+			"nombre"   : "Grupo BYZA S.A.S.",
 			"direccion": "Av. Coral y los Alamos",
-			"idTipo" : "RUC", 
+			"idTipo"   : "RUC", 
 			"idNumero" : "0400201414001",
 			"modelCartaportes": "Model_02_Cartaportes_NTA_BYZA",
 			"modelManifiestos": "Manifiestos_NTA_BYZA_Template",
 			#"modelManifiestos": "Model_Manifiestos_NTA_BYZA_4",
 			"modelDeclaraciones": None,
 			"MRN": None,
-			"MSN": None
+			"MSN": None,
+			"permisos" : {"originario":"PO-CO-0033-22", "servicios1": "PO-CO-0033-22"}
 		},
 		"BOTERO": {
 			'id'     : "BOTERO",
 			"nombre" : "EDUARDO BOTERO SOTO S.A.",
 			"direccion": "Carrera 42 No 75-63 Aut. Sur, Itagui (Antioquia)",
 			"idTipo" : "NIT", 
 			"idNumero" : "890.901.321-5",
 			"modelCartaportes": "Model_Cartaportes_Botero",
 			"modelManifiestos": "Model_Manifiestos_Botero",
 			"modelDeclaraciones": None,
 			"MRN": None,
-			"MSN": None
+			"MSN": None,
+			"permisos" : {"originario":"C.I.-E.C.-0060-04",
+				          "servicios1":"P.P.S.CO015905", "servicios2":"P.P.S.PE000210"}
 		},
 		"NTA" : { 
 			'id'     : "NTA",
 			"nombre" : "NUEVO TRANSPORTE DE AMERICA COMPAÑIA LIMITADA", 
 			"direccion": "ARGENTINA Y JUAN LEON MERA - TULCAN",
 			"idTipo" : "RUC", 
 			"idNumero" : "1791834461001",
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,51 +18,17 @@
 		self.runningDir     = runningDir
 
 		self.empresa        = self.getEmpresaInfo ()   # Overwritten per 'empresa'
 		self.nombreEmpresa  = self.empresa ["id"]
 
 		self.resourcesPath        = os.path.join (runningDir, "resources", "data_cartaportes") 
 		self.fields               = json.load (open (fieldsJsonFile))
-		self.fields ["jsonFile"]  = fieldsJsonFile
+		#self.fields ["jsonFile"]  = fieldsJsonFile
 		self.ecudoc               = {}
 
-#	#----------------------------------------------------------------
-#	# Obsolete: moved to utils
-#	# Return field ({...,02_Remitente:"XXXX"...} 
-#	# from params values (ej. txt00 :{....}) 
-#	# Info is embedded according to Azure format
-#	#----------------------------------------------------------------
-#	def getFieldValuesFromInputs (self, inputValues):
-#		fieldsJsonDic = {}
-#		# Load parameters from package
-#		inputParameters = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
-#		for key, params in inputParameters.items():
-#			fieldName	 = params ["field"]
-#			if fieldName:
-#				value		 = inputValues [key]
-#				fieldsJsonDic [fieldName] = {"value": value, "content": value}
-#
-#		return fieldsJsonDic
-
-#	#----------------------------------------------------------------
-#	#-- Return input parameters file
-#	#----------------------------------------------------------------
-#	def getInputParametersFile (self):
-#		if self.docType == "CARTAPORTE":
-#			self.inputsParametersFile = "cartaporte_input_parameters.json"
-#		elif self.docType == "MANIFIESTO":
-#			self.inputsParametersFile = "manifiesto_input_parameters.json"
-#		elif self.docType == "DECLARACION":
-#			self.inputsParametersFile = "declaracion_input_parameters.json"
-#		else:
-#			message= f"ERROR: Tipo de documento desconocido:", docType
-#			raise Exception (message)
-#		return self.inputsParametersFile
-
-
 	#-- For all types of documents (fixed fro NTA and BYZA, check the others)
 	def getNumeroDocumento (self):
 		text   = Utils.getValue (self.fields, "00b_Numero")
 		numero = Extractor.getNumeroDocumento (text)
 
 		codigo = self.getCodigoPais (numero)
 		self.fields ["00_Pais"] = {"value":codigo, "content":codigo}
@@ -198,20 +164,20 @@
 	#-- Create CODEBIN fields from document fields using input parameters
 	#----------------------------------------------------------------
 	def getCodebinFields (self):
 		try:
 			inputsParams = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
 			codebinFields = {}
 			for key in inputsParams:
-				docField   = inputsParams [key]["ecudocsField"]
-				cbinField  = inputsParams [key]["codebinField"]
-				#print ("-- key:", key, " dfield:", docField, "cfield: ", cbinField)
-				if cbinField:
-					value = self.getDocumentFieldValue (docField, "CODEBIN")
-					codebinFields [cbinField] = value
+				ecudocsField   = inputsParams [key]["ecudocsField"]
+				codebinField  = inputsParams [key]["codebinField"]
+				#print ("-- key:", key, " dfield:", ecudocsField, "cfield: ", codebinField)
+				if codebinField:
+					value = self.getDocumentFieldValue (ecudocsField, "CODEBIN")
+					codebinFields [codebinField] = value
 
 			return codebinFields
 		except Exception as e:
 			Utils.printException ("Creando campos de CODEBIN")
 			return None
 
 	#----------------------------------------------------------------
@@ -229,38 +195,32 @@
 					value = self.getDocumentFieldValue (docField)
 					docFieldsAll [key] = value
 
 			return docFieldsAll
 		except Exception as e:
 			Utils.printException ("Creando campos de ECUAPASSDOCS")
 			return None
+
 	#-----------------------------------------------------------
 	# Implemented for each class: get the document field value
 	#-----------------------------------------------------------
 	def getDocumentFieldValue (self, docField, appName=None):
 		value = None
+		# For ecudocs is "CO" for codebin is "colombia"
 		if "00_Pais" in docField:
 			paises     = {"CO":"CO", "EC":"EC"}
 			if appName == "CODEBIN":
 				paises     = {"CO":"colombia", "EC":"ecuador"}
 
 			codigoPais = self.fields [docField]["value"]
 			value      =  paises [codigoPais]
 
-		#elif "Gastos" in docField and self.docType == "CARTAPORTE" :
-			#value = self.fields [docField]["content"]
-			#value = value if value == "" else None
-			#fieldName	= docField.split (":")[0]
-			#rowName		= docField.split (":")[1].split (",")[0]
-			#colName		= docField.split (":")[1].split (",")[1]
-			#tablaGastos = self.fields [fieldName]["value"]
-			#value		= self.getValueTablaGastos (tablaGastos, rowName, colName)
-
+		# In PDF docs, it is a check box marker with "X"
 		elif "Carga_Tipo" in docField and not "Descripcion" in docField and self.docType == "MANIFIESTO":
 			fieldValue = self.fields [docField]["value"]
-			value = 1 if "x" in fieldValue or "X" in fieldValue else 0
+			value = "X" if "X" in fieldValue.upper() else ""
 
 		else:
 			value = self.fields [docField]["content"]
 
 		return value
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 			#--------------------------------------------------------------
 			# print ("\n>>>>>> Datos Generales de la CPIC: Sujetos <<<<<<<<")
 			#--------------------------------------------------------------
 			#-- Remitente 
 			remitente                             = Utils.checkLow (self.getSubjectInfo ("02_Remitente"))
 			self.ecudoc ["10_PaisRemitente"]      = remitente ["pais"]
 			self.ecudoc ["11_TipoIdRemitente"]    = remitente ["tipoId"]
-			self.ecudoc ["12_NroIdRemitente"]	  = remitente ["numeroId"]
+			self.ecudoc ["12_NroIdRemitente"]	    = remitente ["numeroId"]
 			self.ecudoc ["13_NroCertSanitario"]	  = None
 			self.ecudoc ["14_NombreRemitente"]    = remitente ["nombre"]
 			self.ecudoc ["15_DireccionRemitente"] = remitente ["direccion"]
 
 			#-- Destinatario 
 			destinatario                             = Utils.checkLow (self.getSubjectInfo ("03_Destinatario"))
 			self.ecudoc ["16_PaisDestinatario"]	     = destinatario ["pais"] 
@@ -287,16 +287,16 @@
 		return location
 	#-----------------------------------------------------------
 	# Get "transporte" and "pago" conditions
 	#-----------------------------------------------------------
 	def getCondiciones (self):
 		conditions = {'pago':None, 'transporte':None}
 		# Condiciones transporte
+		text = self.fields ["09_Condiciones"]["value"]
 		try:
-			text = self.fields ["09_Condiciones"]["value"]
 			if "SIN CAMBIO" in text.upper():
 				conditions ["transporte"] = "DIRECTO, SIN CAMBIO DEL CAMION"
 			elif "CON CAMBIO" in text.upper():
 				conditions ["transporte"] = "DIRECTO, CON CAMBIO DEL TRACTO-CAMION"
 			elif "TRANSBORDO" in text.upper():
 				conditions ["transporte"] = "TRANSBORDO"
 		except:
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 
 			#print ("\n>>> Identificación Permisos")
 			permisos                              = self.getPermisosInfo ()
 			self.ecudoc ["07_TipoPermiso_CI"]     = permisos ["tipoPermisoCI"]
 			self.ecudoc ["08_TipoPermiso_PEOTP"]  = permisos ["tipoPermisoPEOTP"]
 			self.ecudoc ["09_TipoPermiso_PO"]     = permisos ["tipoPermisoPO"]
 			self.ecudoc ["10_PermisoOriginario"]  = permisos ["permisoOriginario"]
-			self.ecudoc ["11_PermisoServicios1"]  = permisos ["permisoServicios"]
-			self.ecudoc ["12_PermisoServicios2"]   = None
-			self.ecudoc ["13_PermisoServicios3"]   = None
-			self.ecudoc ["14_PermisoServicios4"]   = None
+			self.ecudoc ["11_PermisoServicios1"]  = permisos ["permisoServicios1"]
+			self.ecudoc ["12_PermisoServicios2"]  = None
+			self.ecudoc ["13_PermisoServicios3"]  = None
+			self.ecudoc ["14_PermisoServicios4"]  = None
 
 			# Empresa
 			self.ecudoc ["15_NombreTransportista"] = self.getNombreEmpresa ()
 			self.ecudoc ["16_DirTransportista"]    = self.getDireccionEmpresa ()
 
 			#print ("\n>>>>>> Identificacion de la Unidad de Carga (Remolque) <<<")
 			remolque                             = self.getRemolqueInfo ()
@@ -224,15 +224,16 @@
 			Utils.printException ("Obteniendo información del transportista")
 		return (transportista)
 
 	#------------------------------------------------------------------
 	# Permisos info
 	#------------------------------------------------------------------
 	def getPermisosInfo (self):
-		permisos = Utils.createEmptyDic (["tipoPermisoCI", "tipoPermisoPEOTP", "tipoPermisoPO", "permisoOriginario", "permisoServicios"])
+		permisos = Utils.createEmptyDic (["tipoPermisoCI", "tipoPermisoPEOTP", 
+									      "tipoPermisoPO", "permisoOriginario", "permisoServicios"])
 		try:
 			permisos ["permisoOriginario"] = self.getPermiso_PerEmpresa ("ORIGINARIO")
 			permisos ["permisoServicios"]  = self.getPermiso_PerEmpresa ("SERVICIOS")
 			#permisos ["permisoOriginario"] = self.getPermiso ("02_Permiso_Originario")
 			#permisos ["permisoServicios"]  = self.getPermiso ("03_Permiso_Servicios").replace ("-","")
 
 			tipoPermiso = permisos ["permisoOriginario"].split ("-")[0]
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,13 +47,25 @@
 	def getCheckCertificadoRemolque (self, key):
 		return None
 
 	#-- None for BYZA 
 	def getCargaDescripcion (self):
 			return None
 
+	#-- Just "Originario"
+	def getPermisosInfo (self):
+		info = EcuData.getEmpresaInfo ("BYZA")
+		permisos = {"tipoPermisoCI"    : None,
+			        "tipoPermisoPEOTP" : None,
+			        "tipoPermisoPO"    : "1", 
+			        "permisoOriginario": info ["permisos"]["originario"],
+			        "permisoServicios1" : None }
+		return permisos
+	
+
+
 #--------------------------------------------------------------------
 # Call main 
 #--------------------------------------------------------------------
 if __name__ == '__main__':
 	main ()
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,13 +38,22 @@
 		elif tipo == "VEHICULO" and not remolque ["placa"]:
 			return "CAMION"
 		elif tipo == "REMOLQUE" and remolque ["placa"]:
 			return "SEMIRREMOLQUE"
 		else:
 			return None
 
+	#-- Just "Originario"
+	def getPermisosInfo (self):
+		info = EcuData.getEmpresaInfo ("NTA")
+		permisos = {"tipoPermisoCI"    : "1",
+			        "tipoPermisoPEOTP" : None,
+			        "tipoPermisoPO"    : None,
+			        "permisoOriginario": info ["permisos"]["originario"],
+			        "permisoServicios1": info ["permisos"]["servicios1"]}
+		return permisos
 #--------------------------------------------------------------------
 # Call main 
 #--------------------------------------------------------------------
 if __name__ == '__main__':
 	main ()
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.76/ecuapassdocs/info/ecuapass_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,16 +52,17 @@
 				Utils.printx (message)
 			raise Exception (message)
 		return False
 
 	def printx (*args, flush=True, end="\n"):
 		print ("SERVER:", *args, flush=flush, end=end)
 
-	def printException (message, text=None):
-		Utils.printx ("EXCEPCION: ", message) 
+	def printException (message=None, text=None):
+		if message:
+			Utils.printx ("EXCEPCION: ", message) 
 		if text:
 			Utils.printx ("TEXT:", text) 
 		Utils.printx (traceback_format_exc())
 
 	#-- Get value from dict fields [key] 
 	def getValue (fields, key):
 		try:
@@ -92,14 +93,15 @@
 
 	#-- Save fields dict in JSON 
 	def saveFields (fieldsDict, filename, suffixName):
 		prefixName	= filename.split(".")[0]
 		outFilename = f"{prefixName}-{suffixName}.json"
 		with open (outFilename, "w") as fp:
 			json.dump (fieldsDict, fp, indent=4, default=str)
+		return outFilename
 
 	def initDicToValue (dic, value):
 		keys = dic.keys ()
 		for k in keys:
 			dic [k] = value
 		return dic
 
@@ -168,45 +170,42 @@
 			newValue += nc
 				
 		#print (">>> Output value str: ", newValue)
 
 		return newValue
 
 	#----------------------------------------------------------------
-	#-- Return input parameters file
+	# Return fields ({02_Remitente:"XXXX"} from codebin values
+	# Info is embedded according to Azure format
 	#----------------------------------------------------------------
-	def getInputsParametersFile (docType):
+	def getAzureValuesFromCodebinValues (docType, codebinValues, docNumber):
+		pdfTitle = ""
 		if docType == "CARTAPORTE":
-			inputsParametersFile = "cartaporte_input_parameters.json"
+			pdfTitle      = "Carta de Porte Internacional por Carretera (CPIC)"
 		elif docType == "MANIFIESTO":
-			inputsParametersFile = "manifiesto_input_parameters.json"
-		elif docType == "DECLARACION":
-			inputsParametersFile = "declaracion_input_parameters.json"
+			pdfTitle      = "Manifiesto de Carga Internacional (MCI)"
 		else:
-			raise Exception (f"Tipo de documento desconocido:", docType)
-		return inputsParametersFile
-	#----------------------------------------------------------------
-	# Return fields ({02_Remitente:"XXXX"} from codebin values
-	# Info is embedded according to Azure format
-	#----------------------------------------------------------------
-	def getAzureValuesFromCodebinValues (docType, codebinValues, codigoPais, pdfTitle, docNumber):
+			printx (f"Tipo de documento desconocido: '{docType}'")
+
+		pais, codigoPais  = Utils.getPaisCodigoFromDocNumber (docNumber)
 		inputsParametersFile = Utils.getInputsParametersFile (docType)
 		azureValues = {}
 		# Load parameters from package
 		inputParameters = ResourceLoader.loadJson ("docs", inputsParametersFile)
 		for key, item in inputParameters.items():
 			try:
 				ecudocsField = item ["ecudocsField"]
 				if not ecudocsField:
 					continue
 				codebinField = item ["codebinField"]
 				value = codebinValues [codebinField] if codebinField else ""
 				azureValues [ecudocsField] = {"value": value, "content": value}
 			except KeyError as ex:
-				Utils.printException (f"EXCEPCION: con campo '{codebinField}'")
+				print (f"Llave '{codebinField}' no encontrada")
+				#Utils.printException (f"EXCEPCION: con campo '{codebinField}'")
 
 		# Azure fields not existing in CODEBIN fields
 		azureValues ["00_Pais"]    = {"value": codigoPais, "content": codigoPais}
 		azureValues ["00a_Tipo"]   = {"value": pdfTitle, "content": pdfTitle}
 		azureValues ["00b_Numero"] = {"value": docNumber, "content": docNumber}
 		return azureValues
 	#----------------------------------------------------------------
@@ -270,7 +269,53 @@
 		if "CPI" in filename:
 			return "CARTAPORTE"
 		elif "MCI" in filename:
 			return "MANIFIESTO"
 		else:
 			raise Exception (f"Tipo de documento desconocido para: '{filename}'")
 
+	#-------------------------------------------------------------------
+	# Get 'pais, codigo' from document number or text
+	#-------------------------------------------------------------------
+	def getPaisCodigoFromDocNumber (docNumber):
+		pais, codigo = "NONE", "NO" 
+		docNumber = docNumber.upper ()
+
+		if docNumber.startswith ("CO"):
+			pais, codigo = "colombia", "CO"
+		elif docNumber.startswith ("EC"):
+			pais, codigo = "ecuador", "EC"
+		else:
+			raise Exception (f"No se encontró país en número: '{docNumber}'")
+
+		return pais, codigo
+
+	#-------------------------------------------------------------------
+	# Get 'pais, codigo' from text
+	#-------------------------------------------------------------------
+	def getPaisCodigoFromText (self, text):
+		pais, codigo = "NONE", "NO" 
+		text = text.upper ()
+
+		if "COLOMBIA" in text:
+			pais, codigo = "colombia", "CO"
+		elif "ECUADOR" in text:
+			pais, codigo = "ecuador", "EC"
+		else:
+			raise Exception (f"No se encontró país en texto: '{text}'")
+
+		return pais, codigo
+
+	#----------------------------------------------------------------
+	#-- Return input parameters file
+	#----------------------------------------------------------------
+	def getInputsParametersFile (docType):
+		if docType == "CARTAPORTE":
+			inputsParametersFile = "cartaporte_input_parameters.json"
+		elif docType == "MANIFIESTO":
+			inputsParametersFile = "manifiesto_input_parameters.json"
+		elif docType == "DECLARACION":
+			inputsParametersFile = "declaracion_input_parameters.json"
+		else:
+			raise Exception (f"Tipo de documento desconocido:", docType)
+		return inputsParametersFile
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/old-utils.py` & `ecuapassdocs-0.76/ecuapassdocs/info/old-utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.76/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990842490842491%*

 * *Differences: {"'txt09'": "{'codebinField': 'notificar'}", "'txt18'": "{'codebinField': 'docmentosr'}"}*

```diff
@@ -179,15 +179,15 @@
         "width": 501,
         "x": 555,
         "y": 405
     },
     "txt09": {
         "align": "left",
         "class": "input_condiciones",
-        "codebinField": "condiciones",
+        "codebinField": "notificar",
         "ecudocsField": "09_Condiciones",
         "font": "normal",
         "fontSize": "14px",
         "height": 70,
         "maxChars": 50,
         "maxLines": 4,
         "value": "",
@@ -573,15 +573,15 @@
         "width": 94,
         "x": 447,
         "y": 1061
     },
     "txt18": {
         "align": "left",
         "class": "input_documento",
-        "codebinField": "documentosr",
+        "codebinField": "docmentosr",
         "ecudocsField": "18_Documentos",
         "font": "normal",
         "fontSize": "14px",
         "height": 36,
         "maxChars": 50,
         "maxLines": 2,
         "value": "",
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion_input_parameters.json` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/declaracion_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/join.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/join.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992997198879552%*

 * *Differences: {"'txt00'": "{'codebinField': 'no'}", "'txt0a'": "{'codebinField': ''}"}*

```diff
@@ -38,15 +38,15 @@
         "width": 233,
         "x": 200,
         "y": 88
     },
     "txt00": {
         "align": "left",
         "class": "input_numero",
-        "codebinField": "",
+        "codebinField": "no",
         "ecudocsField": "00b_Numero",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 12,
         "maxLines": 1,
         "restrictions": [
@@ -194,15 +194,15 @@
         "width": 251,
         "x": 52,
         "y": 464
     },
     "txt0a": {
         "align": "left",
         "class": "input_numero",
-        "codebinField": "pais",
+        "codebinField": "",
         "ecudocsField": "00_Pais",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 2,
         "maxLines": 1,
         "restrictions": [
```

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.76/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.76/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.76/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.75/setup.py` & `ecuapassdocs-0.76/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.75',  # Package version
+    version='0.76',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,14 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
+		"0.76"   : "Improved Utils, getCodebinValues",
 		"0.75"   : "Simplified info classes (e.g. removed Gastos table)",
 		"0.74"   : "Changed tipoProc (Byza === NTA)",
 		"0.73"   : "Improved Byza's clean watermarks",
 		"0.72"   : "Improved infos: embalaje",
 		"0.71"   : "Improved assignation of vehicle type in Manifiestos",
 		"0.70"   : "Added creation of ECUAPASSDOCS fields. Added numero to parameters",
 		"0.63"   : "Added creation of CODEBIN fields",
```

