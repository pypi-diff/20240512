# Comparing `tmp/voiceos-0.8.1.2.tar.gz` & `tmp/voiceos-0.8.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voiceos-0.8.1.2.tar", last modified: Mon Apr  8 03:45:04 2024, max compression
+gzip compressed data, was "voiceos-0.8.1.3.tar", last modified: Sat May 11 22:44:07 2024, max compression
```

## Comparing `voiceos-0.8.1.2.tar` & `voiceos-0.8.1.3.tar`

### file list

```diff
@@ -1,156 +1,176 @@
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.574635 voiceos-0.8.1.2/
--rw-r--r--   0 jonah      (501) staff       (20)     2268 2024-04-08 03:45:04.574717 voiceos-0.8.1.2/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)     1992 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/README.md
--rw-r--r--   0 jonah      (501) staff       (20)     1913 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/pyproject.toml
--rw-r--r--   0 jonah      (501) staff       (20)       69 2024-04-08 03:45:04.575031 voiceos-0.8.1.2/setup.cfg
--rw-r--r--   0 jonah      (501) staff       (20)      917 2024-04-08 03:44:43.000000 voiceos-0.8.1.2/setup.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.549873 voiceos-0.8.1.2/test/
--rw-r--r--   0 jonah      (501) staff       (20)     2290 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     2512 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     1413 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)      602 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_language.py
--rw-r--r--   0 jonah      (501) staff       (20)     4046 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      602 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     3048 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agent_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1142 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_agents_api.py
--rw-r--r--   0 jonah      (501) staff       (20)      609 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_azure_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)      581 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_azure_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1418 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_azure_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     1391 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_azure_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     1358 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_buy_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     3400 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_call_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1310 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_call_recording.py
--rw-r--r--   0 jonah      (501) staff       (20)     4903 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      581 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_call_status.py
--rw-r--r--   0 jonah      (501) staff       (20)      567 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_call_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     1009 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_calls_api.py
--rw-r--r--   0 jonah      (501) staff       (20)     3388 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_calls_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      560 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_chat_gpt.py
--rw-r--r--   0 jonah      (501) staff       (20)     1394 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_create_call.py
--rw-r--r--   0 jonah      (501) staff       (20)     1349 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_create_call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      566 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_currency.py
--rw-r--r--   0 jonah      (501) staff       (20)      630 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_deepgram_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)      602 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_deepgram_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1491 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_deepgram_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)      617 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_eleven_labs_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     1464 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_eleven_labs_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)      595 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_ended_reasons.py
--rw-r--r--   0 jonah      (501) staff       (20)     1142 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_event.py
--rw-r--r--   0 jonah      (501) staff       (20)      574 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_event_name.py
--rw-r--r--   0 jonah      (501) staff       (20)      631 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_event_variable_name.py
--rw-r--r--   0 jonah      (501) staff       (20)     1599 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_http_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     1629 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_language_model_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1289 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_message.py
--rw-r--r--   0 jonah      (501) staff       (20)      588 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_message_role.py
--rw-r--r--   0 jonah      (501) staff       (20)      581 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_method_enum.py
--rw-r--r--   0 jonah      (501) staff       (20)     1520 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_open_ai.py
--rw-r--r--   0 jonah      (501) staff       (20)     1990 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_open_ai_function.py
--rw-r--r--   0 jonah      (501) staff       (20)     1606 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_open_ai_function_parameter.py
--rw-r--r--   0 jonah      (501) staff       (20)      639 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_open_ai_function_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     2399 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     2779 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_phone_number_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)     2546 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_phone_number_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1451 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_phone_number_to_buy.py
--rw-r--r--   0 jonah      (501) staff       (20)     1624 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_phone_numbers_api.py
--rw-r--r--   0 jonah      (501) staff       (20)     1407 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_rime_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     1526 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_synthesizer_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1504 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_telephony_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1381 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     1393 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_transcriber1.py
--rw-r--r--   0 jonah      (501) staff       (20)     1532 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_transcriber_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     1444 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_twilio_telephony.py
--rw-r--r--   0 jonah      (501) staff       (20)     2334 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_update_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     1327 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_update_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     1512 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     1361 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_validation_error_loc_inner.py
--rw-r--r--   0 jonah      (501) staff       (20)     1429 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_voice.py
--rw-r--r--   0 jonah      (501) staff       (20)     1441 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_voice1.py
--rw-r--r--   0 jonah      (501) staff       (20)      753 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_wako_api_models_language_model_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      739 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_wako_api_models_phone_number_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      738 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_wako_api_models_synthesizer_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      738 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_wako_api_models_transcriber_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     1504 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/test/test_webhook.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.553552 voiceos-0.8.1.2/voiceos/
--rw-r--r--   0 jonah      (501) staff       (20)     4574 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/__init__.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.556461 voiceos-0.8.1.2/voiceos/api/
--rw-r--r--   0 jonah      (501) staff       (20)      194 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api/__init__.py
--rw-r--r--   0 jonah      (501) staff       (20)    53221 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api/agents_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    43022 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api/calls_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    66401 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api/phone_numbers_api.py
--rw-r--r--   0 jonah      (501) staff       (20)    25654 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api_client.py
--rw-r--r--   0 jonah      (501) staff       (20)      652 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/api_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      687 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/client.py
--rw-r--r--   0 jonah      (501) staff       (20)    15542 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     5877 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/exceptions.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.574451 voiceos-0.8.1.2/voiceos/models/
--rw-r--r--   0 jonah      (501) staff       (20)     3947 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/__init__.py
--rw-r--r--   0 jonah      (501) staff       (20)     4714 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     5042 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_configuration.py
--rw-r--r--   0 jonah      (501) staff       (20)     3014 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)      671 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_language.py
--rw-r--r--   0 jonah      (501) staff       (20)     3170 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      633 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     5709 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/agent_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     1241 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/azure_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)     1927 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/azure_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3506 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/azure_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     3099 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/azure_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     2991 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/buy_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     4971 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/call_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     2478 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/call_recording.py
--rw-r--r--   0 jonah      (501) staff       (20)     5609 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      647 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/call_status.py
--rw-r--r--   0 jonah      (501) staff       (20)      699 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/call_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     3178 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/calls_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)      735 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/chat_gpt.py
--rw-r--r--   0 jonah      (501) staff       (20)     2790 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/create_call.py
--rw-r--r--   0 jonah      (501) staff       (20)     2385 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/create_call_response.py
--rw-r--r--   0 jonah      (501) staff       (20)      621 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/currency.py
--rw-r--r--   0 jonah      (501) staff       (20)      903 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/deepgram_languages.py
--rw-r--r--   0 jonah      (501) staff       (20)     1129 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/deepgram_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3583 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/deepgram_transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)      989 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/eleven_labs_model.py
--rw-r--r--   0 jonah      (501) staff       (20)     3408 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/eleven_labs_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)      733 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/ended_reasons.py
--rw-r--r--   0 jonah      (501) staff       (20)     4772 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/event.py
--rw-r--r--   0 jonah      (501) staff       (20)      765 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/event_name.py
--rw-r--r--   0 jonah      (501) staff       (20)      701 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/event_variable_name.py
--rw-r--r--   0 jonah      (501) staff       (20)     2881 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/http_validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     3384 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/language_model_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     2586 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/message.py
--rw-r--r--   0 jonah      (501) staff       (20)      651 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/message_role.py
--rw-r--r--   0 jonah      (501) staff       (20)      643 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/method_enum.py
--rw-r--r--   0 jonah      (501) staff       (20)     3649 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/open_ai.py
--rw-r--r--   0 jonah      (501) staff       (20)     3443 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/open_ai_function.py
--rw-r--r--   0 jonah      (501) staff       (20)     3060 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/open_ai_function_parameter.py
--rw-r--r--   0 jonah      (501) staff       (20)      647 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/open_ai_function_type.py
--rw-r--r--   0 jonah      (501) staff       (20)     4066 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     3217 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/phone_number_pagination.py
--rw-r--r--   0 jonah      (501) staff       (20)     4206 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/phone_number_response.py
--rw-r--r--   0 jonah      (501) staff       (20)     3351 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/phone_number_to_buy.py
--rw-r--r--   0 jonah      (501) staff       (20)     3770 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/rime_synthesizer.py
--rw-r--r--   0 jonah      (501) staff       (20)     3169 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/synthesizer_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     3143 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/telephony_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     4912 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/transcriber.py
--rw-r--r--   0 jonah      (501) staff       (20)     4935 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/transcriber1.py
--rw-r--r--   0 jonah      (501) staff       (20)     3174 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/transcriber_cost.py
--rw-r--r--   0 jonah      (501) staff       (20)     3541 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/twilio_telephony.py
--rw-r--r--   0 jonah      (501) staff       (20)     5168 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/update_agent.py
--rw-r--r--   0 jonah      (501) staff       (20)     2613 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/update_phone_number.py
--rw-r--r--   0 jonah      (501) staff       (20)     2982 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/validation_error.py
--rw-r--r--   0 jonah      (501) staff       (20)     4806 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/validation_error_loc_inner.py
--rw-r--r--   0 jonah      (501) staff       (20)     5670 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/voice.py
--rw-r--r--   0 jonah      (501) staff       (20)     5699 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/voice1.py
--rw-r--r--   0 jonah      (501) staff       (20)      679 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/wako_api_models_language_model_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      675 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/wako_api_models_phone_number_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      721 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/wako_api_models_synthesizer_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)      699 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/wako_api_models_transcriber_provider.py
--rw-r--r--   0 jonah      (501) staff       (20)     3211 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/models/webhook.py
--rw-r--r--   0 jonah      (501) staff       (20)        0 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/py.typed
--rw-r--r--   0 jonah      (501) staff       (20)     9130 2024-04-08 03:43:23.000000 voiceos-0.8.1.2/voiceos/rest.py
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-04-08 03:45:04.554315 voiceos-0.8.1.2/voiceos.egg-info/
--rw-r--r--   0 jonah      (501) staff       (20)     2268 2024-04-08 03:45:04.000000 voiceos-0.8.1.2/voiceos.egg-info/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)     4582 2024-04-08 03:45:04.000000 voiceos-0.8.1.2/voiceos.egg-info/SOURCES.txt
--rw-r--r--   0 jonah      (501) staff       (20)        1 2024-04-08 03:45:04.000000 voiceos-0.8.1.2/voiceos.egg-info/dependency_links.txt
--rw-r--r--   0 jonah      (501) staff       (20)       76 2024-04-08 03:45:04.000000 voiceos-0.8.1.2/voiceos.egg-info/requires.txt
--rw-r--r--   0 jonah      (501) staff       (20)        8 2024-04-08 03:45:04.000000 voiceos-0.8.1.2/voiceos.egg-info/top_level.txt
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.867053 voiceos-0.8.1.3/
+-rw-r--r--   0 jonah      (501) staff       (20)     2292 2024-05-11 22:44:07.867139 voiceos-0.8.1.3/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)     2016 2024-05-11 22:42:27.000000 voiceos-0.8.1.3/README.md
+-rw-r--r--   0 jonah      (501) staff       (20)     1913 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/pyproject.toml
+-rw-r--r--   0 jonah      (501) staff       (20)       69 2024-05-11 22:44:07.867382 voiceos-0.8.1.3/setup.cfg
+-rw-r--r--   0 jonah      (501) staff       (20)      917 2024-05-11 21:34:40.000000 voiceos-0.8.1.3/setup.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.849982 voiceos-0.8.1.3/test/
+-rw-r--r--   0 jonah      (501) staff       (20)     2154 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agent_configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1392 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agent_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4156 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agent_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      602 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agent_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2690 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agent_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1142 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_agents_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)      609 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_azure_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)      581 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_azure_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1388 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_azure_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1445 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_azure_transcriber_languages_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1329 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_azure_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1323 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_buy_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)      560 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_chat_gpt.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3088 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversation_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1406 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversation_recording.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4502 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversation_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      637 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversation_status.py
+-rw-r--r--   0 jonah      (501) staff       (20)      623 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversation_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1135 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversations_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3470 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_conversations_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2297 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_create_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)      630 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_deepgram_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1487 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_deepgram_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1307 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_deepgram_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      659 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_default_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)      617 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_eleven_labs_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      624 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_eleven_labs_voices.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1544 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_elevenlabs_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      595 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_ended_reasons.py
+-rw-r--r--   0 jonah      (501) staff       (20)      574 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_event_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1599 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_http_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1178 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_language.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1563 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_language_model_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1289 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_message.py
+-rw-r--r--   0 jonah      (501) staff       (20)      588 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_message_role.py
+-rw-r--r--   0 jonah      (501) staff       (20)      581 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_method_enum.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1142 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1154 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_model1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1154 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_model2.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1154 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_model3.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1154 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_model4.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1221 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_open_ai.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2823 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)      631 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number_events.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3819 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2970 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1488 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number_to_buy.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1734 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_number_webhook.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1438 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_phone_numbers_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)      589 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_play_ht_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1420 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_playht_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      588 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_rime_speaker.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1331 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_rime_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1166 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_speaker.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1438 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_telephony_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1377 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1389 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_transcriber1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1466 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_transcriber_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1469 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_twilio_phone_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1481 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_twilio_telephony.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2070 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_update_agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1804 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_update_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1512 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1361 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_validation_error_loc_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1757 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1769 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_voice1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1388 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_voice_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1167 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_voice_id.py
+-rw-r--r--   0 jonah      (501) staff       (20)      753 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_language_model_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      739 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_phone_number_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      774 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_synthesizer_deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      738 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_synthesizer_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      774 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_transcriber_deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      738 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_wako_api_models_transcriber_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1600 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/test/test_webhook.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.851774 voiceos-0.8.1.3/voiceos/
+-rw-r--r--   0 jonah      (501) staff       (20)     5177 2024-05-11 21:36:13.000000 voiceos-0.8.1.3/voiceos/__init__.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.853439 voiceos-0.8.1.3/voiceos/api/
+-rw-r--r--   0 jonah      (501) staff       (20)      257 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api/__init__.py
+-rw-r--r--   0 jonah      (501) staff       (20)    54952 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api/agents_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    45583 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api/conversations_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)     9815 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api/default_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    68539 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api/phone_numbers_api.py
+-rw-r--r--   0 jonah      (501) staff       (20)    25654 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api_client.py
+-rw-r--r--   0 jonah      (501) staff       (20)      652 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/api_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      738 2024-05-11 21:27:08.000000 voiceos-0.8.1.3/voiceos/client.py
+-rw-r--r--   0 jonah      (501) staff       (20)    14624 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5877 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/exceptions.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.866849 voiceos-0.8.1.3/voiceos/models/
+-rw-r--r--   0 jonah      (501) staff       (20)     4534 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/__init__.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5152 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/agent_configuration.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2844 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/agent_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3170 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/agent_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)      639 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/agent_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5823 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/agent_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1241 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/azure_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1095 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/azure_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3567 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/azure_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4879 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/azure_transcriber_languages_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3621 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/azure_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2821 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/buy_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1315 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/chat_gpt.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4712 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversation_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2510 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversation_recording.py
+-rw-r--r--   0 jonah      (501) staff       (20)     6187 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversation_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)      691 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversation_status.py
+-rw-r--r--   0 jonah      (501) staff       (20)      715 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversation_type.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3242 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/conversations_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3454 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/create_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)      903 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/deepgram_languages.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3843 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/deepgram_transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3189 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/deepgram_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      765 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/eleven_labs_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      771 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/eleven_labs_voices.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4601 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/elevenlabs_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)      699 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/ended_reasons.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1195 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/event_name.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2881 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/http_validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4828 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/language.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3128 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/language_model_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2586 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/message.py
+-rw-r--r--   0 jonah      (501) staff       (20)      649 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/message_role.py
+-rw-r--r--   0 jonah      (501) staff       (20)      643 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/method_enum.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4687 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5104 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/model1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5104 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/model2.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4657 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/model3.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4709 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/model4.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3156 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/open_ai.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4527 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)      701 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number_events.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3217 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number_pagination.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4667 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number_response.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3100 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number_to_buy.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3278 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/phone_number_webhook.py
+-rw-r--r--   0 jonah      (501) staff       (20)      805 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/play_ht_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4714 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/playht_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1837 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/rime_speaker.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3938 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/rime_voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4714 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/speaker.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2955 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/telephony_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4912 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/transcriber.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4935 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/transcriber1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2918 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/transcriber_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3025 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/twilio_phone_call.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3279 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/twilio_telephony.py
+-rw-r--r--   0 jonah      (501) staff       (20)     5195 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/update_agent.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3319 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/update_phone_number.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2982 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/validation_error.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4806 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/validation_error_loc_inner.py
+-rw-r--r--   0 jonah      (501) staff       (20)     6835 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/voice.py
+-rw-r--r--   0 jonah      (501) staff       (20)     6864 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/voice1.py
+-rw-r--r--   0 jonah      (501) staff       (20)     2877 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/voice_cost.py
+-rw-r--r--   0 jonah      (501) staff       (20)     4793 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/voice_id.py
+-rw-r--r--   0 jonah      (501) staff       (20)      679 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_language_model_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)      675 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_phone_number_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1251 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_synthesizer_deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      769 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_synthesizer_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     1177 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_transcriber_deepgram_model.py
+-rw-r--r--   0 jonah      (501) staff       (20)      699 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/wako_api_models_transcriber_provider.py
+-rw-r--r--   0 jonah      (501) staff       (20)     3209 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/models/webhook.py
+-rw-r--r--   0 jonah      (501) staff       (20)        0 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/py.typed
+-rw-r--r--   0 jonah      (501) staff       (20)     9130 2024-05-11 21:32:52.000000 voiceos-0.8.1.3/voiceos/rest.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-11 22:44:07.852447 voiceos-0.8.1.3/voiceos.egg-info/
+-rw-r--r--   0 jonah      (501) staff       (20)     2292 2024-05-11 22:44:07.000000 voiceos-0.8.1.3/voiceos.egg-info/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)     5285 2024-05-11 22:44:07.000000 voiceos-0.8.1.3/voiceos.egg-info/SOURCES.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        1 2024-05-11 22:44:07.000000 voiceos-0.8.1.3/voiceos.egg-info/dependency_links.txt
+-rw-r--r--   0 jonah      (501) staff       (20)       76 2024-05-11 22:44:07.000000 voiceos-0.8.1.3/voiceos.egg-info/requires.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        8 2024-05-11 22:44:07.000000 voiceos-0.8.1.3/voiceos.egg-info/top_level.txt
```

### Comparing `voiceos-0.8.1.2/PKG-INFO` & `voiceos-0.8.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voiceos
-Version: 0.8.1.2
+Version: 0.8.1.3
 Summary: VoiceOS Python SDK
 Home-page: https://github.com/WakoAi/voiceos-python
 Author: WakoAI
 Author-email: hello@wako.ai
 Keywords: VoiceOS,VoiceOS Python ClientSDK,VoiceOS Python
 Description-Content-Type: text/markdown
 
@@ -30,23 +30,23 @@
 
 Create a new instance of the VoiceOS class by passing your API key:
 
 ```python
 voiceos = VoiceOS("your-api-key")
 ```
 
-Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/calls/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
+Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/conversations/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
 
 ```python
 # Get all agents
 agents = voiceos.agents.list_agents()
 print(agents)
 
 # Get all calls
-calls = voiceos.calls.list_calls()
+calls = voiceos.conversations.list_conversations()
 print(calls)
 
 # Get all phone numbers
 phone_numbers = voiceos.phone_numbers.list_phone_numbers()
 print(phone_numbers)
 ```
```

### Comparing `voiceos-0.8.1.2/README.md` & `voiceos-0.8.1.3/voiceos.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: voiceos
+Version: 0.8.1.3
+Summary: VoiceOS Python SDK
+Home-page: https://github.com/WakoAi/voiceos-python
+Author: WakoAI
+Author-email: hello@wako.ai
+Keywords: VoiceOS,VoiceOS Python ClientSDK,VoiceOS Python
+Description-Content-Type: text/markdown
+
 # VoiceOS Python SDK
 
 This python client lets you build with [VoiceOS](https://voiceos.io)
 
 ## Installation
 
 You can install the package via pip:
@@ -20,23 +30,23 @@
 
 Create a new instance of the VoiceOS class by passing your API key:
 
 ```python
 voiceos = VoiceOS("your-api-key")
 ```
 
-Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/calls/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
+Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/conversations/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
 
 ```python
 # Get all agents
 agents = voiceos.agents.list_agents()
 print(agents)
 
 # Get all calls
-calls = voiceos.calls.list_calls()
+calls = voiceos.conversations.list_conversations()
 print(calls)
 
 # Get all phone numbers
 phone_numbers = voiceos.phone_numbers.list_phone_numbers()
 print(phone_numbers)
 ```
 
@@ -60,8 +70,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-```
+```
```

### Comparing `voiceos-0.8.1.2/pyproject.toml` & `voiceos-0.8.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.1.2/setup.py` & `voiceos-0.8.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 NAME = "voiceos"
-VERSION = "0.8.1.2"
+VERSION = "0.8.1.3"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `voiceos-0.8.1.2/test/test_agent.py` & `voiceos-0.8.1.3/test/test_voice1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,67 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.agent import Agent
+from voiceos.models.voice1 import Voice1
 
-class TestAgent(unittest.TestCase):
-    """Agent unit test stubs"""
+class TestVoice1(unittest.TestCase):
+    """Voice1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Agent:
-        """Test Agent
+    def make_instance(self, include_optional) -> Voice1:
+        """Test Voice1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Agent`
+        # uncomment below to create an instance of `Voice1`
         """
-        model = Agent()
+        model = Voice1()
         if include_optional:
-            return Agent(
-                name = None,
-                initial_message = None,
-                prompt = None,
-                language = 'en',
-                language_model = voiceos.models.open_ai.OpenAI(
-                    provider = 'openai', 
-                    model = null, 
-                    functions = [
-                        voiceos.models.open_ai_function.OpenAIFunction(
-                            name = '', 
-                            wait = True, 
-                            description = '', 
-                            parameters = null, )
-                        ], ),
-                voice = None,
-                transcriber = None,
-                max_call_duration = None,
-                webhooks = None,
-                id = None,
-                uri = None,
-                account_id = None,
-                created_at = None,
-                updated_at = None
+            return Voice1(
+                provider = rime,
+                model = None,
+                speed = None,
+                temperature = None,
+                text_guidance = None,
+                style_guidance = None,
+                voice_id = None,
+                model_id = 'eleven_multilingual_v2',
+                optimize_latency = None,
+                use_speaker_boost = None,
+                similarity_boost = None,
+                stability = None,
+                pitch = None,
+                rate = None,
+                speaker = None,
+                speed_alpha = None,
+                reduce_latency = None
             )
         else:
-            return Agent(
-                name = None,
-                initial_message = None,
-                prompt = None,
-                id = None,
-                uri = None,
-                account_id = None,
-                created_at = None,
-                updated_at = None,
+            return Voice1(
         )
         """
 
-    def testAgent(self):
-        """Test Agent"""
+    def testVoice1(self):
+        """Test Voice1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_agent_configuration.py` & `voiceos-0.8.1.3/test/test_agent_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -31,49 +31,40 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AgentConfiguration`
         """
         model = AgentConfiguration()
         if include_optional:
             return AgentConfiguration(
-                name = '',
                 initial_message = '',
                 prompt = '',
-                language = 'en',
+                voice = None,
                 language_model = voiceos.models.open_ai.OpenAI(
                     provider = 'openai', 
-                    model = null, 
-                    functions = [
-                        voiceos.models.open_ai_function.OpenAIFunction(
-                            name = '', 
-                            wait = True, 
-                            description = '', 
-                            parameters = null, )
-                        ], ),
-                voice = None,
+                    model = null, ),
                 transcriber = None,
-                max_call_duration = 56,
+                max_duration_seconds = 56,
                 webhooks = [
                     voiceos.models.webhook.Webhook(
-                        event = null, 
+                        events = [
+                            'phone_call:connection_requested'
+                            ], 
                         url = '', 
                         method = null, 
                         headers = {
                             'key' : ''
                             }, 
-                        filter = {
-                            'key' : 56
-                            }, )
-                    ]
+                        filter = '', )
+                    ],
+                metadata = {
+                    'key' : ''
+                    }
             )
         else:
             return AgentConfiguration(
-                name = '',
-                initial_message = '',
-                prompt = '',
         )
         """
 
     def testAgentConfiguration(self):
         """Test AgentConfiguration"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_agent_cost.py` & `voiceos-0.8.1.3/test/test_model2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.agent_cost import AgentCost
+from voiceos.models.model2 import Model2
 
-class TestAgentCost(unittest.TestCase):
-    """AgentCost unit test stubs"""
+class TestModel2(unittest.TestCase):
+    """Model2 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AgentCost:
-        """Test AgentCost
+    def make_instance(self, include_optional) -> Model2:
+        """Test Model2
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AgentCost`
+        # uncomment below to create an instance of `Model2`
         """
-        model = AgentCost()
+        model = Model2()
         if include_optional:
-            return AgentCost(
-                provider = 'wako',
-                cost = 1.337,
-                seconds = 1.337,
-                discount = 56
+            return Model2(
             )
         else:
-            return AgentCost(
-                cost = 1.337,
-                seconds = 1.337,
-                discount = 56,
+            return Model2(
         )
         """
 
-    def testAgentCost(self):
-        """Test AgentCost"""
+    def testModel2(self):
+        """Test Model2"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_agent_language.py` & `voiceos-0.8.1.3/test/test_azure_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.agent_language import AgentLanguage
+from voiceos.models.azure_model import AzureModel
 
-class TestAgentLanguage(unittest.TestCase):
-    """AgentLanguage unit test stubs"""
+class TestAzureModel(unittest.TestCase):
+    """AzureModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAgentLanguage(self):
-        """Test AgentLanguage"""
-        # inst = AgentLanguage()
+    def testAzureModel(self):
+        """Test AzureModel"""
+        # inst = AzureModel()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_agent_pagination.py` & `voiceos-0.8.1.3/test/test_agent_pagination.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -33,75 +33,77 @@
         # uncomment below to create an instance of `AgentPagination`
         """
         model = AgentPagination()
         if include_optional:
             return AgentPagination(
                 items = [
                     voiceos.models.agent_response.AgentResponse(
-                        name = '', 
                         initial_message = '', 
                         prompt = '', 
-                        language = null, 
-                        language_model = null, 
                         voice = null, 
+                        language_model = null, 
                         transcriber = null, 
-                        max_call_duration = 56, 
+                        max_duration_seconds = 56, 
                         webhooks = [
                             voiceos.models.webhook.Webhook(
-                                event = null, 
+                                events = [
+                                    'phone_call:connection_requested'
+                                    ], 
                                 url = '', 
                                 method = null, 
                                 headers = {
                                     'key' : ''
                                     }, 
-                                filter = {
-                                    'key' : 56
-                                    }, )
+                                filter = '', )
                             ], 
-                        id = '', 
+                        metadata = {
+                            'key' : ''
+                            }, 
                         uri = '', 
                         account_id = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        id = '', )
                     ],
                 index = 56,
-                has_next = True
+                has_more = True
             )
         else:
             return AgentPagination(
                 items = [
                     voiceos.models.agent_response.AgentResponse(
-                        name = '', 
                         initial_message = '', 
                         prompt = '', 
-                        language = null, 
-                        language_model = null, 
                         voice = null, 
+                        language_model = null, 
                         transcriber = null, 
-                        max_call_duration = 56, 
+                        max_duration_seconds = 56, 
                         webhooks = [
                             voiceos.models.webhook.Webhook(
-                                event = null, 
+                                events = [
+                                    'phone_call:connection_requested'
+                                    ], 
                                 url = '', 
                                 method = null, 
                                 headers = {
                                     'key' : ''
                                     }, 
-                                filter = {
-                                    'key' : 56
-                                    }, )
+                                filter = '', )
                             ], 
-                        id = '', 
+                        metadata = {
+                            'key' : ''
+                            }, 
                         uri = '', 
                         account_id = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        id = '', )
                     ],
                 index = 56,
-                has_next = True,
+                has_more = True,
         )
         """
 
     def testAgentPagination(self):
         """Test AgentPagination"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_agent_provider.py` & `voiceos-0.8.1.3/test/test_agent_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_agent_response.py` & `voiceos-0.8.1.3/test/test_agent_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -31,59 +31,50 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AgentResponse`
         """
         model = AgentResponse()
         if include_optional:
             return AgentResponse(
-                name = '',
                 initial_message = '',
                 prompt = '',
-                language = 'en',
+                voice = None,
                 language_model = voiceos.models.open_ai.OpenAI(
                     provider = 'openai', 
-                    model = null, 
-                    functions = [
-                        voiceos.models.open_ai_function.OpenAIFunction(
-                            name = '', 
-                            wait = True, 
-                            description = '', 
-                            parameters = null, )
-                        ], ),
-                voice = None,
+                    model = null, ),
                 transcriber = None,
-                max_call_duration = 56,
+                max_duration_seconds = 56,
                 webhooks = [
                     voiceos.models.webhook.Webhook(
-                        event = null, 
+                        events = [
+                            'phone_call:connection_requested'
+                            ], 
                         url = '', 
                         method = null, 
                         headers = {
                             'key' : ''
                             }, 
-                        filter = {
-                            'key' : 56
-                            }, )
+                        filter = '', )
                     ],
-                id = '',
+                metadata = {
+                    'key' : ''
+                    },
                 uri = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                id = ''
             )
         else:
             return AgentResponse(
-                name = '',
-                initial_message = '',
-                prompt = '',
-                id = '',
                 uri = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                id = '',
         )
         """
 
     def testAgentResponse(self):
         """Test AgentResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_agents_api.py` & `voiceos-0.8.1.3/test/test_agents_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_azure_languages.py` & `voiceos-0.8.1.3/test/test_azure_languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_azure_model.py` & `voiceos-0.8.1.3/test/test_play_ht_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.azure_model import AzureModel
+from voiceos.models.play_ht_model import PlayHTModel
 
-class TestAzureModel(unittest.TestCase):
-    """AzureModel unit test stubs"""
+class TestPlayHTModel(unittest.TestCase):
+    """PlayHTModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAzureModel(self):
-        """Test AzureModel"""
-        # inst = AzureModel()
+    def testPlayHTModel(self):
+        """Test PlayHTModel"""
+        # inst = PlayHTModel()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_azure_synthesizer.py` & `voiceos-0.8.1.3/test/test_rime_voice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.azure_synthesizer import AzureSynthesizer
+from voiceos.models.rime_voice import RimeVoice
 
-class TestAzureSynthesizer(unittest.TestCase):
-    """AzureSynthesizer unit test stubs"""
+class TestRimeVoice(unittest.TestCase):
+    """RimeVoice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AzureSynthesizer:
-        """Test AzureSynthesizer
+    def make_instance(self, include_optional) -> RimeVoice:
+        """Test RimeVoice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AzureSynthesizer`
+        # uncomment below to create an instance of `RimeVoice`
         """
-        model = AzureSynthesizer()
+        model = RimeVoice()
         if include_optional:
-            return AzureSynthesizer(
-                provider = 'azure',
-                model = 'en-US-SteffanNeural',
-                pitch = -20.0,
-                rate = -50.0
+            return RimeVoice(
+                provider = 'rime',
+                speaker = None,
+                speed_alpha = 0.5,
+                reduce_latency = True
             )
         else:
-            return AzureSynthesizer(
+            return RimeVoice(
         )
         """
 
-    def testAzureSynthesizer(self):
-        """Test AzureSynthesizer"""
+    def testRimeVoice(self):
+        """Test RimeVoice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_azure_transcriber.py` & `voiceos-0.8.1.3/test/test_azure_transcriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -33,15 +33,15 @@
         # uncomment below to create an instance of `AzureTranscriber`
         """
         model = AzureTranscriber()
         if include_optional:
             return AzureTranscriber(
                 provider = 'azure',
                 languages = [
-                    'en-US'
+                    null
                     ]
             )
         else:
             return AzureTranscriber(
         )
         """
```

### Comparing `voiceos-0.8.1.2/test/test_buy_phone_number.py` & `voiceos-0.8.1.3/test/test_buy_phone_number.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -36,15 +36,14 @@
         if include_optional:
             return BuyPhoneNumber(
                 provider = 'twilio',
                 phone_number = ''
             )
         else:
             return BuyPhoneNumber(
-                phone_number = '',
         )
         """
 
     def testBuyPhoneNumber(self):
         """Test BuyPhoneNumber"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_call_recording.py` & `voiceos-0.8.1.3/test/test_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.call_recording import CallRecording
+from voiceos.models.model import Model
 
-class TestCallRecording(unittest.TestCase):
-    """CallRecording unit test stubs"""
+class TestModel(unittest.TestCase):
+    """Model unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CallRecording:
-        """Test CallRecording
+    def make_instance(self, include_optional) -> Model:
+        """Test Model
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CallRecording`
+        # uncomment below to create an instance of `Model`
         """
-        model = CallRecording()
+        model = Model()
         if include_optional:
-            return CallRecording(
-                recording_url = ''
+            return Model(
             )
         else:
-            return CallRecording(
-                recording_url = '',
+            return Model(
         )
         """
 
-    def testCallRecording(self):
-        """Test CallRecording"""
+    def testModel(self):
+        """Test Model"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_call_response.py` & `voiceos-0.8.1.3/test/test_conversation_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,124 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.call_response import CallResponse
+from voiceos.models.conversation_response import ConversationResponse
 
-class TestCallResponse(unittest.TestCase):
-    """CallResponse unit test stubs"""
+class TestConversationResponse(unittest.TestCase):
+    """ConversationResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CallResponse:
-        """Test CallResponse
+    def make_instance(self, include_optional) -> ConversationResponse:
+        """Test ConversationResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CallResponse`
+        # uncomment below to create an instance of `ConversationResponse`
         """
-        model = CallResponse()
+        model = ConversationResponse()
         if include_optional:
-            return CallResponse(
+            return ConversationResponse(
                 uri = '',
                 type = 'inbound_phone_call',
-                status = 'live',
-                to_number = '',
-                from_number = '',
-                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                agent = voiceos.models.agent_response.AgentResponse(
-                    name = '', 
+                account_id = '',
+                status = 'started',
+                started_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                ended_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                agent_config = voiceos.models.agent_configuration.AgentConfiguration(
                     initial_message = '', 
                     prompt = '', 
-                    language = null, 
-                    language_model = null, 
                     voice = null, 
+                    language_model = null, 
                     transcriber = null, 
-                    max_call_duration = 56, 
+                    max_duration_seconds = 56, 
                     webhooks = [
                         voiceos.models.webhook.Webhook(
-                            event = null, 
+                            events = [
+                                'phone_call:connection_requested'
+                                ], 
                             url = '', 
                             method = null, 
                             headers = {
                                 'key' : ''
                                 }, 
-                            filter = {
-                                'key' : 56
-                                }, )
+                            filter = '', )
                         ], 
-                    id = '', 
-                    uri = '', 
-                    account_id = '', 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ),
+                    metadata = {
+                        'key' : ''
+                        }, ),
                 agent_id = '',
                 messages = [
                     voiceos.models.message.Message(
                         role = null, 
                         content = '', )
                     ],
-                account_id = '',
-                ended_reason = 'human_hangup',
-                cost = voiceos.models.call_cost.CallCost(
+                phone_call = voiceos.models.twilio_phone_call.TwilioPhoneCall(
+                    provider = 'twilio', 
+                    to_number = '', 
+                    from_number = '', ),
+                ended_reason = 'agent_ended',
+                cost_breakdown = voiceos.models.conversation_cost.ConversationCost(
                     total = 1.337, 
-                    synthesizer = null, 
+                    voice = null, 
                     transcriber = null, 
                     language_model = null, 
                     telephony = null, 
-                    agent = null, 
-                    currency = null, ),
+                    agent = null, ),
                 id = ''
             )
         else:
-            return CallResponse(
+            return ConversationResponse(
                 uri = '',
                 type = 'inbound_phone_call',
-                status = 'live',
-                start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                agent = voiceos.models.agent_response.AgentResponse(
-                    name = '', 
+                account_id = '',
+                status = 'started',
+                agent_config = voiceos.models.agent_configuration.AgentConfiguration(
                     initial_message = '', 
                     prompt = '', 
-                    language = null, 
-                    language_model = null, 
                     voice = null, 
+                    language_model = null, 
                     transcriber = null, 
-                    max_call_duration = 56, 
+                    max_duration_seconds = 56, 
                     webhooks = [
                         voiceos.models.webhook.Webhook(
-                            event = null, 
+                            events = [
+                                'phone_call:connection_requested'
+                                ], 
                             url = '', 
                             method = null, 
                             headers = {
                                 'key' : ''
                                 }, 
-                            filter = {
-                                'key' : 56
-                                }, )
+                            filter = '', )
                         ], 
-                    id = '', 
-                    uri = '', 
-                    account_id = '', 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ),
-                account_id = '',
+                    metadata = {
+                        'key' : ''
+                        }, ),
                 id = '',
         )
         """
 
-    def testCallResponse(self):
-        """Test CallResponse"""
+    def testConversationResponse(self):
+        """Test ConversationResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_call_status.py` & `voiceos-0.8.1.3/test/test_event_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.call_status import CallStatus
+from voiceos.models.event_name import EventName
 
-class TestCallStatus(unittest.TestCase):
-    """CallStatus unit test stubs"""
+class TestEventName(unittest.TestCase):
+    """EventName unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCallStatus(self):
-        """Test CallStatus"""
-        # inst = CallStatus()
+    def testEventName(self):
+        """Test EventName"""
+        # inst = EventName()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_call_type.py` & `voiceos-0.8.1.3/test/test_default_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.call_type import CallType
+from voiceos.api.default_api import DefaultApi
 
-class TestCallType(unittest.TestCase):
-    """CallType unit test stubs"""
 
-    def setUp(self):
+class TestDefaultApi(unittest.TestCase):
+    """DefaultApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = DefaultApi()
+
+    def tearDown(self) -> None:
         pass
 
-    def tearDown(self):
+    def test_health_check_get(self) -> None:
+        """Test case for health_check_get
+
+        Health Check
+        """
         pass
 
-    def testCallType(self):
-        """Test CallType"""
-        # inst = CallType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_calls_api.py` & `voiceos-0.8.1.3/test/test_conversations_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.api.calls_api import CallsApi
+from voiceos.api.conversations_api import ConversationsApi
 
 
-class TestCallsApi(unittest.TestCase):
-    """CallsApi unit test stubs"""
+class TestConversationsApi(unittest.TestCase):
+    """ConversationsApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = CallsApi()
+        self.api = ConversationsApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_create_call(self) -> None:
-        """Test case for create_call
+    def test_create_phone_call(self) -> None:
+        """Test case for create_phone_call
 
-        Create Call
+        Create Phone Call
         """
         pass
 
-    def test_get_call(self) -> None:
-        """Test case for get_call
+    def test_get_audio_recording(self) -> None:
+        """Test case for get_audio_recording
 
-        Get Call
+        Get Conversation Recording
         """
         pass
 
-    def test_get_recording(self) -> None:
-        """Test case for get_recording
+    def test_get_conversation(self) -> None:
+        """Test case for get_conversation
 
-        Get Call Recording
+        Get Conversation
         """
         pass
 
-    def test_list_calls(self) -> None:
-        """Test case for list_calls
+    def test_list_conversations(self) -> None:
+        """Test case for list_conversations
 
-        List Calls
+        List Conversations
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_calls_pagination.py` & `voiceos-0.8.1.3/test/test_conversations_pagination.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,94 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.calls_pagination import CallsPagination
+from voiceos.models.conversations_pagination import ConversationsPagination
 
-class TestCallsPagination(unittest.TestCase):
-    """CallsPagination unit test stubs"""
+class TestConversationsPagination(unittest.TestCase):
+    """ConversationsPagination unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CallsPagination:
-        """Test CallsPagination
+    def make_instance(self, include_optional) -> ConversationsPagination:
+        """Test ConversationsPagination
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CallsPagination`
+        # uncomment below to create an instance of `ConversationsPagination`
         """
-        model = CallsPagination()
+        model = ConversationsPagination()
         if include_optional:
-            return CallsPagination(
+            return ConversationsPagination(
                 items = [
-                    voiceos.models.call_response.CallResponse(
+                    voiceos.models.conversation_response.ConversationResponse(
                         uri = '', 
                         type = null, 
+                        account_id = '', 
                         status = null, 
-                        to_number = '', 
-                        from_number = '', 
-                        start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        agent = null, 
+                        started_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        ended_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        agent_config = null, 
                         agent_id = '', 
                         messages = [
                             voiceos.models.message.Message(
                                 role = null, 
                                 content = '', )
                             ], 
-                        account_id = '', 
+                        phone_call = null, 
                         ended_reason = null, 
-                        cost = null, 
+                        cost_breakdown = null, 
                         id = '', )
                     ],
                 index = 56,
-                has_next = True
+                has_more = True
             )
         else:
-            return CallsPagination(
+            return ConversationsPagination(
                 items = [
-                    voiceos.models.call_response.CallResponse(
+                    voiceos.models.conversation_response.ConversationResponse(
                         uri = '', 
                         type = null, 
+                        account_id = '', 
                         status = null, 
-                        to_number = '', 
-                        from_number = '', 
-                        start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        agent = null, 
+                        started_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        ended_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        agent_config = null, 
                         agent_id = '', 
                         messages = [
                             voiceos.models.message.Message(
                                 role = null, 
                                 content = '', )
                             ], 
-                        account_id = '', 
+                        phone_call = null, 
                         ended_reason = null, 
-                        cost = null, 
+                        cost_breakdown = null, 
                         id = '', )
                     ],
                 index = 56,
-                has_next = True,
+                has_more = True,
         )
         """
 
-    def testCallsPagination(self):
-        """Test CallsPagination"""
+    def testConversationsPagination(self):
+        """Test ConversationsPagination"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_chat_gpt.py` & `voiceos-0.8.1.3/test/test_chat_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_create_call.py` & `voiceos-0.8.1.3/test/test_model1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.create_call import CreateCall
+from voiceos.models.model1 import Model1
 
-class TestCreateCall(unittest.TestCase):
-    """CreateCall unit test stubs"""
+class TestModel1(unittest.TestCase):
+    """Model1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateCall:
-        """Test CreateCall
+    def make_instance(self, include_optional) -> Model1:
+        """Test Model1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateCall`
+        # uncomment below to create an instance of `Model1`
         """
-        model = CreateCall()
+        model = Model1()
         if include_optional:
-            return CreateCall(
-                to_number = '',
-                from_number = '',
-                agent = None
+            return Model1(
             )
         else:
-            return CreateCall(
-                to_number = '',
-                from_number = '',
-                agent = None,
+            return Model1(
         )
         """
 
-    def testCreateCall(self):
-        """Test CreateCall"""
+    def testModel1(self):
+        """Test Model1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_create_call_response.py` & `voiceos-0.8.1.3/test/test_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.create_call_response import CreateCallResponse
+from voiceos.models.message import Message
 
-class TestCreateCallResponse(unittest.TestCase):
-    """CreateCallResponse unit test stubs"""
+class TestMessage(unittest.TestCase):
+    """Message unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateCallResponse:
-        """Test CreateCallResponse
+    def make_instance(self, include_optional) -> Message:
+        """Test Message
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateCallResponse`
+        # uncomment below to create an instance of `Message`
         """
-        model = CreateCallResponse()
+        model = Message()
         if include_optional:
-            return CreateCallResponse(
-                id = ''
+            return Message(
+                role = 'agent',
+                content = ''
             )
         else:
-            return CreateCallResponse(
-                id = '',
+            return Message(
+                role = 'agent',
+                content = '',
         )
         """
 
-    def testCreateCallResponse(self):
-        """Test CreateCallResponse"""
+    def testMessage(self):
+        """Test Message"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_currency.py` & `voiceos-0.8.1.3/test/test_rime_speaker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.currency import Currency
+from voiceos.models.rime_speaker import RimeSpeaker
 
-class TestCurrency(unittest.TestCase):
-    """Currency unit test stubs"""
+class TestRimeSpeaker(unittest.TestCase):
+    """RimeSpeaker unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrency(self):
-        """Test Currency"""
-        # inst = Currency()
+    def testRimeSpeaker(self):
+        """Test RimeSpeaker"""
+        # inst = RimeSpeaker()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_deepgram_languages.py` & `voiceos-0.8.1.3/test/test_deepgram_languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_deepgram_model.py` & `voiceos-0.8.1.3/test/test_method_enum.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.deepgram_model import DeepgramModel
+from voiceos.models.method_enum import MethodEnum
 
-class TestDeepgramModel(unittest.TestCase):
-    """DeepgramModel unit test stubs"""
+class TestMethodEnum(unittest.TestCase):
+    """MethodEnum unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDeepgramModel(self):
-        """Test DeepgramModel"""
-        # inst = DeepgramModel()
+    def testMethodEnum(self):
+        """Test MethodEnum"""
+        # inst = MethodEnum()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_deepgram_transcriber.py` & `voiceos-0.8.1.3/test/test_deepgram_transcriber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -32,16 +32,16 @@
             optional params are included """
         # uncomment below to create an instance of `DeepgramTranscriber`
         """
         model = DeepgramTranscriber()
         if include_optional:
             return DeepgramTranscriber(
                 provider = 'deepgram',
-                model = 'nova-2',
-                language = 'en',
+                model = None,
+                language = None,
                 keywords = [
                     ''
                     ]
             )
         else:
             return DeepgramTranscriber(
         )
```

### Comparing `voiceos-0.8.1.2/test/test_eleven_labs_model.py` & `voiceos-0.8.1.3/test/test_eleven_labs_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_eleven_labs_synthesizer.py` & `voiceos-0.8.1.3/test/test_elevenlabs_voice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.eleven_labs_synthesizer import ElevenLabsSynthesizer
+from voiceos.models.elevenlabs_voice import ElevenlabsVoice
 
-class TestElevenLabsSynthesizer(unittest.TestCase):
-    """ElevenLabsSynthesizer unit test stubs"""
+class TestElevenlabsVoice(unittest.TestCase):
+    """ElevenlabsVoice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ElevenLabsSynthesizer:
-        """Test ElevenLabsSynthesizer
+    def make_instance(self, include_optional) -> ElevenlabsVoice:
+        """Test ElevenlabsVoice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ElevenLabsSynthesizer`
+        # uncomment below to create an instance of `ElevenlabsVoice`
         """
-        model = ElevenLabsSynthesizer()
+        model = ElevenlabsVoice()
         if include_optional:
-            return ElevenLabsSynthesizer(
+            return ElevenlabsVoice(
                 provider = 'elevenlabs',
-                model = '21m00Tcm4TlvDq8ikWAM',
-                optimize_latency = 0.0
+                voice_id = None,
+                model_id = 'eleven_multilingual_v2',
+                optimize_latency = 0.0,
+                use_speaker_boost = True,
+                similarity_boost = 0.0,
+                stability = 0.0
             )
         else:
-            return ElevenLabsSynthesizer(
+            return ElevenlabsVoice(
         )
         """
 
-    def testElevenLabsSynthesizer(self):
-        """Test ElevenLabsSynthesizer"""
+    def testElevenlabsVoice(self):
+        """Test ElevenlabsVoice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_ended_reasons.py` & `voiceos-0.8.1.3/test/test_ended_reasons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_event.py` & `voiceos-0.8.1.3/test/test_model3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.event import Event
+from voiceos.models.model3 import Model3
 
-class TestEvent(unittest.TestCase):
-    """Event unit test stubs"""
+class TestModel3(unittest.TestCase):
+    """Model3 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Event:
-        """Test Event
+    def make_instance(self, include_optional) -> Model3:
+        """Test Model3
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Event`
+        # uncomment below to create an instance of `Model3`
         """
-        model = Event()
+        model = Model3()
         if include_optional:
-            return Event(
+            return Model3(
             )
         else:
-            return Event(
+            return Model3(
         )
         """
 
-    def testEvent(self):
-        """Test Event"""
+    def testModel3(self):
+        """Test Model3"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_event_name.py` & `voiceos-0.8.1.3/test/test_message_role.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.event_name import EventName
+from voiceos.models.message_role import MessageRole
 
-class TestEventName(unittest.TestCase):
-    """EventName unit test stubs"""
+class TestMessageRole(unittest.TestCase):
+    """MessageRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEventName(self):
-        """Test EventName"""
-        # inst = EventName()
+    def testMessageRole(self):
+        """Test MessageRole"""
+        # inst = MessageRole()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_http_validation_error.py` & `voiceos-0.8.1.3/test/test_http_validation_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_language_model_cost.py` & `voiceos-0.8.1.3/test/test_language_model_cost.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -34,24 +34,22 @@
         """
         model = LanguageModelCost()
         if include_optional:
             return LanguageModelCost(
                 provider = 'openai',
                 cost = 1.337,
                 input_tokens = 56,
-                output_tokens = 56,
-                external = True
+                output_tokens = 56
             )
         else:
             return LanguageModelCost(
                 provider = 'openai',
                 cost = 1.337,
                 input_tokens = 56,
                 output_tokens = 56,
-                external = True,
         )
         """
 
     def testLanguageModelCost(self):
         """Test LanguageModelCost"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_message.py` & `voiceos-0.8.1.3/test/test_speaker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.message import Message
+from voiceos.models.speaker import Speaker
 
-class TestMessage(unittest.TestCase):
-    """Message unit test stubs"""
+class TestSpeaker(unittest.TestCase):
+    """Speaker unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Message:
-        """Test Message
+    def make_instance(self, include_optional) -> Speaker:
+        """Test Speaker
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Message`
+        # uncomment below to create an instance of `Speaker`
         """
-        model = Message()
+        model = Speaker()
         if include_optional:
-            return Message(
-                role = 'agent',
-                content = ''
+            return Speaker(
             )
         else:
-            return Message(
-                role = 'agent',
-                content = '',
+            return Speaker(
         )
         """
 
-    def testMessage(self):
-        """Test Message"""
+    def testSpeaker(self):
+        """Test Speaker"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_open_ai.py` & `voiceos-0.8.1.3/test/test_open_ai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -32,22 +32,15 @@
             optional params are included """
         # uncomment below to create an instance of `OpenAI`
         """
         model = OpenAI()
         if include_optional:
             return OpenAI(
                 provider = 'openai',
-                model = 'gpt-4-1106-preview',
-                functions = [
-                    voiceos.models.open_ai_function.OpenAIFunction(
-                        name = '', 
-                        wait = True, 
-                        description = '', 
-                        parameters = null, )
-                    ]
+                model = None
             )
         else:
             return OpenAI(
         )
         """
 
     def testOpenAI(self):
```

### Comparing `voiceos-0.8.1.2/test/test_open_ai_function_parameter.py` & `voiceos-0.8.1.3/test/test_phone_number_to_buy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.open_ai_function_parameter import OpenAIFunctionParameter
+from voiceos.models.phone_number_to_buy import PhoneNumberToBuy
 
-class TestOpenAIFunctionParameter(unittest.TestCase):
-    """OpenAIFunctionParameter unit test stubs"""
+class TestPhoneNumberToBuy(unittest.TestCase):
+    """PhoneNumberToBuy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> OpenAIFunctionParameter:
-        """Test OpenAIFunctionParameter
+    def make_instance(self, include_optional) -> PhoneNumberToBuy:
+        """Test PhoneNumberToBuy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `OpenAIFunctionParameter`
+        # uncomment below to create an instance of `PhoneNumberToBuy`
         """
-        model = OpenAIFunctionParameter()
+        model = PhoneNumberToBuy()
         if include_optional:
-            return OpenAIFunctionParameter(
-                type = 'object',
-                properties = voiceos.models.properties.Properties(),
-                required = [
-                    ''
-                    ]
+            return PhoneNumberToBuy(
+                provider = 'twilio',
+                phone_number = '',
+                postal_code = '',
+                iso_country = ''
             )
         else:
-            return OpenAIFunctionParameter(
-                properties = voiceos.models.properties.Properties(),
+            return PhoneNumberToBuy(
+                provider = 'twilio',
+                phone_number = '',
         )
         """
 
-    def testOpenAIFunctionParameter(self):
-        """Test OpenAIFunctionParameter"""
+    def testPhoneNumberToBuy(self):
+        """Test PhoneNumberToBuy"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_open_ai_function_type.py` & `voiceos-0.8.1.3/test/test_phone_number_events.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.open_ai_function_type import OpenAIFunctionType
+from voiceos.models.phone_number_events import PhoneNumberEvents
 
-class TestOpenAIFunctionType(unittest.TestCase):
-    """OpenAIFunctionType unit test stubs"""
+class TestPhoneNumberEvents(unittest.TestCase):
+    """PhoneNumberEvents unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOpenAIFunctionType(self):
-        """Test OpenAIFunctionType"""
-        # inst = OpenAIFunctionType()
+    def testPhoneNumberEvents(self):
+        """Test PhoneNumberEvents"""
+        # inst = PhoneNumberEvents()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_phone_number.py` & `voiceos-0.8.1.3/test/test_phone_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -32,35 +32,46 @@
             optional params are included """
         # uncomment below to create an instance of `PhoneNumber`
         """
         model = PhoneNumber()
         if include_optional:
             return PhoneNumber(
                 uri = '',
-                inbound_agent_uri = '',
+                inbound_agent_id = '',
                 phone_number = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 telephony = voiceos.models.twilio_telephony.TwilioTelephony(
-                    provider = 'twilio', 
+                    provider = null, 
                     phone_number_sid = '', 
                     account_sid = '', 
                     auth_token = '', ),
-                stripe_subscription_id = ''
+                webhooks = [
+                    voiceos.models.phone_number_webhook.PhoneNumberWebhook(
+                        events = [
+                            'phone_call:connection_requested'
+                            ], 
+                        url = '', 
+                        method = null, 
+                        headers = {
+                            'key' : ''
+                            }, 
+                        filter = '', )
+                    ]
             )
         else:
             return PhoneNumber(
                 uri = '',
                 phone_number = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 telephony = voiceos.models.twilio_telephony.TwilioTelephony(
-                    provider = 'twilio', 
+                    provider = null, 
                     phone_number_sid = '', 
                     account_sid = '', 
                     auth_token = '', ),
         )
         """
 
     def testPhoneNumber(self):
```

### Comparing `voiceos-0.8.1.2/test/test_phone_number_pagination.py` & `voiceos-0.8.1.3/test/test_phone_number_pagination.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -34,42 +34,64 @@
         """
         model = PhoneNumberPagination()
         if include_optional:
             return PhoneNumberPagination(
                 items = [
                     voiceos.models.phone_number_response.PhoneNumberResponse(
                         uri = '', 
-                        inbound_agent_uri = '', 
+                        inbound_agent_id = '', 
                         phone_number = '', 
                         account_id = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         telephony = null, 
-                        stripe_subscription_id = '', 
+                        webhooks = [
+                            voiceos.models.phone_number_webhook.PhoneNumberWebhook(
+                                events = [
+                                    'phone_call:connection_requested'
+                                    ], 
+                                url = '', 
+                                method = null, 
+                                headers = {
+                                    'key' : ''
+                                    }, 
+                                filter = '', )
+                            ], 
                         id = '', )
                     ],
                 index = 56,
-                has_next = True
+                has_more = True
             )
         else:
             return PhoneNumberPagination(
                 items = [
                     voiceos.models.phone_number_response.PhoneNumberResponse(
                         uri = '', 
-                        inbound_agent_uri = '', 
+                        inbound_agent_id = '', 
                         phone_number = '', 
                         account_id = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         telephony = null, 
-                        stripe_subscription_id = '', 
+                        webhooks = [
+                            voiceos.models.phone_number_webhook.PhoneNumberWebhook(
+                                events = [
+                                    'phone_call:connection_requested'
+                                    ], 
+                                url = '', 
+                                method = null, 
+                                headers = {
+                                    'key' : ''
+                                    }, 
+                                filter = '', )
+                            ], 
                         id = '', )
                     ],
                 index = 56,
-                has_next = True,
+                has_more = True,
         )
         """
 
     def testPhoneNumberPagination(self):
         """Test PhoneNumberPagination"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_phone_number_response.py` & `voiceos-0.8.1.3/test/test_phone_number_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -32,36 +32,47 @@
             optional params are included """
         # uncomment below to create an instance of `PhoneNumberResponse`
         """
         model = PhoneNumberResponse()
         if include_optional:
             return PhoneNumberResponse(
                 uri = '',
-                inbound_agent_uri = '',
+                inbound_agent_id = '',
                 phone_number = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 telephony = voiceos.models.twilio_telephony.TwilioTelephony(
-                    provider = 'twilio', 
+                    provider = null, 
                     phone_number_sid = '', 
                     account_sid = '', 
                     auth_token = '', ),
-                stripe_subscription_id = '',
+                webhooks = [
+                    voiceos.models.phone_number_webhook.PhoneNumberWebhook(
+                        events = [
+                            'phone_call:connection_requested'
+                            ], 
+                        url = '', 
+                        method = null, 
+                        headers = {
+                            'key' : ''
+                            }, 
+                        filter = '', )
+                    ],
                 id = ''
             )
         else:
             return PhoneNumberResponse(
                 uri = '',
                 phone_number = '',
                 account_id = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 telephony = voiceos.models.twilio_telephony.TwilioTelephony(
-                    provider = 'twilio', 
+                    provider = null, 
                     phone_number_sid = '', 
                     account_sid = '', 
                     auth_token = '', ),
                 id = '',
         )
         """
```

### Comparing `voiceos-0.8.1.2/test/test_rime_synthesizer.py` & `voiceos-0.8.1.3/test/test_transcriber1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.rime_synthesizer import RimeSynthesizer
+from voiceos.models.transcriber1 import Transcriber1
 
-class TestRimeSynthesizer(unittest.TestCase):
-    """RimeSynthesizer unit test stubs"""
+class TestTranscriber1(unittest.TestCase):
+    """Transcriber1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RimeSynthesizer:
-        """Test RimeSynthesizer
+    def make_instance(self, include_optional) -> Transcriber1:
+        """Test Transcriber1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RimeSynthesizer`
+        # uncomment below to create an instance of `Transcriber1`
         """
-        model = RimeSynthesizer()
+        model = Transcriber1()
         if include_optional:
-            return RimeSynthesizer(
-                provider = 'rime',
-                speaker = 'abbie',
-                reduce_lantency = True,
-                speed_alpha = 0.5
+            return Transcriber1(
+                provider = azure,
+                model = None,
+                language = None,
+                keywords = None,
+                languages = None
             )
         else:
-            return RimeSynthesizer(
+            return Transcriber1(
         )
         """
 
-    def testRimeSynthesizer(self):
-        """Test RimeSynthesizer"""
+    def testTranscriber1(self):
+        """Test Transcriber1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_synthesizer_cost.py` & `voiceos-0.8.1.3/test/test_voice_cost.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.synthesizer_cost import SynthesizerCost
+from voiceos.models.voice_cost import VoiceCost
 
-class TestSynthesizerCost(unittest.TestCase):
-    """SynthesizerCost unit test stubs"""
+class TestVoiceCost(unittest.TestCase):
+    """VoiceCost unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SynthesizerCost:
-        """Test SynthesizerCost
+    def make_instance(self, include_optional) -> VoiceCost:
+        """Test VoiceCost
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SynthesizerCost`
+        # uncomment below to create an instance of `VoiceCost`
         """
-        model = SynthesizerCost()
+        model = VoiceCost()
         if include_optional:
-            return SynthesizerCost(
+            return VoiceCost(
                 provider = 'azure',
                 cost = 1.337,
-                characters = 56,
-                external = True
+                characters = 56
             )
         else:
-            return SynthesizerCost(
+            return VoiceCost(
                 provider = 'azure',
                 cost = 1.337,
                 characters = 56,
-                external = True,
         )
         """
 
-    def testSynthesizerCost(self):
-        """Test SynthesizerCost"""
+    def testVoiceCost(self):
+        """Test VoiceCost"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_telephony_cost.py` & `voiceos-0.8.1.3/test/test_telephony_cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -33,23 +33,21 @@
         # uncomment below to create an instance of `TelephonyCost`
         """
         model = TelephonyCost()
         if include_optional:
             return TelephonyCost(
                 provider = 'twilio',
                 cost = 1.337,
-                seconds = 1.337,
-                external = True
+                seconds = 1.337
             )
         else:
             return TelephonyCost(
                 provider = 'twilio',
                 cost = 1.337,
                 seconds = 1.337,
-                external = True,
         )
         """
 
     def testTelephonyCost(self):
         """Test TelephonyCost"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `voiceos-0.8.1.2/test/test_transcriber.py` & `voiceos-0.8.1.3/test/test_transcriber.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -32,16 +32,16 @@
             optional params are included """
         # uncomment below to create an instance of `Transcriber`
         """
         model = Transcriber()
         if include_optional:
             return Transcriber(
                 provider = azure,
-                model = 'nova-2',
-                language = 'en',
+                model = None,
+                language = None,
                 keywords = None,
                 languages = None
             )
         else:
             return Transcriber(
         )
         """
```

### Comparing `voiceos-0.8.1.2/test/test_transcriber1.py` & `voiceos-0.8.1.3/test/test_transcriber_cost.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.transcriber1 import Transcriber1
+from voiceos.models.transcriber_cost import TranscriberCost
 
-class TestTranscriber1(unittest.TestCase):
-    """Transcriber1 unit test stubs"""
+class TestTranscriberCost(unittest.TestCase):
+    """TranscriberCost unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Transcriber1:
-        """Test Transcriber1
+    def make_instance(self, include_optional) -> TranscriberCost:
+        """Test TranscriberCost
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Transcriber1`
+        # uncomment below to create an instance of `TranscriberCost`
         """
-        model = Transcriber1()
+        model = TranscriberCost()
         if include_optional:
-            return Transcriber1(
-                provider = azure,
-                model = 'nova-2',
-                language = 'en',
-                keywords = None,
-                languages = None
+            return TranscriberCost(
+                provider = 'deepgram',
+                cost = 1.337,
+                seconds = 1.337
             )
         else:
-            return Transcriber1(
+            return TranscriberCost(
+                provider = 'deepgram',
+                cost = 1.337,
+                seconds = 1.337,
         )
         """
 
-    def testTranscriber1(self):
-        """Test Transcriber1"""
+    def testTranscriberCost(self):
+        """Test TranscriberCost"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_twilio_telephony.py` & `voiceos-0.8.1.3/test/test_twilio_telephony.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -38,14 +38,15 @@
                 provider = 'twilio',
                 phone_number_sid = '',
                 account_sid = '',
                 auth_token = ''
             )
         else:
             return TwilioTelephony(
+                provider = 'twilio',
                 phone_number_sid = '',
         )
         """
 
     def testTwilioTelephony(self):
         """Test TwilioTelephony"""
         # inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `voiceos-0.8.1.2/test/test_update_agent.py` & `voiceos-0.8.1.3/test/test_update_agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -31,43 +31,37 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `UpdateAgent`
         """
         model = UpdateAgent()
         if include_optional:
             return UpdateAgent(
-                name = '',
                 initial_message = '',
                 prompt = '',
-                language = 'en',
+                voice = None,
                 language_model = voiceos.models.open_ai.OpenAI(
                     provider = 'openai', 
-                    model = null, 
-                    functions = [
-                        voiceos.models.open_ai_function.OpenAIFunction(
-                            name = '', 
-                            wait = True, 
-                            description = '', 
-                            parameters = null, )
-                        ], ),
-                voice = None,
+                    model = null, ),
                 transcriber = None,
-                max_duration_time = 56,
+                max_duration_seconds = 56,
                 webhooks = [
                     voiceos.models.webhook.Webhook(
-                        event = null, 
+                        events = [
+                            'phone_call:connection_requested'
+                            ], 
                         url = '', 
                         method = null, 
                         headers = {
                             'key' : ''
                             }, 
-                        filter = {
-                            'key' : 56
-                            }, )
-                    ]
+                        filter = '', )
+                    ],
+                metadata = {
+                    'key' : ''
+                    }
             )
         else:
             return UpdateAgent(
         )
         """
 
     def testUpdateAgent(self):
```

### Comparing `voiceos-0.8.1.2/test/test_update_phone_number.py` & `voiceos-0.8.1.3/test/test_language.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.update_phone_number import UpdatePhoneNumber
+from voiceos.models.language import Language
 
-class TestUpdatePhoneNumber(unittest.TestCase):
-    """UpdatePhoneNumber unit test stubs"""
+class TestLanguage(unittest.TestCase):
+    """Language unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> UpdatePhoneNumber:
-        """Test UpdatePhoneNumber
+    def make_instance(self, include_optional) -> Language:
+        """Test Language
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UpdatePhoneNumber`
+        # uncomment below to create an instance of `Language`
         """
-        model = UpdatePhoneNumber()
+        model = Language()
         if include_optional:
-            return UpdatePhoneNumber(
-                inbound_agent_uri = ''
+            return Language(
             )
         else:
-            return UpdatePhoneNumber(
+            return Language(
         )
         """
 
-    def testUpdatePhoneNumber(self):
-        """Test UpdatePhoneNumber"""
+    def testLanguage(self):
+        """Test Language"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_validation_error.py` & `voiceos-0.8.1.3/test/test_validation_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_validation_error_loc_inner.py` & `voiceos-0.8.1.3/test/test_validation_error_loc_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_voice.py` & `voiceos-0.8.1.3/test/test_webhook.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.voice import Voice
+from voiceos.models.webhook import Webhook
 
-class TestVoice(unittest.TestCase):
-    """Voice unit test stubs"""
+class TestWebhook(unittest.TestCase):
+    """Webhook unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Voice:
-        """Test Voice
+    def make_instance(self, include_optional) -> Webhook:
+        """Test Webhook
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Voice`
+        # uncomment below to create an instance of `Webhook`
         """
-        model = Voice()
+        model = Webhook()
         if include_optional:
-            return Voice(
-                provider = rime,
-                model = 'en-US-SteffanNeural',
-                optimize_latency = None,
-                pitch = None,
-                rate = None,
-                speaker = None,
-                reduce_lantency = None,
-                speed_alpha = None
+            return Webhook(
+                events = [
+                    'phone_call:connection_requested'
+                    ],
+                url = '',
+                method = 'GET',
+                headers = {
+                    'key' : ''
+                    },
+                filter = ''
             )
         else:
-            return Voice(
+            return Webhook(
+                events = [
+                    'phone_call:connection_requested'
+                    ],
+                url = '',
+                method = 'GET',
         )
         """
 
-    def testVoice(self):
-        """Test Voice"""
+    def testWebhook(self):
+        """Test Webhook"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_voice1.py` & `voiceos-0.8.1.3/test/test_playht_voice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.voice1 import Voice1
+from voiceos.models.playht_voice import PlayhtVoice
 
-class TestVoice1(unittest.TestCase):
-    """Voice1 unit test stubs"""
+class TestPlayhtVoice(unittest.TestCase):
+    """PlayhtVoice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Voice1:
-        """Test Voice1
+    def make_instance(self, include_optional) -> PlayhtVoice:
+        """Test PlayhtVoice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Voice1`
+        # uncomment below to create an instance of `PlayhtVoice`
         """
-        model = Voice1()
+        model = PlayhtVoice()
         if include_optional:
-            return Voice1(
-                provider = rime,
-                model = 'en-US-SteffanNeural',
-                optimize_latency = None,
-                pitch = None,
-                rate = None,
-                speaker = None,
-                reduce_lantency = None,
-                speed_alpha = None
+            return PlayhtVoice(
+                provider = 'playht',
+                model = None,
+                speed = 0.0,
+                temperature = 0.0,
+                text_guidance = 1.0,
+                style_guidance = 1.0
             )
         else:
-            return Voice1(
+            return PlayhtVoice(
         )
         """
 
-    def testVoice1(self):
-        """Test Voice1"""
+    def testPlayhtVoice(self):
+        """Test PlayhtVoice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/test/test_wako_api_models_language_model_provider.py` & `voiceos-0.8.1.3/test/test_wako_api_models_language_model_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_wako_api_models_phone_number_provider.py` & `voiceos-0.8.1.3/test/test_wako_api_models_phone_number_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_wako_api_models_synthesizer_provider.py` & `voiceos-0.8.1.3/test/test_wako_api_models_synthesizer_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_wako_api_models_transcriber_provider.py` & `voiceos-0.8.1.3/test/test_wako_api_models_transcriber_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `voiceos-0.8.1.2/test/test_webhook.py` & `voiceos-0.8.1.3/test/test_phone_number_webhook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from voiceos.models.webhook import Webhook
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
 
-class TestWebhook(unittest.TestCase):
-    """Webhook unit test stubs"""
+class TestPhoneNumberWebhook(unittest.TestCase):
+    """PhoneNumberWebhook unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Webhook:
-        """Test Webhook
+    def make_instance(self, include_optional) -> PhoneNumberWebhook:
+        """Test PhoneNumberWebhook
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Webhook`
+        # uncomment below to create an instance of `PhoneNumberWebhook`
         """
-        model = Webhook()
+        model = PhoneNumberWebhook()
         if include_optional:
-            return Webhook(
-                event = None,
+            return PhoneNumberWebhook(
+                events = [
+                    'phone_call:connection_requested'
+                    ],
                 url = '',
                 method = 'GET',
                 headers = {
                     'key' : ''
                     },
-                filter = {
-                    'key' : 56
-                    }
+                filter = ''
             )
         else:
-            return Webhook(
-                event = None,
+            return PhoneNumberWebhook(
+                events = [
+                    'phone_call:connection_requested'
+                    ],
                 url = '',
                 method = 'GET',
         )
         """
 
-    def testWebhook(self):
-        """Test Webhook"""
+    def testPhoneNumberWebhook(self):
+        """Test PhoneNumberWebhook"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `voiceos-0.8.1.2/voiceos/__init__.py` & `voiceos-0.8.1.3/voiceos/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,87 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.0"
-
-# import apis into sdk package
-from voiceos.api.agents_api import AgentsApi
-from voiceos.api.calls_api import CallsApi
-from voiceos.api.phone_numbers_api import PhoneNumbersApi
-
-# import ApiClient
-from voiceos.api_response import ApiResponse
-from voiceos.api_client import ApiClient
-from voiceos.configuration import Configuration
-from voiceos.exceptions import OpenApiException
-from voiceos.exceptions import ApiTypeError
-from voiceos.exceptions import ApiValueError
-from voiceos.exceptions import ApiKeyError
-from voiceos.exceptions import ApiAttributeError
-from voiceos.exceptions import ApiException
-
-# import models into sdk package
-from voiceos.models.agent import Agent
+# import models into model package
 from voiceos.models.agent_configuration import AgentConfiguration
 from voiceos.models.agent_cost import AgentCost
-from voiceos.models.agent_language import AgentLanguage
 from voiceos.models.agent_pagination import AgentPagination
 from voiceos.models.agent_provider import AgentProvider
 from voiceos.models.agent_response import AgentResponse
 from voiceos.models.azure_languages import AzureLanguages
 from voiceos.models.azure_model import AzureModel
-from voiceos.models.azure_synthesizer import AzureSynthesizer
 from voiceos.models.azure_transcriber import AzureTranscriber
+from voiceos.models.azure_transcriber_languages_inner import AzureTranscriberLanguagesInner
+from voiceos.models.azure_voice import AzureVoice
 from voiceos.models.buy_phone_number import BuyPhoneNumber
-from voiceos.models.call_cost import CallCost
-from voiceos.models.call_recording import CallRecording
-from voiceos.models.call_response import CallResponse
-from voiceos.models.call_status import CallStatus
-from voiceos.models.call_type import CallType
-from voiceos.models.calls_pagination import CallsPagination
 from voiceos.models.chat_gpt import ChatGPT
+from voiceos.models.conversation_cost import ConversationCost
+from voiceos.models.conversation_recording import ConversationRecording
+from voiceos.models.conversation_response import ConversationResponse
+from voiceos.models.conversation_status import ConversationStatus
+from voiceos.models.conversation_type import ConversationType
+from voiceos.models.conversations_pagination import ConversationsPagination
 from voiceos.models.create_call import CreateCall
-from voiceos.models.create_call_response import CreateCallResponse
-from voiceos.models.currency import Currency
 from voiceos.models.deepgram_languages import DeepgramLanguages
-from voiceos.models.deepgram_model import DeepgramModel
 from voiceos.models.deepgram_transcriber import DeepgramTranscriber
+from voiceos.models.deepgram_voice import DeepgramVoice
 from voiceos.models.eleven_labs_model import ElevenLabsModel
-from voiceos.models.eleven_labs_synthesizer import ElevenLabsSynthesizer
+from voiceos.models.eleven_labs_voices import ElevenLabsVoices
+from voiceos.models.elevenlabs_voice import ElevenlabsVoice
 from voiceos.models.ended_reasons import EndedReasons
-from voiceos.models.event import Event
 from voiceos.models.event_name import EventName
-from voiceos.models.event_variable_name import EventVariableName
 from voiceos.models.http_validation_error import HTTPValidationError
+from voiceos.models.language import Language
 from voiceos.models.language_model_cost import LanguageModelCost
 from voiceos.models.message import Message
 from voiceos.models.message_role import MessageRole
 from voiceos.models.method_enum import MethodEnum
+from voiceos.models.model import Model
+from voiceos.models.model1 import Model1
+from voiceos.models.model2 import Model2
+from voiceos.models.model3 import Model3
+from voiceos.models.model4 import Model4
 from voiceos.models.open_ai import OpenAI
-from voiceos.models.open_ai_function import OpenAIFunction
-from voiceos.models.open_ai_function_parameter import OpenAIFunctionParameter
-from voiceos.models.open_ai_function_type import OpenAIFunctionType
 from voiceos.models.phone_number import PhoneNumber
+from voiceos.models.phone_number_events import PhoneNumberEvents
 from voiceos.models.phone_number_pagination import PhoneNumberPagination
 from voiceos.models.phone_number_response import PhoneNumberResponse
 from voiceos.models.phone_number_to_buy import PhoneNumberToBuy
-from voiceos.models.rime_synthesizer import RimeSynthesizer
-from voiceos.models.synthesizer_cost import SynthesizerCost
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
+from voiceos.models.play_ht_model import PlayHTModel
+from voiceos.models.playht_voice import PlayhtVoice
+from voiceos.models.rime_speaker import RimeSpeaker
+from voiceos.models.rime_voice import RimeVoice
+from voiceos.models.speaker import Speaker
 from voiceos.models.telephony_cost import TelephonyCost
 from voiceos.models.transcriber import Transcriber
 from voiceos.models.transcriber1 import Transcriber1
 from voiceos.models.transcriber_cost import TranscriberCost
+from voiceos.models.twilio_phone_call import TwilioPhoneCall
 from voiceos.models.twilio_telephony import TwilioTelephony
 from voiceos.models.update_agent import UpdateAgent
 from voiceos.models.update_phone_number import UpdatePhoneNumber
 from voiceos.models.validation_error import ValidationError
 from voiceos.models.validation_error_loc_inner import ValidationErrorLocInner
 from voiceos.models.voice import Voice
 from voiceos.models.voice1 import Voice1
+from voiceos.models.voice_cost import VoiceCost
+from voiceos.models.voice_id import VoiceId
 from voiceos.models.wako_api_models_language_model_provider import WakoApiModelsLanguageModelProvider
 from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
+from voiceos.models.wako_api_models_synthesizer_deepgram_model import WakoApiModelsSynthesizerDeepgramModel
 from voiceos.models.wako_api_models_synthesizer_provider import WakoApiModelsSynthesizerProvider
+from voiceos.models.wako_api_models_transcriber_deepgram_model import WakoApiModelsTranscriberDeepgramModel
 from voiceos.models.wako_api_models_transcriber_provider import WakoApiModelsTranscriberProvider
 from voiceos.models.webhook import Webhook
```

### Comparing `voiceos-0.8.1.2/voiceos/api/agents_api.py` & `voiceos-0.8.1.3/voiceos/api/agents_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
-from pydantic import StrictInt, StrictStr
+from pydantic import Field, StrictInt, StrictStr
 from typing import Optional
+from typing_extensions import Annotated
 from voiceos.models.agent_configuration import AgentConfiguration
 from voiceos.models.agent_pagination import AgentPagination
 from voiceos.models.agent_response import AgentResponse
 from voiceos.models.update_agent import UpdateAgent
 
 from voiceos.api_client import ApiClient, RequestSerialized
 from voiceos.api_response import ApiResponse
@@ -288,15 +289,15 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/agents',
             path_params=_path_params,
             query_params=_query_params,
@@ -312,15 +313,15 @@
 
 
 
 
     @validate_call
     def delete_agent(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -329,16 +330,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> AgentResponse:
         """Delete Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -354,15 +355,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -379,15 +380,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def delete_agent_with_http_info(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -396,16 +397,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[AgentResponse]:
         """Delete Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -421,15 +422,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -446,15 +447,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def delete_agent_without_preload_content(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -463,16 +464,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Delete Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -488,15 +489,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._delete_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -508,15 +509,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _delete_agent_serialize(
         self,
-        agent_id,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -528,16 +529,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if agent_id is not None:
-            _path_params['agent_id'] = agent_id
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -546,20 +547,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/agents/{agent_id}',
+            resource_path='/agents/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -570,15 +571,15 @@
 
 
 
 
     @validate_call
     def get_agent(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -587,16 +588,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> AgentResponse:
         """Get Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -612,15 +613,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -637,15 +638,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def get_agent_with_http_info(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -654,16 +655,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[AgentResponse]:
         """Get Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -679,15 +680,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -704,15 +705,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def get_agent_without_preload_content(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -721,16 +722,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -746,15 +747,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -766,15 +767,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _get_agent_serialize(
         self,
-        agent_id,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -786,16 +787,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if agent_id is not None:
-            _path_params['agent_id'] = agent_id
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -804,20 +805,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/agents/{agent_id}',
+            resource_path='/agents/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -828,18 +829,18 @@
 
 
 
 
     @validate_call
     def list_agents(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the agent was created.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the agent was created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -848,22 +849,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> AgentPagination:
         """List Agents
 
 
-        :param created_after:
+        :param created_after: The date after which the agent was created.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date before which the agent was created.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -882,15 +883,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_agents_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -907,18 +908,18 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def list_agents_with_http_info(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the agent was created.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the agent was created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -927,22 +928,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[AgentPagination]:
         """List Agents
 
 
-        :param created_after:
+        :param created_after: The date after which the agent was created.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date before which the agent was created.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -961,15 +962,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_agents_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -986,18 +987,18 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def list_agents_without_preload_content(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the agent was created.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the agent was created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1006,22 +1007,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """List Agents
 
 
-        :param created_after:
+        :param created_after: The date after which the agent was created.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date before which the agent was created.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1040,15 +1041,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_agents_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1063,15 +1064,15 @@
 
 
     def _list_agents_serialize(
         self,
         created_after,
         created_before,
         index,
-        size,
+        limit,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1114,17 +1115,17 @@
             else:
                 _query_params.append(('created_before', created_before))
             
         if index is not None:
             
             _query_params.append(('index', index))
             
-        if size is not None:
+        if limit is not None:
             
-            _query_params.append(('size', size))
+            _query_params.append(('limit', limit))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1133,15 +1134,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/agents',
             path_params=_path_params,
             query_params=_query_params,
@@ -1157,15 +1158,15 @@
 
 
 
 
     @validate_call
     def update_agent(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         update_agent: UpdateAgent,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1175,16 +1176,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> AgentResponse:
         """Update Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param update_agent: (required)
         :type update_agent: UpdateAgent
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1202,15 +1203,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._update_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             update_agent=update_agent,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -1228,15 +1229,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def update_agent_with_http_info(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         update_agent: UpdateAgent,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1246,16 +1247,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[AgentResponse]:
         """Update Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param update_agent: (required)
         :type update_agent: UpdateAgent
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1273,15 +1274,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._update_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             update_agent=update_agent,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -1299,15 +1300,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def update_agent_without_preload_content(
         self,
-        agent_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the agent.")],
         update_agent: UpdateAgent,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1317,16 +1318,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Update Agent
 
 
-        :param agent_id: (required)
-        :type agent_id: str
+        :param id: The id of the agent. (required)
+        :type id: str
         :param update_agent: (required)
         :type update_agent: UpdateAgent
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1344,15 +1345,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._update_agent_serialize(
-            agent_id=agent_id,
+            id=id,
             update_agent=update_agent,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -1365,15 +1366,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _update_agent_serialize(
         self,
-        agent_id,
+        id,
         update_agent,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -1386,16 +1387,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if agent_id is not None:
-            _path_params['agent_id'] = agent_id
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
         if update_agent is not None:
             _body_params = update_agent
 
@@ -1419,20 +1420,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/agents/{agent_id}',
+            resource_path='/agents/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `voiceos-0.8.1.2/voiceos/api/calls_api.py` & `voiceos-0.8.1.3/voiceos/api/conversations_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
-from pydantic import StrictInt, StrictStr
-from typing import Optional
-from voiceos.models.call_recording import CallRecording
-from voiceos.models.call_response import CallResponse
-from voiceos.models.call_status import CallStatus
-from voiceos.models.calls_pagination import CallsPagination
+from pydantic import Field, StrictInt, StrictStr
+from typing import Any, Optional
+from typing_extensions import Annotated
+from voiceos.models.conversation_recording import ConversationRecording
+from voiceos.models.conversation_response import ConversationResponse
+from voiceos.models.conversations_pagination import ConversationsPagination
 from voiceos.models.create_call import CreateCall
-from voiceos.models.create_call_response import CreateCallResponse
 
 from voiceos.api_client import ApiClient, RequestSerialized
 from voiceos.api_response import ApiResponse
 from voiceos.rest import RESTResponseType
 
 
-class CallsApi:
+class ConversationsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def create_call(
+    def create_phone_call(
         self,
         create_call: CreateCall,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateCallResponse:
-        """Create Call
+    ) -> ConversationResponse:
+        """Create Phone Call
 
 
         :param create_call: (required)
         :type create_call: CreateCall
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -84,55 +83,55 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_call_serialize(
+        _param = self._create_phone_call_serialize(
             create_call=create_call,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCallResponse",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_call_with_http_info(
+    def create_phone_call_with_http_info(
         self,
         create_call: CreateCall,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateCallResponse]:
-        """Create Call
+    ) -> ApiResponse[ConversationResponse]:
+        """Create Phone Call
 
 
         :param create_call: (required)
         :type create_call: CreateCall
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -151,39 +150,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_call_serialize(
+        _param = self._create_phone_call_serialize(
             create_call=create_call,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCallResponse",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_call_without_preload_content(
+    def create_phone_call_without_preload_content(
         self,
         create_call: CreateCall,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -191,15 +190,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create Call
+        """Create Phone Call
 
 
         :param create_call: (required)
         :type create_call: CreateCall
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -218,34 +217,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_call_serialize(
+        _param = self._create_phone_call_serialize(
             create_call=create_call,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCallResponse",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_call_serialize(
+    def _create_phone_call_serialize(
         self,
         create_call,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
@@ -290,20 +289,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/calls/create',
+            resource_path='/conversations/create_phone_call',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -312,35 +311,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_call(
+    def get_audio_recording(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CallResponse:
-        """Get Call
+    ) -> ConversationRecording:
+        """Get Conversation Recording
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -355,59 +354,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_call_serialize(
-            call_id=call_id,
+        _param = self._get_audio_recording_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallResponse",
+            '200': "ConversationRecording",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_call_with_http_info(
+    def get_audio_recording_with_http_info(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CallResponse]:
-        """Get Call
+    ) -> ApiResponse[ConversationRecording]:
+        """Get Conversation Recording
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -422,59 +421,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_call_serialize(
-            call_id=call_id,
+        _param = self._get_audio_recording_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallResponse",
+            '200': "ConversationRecording",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_call_without_preload_content(
+    def get_audio_recording_without_preload_content(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get Call
+        """Get Conversation Recording
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -489,36 +488,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_call_serialize(
-            call_id=call_id,
+        _param = self._get_audio_recording_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallResponse",
+            '200': "ConversationRecording",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_call_serialize(
+    def _get_audio_recording_serialize(
         self,
-        call_id,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -530,16 +529,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if call_id is not None:
-            _path_params['call_id'] = call_id
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -548,20 +547,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/calls/{call_id}',
+            resource_path='/conversations/{id}/recording',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -570,35 +569,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_recording(
+    def get_conversation(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CallRecording:
-        """Get Call Recording
+    ) -> ConversationResponse:
+        """Get Conversation
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -613,59 +612,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_recording_serialize(
-            call_id=call_id,
+        _param = self._get_conversation_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallRecording",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_recording_with_http_info(
+    def get_conversation_with_http_info(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CallRecording]:
-        """Get Call Recording
+    ) -> ApiResponse[ConversationResponse]:
+        """Get Conversation
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -680,59 +679,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_recording_serialize(
-            call_id=call_id,
+        _param = self._get_conversation_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallRecording",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_recording_without_preload_content(
+    def get_conversation_without_preload_content(
         self,
-        call_id: StrictStr,
+        id: Annotated[StrictStr, Field(description="The id of the conversation.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get Call Recording
+        """Get Conversation
 
 
-        :param call_id: (required)
-        :type call_id: str
+        :param id: The id of the conversation. (required)
+        :type id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -747,36 +746,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_recording_serialize(
-            call_id=call_id,
+        _param = self._get_conversation_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallRecording",
+            '200': "ConversationResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_recording_serialize(
+    def _get_conversation_serialize(
         self,
-        call_id,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -788,16 +787,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if call_id is not None:
-            _path_params['call_id'] = call_id
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -806,20 +805,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/calls/{call_id}/recording',
+            resource_path='/conversations/{id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -828,47 +827,47 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_calls(
+    def list_conversations(
         self,
-        status: Optional[CallStatus] = None,
-        created_before: Optional[datetime] = None,
-        created_after: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        status: Annotated[Optional[Any], Field(description="The status of the conversations.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the conversations were created.")] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the conversations were created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CallsPagination:
-        """List Calls
+    ) -> ConversationsPagination:
+        """List Conversations
 
 
-        :param status:
-        :type status: CallStatus
-        :param created_before:
+        :param status: The status of the conversations.
+        :type status: ConversationStatus
+        :param created_before: The date before which the conversations were created.
         :type created_before: datetime
-        :param created_after:
+        :param created_after: The date after which the conversations were created.
         :type created_after: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -883,75 +882,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_calls_serialize(
+        _param = self._list_conversations_serialize(
             status=status,
             created_before=created_before,
             created_after=created_after,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallsPagination",
+            '200': "ConversationsPagination",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_calls_with_http_info(
+    def list_conversations_with_http_info(
         self,
-        status: Optional[CallStatus] = None,
-        created_before: Optional[datetime] = None,
-        created_after: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        status: Annotated[Optional[Any], Field(description="The status of the conversations.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the conversations were created.")] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the conversations were created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CallsPagination]:
-        """List Calls
+    ) -> ApiResponse[ConversationsPagination]:
+        """List Conversations
 
 
-        :param status:
-        :type status: CallStatus
-        :param created_before:
+        :param status: The status of the conversations.
+        :type status: ConversationStatus
+        :param created_before: The date before which the conversations were created.
         :type created_before: datetime
-        :param created_after:
+        :param created_after: The date after which the conversations were created.
         :type created_after: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -966,75 +965,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_calls_serialize(
+        _param = self._list_conversations_serialize(
             status=status,
             created_before=created_before,
             created_after=created_after,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallsPagination",
+            '200': "ConversationsPagination",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_calls_without_preload_content(
+    def list_conversations_without_preload_content(
         self,
-        status: Optional[CallStatus] = None,
-        created_before: Optional[datetime] = None,
-        created_after: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        status: Annotated[Optional[Any], Field(description="The status of the conversations.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date before which the conversations were created.")] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date after which the conversations were created.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The limit of items to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """List Calls
+        """List Conversations
 
 
-        :param status:
-        :type status: CallStatus
-        :param created_before:
+        :param status: The status of the conversations.
+        :type status: ConversationStatus
+        :param created_before: The date before which the conversations were created.
         :type created_before: datetime
-        :param created_after:
+        :param created_after: The date after which the conversations were created.
         :type created_after: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The limit of items to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1049,44 +1048,44 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_calls_serialize(
+        _param = self._list_conversations_serialize(
             status=status,
             created_before=created_before,
             created_after=created_after,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CallsPagination",
+            '200': "ConversationsPagination",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_calls_serialize(
+    def _list_conversations_serialize(
         self,
         status,
         created_before,
         created_after,
         index,
-        size,
+        limit,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1133,17 +1132,17 @@
             else:
                 _query_params.append(('created_after', created_after))
             
         if index is not None:
             
             _query_params.append(('index', index))
             
-        if size is not None:
+        if limit is not None:
             
-            _query_params.append(('size', size))
+            _query_params.append(('limit', limit))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1152,20 +1151,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/calls',
+            resource_path='/conversations',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `voiceos-0.8.1.2/voiceos/api/phone_numbers_api.py` & `voiceos-0.8.1.3/voiceos/api/phone_numbers_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
-from pydantic import StrictBool, StrictInt, StrictStr
+from pydantic import Field, StrictBool, StrictInt, StrictStr
 from typing import Optional
+from typing_extensions import Annotated
 from voiceos.models.buy_phone_number import BuyPhoneNumber
 from voiceos.models.phone_number import PhoneNumber
 from voiceos.models.phone_number_pagination import PhoneNumberPagination
 from voiceos.models.phone_number_response import PhoneNumberResponse
 from voiceos.models.phone_number_to_buy import PhoneNumberToBuy
 from voiceos.models.update_phone_number import UpdatePhoneNumber
 
@@ -41,35 +42,38 @@
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def buy_phone_number_phone_numbers_buy_post(
+    def available_numbers_to_buy(
         self,
-        buy_phone_number: BuyPhoneNumber,
+        contains: Annotated[Optional[StrictStr], Field(description="The digits that the phone number contains.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of available phone numbers to return.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PhoneNumberResponse:
-        """Buy Phone Number
+    ) -> List[PhoneNumberToBuy]:
+        """Available Phone Numbers To Buy
 
 
-        :param buy_phone_number: (required)
-        :type buy_phone_number: BuyPhoneNumber
+        :param contains: The digits that the phone number contains.
+        :type contains: str
+        :param limit: The number of available phone numbers to return.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -84,59 +88,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._buy_phone_number_phone_numbers_buy_post_serialize(
-            buy_phone_number=buy_phone_number,
+        _param = self._available_numbers_to_buy_serialize(
+            contains=contains,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "List[PhoneNumberToBuy]",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def buy_phone_number_phone_numbers_buy_post_with_http_info(
+    def available_numbers_to_buy_with_http_info(
         self,
-        buy_phone_number: BuyPhoneNumber,
+        contains: Annotated[Optional[StrictStr], Field(description="The digits that the phone number contains.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of available phone numbers to return.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PhoneNumberResponse]:
-        """Buy Phone Number
+    ) -> ApiResponse[List[PhoneNumberToBuy]]:
+        """Available Phone Numbers To Buy
 
 
-        :param buy_phone_number: (required)
-        :type buy_phone_number: BuyPhoneNumber
+        :param contains: The digits that the phone number contains.
+        :type contains: str
+        :param limit: The number of available phone numbers to return.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -151,59 +159,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._buy_phone_number_phone_numbers_buy_post_serialize(
-            buy_phone_number=buy_phone_number,
+        _param = self._available_numbers_to_buy_serialize(
+            contains=contains,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "List[PhoneNumberToBuy]",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def buy_phone_number_phone_numbers_buy_post_without_preload_content(
+    def available_numbers_to_buy_without_preload_content(
         self,
-        buy_phone_number: BuyPhoneNumber,
+        contains: Annotated[Optional[StrictStr], Field(description="The digits that the phone number contains.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of available phone numbers to return.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Buy Phone Number
+        """Available Phone Numbers To Buy
 
 
-        :param buy_phone_number: (required)
-        :type buy_phone_number: BuyPhoneNumber
+        :param contains: The digits that the phone number contains.
+        :type contains: str
+        :param limit: The number of available phone numbers to return.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -218,36 +230,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._buy_phone_number_phone_numbers_buy_post_serialize(
-            buy_phone_number=buy_phone_number,
+        _param = self._available_numbers_to_buy_serialize(
+            contains=contains,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "List[PhoneNumberToBuy]",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _buy_phone_number_phone_numbers_buy_post_serialize(
+    def _available_numbers_to_buy_serialize(
         self,
-        buy_phone_number,
+        contains,
+        limit,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -260,49 +274,42 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if contains is not None:
+            
+            _query_params.append(('contains', contains))
+            
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if buy_phone_number is not None:
-            _body_params = buy_phone_number
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
+            method='GET',
             resource_path='/phone_numbers/buy',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -312,38 +319,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def delete_phone_number_phone_numbers_phone_number_delete(
+    def buy_phone_number(
         self,
-        phone_number: StrictStr,
-        release_phone_number: Optional[StrictBool] = None,
+        buy_phone_number: BuyPhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PhoneNumber:
-        """Delete Phone Number
+    ) -> PhoneNumberResponse:
+        """Buy Phone Number
 
 
-        :param phone_number: (required)
-        :type phone_number: str
-        :param release_phone_number:
-        :type release_phone_number: bool
+        :param buy_phone_number: (required)
+        :type buy_phone_number: BuyPhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -358,63 +362,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_phone_number_phone_numbers_phone_number_delete_serialize(
-            phone_number=phone_number,
-            release_phone_number=release_phone_number,
+        _param = self._buy_phone_number_serialize(
+            buy_phone_number=buy_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumber",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def delete_phone_number_phone_numbers_phone_number_delete_with_http_info(
+    def buy_phone_number_with_http_info(
         self,
-        phone_number: StrictStr,
-        release_phone_number: Optional[StrictBool] = None,
+        buy_phone_number: BuyPhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PhoneNumber]:
-        """Delete Phone Number
+    ) -> ApiResponse[PhoneNumberResponse]:
+        """Buy Phone Number
 
 
-        :param phone_number: (required)
-        :type phone_number: str
-        :param release_phone_number:
-        :type release_phone_number: bool
+        :param buy_phone_number: (required)
+        :type buy_phone_number: BuyPhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -429,63 +429,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_phone_number_phone_numbers_phone_number_delete_serialize(
-            phone_number=phone_number,
-            release_phone_number=release_phone_number,
+        _param = self._buy_phone_number_serialize(
+            buy_phone_number=buy_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumber",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def delete_phone_number_phone_numbers_phone_number_delete_without_preload_content(
+    def buy_phone_number_without_preload_content(
         self,
-        phone_number: StrictStr,
-        release_phone_number: Optional[StrictBool] = None,
+        buy_phone_number: BuyPhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete Phone Number
+        """Buy Phone Number
 
 
-        :param phone_number: (required)
-        :type phone_number: str
-        :param release_phone_number:
-        :type release_phone_number: bool
+        :param buy_phone_number: (required)
+        :type buy_phone_number: BuyPhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -500,38 +496,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_phone_number_phone_numbers_phone_number_delete_serialize(
-            phone_number=phone_number,
-            release_phone_number=release_phone_number,
+        _param = self._buy_phone_number_serialize(
+            buy_phone_number=buy_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumber",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _delete_phone_number_phone_numbers_phone_number_delete_serialize(
+    def _buy_phone_number_serialize(
         self,
-        phone_number,
-        release_phone_number,
+        buy_phone_number,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -543,42 +537,51 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if phone_number is not None:
-            _path_params['phone_number'] = phone_number
         # process the query parameters
-        if release_phone_number is not None:
-            
-            _query_params.append(('release_phone_number', release_phone_number))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if buy_phone_number is not None:
+            _body_params = buy_phone_number
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/phone_numbers/{phone_number}',
+            method='POST',
+            resource_path='/phone_numbers/buy',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -587,35 +590,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_phone_number(
+    def delete_phone_number(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
+        release_phone_number: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PhoneNumberResponse:
-        """Get Phone Number
+    ) -> PhoneNumber:
+        """Delete Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
+        :param release_phone_number:
+        :type release_phone_number: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -630,59 +636,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_phone_number_serialize(
+        _param = self._delete_phone_number_serialize(
             phone_number=phone_number,
+            release_phone_number=release_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "PhoneNumber",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_phone_number_with_http_info(
+    def delete_phone_number_with_http_info(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
+        release_phone_number: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PhoneNumberResponse]:
-        """Get Phone Number
+    ) -> ApiResponse[PhoneNumber]:
+        """Delete Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
+        :param release_phone_number:
+        :type release_phone_number: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -697,59 +707,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_phone_number_serialize(
+        _param = self._delete_phone_number_serialize(
             phone_number=phone_number,
+            release_phone_number=release_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "PhoneNumber",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_phone_number_without_preload_content(
+    def delete_phone_number_without_preload_content(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
+        release_phone_number: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get Phone Number
+        """Delete Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
+        :param release_phone_number:
+        :type release_phone_number: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -764,36 +778,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_phone_number_serialize(
+        _param = self._delete_phone_number_serialize(
             phone_number=phone_number,
+            release_phone_number=release_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PhoneNumberResponse",
+            '200': "PhoneNumber",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_phone_number_serialize(
+    def _delete_phone_number_serialize(
         self,
         phone_number,
+        release_phone_number,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -808,14 +824,18 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if phone_number is not None:
             _path_params['phone_number'] = phone_number
         # process the query parameters
+        if release_phone_number is not None:
+            
+            _query_params.append(('release_phone_number', release_phone_number))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -823,19 +843,19 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
+            method='DELETE',
             resource_path='/phone_numbers/{phone_number}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -845,41 +865,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_available_phone_numbers(
+    def get_phone_number(
         self,
-        area_code: Optional[StrictStr] = None,
-        contains: Optional[StrictStr] = None,
-        limit: Optional[StrictInt] = None,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[PhoneNumberToBuy]:
-        """List Available Phone Numbers
+    ) -> PhoneNumberResponse:
+        """Get Phone Number
 
 
-        :param area_code:
-        :type area_code: str
-        :param contains:
-        :type contains: str
-        :param limit:
-        :type limit: int
+        :param phone_number: The phone number including the country code. (required)
+        :type phone_number: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -894,67 +908,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_available_phone_numbers_serialize(
-            area_code=area_code,
-            contains=contains,
-            limit=limit,
+        _param = self._get_phone_number_serialize(
+            phone_number=phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[PhoneNumberToBuy]",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_available_phone_numbers_with_http_info(
+    def get_phone_number_with_http_info(
         self,
-        area_code: Optional[StrictStr] = None,
-        contains: Optional[StrictStr] = None,
-        limit: Optional[StrictInt] = None,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[PhoneNumberToBuy]]:
-        """List Available Phone Numbers
+    ) -> ApiResponse[PhoneNumberResponse]:
+        """Get Phone Number
 
 
-        :param area_code:
-        :type area_code: str
-        :param contains:
-        :type contains: str
-        :param limit:
-        :type limit: int
+        :param phone_number: The phone number including the country code. (required)
+        :type phone_number: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -969,67 +975,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_available_phone_numbers_serialize(
-            area_code=area_code,
-            contains=contains,
-            limit=limit,
+        _param = self._get_phone_number_serialize(
+            phone_number=phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[PhoneNumberToBuy]",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_available_phone_numbers_without_preload_content(
+    def get_phone_number_without_preload_content(
         self,
-        area_code: Optional[StrictStr] = None,
-        contains: Optional[StrictStr] = None,
-        limit: Optional[StrictInt] = None,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """List Available Phone Numbers
+        """Get Phone Number
 
 
-        :param area_code:
-        :type area_code: str
-        :param contains:
-        :type contains: str
-        :param limit:
-        :type limit: int
+        :param phone_number: The phone number including the country code. (required)
+        :type phone_number: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1044,40 +1042,36 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_available_phone_numbers_serialize(
-            area_code=area_code,
-            contains=contains,
-            limit=limit,
+        _param = self._get_phone_number_serialize(
+            phone_number=phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[PhoneNumberToBuy]",
+            '200': "PhoneNumberResponse",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_available_phone_numbers_serialize(
+    def _get_phone_number_serialize(
         self,
-        area_code,
-        contains,
-        limit,
+        phone_number,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1089,27 +1083,17 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if phone_number is not None:
+            _path_params['phone_number'] = phone_number
         # process the query parameters
-        if area_code is not None:
-            
-            _query_params.append(('area_code', area_code))
-            
-        if contains is not None:
-            
-            _query_params.append(('contains', contains))
-            
-        if limit is not None:
-            
-            _query_params.append(('limit', limit))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1117,20 +1101,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/phone_numbers/buy',
+            resource_path='/phone_numbers/{phone_number}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1141,18 +1125,18 @@
 
 
 
 
     @validate_call
     def list_phone_numbers(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date the phone number was created after.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date the phone number was created before.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of phone numbers to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1161,22 +1145,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PhoneNumberPagination:
         """List Phone Numbers
 
 
-        :param created_after:
+        :param created_after: The date the phone number was created after.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date the phone number was created before.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The number of phone numbers to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1195,15 +1179,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_phone_numbers_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1220,18 +1204,18 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def list_phone_numbers_with_http_info(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date the phone number was created after.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date the phone number was created before.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of phone numbers to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1240,22 +1224,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PhoneNumberPagination]:
         """List Phone Numbers
 
 
-        :param created_after:
+        :param created_after: The date the phone number was created after.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date the phone number was created before.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The number of phone numbers to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1274,15 +1258,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_phone_numbers_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1299,18 +1283,18 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def list_phone_numbers_without_preload_content(
         self,
-        created_after: Optional[datetime] = None,
-        created_before: Optional[datetime] = None,
-        index: Optional[StrictInt] = None,
-        size: Optional[StrictInt] = None,
+        created_after: Annotated[Optional[datetime], Field(description="The date the phone number was created after.")] = None,
+        created_before: Annotated[Optional[datetime], Field(description="The date the phone number was created before.")] = None,
+        index: Annotated[Optional[StrictInt], Field(description="The index of the page to return.")] = None,
+        limit: Annotated[Optional[StrictInt], Field(description="The number of phone numbers to return in the page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1319,22 +1303,22 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """List Phone Numbers
 
 
-        :param created_after:
+        :param created_after: The date the phone number was created after.
         :type created_after: datetime
-        :param created_before:
+        :param created_before: The date the phone number was created before.
         :type created_before: datetime
-        :param index:
+        :param index: The index of the page to return.
         :type index: int
-        :param size:
-        :type size: int
+        :param limit: The number of phone numbers to return in the page.
+        :type limit: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1353,15 +1337,15 @@
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._list_phone_numbers_serialize(
             created_after=created_after,
             created_before=created_before,
             index=index,
-            size=size,
+            limit=limit,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1376,15 +1360,15 @@
 
 
     def _list_phone_numbers_serialize(
         self,
         created_after,
         created_before,
         index,
-        size,
+        limit,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1427,17 +1411,17 @@
             else:
                 _query_params.append(('created_before', created_before))
             
         if index is not None:
             
             _query_params.append(('index', index))
             
-        if size is not None:
+        if limit is not None:
             
-            _query_params.append(('size', size))
+            _query_params.append(('limit', limit))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1446,15 +1430,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/phone_numbers',
             path_params=_path_params,
             query_params=_query_params,
@@ -1468,17 +1452,17 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def update_phone_number_phone_numbers_phone_number_patch(
+    def update_phone_number(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         update_phone_number: UpdatePhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1488,15 +1472,15 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PhoneNumberResponse:
         """Update Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
         :param update_phone_number: (required)
         :type update_phone_number: UpdatePhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1514,15 +1498,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_phone_number_phone_numbers_phone_number_patch_serialize(
+        _param = self._update_phone_number_serialize(
             phone_number=phone_number,
             update_phone_number=update_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1539,17 +1523,17 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def update_phone_number_phone_numbers_phone_number_patch_with_http_info(
+    def update_phone_number_with_http_info(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         update_phone_number: UpdatePhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1559,15 +1543,15 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PhoneNumberResponse]:
         """Update Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
         :param update_phone_number: (required)
         :type update_phone_number: UpdatePhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1585,15 +1569,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_phone_number_phone_numbers_phone_number_patch_serialize(
+        _param = self._update_phone_number_serialize(
             phone_number=phone_number,
             update_phone_number=update_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1610,17 +1594,17 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def update_phone_number_phone_numbers_phone_number_patch_without_preload_content(
+    def update_phone_number_without_preload_content(
         self,
-        phone_number: StrictStr,
+        phone_number: Annotated[StrictStr, Field(description="The phone number including the country code.")],
         update_phone_number: UpdatePhoneNumber,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1630,15 +1614,15 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Update Phone Number
 
 
-        :param phone_number: (required)
+        :param phone_number: The phone number including the country code. (required)
         :type phone_number: str
         :param update_phone_number: (required)
         :type update_phone_number: UpdatePhoneNumber
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1656,15 +1640,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_phone_number_phone_numbers_phone_number_patch_serialize(
+        _param = self._update_phone_number_serialize(
             phone_number=phone_number,
             update_phone_number=update_phone_number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1676,15 +1660,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _update_phone_number_phone_numbers_phone_number_patch_serialize(
+    def _update_phone_number_serialize(
         self,
         phone_number,
         update_phone_number,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
@@ -1732,15 +1716,15 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'APIKeyHeader'
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
             resource_path='/phone_numbers/{phone_number}',
             path_params=_path_params,
             query_params=_query_params,
```

### Comparing `voiceos-0.8.1.2/voiceos/api_client.py` & `voiceos-0.8.1.3/voiceos/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import datetime
```

### Comparing `voiceos-0.8.1.2/voiceos/api_response.py` & `voiceos-0.8.1.3/voiceos/api_response.py`

 * *Files identical despite different names*

### Comparing `voiceos-0.8.1.2/voiceos/client.py` & `voiceos-0.8.1.3/voiceos/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from voiceos.configuration import Configuration
 from voiceos.api_client import ApiClient
 from voiceos.api.agents_api import AgentsApi
-from voiceos.api.calls_api import CallsApi
+from voiceos.api.conversations_api import ConversationsApi
 from voiceos.api.phone_numbers_api import PhoneNumbersApi
 
 class VoiceOS:
     def __init__(self, api_key):
         self.configuration = Configuration(
-            host="https://api.wako.ai",
+            host="https://api.voiceos.io",
         )
 
         self.client = ApiClient(
             configuration=self.configuration,
-            header_name="X-API-KEY",
-            header_value=api_key,
+            header_name="Authorization",
+            header_value="Bearer " + api_key,
         )
 
         self.agents = AgentsApi(self.client)
 
-        self.calls = CallsApi(self.client)
+        self.conversations = ConversationsApi(self.client)
 
         self.phone_numbers = PhoneNumbersApi(self.client)
```

### Comparing `voiceos-0.8.1.2/voiceos/configuration.py` & `voiceos-0.8.1.3/voiceos/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -52,33 +52,14 @@
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum
       values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
     :Example:
-
-    API Key Authentication Example.
-    Given the following security scheme in the OpenAPI specification:
-      components:
-        securitySchemes:
-          cookieAuth:         # name for the security scheme
-            type: apiKey
-            in: cookie
-            name: JSESSIONID  # cookie name
-
-    You can programmatically set the cookie:
-
-conf = voiceos.Configuration(
-    api_key={'cookieAuth': 'abc123'}
-    api_key_prefix={'cookieAuth': 'JSESSIONID'}
-)
-
-    The following cookie will be added to the HTTP request:
-       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -375,43 +356,32 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if 'APIKeyHeader' in self.api_key:
-            auth['APIKeyHeader'] = {
-                'type': 'api_key',
-                'in': 'header',
-                'key': 'X-API-KEY',
-                'value': self.get_api_key_with_prefix(
-                    'APIKeyHeader',
-                ),
-            }
-        if 'X-API-KEY' in self.api_key:
-            auth['X-API-KEY'] = {
-                'type': 'api_key',
+        if self.access_token is not None:
+            auth['Bearer'] = {
+                'type': 'bearer',
                 'in': 'header',
-                'key': 'X-API-KEY',
-                'value': self.get_api_key_with_prefix(
-                    'X-API-KEY',
-                ),
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.0\n"\
+               "Version of the API: 0.8.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `voiceos-0.8.1.2/voiceos/exceptions.py` & `voiceos-0.8.1.3/voiceos/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
 from typing_extensions import Self
```

### Comparing `voiceos-0.8.1.2/voiceos/models/__init__.py` & `voiceos-0.8.1.3/voiceos/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,106 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-# import models into model package
-from voiceos.models.agent import Agent
+__version__ = "1.0.0"
+
+# import apis into sdk package
+from voiceos.api.agents_api import AgentsApi
+from voiceos.api.conversations_api import ConversationsApi
+from voiceos.api.phone_numbers_api import PhoneNumbersApi
+
+# import ApiClient
+from voiceos.api_response import ApiResponse
+from voiceos.api_client import ApiClient
+from voiceos.configuration import Configuration
+from voiceos.exceptions import OpenApiException
+from voiceos.exceptions import ApiTypeError
+from voiceos.exceptions import ApiValueError
+from voiceos.exceptions import ApiKeyError
+from voiceos.exceptions import ApiAttributeError
+from voiceos.exceptions import ApiException
+
+# import models into sdk package
 from voiceos.models.agent_configuration import AgentConfiguration
 from voiceos.models.agent_cost import AgentCost
-from voiceos.models.agent_language import AgentLanguage
 from voiceos.models.agent_pagination import AgentPagination
 from voiceos.models.agent_provider import AgentProvider
 from voiceos.models.agent_response import AgentResponse
 from voiceos.models.azure_languages import AzureLanguages
 from voiceos.models.azure_model import AzureModel
-from voiceos.models.azure_synthesizer import AzureSynthesizer
 from voiceos.models.azure_transcriber import AzureTranscriber
+from voiceos.models.azure_transcriber_languages_inner import AzureTranscriberLanguagesInner
+from voiceos.models.azure_voice import AzureVoice
 from voiceos.models.buy_phone_number import BuyPhoneNumber
-from voiceos.models.call_cost import CallCost
-from voiceos.models.call_recording import CallRecording
-from voiceos.models.call_response import CallResponse
-from voiceos.models.call_status import CallStatus
-from voiceos.models.call_type import CallType
-from voiceos.models.calls_pagination import CallsPagination
 from voiceos.models.chat_gpt import ChatGPT
+from voiceos.models.conversation_cost import ConversationCost
+from voiceos.models.conversation_recording import ConversationRecording
+from voiceos.models.conversation_response import ConversationResponse
+from voiceos.models.conversation_status import ConversationStatus
+from voiceos.models.conversation_type import ConversationType
+from voiceos.models.conversations_pagination import ConversationsPagination
 from voiceos.models.create_call import CreateCall
-from voiceos.models.create_call_response import CreateCallResponse
-from voiceos.models.currency import Currency
 from voiceos.models.deepgram_languages import DeepgramLanguages
-from voiceos.models.deepgram_model import DeepgramModel
 from voiceos.models.deepgram_transcriber import DeepgramTranscriber
+from voiceos.models.deepgram_voice import DeepgramVoice
 from voiceos.models.eleven_labs_model import ElevenLabsModel
-from voiceos.models.eleven_labs_synthesizer import ElevenLabsSynthesizer
+from voiceos.models.eleven_labs_voices import ElevenLabsVoices
+from voiceos.models.elevenlabs_voice import ElevenlabsVoice
 from voiceos.models.ended_reasons import EndedReasons
-from voiceos.models.event import Event
 from voiceos.models.event_name import EventName
-from voiceos.models.event_variable_name import EventVariableName
 from voiceos.models.http_validation_error import HTTPValidationError
+from voiceos.models.language import Language
 from voiceos.models.language_model_cost import LanguageModelCost
 from voiceos.models.message import Message
 from voiceos.models.message_role import MessageRole
 from voiceos.models.method_enum import MethodEnum
+from voiceos.models.model import Model
+from voiceos.models.model1 import Model1
+from voiceos.models.model2 import Model2
+from voiceos.models.model3 import Model3
+from voiceos.models.model4 import Model4
 from voiceos.models.open_ai import OpenAI
-from voiceos.models.open_ai_function import OpenAIFunction
-from voiceos.models.open_ai_function_parameter import OpenAIFunctionParameter
-from voiceos.models.open_ai_function_type import OpenAIFunctionType
 from voiceos.models.phone_number import PhoneNumber
+from voiceos.models.phone_number_events import PhoneNumberEvents
 from voiceos.models.phone_number_pagination import PhoneNumberPagination
 from voiceos.models.phone_number_response import PhoneNumberResponse
 from voiceos.models.phone_number_to_buy import PhoneNumberToBuy
-from voiceos.models.rime_synthesizer import RimeSynthesizer
-from voiceos.models.synthesizer_cost import SynthesizerCost
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
+from voiceos.models.play_ht_model import PlayHTModel
+from voiceos.models.playht_voice import PlayhtVoice
+from voiceos.models.rime_speaker import RimeSpeaker
+from voiceos.models.rime_voice import RimeVoice
+from voiceos.models.speaker import Speaker
 from voiceos.models.telephony_cost import TelephonyCost
 from voiceos.models.transcriber import Transcriber
 from voiceos.models.transcriber1 import Transcriber1
 from voiceos.models.transcriber_cost import TranscriberCost
+from voiceos.models.twilio_phone_call import TwilioPhoneCall
 from voiceos.models.twilio_telephony import TwilioTelephony
 from voiceos.models.update_agent import UpdateAgent
 from voiceos.models.update_phone_number import UpdatePhoneNumber
 from voiceos.models.validation_error import ValidationError
 from voiceos.models.validation_error_loc_inner import ValidationErrorLocInner
 from voiceos.models.voice import Voice
 from voiceos.models.voice1 import Voice1
+from voiceos.models.voice_cost import VoiceCost
+from voiceos.models.voice_id import VoiceId
 from voiceos.models.wako_api_models_language_model_provider import WakoApiModelsLanguageModelProvider
 from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
+from voiceos.models.wako_api_models_synthesizer_deepgram_model import WakoApiModelsSynthesizerDeepgramModel
 from voiceos.models.wako_api_models_synthesizer_provider import WakoApiModelsSynthesizerProvider
+from voiceos.models.wako_api_models_transcriber_deepgram_model import WakoApiModelsTranscriberDeepgramModel
 from voiceos.models.wako_api_models_transcriber_provider import WakoApiModelsTranscriberProvider
 from voiceos.models.webhook import Webhook
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent.py` & `voiceos-0.8.1.3/voiceos/models/speaker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Optional
-from voiceos.models.agent_response import AgentResponse
+from voiceos.models.rime_speaker import RimeSpeaker
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-AGENT_ANY_OF_SCHEMAS = ["AgentResponse", "str"]
+SPEAKER_ANY_OF_SCHEMAS = ["RimeSpeaker", "str"]
 
-class Agent(BaseModel):
+class Speaker(BaseModel):
     """
-    Agent
+    The speaker of the voice.
     """
 
+    # data type: RimeSpeaker
+    anyof_schema_1_validator: Optional[RimeSpeaker] = None
     # data type: str
-    anyof_schema_1_validator: Optional[StrictStr] = None
-    # data type: AgentResponse
-    anyof_schema_2_validator: Optional[AgentResponse] = None
+    anyof_schema_2_validator: Optional[StrictStr] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[AgentResponse, str]] = None
+        actual_instance: Optional[Union[RimeSpeaker, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["AgentResponse", "str"])
+    any_of_schemas: List[str] = Field(default=Literal["RimeSpeaker", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +54,76 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Agent.model_construct()
+        instance = Speaker.model_construct()
         error_messages = []
+        # validate data type: RimeSpeaker
+        if not isinstance(v, RimeSpeaker):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `RimeSpeaker`")
+        else:
+            return v
+
         # validate data type: str
         try:
-            instance.anyof_schema_1_validator = v
+            instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # validate data type: AgentResponse
-        if not isinstance(v, AgentResponse):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AgentResponse`")
-        else:
-            return v
-
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Agent with anyOf schemas: AgentResponse, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Speaker with anyOf schemas: RimeSpeaker, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
+        # anyof_schema_1_validator: Optional[RimeSpeaker] = None
+        try:
+            instance.actual_instance = RimeSpeaker.from_json(json_str)
+            return instance
+        except (ValidationError, ValueError) as e:
+             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.anyof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.anyof_schema_1_validator
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[AgentResponse] = None
-        try:
-            instance.actual_instance = AgentResponse.from_json(json_str)
-            return instance
-        except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Agent with anyOf schemas: AgentResponse, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Speaker with anyOf schemas: RimeSpeaker, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], AgentResponse, str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], RimeSpeaker, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_configuration.py` & `voiceos-0.8.1.3/voiceos/models/agent_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.agent_language import AgentLanguage
 from voiceos.models.open_ai import OpenAI
 from voiceos.models.transcriber import Transcriber
 from voiceos.models.voice import Voice
 from voiceos.models.webhook import Webhook
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AgentConfiguration(BaseModel):
     """
     AgentConfiguration
     """ # noqa: E501
-    name: StrictStr = Field(description="The name of the agent")
-    initial_message: StrictStr = Field(description="The initial message of the agent")
-    prompt: StrictStr = Field(description="The prompt of the agent")
-    language: Optional[AgentLanguage] = Field(default=None, description="DO NOT USE! Deprecated!")
-    language_model: Optional[OpenAI] = None
+    initial_message: Optional[StrictStr] = Field(default=None, description="The initial message that the agent will say. If null, the agent will wait for the user to speak first.")
+    prompt: Optional[StrictStr] = Field(default=None, description="The prompt of the agent.")
     voice: Optional[Voice] = None
+    language_model: Optional[OpenAI] = None
     transcriber: Optional[Transcriber] = None
-    max_call_duration: Optional[StrictInt] = Field(default=600, description="The maximum call duration in seconds. If null, the call can be of any duration. The default value is 10 min.")
-    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent")
-    __properties: ClassVar[List[str]] = ["name", "initial_message", "prompt", "language", "language_model", "voice", "transcriber", "max_call_duration", "webhooks"]
+    max_duration_seconds: Optional[StrictInt] = Field(default=600, description="The maximum conversation duration in seconds. If null, the conversation can be of any duration. The default value is 10 min.")
+    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent. These are used for real-time conversation events such as function_calls, messages and much more.")
+    metadata: Optional[Dict[str, StrictStr]] = Field(default=None, description="The metadata of the agent. This is used to store additional information about the agent.")
+    __properties: ClassVar[List[str]] = ["initial_message", "prompt", "voice", "language_model", "transcriber", "max_duration_seconds", "webhooks", "metadata"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -77,20 +75,20 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of language_model
-        if self.language_model:
-            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of voice
         if self.voice:
             _dict['voice'] = self.voice.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of language_model
+        if self.language_model:
+            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of transcriber
         if self.transcriber:
             _dict['transcriber'] = self.transcriber.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
         _items = []
         if self.webhooks:
             for _item in self.webhooks:
@@ -105,20 +103,18 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
             "initial_message": obj.get("initial_message"),
             "prompt": obj.get("prompt"),
-            "language": obj.get("language"),
-            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "voice": Voice.from_dict(obj["voice"]) if obj.get("voice") is not None else None,
+            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "transcriber": Transcriber.from_dict(obj["transcriber"]) if obj.get("transcriber") is not None else None,
-            "max_call_duration": obj.get("max_call_duration") if obj.get("max_call_duration") is not None else 600,
-            "webhooks": [Webhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None
+            "max_duration_seconds": obj.get("max_duration_seconds") if obj.get("max_duration_seconds") is not None else 600,
+            "webhooks": [Webhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None,
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_cost.py` & `voiceos-0.8.1.3/voiceos/models/open_ai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from voiceos.models.agent_provider import AgentProvider
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
+from voiceos.models.model3 import Model3
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AgentCost(BaseModel):
+class OpenAI(BaseModel):
     """
-    AgentCost
+    OpenAI
     """ # noqa: E501
-    provider: Optional[AgentProvider] = Field(default=None, description="The provider of the agent.")
-    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the agent compute usage, discount included.")
-    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of minutes used for the agent.")
-    discount: StrictInt = Field(description="The discount percentage of agent cost.")
-    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds", "discount"]
+    provider: Optional[StrictStr] = Field(default='openai', description="The language model provider.")
+    model: Optional[Model3] = None
+    __properties: ClassVar[List[str]] = ["provider", "model"]
+
+    @field_validator('provider')
+    def provider_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['openai']):
+            raise ValueError("must be one of enum values ('openai')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AgentCost from a JSON string"""
+        """Create an instance of OpenAI from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,27 +76,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AgentCost from a dict"""
+        """Create an instance of OpenAI from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider"),
-            "cost": obj.get("cost"),
-            "seconds": obj.get("seconds"),
-            "discount": obj.get("discount")
+            "provider": obj.get("provider") if obj.get("provider") is not None else 'openai',
+            "model": Model3.from_dict(obj["model"]) if obj.get("model") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_language.py` & `voiceos-0.8.1.3/voiceos/models/message_role.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class AgentLanguage(str, Enum):
+class MessageRole(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    EN = 'en'
-    FR = 'fr'
-    JA = 'ja'
-    ES = 'es'
+    AGENT = 'agent'
+    USER = 'user'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AgentLanguage from a JSON string"""
+        """Create an instance of MessageRole from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_pagination.py` & `voiceos-0.8.1.3/voiceos/models/agent_pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -25,16 +25,16 @@
 
 class AgentPagination(BaseModel):
     """
     AgentPagination
     """ # noqa: E501
     items: List[AgentResponse] = Field(description="The list of agents returned.")
     index: StrictInt = Field(description="The current index of the page selected.")
-    has_next: StrictBool = Field(description="Whether there is a next page.")
-    __properties: ClassVar[List[str]] = ["items", "index", "has_next"]
+    has_more: StrictBool = Field(description="Whether there is a next page.")
+    __properties: ClassVar[List[str]] = ["items", "index", "has_more"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -88,12 +88,12 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "items": [AgentResponse.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None,
             "index": obj.get("index"),
-            "has_next": obj.get("has_next")
+            "has_more": obj.get("has_more")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_provider.py` & `voiceos-0.8.1.3/voiceos/models/agent_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,15 +22,15 @@
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    WAKO = 'wako'
+    VOICEOS = 'voiceos'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of AgentProvider from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/agent_response.py` & `voiceos-0.8.1.3/voiceos/models/agent_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.agent_language import AgentLanguage
 from voiceos.models.open_ai import OpenAI
 from voiceos.models.transcriber import Transcriber
 from voiceos.models.voice import Voice
 from voiceos.models.webhook import Webhook
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AgentResponse(BaseModel):
     """
     AgentResponse
     """ # noqa: E501
-    name: StrictStr = Field(description="The name of the agent")
-    initial_message: StrictStr = Field(description="The initial message of the agent")
-    prompt: StrictStr = Field(description="The prompt of the agent")
-    language: Optional[AgentLanguage] = Field(default=None, description="DO NOT USE! Deprecated!")
-    language_model: Optional[OpenAI] = None
+    initial_message: Optional[StrictStr] = Field(default=None, description="The initial message that the agent will say. If null, the agent will wait for the user to speak first.")
+    prompt: Optional[StrictStr] = Field(default=None, description="The prompt of the agent.")
     voice: Optional[Voice] = None
+    language_model: Optional[OpenAI] = None
     transcriber: Optional[Transcriber] = None
-    max_call_duration: Optional[StrictInt] = Field(default=600, description="The maximum call duration in seconds. If null, the call can be of any duration. The default value is 10 min.")
-    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent")
-    id: StrictStr = Field(description="The id of the agent")
-    uri: StrictStr = Field(description="The uri of the agent")
-    account_id: StrictStr = Field(description="The id of the owner of the agent")
-    created_at: datetime = Field(description="The date and time the agent was created")
-    updated_at: datetime = Field(description="The date and time the agent was last updated")
-    __properties: ClassVar[List[str]] = ["name", "initial_message", "prompt", "language", "language_model", "voice", "transcriber", "max_call_duration", "webhooks", "id", "uri", "account_id", "created_at", "updated_at"]
+    max_duration_seconds: Optional[StrictInt] = Field(default=600, description="The maximum conversation duration in seconds. If null, the conversation can be of any duration. The default value is 10 min.")
+    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent. These are used for real-time conversation events such as function_calls, messages and much more.")
+    metadata: Optional[Dict[str, StrictStr]] = Field(default=None, description="The metadata of the agent. This is used to store additional information about the agent.")
+    uri: StrictStr = Field(description="The uri of the agent.")
+    account_id: StrictStr = Field(description="The id of the owner of the agent.")
+    created_at: datetime = Field(description="The date and time the agent was created.")
+    updated_at: datetime = Field(description="The date and time the agent was last updated.")
+    id: StrictStr = Field(description="The id of the agent.")
+    __properties: ClassVar[List[str]] = ["initial_message", "prompt", "voice", "language_model", "transcriber", "max_duration_seconds", "webhooks", "metadata", "uri", "account_id", "created_at", "updated_at", "id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -83,20 +81,20 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of language_model
-        if self.language_model:
-            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of voice
         if self.voice:
             _dict['voice'] = self.voice.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of language_model
+        if self.language_model:
+            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of transcriber
         if self.transcriber:
             _dict['transcriber'] = self.transcriber.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
         _items = []
         if self.webhooks:
             for _item in self.webhooks:
@@ -111,25 +109,23 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
             "initial_message": obj.get("initial_message"),
             "prompt": obj.get("prompt"),
-            "language": obj.get("language"),
-            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "voice": Voice.from_dict(obj["voice"]) if obj.get("voice") is not None else None,
+            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "transcriber": Transcriber.from_dict(obj["transcriber"]) if obj.get("transcriber") is not None else None,
-            "max_call_duration": obj.get("max_call_duration") if obj.get("max_call_duration") is not None else 600,
+            "max_duration_seconds": obj.get("max_duration_seconds") if obj.get("max_duration_seconds") is not None else 600,
             "webhooks": [Webhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None,
-            "id": obj.get("id"),
             "uri": obj.get("uri"),
             "account_id": obj.get("account_id"),
             "created_at": obj.get("created_at"),
-            "updated_at": obj.get("updated_at")
+            "updated_at": obj.get("updated_at"),
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/azure_languages.py` & `voiceos-0.8.1.3/voiceos/models/azure_languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/azure_synthesizer.py` & `voiceos-0.8.1.3/voiceos/models/azure_transcriber.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from typing_extensions import Annotated
-from voiceos.models.azure_model import AzureModel
+from voiceos.models.azure_transcriber_languages_inner import AzureTranscriberLanguagesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AzureSynthesizer(BaseModel):
+class AzureTranscriber(BaseModel):
     """
-    AzureSynthesizer
+    AzureTranscriber
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='azure', description="The synthesizer provider.")
-    model: Optional[AzureModel] = Field(default=None, description="The azure model to use")
-    pitch: Optional[Annotated[int, Field(le=20, strict=True, ge=-20)]] = Field(default=0, description="The pitch of the voice")
-    rate: Optional[Annotated[int, Field(le=50, strict=True, ge=-50)]] = Field(default=0, description="The rate of the voice")
-    __properties: ClassVar[List[str]] = ["provider", "model", "pitch", "rate"]
+    provider: Optional[StrictStr] = Field(default='azure', description="The transcriber provider.")
+    languages: Optional[List[AzureTranscriberLanguagesInner]] = Field(default=None, description="The selected languages for the transcription.")
+    __properties: ClassVar[List[str]] = ["provider", "languages"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -58,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AzureSynthesizer from a JSON string"""
+        """Create an instance of AzureTranscriber from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,27 +76,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in languages (list)
+        _items = []
+        if self.languages:
+            for _item in self.languages:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['languages'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AzureSynthesizer from a dict"""
+        """Create an instance of AzureTranscriber from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider") if obj.get("provider") is not None else 'azure',
-            "model": obj.get("model"),
-            "pitch": obj.get("pitch") if obj.get("pitch") is not None else 0,
-            "rate": obj.get("rate") if obj.get("rate") is not None else 0
+            "languages": [AzureTranscriberLanguagesInner.from_dict(_item) for _item in obj["languages"]] if obj.get("languages") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/azure_transcriber.py` & `voiceos-0.8.1.3/voiceos/models/update_phone_number.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.azure_languages import AzureLanguages
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AzureTranscriber(BaseModel):
+class UpdatePhoneNumber(BaseModel):
     """
-    AzureTranscriber
+    UpdatePhoneNumber
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='azure', description="The transcriber provider.")
-    languages: Optional[List[AzureLanguages]] = Field(default=None, description="The selected languages for the transcription.")
-    __properties: ClassVar[List[str]] = ["provider", "languages"]
-
-    @field_validator('provider')
-    def provider_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['azure']):
-            raise ValueError("must be one of enum values ('azure')")
-        return value
+    inbound_agent_id: Optional[StrictStr] = Field(default=None, description="The agent id that will be used for inbound calls. If null, the phone number is will not receive any calls.")
+    webhooks: Optional[List[PhoneNumberWebhook]] = Field(default=None, description="The webhooks of the phone number. This is used to fetch the agent at the start of the conversation.")
+    __properties: ClassVar[List[str]] = ["inbound_agent_id", "webhooks"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -55,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AzureTranscriber from a JSON string"""
+        """Create an instance of UpdatePhoneNumber from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,25 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
+        _items = []
+        if self.webhooks:
+            for _item in self.webhooks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['webhooks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AzureTranscriber from a dict"""
+        """Create an instance of UpdatePhoneNumber from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider") if obj.get("provider") is not None else 'azure',
-            "languages": obj.get("languages")
+            "inbound_agent_id": obj.get("inbound_agent_id"),
+            "webhooks": [PhoneNumberWebhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/buy_phone_number.py` & `voiceos-0.8.1.3/voiceos/models/twilio_phone_call.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class BuyPhoneNumber(BaseModel):
+class TwilioPhoneCall(BaseModel):
     """
-    BuyPhoneNumber
+    TwilioPhoneCall
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='twilio', description="The telephony provider.")
-    phone_number: StrictStr = Field(description="The phone number to buy.")
-    __properties: ClassVar[List[str]] = ["provider", "phone_number"]
+    provider: StrictStr = Field(description="The telephony provider of the phone call.")
+    to_number: StrictStr = Field(description="The phone number called.")
+    from_number: StrictStr = Field(description="The phone number from which the call was made.")
+    __properties: ClassVar[List[str]] = ["provider", "to_number", "from_number"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
-
         if value not in set(['twilio']):
             raise ValueError("must be one of enum values ('twilio')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -54,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of BuyPhoneNumber from a JSON string"""
+        """Create an instance of TwilioPhoneCall from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,21 +77,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of BuyPhoneNumber from a dict"""
+        """Create an instance of TwilioPhoneCall from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider") if obj.get("provider") is not None else 'twilio',
-            "phone_number": obj.get("phone_number")
+            "provider": obj.get("provider"),
+            "to_number": obj.get("to_number"),
+            "from_number": obj.get("from_number")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/call_cost.py` & `voiceos-0.8.1.3/voiceos/models/conversation_cost.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from voiceos.models.agent_cost import AgentCost
-from voiceos.models.currency import Currency
 from voiceos.models.language_model_cost import LanguageModelCost
-from voiceos.models.synthesizer_cost import SynthesizerCost
 from voiceos.models.telephony_cost import TelephonyCost
 from voiceos.models.transcriber_cost import TranscriberCost
+from voiceos.models.voice_cost import VoiceCost
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CallCost(BaseModel):
+class ConversationCost(BaseModel):
     """
-    CallCost
+    ConversationCost
     """ # noqa: E501
-    total: Union[StrictFloat, StrictInt] = Field(description="The total cost of the call.")
-    synthesizer: SynthesizerCost = Field(description="The synthetizer cost.")
+    total: Union[StrictFloat, StrictInt] = Field(description="The total cost of the conversation (USD).")
+    voice: VoiceCost = Field(description="The voice cost.")
     transcriber: TranscriberCost = Field(description="The transcriber cost.")
     language_model: LanguageModelCost = Field(description="The language model cost.")
-    telephony: Optional[TelephonyCost] = Field(default=None, description="The telephony cost. Returns null if the call was not a phone call.")
+    telephony: Optional[TelephonyCost] = Field(default=None, description="The telephony cost. Returns null if the conversation was over web.")
     agent: AgentCost = Field(description="The cost of the agent.")
-    currency: Optional[Currency] = Field(default=None, description="The currency used. As of now, we only offer USD.")
-    __properties: ClassVar[List[str]] = ["total", "synthesizer", "transcriber", "language_model", "telephony", "agent", "currency"]
+    __properties: ClassVar[List[str]] = ["total", "voice", "transcriber", "language_model", "telephony", "agent"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -55,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CallCost from a JSON string"""
+        """Create an instance of ConversationCost from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,17 +74,17 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of synthesizer
-        if self.synthesizer:
-            _dict['synthesizer'] = self.synthesizer.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of voice
+        if self.voice:
+            _dict['voice'] = self.voice.to_dict()
         # override the default output from pydantic by calling `to_dict()` of transcriber
         if self.transcriber:
             _dict['transcriber'] = self.transcriber.to_dict()
         # override the default output from pydantic by calling `to_dict()` of language_model
         if self.language_model:
             _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of telephony
@@ -95,26 +93,25 @@
         # override the default output from pydantic by calling `to_dict()` of agent
         if self.agent:
             _dict['agent'] = self.agent.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CallCost from a dict"""
+        """Create an instance of ConversationCost from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "total": obj.get("total"),
-            "synthesizer": SynthesizerCost.from_dict(obj["synthesizer"]) if obj.get("synthesizer") is not None else None,
+            "voice": VoiceCost.from_dict(obj["voice"]) if obj.get("voice") is not None else None,
             "transcriber": TranscriberCost.from_dict(obj["transcriber"]) if obj.get("transcriber") is not None else None,
             "language_model": LanguageModelCost.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "telephony": TelephonyCost.from_dict(obj["telephony"]) if obj.get("telephony") is not None else None,
-            "agent": AgentCost.from_dict(obj["agent"]) if obj.get("agent") is not None else None,
-            "currency": obj.get("currency")
+            "agent": AgentCost.from_dict(obj["agent"]) if obj.get("agent") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/call_recording.py` & `voiceos-0.8.1.3/voiceos/models/conversation_recording.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CallRecording(BaseModel):
+class ConversationRecording(BaseModel):
     """
-    CallRecording
+    ConversationRecording
     """ # noqa: E501
     recording_url: StrictStr = Field(description="The recording url of the conversation.")
     __properties: ClassVar[List[str]] = ["recording_url"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -43,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CallRecording from a JSON string"""
+        """Create an instance of ConversationRecording from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,15 +68,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CallRecording from a dict"""
+        """Create an instance of ConversationRecording from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `voiceos-0.8.1.2/voiceos/models/call_response.py` & `voiceos-0.8.1.3/voiceos/models/conversation_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.agent_response import AgentResponse
-from voiceos.models.call_cost import CallCost
-from voiceos.models.call_status import CallStatus
-from voiceos.models.call_type import CallType
+from voiceos.models.agent_configuration import AgentConfiguration
+from voiceos.models.conversation_cost import ConversationCost
+from voiceos.models.conversation_status import ConversationStatus
+from voiceos.models.conversation_type import ConversationType
 from voiceos.models.ended_reasons import EndedReasons
 from voiceos.models.message import Message
+from voiceos.models.twilio_phone_call import TwilioPhoneCall
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CallResponse(BaseModel):
+class ConversationResponse(BaseModel):
     """
-    CallResponse
+    ConversationResponse
     """ # noqa: E501
     uri: StrictStr = Field(description="The uri of the conversation.")
-    type: CallType = Field(description="The type of the call.")
-    status: CallStatus = Field(description="The status of the conversation (live or ended).")
-    to_number: Optional[StrictStr] = Field(default=None, description="The phone number that the call is going to.")
-    from_number: Optional[StrictStr] = Field(default=None, description="The phone number that call is coming from.")
-    start_time: datetime = Field(description="The start time of the conversation.")
-    end_time: Optional[datetime] = Field(default=None, description="The end time of the conversation.")
-    agent: AgentResponse = Field(description="The agent used for the call.")
-    agent_id: Optional[StrictStr] = Field(default=None, description="The id of the agent used in the call. Returns null if the call did not use an existing agent.")
-    messages: Optional[List[Message]] = Field(default=None, description="The messages of the conversation.")
+    type: ConversationType = Field(description="The type of conversation.")
     account_id: StrictStr = Field(description="The account id associated with of the conversation.")
+    status: ConversationStatus = Field(description="The status of the conversation.")
+    started_at: Optional[datetime] = Field(default=None, description="The start time of the conversation.")
+    ended_at: Optional[datetime] = Field(default=None, description="The end time of the conversation. Returns null if the conversation is has not ended.")
+    agent_config: AgentConfiguration = Field(description="The agent configuration used for the conversation.")
+    agent_id: Optional[StrictStr] = Field(default=None, description="The id of the agent used in the conversation. Returns null if the conversation did not use an existing agent.")
+    messages: Optional[List[Message]] = Field(default=None, description="The messages of the conversation.")
+    phone_call: Optional[TwilioPhoneCall] = Field(default=None, description="The phone call details of the conversation. Returns null if the conversation was over web.")
     ended_reason: Optional[EndedReasons] = Field(default=None, description="The reasons the conversation ended.")
-    cost: Optional[CallCost] = Field(default=None, description="The cost of the conversation.")
+    cost_breakdown: Optional[ConversationCost] = Field(default=None, description="The cost breakdown of the conversation.")
     id: StrictStr = Field(description="The id of the conversation.")
-    __properties: ClassVar[List[str]] = ["uri", "type", "status", "to_number", "from_number", "start_time", "end_time", "agent", "agent_id", "messages", "account_id", "ended_reason", "cost", "id"]
+    __properties: ClassVar[List[str]] = ["uri", "type", "account_id", "status", "started_at", "ended_at", "agent_config", "agent_id", "messages", "phone_call", "ended_reason", "cost_breakdown", "id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -63,15 +63,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CallResponse from a JSON string"""
+        """Create an instance of ConversationResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,50 +84,52 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of agent
-        if self.agent:
-            _dict['agent'] = self.agent.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of agent_config
+        if self.agent_config:
+            _dict['agent_config'] = self.agent_config.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in messages (list)
         _items = []
         if self.messages:
             for _item in self.messages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['messages'] = _items
-        # override the default output from pydantic by calling `to_dict()` of cost
-        if self.cost:
-            _dict['cost'] = self.cost.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of phone_call
+        if self.phone_call:
+            _dict['phone_call'] = self.phone_call.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of cost_breakdown
+        if self.cost_breakdown:
+            _dict['cost_breakdown'] = self.cost_breakdown.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CallResponse from a dict"""
+        """Create an instance of ConversationResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "uri": obj.get("uri"),
             "type": obj.get("type"),
+            "account_id": obj.get("account_id"),
             "status": obj.get("status"),
-            "to_number": obj.get("to_number"),
-            "from_number": obj.get("from_number"),
-            "start_time": obj.get("start_time"),
-            "end_time": obj.get("end_time"),
-            "agent": AgentResponse.from_dict(obj["agent"]) if obj.get("agent") is not None else None,
+            "started_at": obj.get("started_at"),
+            "ended_at": obj.get("ended_at"),
+            "agent_config": AgentConfiguration.from_dict(obj["agent_config"]) if obj.get("agent_config") is not None else None,
             "agent_id": obj.get("agent_id"),
             "messages": [Message.from_dict(_item) for _item in obj["messages"]] if obj.get("messages") is not None else None,
-            "account_id": obj.get("account_id"),
+            "phone_call": TwilioPhoneCall.from_dict(obj["phone_call"]) if obj.get("phone_call") is not None else None,
             "ended_reason": obj.get("ended_reason"),
-            "cost": CallCost.from_dict(obj["cost"]) if obj.get("cost") is not None else None,
+            "cost_breakdown": ConversationCost.from_dict(obj["cost_breakdown"]) if obj.get("cost_breakdown") is not None else None,
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/call_status.py` & `voiceos-0.8.1.3/voiceos/models/wako_api_models_phone_number_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class CallStatus(str, Enum):
+class WakoApiModelsPhoneNumberProvider(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    LIVE = 'live'
-    ENDED = 'ended'
+    TWILIO = 'twilio'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CallStatus from a JSON string"""
+        """Create an instance of WakoApiModelsPhoneNumberProvider from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/call_type.py` & `voiceos-0.8.1.3/voiceos/models/wako_api_models_language_model_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class CallType(str, Enum):
+class WakoApiModelsLanguageModelProvider(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    INBOUND_PHONE_CALL = 'inbound_phone_call'
-    OUTBOUND_PHONE_CALL = 'outbound_phone_call'
+    OPENAI = 'openai'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CallType from a JSON string"""
+        """Create an instance of WakoApiModelsLanguageModelProvider from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/calls_pagination.py` & `voiceos-0.8.1.3/voiceos/models/conversations_pagination.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt
 from typing import Any, ClassVar, Dict, List
-from voiceos.models.call_response import CallResponse
+from voiceos.models.conversation_response import ConversationResponse
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CallsPagination(BaseModel):
+class ConversationsPagination(BaseModel):
     """
-    CallsPagination
+    ConversationsPagination
     """ # noqa: E501
-    items: List[CallResponse] = Field(description="The list of conversations returned.")
+    items: List[ConversationResponse] = Field(description="The list of conversations returned.")
     index: StrictInt = Field(description="The current index of the page selected.")
-    has_next: StrictBool = Field(description="The total number of conversations.")
-    __properties: ClassVar[List[str]] = ["items", "index", "has_next"]
+    has_more: StrictBool = Field(description="The total number of conversations.")
+    __properties: ClassVar[List[str]] = ["items", "index", "has_more"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CallsPagination from a JSON string"""
+        """Create an instance of ConversationsPagination from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,22 +78,22 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['items'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CallsPagination from a dict"""
+        """Create an instance of ConversationsPagination from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "items": [CallResponse.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None,
+            "items": [ConversationResponse.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None,
             "index": obj.get("index"),
-            "has_next": obj.get("has_next")
+            "has_more": obj.get("has_more")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/chat_gpt.py` & `voiceos-0.8.1.3/voiceos/models/conversation_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class ChatGPT(str, Enum):
+class ConversationType(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    GPT_MINUS_4_MINUS_1106_MINUS_PREVIEW = 'gpt-4-1106-preview'
-    GPT_MINUS_3_DOT_5_MINUS_TURBO_MINUS_1106 = 'gpt-3.5-turbo-1106'
+    INBOUND_PHONE_CALL = 'inbound_phone_call'
+    OUTBOUND_PHONE_CALL = 'outbound_phone_call'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ChatGPT from a JSON string"""
+        """Create an instance of ConversationType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/create_call.py` & `voiceos-0.8.1.3/voiceos/models/validation_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from voiceos.models.agent import Agent
+from voiceos.models.validation_error_loc_inner import ValidationErrorLocInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateCall(BaseModel):
+class ValidationError(BaseModel):
     """
-    CreateCall
+    ValidationError
     """ # noqa: E501
-    to_number: StrictStr
-    from_number: StrictStr
-    agent: Agent
-    __properties: ClassVar[List[str]] = ["to_number", "from_number", "agent"]
+    loc: List[ValidationErrorLocInner]
+    msg: StrictStr
+    type: StrictStr
+    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateCall from a JSON string"""
+        """Create an instance of ValidationError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,29 +67,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of agent
-        if self.agent:
-            _dict['agent'] = self.agent.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
+        _items = []
+        if self.loc:
+            for _item in self.loc:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateCall from a dict"""
+        """Create an instance of ValidationError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "to_number": obj.get("to_number"),
-            "from_number": obj.get("from_number"),
-            "agent": Agent.from_dict(obj["agent"]) if obj.get("agent") is not None else None
+            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
+            "msg": obj.get("msg"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/create_call_response.py` & `voiceos-0.8.1.3/voiceos/models/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
+from voiceos.models.message_role import MessageRole
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateCallResponse(BaseModel):
+class Message(BaseModel):
     """
-    CreateCallResponse
+    Message
     """ # noqa: E501
-    id: StrictStr
-    __properties: ClassVar[List[str]] = ["id"]
+    role: MessageRole = Field(description="The role of the message.")
+    content: StrictStr = Field(description="The content of the message.")
+    __properties: ClassVar[List[str]] = ["role", "content"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -43,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateCallResponse from a JSON string"""
+        """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateCallResponse from a dict"""
+        """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id")
+            "role": obj.get("role"),
+            "content": obj.get("content")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/currency.py` & `voiceos-0.8.1.3/voiceos/models/phone_number_events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class Currency(str, Enum):
+class PhoneNumberEvents(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    USD = 'usd'
+    PHONE_CALL_COLON_CONNECTION_REQUESTED = 'phone_call:connection_requested'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Currency from a JSON string"""
+        """Create an instance of PhoneNumberEvents from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/deepgram_languages.py` & `voiceos-0.8.1.3/voiceos/models/deepgram_languages.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/deepgram_model.py` & `voiceos-0.8.1.3/voiceos/models/wako_api_models_transcriber_deepgram_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class DeepgramModel(str, Enum):
+class WakoApiModelsTranscriberDeepgramModel(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
@@ -35,11 +35,11 @@
     NOVA_MINUS_2_MINUS_MEDICAL = 'nova-2-medical'
     NOVA_MINUS_2_MINUS_DRIVETHRU = 'nova-2-drivethru'
     NOVA_MINUS_2_MINUS_AUTOMOTIVE = 'nova-2-automotive'
     NOVA_MINUS_2_MINUS_CONVERSATIONALAI = 'nova-2-conversationalai'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DeepgramModel from a JSON string"""
+        """Create an instance of WakoApiModelsTranscriberDeepgramModel from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/deepgram_transcriber.py` & `voiceos-0.8.1.3/voiceos/models/deepgram_transcriber.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.deepgram_languages import DeepgramLanguages
-from voiceos.models.deepgram_model import DeepgramModel
+from voiceos.models.language import Language
+from voiceos.models.model1 import Model1
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DeepgramTranscriber(BaseModel):
     """
     DeepgramTranscriber
     """ # noqa: E501
     provider: Optional[StrictStr] = Field(default='deepgram', description="The transcriber provider.")
-    model: Optional[DeepgramModel] = Field(default=None, description="The deepgram model to use.")
-    language: Optional[DeepgramLanguages] = Field(default=None, description="The selected language for the transcription.")
-    keywords: Optional[List[StrictStr]] = Field(default=None, description="Specific keywords you want to detect in the transcription. This is usefull to correctly understand product or company names.")
+    model: Optional[Model1] = None
+    language: Optional[Language] = None
+    keywords: Optional[List[StrictStr]] = Field(default=None, description="Specific keywords you want to detect in the transcription. This is useful to correctly understand product or company names.")
     __properties: ClassVar[List[str]] = ["provider", "model", "language", "keywords"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -79,27 +79,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of language
+        if self.language:
+            _dict['language'] = self.language.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of DeepgramTranscriber from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider") if obj.get("provider") is not None else 'deepgram',
-            "model": obj.get("model"),
-            "language": obj.get("language"),
+            "model": Model1.from_dict(obj["model"]) if obj.get("model") is not None else None,
+            "language": Language.from_dict(obj["language"]) if obj.get("language") is not None else None,
             "keywords": obj.get("keywords")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/eleven_labs_model.py` & `voiceos-0.8.1.3/voiceos/models/wako_api_models_transcriber_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class ElevenLabsModel(str, Enum):
+class WakoApiModelsTranscriberProvider(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    ENUM_21M00TCM4TLVDQ8IKWAM = '21m00Tcm4TlvDq8ikWAM'
-    ENUM_5Q0T7UMCJVNAGUMLFVZI = '5Q0t7uMcjvnagumLfvZi'
-    ENUM_29VD33N1CTXCMQQRPOHJ = '29vD33N1CtxCmqQRPOHJ'
-    ENUM_2EIWWNXFNVU5JABPNV8N = '2EiwWnXFnvU5JabPnv8n'
-    CYW3KZ02HS0563KHS1FJ = 'CYw3kZ02Hs0563khs1Fj'
-    D38Z5RCWU1VOKY8WS1JA = 'D38z5RcWu1voky8WS1ja'
-    EXAVITQU4VR4XNSDXMAL = 'EXAVITQu4vr4xnSDxMaL'
+    DEEPGRAM = 'deepgram'
+    AZURE = 'azure'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ElevenLabsModel from a JSON string"""
+        """Create an instance of WakoApiModelsTranscriberProvider from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/eleven_labs_synthesizer.py` & `voiceos-0.8.1.3/voiceos/models/azure_voice.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from voiceos.models.eleven_labs_model import ElevenLabsModel
+from voiceos.models.model import Model
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ElevenLabsSynthesizer(BaseModel):
+class AzureVoice(BaseModel):
     """
-    ElevenLabsSynthesizer
+    AzureVoice
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='elevenlabs', description="The synthesizer provider.")
-    model: Optional[ElevenLabsModel] = Field(default=None, description="The elevenlabs model to use")
-    optimize_latency: Optional[Annotated[int, Field(le=4, strict=True, ge=0)]] = Field(default=0, description="Optimize for latency")
-    __properties: ClassVar[List[str]] = ["provider", "model", "optimize_latency"]
+    provider: Optional[StrictStr] = Field(default='azure', description="The voice provider.")
+    model: Optional[Model] = None
+    pitch: Optional[Annotated[int, Field(le=20, strict=True, ge=-20)]] = Field(default=0, description="The pitch of the voice.")
+    rate: Optional[Annotated[int, Field(le=50, strict=True, ge=-50)]] = Field(default=0, description="The rate of the voice.")
+    __properties: ClassVar[List[str]] = ["provider", "model", "pitch", "rate"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['elevenlabs']):
-            raise ValueError("must be one of enum values ('elevenlabs')")
+        if value not in set(['azure']):
+            raise ValueError("must be one of enum values ('azure')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -57,15 +58,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ElevenLabsSynthesizer from a JSON string"""
+        """Create an instance of AzureVoice from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,26 +79,30 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ElevenLabsSynthesizer from a dict"""
+        """Create an instance of AzureVoice from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider") if obj.get("provider") is not None else 'elevenlabs',
-            "model": obj.get("model"),
-            "optimize_latency": obj.get("optimize_latency") if obj.get("optimize_latency") is not None else 0
+            "provider": obj.get("provider") if obj.get("provider") is not None else 'azure',
+            "model": Model.from_dict(obj["model"]) if obj.get("model") is not None else None,
+            "pitch": obj.get("pitch") if obj.get("pitch") is not None else 0,
+            "rate": obj.get("rate") if obj.get("rate") is not None else 0
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/ended_reasons.py` & `voiceos-0.8.1.3/voiceos/models/ended_reasons.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,17 +22,16 @@
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    HUMAN_HANGUP = 'human_hangup'
-    AGENT_HANGUP = 'agent_hangup'
-    NO_ANSWER = 'no_answer'
+    AGENT_ENDED = 'agent_ended'
+    USER_ENDED = 'user_ended'
     UNKNOWN = 'unknown'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of EndedReasons from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/event.py` & `voiceos-0.8.1.3/voiceos/models/voice_id.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Optional
-from voiceos.models.event_name import EventName
-from voiceos.models.event_variable_name import EventVariableName
+from voiceos.models.eleven_labs_voices import ElevenLabsVoices
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-EVENT_ANY_OF_SCHEMAS = ["EventName", "EventVariableName"]
+VOICEID_ANY_OF_SCHEMAS = ["ElevenLabsVoices", "str"]
 
-class Event(BaseModel):
+class VoiceId(BaseModel):
     """
-    The event that triggers the webhook
+    The elevenlabs model to use.
     """
 
-    # data type: EventVariableName
-    anyof_schema_1_validator: Optional[EventVariableName] = None
-    # data type: EventName
-    anyof_schema_2_validator: Optional[EventName] = None
+    # data type: ElevenLabsVoices
+    anyof_schema_1_validator: Optional[ElevenLabsVoices] = None
+    # data type: str
+    anyof_schema_2_validator: Optional[StrictStr] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[EventName, EventVariableName]] = None
+        actual_instance: Optional[Union[ElevenLabsVoices, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["EventName", "EventVariableName"])
+    any_of_schemas: List[str] = Field(default=Literal["ElevenLabsVoices", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -55,73 +54,76 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Event.model_construct()
+        instance = VoiceId.model_construct()
         error_messages = []
-        # validate data type: EventVariableName
-        if not isinstance(v, EventVariableName):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `EventVariableName`")
+        # validate data type: ElevenLabsVoices
+        if not isinstance(v, ElevenLabsVoices):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ElevenLabsVoices`")
         else:
             return v
 
-        # validate data type: EventName
-        if not isinstance(v, EventName):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `EventName`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Event with anyOf schemas: EventName, EventVariableName. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in VoiceId with anyOf schemas: ElevenLabsVoices, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[EventVariableName] = None
+        # anyof_schema_1_validator: Optional[ElevenLabsVoices] = None
         try:
-            instance.actual_instance = EventVariableName.from_json(json_str)
+            instance.actual_instance = ElevenLabsVoices.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[EventName] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = EventName.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Event with anyOf schemas: EventName, EventVariableName. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into VoiceId with anyOf schemas: ElevenLabsVoices, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], EventName, EventVariableName]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], ElevenLabsVoices, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `voiceos-0.8.1.2/voiceos/models/event_name.py` & `voiceos-0.8.1.3/voiceos/models/wako_api_models_synthesizer_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class EventName(str, Enum):
+class WakoApiModelsSynthesizerProvider(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    OPENAI_FUNCTION_CALL_TRIGGERED = 'openai_function_call_triggered'
-    CALL_STARTED = 'call_started'
-    MESSAGE = 'message'
-    CALL_ENDED = 'call_ended'
+    AZURE = 'azure'
+    ELEVENLABS = 'elevenlabs'
+    RIME = 'rime'
+    DEEPGRAM = 'deepgram'
+    PLAYHT = 'playht'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of EventName from a JSON string"""
+        """Create an instance of WakoApiModelsSynthesizerProvider from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/event_variable_name.py` & `voiceos-0.8.1.3/voiceos/models/eleven_labs_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class EventVariableName(str, Enum):
+class ElevenLabsModel(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    CALL_DURATION = 'call_duration'
-    SILENCE_DURATION = 'silence_duration'
+    ELEVEN_MULTILINGUAL_V2 = 'eleven_multilingual_v2'
+    ELEVEN_MONOLINGUAL_V1 = 'eleven_monolingual_v1'
+    ELEVEN_TURBO_V2 = 'eleven_turbo_v2'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of EventVariableName from a JSON string"""
+        """Create an instance of ElevenLabsModel from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/http_validation_error.py` & `voiceos-0.8.1.3/voiceos/models/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/language_model_cost.py` & `voiceos-0.8.1.3/voiceos/models/language_model_cost.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Union
 from voiceos.models.wako_api_models_language_model_provider import WakoApiModelsLanguageModelProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
 class LanguageModelCost(BaseModel):
     """
     LanguageModelCost
     """ # noqa: E501
     provider: WakoApiModelsLanguageModelProvider = Field(description="The provider of the language model.")
-    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the language model usage. Returns zero, if the provider account you provided was used.")
+    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the language model usage (USD).")
     input_tokens: StrictInt = Field(description="The number of input tokens used for the language model.")
     output_tokens: StrictInt = Field(description="The number of output tokens used for the language model.")
-    external: StrictBool = Field(description="Whether the provider account you provided was used. If true, the cost will be zero.")
-    __properties: ClassVar[List[str]] = ["provider", "cost", "input_tokens", "output_tokens", "external"]
+    __properties: ClassVar[List[str]] = ["provider", "cost", "input_tokens", "output_tokens"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -84,13 +83,12 @@
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider"),
             "cost": obj.get("cost"),
             "input_tokens": obj.get("input_tokens"),
-            "output_tokens": obj.get("output_tokens"),
-            "external": obj.get("external")
+            "output_tokens": obj.get("output_tokens")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/message.py` & `voiceos-0.8.1.3/voiceos/models/voice_cost.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
-from voiceos.models.message_role import MessageRole
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
+from typing import Any, ClassVar, Dict, List, Union
+from voiceos.models.wako_api_models_synthesizer_provider import WakoApiModelsSynthesizerProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Message(BaseModel):
+class VoiceCost(BaseModel):
     """
-    Message
+    VoiceCost
     """ # noqa: E501
-    role: MessageRole = Field(description="The role of the message.")
-    content: StrictStr = Field(description="The content of the message.")
-    __properties: ClassVar[List[str]] = ["role", "content"]
+    provider: WakoApiModelsSynthesizerProvider = Field(description="The provider of the synthetizer.")
+    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the voice usage (USD).")
+    characters: StrictInt = Field(description="The number of characters used for the voice.")
+    __properties: ClassVar[List[str]] = ["provider", "cost", "characters"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Message from a JSON string"""
+        """Create an instance of VoiceCost from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +71,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Message from a dict"""
+        """Create an instance of VoiceCost from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "role": obj.get("role"),
-            "content": obj.get("content")
+            "provider": obj.get("provider"),
+            "cost": obj.get("cost"),
+            "characters": obj.get("characters")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/message_role.py` & `voiceos-0.8.1.3/voiceos/models/conversation_status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class MessageRole(str, Enum):
+class ConversationStatus(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    AGENT = 'agent'
-    HUMAN = 'human'
+    STARTED = 'started'
+    ENDED = 'ended'
+    QUEUED = 'queued'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of MessageRole from a JSON string"""
+        """Create an instance of ConversationStatus from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/method_enum.py` & `voiceos-0.8.1.3/voiceos/models/method_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/open_ai.py` & `voiceos-0.8.1.3/voiceos/models/deepgram_voice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.chat_gpt import ChatGPT
-from voiceos.models.open_ai_function import OpenAIFunction
+from voiceos.models.model2 import Model2
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OpenAI(BaseModel):
+class DeepgramVoice(BaseModel):
     """
-    OpenAI
+    DeepgramVoice
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='openai', description="The lnaguage model provider.")
-    model: Optional[ChatGPT] = Field(default=None, description="The OpenAI Chat GPT model to use")
-    functions: Optional[List[OpenAIFunction]] = Field(default=None, description="The list of OpenAI function calls.")
-    __properties: ClassVar[List[str]] = ["provider", "model", "functions"]
+    provider: Optional[StrictStr] = Field(default='deepgram', description="The synthesizer provider.")
+    model: Optional[Model2] = None
+    __properties: ClassVar[List[str]] = ["provider", "model"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['openai']):
-            raise ValueError("must be one of enum values ('openai')")
+        if value not in set(['deepgram']):
+            raise ValueError("must be one of enum values ('deepgram')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -57,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OpenAI from a JSON string"""
+        """Create an instance of DeepgramVoice from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,33 +76,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in functions (list)
-        _items = []
-        if self.functions:
-            for _item in self.functions:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['functions'] = _items
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OpenAI from a dict"""
+        """Create an instance of DeepgramVoice from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider") if obj.get("provider") is not None else 'openai',
-            "model": obj.get("model"),
-            "functions": [OpenAIFunction.from_dict(_item) for _item in obj["functions"]] if obj.get("functions") is not None else None
+            "provider": obj.get("provider") if obj.get("provider") is not None else 'deepgram',
+            "model": Model2.from_dict(obj["model"]) if obj.get("model") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/open_ai_function.py` & `voiceos-0.8.1.3/voiceos/models/phone_number_webhook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.open_ai_function_parameter import OpenAIFunctionParameter
+from voiceos.models.method_enum import MethodEnum
+from voiceos.models.phone_number_events import PhoneNumberEvents
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OpenAIFunction(BaseModel):
+class PhoneNumberWebhook(BaseModel):
     """
-    OpenAIFunction
+    PhoneNumberWebhook
     """ # noqa: E501
-    name: StrictStr = Field(description="This is the name of the function to be called. Must be less than 64 characters (a-z, A-Z, 0-9, including underscores).")
-    wait: Optional[StrictBool] = Field(default=False, description="If true, the agent will wait for the function to return before continuing.")
-    description: StrictStr = Field(description="The description of the OpenAI function call.")
-    parameters: OpenAIFunctionParameter = Field(description="The parameters of the OpenAI function call.")
-    __properties: ClassVar[List[str]] = ["name", "wait", "description", "parameters"]
+    events: List[PhoneNumberEvents] = Field(description="The events that will trigger the webhook to send a request.")
+    url: StrictStr = Field(description="The url of the webhook. Where the requests will be sent.")
+    method: MethodEnum = Field(description="The method of the webhook.")
+    headers: Optional[Dict[str, StrictStr]] = Field(default=None, description="The headers of the webhook. Use the headers to authenticate requests to your backend.")
+    filter: Optional[StrictStr] = Field(default=None, description="The filter for the webhook events. Use to filter events with conditional statements.")
+    __properties: ClassVar[List[str]] = ["events", "url", "method", "headers", "filter"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OpenAIFunction from a JSON string"""
+        """Create an instance of PhoneNumberWebhook from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,30 +70,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of parameters
-        if self.parameters:
-            _dict['parameters'] = self.parameters.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OpenAIFunction from a dict"""
+        """Create an instance of PhoneNumberWebhook from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "wait": obj.get("wait") if obj.get("wait") is not None else False,
-            "description": obj.get("description"),
-            "parameters": OpenAIFunctionParameter.from_dict(obj["parameters"]) if obj.get("parameters") is not None else None
+            "events": obj.get("events"),
+            "url": obj.get("url"),
+            "method": obj.get("method"),
+            "filter": obj.get("filter")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/open_ai_function_parameter.py` & `voiceos-0.8.1.3/voiceos/models/create_call.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.open_ai_function_type import OpenAIFunctionType
+from voiceos.models.agent_configuration import AgentConfiguration
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OpenAIFunctionParameter(BaseModel):
+class CreateCall(BaseModel):
     """
-    OpenAIFunctionParameter
+    CreateCall
     """ # noqa: E501
-    type: Optional[OpenAIFunctionType] = Field(default=None, description="This must be set to 'object'. It instructs the model to return a JSON object containing the function call properties.")
-    properties: Dict[str, Any] = Field(description="This provides a description of the properties required by the function.")
-    required: Optional[List[StrictStr]] = Field(default=None, description="This specifies the properties that are required by the function.")
-    __properties: ClassVar[List[str]] = ["type", "properties", "required"]
+    from_number: StrictStr = Field(description="The phone number associated with the account from which the call will be made.")
+    to_number: StrictStr = Field(description="The phone number to call including the country code.")
+    agent_id: Optional[StrictStr] = Field(default=None, description="The agent id to use for the conversation. If null, the agent configuration will be used.")
+    agent_config: Optional[AgentConfiguration] = Field(default=None, description="The agent configuration to use for the conversation. If null, the agent id will be used.")
+    __properties: ClassVar[List[str]] = ["from_number", "to_number", "agent_id", "agent_config"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OpenAIFunctionParameter from a JSON string"""
+        """Create an instance of CreateCall from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,26 +68,30 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of agent_config
+        if self.agent_config:
+            _dict['agent_config'] = self.agent_config.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OpenAIFunctionParameter from a dict"""
+        """Create an instance of CreateCall from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "properties": obj.get("properties"),
-            "required": obj.get("required")
+            "from_number": obj.get("from_number"),
+            "to_number": obj.get("to_number"),
+            "agent_id": obj.get("agent_id"),
+            "agent_config": AgentConfiguration.from_dict(obj["agent_config"]) if obj.get("agent_config") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/open_ai_function_type.py` & `voiceos-0.8.1.3/voiceos/models/play_ht_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class OpenAIFunctionType(str, Enum):
+class PlayHTModel(str, Enum):
     """
     An enumeration.
     """
 
     """
     allowed enum values
     """
-    OBJECT = 'object'
+    SUSAN = 'susan'
+    WILLIAM = 'william'
+    PHOEBE = 'phoebe'
+    ARTHUR = 'arthur'
+    AYLA = 'ayla'
+    DYLAN = 'dylan'
+    MADELYN = 'madelyn'
+    OLIVER = 'oliver'
+    SOPHIA = 'sophia'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of OpenAIFunctionType from a JSON string"""
+        """Create an instance of PlayHTModel from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `voiceos-0.8.1.2/voiceos/models/phone_number.py` & `voiceos-0.8.1.3/voiceos/models/phone_number.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
 from voiceos.models.twilio_telephony import TwilioTelephony
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PhoneNumber(BaseModel):
     """
     PhoneNumber
     """ # noqa: E501
     uri: StrictStr = Field(description="The uri of the phone number.")
-    inbound_agent_uri: Optional[StrictStr] = Field(default=None, description="The agent uri that will be used for inbound calls. If null, the phone number is will not receive any calls.")
-    phone_number: StrictStr = Field(description="The phone number.")
+    inbound_agent_id: Optional[StrictStr] = Field(default=None, description="The agent id that will be used for inbound calls. If null, the phone number will not receive any calls.")
+    phone_number: StrictStr = Field(description="The phone number including the country code.")
     account_id: StrictStr = Field(description="The account id associated with the phone number.")
     created_at: datetime = Field(description="The date the phone number was created.")
     updated_at: datetime = Field(description="The date the phone number was last updated.")
-    telephony: TwilioTelephony = Field(description="The telephony of the phone number.")
-    stripe_subscription_id: Optional[StrictStr] = Field(default=None, description="The stripe subscription id of the phone number. Returns null if the phone number was imported.")
-    __properties: ClassVar[List[str]] = ["uri", "inbound_agent_uri", "phone_number", "account_id", "created_at", "updated_at", "telephony", "stripe_subscription_id"]
+    telephony: TwilioTelephony = Field(description="The telephony provider for the phone number.")
+    webhooks: Optional[List[PhoneNumberWebhook]] = Field(default=None, description="The webhooks of the phone number. This is used to fetch the agent at the start of the conversation.")
+    __properties: ClassVar[List[str]] = ["uri", "inbound_agent_id", "phone_number", "account_id", "created_at", "updated_at", "telephony", "webhooks"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -76,31 +77,38 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of telephony
         if self.telephony:
             _dict['telephony'] = self.telephony.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
+        _items = []
+        if self.webhooks:
+            for _item in self.webhooks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['webhooks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of PhoneNumber from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "uri": obj.get("uri"),
-            "inbound_agent_uri": obj.get("inbound_agent_uri"),
+            "inbound_agent_id": obj.get("inbound_agent_id"),
             "phone_number": obj.get("phone_number"),
             "account_id": obj.get("account_id"),
             "created_at": obj.get("created_at"),
             "updated_at": obj.get("updated_at"),
             "telephony": TwilioTelephony.from_dict(obj["telephony"]) if obj.get("telephony") is not None else None,
-            "stripe_subscription_id": obj.get("stripe_subscription_id")
+            "webhooks": [PhoneNumberWebhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/phone_number_pagination.py` & `voiceos-0.8.1.3/voiceos/models/phone_number_pagination.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -25,16 +25,16 @@
 
 class PhoneNumberPagination(BaseModel):
     """
     PhoneNumberPagination
     """ # noqa: E501
     items: List[PhoneNumberResponse] = Field(description="The list of phone numbers returned.")
     index: StrictInt = Field(description="The current index of the page.")
-    has_next: StrictBool = Field(description="Whether there is a next page.")
-    __properties: ClassVar[List[str]] = ["items", "index", "has_next"]
+    has_more: StrictBool = Field(description="Whether there is a next page.")
+    __properties: ClassVar[List[str]] = ["items", "index", "has_more"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -88,12 +88,12 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "items": [PhoneNumberResponse.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None,
             "index": obj.get("index"),
-            "has_next": obj.get("has_next")
+            "has_more": obj.get("has_more")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/phone_number_response.py` & `voiceos-0.8.1.3/voiceos/models/phone_number_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from voiceos.models.phone_number_webhook import PhoneNumberWebhook
 from voiceos.models.twilio_telephony import TwilioTelephony
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PhoneNumberResponse(BaseModel):
     """
     PhoneNumberResponse
     """ # noqa: E501
     uri: StrictStr = Field(description="The uri of the phone number.")
-    inbound_agent_uri: Optional[StrictStr] = Field(default=None, description="The agent uri that will be used for inbound calls. If null, the phone number is will not receive any calls.")
-    phone_number: StrictStr = Field(description="The phone number.")
+    inbound_agent_id: Optional[StrictStr] = Field(default=None, description="The agent id that will be used for inbound calls. If null, the phone number will not receive any calls.")
+    phone_number: StrictStr = Field(description="The phone number including the country code.")
     account_id: StrictStr = Field(description="The account id associated with the phone number.")
     created_at: datetime = Field(description="The date the phone number was created.")
     updated_at: datetime = Field(description="The date the phone number was last updated.")
-    telephony: TwilioTelephony = Field(description="The telephony of the phone number.")
-    stripe_subscription_id: Optional[StrictStr] = Field(default=None, description="The stripe subscription id of the phone number. Returns null if the phone number was imported.")
+    telephony: TwilioTelephony = Field(description="The telephony provider for the phone number.")
+    webhooks: Optional[List[PhoneNumberWebhook]] = Field(default=None, description="The webhooks of the phone number. This is used to fetch the agent at the start of the conversation.")
     id: StrictStr = Field(description="The id of the phone number.")
-    __properties: ClassVar[List[str]] = ["uri", "inbound_agent_uri", "phone_number", "account_id", "created_at", "updated_at", "telephony", "stripe_subscription_id", "id"]
+    __properties: ClassVar[List[str]] = ["uri", "inbound_agent_id", "phone_number", "account_id", "created_at", "updated_at", "telephony", "webhooks", "id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -77,32 +78,39 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of telephony
         if self.telephony:
             _dict['telephony'] = self.telephony.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
+        _items = []
+        if self.webhooks:
+            for _item in self.webhooks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['webhooks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of PhoneNumberResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "uri": obj.get("uri"),
-            "inbound_agent_uri": obj.get("inbound_agent_uri"),
+            "inbound_agent_id": obj.get("inbound_agent_id"),
             "phone_number": obj.get("phone_number"),
             "account_id": obj.get("account_id"),
             "created_at": obj.get("created_at"),
             "updated_at": obj.get("updated_at"),
             "telephony": TwilioTelephony.from_dict(obj["telephony"]) if obj.get("telephony") is not None else None,
-            "stripe_subscription_id": obj.get("stripe_subscription_id"),
+            "webhooks": [PhoneNumberWebhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None,
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/phone_number_to_buy.py` & `voiceos-0.8.1.3/voiceos/models/phone_number_to_buy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PhoneNumberToBuy(BaseModel):
     """
     PhoneNumberToBuy
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='twilio', description="The telephony provider.")
-    phone_number: StrictStr = Field(description="The phone number.")
+    provider: WakoApiModelsPhoneNumberProvider = Field(description="The telephony provider.")
+    phone_number: StrictStr = Field(description="The available phone number to buy.")
     postal_code: Optional[StrictStr] = Field(default=None, description="The postal code of the phone number.")
     iso_country: Optional[StrictStr] = Field(default=None, description="The iso country code of the phone number.")
     __properties: ClassVar[List[str]] = ["provider", "phone_number", "postal_code", "iso_country"]
 
-    @field_validator('provider')
-    def provider_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['twilio']):
-            raise ValueError("must be one of enum values ('twilio')")
-        return value
-
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -89,15 +80,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider") if obj.get("provider") is not None else 'twilio',
+            "provider": obj.get("provider"),
             "phone_number": obj.get("phone_number"),
             "postal_code": obj.get("postal_code"),
             "iso_country": obj.get("iso_country")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/rime_synthesizer.py` & `voiceos-0.8.1.3/voiceos/models/rime_voice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing_extensions import Annotated
+from voiceos.models.speaker import Speaker
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RimeSynthesizer(BaseModel):
+class RimeVoice(BaseModel):
     """
-    RimeSynthesizer
+    RimeVoice
     """ # noqa: E501
-    provider: Optional[StrictStr] = Field(default='rime', description="The synthesizer provider.")
-    speaker: Optional[StrictStr] = Field(default='abbie', description="The speaker of the voice.")
-    reduce_lantency: Optional[StrictBool] = Field(default=False, description="Reduces the latency of response, at the cost of some possible mispronunciation of digits and abbreviations.")
-    speed_alpha: Optional[Union[Annotated[float, Field(le=2.0, strict=True, ge=0.5)], Annotated[int, Field(le=2, strict=True, ge=1)]]] = Field(default=1.0, description="Adjusts the speed of speech. Lower is faster. Higher is slower.")
-    __properties: ClassVar[List[str]] = ["provider", "speaker", "reduce_lantency", "speed_alpha"]
+    provider: Optional[StrictStr] = Field(default='rime', description="The voice provider.")
+    speaker: Optional[Speaker] = None
+    speed_alpha: Optional[Union[Annotated[float, Field(le=2.0, strict=True, ge=0.5)], Annotated[int, Field(le=2, strict=True, ge=1)]]] = Field(default=1.0, description="Adjusts the speed of speech. Lower than 1.0 is faster than default. Higher than 1.0 is slower than default.")
+    reduce_latency: Optional[StrictBool] = Field(default=False, description="Reduces the latency of response, at the cost of some possible mispronunciation of digits and abbreviations.")
+    __properties: ClassVar[List[str]] = ["provider", "speaker", "speed_alpha", "reduce_latency"]
 
     @field_validator('provider')
     def provider_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -57,15 +58,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RimeSynthesizer from a JSON string"""
+        """Create an instance of RimeVoice from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,27 +79,30 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of speaker
+        if self.speaker:
+            _dict['speaker'] = self.speaker.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RimeSynthesizer from a dict"""
+        """Create an instance of RimeVoice from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider") if obj.get("provider") is not None else 'rime',
-            "speaker": obj.get("speaker") if obj.get("speaker") is not None else 'abbie',
-            "reduce_lantency": obj.get("reduce_lantency") if obj.get("reduce_lantency") is not None else False,
-            "speed_alpha": obj.get("speed_alpha") if obj.get("speed_alpha") is not None else 1.0
+            "speaker": Speaker.from_dict(obj["speaker"]) if obj.get("speaker") is not None else None,
+            "speed_alpha": obj.get("speed_alpha") if obj.get("speed_alpha") is not None else 1.0,
+            "reduce_latency": obj.get("reduce_latency") if obj.get("reduce_latency") is not None else False
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/synthesizer_cost.py` & `voiceos-0.8.1.3/voiceos/models/telephony_cost.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Union
-from voiceos.models.wako_api_models_synthesizer_provider import WakoApiModelsSynthesizerProvider
+from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SynthesizerCost(BaseModel):
+class TelephonyCost(BaseModel):
     """
-    SynthesizerCost
+    TelephonyCost
     """ # noqa: E501
-    provider: WakoApiModelsSynthesizerProvider = Field(description="The provider of the synthetizer.")
-    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the synthetizer usage. Returns zero, if the provider account you provided was used.")
-    characters: StrictInt = Field(description="The number of characters used for the synthetizer.")
-    external: StrictBool = Field(description="Whether the provider account you provided was used. If true, the cost will be zero.")
-    __properties: ClassVar[List[str]] = ["provider", "cost", "characters", "external"]
+    provider: WakoApiModelsPhoneNumberProvider = Field(description="The provider of the phone number used.")
+    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the telephony usage. Returns zero, if the phone number was imported.")
+    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of seconds used for the telephony.")
+    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SynthesizerCost from a JSON string"""
+        """Create an instance of TelephonyCost from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,23 +71,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SynthesizerCost from a dict"""
+        """Create an instance of TelephonyCost from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider"),
             "cost": obj.get("cost"),
-            "characters": obj.get("characters"),
-            "external": obj.get("external")
+            "seconds": obj.get("seconds")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/telephony_cost.py` & `voiceos-0.8.1.3/voiceos/models/twilio_telephony.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TelephonyCost(BaseModel):
+class TwilioTelephony(BaseModel):
     """
-    TelephonyCost
+    TwilioTelephony
     """ # noqa: E501
-    provider: WakoApiModelsPhoneNumberProvider = Field(description="The provider of the phone number used.")
-    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the telephony usage. Returns zero, if the phone number was imported.")
-    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of minutes used for the telephony.")
-    external: StrictBool = Field(description="Whether the phone number was imported. If true, the cost will be zero.")
-    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds", "external"]
+    provider: WakoApiModelsPhoneNumberProvider = Field(description="The telephony provider.")
+    phone_number_sid: StrictStr = Field(description="The twilio phone number SID.")
+    account_sid: Optional[StrictStr] = Field(default=None, description="The account sid of the telephony provider (i.e Twilio Account SID). Returns null if the phone number was purchased with VoiceOS.")
+    auth_token: Optional[StrictStr] = Field(default=None, description="The auth token of the telephony provider (i.e Twilio Auth Token). Returns null if the phone number was purchased with VoiceOS.")
+    __properties: ClassVar[List[str]] = ["provider", "phone_number_sid", "account_sid", "auth_token"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TelephonyCost from a JSON string"""
+        """Create an instance of TwilioTelephony from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,23 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TelephonyCost from a dict"""
+        """Create an instance of TwilioTelephony from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider"),
-            "cost": obj.get("cost"),
-            "seconds": obj.get("seconds"),
-            "external": obj.get("external")
+            "phone_number_sid": obj.get("phone_number_sid"),
+            "account_sid": obj.get("account_sid"),
+            "auth_token": obj.get("auth_token")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/transcriber.py` & `voiceos-0.8.1.3/voiceos/models/transcriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/transcriber1.py` & `voiceos-0.8.1.3/voiceos/models/transcriber1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/transcriber_cost.py` & `voiceos-0.8.1.3/voiceos/models/transcriber_cost.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Union
 from voiceos.models.wako_api_models_transcriber_provider import WakoApiModelsTranscriberProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
 class TranscriberCost(BaseModel):
     """
     TranscriberCost
     """ # noqa: E501
     provider: WakoApiModelsTranscriberProvider = Field(description="The provider of the transcriber.")
-    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the synthetizer usage. Returns zero, if the provider account you provided was used.")
-    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of minutes used for the transcriber.")
-    external: StrictBool = Field(description="Whether the provider account you provided was used. If true, the cost will be zero.")
-    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds", "external"]
+    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the transcriber usage (USD).")
+    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of seconds used for the transcriber.")
+    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -82,13 +81,12 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "provider": obj.get("provider"),
             "cost": obj.get("cost"),
-            "seconds": obj.get("seconds"),
-            "external": obj.get("external")
+            "seconds": obj.get("seconds")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/update_agent.py` & `voiceos-0.8.1.3/voiceos/models/update_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.agent_language import AgentLanguage
 from voiceos.models.open_ai import OpenAI
 from voiceos.models.transcriber1 import Transcriber1
 from voiceos.models.voice1 import Voice1
 from voiceos.models.webhook import Webhook
 from typing import Optional, Set
 from typing_extensions import Self
 
 class UpdateAgent(BaseModel):
     """
     UpdateAgent
     """ # noqa: E501
-    name: Optional[StrictStr] = Field(default=None, description="The name of the agent")
-    initial_message: Optional[StrictStr] = Field(default=None, description="The initial message of the agent")
-    prompt: Optional[StrictStr] = Field(default=None, description="The prompt preamble of the agent")
-    language: Optional[AgentLanguage] = Field(default=None, description="The language of the agent")
-    language_model: Optional[OpenAI] = Field(default=None, description="The language model of the agent.")
+    initial_message: Optional[StrictStr] = Field(default=None, description="The initial message that the agent will say. If null, the agent will wait for the user to speak first.")
+    prompt: Optional[StrictStr] = Field(default=None, description="The prompt of the agent.")
     voice: Optional[Voice1] = None
+    language_model: Optional[OpenAI] = Field(default=None, description="The language model of the agent.")
     transcriber: Optional[Transcriber1] = None
-    max_duration_time: Optional[StrictInt] = Field(default=600, description="The maximum call duration in seconds. If null, the call can be of any duration. The default value is 10 min.")
-    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent")
-    __properties: ClassVar[List[str]] = ["name", "initial_message", "prompt", "language", "language_model", "voice", "transcriber", "max_duration_time", "webhooks"]
+    max_duration_seconds: Optional[StrictInt] = Field(default=600, description="The maximum conversation duration in seconds. If null, the conversation can be of any duration. The default value is 10 min.")
+    webhooks: Optional[List[Webhook]] = Field(default=None, description="The webhooks of the agent. These are used for real-time conversation events such as function_calls, messages and much more.")
+    metadata: Optional[Dict[str, StrictStr]] = Field(default=None, description="The metadata of the agent. This is used to store additional information about the agent.")
+    __properties: ClassVar[List[str]] = ["initial_message", "prompt", "voice", "language_model", "transcriber", "max_duration_seconds", "webhooks", "metadata"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -77,20 +75,20 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of language_model
-        if self.language_model:
-            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of voice
         if self.voice:
             _dict['voice'] = self.voice.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of language_model
+        if self.language_model:
+            _dict['language_model'] = self.language_model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of transcriber
         if self.transcriber:
             _dict['transcriber'] = self.transcriber.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in webhooks (list)
         _items = []
         if self.webhooks:
             for _item in self.webhooks:
@@ -105,20 +103,18 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
             "initial_message": obj.get("initial_message"),
             "prompt": obj.get("prompt"),
-            "language": obj.get("language"),
-            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "voice": Voice1.from_dict(obj["voice"]) if obj.get("voice") is not None else None,
+            "language_model": OpenAI.from_dict(obj["language_model"]) if obj.get("language_model") is not None else None,
             "transcriber": Transcriber1.from_dict(obj["transcriber"]) if obj.get("transcriber") is not None else None,
-            "max_duration_time": obj.get("max_duration_time") if obj.get("max_duration_time") is not None else 600,
-            "webhooks": [Webhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None
+            "max_duration_seconds": obj.get("max_duration_seconds") if obj.get("max_duration_seconds") is not None else 600,
+            "webhooks": [Webhook.from_dict(_item) for _item in obj["webhooks"]] if obj.get("webhooks") is not None else None,
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/update_phone_number.py` & `voiceos-0.8.1.3/voiceos/models/webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from voiceos.models.event_name import EventName
+from voiceos.models.method_enum import MethodEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UpdatePhoneNumber(BaseModel):
+class Webhook(BaseModel):
     """
-    UpdatePhoneNumber
+    Webhook
     """ # noqa: E501
-    inbound_agent_uri: Optional[StrictStr] = Field(default=None, description="The agent uri that will be used for inbound calls. If null, the phone number is will not receive any calls.")
-    __properties: ClassVar[List[str]] = ["inbound_agent_uri"]
+    events: List[EventName] = Field(description="The events that will trigger the webhook to send a request.")
+    url: StrictStr = Field(description="The url of the webhook. Where the requests will be sent.")
+    method: MethodEnum = Field(description="The method of the webhook.")
+    headers: Optional[Dict[str, StrictStr]] = Field(default=None, description="The headers of the webhook. Use the headers to authenticate requests to your backend.")
+    filter: Optional[StrictStr] = Field(default=None, description="The filter for the webhook events. Use to filter events with conditional statements.")
+    __properties: ClassVar[List[str]] = ["events", "url", "method", "headers", "filter"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -43,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UpdatePhoneNumber from a JSON string"""
+        """Create an instance of Webhook from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +74,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UpdatePhoneNumber from a dict"""
+        """Create an instance of Webhook from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "inbound_agent_uri": obj.get("inbound_agent_uri")
+            "events": obj.get("events"),
+            "url": obj.get("url"),
+            "method": obj.get("method"),
+            "filter": obj.get("filter")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/validation_error.py` & `voiceos-0.8.1.3/voiceos/models/agent_cost.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
-from voiceos.models.validation_error_loc_inner import ValidationErrorLocInner
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
+from typing import Any, ClassVar, Dict, List, Union
+from voiceos.models.agent_provider import AgentProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ValidationError(BaseModel):
+class AgentCost(BaseModel):
     """
-    ValidationError
+    AgentCost
     """ # noqa: E501
-    loc: List[ValidationErrorLocInner]
-    msg: StrictStr
-    type: StrictStr
-    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
+    provider: AgentProvider = Field(description="The provider of the agent (i.e VoiceOS).")
+    cost: Union[StrictFloat, StrictInt] = Field(description="The cost for the agent usage (USD).")
+    seconds: Union[StrictFloat, StrictInt] = Field(description="The number of seconds used for the agent orchestration.")
+    __properties: ClassVar[List[str]] = ["provider", "cost", "seconds"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ValidationError from a JSON string"""
+        """Create an instance of AgentCost from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,33 +67,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
-        _items = []
-        if self.loc:
-            for _item in self.loc:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ValidationError from a dict"""
+        """Create an instance of AgentCost from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
-            "msg": obj.get("msg"),
-            "type": obj.get("type")
+            "provider": obj.get("provider"),
+            "cost": obj.get("cost"),
+            "seconds": obj.get("seconds")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/models/validation_error_loc_inner.py` & `voiceos-0.8.1.3/voiceos/models/validation_error_loc_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `voiceos-0.8.1.2/voiceos/models/voice.py` & `voiceos-0.8.1.3/voiceos/models/model2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Optional
-from voiceos.models.azure_synthesizer import AzureSynthesizer
-from voiceos.models.eleven_labs_synthesizer import ElevenLabsSynthesizer
-from voiceos.models.rime_synthesizer import RimeSynthesizer
+from voiceos.models.wako_api_models_synthesizer_deepgram_model import WakoApiModelsSynthesizerDeepgramModel
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-VOICE_ANY_OF_SCHEMAS = ["AzureSynthesizer", "ElevenLabsSynthesizer", "RimeSynthesizer"]
+MODEL2_ANY_OF_SCHEMAS = ["WakoApiModelsSynthesizerDeepgramModel", "str"]
 
-class Voice(BaseModel):
+class Model2(BaseModel):
     """
-    Voice
+    The deepgram model to use.
     """
 
-    # data type: ElevenLabsSynthesizer
-    anyof_schema_1_validator: Optional[ElevenLabsSynthesizer] = None
-    # data type: AzureSynthesizer
-    anyof_schema_2_validator: Optional[AzureSynthesizer] = None
-    # data type: RimeSynthesizer
-    anyof_schema_3_validator: Optional[RimeSynthesizer] = None
+    # data type: WakoApiModelsSynthesizerDeepgramModel
+    anyof_schema_1_validator: Optional[WakoApiModelsSynthesizerDeepgramModel] = None
+    # data type: str
+    anyof_schema_2_validator: Optional[StrictStr] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer]] = None
+        actual_instance: Optional[Union[WakoApiModelsSynthesizerDeepgramModel, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["AzureSynthesizer", "ElevenLabsSynthesizer", "RimeSynthesizer"])
+    any_of_schemas: List[str] = Field(default=Literal["WakoApiModelsSynthesizerDeepgramModel", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -58,85 +54,76 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Voice.model_construct()
+        instance = Model2.model_construct()
         error_messages = []
-        # validate data type: ElevenLabsSynthesizer
-        if not isinstance(v, ElevenLabsSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `ElevenLabsSynthesizer`")
+        # validate data type: WakoApiModelsSynthesizerDeepgramModel
+        if not isinstance(v, WakoApiModelsSynthesizerDeepgramModel):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `WakoApiModelsSynthesizerDeepgramModel`")
         else:
             return v
 
-        # validate data type: AzureSynthesizer
-        if not isinstance(v, AzureSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AzureSynthesizer`")
-        else:
-            return v
-
-        # validate data type: RimeSynthesizer
-        if not isinstance(v, RimeSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `RimeSynthesizer`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Voice with anyOf schemas: AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Model2 with anyOf schemas: WakoApiModelsSynthesizerDeepgramModel, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[ElevenLabsSynthesizer] = None
-        try:
-            instance.actual_instance = ElevenLabsSynthesizer.from_json(json_str)
-            return instance
-        except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[AzureSynthesizer] = None
+        # anyof_schema_1_validator: Optional[WakoApiModelsSynthesizerDeepgramModel] = None
         try:
-            instance.actual_instance = AzureSynthesizer.from_json(json_str)
+            instance.actual_instance = WakoApiModelsSynthesizerDeepgramModel.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
-        # anyof_schema_3_validator: Optional[RimeSynthesizer] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = RimeSynthesizer.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Voice with anyOf schemas: AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Model2 with anyOf schemas: WakoApiModelsSynthesizerDeepgramModel, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], WakoApiModelsSynthesizerDeepgramModel, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `voiceos-0.8.1.2/voiceos/models/voice1.py` & `voiceos-0.8.1.3/voiceos/models/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Optional
-from voiceos.models.azure_synthesizer import AzureSynthesizer
-from voiceos.models.eleven_labs_synthesizer import ElevenLabsSynthesizer
-from voiceos.models.rime_synthesizer import RimeSynthesizer
+from voiceos.models.azure_model import AzureModel
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-VOICE1_ANY_OF_SCHEMAS = ["AzureSynthesizer", "ElevenLabsSynthesizer", "RimeSynthesizer"]
+MODEL_ANY_OF_SCHEMAS = ["AzureModel", "str"]
 
-class Voice1(BaseModel):
+class Model(BaseModel):
     """
-    The synthesizer of the agent.
+    The azure model to use.
     """
 
-    # data type: ElevenLabsSynthesizer
-    anyof_schema_1_validator: Optional[ElevenLabsSynthesizer] = None
-    # data type: AzureSynthesizer
-    anyof_schema_2_validator: Optional[AzureSynthesizer] = None
-    # data type: RimeSynthesizer
-    anyof_schema_3_validator: Optional[RimeSynthesizer] = None
+    # data type: AzureModel
+    anyof_schema_1_validator: Optional[AzureModel] = None
+    # data type: str
+    anyof_schema_2_validator: Optional[StrictStr] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer]] = None
+        actual_instance: Optional[Union[AzureModel, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["AzureSynthesizer", "ElevenLabsSynthesizer", "RimeSynthesizer"])
+    any_of_schemas: List[str] = Field(default=Literal["AzureModel", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -58,85 +54,76 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Voice1.model_construct()
+        instance = Model.model_construct()
         error_messages = []
-        # validate data type: ElevenLabsSynthesizer
-        if not isinstance(v, ElevenLabsSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `ElevenLabsSynthesizer`")
+        # validate data type: AzureModel
+        if not isinstance(v, AzureModel):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AzureModel`")
         else:
             return v
 
-        # validate data type: AzureSynthesizer
-        if not isinstance(v, AzureSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AzureSynthesizer`")
-        else:
-            return v
-
-        # validate data type: RimeSynthesizer
-        if not isinstance(v, RimeSynthesizer):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `RimeSynthesizer`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Voice1 with anyOf schemas: AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Model with anyOf schemas: AzureModel, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[ElevenLabsSynthesizer] = None
-        try:
-            instance.actual_instance = ElevenLabsSynthesizer.from_json(json_str)
-            return instance
-        except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[AzureSynthesizer] = None
+        # anyof_schema_1_validator: Optional[AzureModel] = None
         try:
-            instance.actual_instance = AzureSynthesizer.from_json(json_str)
+            instance.actual_instance = AzureModel.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
-        # anyof_schema_3_validator: Optional[RimeSynthesizer] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = RimeSynthesizer.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Voice1 with anyOf schemas: AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Model with anyOf schemas: AzureModel, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], AzureSynthesizer, ElevenLabsSynthesizer, RimeSynthesizer]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], AzureModel, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `voiceos-0.8.1.2/voiceos/models/webhook.py` & `voiceos-0.8.1.3/voiceos/models/buy_phone_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from voiceos.models.event import Event
-from voiceos.models.method_enum import MethodEnum
+from voiceos.models.wako_api_models_phone_number_provider import WakoApiModelsPhoneNumberProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Webhook(BaseModel):
+class BuyPhoneNumber(BaseModel):
     """
-    Webhook
+    BuyPhoneNumber
     """ # noqa: E501
-    event: Event
-    url: StrictStr = Field(description="The url to call when the event is triggered")
-    method: MethodEnum = Field(description="The method to use when calling the url")
-    headers: Optional[Dict[str, StrictStr]] = Field(default=None, description="The headers to use when calling the url")
-    filter: Optional[Dict[str, StrictInt]] = Field(default=None, description="The filter to use when triggering the webhook")
-    __properties: ClassVar[List[str]] = ["event", "url", "method", "headers", "filter"]
+    provider: Optional[WakoApiModelsPhoneNumberProvider] = Field(default=None, description="The telephony provider.")
+    phone_number: Optional[StrictStr] = Field(default=None, description="The phone number to buy. If null, a random phone number will be purchased.")
+    __properties: ClassVar[List[str]] = ["provider", "phone_number"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Webhook from a JSON string"""
+        """Create an instance of BuyPhoneNumber from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,29 +66,25 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of event
-        if self.event:
-            _dict['event'] = self.event.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Webhook from a dict"""
+        """Create an instance of BuyPhoneNumber from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "event": Event.from_dict(obj["event"]) if obj.get("event") is not None else None,
-            "url": obj.get("url"),
-            "method": obj.get("method"),
+            "provider": obj.get("provider"),
+            "phone_number": obj.get("phone_number")
         })
         return _obj
```

### Comparing `voiceos-0.8.1.2/voiceos/rest.py` & `voiceos-0.8.1.3/voiceos/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     VoiceOS
 
     VoiceOS API
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `voiceos-0.8.1.2/voiceos.egg-info/PKG-INFO` & `voiceos-0.8.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: voiceos
-Version: 0.8.1.2
-Summary: VoiceOS Python SDK
-Home-page: https://github.com/WakoAi/voiceos-python
-Author: WakoAI
-Author-email: hello@wako.ai
-Keywords: VoiceOS,VoiceOS Python ClientSDK,VoiceOS Python
-Description-Content-Type: text/markdown
-
 # VoiceOS Python SDK
 
 This python client lets you build with [VoiceOS](https://voiceos.io)
 
 ## Installation
 
 You can install the package via pip:
@@ -30,23 +20,23 @@
 
 Create a new instance of the VoiceOS class by passing your API key:
 
 ```python
 voiceos = VoiceOS("your-api-key")
 ```
 
-Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/calls/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
+Start using the python client to access the [agent](https://docs.voiceos.io/api-reference/agents/get), [calls](https://docs.voiceos.io/api-reference/conversations/get) and [phone numbers](https://docs.voiceos.io/api-reference/phone-numbers/get) resources.
 
 ```python
 # Get all agents
 agents = voiceos.agents.list_agents()
 print(agents)
 
 # Get all calls
-calls = voiceos.calls.list_calls()
+calls = voiceos.conversations.list_conversations()
 print(calls)
 
 # Get all phone numbers
 phone_numbers = voiceos.phone_numbers.list_phone_numbers()
 print(phone_numbers)
 ```
 
@@ -70,8 +60,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-```
+```
```

### Comparing `voiceos-0.8.1.2/voiceos.egg-info/SOURCES.txt` & `voiceos-0.8.1.3/voiceos.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,84 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-test/test_agent.py
 test/test_agent_configuration.py
 test/test_agent_cost.py
-test/test_agent_language.py
 test/test_agent_pagination.py
 test/test_agent_provider.py
 test/test_agent_response.py
 test/test_agents_api.py
 test/test_azure_languages.py
 test/test_azure_model.py
-test/test_azure_synthesizer.py
 test/test_azure_transcriber.py
+test/test_azure_transcriber_languages_inner.py
+test/test_azure_voice.py
 test/test_buy_phone_number.py
-test/test_call_cost.py
-test/test_call_recording.py
-test/test_call_response.py
-test/test_call_status.py
-test/test_call_type.py
-test/test_calls_api.py
-test/test_calls_pagination.py
 test/test_chat_gpt.py
+test/test_conversation_cost.py
+test/test_conversation_recording.py
+test/test_conversation_response.py
+test/test_conversation_status.py
+test/test_conversation_type.py
+test/test_conversations_api.py
+test/test_conversations_pagination.py
 test/test_create_call.py
-test/test_create_call_response.py
-test/test_currency.py
 test/test_deepgram_languages.py
-test/test_deepgram_model.py
 test/test_deepgram_transcriber.py
+test/test_deepgram_voice.py
+test/test_default_api.py
 test/test_eleven_labs_model.py
-test/test_eleven_labs_synthesizer.py
+test/test_eleven_labs_voices.py
+test/test_elevenlabs_voice.py
 test/test_ended_reasons.py
-test/test_event.py
 test/test_event_name.py
-test/test_event_variable_name.py
 test/test_http_validation_error.py
+test/test_language.py
 test/test_language_model_cost.py
 test/test_message.py
 test/test_message_role.py
 test/test_method_enum.py
+test/test_model.py
+test/test_model1.py
+test/test_model2.py
+test/test_model3.py
+test/test_model4.py
 test/test_open_ai.py
-test/test_open_ai_function.py
-test/test_open_ai_function_parameter.py
-test/test_open_ai_function_type.py
 test/test_phone_number.py
+test/test_phone_number_events.py
 test/test_phone_number_pagination.py
 test/test_phone_number_response.py
 test/test_phone_number_to_buy.py
+test/test_phone_number_webhook.py
 test/test_phone_numbers_api.py
-test/test_rime_synthesizer.py
-test/test_synthesizer_cost.py
+test/test_play_ht_model.py
+test/test_playht_voice.py
+test/test_rime_speaker.py
+test/test_rime_voice.py
+test/test_speaker.py
 test/test_telephony_cost.py
 test/test_transcriber.py
 test/test_transcriber1.py
 test/test_transcriber_cost.py
+test/test_twilio_phone_call.py
 test/test_twilio_telephony.py
 test/test_update_agent.py
 test/test_update_phone_number.py
 test/test_validation_error.py
 test/test_validation_error_loc_inner.py
 test/test_voice.py
 test/test_voice1.py
+test/test_voice_cost.py
+test/test_voice_id.py
 test/test_wako_api_models_language_model_provider.py
 test/test_wako_api_models_phone_number_provider.py
+test/test_wako_api_models_synthesizer_deepgram_model.py
 test/test_wako_api_models_synthesizer_provider.py
+test/test_wako_api_models_transcriber_deepgram_model.py
 test/test_wako_api_models_transcriber_provider.py
 test/test_webhook.py
 voiceos/__init__.py
 voiceos/api_client.py
 voiceos/api_response.py
 voiceos/client.py
 voiceos/configuration.py
@@ -78,72 +88,82 @@
 voiceos.egg-info/PKG-INFO
 voiceos.egg-info/SOURCES.txt
 voiceos.egg-info/dependency_links.txt
 voiceos.egg-info/requires.txt
 voiceos.egg-info/top_level.txt
 voiceos/api/__init__.py
 voiceos/api/agents_api.py
-voiceos/api/calls_api.py
+voiceos/api/conversations_api.py
+voiceos/api/default_api.py
 voiceos/api/phone_numbers_api.py
 voiceos/models/__init__.py
-voiceos/models/agent.py
 voiceos/models/agent_configuration.py
 voiceos/models/agent_cost.py
-voiceos/models/agent_language.py
 voiceos/models/agent_pagination.py
 voiceos/models/agent_provider.py
 voiceos/models/agent_response.py
 voiceos/models/azure_languages.py
 voiceos/models/azure_model.py
-voiceos/models/azure_synthesizer.py
 voiceos/models/azure_transcriber.py
+voiceos/models/azure_transcriber_languages_inner.py
+voiceos/models/azure_voice.py
 voiceos/models/buy_phone_number.py
-voiceos/models/call_cost.py
-voiceos/models/call_recording.py
-voiceos/models/call_response.py
-voiceos/models/call_status.py
-voiceos/models/call_type.py
-voiceos/models/calls_pagination.py
 voiceos/models/chat_gpt.py
+voiceos/models/conversation_cost.py
+voiceos/models/conversation_recording.py
+voiceos/models/conversation_response.py
+voiceos/models/conversation_status.py
+voiceos/models/conversation_type.py
+voiceos/models/conversations_pagination.py
 voiceos/models/create_call.py
-voiceos/models/create_call_response.py
-voiceos/models/currency.py
 voiceos/models/deepgram_languages.py
-voiceos/models/deepgram_model.py
 voiceos/models/deepgram_transcriber.py
+voiceos/models/deepgram_voice.py
 voiceos/models/eleven_labs_model.py
-voiceos/models/eleven_labs_synthesizer.py
+voiceos/models/eleven_labs_voices.py
+voiceos/models/elevenlabs_voice.py
 voiceos/models/ended_reasons.py
-voiceos/models/event.py
 voiceos/models/event_name.py
-voiceos/models/event_variable_name.py
 voiceos/models/http_validation_error.py
+voiceos/models/language.py
 voiceos/models/language_model_cost.py
 voiceos/models/message.py
 voiceos/models/message_role.py
 voiceos/models/method_enum.py
+voiceos/models/model.py
+voiceos/models/model1.py
+voiceos/models/model2.py
+voiceos/models/model3.py
+voiceos/models/model4.py
 voiceos/models/open_ai.py
-voiceos/models/open_ai_function.py
-voiceos/models/open_ai_function_parameter.py
-voiceos/models/open_ai_function_type.py
 voiceos/models/phone_number.py
+voiceos/models/phone_number_events.py
 voiceos/models/phone_number_pagination.py
 voiceos/models/phone_number_response.py
 voiceos/models/phone_number_to_buy.py
-voiceos/models/rime_synthesizer.py
-voiceos/models/synthesizer_cost.py
+voiceos/models/phone_number_webhook.py
+voiceos/models/play_ht_model.py
+voiceos/models/playht_voice.py
+voiceos/models/rime_speaker.py
+voiceos/models/rime_voice.py
+voiceos/models/speaker.py
 voiceos/models/telephony_cost.py
 voiceos/models/transcriber.py
 voiceos/models/transcriber1.py
 voiceos/models/transcriber_cost.py
+voiceos/models/twilio_phone_call.py
 voiceos/models/twilio_telephony.py
 voiceos/models/update_agent.py
 voiceos/models/update_phone_number.py
 voiceos/models/validation_error.py
 voiceos/models/validation_error_loc_inner.py
 voiceos/models/voice.py
 voiceos/models/voice1.py
+voiceos/models/voice_cost.py
+voiceos/models/voice_id.py
 voiceos/models/wako_api_models_language_model_provider.py
 voiceos/models/wako_api_models_phone_number_provider.py
+voiceos/models/wako_api_models_synthesizer_deepgram_model.py
 voiceos/models/wako_api_models_synthesizer_provider.py
+voiceos/models/wako_api_models_transcriber_deepgram_model.py
 voiceos/models/wako_api_models_transcriber_provider.py
 voiceos/models/webhook.py
```

