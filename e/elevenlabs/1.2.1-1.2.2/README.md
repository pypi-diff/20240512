# Comparing `tmp/elevenlabs-1.2.1.tar.gz` & `tmp/elevenlabs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.2.1.tar", max compression
+gzip compressed data, was "elevenlabs-1.2.2.tar", max compression
```

## Comparing `elevenlabs-1.2.1.tar` & `elevenlabs-1.2.2.tar`

### file list

```diff
@@ -1,132 +1,136 @@
--rw-r--r--   0        0        0     1067 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/LICENSE
--rw-r--r--   0        0        0     9366 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/README.md
--rw-r--r--   0        0        0      658 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5583 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13857 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     8308 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    36655 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20882 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/client.py
--rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/unchecked_base_model.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    29465 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    29717 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    64710 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0      303 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    38937 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0      344 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/types/__init__.py
--rw-r--r--   0        0        0     1192 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py
--rw-r--r--   0        0        0        0 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11479 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    29158 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    24639 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     7085 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      188 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      977 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1057 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      955 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      918 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      158 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      979 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1568 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0      177 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/category.py
--rw-r--r--   0        0        0     1195 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1010 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1028 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      146 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      949 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/dubbing_metadata_response.py
--rw-r--r--   0        0        0      211 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1081 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1836 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      220 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      148 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2290 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1071 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1159 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
--rw-r--r--   0        0        0     1067 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1072 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      952 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      991 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1009 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      947 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      930 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1764 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1010 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1085 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1670 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2215 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      173 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      405 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1277 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1258 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      990 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      965 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
--rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
--rw-r--r--   0        0        0      973 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1488 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      958 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      217 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2361 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      144 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1864 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      223 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1078 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      170 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1878 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1610 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      197 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      253 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1140 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1028 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1119 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     2088 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      945 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1324 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      213 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1101 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1082 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2484 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      193 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1244 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9597 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    21042 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    62413 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/LICENSE
+-rw-r--r--   0        0        0     9366 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/README.md
+-rw-r--r--   0        0        0      658 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5740 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    14317 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     8312 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    38363 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/client.py
+-rw-r--r--   0        0        0     1006 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0     7165 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/core/unchecked_base_model.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    30806 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    31344 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5533 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    67107 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0      303 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    40673 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0      344 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/pronunciation_dictionary/types/__init__.py
+-rw-r--r--   0        0        0     2031 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py
+-rw-r--r--   0        0        0        0 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5396 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    12067 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    20923 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0      123 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    24429 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0      130 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/text_to_speech/types/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-12 02:06:33.011434 elevenlabs-1.2.2/src/elevenlabs/text_to_speech/types/send_message.py
+-rw-r--r--   0        0        0     7238 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      977 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1057 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      955 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      918 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      158 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      979 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1568 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0      177 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/category.py
+-rw-r--r--   0        0        0     1195 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1010 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1028 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0     1001 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/close_connection.py
+-rw-r--r--   0        0        0      146 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      949 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0     1006 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/dubbing_metadata_response.py
+-rw-r--r--   0        0        0      211 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1081 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1836 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      220 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      148 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2290 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      987 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1071 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      987 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1159 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
+-rw-r--r--   0        0        0     1067 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1072 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      952 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      991 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1009 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0     1765 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/initialize_connection.py
+-rw-r--r--   0        0        0      947 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      930 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1764 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1010 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1085 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1670 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2215 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      173 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      405 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1277 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1258 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      990 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      965 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
+-rw-r--r--   0        0        0      987 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
+-rw-r--r--   0        0        0      973 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1488 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1006 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      958 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      217 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     1856 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      144 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1864 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      223 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1078 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      170 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1878 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1610 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      197 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      253 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1140 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1028 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1119 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     2088 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      945 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1324 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      213 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1101 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1082 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2484 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      193 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1244 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0    10113 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    22211 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    66097 2024-05-12 02:06:33.015434 elevenlabs-1.2.2/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.2.2/PKG-INFO
```

### Comparing `elevenlabs-1.2.1/LICENSE` & `elevenlabs-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/README.md` & `elevenlabs-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/pyproject.toml` & `elevenlabs-1.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elevenlabs"
-version = "v1.2.1"
+version = "v1.2.2"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "elevenlabs", from = "src"}
 ]
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/__init__.py` & `elevenlabs-1.2.2/src/elevenlabs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     AudioOutput,
     Category,
     ChapterResponse,
     ChapterSnapshotResponse,
     ChapterSnapshotsResponse,
     ChapterState,
     ChapterStatisticsResponse,
+    CloseConnection,
     Currency,
     DoDubbingResponse,
     DubbingMetadataResponse,
     ExtendedSubscriptionResponseModelBillingPeriod,
     FeedbackItem,
     FineTuningResponse,
     FinetuningState,
@@ -31,14 +32,15 @@
     GetPronunciationDictionariesMetadataResponseModel,
     GetPronunciationDictionaryMetadataResponse,
     GetSpeechHistoryResponse,
     GetVoicesResponse,
     History,
     HistoryItem,
     HttpValidationError,
+    InitializeConnection,
     Invoice,
     LanguageResponse,
     LibraryVoiceResponse,
     ManualVerificationFileResponse,
     ManualVerificationResponse,
     Model,
     NormalizedAlignment,
@@ -99,14 +101,15 @@
 from .environment import ElevenLabsEnvironment
 from .play import play, save, stream
 from .pronunciation_dictionary import (
     PronunciationDictionaryRule,
     PronunciationDictionaryRule_Alias,
     PronunciationDictionaryRule_Phoneme,
 )
+from .text_to_speech import SendMessage
 from .version import __version__
 
 __all__ = [
     "Accent",
     "AddProjectResponseModel",
     "AddPronunciationDictionaryResponseModel",
     "AddPronunciationDictionaryRulesResponseModel",
@@ -117,14 +120,15 @@
     "AudioOutput",
     "Category",
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
+    "CloseConnection",
     "Currency",
     "DoDubbingResponse",
     "DubbingMetadataResponse",
     "ElevenLabsEnvironment",
     "ExtendedSubscriptionResponseModelBillingPeriod",
     "FeedbackItem",
     "FineTuningResponse",
@@ -137,14 +141,15 @@
     "GetPronunciationDictionariesMetadataResponseModel",
     "GetPronunciationDictionaryMetadataResponse",
     "GetSpeechHistoryResponse",
     "GetVoicesResponse",
     "History",
     "HistoryItem",
     "HttpValidationError",
+    "InitializeConnection",
     "Invoice",
     "LanguageResponse",
     "LibraryVoiceResponse",
     "ManualVerificationFileResponse",
     "ManualVerificationResponse",
     "Model",
     "NormalizedAlignment",
@@ -161,14 +166,15 @@
     "PronunciationDictionaryRule_Alias",
     "PronunciationDictionaryRule_Phoneme",
     "PronunciationDictionaryVersionLocator",
     "RealtimeVoiceSettings",
     "RecordingResponse",
     "RemovePronunciationDictionaryRulesResponseModel",
     "ReviewStatus",
+    "SendMessage",
     "SendText",
     "Source",
     "SpeechHistoryItemResponse",
     "SpeechHistoryItemResponseModelVoiceCategory",
     "SsoProviderDbModel",
     "SsoProviderDbModelProviderType",
     "Subscription",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.2.2/src/elevenlabs/audio_native/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,57 +23,78 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self,
         *,
         name: str,
+        file: core.File,
         image: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         small: typing.Optional[bool] = None,
         text_color: typing.Optional[str] = None,
         background_color: typing.Optional[str] = None,
         sessionization: typing.Optional[int] = None,
         voice_id: typing.Optional[str] = None,
         model_id: typing.Optional[str] = None,
-        file: core.File,
         auto_convert: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudioNativeCreateProjectResponseModel:
         """
         Creates AudioNative enabled project, optionally starts conversion and returns project id and embeddable html snippet.
 
-        Parameters:
-            - name: str. Project name.
+        Parameters
+        ----------
+        name : str
+            Project name.
+
+        file : core.File
+            See core.File for more documentation
+
+        image : typing.Optional[str]
+            Image URL used in the player. If not provided, default image set in the Player settings is used.
 
-            - image: typing.Optional[str]. Image URL used in the player. If not provided, default image set in the Player settings is used.
+        author : typing.Optional[str]
+            Author used in the player and inserted at the start of the uploaded article. If not provided, the default author set in the Player settings is used.
 
-            - author: typing.Optional[str]. Author used in the player and inserted at the start of the uploaded article. If not provided, the default author set in the Player settings is used.
+        title : typing.Optional[str]
+            Title used in the player and inserted at the top of the uploaded article. If not provided, the default title set in the Player settings is used.
 
-            - title: typing.Optional[str]. Title used in the player and inserted at the top of the uploaded article. If not provided, the default title set in the Player settings is used.
+        small : typing.Optional[bool]
+            Whether to use small player or not. If not provided, default value set in the Player settings is used.
 
-            - small: typing.Optional[bool]. Whether to use small player or not. If not provided, default value set in the Player settings is used.
+        text_color : typing.Optional[str]
+            Text color used in the player. If not provided, default text color set in the Player settings is used.
 
-            - text_color: typing.Optional[str]. Text color used in the player. If not provided, default text color set in the Player settings is used.
+        background_color : typing.Optional[str]
+            Background color used in the player. If not provided, default background color set in the Player settings is used.
 
-            - background_color: typing.Optional[str]. Background color used in the player. If not provided, default background color set in the Player settings is used.
+        sessionization : typing.Optional[int]
+            Specifies for how many minutes to persist the session across page reloads. If not provided, default sessionization set in the Player settings is used.
 
-            - sessionization: typing.Optional[int]. Specifies for how many minutes to persist the session across page reloads. If not provided, default sessionization set in the Player settings is used.
+        voice_id : typing.Optional[str]
+            Voice ID used to voice the content. If not provided, default voice ID set in the Player settings is used.
 
-            - voice_id: typing.Optional[str]. Voice ID used to voice the content. If not provided, default voice ID set in the Player settings is used.
+        model_id : typing.Optional[str]
+            TTS Model ID used in the player. If not provided, default model ID set in the Player settings is used.
 
-            - model_id: typing.Optional[str]. TTS Model ID used in the player. If not provided, default model ID set in the Player settings is used.
+        auto_convert : typing.Optional[bool]
+            Whether to auto convert the project to audio or not.
 
-            - file: core.File. See core.File for more documentation
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - auto_convert: typing.Optional[bool]. Whether to auto convert the project to audio or not.
+        Returns
+        -------
+        AudioNativeCreateProjectResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.audio_native.create(
             name="name",
@@ -155,57 +176,78 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
         self,
         *,
         name: str,
+        file: core.File,
         image: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         small: typing.Optional[bool] = None,
         text_color: typing.Optional[str] = None,
         background_color: typing.Optional[str] = None,
         sessionization: typing.Optional[int] = None,
         voice_id: typing.Optional[str] = None,
         model_id: typing.Optional[str] = None,
-        file: core.File,
         auto_convert: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AudioNativeCreateProjectResponseModel:
         """
         Creates AudioNative enabled project, optionally starts conversion and returns project id and embeddable html snippet.
 
-        Parameters:
-            - name: str. Project name.
+        Parameters
+        ----------
+        name : str
+            Project name.
+
+        file : core.File
+            See core.File for more documentation
+
+        image : typing.Optional[str]
+            Image URL used in the player. If not provided, default image set in the Player settings is used.
 
-            - image: typing.Optional[str]. Image URL used in the player. If not provided, default image set in the Player settings is used.
+        author : typing.Optional[str]
+            Author used in the player and inserted at the start of the uploaded article. If not provided, the default author set in the Player settings is used.
 
-            - author: typing.Optional[str]. Author used in the player and inserted at the start of the uploaded article. If not provided, the default author set in the Player settings is used.
+        title : typing.Optional[str]
+            Title used in the player and inserted at the top of the uploaded article. If not provided, the default title set in the Player settings is used.
 
-            - title: typing.Optional[str]. Title used in the player and inserted at the top of the uploaded article. If not provided, the default title set in the Player settings is used.
+        small : typing.Optional[bool]
+            Whether to use small player or not. If not provided, default value set in the Player settings is used.
 
-            - small: typing.Optional[bool]. Whether to use small player or not. If not provided, default value set in the Player settings is used.
+        text_color : typing.Optional[str]
+            Text color used in the player. If not provided, default text color set in the Player settings is used.
 
-            - text_color: typing.Optional[str]. Text color used in the player. If not provided, default text color set in the Player settings is used.
+        background_color : typing.Optional[str]
+            Background color used in the player. If not provided, default background color set in the Player settings is used.
 
-            - background_color: typing.Optional[str]. Background color used in the player. If not provided, default background color set in the Player settings is used.
+        sessionization : typing.Optional[int]
+            Specifies for how many minutes to persist the session across page reloads. If not provided, default sessionization set in the Player settings is used.
 
-            - sessionization: typing.Optional[int]. Specifies for how many minutes to persist the session across page reloads. If not provided, default sessionization set in the Player settings is used.
+        voice_id : typing.Optional[str]
+            Voice ID used to voice the content. If not provided, default voice ID set in the Player settings is used.
 
-            - voice_id: typing.Optional[str]. Voice ID used to voice the content. If not provided, default voice ID set in the Player settings is used.
+        model_id : typing.Optional[str]
+            TTS Model ID used in the player. If not provided, default model ID set in the Player settings is used.
 
-            - model_id: typing.Optional[str]. TTS Model ID used in the player. If not provided, default model ID set in the Player settings is used.
+        auto_convert : typing.Optional[bool]
+            Whether to auto convert the project to audio or not.
 
-            - file: core.File. See core.File for more documentation
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - auto_convert: typing.Optional[bool]. Whether to auto convert the project to audio or not.
+        Returns
+        -------
+        AudioNativeCreateProjectResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.audio_native.create(
             name="name",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/base_client.py` & `elevenlabs-1.2.2/src/elevenlabs/base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,40 @@
 from .voices.client import AsyncVoicesClient, VoicesClient
 
 
 class BaseElevenLabs:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: ElevenLabsEnvironment. The environment to use for requests from the client. from .environment import ElevenLabsEnvironment
+    environment : ElevenLabsEnvironment
+        The environment to use for requests from the client. from .environment import ElevenLabsEnvironment
 
-                                              Defaults to ElevenLabsEnvironment.PRODUCTION
 
-        - api_key: typing.Optional[str].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+        Defaults to ElevenLabsEnvironment.PRODUCTION
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+    api_key : typing.Optional[str]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.Client]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from elevenlabs.client import ElevenLabs
 
     client = ElevenLabs(
         api_key="YOUR_API_KEY",
     )
     """
 
@@ -84,29 +95,40 @@
         self.pronunciation_dictionary = PronunciationDictionaryClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseElevenLabs:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
+
+    environment : ElevenLabsEnvironment
+        The environment to use for requests from the client. from .environment import ElevenLabsEnvironment
+
+
+
+        Defaults to ElevenLabsEnvironment.PRODUCTION
 
-        - environment: ElevenLabsEnvironment. The environment to use for requests from the client. from .environment import ElevenLabsEnvironment
 
-                                              Defaults to ElevenLabsEnvironment.PRODUCTION
 
-        - api_key: typing.Optional[str].
+    api_key : typing.Optional[str]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+    httpx_client : typing.Optional[httpx.AsyncClient]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
-        - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+    Examples
+    --------
     from elevenlabs.client import AsyncElevenLabs
 
     client = AsyncElevenLabs(
         api_key="YOUR_API_KEY",
     )
     """
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/chapters/client.py` & `elevenlabs-1.2.2/src/elevenlabs/chapters/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,29 @@
 
     def get_all(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetChaptersResponse:
         """
         Returns a list of your chapters for a project together and its metadata.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetChaptersResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.get_all(
             project_id="project_id",
@@ -80,21 +90,32 @@
 
     def get(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ChapterResponse:
         """
         Returns information about a specific chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChapterResponse
+            Successful Response
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.get(
             project_id="project_id",
@@ -138,21 +159,32 @@
 
     def delete(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Delete a chapter by its chapter_id.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.delete(
             project_id="project_id",
@@ -196,21 +228,32 @@
 
     def convert(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Starts conversion of a specific chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.convert(
             project_id="project_id",
@@ -257,21 +300,32 @@
 
     def get_all_snapshots(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ChapterSnapshotsResponse:
         """
         Gets information about all the snapshots of a chapter, each snapshot corresponds can be downloaded as audio. Whenever a chapter is converted a snapshot will be automatically created.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChapterSnapshotsResponse
+            Successful Response
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.get_all_snapshots(
             project_id="project_id",
@@ -321,25 +375,37 @@
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Stream the audio from a chapter snapshot. Use `GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots` to return the chapter snapshots of a chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        chapter_snapshot_id : str
+            The chapter_snapshot_id of the chapter snapshot. You can query GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots to the all available snapshots for a chapter.
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        convert_to_mpeg : typing.Optional[bool]
+            Whether to convert the audio to mpeg format.
 
-            - chapter_snapshot_id: str. The chapter_snapshot_id of the chapter snapshot. You can query GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots to the all available snapshots for a chapter.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - convert_to_mpeg: typing.Optional[bool]. Whether to convert the audio to mpeg format.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.chapters.stream_snapshot(
             project_id="project_id",
@@ -398,19 +464,29 @@
 
     async def get_all(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetChaptersResponse:
         """
         Returns a list of your chapters for a project together and its metadata.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetChaptersResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.get_all(
             project_id="project_id",
@@ -452,21 +528,32 @@
 
     async def get(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ChapterResponse:
         """
         Returns information about a specific chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChapterResponse
+            Successful Response
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.get(
             project_id="project_id",
@@ -510,21 +597,32 @@
 
     async def delete(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Delete a chapter by its chapter_id.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.delete(
             project_id="project_id",
@@ -568,21 +666,32 @@
 
     async def convert(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Starts conversion of a specific chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.convert(
             project_id="project_id",
@@ -629,21 +738,32 @@
 
     async def get_all_snapshots(
         self, project_id: str, chapter_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ChapterSnapshotsResponse:
         """
         Gets information about all the snapshots of a chapter, each snapshot corresponds can be downloaded as audio. Whenever a chapter is converted a snapshot will be automatically created.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChapterSnapshotsResponse
+            Successful Response
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.get_all_snapshots(
             project_id="project_id",
@@ -693,25 +813,37 @@
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Stream the audio from a chapter snapshot. Use `GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots` to return the chapter snapshots of a chapter.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        chapter_id : str
+            The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+
+        chapter_snapshot_id : str
+            The chapter_snapshot_id of the chapter snapshot. You can query GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots to the all available snapshots for a chapter.
 
-            - chapter_id: str. The chapter_id of the chapter. You can query GET https://api.elevenlabs.io/v1/projects/{project_id}/chapters to list all available chapters for a project.
+        convert_to_mpeg : typing.Optional[bool]
+            Whether to convert the audio to mpeg format.
 
-            - chapter_snapshot_id: str. The chapter_snapshot_id of the chapter snapshot. You can query GET /v1/projects/{project_id}/chapters/{chapter_id}/snapshots to the all available snapshots for a chapter.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - convert_to_mpeg: typing.Optional[bool]. Whether to convert the audio to mpeg format.
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.chapters.stream_snapshot(
             project_id="project_id",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/client.py` & `elevenlabs-1.2.2/src/elevenlabs/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/__init__.py` & `elevenlabs-1.2.2/src/elevenlabs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.2.2/src/elevenlabs/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.2.1",
+            "X-Fern-SDK-Version": "v1.2.2",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.2.2/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/file.py` & `elevenlabs-1.2.2/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/http_client.py` & `elevenlabs-1.2.2/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.2.2/src/elevenlabs/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/request_options.py` & `elevenlabs-1.2.2/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/core/unchecked_base_model.py` & `elevenlabs-1.2.2/src/elevenlabs/core/unchecked_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,18 @@
         inner_type = pydantic_v1.typing.get_args(type_)[0]
         return {construct_type(object_=entry, type_=inner_type) for entry in object_}
 
     if pydantic_v1.typing.is_union(base_type) or is_annotated_union:
         return _convert_union_type(type_, object_)
 
     # Cannot do an `issubclass` with a literal type, let's also just confirm we have a class before this call
-    if not pydantic_v1.typing.is_literal_type(type_) and (
-        inspect.isclass(base_type) and issubclass(base_type, pydantic_v1.BaseModel)
+    if (
+        object_ is not None
+        and not pydantic_v1.typing.is_literal_type(type_)
+        and (inspect.isclass(base_type) and issubclass(base_type, pydantic_v1.BaseModel))
     ):
         return type_.construct(**object_)
 
     if base_type == dt.datetime:
         try:
             return pydantic_v1.datetime_parse.parse_datetime(object_)
         except Exception:
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.2.2/src/elevenlabs/dubbing/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,67 +23,91 @@
 class DubbingClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def dub_a_video_or_an_audio_file(
         self,
         *,
+        target_lang: str,
         mode: typing.Optional[str] = None,
         file: typing.Optional[core.File] = None,
         csv_file: typing.Optional[core.File] = None,
         foreground_audio_file: typing.Optional[core.File] = None,
         background_audio_file: typing.Optional[core.File] = None,
         name: typing.Optional[str] = None,
         source_url: typing.Optional[str] = None,
         source_lang: typing.Optional[str] = None,
-        target_lang: str,
         num_speakers: typing.Optional[int] = None,
         watermark: typing.Optional[bool] = None,
         start_time: typing.Optional[int] = None,
         end_time: typing.Optional[int] = None,
         highest_resolution: typing.Optional[bool] = None,
         dubbing_studio: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DoDubbingResponse:
         """
         Dubs provided audio or video file into given language.
 
-        Parameters:
-            - mode: typing.Optional[str]. automatic or manual.
+        Parameters
+        ----------
+        target_lang : str
+            The Target language to dub the content into. Can be none if dubbing studio editor is enabled and running manual mode
+
+        mode : typing.Optional[str]
+            automatic or manual.
 
-            - file: typing.Optional[core.File]. See core.File for more documentation
+        file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - csv_file: typing.Optional[core.File]. See core.File for more documentation
+        csv_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - foreground_audio_file: typing.Optional[core.File]. See core.File for more documentation
+        foreground_audio_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - background_audio_file: typing.Optional[core.File]. See core.File for more documentation
+        background_audio_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - name: typing.Optional[str]. Name of the dubbing project.
+        name : typing.Optional[str]
+            Name of the dubbing project.
 
-            - source_url: typing.Optional[str]. URL of the source video/audio file.
+        source_url : typing.Optional[str]
+            URL of the source video/audio file.
 
-            - source_lang: typing.Optional[str]. Source language.
+        source_lang : typing.Optional[str]
+            Source language.
 
-            - target_lang: str. The Target language to dub the content into. Can be none if dubbing studio editor is enabled and running manual mode
+        num_speakers : typing.Optional[int]
+            Number of speakers to use for the dubbing.
 
-            - num_speakers: typing.Optional[int]. Number of speakers to use for the dubbing.
+        watermark : typing.Optional[bool]
+            Whether to apply watermark to the output video.
 
-            - watermark: typing.Optional[bool]. Whether to apply watermark to the output video.
+        start_time : typing.Optional[int]
+            Start time of the source video/audio file.
 
-            - start_time: typing.Optional[int]. Start time of the source video/audio file.
+        end_time : typing.Optional[int]
+            End time of the source video/audio file.
 
-            - end_time: typing.Optional[int]. End time of the source video/audio file.
+        highest_resolution : typing.Optional[bool]
+            Whether to use the highest resolution available.
 
-            - highest_resolution: typing.Optional[bool]. Whether to use the highest resolution available.
+        dubbing_studio : typing.Optional[bool]
+            Whether to prepare dub for edits in dubbing studio.
 
-            - dubbing_studio: typing.Optional[bool]. Whether to prepare dub for edits in dubbing studio.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        DoDubbingResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.dubbing.dub_a_video_or_an_audio_file(
             target_lang="target_lang",
@@ -171,19 +195,29 @@
 
     def get_dubbing_project_metadata(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DubbingMetadataResponse:
         """
         Returns metadata about a dubbing project, including whether it's still in progress or not
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DubbingMetadataResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.dubbing.get_dubbing_project_metadata(
             dubbing_id="dubbing_id",
@@ -225,19 +259,29 @@
 
     def delete_dubbing_project(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Deletes a dubbing project.
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.dubbing.delete_dubbing_project(
             dubbing_id="dubbing_id",
@@ -279,21 +323,32 @@
 
     def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Iterator[bytes]:
         """
         Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
-
-            - language_code: str. ID of the language.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        language_code : str
+            ID of the language.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.dubbing.get_dubbed_file(
             dubbing_id="string",
@@ -342,67 +397,91 @@
 class AsyncDubbingClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def dub_a_video_or_an_audio_file(
         self,
         *,
+        target_lang: str,
         mode: typing.Optional[str] = None,
         file: typing.Optional[core.File] = None,
         csv_file: typing.Optional[core.File] = None,
         foreground_audio_file: typing.Optional[core.File] = None,
         background_audio_file: typing.Optional[core.File] = None,
         name: typing.Optional[str] = None,
         source_url: typing.Optional[str] = None,
         source_lang: typing.Optional[str] = None,
-        target_lang: str,
         num_speakers: typing.Optional[int] = None,
         watermark: typing.Optional[bool] = None,
         start_time: typing.Optional[int] = None,
         end_time: typing.Optional[int] = None,
         highest_resolution: typing.Optional[bool] = None,
         dubbing_studio: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DoDubbingResponse:
         """
         Dubs provided audio or video file into given language.
 
-        Parameters:
-            - mode: typing.Optional[str]. automatic or manual.
+        Parameters
+        ----------
+        target_lang : str
+            The Target language to dub the content into. Can be none if dubbing studio editor is enabled and running manual mode
+
+        mode : typing.Optional[str]
+            automatic or manual.
 
-            - file: typing.Optional[core.File]. See core.File for more documentation
+        file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - csv_file: typing.Optional[core.File]. See core.File for more documentation
+        csv_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - foreground_audio_file: typing.Optional[core.File]. See core.File for more documentation
+        foreground_audio_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - background_audio_file: typing.Optional[core.File]. See core.File for more documentation
+        background_audio_file : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - name: typing.Optional[str]. Name of the dubbing project.
+        name : typing.Optional[str]
+            Name of the dubbing project.
 
-            - source_url: typing.Optional[str]. URL of the source video/audio file.
+        source_url : typing.Optional[str]
+            URL of the source video/audio file.
 
-            - source_lang: typing.Optional[str]. Source language.
+        source_lang : typing.Optional[str]
+            Source language.
 
-            - target_lang: str. The Target language to dub the content into. Can be none if dubbing studio editor is enabled and running manual mode
+        num_speakers : typing.Optional[int]
+            Number of speakers to use for the dubbing.
 
-            - num_speakers: typing.Optional[int]. Number of speakers to use for the dubbing.
+        watermark : typing.Optional[bool]
+            Whether to apply watermark to the output video.
 
-            - watermark: typing.Optional[bool]. Whether to apply watermark to the output video.
+        start_time : typing.Optional[int]
+            Start time of the source video/audio file.
 
-            - start_time: typing.Optional[int]. Start time of the source video/audio file.
+        end_time : typing.Optional[int]
+            End time of the source video/audio file.
 
-            - end_time: typing.Optional[int]. End time of the source video/audio file.
+        highest_resolution : typing.Optional[bool]
+            Whether to use the highest resolution available.
 
-            - highest_resolution: typing.Optional[bool]. Whether to use the highest resolution available.
+        dubbing_studio : typing.Optional[bool]
+            Whether to prepare dub for edits in dubbing studio.
 
-            - dubbing_studio: typing.Optional[bool]. Whether to prepare dub for edits in dubbing studio.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        DoDubbingResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.dub_a_video_or_an_audio_file(
             target_lang="target_lang",
@@ -490,19 +569,29 @@
 
     async def get_dubbing_project_metadata(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DubbingMetadataResponse:
         """
         Returns metadata about a dubbing project, including whether it's still in progress or not
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DubbingMetadataResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.get_dubbing_project_metadata(
             dubbing_id="dubbing_id",
@@ -544,19 +633,29 @@
 
     async def delete_dubbing_project(
         self, dubbing_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Deletes a dubbing project.
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.delete_dubbing_project(
             dubbing_id="dubbing_id",
@@ -598,21 +697,32 @@
 
     async def get_dubbed_file(
         self, dubbing_id: str, language_code: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.AsyncIterator[bytes]:
         """
         Returns dubbed file as a streamed file. Videos will be returned in MP4 format and audio only dubs will be returned in MP3.
 
-        Parameters:
-            - dubbing_id: str. ID of the dubbing project.
-
-            - language_code: str. ID of the language.
+        Parameters
+        ----------
+        dubbing_id : str
+            ID of the dubbing project.
+
+        language_code : str
+            ID of the language.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.dubbing.get_dubbed_file(
             dubbing_id="string",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/history/client.py` & `elevenlabs-1.2.2/src/elevenlabs/history/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,29 +30,44 @@
         start_after_history_item_id: typing.Optional[str] = None,
         voice_id: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetSpeechHistoryResponse:
         """
         Returns metadata about all your generated audio.
 
-        Parameters:
-            - page_size: typing.Optional[int]. How many history items to return at maximum. Can not exceed 1000, defaults to 100.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            How many history items to return at maximum. Can not exceed 1000, defaults to 100.
+
+        start_after_history_item_id : typing.Optional[str]
+            After which ID to start fetching, use this parameter to paginate across a large collection of history items. In case this parameter is not provided history items will be fetched starting from the most recently created one ordered descending by their creation date.
+
+        voice_id : typing.Optional[str]
+            Voice ID to be filtered for, you can use GET https://api.elevenlabs.io/v1/voices to receive a list of voices and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetSpeechHistoryResponse
+            Successful Response
 
-            - start_after_history_item_id: typing.Optional[str]. After which ID to start fetching, use this parameter to paginate across a large collection of history items. In case this parameter is not provided history items will be fetched starting from the most recently created one ordered descending by their creation date.
-
-            - voice_id: typing.Optional[str]. Voice ID to be filtered for, you can use GET https://api.elevenlabs.io/v1/voices to receive a list of voices and their IDs.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.history.get_all()
+        client.history.get_all(
+            page_size=1,
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -95,26 +110,36 @@
 
     def get(
         self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SpeechHistoryItemResponse:
         """
         Returns information about an history item by its ID.
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        SpeechHistoryItemResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.get(
-            history_item_id="history_item_id",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
@@ -147,26 +172,36 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a history item by its ID
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.delete(
-            history_item_id="history_item_id",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
@@ -201,26 +236,36 @@
 
     def get_audio(
         self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Iterator[bytes]:
         """
         Returns the audio of an history item.
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.get_audio(
-            history_item_id="string",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         with self._client_wrapper.httpx_client.stream(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}/audio"
             ),
@@ -262,28 +307,38 @@
         history_item_ids: typing.Sequence[str],
         output_format: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Download one or more history items. If one history item ID is provided, we will return a single audio file. If more than one history item IDs are provided, we will provide the history items packed into a .zip file.
 
-        Parameters:
-            - history_item_ids: typing.Sequence[str]. A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
-
-            - output_format: typing.Optional[str]. Output format to transcode the audio file, can be wav or default.
+        Parameters
+        ----------
+        history_item_ids : typing.Sequence[str]
+            A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
+
+        output_format : typing.Optional[str]
+            Output format to transcode the audio file, can be wav or default.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.history.download(
-            history_item_ids=["history_item_ids"],
+            history_item_ids=["ja9xsmfGhxYcymxGcOGB"],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
         if output_format is not OMIT:
             _request["output_format"] = output_format
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
@@ -335,29 +390,44 @@
         start_after_history_item_id: typing.Optional[str] = None,
         voice_id: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetSpeechHistoryResponse:
         """
         Returns metadata about all your generated audio.
 
-        Parameters:
-            - page_size: typing.Optional[int]. How many history items to return at maximum. Can not exceed 1000, defaults to 100.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            How many history items to return at maximum. Can not exceed 1000, defaults to 100.
+
+        start_after_history_item_id : typing.Optional[str]
+            After which ID to start fetching, use this parameter to paginate across a large collection of history items. In case this parameter is not provided history items will be fetched starting from the most recently created one ordered descending by their creation date.
+
+        voice_id : typing.Optional[str]
+            Voice ID to be filtered for, you can use GET https://api.elevenlabs.io/v1/voices to receive a list of voices and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetSpeechHistoryResponse
+            Successful Response
 
-            - start_after_history_item_id: typing.Optional[str]. After which ID to start fetching, use this parameter to paginate across a large collection of history items. In case this parameter is not provided history items will be fetched starting from the most recently created one ordered descending by their creation date.
-
-            - voice_id: typing.Optional[str]. Voice ID to be filtered for, you can use GET https://api.elevenlabs.io/v1/voices to receive a list of voices and their IDs.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.history.get_all()
+        await client.history.get_all(
+            page_size=1,
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/history"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -400,26 +470,36 @@
 
     async def get(
         self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> SpeechHistoryItemResponse:
         """
         Returns information about an history item by its ID.
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        SpeechHistoryItemResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.get(
-            history_item_id="history_item_id",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
@@ -454,26 +534,36 @@
 
     async def delete(
         self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Delete a history item by its ID
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.delete(
-            history_item_id="history_item_id",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}"
             ),
@@ -508,26 +598,36 @@
 
     async def get_audio(
         self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.AsyncIterator[bytes]:
         """
         Returns the audio of an history item.
 
-        Parameters:
-            - history_item_id: str. History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+        Parameters
+        ----------
+        history_item_id : str
+            History item ID to be used, you can use GET https://api.elevenlabs.io/v1/history to receive a list of history items and their IDs.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.get_audio(
-            history_item_id="string",
+            history_item_id="ja9xsmfGhxYcymxGcOGB",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/history/{jsonable_encoder(history_item_id)}/audio"
             ),
@@ -569,28 +669,38 @@
         history_item_ids: typing.Sequence[str],
         output_format: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Download one or more history items. If one history item ID is provided, we will return a single audio file. If more than one history item IDs are provided, we will provide the history items packed into a .zip file.
 
-        Parameters:
-            - history_item_ids: typing.Sequence[str]. A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
-
-            - output_format: typing.Optional[str]. Output format to transcode the audio file, can be wav or default.
+        Parameters
+        ----------
+        history_item_ids : typing.Sequence[str]
+            A list of history items to download, you can get IDs of history items and other metadata using the GET https://api.elevenlabs.io/v1/history endpoint.
+
+        output_format : typing.Optional[str]
+            Output format to transcode the audio file, can be wav or default.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.history.download(
-            history_item_ids=["history_item_ids"],
+            history_item_ids=["ja9xsmfGhxYcymxGcOGB"],
         )
         """
         _request: typing.Dict[str, typing.Any] = {"history_item_ids": history_item_ids}
         if output_format is not OMIT:
             _request["output_format"] = output_format
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/models/client.py` & `elevenlabs-1.2.2/src/elevenlabs/models/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,17 +19,26 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Model]:
         """
         Gets a list of available models.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.List[Model]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.models.get_all()
         """
@@ -70,17 +79,26 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Model]:
         """
         Gets a list of available models.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.List[Model]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.models.get_all()
         """
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/play.py` & `elevenlabs-1.2.2/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/projects/client.py` & `elevenlabs-1.2.2/src/elevenlabs/projects/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,26 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetProjectsResponse:
         """
         Returns a list of your projects together and its metadata.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetProjectsResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.get_all()
         """
@@ -73,67 +82,91 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add(
         self,
         *,
         name: str,
-        from_url: typing.Optional[str] = None,
-        from_document: typing.Optional[core.File] = None,
         default_title_voice_id: str,
         default_paragraph_voice_id: str,
         default_model_id: str,
+        from_url: typing.Optional[str] = None,
+        from_document: typing.Optional[core.File] = None,
         quality_preset: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         isbn_number: typing.Optional[str] = None,
         acx_volume_normalization: typing.Optional[bool] = None,
         volume_normalization: typing.Optional[bool] = None,
         pronunciation_dictionary_locators: typing.Optional[typing.List[str]] = None,
         callback_url: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddProjectResponseModel:
         """
         Creates a new project, it can be either initialized as blank, from a document or from a URL.
 
-        Parameters:
-            - name: str. The name of the project, used for identification only.
+        Parameters
+        ----------
+        name : str
+            The name of the project, used for identification only.
+
+        default_title_voice_id : str
+            The voice_id that corresponds to the default voice used for new titles.
 
-            - from_url: typing.Optional[str]. An optional URL from which we will extract content to initialize the project. If this is set, 'from_url' must be null. If neither 'from_url' or 'from_document' are provided we will initialize the project as blank.
+        default_paragraph_voice_id : str
+            The voice_id that corresponds to the default voice used for new paragraphs.
 
-            - from_document: typing.Optional[core.File]. See core.File for more documentation
+        default_model_id : str
+            The model_id of the model to be used for this project, you can query GET https://api.elevenlabs.io/v1/models to list all available models.
 
-            - default_title_voice_id: str. The voice_id that corresponds to the default voice used for new titles.
+        from_url : typing.Optional[str]
+            An optional URL from which we will extract content to initialize the project. If this is set, 'from_url' must be null. If neither 'from_url' or 'from_document' are provided we will initialize the project as blank.
 
-            - default_paragraph_voice_id: str. The voice_id that corresponds to the default voice used for new paragraphs.
+        from_document : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - default_model_id: str. The model_id of the model to be used for this project, you can query GET https://api.elevenlabs.io/v1/models to list all available models.
+        quality_preset : typing.Optional[str]
+            Output quality of the generated audio. Must be one of:
+            standard - standard output format, 128kbps with 44.1kHz sample rate.
+            high - high quality output format, 192kbps with 44.1kHz sample rate and major improvements on our side. Using this setting increases the character cost by 20%.
+            ultra - ultra quality output format, 192kbps with 44.1kHz sample rate and highest improvements on our side. Using this setting increases the character cost by 50%.
+            ultra lossless - ultra quality output format, 705.6kbps with 44.1kHz sample rate and highest improvements on our side in a fully lossless format. Using this setting increases the character cost by 100%.
 
-            - quality_preset: typing.Optional[str]. Output quality of the generated audio. Must be one of:
-                                                    standard - standard output format, 128kbps with 44.1kHz sample rate.
-                                                    high - high quality output format, 192kbps with 44.1kHz sample rate and major improvements on our side. Using this setting increases the character cost by 20%.
-                                                    ultra - ultra quality output format, 192kbps with 44.1kHz sample rate and highest improvements on our side. Using this setting increases the character cost by 50%.
-                                                    ultra lossless - ultra quality output format, 705.6kbps with 44.1kHz sample rate and highest improvements on our side in a fully lossless format. Using this setting increases the character cost by 100%.
 
-            - title: typing.Optional[str]. An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
+        title : typing.Optional[str]
+            An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - author: typing.Optional[str]. An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
+        author : typing.Optional[str]
+            An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - isbn_number: typing.Optional[str]. An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
+        isbn_number : typing.Optional[str]
+            An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - acx_volume_normalization: typing.Optional[bool]. [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
+        acx_volume_normalization : typing.Optional[bool]
+            [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - volume_normalization: typing.Optional[bool]. When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
+        volume_normalization : typing.Optional[bool]
+            When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.List[str]]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+        pronunciation_dictionary_locators : typing.Optional[typing.List[str]]
+            A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
 
-            - callback_url: typing.Optional[str]. A url that will be called by our service when the project is converted with a json containing the status of the conversion
+        callback_url : typing.Optional[str]
+            A url that will be called by our service when the project is converted with a json containing the status of the conversion
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddProjectResponseModel
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.add(
             name="name",
@@ -219,19 +252,29 @@
 
     def get(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ProjectExtendedResponseModel:
         """
         Returns information about a specific project. This endpoint returns more detailed information about a project than GET api.elevenlabs.io/v1/projects.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProjectExtendedResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.get(
             project_id="project_id",
@@ -271,19 +314,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a project by its project_id.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.delete(
             project_id="project_id",
@@ -323,19 +376,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Starts conversion of a project and all of its chapters.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.convert(
             project_id="project_id",
@@ -380,19 +443,29 @@
 
     def get_snapshots(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ProjectSnapshotsResponse:
         """
         Gets the snapshots of a project.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProjectSnapshotsResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.get_snapshots(
             project_id="project_id",
@@ -439,23 +512,35 @@
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
         Stream the audio from a project snapshot.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        project_snapshot_id : str
+            The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+
+        convert_to_mpeg : typing.Optional[bool]
+            Whether to convert the audio to mpeg format.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
 
-            - convert_to_mpeg: typing.Optional[bool]. Whether to convert the audio to mpeg format.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.stream_audio(
             project_id="string",
@@ -512,21 +597,31 @@
 
     def stream_archive(
         self, project_id: str, project_snapshot_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Streams archive with project audio.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        project_snapshot_id : str
+            The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.stream_archive(
             project_id="project_id",
@@ -577,21 +672,32 @@
         *,
         pronunciation_dictionary_locators: typing.Sequence[PronunciationDictionaryVersionLocator],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Updates the set of pronunciation dictionaries acting on a project. This will automatically mark text within this project as requiring reconverting where the new dictionary would apply or the old one no longer does.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - pronunciation_dictionary_locators: typing.Sequence[PronunciationDictionaryVersionLocator]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        pronunciation_dictionary_locators : typing.Sequence[PronunciationDictionaryVersionLocator]
+            A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs import PronunciationDictionaryVersionLocator
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.update_pronunciation_dictionaries(
@@ -650,17 +756,26 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetProjectsResponse:
         """
         Returns a list of your projects together and its metadata.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetProjectsResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.get_all()
         """
@@ -696,67 +811,91 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add(
         self,
         *,
         name: str,
-        from_url: typing.Optional[str] = None,
-        from_document: typing.Optional[core.File] = None,
         default_title_voice_id: str,
         default_paragraph_voice_id: str,
         default_model_id: str,
+        from_url: typing.Optional[str] = None,
+        from_document: typing.Optional[core.File] = None,
         quality_preset: typing.Optional[str] = None,
         title: typing.Optional[str] = None,
         author: typing.Optional[str] = None,
         isbn_number: typing.Optional[str] = None,
         acx_volume_normalization: typing.Optional[bool] = None,
         volume_normalization: typing.Optional[bool] = None,
         pronunciation_dictionary_locators: typing.Optional[typing.List[str]] = None,
         callback_url: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddProjectResponseModel:
         """
         Creates a new project, it can be either initialized as blank, from a document or from a URL.
 
-        Parameters:
-            - name: str. The name of the project, used for identification only.
+        Parameters
+        ----------
+        name : str
+            The name of the project, used for identification only.
+
+        default_title_voice_id : str
+            The voice_id that corresponds to the default voice used for new titles.
 
-            - from_url: typing.Optional[str]. An optional URL from which we will extract content to initialize the project. If this is set, 'from_url' must be null. If neither 'from_url' or 'from_document' are provided we will initialize the project as blank.
+        default_paragraph_voice_id : str
+            The voice_id that corresponds to the default voice used for new paragraphs.
 
-            - from_document: typing.Optional[core.File]. See core.File for more documentation
+        default_model_id : str
+            The model_id of the model to be used for this project, you can query GET https://api.elevenlabs.io/v1/models to list all available models.
 
-            - default_title_voice_id: str. The voice_id that corresponds to the default voice used for new titles.
+        from_url : typing.Optional[str]
+            An optional URL from which we will extract content to initialize the project. If this is set, 'from_url' must be null. If neither 'from_url' or 'from_document' are provided we will initialize the project as blank.
 
-            - default_paragraph_voice_id: str. The voice_id that corresponds to the default voice used for new paragraphs.
+        from_document : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - default_model_id: str. The model_id of the model to be used for this project, you can query GET https://api.elevenlabs.io/v1/models to list all available models.
+        quality_preset : typing.Optional[str]
+            Output quality of the generated audio. Must be one of:
+            standard - standard output format, 128kbps with 44.1kHz sample rate.
+            high - high quality output format, 192kbps with 44.1kHz sample rate and major improvements on our side. Using this setting increases the character cost by 20%.
+            ultra - ultra quality output format, 192kbps with 44.1kHz sample rate and highest improvements on our side. Using this setting increases the character cost by 50%.
+            ultra lossless - ultra quality output format, 705.6kbps with 44.1kHz sample rate and highest improvements on our side in a fully lossless format. Using this setting increases the character cost by 100%.
 
-            - quality_preset: typing.Optional[str]. Output quality of the generated audio. Must be one of:
-                                                    standard - standard output format, 128kbps with 44.1kHz sample rate.
-                                                    high - high quality output format, 192kbps with 44.1kHz sample rate and major improvements on our side. Using this setting increases the character cost by 20%.
-                                                    ultra - ultra quality output format, 192kbps with 44.1kHz sample rate and highest improvements on our side. Using this setting increases the character cost by 50%.
-                                                    ultra lossless - ultra quality output format, 705.6kbps with 44.1kHz sample rate and highest improvements on our side in a fully lossless format. Using this setting increases the character cost by 100%.
 
-            - title: typing.Optional[str]. An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
+        title : typing.Optional[str]
+            An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - author: typing.Optional[str]. An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
+        author : typing.Optional[str]
+            An optional name of the author of the project, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - isbn_number: typing.Optional[str]. An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
+        isbn_number : typing.Optional[str]
+            An optional ISBN number of the project you want to create, this will be added as metadata to the mp3 file on project / chapter download.
 
-            - acx_volume_normalization: typing.Optional[bool]. [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
+        acx_volume_normalization : typing.Optional[bool]
+            [Deprecated] When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - volume_normalization: typing.Optional[bool]. When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
+        volume_normalization : typing.Optional[bool]
+            When the project is downloaded, should the returned audio have postprocessing in order to make it compliant with audiobook normalized volume requirements
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.List[str]]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+        pronunciation_dictionary_locators : typing.Optional[typing.List[str]]
+            A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
 
-            - callback_url: typing.Optional[str]. A url that will be called by our service when the project is converted with a json containing the status of the conversion
+        callback_url : typing.Optional[str]
+            A url that will be called by our service when the project is converted with a json containing the status of the conversion
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddProjectResponseModel
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.add(
             name="name",
@@ -842,19 +981,29 @@
 
     async def get(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ProjectExtendedResponseModel:
         """
         Returns information about a specific project. This endpoint returns more detailed information about a project than GET api.elevenlabs.io/v1/projects.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProjectExtendedResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.get(
             project_id="project_id",
@@ -894,19 +1043,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a project by its project_id.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.delete(
             project_id="project_id",
@@ -946,19 +1105,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Starts conversion of a project and all of its chapters.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.convert(
             project_id="project_id",
@@ -1003,19 +1172,29 @@
 
     async def get_snapshots(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ProjectSnapshotsResponse:
         """
         Gets the snapshots of a project.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ProjectSnapshotsResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.get_snapshots(
             project_id="project_id",
@@ -1062,23 +1241,35 @@
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
         Stream the audio from a project snapshot.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        project_snapshot_id : str
+            The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+
+        convert_to_mpeg : typing.Optional[bool]
+            Whether to convert the audio to mpeg format.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
 
-            - convert_to_mpeg: typing.Optional[bool]. Whether to convert the audio to mpeg format.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.stream_audio(
             project_id="string",
@@ -1135,21 +1326,31 @@
 
     async def stream_archive(
         self, project_id: str, project_snapshot_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Streams archive with project audio.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        project_snapshot_id : str
+            The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.stream_archive(
             project_id="project_id",
@@ -1200,21 +1401,32 @@
         *,
         pronunciation_dictionary_locators: typing.Sequence[PronunciationDictionaryVersionLocator],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Updates the set of pronunciation dictionaries acting on a project. This will automatically mark text within this project as requiring reconverting where the new dictionary would apply or the old one no longer does.
 
-        Parameters:
-            - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
-
-            - pronunciation_dictionary_locators: typing.Sequence[PronunciationDictionaryVersionLocator]. A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+        Parameters
+        ----------
+        project_id : str
+            The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
+
+        pronunciation_dictionary_locators : typing.Sequence[PronunciationDictionaryVersionLocator]
+            A list of pronunciation dictionary locators (id, version_id) encoded as a list of JSON strings for pronunciation dictionaries to be applied to the text.  A list of json encoded strings is required as adding projects may occur through formData as opposed to jsonBody
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs import PronunciationDictionaryVersionLocator
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.update_pronunciation_dictionaries(
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/client.py` & `elevenlabs-1.2.2/src/elevenlabs/pronunciation_dictionary/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,31 +29,43 @@
 class PronunciationDictionaryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def add_from_file(
         self,
         *,
-        file: typing.Optional[core.File] = None,
         name: str,
+        file: typing.Optional[core.File] = None,
         description: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryResponseModel:
         """
         Creates a new pronunciation dictionary from a lexicon .PLS file
 
-        Parameters:
-            - file: typing.Optional[core.File]. See core.File for more documentation
-
-            - name: str. The name of the pronunciation dictionary, used for identification only.
+        Parameters
+        ----------
+        name : str
+            The name of the pronunciation dictionary, used for identification only.
+
+        file : typing.Optional[core.File]
+            See core.File for more documentation
+
+        description : typing.Optional[str]
+            A description of the pronunciation dictionary, used for identification only.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddPronunciationDictionaryResponseModel
+            Successful Response
 
-            - description: typing.Optional[str]. A description of the pronunciation dictionary, used for identification only.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.add_from_file(
             name="name",
@@ -106,22 +118,34 @@
         *,
         rules: typing.Sequence[PronunciationDictionaryRule],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryRulesResponseModel:
         """
         Add rules to the pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        rules : typing.Sequence[PronunciationDictionaryRule]
+            List of pronunciation rules. Rule can be either:
+                an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
+                or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddPronunciationDictionaryRulesResponseModel
+            Successful Response
 
-            - rules: typing.Sequence[PronunciationDictionaryRule]. List of pronunciation rules. Rule can be either:
-                                                                       an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
-                                                                       or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.add_rules_to_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
@@ -175,21 +199,32 @@
         *,
         rule_strings: typing.Sequence[str],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RemovePronunciationDictionaryRulesResponseModel:
         """
         Remove rules from the pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
-
-            - rule_strings: typing.Sequence[str]. List of strings to remove from the pronunciation dictionary.
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        rule_strings : typing.Sequence[str]
+            List of strings to remove from the pronunciation dictionary.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RemovePronunciationDictionaryRulesResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.remove_rules_from_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
@@ -233,35 +268,46 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_pls_file_with_a_pronunciation_dictionary_version_rules(
+    def download(
         self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> str:
         """
         Get PLS file with a pronunciation dictionary version rules
 
-        Parameters:
-            - dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        dictionary_id : str
+            The id of the pronunciation dictionary
+
+        version_id : str
+            The id of the version of the pronunciation dictionary
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        str
+            Successful Response
 
-            - version_id: str. The id of the version of the pronunciation dictionary
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
-            dictionary_id="string",
-            version_id="string",
+        client.pronunciation_dictionary.download(
+            dictionary_id="Fm6AvNgS53NXe6Kqxp3e",
+            version_id="KZFyRUq3R6kaqhKI146w",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
@@ -297,26 +343,36 @@
 
     def get(
         self, pronunciation_dictionary_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetPronunciationDictionaryMetadataResponse:
         """
         Get metadata for a pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetPronunciationDictionaryMetadataResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.pronunciation_dictionary.get(
-            pronunciation_dictionary_id="pronunciation_dictionary_id",
+            pronunciation_dictionary_id="Fm6AvNgS53NXe6Kqxp3e",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/",
@@ -356,27 +412,40 @@
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetPronunciationDictionariesMetadataResponseModel:
         """
         Get a list of the pronunciation dictionaries you have access to and their metadata
 
-        Parameters:
-            - cursor: typing.Optional[str]. Used for fetching next page. Cursor is returned in the response.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            Used for fetching next page. Cursor is returned in the response.
+
+        page_size : typing.Optional[int]
+            How many pronunciation dictionaries to return at maximum. Can not exceed 100, defaults to 30.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetPronunciationDictionariesMetadataResponseModel
+            Successful Response
 
-            - page_size: typing.Optional[int]. How many pronunciation dictionaries to return at maximum. Can not exceed 100, defaults to 30.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.pronunciation_dictionary.get_all()
+        client.pronunciation_dictionary.get_all(
+            page_size=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -420,31 +489,43 @@
 class AsyncPronunciationDictionaryClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def add_from_file(
         self,
         *,
-        file: typing.Optional[core.File] = None,
         name: str,
+        file: typing.Optional[core.File] = None,
         description: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryResponseModel:
         """
         Creates a new pronunciation dictionary from a lexicon .PLS file
 
-        Parameters:
-            - file: typing.Optional[core.File]. See core.File for more documentation
-
-            - name: str. The name of the pronunciation dictionary, used for identification only.
+        Parameters
+        ----------
+        name : str
+            The name of the pronunciation dictionary, used for identification only.
+
+        file : typing.Optional[core.File]
+            See core.File for more documentation
+
+        description : typing.Optional[str]
+            A description of the pronunciation dictionary, used for identification only.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddPronunciationDictionaryResponseModel
+            Successful Response
 
-            - description: typing.Optional[str]. A description of the pronunciation dictionary, used for identification only.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.add_from_file(
             name="name",
@@ -497,22 +578,34 @@
         *,
         rules: typing.Sequence[PronunciationDictionaryRule],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddPronunciationDictionaryRulesResponseModel:
         """
         Add rules to the pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        rules : typing.Sequence[PronunciationDictionaryRule]
+            List of pronunciation rules. Rule can be either:
+                an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
+                or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddPronunciationDictionaryRulesResponseModel
+            Successful Response
 
-            - rules: typing.Sequence[PronunciationDictionaryRule]. List of pronunciation rules. Rule can be either:
-                                                                       an alias rule: {'string_to_replace': 'a', 'type': 'alias', 'alias': 'b', }
-                                                                       or a phoneme rule: {'string_to_replace': 'a', 'type': 'phoneme', 'phoneme': 'b', 'alphabet': 'ipa' }
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.add_rules_to_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
@@ -566,21 +659,32 @@
         *,
         rule_strings: typing.Sequence[str],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RemovePronunciationDictionaryRulesResponseModel:
         """
         Remove rules from the pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
-
-            - rule_strings: typing.Sequence[str]. List of strings to remove from the pronunciation dictionary.
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        rule_strings : typing.Sequence[str]
+            List of strings to remove from the pronunciation dictionary.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RemovePronunciationDictionaryRulesResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.remove_rules_from_the_pronunciation_dictionary(
             pronunciation_dictionary_id="pronunciation_dictionary_id",
@@ -624,35 +728,46 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_pls_file_with_a_pronunciation_dictionary_version_rules(
+    async def download(
         self, dictionary_id: str, version_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> str:
         """
         Get PLS file with a pronunciation dictionary version rules
 
-        Parameters:
-            - dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        dictionary_id : str
+            The id of the pronunciation dictionary
+
+        version_id : str
+            The id of the version of the pronunciation dictionary
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        str
+            Successful Response
 
-            - version_id: str. The id of the version of the pronunciation dictionary
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.pronunciation_dictionary.get_pls_file_with_a_pronunciation_dictionary_version_rules(
-            dictionary_id="string",
-            version_id="string",
+        await client.pronunciation_dictionary.download(
+            dictionary_id="Fm6AvNgS53NXe6Kqxp3e",
+            version_id="KZFyRUq3R6kaqhKI146w",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(dictionary_id)}/{jsonable_encoder(version_id)}/download",
@@ -688,26 +803,36 @@
 
     async def get(
         self, pronunciation_dictionary_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetPronunciationDictionaryMetadataResponse:
         """
         Get metadata for a pronunciation dictionary
 
-        Parameters:
-            - pronunciation_dictionary_id: str. The id of the pronunciation dictionary
+        Parameters
+        ----------
+        pronunciation_dictionary_id : str
+            The id of the pronunciation dictionary
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetPronunciationDictionaryMetadataResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.pronunciation_dictionary.get(
-            pronunciation_dictionary_id="pronunciation_dictionary_id",
+            pronunciation_dictionary_id="Fm6AvNgS53NXe6Kqxp3e",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/pronunciation-dictionaries/{jsonable_encoder(pronunciation_dictionary_id)}/",
@@ -747,27 +872,40 @@
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetPronunciationDictionariesMetadataResponseModel:
         """
         Get a list of the pronunciation dictionaries you have access to and their metadata
 
-        Parameters:
-            - cursor: typing.Optional[str]. Used for fetching next page. Cursor is returned in the response.
+        Parameters
+        ----------
+        cursor : typing.Optional[str]
+            Used for fetching next page. Cursor is returned in the response.
+
+        page_size : typing.Optional[int]
+            How many pronunciation dictionaries to return at maximum. Can not exceed 100, defaults to 30.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetPronunciationDictionariesMetadataResponseModel
+            Successful Response
 
-            - page_size: typing.Optional[int]. How many pronunciation dictionaries to return at maximum. Can not exceed 100, defaults to 30.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.pronunciation_dictionary.get_all()
+        await client.pronunciation_dictionary.get_all(
+            page_size=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/pronunciation-dictionaries/"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.2.2/src/elevenlabs/realtime_tts.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,40 +93,44 @@
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             )
         ) as socket:
-            socket.send(json.dumps(
-                dict(
-                    text=" ",
-                    try_trigger_generation=True,
-                    voice_settings=voice_settings.dict() if voice_settings else None,
-                    generation_config=dict(
-                        chunk_length_schedule=[50],
-                    ),
-                )
-            ))
+            try:
+                socket.send(json.dumps(
+                    dict(
+                        text=" ",
+                        try_trigger_generation=True,
+                        voice_settings=voice_settings.dict() if voice_settings else None,
+                        generation_config=dict(
+                            chunk_length_schedule=[50],
+                        ),
+                    )
+                ))
+            except websockets.exceptions.ConnectionClosedError as ce:
+                raise ApiError(body=ce.reason, status_code=ce.code)
 
-            for text_chunk in text_chunker(text):
-                data = dict(text=text_chunk, try_trigger_generation=True)
-                socket.send(json.dumps(data))
-                try:
-                    data = json.loads(socket.recv(1e-4))
-                    if "audio" in data and data["audio"]:
-                        yield base64.b64decode(data["audio"])  # type: ignore
-                except TimeoutError:
-                    pass
-            
-            socket.send(json.dumps(dict(text="")))
+            try:
+                for text_chunk in text_chunker(text):
+                    data = dict(text=text_chunk, try_trigger_generation=True)
+                    socket.send(json.dumps(data))
+                    try:
+                        data = json.loads(socket.recv(1e-4))
+                        if "audio" in data and data["audio"]:
+                            yield base64.b64decode(data["audio"])  # type: ignore
+                    except TimeoutError:
+                        pass
 
-            while True:
-                try:
-                    data = json.loads(socket.recv())                   
+                socket.send(json.dumps(dict(text="")))
+
+                while True:
+
+                    data = json.loads(socket.recv())
                     if "audio" in data and data["audio"]:
                         yield base64.b64decode(data["audio"])  # type: ignore
-                except websockets.exceptions.ConnectionClosed:
-                    if "message" in data:
-                        raise ApiError(body=data)
-                    break
-
+            except websockets.exceptions.ConnectionClosed as ce:
+                if "message" in data:
+                    raise ApiError(body=data, status_code=ce.code)
+                elif ce.code != 1000:
+                    raise ApiError(body=ce.reason, status_code=ce.code)
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/samples/client.py` & `elevenlabs-1.2.2/src/elevenlabs/samples/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,29 +20,40 @@
 
     def delete(
         self, voice_id: str, sample_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Removes a sample by its ID.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        sample_id : str
+            Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - sample_id: str. Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.samples.delete(
-            voice_id="voice_id",
-            sample_id="sample_id",
+            voice_id="ja9xsmfGhxYcymxGcOGB",
+            sample_id="pMsXgVXv3BLzUgSXRplE",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}",
@@ -78,29 +89,39 @@
 
     def get_audio(
         self, voice_id: str, sample_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Returns the audio corresponding to a sample attached to a voice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - sample_id: str. Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        sample_id : str
+            Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.samples.get_audio(
-            voice_id="voice_id",
-            sample_id="sample_id",
+            voice_id="ja9xsmfGhxYcymxGcOGB",
+            sample_id="pMsXgVXv3BLzUgSXRplE",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}/audio",
@@ -141,29 +162,40 @@
 
     async def delete(
         self, voice_id: str, sample_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Removes a sample by its ID.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        sample_id : str
+            Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - sample_id: str. Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.samples.delete(
-            voice_id="voice_id",
-            sample_id="sample_id",
+            voice_id="ja9xsmfGhxYcymxGcOGB",
+            sample_id="pMsXgVXv3BLzUgSXRplE",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}",
@@ -199,29 +231,39 @@
 
     async def get_audio(
         self, voice_id: str, sample_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Returns the audio corresponding to a sample attached to a voice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - sample_id: str. Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        sample_id : str
+            Sample ID to be used, you can use GET https://api.elevenlabs.io/v1/voices/{voice_id} to list all the available samples for a voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.samples.get_audio(
-            voice_id="voice_id",
-            sample_id="sample_id",
+            voice_id="ja9xsmfGhxYcymxGcOGB",
+            sample_id="pMsXgVXv3BLzUgSXRplE",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/{jsonable_encoder(voice_id)}/samples/{jsonable_encoder(sample_id)}/audio",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.2.2/src/elevenlabs/text_to_speech/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,133 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
+from ..types.optimize_streaming_latency import OptimizeStreamingLatency
+from ..types.output_format import OutputFormat
+from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
+from ..types.voice_settings import VoiceSettings
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class SpeechToSpeechClient:
+class TextToSpeechClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def convert(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        output_format: typing.Optional[str] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        text: str,
+        optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
+        output_format: typing.Optional[OutputFormat] = None,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
+        Converts text into speech using a voice of your choice and returns audio.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
-
-                                                                Defaults to 0.
-            - output_format: typing.Optional[str]. Output format of the generated audio. Must be one of:
-                                                   mp3_22050_32 - output format, mp3 with 22.05kHz sample rate at 32kbps.
-                                                   mp3_44100_32 - output format, mp3 with 44.1kHz sample rate at 32kbps.
-                                                   mp3_44100_64 - output format, mp3 with 44.1kHz sample rate at 64kbps.
-                                                   mp3_44100_96 - output format, mp3 with 44.1kHz sample rate at 96kbps.
-                                                   mp3_44100_128 - default output format, mp3 with 44.1kHz sample rate at 128kbps.
-                                                   mp3_44100_192 - output format, mp3 with 44.1kHz sample rate at 192kbps. Requires you to be subscribed to Creator tier or above.
-                                                   pcm_16000 - PCM format (S16LE) with 16kHz sample rate.
-                                                   pcm_22050 - PCM format (S16LE) with 22.05kHz sample rate.
-                                                   pcm_24000 - PCM format (S16LE) with 24kHz sample rate.
-                                                   pcm_44100 - PCM format (S16LE) with 44.1kHz sample rate. Requires you to be subscribed to Pro tier or above.
-                                                   ulaw_8000 - μ-law format (sometimes written mu-law, often approximated as u-law) with 8kHz sample rate. Note that this format is commonly used for Twilio audio inputs.
-            - audio: core.File. See core.File for more documentation
+        text : str
+            The text that will get converted into speech.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+        voice_settings : typing.Optional[VoiceSettings]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+        pronunciation_dictionary_locators : typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]
+            A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
+
+        Examples
+        --------
+        from elevenlabs import VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.speech_to_speech.convert(
-            voice_id="string",
-            optimize_streaming_latency=1,
-            output_format="string",
+        client.text_to_speech.convert(
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
+            voice_settings=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -132,91 +153,109 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert_as_stream(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        output_format: typing.Optional[str] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        text: str,
+        optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
+        output_format: typing.Optional[OutputFormat] = None,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
+        Converts text into speech using a voice of your choice and returns audio as an audio stream.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
-
-                                                                Defaults to 0.
-            - output_format: typing.Optional[str]. Output format of the generated audio. Must be one of:
-                                                   mp3_22050_32 - output format, mp3 with 22.05kHz sample rate at 32kbps.
-                                                   mp3_44100_32 - output format, mp3 with 44.1kHz sample rate at 32kbps.
-                                                   mp3_44100_64 - output format, mp3 with 44.1kHz sample rate at 64kbps.
-                                                   mp3_44100_96 - output format, mp3 with 44.1kHz sample rate at 96kbps.
-                                                   mp3_44100_128 - default output format, mp3 with 44.1kHz sample rate at 128kbps.
-                                                   mp3_44100_192 - output format, mp3 with 44.1kHz sample rate at 192kbps. Requires you to be subscribed to Creator tier or above.
-                                                   pcm_16000 - PCM format (S16LE) with 16kHz sample rate.
-                                                   pcm_22050 - PCM format (S16LE) with 22.05kHz sample rate.
-                                                   pcm_24000 - PCM format (S16LE) with 24kHz sample rate.
-                                                   pcm_44100 - PCM format (S16LE) with 44.1kHz sample rate. Requires you to be subscribed to Pro tier or above.
-                                                   ulaw_8000 - μ-law format (sometimes written mu-law, often approximated as u-law) with 8kHz sample rate. Note that this format is commonly used for Twilio audio inputs.
-            - audio: core.File. See core.File for more documentation
+        text : str
+            The text that will get converted into speech.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+        voice_settings : typing.Optional[VoiceSettings]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+        pronunciation_dictionary_locators : typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]
+            A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
+
+        Examples
+        --------
+        from elevenlabs import VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.speech_to_speech.convert_as_stream(
-            voice_id="string",
-            optimize_streaming_latency=1,
-            output_format="string",
+        client.text_to_speech.convert_as_stream(
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
+            voice_settings=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -239,99 +278,117 @@
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncSpeechToSpeechClient:
+class AsyncTextToSpeechClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def convert(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        output_format: typing.Optional[str] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        text: str,
+        optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
+        output_format: typing.Optional[OutputFormat] = None,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
+        Converts text into speech using a voice of your choice and returns audio.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
-
-                                                                Defaults to 0.
-            - output_format: typing.Optional[str]. Output format of the generated audio. Must be one of:
-                                                   mp3_22050_32 - output format, mp3 with 22.05kHz sample rate at 32kbps.
-                                                   mp3_44100_32 - output format, mp3 with 44.1kHz sample rate at 32kbps.
-                                                   mp3_44100_64 - output format, mp3 with 44.1kHz sample rate at 64kbps.
-                                                   mp3_44100_96 - output format, mp3 with 44.1kHz sample rate at 96kbps.
-                                                   mp3_44100_128 - default output format, mp3 with 44.1kHz sample rate at 128kbps.
-                                                   mp3_44100_192 - output format, mp3 with 44.1kHz sample rate at 192kbps. Requires you to be subscribed to Creator tier or above.
-                                                   pcm_16000 - PCM format (S16LE) with 16kHz sample rate.
-                                                   pcm_22050 - PCM format (S16LE) with 22.05kHz sample rate.
-                                                   pcm_24000 - PCM format (S16LE) with 24kHz sample rate.
-                                                   pcm_44100 - PCM format (S16LE) with 44.1kHz sample rate. Requires you to be subscribed to Pro tier or above.
-                                                   ulaw_8000 - μ-law format (sometimes written mu-law, often approximated as u-law) with 8kHz sample rate. Note that this format is commonly used for Twilio audio inputs.
-            - audio: core.File. See core.File for more documentation
+        text : str
+            The text that will get converted into speech.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+        voice_settings : typing.Optional[VoiceSettings]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+        pronunciation_dictionary_locators : typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]
+            A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
+
+        Examples
+        --------
+        from elevenlabs import VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.speech_to_speech.convert(
-            voice_id="string",
-            optimize_streaming_latency=1,
-            output_format="string",
+        await client.text_to_speech.convert(
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
+            voice_settings=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -357,91 +414,109 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert_as_stream(
         self,
         voice_id: str,
         *,
-        optimize_streaming_latency: typing.Optional[int] = None,
-        output_format: typing.Optional[str] = None,
-        audio: core.File,
-        model_id: typing.Optional[str] = None,
-        voice_settings: typing.Optional[str] = None,
+        text: str,
+        optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
+        output_format: typing.Optional[OutputFormat] = None,
+        model_id: typing.Optional[str] = OMIT,
+        voice_settings: typing.Optional[VoiceSettings] = OMIT,
+        pronunciation_dictionary_locators: typing.Optional[
+            typing.Sequence[PronunciationDictionaryVersionLocator]
+        ] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
+        Converts text into speech using a voice of your choice and returns audio as an audio stream.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[int]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model. Possible values:
-                                                                0 - default mode (no latency optimizations)
-                                                                1 - normal latency optimizations (about 50% of possible latency improvement of option 3)
-                                                                2 - strong latency optimizations (about 75% of possible latency improvement of option 3)
-                                                                3 - max latency optimizations
-                                                                4 - max latency optimizations, but also with text normalizer turned off for even more latency savings (best latency, but can mispronounce eg numbers and dates).
-
-                                                                Defaults to 0.
-            - output_format: typing.Optional[str]. Output format of the generated audio. Must be one of:
-                                                   mp3_22050_32 - output format, mp3 with 22.05kHz sample rate at 32kbps.
-                                                   mp3_44100_32 - output format, mp3 with 44.1kHz sample rate at 32kbps.
-                                                   mp3_44100_64 - output format, mp3 with 44.1kHz sample rate at 64kbps.
-                                                   mp3_44100_96 - output format, mp3 with 44.1kHz sample rate at 96kbps.
-                                                   mp3_44100_128 - default output format, mp3 with 44.1kHz sample rate at 128kbps.
-                                                   mp3_44100_192 - output format, mp3 with 44.1kHz sample rate at 192kbps. Requires you to be subscribed to Creator tier or above.
-                                                   pcm_16000 - PCM format (S16LE) with 16kHz sample rate.
-                                                   pcm_22050 - PCM format (S16LE) with 22.05kHz sample rate.
-                                                   pcm_24000 - PCM format (S16LE) with 24kHz sample rate.
-                                                   pcm_44100 - PCM format (S16LE) with 44.1kHz sample rate. Requires you to be subscribed to Pro tier or above.
-                                                   ulaw_8000 - μ-law format (sometimes written mu-law, often approximated as u-law) with 8kHz sample rate. Note that this format is commonly used for Twilio audio inputs.
-            - audio: core.File. See core.File for more documentation
+        text : str
+            The text that will get converted into speech.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - voice_settings: typing.Optional[str]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+
+        voice_settings : typing.Optional[VoiceSettings]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+
+        pronunciation_dictionary_locators : typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]
+            A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
+
+        Examples
+        --------
+        from elevenlabs import VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.speech_to_speech.convert_as_stream(
-            voice_id="string",
-            optimize_streaming_latency=1,
-            output_format="string",
+        await client.text_to_speech.convert_as_stream(
+            voice_id="pMsXgVXv3BLzUgSXRplE",
+            optimize_streaming_latency="0",
+            output_format="mp3_22050_32",
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
+            voice_settings=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"text": text}
+        if model_id is not OMIT:
+            _request["model_id"] = model_id
+        if voice_settings is not OMIT:
+            _request["voice_settings"] = voice_settings
+        if pronunciation_dictionary_locators is not OMIT:
+            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.2.2/src/elevenlabs/speech_to_speech/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,113 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
+from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.optimize_streaming_latency import OptimizeStreamingLatency
 from ..types.output_format import OutputFormat
-from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
-from ..types.voice_settings import VoiceSettings
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class TextToSpeechClient:
+class SpeechToSpeechClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def convert(
         self,
         voice_id: str,
         *,
+        audio: core.File,
         optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
         output_format: typing.Optional[OutputFormat] = None,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        model_id: typing.Optional[str] = None,
+        voice_settings: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio.
+        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+        audio : core.File
+            See core.File for more documentation
 
-            - output_format: typing.Optional[OutputFormat]. The output format of the generated audio.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - text: str. The text that will get converted into speech.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
 
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+        voice_settings : typing.Optional[str]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.text_to_speech.convert(
+        client.speech_to_speech.convert(
             voice_id="string",
             optimize_streaming_latency="0",
             output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            json=jsonable_encoder(_request)
+            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
+            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -145,101 +133,90 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert_as_stream(
         self,
         voice_id: str,
         *,
+        audio: core.File,
         optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
         output_format: typing.Optional[OutputFormat] = None,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        model_id: typing.Optional[str] = None,
+        voice_settings: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio as an audio stream.
+        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+        audio : core.File
+            See core.File for more documentation
 
-            - output_format: typing.Optional[OutputFormat]. The output format of the generated audio.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - text: str. The text that will get converted into speech.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
 
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+        voice_settings : typing.Optional[str]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.text_to_speech.convert_as_stream(
+        client.speech_to_speech.convert_as_stream(
             voice_id="string",
             optimize_streaming_latency="0",
             output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            json=jsonable_encoder(_request)
+            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
+            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -262,109 +239,98 @@
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTextToSpeechClient:
+class AsyncSpeechToSpeechClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def convert(
         self,
         voice_id: str,
         *,
+        audio: core.File,
         optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
         output_format: typing.Optional[OutputFormat] = None,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        model_id: typing.Optional[str] = None,
+        voice_settings: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio.
+        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+        audio : core.File
+            See core.File for more documentation
 
-            - output_format: typing.Optional[OutputFormat]. The output format of the generated audio.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - text: str. The text that will get converted into speech.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
 
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+        voice_settings : typing.Optional[str]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.text_to_speech.convert(
+        await client.speech_to_speech.convert(
             voice_id="string",
             optimize_streaming_latency="0",
             output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            json=jsonable_encoder(_request)
+            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
+            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -390,101 +356,90 @@
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert_as_stream(
         self,
         voice_id: str,
         *,
+        audio: core.File,
         optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency] = None,
         output_format: typing.Optional[OutputFormat] = None,
-        text: str,
-        model_id: typing.Optional[str] = OMIT,
-        voice_settings: typing.Optional[VoiceSettings] = OMIT,
-        pronunciation_dictionary_locators: typing.Optional[
-            typing.Sequence[PronunciationDictionaryVersionLocator]
-        ] = OMIT,
+        model_id: typing.Optional[str] = None,
+        voice_settings: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
-        Converts text into speech using a voice of your choice and returns audio as an audio stream.
+        Create speech by combining the content and emotion of the uploaded audio with a voice of your choice and returns an audio stream.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - optimize_streaming_latency: typing.Optional[OptimizeStreamingLatency]. You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
+        audio : core.File
+            See core.File for more documentation
 
-            - output_format: typing.Optional[OutputFormat]. The output format of the generated audio.
+        optimize_streaming_latency : typing.Optional[OptimizeStreamingLatency]
+            You can turn on latency optimizations at some cost of quality. The best possible final latency varies by model.
 
-            - text: str. The text that will get converted into speech.
+        output_format : typing.Optional[OutputFormat]
+            The output format of the generated audio.
 
-            - model_id: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for text to speech, you can check this using the can_do_text_to_speech property.
+        model_id : typing.Optional[str]
+            Identifier of the model that will be used, you can query them using GET /v1/models. The model needs to have support for speech to speech, you can check this using the can_do_voice_conversion property.
 
-            - voice_settings: typing.Optional[VoiceSettings]. Voice settings overriding stored setttings for the given voice. They are applied only on the given request.
+        voice_settings : typing.Optional[str]
+            Voice settings overriding stored setttings for the given voice. They are applied only on the given request. Needs to be send as a JSON encoded string.
 
-            - pronunciation_dictionary_locators: typing.Optional[typing.Sequence[PronunciationDictionaryVersionLocator]]. A list of pronunciation dictionary locators (id, version_id) to be applied to the text. They will be applied in order. You may have up to 3 locators per request
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from elevenlabs import PronunciationDictionaryVersionLocator, VoiceSettings
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.text_to_speech.convert_as_stream(
+        await client.speech_to_speech.convert_as_stream(
             voice_id="string",
             optimize_streaming_latency="0",
             output_format="mp3_22050_32",
-            text="string",
-            model_id="string",
-            voice_settings=VoiceSettings(
-                stability=1.1,
-                similarity_boost=1.1,
-                style=1.1,
-                use_speaker_boost=True,
-            ),
-            pronunciation_dictionary_locators=[
-                PronunciationDictionaryVersionLocator(
-                    pronunciation_dictionary_id="string",
-                    version_id="string",
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text": text}
-        if model_id is not OMIT:
-            _request["model_id"] = model_id
-        if voice_settings is not OMIT:
-            _request["voice_settings"] = voice_settings
-        if pronunciation_dictionary_locators is not OMIT:
-            _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
         async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/speech-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "optimize_streaming_latency": optimize_streaming_latency,
                         "output_format": output_format,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
             ),
-            json=jsonable_encoder(_request)
+            data=jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder(remove_none_from_dict({"model_id": model_id, "voice_settings": voice_settings})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
+            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"audio": audio})),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/__init__.py` & `elevenlabs-1.2.2/src/elevenlabs/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .audio_output import AudioOutput
 from .category import Category
 from .chapter_response import ChapterResponse
 from .chapter_snapshot_response import ChapterSnapshotResponse
 from .chapter_snapshots_response import ChapterSnapshotsResponse
 from .chapter_state import ChapterState
 from .chapter_statistics_response import ChapterStatisticsResponse
+from .close_connection import CloseConnection
 from .currency import Currency
 from .do_dubbing_response import DoDubbingResponse
 from .dubbing_metadata_response import DubbingMetadataResponse
 from .extended_subscription_response_model_billing_period import ExtendedSubscriptionResponseModelBillingPeriod
 from .feedback_item import FeedbackItem
 from .fine_tuning_response import FineTuningResponse
 from .finetuning_state import FinetuningState
@@ -30,14 +31,15 @@
 from .get_pronunciation_dictionaries_metadata_response_model import GetPronunciationDictionariesMetadataResponseModel
 from .get_pronunciation_dictionary_metadata_response import GetPronunciationDictionaryMetadataResponse
 from .get_speech_history_response import GetSpeechHistoryResponse
 from .get_voices_response import GetVoicesResponse
 from .history import History
 from .history_item import HistoryItem
 from .http_validation_error import HttpValidationError
+from .initialize_connection import InitializeConnection
 from .invoice import Invoice
 from .language_response import LanguageResponse
 from .library_voice_response import LibraryVoiceResponse
 from .manual_verification_file_response import ManualVerificationFileResponse
 from .manual_verification_response import ManualVerificationResponse
 from .model import Model
 from .normalized_alignment import NormalizedAlignment
@@ -91,14 +93,15 @@
     "AudioOutput",
     "Category",
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
+    "CloseConnection",
     "Currency",
     "DoDubbingResponse",
     "DubbingMetadataResponse",
     "ExtendedSubscriptionResponseModelBillingPeriod",
     "FeedbackItem",
     "FineTuningResponse",
     "FinetuningState",
@@ -110,14 +113,15 @@
     "GetPronunciationDictionariesMetadataResponseModel",
     "GetPronunciationDictionaryMetadataResponse",
     "GetSpeechHistoryResponse",
     "GetVoicesResponse",
     "History",
     "HistoryItem",
     "HttpValidationError",
+    "InitializeConnection",
     "Invoice",
     "LanguageResponse",
     "LibraryVoiceResponse",
     "ManualVerificationFileResponse",
     "ManualVerificationResponse",
     "Model",
     "NormalizedAlignment",
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/add_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/add_voice_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.2.2/src/elevenlabs/types/audio_output.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/chapter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/chapter_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/do_dubbing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/dubbing_metadata_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/dubbing_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.2.2/src/elevenlabs/types/feedback_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.2.2/src/elevenlabs/types/generation_config.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_chapters_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_library_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_speech_history_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/get_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/history_item.py` & `elevenlabs-1.2.2/src/elevenlabs/types/history_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.2.2/src/elevenlabs/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/invoice.py` & `elevenlabs-1.2.2/src/elevenlabs/types/invoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/language_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/language_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/library_voice_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/manual_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.2.2/src/elevenlabs/types/normalized_alignment.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/project_extended_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/project_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/project_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/project_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/project_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.2.2/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.2.2/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/recording_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/send_text.py` & `elevenlabs-1.2.2/src/elevenlabs/types/send_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .generation_config import GenerationConfig
-from .realtime_voice_settings import RealtimeVoiceSettings
 
 
 class SendText(UncheckedBaseModel):
-    text: str = pydantic_v1.Field()
-    """
-    Should always end with a single space string `" "`. In the first message, the text should be a space `" "`.
-    """
-
+    text: str
     try_trigger_generation: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     This is an advanced setting that most users shouldn't need to use. It relates to our generation schedule
     explained [here](#understanding-how-our-websockets-buffer-text).
     
     Use this to attempt to immediately trigger the generation of audio, overriding the `chunk_length_schedule`.
     Unlike flush, `try_trigger_generation` will only generate audio if our
@@ -28,20 +22,14 @@
     
     Note that overriding the chunk schedule to generate small amounts of
     text may result in lower quality audio, therefore, only use this parameter if you
     really need text to be processed immediately. We generally recommend keeping the default value of
     `false` and adjusting the `chunk_length_schedule` in the `generation_config` instead.
     """
 
-    voice_settings: typing.Optional[RealtimeVoiceSettings] = None
-    generation_config: typing.Optional[GenerationConfig] = pydantic_v1.Field(default=None)
-    """
-    This property should only be provided in the first message you send.
-    """
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/speech_history_item_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.2.2/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/subscription.py` & `elevenlabs-1.2.2/src/elevenlabs/types/subscription.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/subscription_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/user.py` & `elevenlabs-1.2.2/src/elevenlabs/types/user.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.2.2/src/elevenlabs/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/verification_attempt_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/verification_attempt_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_sample.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_settings.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_sharing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.2.2/src/elevenlabs/types/voice_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.1/src/elevenlabs/user/client.py` & `elevenlabs-1.2.2/src/elevenlabs/user/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,26 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_subscription(self, *, request_options: typing.Optional[RequestOptions] = None) -> Subscription:
         """
         Gets extended information about the users subscription
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Subscription
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.user.get_subscription()
         """
@@ -66,17 +75,26 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> User:
         """
         Gets information about the user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        User
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.user.get()
         """
@@ -117,17 +135,26 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_subscription(self, *, request_options: typing.Optional[RequestOptions] = None) -> Subscription:
         """
         Gets extended information about the users subscription
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Subscription
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.user.get_subscription()
         """
@@ -163,17 +190,26 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> User:
         """
         Gets information about the user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        User
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.user.get()
         """
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/voice_generation/client.py` & `elevenlabs-1.2.2/src/elevenlabs/voice_generation/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,17 +27,26 @@
 
     def generate_parameters(
         self, *, request_options: typing.Optional[RequestOptions] = None
     ) -> VoiceGenerationParameterResponse:
         """
         Get possible parameters for the /v1/voice-generation/generate-voice endpoint.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceGenerationParameterResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voice_generation.generate_parameters()
         """
@@ -80,38 +89,52 @@
         accent_strength: float,
         text: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[bytes]:
         """
         Generate a random voice based on parameters. This method returns a generated_voice_id in the response header, and a sample of the voice in the body. If you like the generated voice call /v1/voice-generation/create-voice with the generated_voice_id to create the voice.
 
-        Parameters:
-            - gender: Gender. Category code corresponding to the gender of the generated voice. Possible values: female, male.
+        Parameters
+        ----------
+        gender : Gender
+            Category code corresponding to the gender of the generated voice. Possible values: female, male.
+
+        accent : str
+            Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
+
+        age : Age
+            Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
 
-            - accent: str. Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
+        accent_strength : float
+            The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
 
-            - age: Age. Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
+        text : str
+            Text to generate, text length has to be between 100 and 1000.
 
-            - accent_strength: float. The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - text: str. Text to generate, text length has to be between 100 and 1000.
+        Yields
+        ------
+        typing.Iterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voice_generation.generate(
-            gender="male",
-            accent="string",
-            age="young",
-            accent_strength=1.1,
-            text="string",
+            gender="female",
+            accent="american",
+            age="middle_aged",
+            accent_strength=2.0,
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
         )
         """
         with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -163,34 +186,47 @@
         generated_voice_id: str,
         labels: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Voice:
         """
         Create a previously generated voice. This endpoint should be called after you fetched a generated_voice_id using /v1/voice-generation/generate-voice.
 
-        Parameters:
-            - voice_name: str. Name to use for the created voice.
-
-            - voice_description: str. Description to use for the created voice.
-
-            - generated_voice_id: str. The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
-
-            - labels: typing.Optional[typing.Dict[str, str]]. Optional, metadata to add to the created voice. Defaults to None.
+        Parameters
+        ----------
+        voice_name : str
+            Name to use for the created voice.
+
+        voice_description : str
+            Description to use for the created voice.
+
+        generated_voice_id : str
+            The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
+
+        labels : typing.Optional[typing.Dict[str, str]]
+            Optional, metadata to add to the created voice. Defaults to None.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Voice
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voice_generation.create_a_previously_generated_voice(
-            voice_name="voice_name",
-            voice_description="voice_description",
-            generated_voice_id="generated_voice_id",
+            voice_name="Alex",
+            voice_description="Middle-aged American woman",
+            generated_voice_id="rbVJFu6SGRD1dbWpKnWl",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "voice_name": voice_name,
             "voice_description": voice_description,
             "generated_voice_id": generated_voice_id,
         }
@@ -241,17 +277,26 @@
 
     async def generate_parameters(
         self, *, request_options: typing.Optional[RequestOptions] = None
     ) -> VoiceGenerationParameterResponse:
         """
         Get possible parameters for the /v1/voice-generation/generate-voice endpoint.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceGenerationParameterResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voice_generation.generate_parameters()
         """
@@ -294,38 +339,52 @@
         accent_strength: float,
         text: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[bytes]:
         """
         Generate a random voice based on parameters. This method returns a generated_voice_id in the response header, and a sample of the voice in the body. If you like the generated voice call /v1/voice-generation/create-voice with the generated_voice_id to create the voice.
 
-        Parameters:
-            - gender: Gender. Category code corresponding to the gender of the generated voice. Possible values: female, male.
+        Parameters
+        ----------
+        gender : Gender
+            Category code corresponding to the gender of the generated voice. Possible values: female, male.
+
+        accent : str
+            Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
+
+        age : Age
+            Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
 
-            - accent: str. Category code corresponding to the accent of the generated voice. Possible values: american, british, african, australian, indian.
+        accent_strength : float
+            The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
 
-            - age: Age. Category code corresponding to the age of the generated voice. Possible values: young, middle_aged, old.
+        text : str
+            Text to generate, text length has to be between 100 and 1000.
 
-            - accent_strength: float. The strength of the accent of the generated voice. Has to be between 0.3 and 2.0.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - text: str. Text to generate, text length has to be between 100 and 1000.
+        Yields
+        ------
+        typing.AsyncIterator[bytes]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voice_generation.generate(
-            gender="male",
-            accent="string",
-            age="young",
-            accent_strength=1.1,
-            text="string",
+            gender="female",
+            accent="american",
+            age="middle_aged",
+            accent_strength=2.0,
+            text="It sure does, Jackie… My mama always said: “In Carolina, the air's so thick you can wear it!”",
         )
         """
         async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voice-generation/generate-voice"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -377,34 +436,47 @@
         generated_voice_id: str,
         labels: typing.Optional[typing.Dict[str, str]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Voice:
         """
         Create a previously generated voice. This endpoint should be called after you fetched a generated_voice_id using /v1/voice-generation/generate-voice.
 
-        Parameters:
-            - voice_name: str. Name to use for the created voice.
-
-            - voice_description: str. Description to use for the created voice.
-
-            - generated_voice_id: str. The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
-
-            - labels: typing.Optional[typing.Dict[str, str]]. Optional, metadata to add to the created voice. Defaults to None.
+        Parameters
+        ----------
+        voice_name : str
+            Name to use for the created voice.
+
+        voice_description : str
+            Description to use for the created voice.
+
+        generated_voice_id : str
+            The generated_voice_id to create, call POST /v1/voice-generation/generate-voice and fetch the generated_voice_id from the response header if don't have one yet.
+
+        labels : typing.Optional[typing.Dict[str, str]]
+            Optional, metadata to add to the created voice. Defaults to None.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Voice
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voice_generation.create_a_previously_generated_voice(
-            voice_name="voice_name",
-            voice_description="voice_description",
-            generated_voice_id="generated_voice_id",
+            voice_name="Alex",
+            voice_description="Middle-aged American woman",
+            generated_voice_id="rbVJFu6SGRD1dbWpKnWl",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "voice_name": voice_name,
             "voice_description": voice_description,
             "generated_voice_id": generated_voice_id,
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elevenlabs-1.2.1/src/elevenlabs/voices/client.py` & `elevenlabs-1.2.2/src/elevenlabs/voices/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,17 +27,26 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetVoicesResponse:
         """
         Gets a list of all available voices for a user.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetVoicesResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_all()
         """
@@ -73,17 +82,26 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_default_settings(self, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
         """
         Gets the default settings for voices. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceSettings
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_default_settings()
         """
@@ -115,26 +133,36 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_settings(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
         """
         Returns the settings for a specific voice. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceSettings
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get_settings(
-            voice_id="voice_id",
+            voice_id="2EiwWnXFnvU5JabPnv8n",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings"
             ),
@@ -173,28 +201,39 @@
         *,
         with_settings: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Voice:
         """
         Returns metadata about a specific voice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        with_settings : typing.Optional[bool]
+            If set will return settings information corresponding to the voice, requires authorization.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Voice
+            Successful Response
 
-            - with_settings: typing.Optional[bool]. If set will return settings information corresponding to the voice, requires authorization.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.get(
-            voice_id="voice_id",
+            voice_id="29vD33N1CtxCmqQRPOHJ",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
             ),
@@ -236,26 +275,36 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Deletes a voice by its ID.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.delete(
-            voice_id="voice_id",
+            voice_id="29vD33N1CtxCmqQRPOHJ",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
             ),
@@ -290,30 +339,44 @@
 
     def edit_settings(
         self, voice_id: str, *, request: VoiceSettings, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Edit your settings for a specific voice. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - request: VoiceSettings.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request : VoiceSettings
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs import VoiceSettings
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.edit_settings(
-            voice_id="voice_id",
-            request=VoiceSettings(),
+            voice_id="29vD33N1CtxCmqQRPOHJ",
+            request=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings/edit"
             ),
@@ -360,32 +423,45 @@
         description: typing.Optional[str] = None,
         labels: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddVoiceResponseModel:
         """
         Add a new voice to your collection of voices in VoiceLab.
 
-        Parameters:
-            - name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
-
-            - files: typing.List[core.File]. See core.File for more documentation
-
-            - description: typing.Optional[str]. How would you describe the voice?
-
-            - labels: typing.Optional[str]. Serialized labels dictionary for the voice.
+        Parameters
+        ----------
+        name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
+
+        files : typing.List[core.File]
+            See core.File for more documentation
+
+        description : typing.Optional[str]
+            How would you describe the voice?
+
+        labels : typing.Optional[str]
+            Serialized labels dictionary for the voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddVoiceResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.add(
-            name="name",
+            name="Alex",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -432,35 +508,49 @@
         description: typing.Optional[str] = None,
         labels: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Edit a voice created by you.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
+        name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
 
-            - files: typing.Optional[typing.List[core.File]]. See core.File for more documentation
+        files : typing.Optional[typing.List[core.File]]
+            See core.File for more documentation
 
-            - description: typing.Optional[str]. How would you describe the voice?
+        description : typing.Optional[str]
+            How would you describe the voice?
 
-            - labels: typing.Optional[str]. Serialized labels dictionary for the voice.
+        labels : typing.Optional[str]
+            Serialized labels dictionary for the voice.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.edit(
-            voice_id="voice_id",
-            name="name",
+            voice_id="JBFqnCBsd6RMkjVDRZzb",
+            name="George",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/edit"
             ),
@@ -507,32 +597,44 @@
         *,
         new_name: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddVoiceResponseModel:
         """
         Add a sharing voice to your collection of voices in VoiceLab.
 
-        Parameters:
-            - public_user_id: str. Public user ID used to publicly identify ElevenLabs users.
-
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - new_name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
+        Parameters
+        ----------
+        public_user_id : str
+            Public user ID used to publicly identify ElevenLabs users.
+
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        new_name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddVoiceResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.voices.add_sharing_voice(
-            public_user_id="public_user_id",
-            voice_id="voice_id",
-            new_name="new_name",
+            public_user_id="63e84100a6bf7874ba37a1bab9a31828a379ec94b891b401653b655c5110880f",
+            voice_id="sB1b5zUrxQVAFl2PhZFp",
+            new_name="Alita",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/add/{jsonable_encoder(public_user_id)}/{jsonable_encoder(voice_id)}",
@@ -590,51 +692,77 @@
         sort: typing.Optional[str] = None,
         page: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetLibraryVoicesResponse:
         """
         Gets a list of shared voices.
 
-        Parameters:
-            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
 
-            - category: typing.Optional[str]. voice category used for filtering
+        category : typing.Optional[str]
+            voice category used for filtering
 
-            - gender: typing.Optional[str]. gender used for filtering
+        gender : typing.Optional[str]
+            gender used for filtering
 
-            - age: typing.Optional[str]. age used for filtering
+        age : typing.Optional[str]
+            age used for filtering
 
-            - accent: typing.Optional[str]. accent used for filtering
+        accent : typing.Optional[str]
+            accent used for filtering
 
-            - language: typing.Optional[str]. language used for filtering
+        language : typing.Optional[str]
+            language used for filtering
 
-            - search: typing.Optional[str]. search term used for filtering
+        search : typing.Optional[str]
+            search term used for filtering
 
-            - use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]]. use-case used for filtering
+        use_cases : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            use-case used for filtering
 
-            - descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]]. search term used for filtering
+        descriptives : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            search term used for filtering
 
-            - featured: typing.Optional[bool]. Filter featured voices
+        featured : typing.Optional[bool]
+            Filter featured voices
 
-            - reader_app_enabled: typing.Optional[bool]. Filter voices that are enabled for the reader app
+        reader_app_enabled : typing.Optional[bool]
+            Filter voices that are enabled for the reader app
 
-            - owner_id: typing.Optional[str]. Filter voices by public owner ID
+        owner_id : typing.Optional[str]
+            Filter voices by public owner ID
 
-            - sort: typing.Optional[str]. sort criteria
+        sort : typing.Optional[str]
+            sort criteria
 
-            - page: typing.Optional[int].
+        page : typing.Optional[int]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetLibraryVoicesResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.voices.get_shared()
+        client.voices.get_shared(
+            page_size=1,
+            gender="female",
+            language="en",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -691,17 +819,26 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetVoicesResponse:
         """
         Gets a list of all available voices for a user.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetVoicesResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_all()
         """
@@ -737,17 +874,26 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_default_settings(self, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
         """
         Gets the default settings for voices. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceSettings
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_default_settings()
         """
@@ -781,26 +927,36 @@
 
     async def get_settings(
         self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> VoiceSettings:
         """
         Returns the settings for a specific voice. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VoiceSettings
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get_settings(
-            voice_id="voice_id",
+            voice_id="2EiwWnXFnvU5JabPnv8n",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings"
             ),
@@ -839,28 +995,39 @@
         *,
         with_settings: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Voice:
         """
         Returns metadata about a specific voice.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        with_settings : typing.Optional[bool]
+            If set will return settings information corresponding to the voice, requires authorization.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Voice
+            Successful Response
 
-            - with_settings: typing.Optional[bool]. If set will return settings information corresponding to the voice, requires authorization.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.get(
-            voice_id="voice_id",
+            voice_id="29vD33N1CtxCmqQRPOHJ",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
             ),
@@ -902,26 +1069,36 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Deletes a voice by its ID.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.delete(
-            voice_id="voice_id",
+            voice_id="29vD33N1CtxCmqQRPOHJ",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}"
             ),
@@ -956,30 +1133,44 @@
 
     async def edit_settings(
         self, voice_id: str, *, request: VoiceSettings, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Edit your settings for a specific voice. "similarity_boost" corresponds to"Clarity + Similarity Enhancement" in the web app and "stability" corresponds to "Stability" slider in the web app.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - request: VoiceSettings.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        request : VoiceSettings
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs import VoiceSettings
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.edit_settings(
-            voice_id="voice_id",
-            request=VoiceSettings(),
+            voice_id="29vD33N1CtxCmqQRPOHJ",
+            request=VoiceSettings(
+                stability=0.1,
+                similarity_boost=0.3,
+                style=0.2,
+            ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/settings/edit"
             ),
@@ -1026,32 +1217,45 @@
         description: typing.Optional[str] = None,
         labels: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddVoiceResponseModel:
         """
         Add a new voice to your collection of voices in VoiceLab.
 
-        Parameters:
-            - name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
-
-            - files: typing.List[core.File]. See core.File for more documentation
-
-            - description: typing.Optional[str]. How would you describe the voice?
-
-            - labels: typing.Optional[str]. Serialized labels dictionary for the voice.
+        Parameters
+        ----------
+        name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
+
+        files : typing.List[core.File]
+            See core.File for more documentation
+
+        description : typing.Optional[str]
+            How would you describe the voice?
+
+        labels : typing.Optional[str]
+            Serialized labels dictionary for the voice.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddVoiceResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.add(
-            name="name",
+            name="Alex",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/voices/add"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -1098,35 +1302,49 @@
         description: typing.Optional[str] = None,
         labels: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Edit a voice created by you.
 
-        Parameters:
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+        Parameters
+        ----------
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
 
-            - name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
+        name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
 
-            - files: typing.Optional[typing.List[core.File]]. See core.File for more documentation
+        files : typing.Optional[typing.List[core.File]]
+            See core.File for more documentation
 
-            - description: typing.Optional[str]. How would you describe the voice?
+        description : typing.Optional[str]
+            How would you describe the voice?
 
-            - labels: typing.Optional[str]. Serialized labels dictionary for the voice.
+        labels : typing.Optional[str]
+            Serialized labels dictionary for the voice.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.edit(
-            voice_id="voice_id",
-            name="name",
+            voice_id="JBFqnCBsd6RMkjVDRZzb",
+            name="George",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/voices/{jsonable_encoder(voice_id)}/edit"
             ),
@@ -1173,32 +1391,44 @@
         *,
         new_name: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AddVoiceResponseModel:
         """
         Add a sharing voice to your collection of voices in VoiceLab.
 
-        Parameters:
-            - public_user_id: str. Public user ID used to publicly identify ElevenLabs users.
-
-            - voice_id: str. Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
-
-            - new_name: str. The name that identifies this voice. This will be displayed in the dropdown of the website.
+        Parameters
+        ----------
+        public_user_id : str
+            Public user ID used to publicly identify ElevenLabs users.
+
+        voice_id : str
+            Voice ID to be used, you can use https://api.elevenlabs.io/v1/voices to list all the available voices.
+
+        new_name : str
+            The name that identifies this voice. This will be displayed in the dropdown of the website.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AddVoiceResponseModel
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.voices.add_sharing_voice(
-            public_user_id="public_user_id",
-            voice_id="voice_id",
-            new_name="new_name",
+            public_user_id="63e84100a6bf7874ba37a1bab9a31828a379ec94b891b401653b655c5110880f",
+            voice_id="sB1b5zUrxQVAFl2PhZFp",
+            new_name="Alita",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/voices/add/{jsonable_encoder(public_user_id)}/{jsonable_encoder(voice_id)}",
@@ -1256,51 +1486,77 @@
         sort: typing.Optional[str] = None,
         page: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> GetLibraryVoicesResponse:
         """
         Gets a list of shared voices.
 
-        Parameters:
-            - page_size: typing.Optional[int]. How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            How many shared voices to return at maximum. Can not exceed 100, defaults to 30.
 
-            - category: typing.Optional[str]. voice category used for filtering
+        category : typing.Optional[str]
+            voice category used for filtering
 
-            - gender: typing.Optional[str]. gender used for filtering
+        gender : typing.Optional[str]
+            gender used for filtering
 
-            - age: typing.Optional[str]. age used for filtering
+        age : typing.Optional[str]
+            age used for filtering
 
-            - accent: typing.Optional[str]. accent used for filtering
+        accent : typing.Optional[str]
+            accent used for filtering
 
-            - language: typing.Optional[str]. language used for filtering
+        language : typing.Optional[str]
+            language used for filtering
 
-            - search: typing.Optional[str]. search term used for filtering
+        search : typing.Optional[str]
+            search term used for filtering
 
-            - use_cases: typing.Optional[typing.Union[str, typing.Sequence[str]]]. use-case used for filtering
+        use_cases : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            use-case used for filtering
 
-            - descriptives: typing.Optional[typing.Union[str, typing.Sequence[str]]]. search term used for filtering
+        descriptives : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            search term used for filtering
 
-            - featured: typing.Optional[bool]. Filter featured voices
+        featured : typing.Optional[bool]
+            Filter featured voices
 
-            - reader_app_enabled: typing.Optional[bool]. Filter voices that are enabled for the reader app
+        reader_app_enabled : typing.Optional[bool]
+            Filter voices that are enabled for the reader app
 
-            - owner_id: typing.Optional[str]. Filter voices by public owner ID
+        owner_id : typing.Optional[str]
+            Filter voices by public owner ID
 
-            - sort: typing.Optional[str]. sort criteria
+        sort : typing.Optional[str]
+            sort criteria
 
-            - page: typing.Optional[int].
+        page : typing.Optional[int]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetLibraryVoicesResponse
+            Successful Response
+
+        Examples
+        --------
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.voices.get_shared()
+        await client.voices.get_shared(
+            page_size=1,
+            gender="female",
+            language="en",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `elevenlabs-1.2.1/PKG-INFO` & `elevenlabs-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

