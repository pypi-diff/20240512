# Comparing `tmp/ofscraper-3.9.6.tar.gz` & `tmp/ofscraper-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.6.tar", max compression
+gzip compressed data, was "ofscraper-3.9.7.tar", max compression
```

## Comparing `ofscraper-3.9.6.tar` & `ofscraper-3.9.7.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     1067 2024-05-10 19:08:59.308061 ofscraper-3.9.6/LICENSE
--rw-r--r--   0        0        0     4213 2024-05-10 19:08:59.308061 ofscraper-3.9.6/README.md
--rwxr-xr-x   0        0        0      283 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__version__.pye
--rw-r--r--   0        0        0    15951 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14697 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/init.py
--rw-r--r--   0        0        0    14238 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/me.py
--rw-r--r--   0        0        0    18146 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13861 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8581 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6176 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1718 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3381 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    12660 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8171 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    17037 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1460 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15560 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20597 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/posts.py
--rw-r--r--   0        0        0    18427 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0      156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/button.py
--rw-r--r--   0        0        0     1689 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/boolfield.py
--rw-r--r--   0        0        0     1370 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/datefield.py
--rw-r--r--   0        0        0      629 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/mediafield.py
--rw-r--r--   0        0        0      694 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/numfield.py
--rw-r--r--   0        0        0     1302 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/pricefield.py
--rw-r--r--   0        0        0      678 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/responsefield.py
--rw-r--r--   0        0        0     1417 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/selectfield.py
--rw-r--r--   0        0        0     1487 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/textsearch.py
--rw-r--r--   0        0        0     2460 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/timefield.py
--rw-r--r--   0        0        0     1893 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/filterinput.py
--rw-r--r--   0        0        0      117 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/intergerinput.py
--rw-r--r--   0        0        0      113 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/strinput.py
--rw-r--r--   0        0        0      297 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/row_names.py
--rw-r--r--   0        0        0     4583 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/status.py
--rw-r--r--   0        0        0    21258 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/table.py
--rw-r--r--   0        0        0      156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/table_console.py
--rw-r--r--   0        0        0        1 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/__init__.py
--rw-r--r--   0        0        0     6447 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/download/download.py
--rw-r--r--   0        0        0    21813 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/download/post.py
--rw-r--r--   0        0        0    11597 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/like.py
--rw-r--r--   0        0        0     1545 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/scrape_context.py
--rw-r--r--   0        0        0     1039 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/add_select/add_selected.py
--rw-r--r--   0        0        0    26132 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/check.py
--rw-r--r--   0        0        0    11014 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/manual.py
--rw-r--r--   0        0        0     8188 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/metadata.py
--rw-r--r--   0        0        0      556 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3785 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/config.py
--rw-r--r--   0        0        0     1002 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/date.py
--rw-r--r--   0        0        0      190 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/files.py
--rw-r--r--   0        0        0     1375 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/logger.py
--rw-r--r--   0        0        0      120 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1908 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1807 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/req.py
--rw-r--r--   0        0        0      271 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/table.py
--rw-r--r--   0        0        0   265533 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/time.py
--rw-r--r--   0        0        0     3594 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    15609 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19876 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0    11553 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8494 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6725 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10881 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10682 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     4914 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/download.py
--rw-r--r--   0        0        0    17191 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9077 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10787 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1414 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1356 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3795 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6372 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2063 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2341 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9440 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     5698 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     8075 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5019 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     3136 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     3143 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      957 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/helpers.py
--rw-r--r--   0        0        0      726 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     7561 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1538 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1454 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3414 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8105 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15219 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6834 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4438 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27916 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     3112 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16090 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10346 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1578 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2743 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0     1089 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_processing.py
--rw-r--r--   0        0        0     1546 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_program.py
--rw-r--r--   0        0        0     4411 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_user_filter.py
--rw-r--r--   0        0        0      997 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/automatic.py
--rw-r--r--   0        0        0     5183 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/content.py
--rw-r--r--   0        0        0      944 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/download.py
--rw-r--r--   0        0        0      905 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/file.py
--rw-r--r--   0        0        0     1185 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/logging.py
--rw-r--r--   0        0        0     1282 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/media_type.py
--rw-r--r--   0        0        0      935 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/program.py
--rw-r--r--   0        0        0     3825 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_list.py
--rw-r--r--   0        0        0     2683 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_select.py
--rw-r--r--   0        0        0      971 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_sort.py
--rw-r--r--   0        0        0      319 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/advanced_common.py
--rw-r--r--   0        0        0      661 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/common.py
--rw-r--r--   0        0        0     1020 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/main.py
--rw-r--r--   0        0        0     1579 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/manual.py
--rw-r--r--   0        0        0     2281 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/message_check.py
--rw-r--r--   0        0        0     4145 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/metadata.py
--rw-r--r--   0        0        0     1862 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/paid_check.py
--rw-r--r--   0        0        0     2277 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/post_check.py
--rw-r--r--   0        0        0     1928 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/story_check.py
--rw-r--r--   0        0        0      502 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/main.py
--rw-r--r--   0        0        0      189 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/manual.py
--rw-r--r--   0        0        0      217 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/message.py
--rw-r--r--   0        0        0      197 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/metadata.py
--rw-r--r--   0        0        0      205 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/paid.py
--rw-r--r--   0        0        0      205 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/post.py
--rw-r--r--   0        0        0      209 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/story.py
--rw-r--r--   0        0        0       12 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     5616 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     2031 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      960 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      403 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1669 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6902 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1612 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2952 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1442 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    24693 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2073 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      409 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/console.py
--rw-r--r--   0        0        0      788 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1004 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1745 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7226 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1670 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      601 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      576 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4167 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1022 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1710 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3091 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      703 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     4912 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1034 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1583 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10893 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4406 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1672 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4691 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3279 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2055 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2117 2024-05-10 19:09:27.052271 ofscraper-3.9.6/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-12 12:52:16.784428 ofscraper-3.9.7/LICENSE
+-rw-r--r--   0        0        0     4213 2024-05-12 12:52:16.784428 ofscraper-3.9.7/README.md
+-rwxr-xr-x   0        0        0      283 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/__version__.pye
+-rw-r--r--   0        0        0    16148 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14697 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14238 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18425 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13861 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8581 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1718 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3381 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12660 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8171 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    17204 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1460 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15560 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20597 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5156 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    18209 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0      156 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/button.py
+-rw-r--r--   0        0        0     1689 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/boolfield.py
+-rw-r--r--   0        0        0     1370 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/datefield.py
+-rw-r--r--   0        0        0      629 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/mediafield.py
+-rw-r--r--   0        0        0      694 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/numfield.py
+-rw-r--r--   0        0        0     1302 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/pricefield.py
+-rw-r--r--   0        0        0      678 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/responsefield.py
+-rw-r--r--   0        0        0     1417 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/selectfield.py
+-rw-r--r--   0        0        0     1487 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/textsearch.py
+-rw-r--r--   0        0        0     2460 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/fields/timefield.py
+-rw-r--r--   0        0        0     1893 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/filterinput.py
+-rw-r--r--   0        0        0      117 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/intergerinput.py
+-rw-r--r--   0        0        0      113 2024-05-12 12:52:16.788428 ofscraper-3.9.7/ofscraper/classes/table/inputs/strinput.py
+-rw-r--r--   0        0        0      297 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/row_names.py
+-rw-r--r--   0        0        0     4583 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/status.py
+-rw-r--r--   0        0        0    21258 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/table.py
+-rw-r--r--   0        0        0      156 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/classes/table/table_console.py
+-rw-r--r--   0        0        0        1 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/__init__.py
+-rw-r--r--   0        0        0     6465 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/download/download.py
+-rw-r--r--   0        0        0    21884 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/download/post.py
+-rw-r--r--   0        0        0    11597 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/like.py
+-rw-r--r--   0        0        0     1545 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/actions/scrape_context.py
+-rw-r--r--   0        0        0     1039 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/add_select/add_selected.py
+-rw-r--r--   0        0        0    26132 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    11014 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0     8260 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/metadata.py
+-rw-r--r--   0        0        0      556 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3785 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/config.py
+-rw-r--r--   0        0        0     1002 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/date.py
+-rw-r--r--   0        0        0      190 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1375 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/logger.py
+-rw-r--r--   0        0        0      120 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1908 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1808 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/req.py
+-rw-r--r--   0        0        0      271 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/table.py
+-rw-r--r--   0        0        0   265533 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3594 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    15609 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19852 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0    11553 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8494 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10881 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10682 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     2383 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17191 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9094 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10787 2024-05-12 12:52:16.792428 ofscraper-3.9.7/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1414 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1356 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3795 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6372 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2063 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2341 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9440 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     5698 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     9970 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5335 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3136 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3143 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      957 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      726 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7561 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1538 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1454 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3414 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8105 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15219 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6834 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4438 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27916 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     3112 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16090 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10346 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1578 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2743 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0     1089 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_processing.py
+-rw-r--r--   0        0        0     1546 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_program.py
+-rw-r--r--   0        0        0     4411 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_user_filter.py
+-rw-r--r--   0        0        0      997 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/automatic.py
+-rw-r--r--   0        0        0     5198 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/content.py
+-rw-r--r--   0        0        0      944 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/download.py
+-rw-r--r--   0        0        0      905 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/file.py
+-rw-r--r--   0        0        0     1185 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/logging.py
+-rw-r--r--   0        0        0     1282 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/media_type.py
+-rw-r--r--   0        0        0      935 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/program.py
+-rw-r--r--   0        0        0     3825 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_list.py
+-rw-r--r--   0        0        0     2683 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_select.py
+-rw-r--r--   0        0        0      971 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/arguments/user_sort.py
+-rw-r--r--   0        0        0      319 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/advanced_common.py
+-rw-r--r--   0        0        0      661 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/common.py
+-rw-r--r--   0        0        0     1020 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/main.py
+-rw-r--r--   0        0        0     1579 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/manual.py
+-rw-r--r--   0        0        0     2281 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/message_check.py
+-rw-r--r--   0        0        0     4145 2024-05-12 12:52:16.796428 ofscraper-3.9.7/ofscraper/utils/args/bundles/metadata.py
+-rw-r--r--   0        0        0     1862 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/paid_check.py
+-rw-r--r--   0        0        0     2277 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/post_check.py
+-rw-r--r--   0        0        0     1928 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/bundles/story_check.py
+-rw-r--r--   0        0        0      502 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/main.py
+-rw-r--r--   0        0        0      189 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/manual.py
+-rw-r--r--   0        0        0      217 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/message.py
+-rw-r--r--   0        0        0      197 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/metadata.py
+-rw-r--r--   0        0        0      205 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/paid.py
+-rw-r--r--   0        0        0      205 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/post.py
+-rw-r--r--   0        0        0      209 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/commands/story.py
+-rw-r--r--   0        0        0       12 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     5616 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     2031 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      960 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      403 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1669 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6704 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1612 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2952 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1442 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24693 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2073 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      409 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      788 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1004 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1745 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7226 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1670 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      601 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      576 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4167 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1022 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1710 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3091 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      703 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     4912 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1034 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1583 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10893 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4406 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1672 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4691 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3279 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2055 2024-05-12 12:52:16.800428 ofscraper-3.9.7/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2117 2024-05-12 12:52:41.864739 ofscraper-3.9.7/pyproject.toml
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.7/PKG-INFO
```

### Comparing `ofscraper-3.9.6/LICENSE` & `ofscraper-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/README.md` & `ofscraper-3.9.7/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/__version__.py` & `ofscraper-3.9.7/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/__version__.pye` & `ofscraper-3.9.7/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/archive.py` & `ofscraper-3.9.7/ofscraper/api/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import ofscraper.api.common.logs as common_logs
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
-from ofscraper.db.operations_.media import get_archived_media
+from ofscraper.db.operations_.media import get_media_ids_downloaded_model,get_archived_media
 from ofscraper.db.operations_.posts import (
     get_archived_post_info,
     get_youngest_archived_date,
 )
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
 
@@ -260,19 +260,21 @@
         return read_args.retriveArgs().after.float_timestamp
 
     elif cache.get(f"{model_id}_full_archived_scrape"):
         log.info(
             "Used --after previously. Scraping all archived posts required to make sure content is not missing"
         )
         return 0
-    curr = await get_archived_media(model_id=model_id, username=username)
+
+    curr=await get_archived_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
+    curr_downloaded = await get_media_ids_downloaded_model(model_id=model_id, username=username)
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1 and x.get("post_id") not in curr_downloaded and x.get("unlocked") != 0, curr))
     missing_items = list(sorted(missing_items, key=lambda x: x.get("posted_at") or 0))
     if len(missing_items) == 0:
         log.debug(
             "Using newest db date because,all downloads in db marked as downloaded"
         )
         return arrow.get(
             await get_youngest_archived_date(model_id=model_id, username=username)
@@ -415,13 +417,13 @@
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def time_log(username, after):
     log.info(
         f"""
-Setting archived scan range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}  to {arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
+Setting archived scan range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to {arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all archived posts + download/re-download of all files[/yellow]
 
             """
     )
```

### Comparing `ofscraper-3.9.6/ofscraper/api/highlights.py` & `ofscraper-3.9.7/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/init.py` & `ofscraper-3.9.7/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/labels.py` & `ofscraper-3.9.7/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/me.py` & `ofscraper-3.9.7/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/messages.py` & `ofscraper-3.9.7/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
-from ofscraper.db.operations_.media import get_messages_media
+from ofscraper.db.operations_.media import get_messages_media,get_media_ids_downloaded_model
 from ofscraper.db.operations_.messages import (
     get_messages_post_info,
     get_youngest_message_date,
 )
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
 
@@ -427,14 +427,16 @@
             "Used --after previously. Scraping all messages required to make sure content is not missing"
         )
         return 0
     curr = await get_messages_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
+    curr_downloaded = await get_media_ids_downloaded_model(model_id=model_id, username=username)
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1 and x.get("post_id") not in curr_downloaded and x.get("unlocked") != 0, curr))
     missing_items = list(
         filter(lambda x: x.get("downloaded") != 1 and x.get("unlocked") != 0, curr)
     )
     missing_items = list(
         sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
     )
     if len(missing_items) == 0:
@@ -490,15 +492,15 @@
             break  # Exit the loop if we've processed all elements
 
 
 def log_after_before(after, before, username):
 
     log.info(
         f"""
-Setting Message range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to {arrow.get(before).format(constants.getattr('API_DATE_FORMAT'))}
+Setting Message scan range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to {arrow.get(before).format(constants.getattr('API_DATE_FORMAT'))}
 
 [yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
 
         """
     )
```

### Comparing `ofscraper-3.9.6/ofscraper/api/paid.py` & `ofscraper-3.9.7/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/pinned.py` & `ofscraper-3.9.7/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/profile.py` & `ofscraper-3.9.7/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.7/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.7/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.7/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.7/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/api/timeline.py` & `ofscraper-3.9.7/ofscraper/api/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
-from ofscraper.db.operations_.media import get_timeline_media
+from ofscraper.db.operations_.media import get_timeline_media,get_media_ids_downloaded_model
 from ofscraper.db.operations_.posts import (
     get_timeline_posts_info,
     get_youngest_timeline_date,
 )
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
 
@@ -292,17 +292,18 @@
             "Used --after previously. Scraping all timeline posts required to make sure content is not missing"
         )
         return 0
     curr = await get_timeline_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting oldest date to zero because database is empty")
         return 0
-    missing_items = list(
-        filter(lambda x: x.get("downloaded") != 1 and x.get("unlocked") != 0, curr)
-    )
+    curr_downloaded = await get_media_ids_downloaded_model(model_id=model_id, username=username)
+
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1 and x.get("post_id") not in curr_downloaded and x.get("unlocked") != 0, curr))
+    
     missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x["posted_at"])))
     if len(missing_items) == 0:
         log.debug(
             "Using using newest db date, because all downloads in db marked as downloaded"
         )
         return arrow.get(
             await get_youngest_timeline_date(model_id=model_id, username=username)
@@ -445,13 +446,13 @@
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def time_log(username, after):
     log.info(
         f"""
-Setting timeline scan range for{username} rom {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to{arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
+Setting timeline scan range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to {arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
 
             """
     )
```

### Comparing `ofscraper-3.9.6/ofscraper/classes/base.py` & `ofscraper-3.9.7/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/labels.py` & `ofscraper-3.9.7/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/media.py` & `ofscraper-3.9.7/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/models.py` & `ofscraper-3.9.7/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.7/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/placeholder.py` & `ofscraper-3.9.7/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/posts.py` & `ofscraper-3.9.7/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.7/ofscraper/classes/sessionmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,14 @@
         self.wait_exponential = wait_exponential or tenacity.wait_exponential(
             min=constants.getattr("OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT"),
             max=constants.getattr("OF_MAX_WAIT_EXPONENTIAL_SESSION_DEFAULT"),
         )
         self.wait = self._wait_picker
 
     def _wait_picker(self, retry_state) -> None:
-        exception = retry_state.outcome.exception()
-        # if is_rate_limited(exception):
-        #     sleep = self.wait_exponential(retry_state)
-        # else:
-        #     sleep = self.wait_random(retry_state)
         sleep = self.wait_random(retry_state)
         logging.getLogger("shared").debug(f"sleeping for {sleep} seconds before retry")
         return sleep
 
     def _after_func(self, retry_state) -> None:
         exception = retry_state.outcome.exception()
         if (
```

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/boolfield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/boolfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/datefield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/datefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/mediafield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/mediafield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/numfield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/numfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/pricefield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/pricefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/responsefield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/responsefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/selectfield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/selectfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/textsearch.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/textsearch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/fields/timefield.py` & `ofscraper-3.9.7/ofscraper/classes/table/fields/timefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/inputs/filterinput.py` & `ofscraper-3.9.7/ofscraper/classes/table/inputs/filterinput.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/status.py` & `ofscraper-3.9.7/ofscraper/classes/table/status.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/classes/table/table.py` & `ofscraper-3.9.7/ofscraper/classes/table/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/actions/download/download.py` & `ofscraper-3.9.7/ofscraper/commands/actions/download/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         log.warning(f"Avatar : {avatar}")
     if bool(areas.get_download_area()):
         log.info(
             f"Getting {','.join(areas.get_download_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
         )
     try:
         operations.table_init_create(model_id=model_id, username=username)
-        media, posts = OF.process_areas(ele, model_id)
+        media, posts = OF.process_areas(ele, model_id,username)
         return {model_id: {"username": username, "posts": posts, "media": media,"avatar":avatar}}
     except Exception as e:
         if isinstance(e, KeyboardInterrupt):
             raise e
         log.traceback_(f"failed with exception: {e}")
         log.traceback_(traceback.format_exc())
 
@@ -137,15 +137,15 @@
             log.warning(
                 f"Getting {','.join(areas.get_download_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
             )
             try:
                 model_id = ele.id
                 username = ele.name
                 operations.table_init_create(model_id=model_id, username=username)
-                combined_urls, posts = OF.process_areas(ele, model_id)
+                combined_urls, posts = OF.process_areas(ele, model_id,username)
                 download.download_process(
                     username, model_id, combined_urls, posts=posts
                 )
             except Exception as e:
                 if isinstance(e, KeyboardInterrupt):
                     raise e
                 log.traceback_(f"failed with exception: {e}")
```

### Comparing `ofscraper-3.9.6/ofscraper/commands/actions/download/post.py` & `ofscraper-3.9.7/ofscraper/commands/actions/download/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,15 +390,15 @@
             seen = set()
             new_posts = [
                 post
                 for post in all_posts
                 if post.id not in seen and not seen.add(post.id)
             ]
             new_medias = [item for post in new_posts for item in post.all_media]
-            new_medias = filters.filterMedia(new_medias)
+            new_medias = filters.filterMedia(new_medias,model_id=model_id,username=username)
             new_posts = filters.filterPost(new_posts)
             await operations.make_post_table_changes(
                 new_posts,
                 model_id=model_id,
                 username=username,
             )
             await batch_mediainsert(
@@ -477,17 +477,17 @@
                 posts,
             )
         except Exception as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
 
 @run
-async def process_areas(model_id, username):
-    media, posts = await process_areas_helper(model_id, username)
-    return filters.filterMedia(media), filters.filterPost(posts)
+async def process_areas(ele,model_id, username):
+    media, posts = await process_areas_helper(ele, model_id)
+    return filters.filterMedia(media,model_id=model_id,username=username), filters.filterPost(posts)
 
 
 async def process_task(model_id, username, ele):
     mediaObjs = []
     postObjs = []
     final_post_areas = set(areas.get_download_area())
     tasks = []
```

### Comparing `ofscraper-3.9.6/ofscraper/commands/actions/like.py` & `ofscraper-3.9.7/ofscraper/commands/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/actions/scrape_context.py` & `ofscraper-3.9.7/ofscraper/commands/actions/scrape_context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/add_select/add_selected.py` & `ofscraper-3.9.7/ofscraper/commands/add_select/add_selected.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/check.py` & `ofscraper-3.9.7/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/manual.py` & `ofscraper-3.9.7/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/metadata.py` & `ofscraper-3.9.7/ofscraper/commands/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             )
             try:
                 model_id = ele.id
                 username = ele.name
 
                 media, _ = process_areas_helper(ele, model_id)
                 operations.table_init_create(model_id=model_id, username=username)
-                filterMedia = filters.filterMedia(media)
+                filterMedia = filters.filterMedia(media,username=username,model_id=model_id)
                 download.download_process(username, model_id, filterMedia)
                 metadata_stray_media(username,model_id, media)
             except Exception as e:
                 if isinstance(e, KeyboardInterrupt):
                     raise e
                 log.traceback_(f"failed with exception: {e}")
                 log.traceback_(traceback.format_exc())
@@ -128,15 +128,15 @@
             avatar=val['avatar']
             try:
                 log.warning(
                 f"Download action progressing on model {count+1}/{length} models "
                 )
                 if constants.getattr("SHOW_AVATAR") and avatar:
                     log.warning(f"Avatar : {avatar}")
-                filterMedia = filters.filterMedia(media)
+                filterMedia = filters.filterMedia(media,username=username,model_id=model_id)
                 download.download_process(
                     username, model_id, filterMedia
                 )
                 metadata_stray_media(username,model_id, media)
             except Exception as e:
                 if isinstance(e, KeyboardInterrupt):
                     raise e
```

### Comparing `ofscraper-3.9.6/ofscraper/commands/picker.py` & `ofscraper-3.9.7/ofscraper/commands/picker.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/commands/scraper.py` & `ofscraper-3.9.7/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/config.py` & `ofscraper-3.9.7/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/constants.py` & `ofscraper-3.9.7/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/general.py` & `ofscraper-3.9.7/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/other_url.py` & `ofscraper-3.9.7/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/prompts.py` & `ofscraper-3.9.7/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/req.py` & `ofscraper-3.9.7/ofscraper/const/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 PROXY_MOUNTS = None
 PROXY_AUTH = None
 maxChunkSize = 1024 * 1024 * 10
 maxChunkSizeB = 1024 * 1024
 CHUNK_ITER = 10
 
 REQ_SEMAPHORE_MULTI = 5
-API_REQ_SEM_MAX = 8
+API_REQ_SEM_MAX = 12
 SCRAPE_PAID_SEMS = 10
 SUBSCRIPTION_SEMS = 5
 API_REQ_CHECK_MAX = 12
 LIKE_MAX_SEMS = 12
 MAX_SEMS_BATCH_DOWNLOAD = 12
 MAX_SEMS_SINGLE_THREAD_DOWNLOAD = 50
 MPD_MAX_SEMS = 4
```

### Comparing `ofscraper-3.9.6/ofscraper/const/test_constants.py` & `ofscraper-3.9.7/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/const/url.py` & `ofscraper-3.9.7/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations.py` & `ofscraper-3.9.7/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.7/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/media.py` & `ofscraper-3.9.7/ofscraper/db/operations_/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,27 +285,27 @@
 def get_media_ids(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allIDCheck)
         return [dict(row)["media_id"] for row in cur.fetchall()]
 
 
 @wrapper.operation_wrapper
-def get_media_ids_downloaded(model_id=None, username=None, conn=None, **kwargs) -> list:
+def get_media_ids_downloaded(conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allDLIDCheck)
-        return [dict(row)["media_id"] for row in cur.fetchall()]
-
+        return set([dict(row)["media_id"] for row in cur.fetchall()])
 
-@wrapper.operation_wrapper
+@run
+@wrapper.operation_wrapper_async
 def get_media_ids_downloaded_model(
-    model_id=None, username=None, conn=None, **kwargs
+    model_id=None, conn=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allDLModelIDCheck, [model_id])
-        return [dict(row)["media_id"] for row in cur.fetchall()]
+        return set([dict(row)["media_id"] for row in cur.fetchall()])
 
 
 @wrapper.operation_wrapper
 def get_dupe_media_hashes(
     model_id=None, username=None, conn=None, mediatype=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
@@ -461,14 +461,15 @@
 
 @wrapper.operation_wrapper_async
 def drop_media_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(mediaDrop)
         conn.commit()
 
+
 @run
 @wrapper.operation_wrapper_async
 def get_messages_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getMessagesMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
```

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.7/ofscraper/db/operations_/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.7/ofscraper/db/operations_/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/others.py` & `ofscraper-3.9.7/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.7/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.7/ofscraper/db/operations_/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.7/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.7/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/alt_download.py` & `ofscraper-3.9.7/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.7/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.7/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.7/ofscraper/download/downloadnormal.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                 input_=otherqueue, name="ofscraper_normal_other"
             )
             with Live(
                 progress_group,
                 refresh_per_second=constants.getattr("refreshScreen"),
                 console=console.shared_console,
                 transient=True,
+                
             ):
                 aws = []
 
                 async with download_session() as c:
                     for ele in medialist:
                         aws.append(
                             asyncio.create_task(
```

### Comparing `ofscraper-3.9.6/ofscraper/download/main_download.py` & `ofscraper-3.9.7/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.7/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.7/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.7/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.7/ofscraper/download/shared/common/alt_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.7/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.7/ofscraper/download/shared/common/main_common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/globals.py` & `ofscraper-3.9.7/ofscraper/download/shared/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/metadata.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.7/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/media/main.py` & `ofscraper-3.9.7/ofscraper/filters/media/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,146 @@
 import logging
 
 import ofscraper.filters.media.helpers as helpers
+import ofscraper.utils.args.read as read_args
+import ofscraper.utils.constants as constants
+
 
 log = logging.getLogger("shared")
 
 
-def filterMedia(media):
+def filterMedia(media,username=None, model_id=None):
     count = 1
-    helpers.trace_log_media(count, media, "all media no filter:")
-    log.debug(f"filter {count}-> all media no filter count: {len(media)}")
-    media = helpers.sort_media(media)
-    count += 1
-    helpers.trace_log_media(count, media, "final media  from retrived post:")
-    log.debug(f"filter {count}->  final media count from retrived post: {len(media)}")
-    media = helpers.dupefilter(media)
+
+    helpers.trace_log_media(count, media, "initial media no filter:")
+    log.debug(f"filter {count}-> initial media no filter count: {len(media)}")
+
+    media = helpers.sort_by_date(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media dupe filter:")
+    helpers.trace_log_media(count, media, "sorted by date initial")
+
 
-    log.debug(f"filter {count}-> all media dupe filter count: {len(media)}")
     media = helpers.post_datesorter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media datesort:")
+    helpers.trace_log_media(count, media, "media datesort:")
+    log.debug(f"filter {count}-> media datesort count: {len(media)}")
 
-    log.debug(f"filter {count}-> all media datesort count: {len(media)}")
     media = helpers.posts_type_filter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media post media type filter:")
+    helpers.trace_log_media(count, media, "media post media type filter:")
+    log.debug(f"filter {count}-> media post media type filter count: {len(media)}")
 
-    log.debug(f"filter {count}-> all media post media type filter count: {len(media)}")
     media = helpers.posts_date_filter_media(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media post date filter:")
+    helpers.trace_log_media(count, media, "media post date filter:")
+    log.debug(f"filter {count}-> media post date filter: {len(media)}")
 
-    log.debug(f"filter {count}-> all media post date filter: {len(media)}")
-    media = helpers.post_timed_filter(media)
+    media = helpers.temp_post_filter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media post timed post filter:")
-
-    log.debug(f"filter {count}->  all media post timed post filter count: {len(media)}")
-    media = helpers.post_user_filter(media)
+    helpers.trace_log_media(count, media, "media post timed post filter:")
+    log.debug(f"filter {count}->  media post timed post filter count: {len(media)}")
+    
+    media = helpers.post_text_filter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media post included text filter:")
-
+    helpers.trace_log_media(count, media, "media text filter:")
     log.debug(
-        f"filter {count}->  all media post included text filter count: {len(media)}"
+        f"filter {count}->  media text filter count: {len(media)}"
     )
-    media = helpers.anti_post_user_filter(media)
+
+    media = helpers.post_neg_text_filter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media post excluded text filter:")
+    helpers.trace_log_media(count, media, "media excluded text filter:")
 
     log.debug(
-        f"filter {count}->  all media post excluded text filter count: {len(media)}"
+        f"filter {count}->  media excluded text filter count: {len(media)}"
     )
+
     media = helpers.download_type_filter(media)
     count += 1
-    helpers.trace_log_media(count, media, "all download type filter:")
-
-    log.debug(f"filter {count}->  all media download type filter count: {len(media)}")
+    helpers.trace_log_media(count, media, "download type filter:")
+    log.debug(f"filter {count}->  media download type filter count: {len(media)}")
 
     media = helpers.mass_msg_filter(media)
     count += 1
     helpers.trace_log_media(count, media, "mass message filter:")
+    log.debug(f"filter {count}->  media mass message filter count: {len(media)}")
+
 
     media = helpers.final_post_sort(media)
     count += 1
-    helpers.trace_log_media(count, media, "all media final sort:")
-    log.debug(f"filter{count}-> all media final sort count {len(media)}")
+    helpers.trace_log_media(count, media, "final sort filter:")
+    log.debug(f"filter {count}->  media final sort filter count: {len(media)}")
+
+    # additional filters
+    if not read_args.retriveArgs().command=="metadata":
+        media = helpers.dupefilter(media)
+        count += 1
+        helpers.trace_log_media(count, media, "media dupe media_id filter:")
+        log.debug(f"filter {count}->  media dupe media_id filter count: {len(media)}")
+        media=helpers.unviewable_media_filter(media)
+        count+=1
+        helpers.trace_log_media(count, media, "unviewable media filter:")
+        log.debug(f"filter {count}->  media unviewable filter count: {len(media)}")
+    elif read_args.retriveArgs().command=="metadata":
+         if constants.getattr("REMOVE_UNVIEWABLE_METADATA"):
+            media=helpers.unviewable_media_filter(media)
+            count+=1
+            helpers.trace_log_media(count, media, "unviewable media filter:")
+            log.debug(f"filter {count}->  media unviewable filter count: {len(media)}")
+    return helpers.previous_download_filter(media,username=username,model_id=model_id)
 
-    return media
 
 
 def filterPost(post):
     count = 1
-    helpers.trace_log_post(count, post, "all post no filter:")
+    helpers.trace_log_post(count, post, "initial posts no filter:")
+    log.debug(f"filter {count}-> initial posts no filter count: {len(post)}")
+    
+    count += 1
+    post = helpers.sort_by_date(post)
+    helpers.trace_log_post(count, post, "post date sort filter:")
+    log.debug(f"filter {count}->  post date sort filter count: {len(post)}")
 
-    log.debug(f"filter {count}-> all post no filter count: {len(post)}")
-    post = helpers.sort_media(post)
     count += 1
-    helpers.trace_log_post(count, post, "final post  from retrived post:")
-
-    log.debug(f"filter {count}->  final post count from retrived post: {len(post)}")
     post = helpers.dupefilter(post)
-    count += 1
-    helpers.trace_log_post(count, post, "all post dupe filter:")
-
-    log.debug(f"filter {count}-> all post dupe filter count: {len(post)}")
-    post = helpers.post_datesorter(post)
-    count += 1
-    helpers.trace_log_post(count, post, "all post datesort:")
+    helpers.trace_log_post(count, post, "post dupe filter:")
+    log.debug(f"filter {count}-> post dupe filter count: {len(post)}")   
 
-    log.debug(f"filter {count}-> all post datesort count: {len(post)}")
-    post = helpers.posts_date_filter(post)
-    count += 1
-    helpers.trace_log_post(count, post, "all post post date filter:")
+    count+=1
+    post = helpers.temp_post_filter(post)
+    log.debug(f"filter {count}-> timed posts filter count: {len(post)}")
+    helpers.trace_log_post(count, post, "timed posts filter:")
 
-    log.debug(f"filter {count}-> all post post date filter: {len(post)}")
-    post = helpers.post_timed_filter(post)
     count += 1
-    helpers.trace_log_post(count, post, "all post post timed post filter:")
+    post = helpers.post_text_filter(post)
+    log.debug(f"filter {count}->  post text filter count: {len(post)}")
+    helpers.trace_log_post(count, post, "post text filter:")
 
-    log.debug(f"filter {count}->  all post post timed post filter count: {len(post)}")
-    post = helpers.post_user_filter(post)
     count += 1
-    helpers.trace_log_post(count, post, "all post post included text filter:")
-
+    post = helpers.post_neg_text_filter(post)
     log.debug(
-        f"filter {count}->  all post post included text filter count: {len(post)}"
+        f"filter {count}->  post excluded text filter count {len(post)}"
     )
-    post = helpers.anti_post_user_filter(post)
-    count += 1
-    helpers.trace_log_post(count, post, "all post post excluded text filter:")
+    helpers.trace_log_post(count, post, "post excluded text filter:")
 
+    count += 1
+    post = helpers.mass_msg_filter(post)
     log.debug(
-        f"filter {count}->  all post post excluded text filter count: {len(post)}"
+        f"filter {count}->  mass msg filter count {len(post)}"
     )
 
-    post = helpers.mass_msg_filter(post)
     count += 1
-    helpers.trace_log_post(count, post, "mass message filter:")
-
     post = helpers.final_post_sort(post)
-    count += 1
     helpers.trace_log_post(count, post, "all post final sort:")
 
     return post
 
 
 def post_filter_for_like(media, like=False):
-    media = helpers.post_timed_filter(media)
+    media = helpers.temp_post_filter(media)
     post_type = "likable" if like else "unlikable"
     log.debug(
         f"[bold]Number of {post_type} posts left after date filter[/bold] {len(media)}"
     )
     media = helpers.final_post_sort(media)
     media = helpers.ele_count_filter(media)
     log.debug(f"[bold]Final Number of open and {post_type} post[/bold] {len(media)}")
```

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/date.py` & `ofscraper-3.9.7/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/flags.py` & `ofscraper-3.9.7/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/helpers.py` & `ofscraper-3.9.7/ofscraper/filters/models/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/other.py` & `ofscraper-3.9.7/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/price.py` & `ofscraper-3.9.7/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/sort.py` & `ofscraper-3.9.7/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.7/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/models/retriver.py` & `ofscraper-3.9.7/ofscraper/models/retriver.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/models/selector.py` & `ofscraper-3.9.7/ofscraper/models/selector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.7/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.7/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.7/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.7/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.7/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/prompts/prompts.py` & `ofscraper-3.9.7/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/runner/exit.py` & `ofscraper-3.9.7/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/runner/load.py` & `ofscraper-3.9.7/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/runner/run.py` & `ofscraper-3.9.7/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/actions.py` & `ofscraper-3.9.7/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/areas.py` & `ofscraper-3.9.7/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_processing.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_processing.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_program.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_program.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_user_filter.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/advanced_user_filter.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/automatic.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/automatic.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/content.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 force_model_unique_option = click.option(
     "-eq",
     "--force-model-unique",
     "--dupe-model-unique",
     "--dupe-model",
     "--force_model_unique",
-    help="Only download files not present for the current model in the database",
+    help="Only download files with media ids not present for the current model in the database",
     default=False,
     is_flag=True,
 )
 
 label_option = click.option(
     "-lb",
     "--label",
```

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/download.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/file.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/logging.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/logging.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/media_type.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/media_type.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/program.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/program.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/user_list.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_list.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/user_select.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_select.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/arguments/user_sort.py` & `ofscraper-3.9.7/ofscraper/utils/args/arguments/user_sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/common.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/main.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/manual.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/message_check.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/message_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/metadata.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/metadata.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/paid_check.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/paid_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/post_check.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/post_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/bundles/story_check.py` & `ofscraper-3.9.7/ofscraper/utils/args/bundles/story_check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.7/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/parse.py` & `ofscraper-3.9.7/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/read.py` & `ofscraper-3.9.7/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/args/user.py` & `ofscraper-3.9.7/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/context.py` & `ofscraper-3.9.7/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/data.py` & `ofscraper-3.9.7/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/file.py` & `ofscraper-3.9.7/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.7/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/make.py` & `ofscraper-3.9.7/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/request.py` & `ofscraper-3.9.7/ofscraper/utils/auth/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     (*values,) = result
 
     request_auth.update(zip(request_auth.keys(), values))
     return request_auth
 
 
 def get_request_auth(forced=False):
-    if (settings.get_dynamic_rules()) in {
+    if not forced and cache.get("api_onlyfans_sign"):
+        return cache.get("api_onlyfans_sign")
+    elif (settings.get_dynamic_rules()) in {
         "deviint",
         "dv",
         "dev",
     }:
 
         return get_request_auth_deviint(forced=forced)
     elif (settings.get_dynamic_rules()) in {
@@ -55,16 +57,14 @@
 
         return get_request_auth_sneaky(forced=forced)
     else:
         return get_request_auth_digitalcriminals(forced=forced)
 
 
 def get_request_auth_deviint(forced=None):
-    if not forced and cache.get("api_onlyfans_sign"):
-        return cache.get("api_onlyfans_sign")
     with sessionManager.sessionManager(
         backend="httpx",
         retries=constants.getattr("GIT_NUM_TRIES"),
         wait_min=constants.getattr("GIT_MIN_WAIT"),
         wait_max=constants.getattr("GIT_MAX_WAIT"),
     ) as c:
         with c.requests(
@@ -83,16 +83,14 @@
                 [static_param, fmt, checksum_indexes, checksum_constant],
                 expire=constants.getattr("HOURLY_EXPIRY"),
             )
             return (static_param, fmt, checksum_indexes, checksum_constant)
 
 
 def get_request_auth_sneaky(forced=None):
-    if not forced and cache.get("api_onlyfans_sign"):
-        return cache.get("api_onlyfans_sign")
     with sessionManager.sessionManager(
         backend="httpx",
         retries=constants.getattr("GIT_NUM_TRIES"),
         wait_min=constants.getattr("GIT_MIN_WAIT"),
         wait_max=constants.getattr("GIT_MAX_WAIT"),
     ) as c:
         with c.requests(
@@ -111,16 +109,14 @@
                 [static_param, fmt, checksum_indexes, checksum_constant],
                 expire=constants.getattr("HOURLY_EXPIRY"),
             )
             return (static_param, fmt, checksum_indexes, checksum_constant)
 
 
 def get_request_auth_digitalcriminals(forced=None):
-    if not forced and cache.get("api_onlyfans_sign"):
-        return cache.get("api_onlyfans_sign")
     with sessionManager.sessionManager(
         backend="httpx",
         retries=constants.getattr("GIT_NUM_TRIES"),
         wait_min=constants.getattr("GIT_MIN_WAIT"),
         wait_max=constants.getattr("GIT_MAX_WAIT"),
     ) as c:
         with c.requests(
```

### Comparing `ofscraper-3.9.6/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.7/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/binaries.py` & `ofscraper-3.9.7/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/cache.py` & `ofscraper-3.9.7/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/checkers.py` & `ofscraper-3.9.7/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/config.py` & `ofscraper-3.9.7/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/context.py` & `ofscraper-3.9.7/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/custom.py` & `ofscraper-3.9.7/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/data.py` & `ofscraper-3.9.7/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/file.py` & `ofscraper-3.9.7/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/menu.py` & `ofscraper-3.9.7/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/config/schema.py` & `ofscraper-3.9.7/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/constants.py` & `ofscraper-3.9.7/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/context/exit.py` & `ofscraper-3.9.7/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.7/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.7/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/dates.py` & `ofscraper-3.9.7/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/encoding.py` & `ofscraper-3.9.7/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/hash.py` & `ofscraper-3.9.7/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.7/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/close.py` & `ofscraper-3.9.7/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.7/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.7/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.7/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/other.py` & `ofscraper-3.9.7/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.7/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/manager.py` & `ofscraper-3.9.7/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/me.py` & `ofscraper-3.9.7/ofscraper/utils/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/menu.py` & `ofscraper-3.9.7/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/merge.py` & `ofscraper-3.9.7/ofscraper/utils/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/paths/check.py` & `ofscraper-3.9.7/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/paths/common.py` & `ofscraper-3.9.7/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/paths/manage.py` & `ofscraper-3.9.7/ofscraper/utils/paths/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.7/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.7/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.7/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.7/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/progress.py` & `ofscraper-3.9.7/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/run.py` & `ofscraper-3.9.7/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/separate.py` & `ofscraper-3.9.7/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/settings.py` & `ofscraper-3.9.7/ofscraper/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/system/network.py` & `ofscraper-3.9.7/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/system/system.py` & `ofscraper-3.9.7/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/ofscraper/utils/text.py` & `ofscraper-3.9.7/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.6/pyproject.toml` & `ofscraper-3.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.6"
+version = "3.9.7"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.6/PKG-INFO` & `ofscraper-3.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.6
+Version: 3.9.7
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.6 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.7 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (==3.9.4) Requires-Dist:
 aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist: browser-cookie3 (==0.19.1)
```

