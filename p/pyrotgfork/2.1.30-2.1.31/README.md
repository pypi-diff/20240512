# Comparing `tmp/pyrotgfork-2.1.30.tar.gz` & `tmp/pyrotgfork-2.1.31.tar.gz`

## Comparing `pyrotgfork-2.1.30.tar` & `pyrotgfork-2.1.31.tar`

### file list

```diff
@@ -1,507 +1,513 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/__init__.py
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   208169 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/api/template/type.txt
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/__init__.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/compiler.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/__init__.py
--rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/client.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/emoji.py
--rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/file_id.py
--rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/py.typed
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/sync.py
--rw-r--r--   0        0        0    17454 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/accent_color.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_description.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_short_description.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_name.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_description.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_short_description.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_name.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/get_business_connection.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/business/get_collectible_item_info.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/close_forum_topic.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/create_forum_topic.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/delete_forum_topic.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/edit_forum_topic.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topics.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/hide_forum_topic.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/reopen_forum_topic.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chat_topics/unhide_forum_topic.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_created_chats.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/search_chats.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_cached_media.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/set_reaction.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/stickers/get_stickers.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_birthdate.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_personal_chat.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/html.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/auth.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/aio_sqlite_storage.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/list.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/object.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/update.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_connection.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_intro.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_location.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours_interval.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/business/collectible_item_info.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/__init__.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_closed.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_created.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_edited.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_reopened.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_media/link_preview_options.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/external_reply_info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_poll_option.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/reply_parameters.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/input_message_content/text_quote.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_import_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_channel.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_chat.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_hidden_user.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_user.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/chat_boost_added.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gifted_premium.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_completed.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_winners.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   194829 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/birthdate.py
--rw-r--r--   0        0        0    47521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    19921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_shared.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/users_shared.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_participants_invited.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/COPYING.lesser
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/NOTICE
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/README.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/hatch_build.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/pyproject.toml
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pyrotgfork-2.1.30/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/__init__.py
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   209214 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/__init__.py
+-rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/client.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/emoji.py
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/py.typed
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/sync.py
+-rw-r--r--   0        0        0    17454 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/accent_color.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_info_description.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_info_short_description.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_name.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_info_description.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_info_short_description.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_name.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/business/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/business/get_business_connection.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/business/get_collectible_item_info.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/__init__.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/close_forum_topic.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/create_forum_topic.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/delete_forum_topic.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/edit_forum_topic.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topic.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topics.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/hide_forum_topic.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/reopen_forum_topic.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chat_topics/unhide_forum_topic.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_created_chats.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/search_chats.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_cached_media.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_chat_sponsored_messages.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/set_reaction.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/view_messages.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/phone/__init__.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/phone/load_group_call_participants.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/stickers/get_stickers.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/set_birthdate.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/set_personal_chat.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/aio_sqlite_storage.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/update.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/business_connection.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/business_intro.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/business_location.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/business_opening_hours.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/business_opening_hours_interval.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/business/collectible_item_info.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/__init__.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_closed.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_created.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_edited.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_media/link_preview_options.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/external_reply_info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_poll_option.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/reply_parameters.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/input_message_content/text_quote.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_import_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_channel.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_chat.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_hidden_user.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_user.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/chat_boost_added.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/gifted_premium.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway_completed.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway_winners.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   197463 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/sponsored_message.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/birthdate.py
+-rw-r--r--   0        0        0    47521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    19921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_shared.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/group_call_participant.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/users_shared.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_participants_invited.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/COPYING.lesser
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/NOTICE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/hatch_build.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/pyproject.toml
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 pyrotgfork-2.1.31/PKG-INFO
```

### Comparing `pyrotgfork-2.1.30/compiler/__init__.py` & `pyrotgfork-2.1.31/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/__init__.py` & `pyrotgfork-2.1.31/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/compiler.py` & `pyrotgfork-2.1.31/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/source/auth_key.tl` & `pyrotgfork-2.1.31/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/source/main_api.tl` & `pyrotgfork-2.1.31/compiler/api/source/main_api.tl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 // https://github.com/telegramdesktop/tdesktop/blob/dev/Telegram/SourceFiles/mtproto/scheme/api.tl
 
 ///////////////////////////////
+/////////////////// Layer cons
+///////////////////////////////
+
+//invokeAfterMsg#cb9f372d msg_id:long query:!X = X;
+//invokeAfterMsgs#3dc4b4f0 msg_ids:Vector<long> query:!X = X;
+//invokeWithLayer1#53835315 query:!X = X;
+//invokeWithLayer2#289dd1f6 query:!X = X;
+//invokeWithLayer3#b7475268 query:!X = X;
+//invokeWithLayer4#dea0d430 query:!X = X;
+//invokeWithLayer5#417a57ae query:!X = X;
+//invokeWithLayer6#3a64d54d query:!X = X;
+//invokeWithLayer7#a5be56d3 query:!X = X;
+//invokeWithLayer8#e9abd9fd query:!X = X;
+//invokeWithLayer9#76715a63 query:!X = X;
+//invokeWithLayer10#39620c41 query:!X = X;
+//invokeWithLayer11#a6b88fdf query:!X = X;
+//invokeWithLayer12#dda60d3c query:!X = X;
+//invokeWithLayer13#427c8ea2 query:!X = X;
+//invokeWithLayer14#2b9b08fa query:!X = X;
+//invokeWithLayer15#b4418b64 query:!X = X;
+//invokeWithLayer16#cf5f0987 query:!X = X;
+//invokeWithLayer17#50858a19 query:!X = X;
+//invokeWithLayer18#1c900537 query:!X = X;
+//invokeWithLayer#da9b0d0d layer:int query:!X = X; // after 18 layer
+
+///////////////////////////////
 ///////// Main application API
 ///////////////////////////////
 
 ---types---
 
 int ? = Int;
 long ? = Long;
```

### Comparing `pyrotgfork-2.1.30/compiler/api/source/sys_msgs.tl` & `pyrotgfork-2.1.31/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/template/combinator.txt` & `pyrotgfork-2.1.31/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/api/template/type.txt` & `pyrotgfork-2.1.31/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/__init__.py` & `pyrotgfork-2.1.31/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/compiler.py` & `pyrotgfork-2.1.31/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/sort.py` & `pyrotgfork-2.1.31/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/403_FORBIDDEN.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/420_FLOOD.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyrotgfork-2.1.31/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/__init__.py` & `pyrotgfork-2.1.31/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "pyrotgfork"
-__version__ = "2.1.30"
+__version__ = "2.1.31"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrotgfork-2.1.30/pyrogram/client.py` & `pyrotgfork-2.1.31/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/dispatcher.py` & `pyrotgfork-2.1.31/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/emoji.py` & `pyrotgfork-2.1.31/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/file_id.py` & `pyrotgfork-2.1.31/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/filters.py` & `pyrotgfork-2.1.31/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/mime_types.py` & `pyrotgfork-2.1.31/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/sync.py` & `pyrotgfork-2.1.31/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/utils.py` & `pyrotgfork-2.1.31/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/__init__.py` & `pyrotgfork-2.1.31/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/connection.py` & `pyrotgfork-2.1.31/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/__init__.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/__init__.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrotgfork-2.1.31/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/crypto/__init__.py` & `pyrotgfork-2.1.31/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/crypto/aes.py` & `pyrotgfork-2.1.31/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/crypto/mtproto.py` & `pyrotgfork-2.1.31/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/crypto/prime.py` & `pyrotgfork-2.1.31/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/crypto/rsa.py` & `pyrotgfork-2.1.31/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/__init__.py` & `pyrotgfork-2.1.31/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/accent_color.py` & `pyrotgfork-2.1.31/pyrogram/enums/accent_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/auto_name.py` & `pyrotgfork-2.1.31/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/chat_action.py` & `pyrotgfork-2.1.31/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/chat_event_action.py` & `pyrotgfork-2.1.31/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/chat_member_status.py` & `pyrotgfork-2.1.31/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/chat_members_filter.py` & `pyrotgfork-2.1.31/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/chat_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/client_platform.py` & `pyrotgfork-2.1.31/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/message_entity_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/message_media_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/message_service_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/messages_filter.py` & `pyrotgfork-2.1.31/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/next_code_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/parse_mode.py` & `pyrotgfork-2.1.31/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/poll_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/profile_color.py` & `pyrotgfork-2.1.31/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/sent_code_type.py` & `pyrotgfork-2.1.31/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/enums/user_status.py` & `pyrotgfork-2.1.31/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/errors/__init__.py` & `pyrotgfork-2.1.31/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/errors/rpc_error.py` & `pyrotgfork-2.1.31/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/__init__.py` & `pyrotgfork-2.1.31/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/callback_query_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/chat_join_request_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/chat_member_updated_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/deleted_messages_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/disconnect_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/edited_message_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/inline_query_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/message_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/poll_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/raw_update_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/handlers/user_status_handler.py` & `pyrotgfork-2.1.31/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .chats import Chats
 from .chat_topics import ChatTopics
 from .contacts import Contacts
 from .decorators import Decorators
 from .invite_links import InviteLinks
 from .messages import Messages
 from .password import Password
+from .phone import Phone
 from .stickers import Stickers
 from .users import Users
 from .utilities import Utilities
 from .business import TelegramBusiness
 
 
 class Methods(
@@ -39,13 +40,14 @@
     Bots,
     Chats,
     ChatTopics,
     Contacts,
     InviteLinks,
     Messages,
     Password,
+    Phone,
     Stickers,
     TelegramBusiness,
     Users,
     Utilities,
 ):
     pass
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/advanced/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/advanced/invoke.py` & `pyrotgfork-2.1.31/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/advanced/resolve_peer.py` & `pyrotgfork-2.1.31/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/advanced/save_file.py` & `pyrotgfork-2.1.31/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/check_password.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/connect.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/disconnect.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/get_password_hint.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/initialize.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/log_out.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/recover_password.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/resend_code.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/send_code.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/send_recovery_code.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_in_bot.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/sign_up.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/auth/terminate.py` & `pyrotgfork-2.1.31/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_callback_query.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_inline_query.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/answer_web_app_query.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/delete_bot_commands.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_commands.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_description.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_info_short_description.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_bot_name.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_game_high_scores.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/request_callback_answer.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/send_game.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_commands.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_description.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_info_short_description.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_bot_name.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/bots/set_game_score.py` & `pyrotgfork-2.1.31/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/business/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/business/get_business_connection.py` & `pyrotgfork-2.1.31/pyrogram/methods/business/get_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/business/get_collectible_item_info.py` & `pyrotgfork-2.1.31/pyrogram/methods/business/get_collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/close_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/create_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/delete_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/edit_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/get_forum_topics.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/hide_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/hide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/reopen_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chat_topics/unhide_forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/methods/chat_topics/unhide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/add_chat_members.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/archive_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/ban_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/create_channel.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/create_group.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/create_supergroup.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_channel.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_chat_photo.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_supergroup.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/delete_user_history.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_event_log.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_members_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_chat_online_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_created_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_created_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_dialogs_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_nearby_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/get_send_as_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/join_chat.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/leave_chat.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/mark_chat_unread.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/pin_chat_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/promote_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/restrict_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/search_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/search_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_administrator_title.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_description.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_permissions.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_photo.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_title.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_ttl.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_chat_username.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_send_as_chat.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/set_slow_mode.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/unarchive_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/unban_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/chats/unpin_chat_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/add_contact.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/delete_contacts.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/get_contacts_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/contacts/import_contacts.py` & `pyrotgfork-2.1.31/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_callback_query.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_disconnect.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_edited_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_inline_query.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_poll.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_raw_update.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/decorators/on_user_status.py` & `pyrotgfork-2.1.31/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 from .send_sticker import SendSticker
 from .send_venue import SendVenue
 from .send_video import SendVideo
 from .send_video_note import SendVideoNote
 from .send_voice import SendVoice
 from .stop_poll import StopPoll
 from .stream_media import StreamMedia
+from .view_messages import ViewMessages
 from .vote_poll import VotePoll
+from .get_chat_sponsored_messages import GetChatSponsoredMessages
 
 
 class Messages(
     CopyMediaGroup,
     CopyMessage,
     DeleteMessages,
     DownloadMedia,
@@ -114,10 +116,12 @@
     SendVenue,
     SendVideo,
     SendVideoNote,
     SendVoice,
     SetReaction,
     StopPoll,
     StreamMedia,
+    ViewMessages,
     VotePoll,
+    GetChatSponsoredMessages,
 ):
     pass
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/copy_media_group.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/copy_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/copy_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
         schedule_date: datetime = None,
+        business_connection_id: str = None,
+        protect_content: bool = None,
+        message_thread_id: int = None,
         reply_to_message_id: int = None
     ) -> "types.Message":
         """Copy messages of any kind.
 
         The method is analogous to the method :meth:`~Client.forward_messages`, but the copied message doesn't have a
         link to the original message.
 
@@ -89,14 +92,23 @@
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
+            business_connection_id (``str``, *optional*):
+                Unique identifier of the business connection on behalf of which the message will be sent
+
+            protect_content (``bool``, *optional*):
+                Protects the contents of the sent message from forwarding and saving
+
+            message_thread_id (``int``, *optional*):
+                Unique identifier for the target message thread (topic) of the forum; for forum supergroups only
+
         Returns:
             :obj:`~pyrogram.types.Message`: On success, the copied message is returned.
 
         Example:
             .. code-block:: python
 
                 # Copy a message
@@ -126,9 +138,12 @@
             chat_id=chat_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
             disable_notification=disable_notification,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
-            schedule_date=schedule_date
+            schedule_date=schedule_date,
+            business_connection_id=business_connection_id,
+            protect_content=protect_content,
+            message_thread_id=message_thread_id
         )
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/delete_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/download_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_cached_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_caption.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_inline_text.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_caption.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/edit_message_text.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/forward_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_chat_history_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_media_group.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/get_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/inline_session.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/read_chat_history.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/retract_vote.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/search_global.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/search_global.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class SearchGlobal:
     async def search_global(
         self: "pyrogram.Client",
         query: str = "",
         filter: "enums.MessagesFilter" = enums.MessagesFilter.EMPTY,
         limit: int = 0,
         chat_list: int = 0,
-        is_channel: bool = False,
+        only_in_channels: bool = False,
     ) -> Optional[AsyncGenerator["types.Message", None]]:
         """Search messages globally from all of your chats.
 
         If you want to get the messages count only, see :meth:`~pyrogram.Client.search_global_count`.
 
         .. note::
 
@@ -56,15 +56,15 @@
             limit (``int``, *optional*):
                 Limits the number of messages to be retrieved.
                 By default, no limit is applied and all messages are returned.
 
             chat_list (``int``, *optional*):
                 Chat list in which to search messages; Only Main (0) and Archive (1) chat lists are supported. Defaults to (0) Main chat list.
 
-            is_channel (``bool``, *optional*):
+            only_in_channels (``bool``, *optional*):
                 True, if should search only in joined channels.
                 Defaults to False. All available chats are searched.
 
         Returns:
             ``Generator``: A generator yielding :obj:`~pyrogram.types.Message` objects.
 
         Example:
@@ -99,15 +99,15 @@
                         min_date=0,
                         max_date=0,
                         offset_rate=offset_date,
                         offset_peer=offset_peer,
                         offset_id=offset_id,
                         limit=limit,
                         folder_id=chat_list,
-                        broadcasts_only=is_channel
+                        broadcasts_only=only_in_channels
                     ),
                     sleep_threshold=60
                 ),
                 replies=0
             )
 
             if not messages:
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/search_global_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/search_global_count.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class SearchGlobalCount:
     async def search_global_count(
         self: "pyrogram.Client",
         query: str = "",
         filter: "enums.MessagesFilter" = enums.MessagesFilter.EMPTY,
         chat_list: int = 0,
-        is_channel: bool = False,
+        only_in_channels: bool = False,
     ) -> int:
         """Get the count of messages resulting from a global search.
 
         If you want to get the actual messages, see :meth:`~pyrogram.Client.search_global`.
 
         .. include:: /_includes/usable-by/users.rst
 
@@ -41,15 +41,15 @@
 
             filter (:obj:`~pyrogram.enums.MessagesFilter`, *optional*):
                 Pass a filter in order to search for specific kind of messages only:
 
             chat_list (``int``, *optional*):
                 Chat list in which to search messages; Only Main (0) and Archive (1) chat lists are supported. Defaults to (0) Main chat list.
 
-            is_channel (``bool``, *optional*):
+            only_in_channels (``bool``, *optional*):
                 True, if should search only in joined channels.
                 Defaults to False. All available chats are searched.
 
         Returns:
             ``int``: On success, the messages count is returned.
         """
         r = await self.invoke(
@@ -59,15 +59,15 @@
                 min_date=0,
                 max_date=0,
                 offset_rate=0,
                 offset_peer=raw.types.InputPeerEmpty(),
                 offset_id=0,
                 limit=1,
                 folder_id=chat_list,
-                broadcasts_only=is_channel
+                broadcasts_only=only_in_channels
             )
         )
 
         if hasattr(r, "count"):
             return r.count
         else:
             return len(r.messages)
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/search_messages_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_animation.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_audio.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_cached_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_chat_action.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_contact.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_dice.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_document.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_location.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_media_group.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_message.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_photo.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_poll.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_sticker.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_venue.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_video.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_video_note.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/send_voice.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/set_reaction.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/set_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/stop_poll.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/stream_media.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/messages/vote_poll.py` & `pyrotgfork-2.1.31/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/password/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/password/change_cloud_password.py` & `pyrotgfork-2.1.31/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/password/enable_cloud_password.py` & `pyrotgfork-2.1.31/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/password/remove_cloud_password.py` & `pyrotgfork-2.1.31/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/stickers/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/stickers/get_stickers.py` & `pyrotgfork-2.1.31/pyrogram/methods/stickers/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/block_user.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/delete_profile_photos.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/delete_profile_photos.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self: "pyrogram.Client",
         photo_ids: Union[str, List[str]] = None,
         public: bool = False,
         for_my_bot: Union[int, str] = None,
     ) -> bool:
         """Delete your own profile photos.
 
-        .. include:: /_includes/usable-by/users.rst
+        .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             photo_ids (``str`` | List of ``str``, *optional*):
                 A single :obj:`~pyrogram.types.Photo` id as string or multiple ids as list of strings for deleting
                 more than one photos at once.
                 If not specified, the most recent profile photo of the user would be deleted.
 
@@ -76,12 +76,14 @@
                     )
                 )
             )
 
         photo_ids = photo_ids if isinstance(photo_ids, list) else [photo_ids]
         input_photos = [utils.get_input_media_from_file_id(i, FileType.PHOTO).id for i in photo_ids]
 
-        return bool(await self.invoke(
-            raw.functions.photos.DeletePhotos(
-                id=input_photos
+        return bool(
+            await self.invoke(
+                raw.functions.photos.DeletePhotos(
+                    id=input_photos
+                )
             )
-        ))
+        )
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_chat_photos.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,20 @@
 class GetChatPhotos:
     async def get_chat_photos(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         limit: int = 0,
     ) -> Optional[AsyncGenerator["types.Photo", None]]:
         """Get a chat or a user profile photos sequentially.
+        
+        .. note::
 
-        .. include:: /_includes/usable-by/users.rst
+            This method works for bot Clients only in :obj:`~pyrogram.enums.ChatType.PRIVATE` and :obj:`~pyrogram.enums.ChatType.GROUP`
+
+        .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
                 For your personal cloud (Saved Messages) you can simply use "me" or "self".
                 For a contact that exists in your Telegram address book you can use his phone number (str).
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_chat_photos_count.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 class GetChatPhotosCount:
     async def get_chat_photos_count(
         self: "pyrogram.Client",
         chat_id: Union[int, str]
     ) -> int:
         """Get the total count of photos for a chat.
 
+        .. note::
+
+            This method works for bot Clients only in :obj:`~pyrogram.enums.ChatType.PRIVATE` and :obj:`~pyrogram.enums.ChatType.GROUP`
+
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
                 For your personal cloud (Saved Messages) you can simply use "me" or "self".
                 For a contact that exists in your Telegram address book you can use his phone number (str).
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_common_chats.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_me.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/get_users.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/set_birthdate.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/set_birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/set_emoji_status.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/set_personal_chat.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/set_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/set_profile_photo.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/set_profile_photo.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,14 @@
         photo_frame_start_timestamp: float = None
     ) -> bool:
         """Set a new profile photo or video (H.264/MPEG-4 AVC video, max 5 seconds).
 
         The ``photo`` and ``video`` arguments are mutually exclusive.
         Pass either one as named argument (see examples below).
 
-        .. note::
-
-            This method only works for Users.
-
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             photo (``str`` | ``BinaryIO``, *optional*):
                 Profile photo to set.
                 Pass a file path as string to upload a new photo that exists on your local machine or
                 pass a binary file-like object with its attribute ".name" set for in-memory uploads.
```

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/set_username.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/unblock_user.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/users/update_profile.py` & `pyrotgfork-2.1.31/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/__init__.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/add_handler.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/compose.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/export_session_string.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/idle.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/remove_handler.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/restart.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/run.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/start.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/stop.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/methods/utilities/stop_transmission.py` & `pyrotgfork-2.1.31/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/parser/__init__.py` & `pyrotgfork-2.1.31/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/parser/html.py` & `pyrotgfork-2.1.31/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/parser/markdown.py` & `pyrotgfork-2.1.31/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/parser/parser.py` & `pyrotgfork-2.1.31/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/parser/utils.py` & `pyrotgfork-2.1.31/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/__init__.py` & `pyrotgfork-2.1.31/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/__init__.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/future_salt.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/future_salts.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/gzip_packed.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/list.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/message.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/msg_container.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/tl_object.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/__init__.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bool.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/bytes.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/double.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/int.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/string.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/raw/core/primitives/vector.py` & `pyrotgfork-2.1.31/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/__init__.py` & `pyrotgfork-2.1.31/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/auth.py` & `pyrotgfork-2.1.31/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/session.py` & `pyrotgfork-2.1.31/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/internals/__init__.py` & `pyrotgfork-2.1.31/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/internals/data_center.py` & `pyrotgfork-2.1.31/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/internals/msg_factory.py` & `pyrotgfork-2.1.31/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/internals/msg_id.py` & `pyrotgfork-2.1.31/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/session/internals/seq_no.py` & `pyrotgfork-2.1.31/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/__init__.py` & `pyrotgfork-2.1.31/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/aio_sqlite_storage.py` & `pyrotgfork-2.1.31/pyrogram/storage/aio_sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/file_storage.py` & `pyrotgfork-2.1.31/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/memory_storage.py` & `pyrotgfork-2.1.31/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/sqlite_storage.py` & `pyrotgfork-2.1.31/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/storage/storage.py` & `pyrotgfork-2.1.31/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/list.py` & `pyrotgfork-2.1.31/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/object.py` & `pyrotgfork-2.1.31/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/update.py` & `pyrotgfork-2.1.31/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/authorization/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/authorization/sent_code.py` & `pyrotgfork-2.1.31/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/authorization/terms_of_service.py` & `pyrotgfork-2.1.31/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,8 +35,10 @@
     ):
         super().__init__()
 
         self.inline_message_id = inline_message_id
 
     @staticmethod
     def _parse(obj: "raw.types.WebViewMessageSent"):
-        return SentWebAppMessage(inline_message_id=utils.pack_inline_message_id(obj.msg_id))
+        return SentWebAppMessage(
+            inline_message_id=utils.pack_inline_message_id(obj.msg_id)
+        ) if obj.msg_id else None
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrotgfork-2.1.31/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/business_connection.py` & `pyrotgfork-2.1.31/pyrogram/types/business/business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/business_intro.py` & `pyrotgfork-2.1.31/pyrogram/types/business/business_intro.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/business_location.py` & `pyrotgfork-2.1.31/pyrogram/types/business/business_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours.py` & `pyrotgfork-2.1.31/pyrogram/types/business/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/business_opening_hours_interval.py` & `pyrotgfork-2.1.31/pyrogram/types/business/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/business/collectible_item_info.py` & `pyrotgfork-2.1.31/pyrogram/types/business/collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_closed.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_created.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_edited.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/forum_topic_reopened.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_hidden.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/chat_topics/general_forum_topic_unhidden.py` & `pyrotgfork-2.1.31/pyrogram/types/chat_topics/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.location = location
         self.inline_message_id = inline_message_id
 
     @staticmethod
     def _parse(client, chosen_inline_result: raw.types.UpdateBotInlineSend, users) -> "ChosenInlineResult":
         inline_message_id = utils.pack_inline_message_id(
             chosen_inline_result.msg_id
-        )
+        ) if chosen_inline_result.msg_id else None
 
         return ChosenInlineResult(
             result_id=str(chosen_inline_result.id),
             from_user=types.User._parse(client, users[chosen_inline_result.user_id]),
             query=chosen_inline_result.query,
             location=types.Location(
                 longitude=chosen_inline_result.geo.long,
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrotgfork-2.1.31/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_animation.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_audio.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_document.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_photo.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_media_video.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/input_phone_contact.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_media/link_preview_options.py` & `pyrotgfork-2.1.31/pyrogram/types/input_media/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/external_reply_info.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_message_content.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_poll_option.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/reply_parameters.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/input_message_content/text_quote.py` & `pyrotgfork-2.1.31/pyrogram/types/input_message_content/text_quote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_import_info.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_import_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_channel.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_chat.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_hidden_user.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_hidden_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/message_origin/message_origin_user.py` & `pyrotgfork-2.1.31/pyrogram/types/message_origin/message_origin_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from .reaction import (
     Reaction,
     ReactionType,
     ReactionTypeEmoji,
     ReactionTypeCustomEmoji,
     ReactionCount
 )
+from .sponsored_message import SponsoredMessage
 from .sticker import Sticker
 from .stripped_thumbnail import StrippedThumbnail
 from .thumbnail import Thumbnail
 from .venue import Venue
 from .video import Video
 from .video_note import VideoNote
 from .voice import Voice
@@ -80,14 +81,15 @@
     "ReactionType",
     "ReactionTypeEmoji",
     "ReactionTypeCustomEmoji",
     "Thumbnail",
     "StrippedThumbnail",
     "Poll",
     "PollOption",
+    "SponsoredMessage",
     "Sticker",
     "Story",
     "Venue",
     "Video",
     "VideoNote",
     "Voice",
     "WebAppData",
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/animation.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/audio.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/chat_boost_added.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/contact.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/dice.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/document.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/game.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gift_code.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/gifted_premium.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/gifted_premium.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_completed.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/giveaway_winners.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/location.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -10190,1988 +10190,2153 @@
 00027cd0: 626f 6172 644d 6172 6b75 7022 2c0a 2020  boardMarkup",.  
 00027ce0: 2020 2020 2020 2020 2020 2274 7970 6573            "types
 00027cf0: 2e52 6570 6c79 4b65 7962 6f61 7264 5265  .ReplyKeyboardRe
 00027d00: 6d6f 7665 222c 0a20 2020 2020 2020 2020  move",.         
 00027d10: 2020 2022 7479 7065 732e 466f 7263 6552     "types.ForceR
 00027d20: 6570 6c79 220a 2020 2020 2020 2020 5d20  eply".        ] 
 00027d30: 3d20 6f62 6a65 6374 2c0a 2020 2020 2020  = object,.      
-00027d40: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00027d50: 6765 5f69 643a 2069 6e74 203d 204e 6f6e  ge_id: int = Non
-00027d60: 652c 0a20 2020 2020 2020 2073 6368 6564  e,.        sched
-00027d70: 756c 655f 6461 7465 3a20 6461 7465 7469  ule_date: dateti
-00027d80: 6d65 203d 204e 6f6e 650a 2020 2020 2920  me = None.    ) 
-00027d90: 2d3e 2055 6e69 6f6e 5b22 7479 7065 732e  -> Union["types.
-00027da0: 4d65 7373 6167 6522 2c20 4c69 7374 5b22  Message", List["
-00027db0: 7479 7065 732e 4d65 7373 6167 6522 5d5d  types.Message"]]
-00027dc0: 3a0a 2020 2020 2020 2020 2222 2242 6f75  :.        """Bou
-00027dd0: 6e64 206d 6574 686f 6420 2a63 6f70 792a  nd method *copy*
-00027de0: 206f 6620 3a6f 626a 3a60 7e70 7972 6f67   of :obj:`~pyrog
-00027df0: 7261 6d2e 7479 7065 732e 4d65 7373 6167  ram.types.Messag
-00027e00: 6560 2e0a 0a20 2020 2020 2020 2055 7365  e`...        Use
-00027e10: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
-00027e20: 6f72 3a0a 0a20 2020 2020 2020 202e 2e20  or:..        .. 
-00027e30: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00027e40: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
-00027e50: 2061 7761 6974 2063 6c69 656e 742e 636f   await client.co
-00027e60: 7079 5f6d 6573 7361 6765 280a 2020 2020  py_message(.    
-00027e70: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00027e80: 5f69 643d 6368 6174 5f69 642c 0a20 2020  _id=chat_id,.   
-00027e90: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-00027ea0: 6d5f 6368 6174 5f69 643d 6d65 7373 6167  m_chat_id=messag
-00027eb0: 652e 6368 6174 2e69 642c 0a20 2020 2020  e.chat.id,.     
-00027ec0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00027ed0: 6765 5f69 643d 6d65 7373 6167 652e 6964  ge_id=message.id
-00027ee0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00027ef0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00027f00: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
-00027f10: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00027f20: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
-00027f30: 2020 2020 2061 7761 6974 206d 6573 7361       await messa
-00027f40: 6765 2e63 6f70 7928 6368 6174 5f69 6429  ge.copy(chat_id)
-00027f50: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00027f60: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-00027f70: 2020 6368 6174 5f69 6420 2860 6069 6e74    chat_id (``int
-00027f80: 6060 207c 2060 6073 7472 6060 293a 0a20  `` | ``str``):. 
-00027f90: 2020 2020 2020 2020 2020 2020 2020 2055                 U
-00027fa0: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
-00027fb0: 2028 696e 7429 206f 7220 7573 6572 6e61   (int) or userna
-00027fc0: 6d65 2028 7374 7229 206f 6620 7468 6520  me (str) of the 
-00027fd0: 7461 7267 6574 2063 6861 742e 0a20 2020  target chat..   
-00027fe0: 2020 2020 2020 2020 2020 2020 2046 6f72               For
-00027ff0: 2079 6f75 7220 7065 7273 6f6e 616c 2063   your personal c
-00028000: 6c6f 7564 2028 5361 7665 6420 4d65 7373  loud (Saved Mess
-00028010: 6167 6573 2920 796f 7520 6361 6e20 7369  ages) you can si
-00028020: 6d70 6c79 2075 7365 2022 6d65 2220 6f72  mply use "me" or
-00028030: 2022 7365 6c66 222e 0a20 2020 2020 2020   "self"..       
-00028040: 2020 2020 2020 2020 2046 6f72 2061 2063           For a c
-00028050: 6f6e 7461 6374 2074 6861 7420 6578 6973  ontact that exis
-00028060: 7473 2069 6e20 796f 7572 2054 656c 6567  ts in your Teleg
-00028070: 7261 6d20 6164 6472 6573 7320 626f 6f6b  ram address book
-00028080: 2079 6f75 2063 616e 2075 7365 2068 6973   you can use his
-00028090: 2070 686f 6e65 206e 756d 6265 7220 2873   phone number (s
-000280a0: 7472 292e 0a0a 2020 2020 2020 2020 2020  tr)...          
-000280b0: 2020 6361 7074 696f 6e20 2860 6073 7472    caption (``str
-000280c0: 696e 6760 602c 202a 6f70 7469 6f6e 616c  ing``, *optional
-000280d0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-000280e0: 2020 2020 4e65 7720 6361 7074 696f 6e20      New caption 
-000280f0: 666f 7220 6d65 6469 612c 2030 2d31 3032  for media, 0-102
-00028100: 3420 6368 6172 6163 7465 7273 2061 6674  4 characters aft
-00028110: 6572 2065 6e74 6974 6965 7320 7061 7273  er entities pars
-00028120: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00028130: 2020 2020 2049 6620 6e6f 7420 7370 6563       If not spec
-00028140: 6966 6965 642c 2074 6865 206f 7269 6769  ified, the origi
-00028150: 6e61 6c20 6361 7074 696f 6e20 6973 206b  nal caption is k
-00028160: 6570 742e 0a20 2020 2020 2020 2020 2020  ept..           
-00028170: 2020 2020 2050 6173 7320 2222 2028 656d       Pass "" (em
-00028180: 7074 7920 7374 7269 6e67 2920 746f 2072  pty string) to r
-00028190: 656d 6f76 6520 7468 6520 6361 7074 696f  emove the captio
-000281a0: 6e2e 0a0a 2020 2020 2020 2020 2020 2020  n...            
-000281b0: 7061 7273 655f 6d6f 6465 2028 3a6f 626a  parse_mode (:obj
-000281c0: 3a60 7e70 7972 6f67 7261 6d2e 656e 756d  :`~pyrogram.enum
-000281d0: 732e 5061 7273 654d 6f64 6560 2c20 2a6f  s.ParseMode`, *o
-000281e0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-000281f0: 2020 2020 2020 2020 2020 2042 7920 6465             By de
-00028200: 6661 756c 742c 2074 6578 7473 2061 7265  fault, texts are
-00028210: 2070 6172 7365 6420 7573 696e 6720 626f   parsed using bo
-00028220: 7468 204d 6172 6b64 6f77 6e20 616e 6420  th Markdown and 
-00028230: 4854 4d4c 2073 7479 6c65 732e 0a20 2020  HTML styles..   
-00028240: 2020 2020 2020 2020 2020 2020 2059 6f75               You
-00028250: 2063 616e 2063 6f6d 6269 6e65 2062 6f74   can combine bot
-00028260: 6820 7379 6e74 6178 6573 2074 6f67 6574  h syntaxes toget
-00028270: 6865 722e 0a0a 2020 2020 2020 2020 2020  her...          
-00028280: 2020 6361 7074 696f 6e5f 656e 7469 7469    caption_entiti
-00028290: 6573 2028 4c69 7374 206f 6620 3a6f 626a  es (List of :obj
-000282a0: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-000282b0: 732e 4d65 7373 6167 6545 6e74 6974 7960  s.MessageEntity`
-000282c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000282d0: 2020 204c 6973 7420 6f66 2073 7065 6369     List of speci
-000282e0: 616c 2065 6e74 6974 6965 7320 7468 6174  al entities that
-000282f0: 2061 7070 6561 7220 696e 2074 6865 206e   appear in the n
-00028300: 6577 2063 6170 7469 6f6e 2c20 7768 6963  ew caption, whic
-00028310: 6820 6361 6e20 6265 2073 7065 6369 6669  h can be specifi
-00028320: 6564 2069 6e73 7465 6164 206f 6620 2a70  ed instead of *p
-00028330: 6172 7365 5f6d 6f64 652a 2e0a 0a20 2020  arse_mode*...   
-00028340: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-00028350: 5f6e 6f74 6966 6963 6174 696f 6e20 2860  _notification (`
-00028360: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
-00028370: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
-00028380: 2020 2020 2020 5365 6e64 7320 7468 6520        Sends the 
-00028390: 6d65 7373 6167 6520 7369 6c65 6e74 6c79  message silently
-000283a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000283b0: 2020 5573 6572 7320 7769 6c6c 2072 6563    Users will rec
-000283c0: 6569 7665 2061 206e 6f74 6966 6963 6174  eive a notificat
-000283d0: 696f 6e20 7769 7468 206e 6f20 736f 756e  ion with no soun
-000283e0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-000283f0: 7265 706c 795f 7061 7261 6d65 7465 7273  reply_parameters
-00028400: 2028 3a6f 626a 3a60 7e70 7972 6f67 7261   (:obj:`~pyrogra
-00028410: 6d2e 7479 7065 732e 5265 706c 7950 6172  m.types.ReplyPar
-00028420: 616d 6574 6572 7360 2c20 2a6f 7074 696f  ameters`, *optio
-00028430: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
-00028440: 2020 2020 2020 2044 6573 6372 6970 7469         Descripti
-00028450: 6f6e 206f 6620 7468 6520 6d65 7373 6167  on of the messag
-00028460: 6520 746f 2072 6570 6c79 2074 6f0a 0a20  e to reply to.. 
-00028470: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00028480: 5f6d 6172 6b75 7020 283a 6f62 6a3a 607e  _markup (:obj:`~
-00028490: 7079 726f 6772 616d 2e74 7970 6573 2e49  pyrogram.types.I
-000284a0: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
-000284b0: 6b75 7060 207c 203a 6f62 6a3a 607e 7079  kup` | :obj:`~py
-000284c0: 726f 6772 616d 2e74 7970 6573 2e52 6570  rogram.types.Rep
-000284d0: 6c79 4b65 7962 6f61 7264 4d61 726b 7570  lyKeyboardMarkup
-000284e0: 6020 7c20 3a6f 626a 3a60 7e70 7972 6f67  ` | :obj:`~pyrog
-000284f0: 7261 6d2e 7479 7065 732e 5265 706c 794b  ram.types.ReplyK
-00028500: 6579 626f 6172 6452 656d 6f76 6560 207c  eyboardRemove` |
-00028510: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
-00028520: 2e74 7970 6573 2e46 6f72 6365 5265 706c  .types.ForceRepl
-00028530: 7960 2c20 2a6f 7074 696f 6e61 6c2a 293a  y`, *optional*):
-00028540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028550: 2041 6464 6974 696f 6e61 6c20 696e 7465   Additional inte
-00028560: 7266 6163 6520 6f70 7469 6f6e 732e 2041  rface options. A
-00028570: 6e20 6f62 6a65 6374 2066 6f72 2061 6e20  n object for an 
-00028580: 696e 6c69 6e65 206b 6579 626f 6172 642c  inline keyboard,
-00028590: 2063 7573 746f 6d20 7265 706c 7920 6b65   custom reply ke
-000285a0: 7962 6f61 7264 2c0a 2020 2020 2020 2020  yboard,.        
-000285b0: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
-000285c0: 696f 6e73 2074 6f20 7265 6d6f 7665 2072  ions to remove r
-000285d0: 6570 6c79 206b 6579 626f 6172 6420 6f72  eply keyboard or
-000285e0: 2074 6f20 666f 7263 6520 6120 7265 706c   to force a repl
-000285f0: 7920 6672 6f6d 2074 6865 2075 7365 722e  y from the user.
-00028600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028610: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
-00028620: 642c 2074 6865 206f 7269 6769 6e61 6c20  d, the original 
-00028630: 7265 706c 7920 6d61 726b 7570 2069 7320  reply markup is 
-00028640: 6b65 7074 2e0a 2020 2020 2020 2020 2020  kept..          
-00028650: 2020 2020 2020 5061 7373 204e 6f6e 6520        Pass None 
-00028660: 746f 2072 656d 6f76 6520 7468 6520 7265  to remove the re
-00028670: 706c 7920 6d61 726b 7570 2e0a 0a20 2020  ply markup...   
-00028680: 2020 2020 2020 2020 2073 6368 6564 756c           schedul
-00028690: 655f 6461 7465 2028 3a70 793a 6f62 6a3a  e_date (:py:obj:
-000286a0: 607e 6461 7465 7469 6d65 2e64 6174 6574  `~datetime.datet
-000286b0: 696d 6560 2c20 2a6f 7074 696f 6e61 6c2a  ime`, *optional*
-000286c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000286d0: 2020 2044 6174 6520 7768 656e 2074 6865     Date when the
-000286e0: 206d 6573 7361 6765 2077 696c 6c20 6265   message will be
-000286f0: 2061 7574 6f6d 6174 6963 616c 6c79 2073   automatically s
-00028700: 656e 742e 0a0a 2020 2020 2020 2020 5265  ent...        Re
-00028710: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00028720: 2020 203a 6f62 6a3a 607e 7079 726f 6772     :obj:`~pyrogr
-00028730: 616d 2e74 7970 6573 2e4d 6573 7361 6765  am.types.Message
-00028740: 603a 204f 6e20 7375 6363 6573 732c 2074  `: On success, t
-00028750: 6865 2063 6f70 6965 6420 6d65 7373 6167  he copied messag
-00028760: 6520 6973 2072 6574 7572 6e65 642e 0a0a  e is returned...
-00028770: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-00028780: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-00028790: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-000287a0: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-000287b0: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
-000287c0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-000287d0: 6c66 2e73 6572 7669 6365 3a0a 2020 2020  lf.service:.    
-000287e0: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
-000287f0: 696e 6728 2253 6572 7669 6365 206d 6573  ing("Service mes
-00028800: 7361 6765 7320 6361 6e6e 6f74 2062 6520  sages cannot be 
-00028810: 636f 7069 6564 2e20 6368 6174 5f69 643a  copied. chat_id:
-00028820: 2025 732c 206d 6573 7361 6765 5f69 643a   %s, message_id:
-00028830: 2025 7322 2c0a 2020 2020 2020 2020 2020   %s",.          
-00028840: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00028850: 6c66 2e63 6861 742e 6964 2c20 7365 6c66  lf.chat.id, self
-00028860: 2e69 6429 0a20 2020 2020 2020 2065 6c69  .id).        eli
-00028870: 6620 7365 6c66 2e67 616d 6520 616e 6420  f self.game and 
-00028880: 6e6f 7420 7365 6c66 2e5f 636c 6965 6e74  not self._client
-00028890: 2e6d 652e 6973 5f62 6f74 3a0a 2020 2020  .me.is_bot:.    
-000288a0: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
-000288b0: 696e 6728 2255 7365 7273 2063 616e 6e6f  ing("Users canno
-000288c0: 7420 7365 6e64 206d 6573 7361 6765 7320  t send messages 
-000288d0: 7769 7468 2047 616d 6520 6d65 6469 6120  with Game media 
-000288e0: 7479 7065 2e20 6368 6174 5f69 643a 2025  type. chat_id: %
-000288f0: 732c 206d 6573 7361 6765 5f69 643a 2025  s, message_id: %
-00028900: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00028910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00028920: 2e63 6861 742e 6964 2c20 7365 6c66 2e69  .chat.id, self.i
-00028930: 6429 0a20 2020 2020 2020 2065 6c69 6620  d).        elif 
-00028940: 7365 6c66 2e65 6d70 7479 3a0a 2020 2020  self.empty:.    
-00028950: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
-00028960: 696e 6728 2245 6d70 7479 206d 6573 7361  ing("Empty messa
-00028970: 6765 7320 6361 6e6e 6f74 2062 6520 636f  ges cannot be co
-00028980: 7069 6564 2e22 290a 2020 2020 2020 2020  pied.").        
-00028990: 656c 6966 2073 656c 662e 7465 7874 3a0a  elif self.text:.
-000289a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000289b0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-000289c0: 6c69 656e 742e 7365 6e64 5f6d 6573 7361  lient.send_messa
-000289d0: 6765 280a 2020 2020 2020 2020 2020 2020  ge(.            
-000289e0: 2020 2020 6368 6174 5f69 643d 6368 6174      chat_id=chat
-000289f0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00028a00: 2020 2020 206d 6573 7361 6765 5f74 6872       message_thr
-00028a10: 6561 645f 6964 3d73 656c 662e 6d65 7373  ead_id=self.mess
-00028a20: 6167 655f 7468 7265 6164 5f69 642c 0a20  age_thread_id,. 
-00028a30: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00028a40: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
-00028a50: 6f6e 5f69 643d 7365 6c66 2e62 7573 696e  on_id=self.busin
-00028a60: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
-00028a70: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00028a80: 2020 2074 6578 743d 7365 6c66 2e74 6578     text=self.tex
-00028a90: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00028aa0: 2020 2070 6172 7365 5f6d 6f64 653d 656e     parse_mode=en
-00028ab0: 756d 732e 5061 7273 654d 6f64 652e 4449  ums.ParseMode.DI
-00028ac0: 5341 424c 4544 2c0a 2020 2020 2020 2020  SABLED,.        
-00028ad0: 2020 2020 2020 2020 656e 7469 7469 6573          entities
-00028ae0: 3d73 656c 662e 656e 7469 7469 6573 2c0a  =self.entities,.
-00028af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b00: 6c69 6e6b 5f70 7265 7669 6577 5f6f 7074  link_preview_opt
-00028b10: 696f 6e73 3d73 656c 662e 6c69 6e6b 5f70  ions=self.link_p
-00028b20: 7265 7669 6577 5f6f 7074 696f 6e73 2c0a  review_options,.
-00028b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028b40: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00028b50: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
-00028b60: 6966 6963 6174 696f 6e2c 0a20 2020 2020  ification,.     
-00028b70: 2020 2020 2020 2020 2020 2070 726f 7465             prote
-00028b80: 6374 5f63 6f6e 7465 6e74 3d73 656c 662e  ct_content=self.
-00028b90: 6861 735f 7072 6f74 6563 7465 645f 636f  has_protected_co
-00028ba0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
-00028bb0: 2020 2020 2020 2072 6570 6c79 5f70 6172         reply_par
-00028bc0: 616d 6574 6572 733d 7265 706c 795f 7061  ameters=reply_pa
-00028bd0: 7261 6d65 7465 7273 2c0a 2020 2020 2020  rameters,.      
-00028be0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00028bf0: 6d61 726b 7570 3d73 656c 662e 7265 706c  markup=self.repl
-00028c00: 795f 6d61 726b 7570 2069 6620 7265 706c  y_markup if repl
-00028c10: 795f 6d61 726b 7570 2069 7320 6f62 6a65  y_markup is obje
-00028c20: 6374 2065 6c73 6520 7265 706c 795f 6d61  ct else reply_ma
-00028c30: 726b 7570 2c0a 2020 2020 2020 2020 2020  rkup,.          
-00028c40: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
-00028c50: 6573 7361 6765 5f69 643d 7265 706c 795f  essage_id=reply_
-00028c60: 746f 5f6d 6573 7361 6765 5f69 642c 0a20  to_message_id,. 
-00028c70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028c80: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
-00028c90: 6564 756c 655f 6461 7465 0a20 2020 2020  edule_date.     
-00028ca0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00028cb0: 2065 6c69 6620 7365 6c66 2e6d 6564 6961   elif self.media
-00028cc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00028cd0: 6e64 5f6d 6564 6961 203d 2070 6172 7469  nd_media = parti
-00028ce0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00028cf0: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-00028d00: 2e73 656e 645f 6361 6368 6564 5f6d 6564  .send_cached_med
-00028d10: 6961 2c0a 2020 2020 2020 2020 2020 2020  ia,.            
-00028d20: 2020 2020 6368 6174 5f69 643d 6368 6174      chat_id=chat
-00028d30: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00028d40: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-00028d50: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
-00028d60: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0a  e_notification,.
-00028d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028d80: 7265 706c 795f 7061 7261 6d65 7465 7273  reply_parameters
-00028d90: 3d72 6570 6c79 5f70 6172 616d 6574 6572  =reply_parameter
-00028da0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00028db0: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-00028dc0: 645f 6964 3d73 656c 662e 6d65 7373 6167  d_id=self.messag
-00028dd0: 655f 7468 7265 6164 5f69 642c 0a20 2020  e_thread_id,.   
-00028de0: 2020 2020 2020 2020 2020 2020 2062 7573               bus
-00028df0: 696e 6573 735f 636f 6e6e 6563 7469 6f6e  iness_connection
-00028e00: 5f69 643d 7365 6c66 2e62 7573 696e 6573  _id=self.busines
-00028e10: 735f 636f 6e6e 6563 7469 6f6e 5f69 642c  s_connection_id,
-00028e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028e30: 2073 6368 6564 756c 655f 6461 7465 3d73   schedule_date=s
-00028e40: 6368 6564 756c 655f 6461 7465 2c0a 2020  chedule_date,.  
-00028e50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00028e60: 6f74 6563 745f 636f 6e74 656e 743d 7365  otect_content=se
-00028e70: 6c66 2e68 6173 5f70 726f 7465 6374 6564  lf.has_protected
-00028e80: 5f63 6f6e 7465 6e74 2c0a 2020 2020 2020  _content,.      
-00028e90: 2020 2020 2020 2020 2020 6861 735f 7370            has_sp
-00028ea0: 6f69 6c65 723d 7365 6c66 2e68 6173 5f6d  oiler=self.has_m
-00028eb0: 6564 6961 5f73 706f 696c 6572 2c0a 2020  edia_spoiler,.  
-00028ec0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00028ed0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00028ee0: 643d 7265 706c 795f 746f 5f6d 6573 7361  d=reply_to_messa
-00028ef0: 6765 5f69 642c 0a20 2020 2020 2020 2020  ge_id,.         
-00028f00: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-00028f10: 6b75 703d 7365 6c66 2e72 6570 6c79 5f6d  kup=self.reply_m
-00028f20: 6172 6b75 7020 6966 2072 6570 6c79 5f6d  arkup if reply_m
-00028f30: 6172 6b75 7020 6973 206f 626a 6563 7420  arkup is object 
-00028f40: 656c 7365 2072 6570 6c79 5f6d 6172 6b75  else reply_marku
-00028f50: 700a 2020 2020 2020 2020 2020 2020 290a  p.            ).
-00028f60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00028f70: 7365 6c66 2e70 686f 746f 3a0a 2020 2020  self.photo:.    
-00028f80: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00028f90: 5f69 6420 3d20 7365 6c66 2e70 686f 746f  _id = self.photo
-00028fa0: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
-00028fb0: 2020 2020 2065 6c69 6620 7365 6c66 2e61       elif self.a
-00028fc0: 7564 696f 3a0a 2020 2020 2020 2020 2020  udio:.          
-00028fd0: 2020 2020 2020 6669 6c65 5f69 6420 3d20        file_id = 
-00028fe0: 7365 6c66 2e61 7564 696f 2e66 696c 655f  self.audio.file_
-00028ff0: 6964 0a20 2020 2020 2020 2020 2020 2065  id.            e
-00029000: 6c69 6620 7365 6c66 2e64 6f63 756d 656e  lif self.documen
-00029010: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00029020: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
-00029030: 662e 646f 6375 6d65 6e74 2e66 696c 655f  f.document.file_
-00029040: 6964 0a20 2020 2020 2020 2020 2020 2065  id.            e
-00029050: 6c69 6620 7365 6c66 2e76 6964 656f 3a0a  lif self.video:.
-00029060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029070: 6669 6c65 5f69 6420 3d20 7365 6c66 2e76  file_id = self.v
-00029080: 6964 656f 2e66 696c 655f 6964 0a20 2020  ideo.file_id.   
-00029090: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
-000290a0: 6c66 2e61 6e69 6d61 7469 6f6e 3a0a 2020  lf.animation:.  
-000290b0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-000290c0: 6c65 5f69 6420 3d20 7365 6c66 2e61 6e69  le_id = self.ani
-000290d0: 6d61 7469 6f6e 2e66 696c 655f 6964 0a20  mation.file_id. 
-000290e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000290f0: 7365 6c66 2e76 6f69 6365 3a0a 2020 2020  self.voice:.    
-00029100: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00029110: 5f69 6420 3d20 7365 6c66 2e76 6f69 6365  _id = self.voice
-00029120: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
-00029130: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
-00029140: 7469 636b 6572 3a0a 2020 2020 2020 2020  ticker:.        
-00029150: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
-00029160: 3d20 7365 6c66 2e73 7469 636b 6572 2e66  = self.sticker.f
-00029170: 696c 655f 6964 0a20 2020 2020 2020 2020  ile_id.         
-00029180: 2020 2065 6c69 6620 7365 6c66 2e76 6964     elif self.vid
-00029190: 656f 5f6e 6f74 653a 0a20 2020 2020 2020  eo_note:.       
-000291a0: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
-000291b0: 203d 2073 656c 662e 7669 6465 6f5f 6e6f   = self.video_no
-000291c0: 7465 2e66 696c 655f 6964 0a20 2020 2020  te.file_id.     
-000291d0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-000291e0: 2e63 6f6e 7461 6374 3a0a 2020 2020 2020  .contact:.      
-000291f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00029200: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
-00029210: 656e 742e 7365 6e64 5f63 6f6e 7461 6374  ent.send_contact
-00029220: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00029230: 2020 2020 2020 6368 6174 5f69 642c 0a20        chat_id,. 
-00029240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029250: 2020 2070 686f 6e65 5f6e 756d 6265 723d     phone_number=
-00029260: 7365 6c66 2e63 6f6e 7461 6374 2e70 686f  self.contact.pho
-00029270: 6e65 5f6e 756d 6265 722c 0a20 2020 2020  ne_number,.     
-00029280: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00029290: 6972 7374 5f6e 616d 653d 7365 6c66 2e63  irst_name=self.c
-000292a0: 6f6e 7461 6374 2e66 6972 7374 5f6e 616d  ontact.first_nam
-000292b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000292c0: 2020 2020 2020 206c 6173 745f 6e61 6d65         last_name
-000292d0: 3d73 656c 662e 636f 6e74 6163 742e 6c61  =self.contact.la
-000292e0: 7374 5f6e 616d 652c 0a20 2020 2020 2020  st_name,.       
-000292f0: 2020 2020 2020 2020 2020 2020 2076 6361               vca
-00029300: 7264 3d73 656c 662e 636f 6e74 6163 742e  rd=self.contact.
-00029310: 7663 6172 642c 0a20 2020 2020 2020 2020  vcard,.         
-00029320: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00029330: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-00029340: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00029350: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00029360: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00029370: 7061 7261 6d65 7465 7273 3d72 6570 6c79  parameters=reply
-00029380: 5f70 6172 616d 6574 6572 732c 0a20 2020  _parameters,.   
-00029390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000293a0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-000293b0: 6964 3d73 656c 662e 6d65 7373 6167 655f  id=self.message_
-000293c0: 7468 7265 6164 5f69 642c 0a20 2020 2020  thread_id,.     
-000293d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000293e0: 7573 696e 6573 735f 636f 6e6e 6563 7469  usiness_connecti
-000293f0: 6f6e 5f69 643d 7365 6c66 2e62 7573 696e  on_id=self.busin
-00029400: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
-00029410: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00029420: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-00029430: 6461 7465 3d73 6368 6564 756c 655f 6461  date=schedule_da
-00029440: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-00029450: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
-00029460: 636f 6e74 656e 743d 7365 6c66 2e68 6173  content=self.has
-00029470: 5f70 726f 7465 6374 6564 5f63 6f6e 7465  _protected_conte
-00029480: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00029490: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-000294a0: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
-000294b0: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
-000294c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000294d0: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
-000294e0: 703d 7365 6c66 2e72 6570 6c79 5f6d 6172  p=self.reply_mar
-000294f0: 6b75 7020 6966 2072 6570 6c79 5f6d 6172  kup if reply_mar
-00029500: 6b75 7020 6973 206f 626a 6563 7420 656c  kup is object el
-00029510: 7365 2072 6570 6c79 5f6d 6172 6b75 700a  se reply_markup.
-00029520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029530: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00029540: 6966 2073 656c 662e 6c6f 6361 7469 6f6e  if self.location
-00029550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00029560: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00029570: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
-00029580: 5f6c 6f63 6174 696f 6e28 0a20 2020 2020  _location(.     
-00029590: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000295a0: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
-000295b0: 2020 2020 2020 2020 2020 2020 6c61 7469              lati
-000295c0: 7475 6465 3d73 656c 662e 6c6f 6361 7469  tude=self.locati
-000295d0: 6f6e 2e6c 6174 6974 7564 652c 0a20 2020  on.latitude,.   
-000295e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000295f0: 206c 6f6e 6769 7475 6465 3d73 656c 662e   longitude=self.
-00029600: 6c6f 6361 7469 6f6e 2e6c 6f6e 6769 7475  location.longitu
-00029610: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-00029620: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-00029630: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-00029640: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00029650: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00029660: 2020 2020 2020 2072 6570 6c79 5f70 6172         reply_par
-00029670: 616d 6574 6572 733d 7265 706c 795f 7061  ameters=reply_pa
-00029680: 7261 6d65 7465 7273 2c0a 2020 2020 2020  rameters,.      
-00029690: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000296a0: 7373 6167 655f 7468 7265 6164 5f69 643d  ssage_thread_id=
-000296b0: 7365 6c66 2e6d 6573 7361 6765 5f74 6872  self.message_thr
-000296c0: 6561 645f 6964 2c0a 2020 2020 2020 2020  ead_id,.        
-000296d0: 2020 2020 2020 2020 2020 2020 6275 7369              busi
-000296e0: 6e65 7373 5f63 6f6e 6e65 6374 696f 6e5f  ness_connection_
-000296f0: 6964 3d73 656c 662e 6275 7369 6e65 7373  id=self.business
-00029700: 5f63 6f6e 6e65 6374 696f 6e5f 6964 2c0a  _connection_id,.
-00029710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029720: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
-00029730: 653d 7363 6865 6475 6c65 5f64 6174 652c  e=schedule_date,
-00029740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029750: 2020 2020 2070 726f 7465 6374 5f63 6f6e       protect_con
-00029760: 7465 6e74 3d73 656c 662e 6861 735f 7072  tent=self.has_pr
-00029770: 6f74 6563 7465 645f 636f 6e74 656e 742c  otected_content,
-00029780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029790: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
-000297a0: 7373 6167 655f 6964 3d72 6570 6c79 5f74  ssage_id=reply_t
-000297b0: 6f5f 6d65 7373 6167 655f 6964 2c0a 2020  o_message_id,.  
-000297c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000297d0: 2020 7265 706c 795f 6d61 726b 7570 3d73    reply_markup=s
-000297e0: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-000297f0: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
-00029800: 2069 7320 6f62 6a65 6374 2065 6c73 6520   is object else 
-00029810: 7265 706c 795f 6d61 726b 7570 0a20 2020  reply_markup.   
-00029820: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00029830: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00029840: 7365 6c66 2e76 656e 7565 3a0a 2020 2020  self.venue:.    
-00029850: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00029860: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-00029870: 6c69 656e 742e 7365 6e64 5f76 656e 7565  lient.send_venue
-00029880: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00029890: 2020 2020 2020 6368 6174 5f69 642c 0a20        chat_id,. 
+00027d40: 2020 7363 6865 6475 6c65 5f64 6174 653a    schedule_date:
+00027d50: 2064 6174 6574 696d 6520 3d20 4e6f 6e65   datetime = None
+00027d60: 2c0a 2020 2020 2020 2020 6275 7369 6e65  ,.        busine
+00027d70: 7373 5f63 6f6e 6e65 6374 696f 6e5f 6964  ss_connection_id
+00027d80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00027d90: 2020 2020 2020 7072 6f74 6563 745f 636f        protect_co
+00027da0: 6e74 656e 743a 2062 6f6f 6c20 3d20 4e6f  ntent: bool = No
+00027db0: 6e65 2c0a 2020 2020 2020 2020 6d65 7373  ne,.        mess
+00027dc0: 6167 655f 7468 7265 6164 5f69 643a 2069  age_thread_id: i
+00027dd0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+00027de0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+00027df0: 6167 655f 6964 3a20 696e 7420 3d20 4e6f  age_id: int = No
+00027e00: 6e65 0a20 2020 2029 202d 3e20 556e 696f  ne.    ) -> Unio
+00027e10: 6e5b 2274 7970 6573 2e4d 6573 7361 6765  n["types.Message
+00027e20: 222c 204c 6973 745b 2274 7970 6573 2e4d  ", List["types.M
+00027e30: 6573 7361 6765 225d 5d3a 0a20 2020 2020  essage"]]:.     
+00027e40: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+00027e50: 6f64 202a 636f 7079 2a20 6f66 203a 6f62  od *copy* of :ob
+00027e60: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+00027e70: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
+00027e80: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+00027e90: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
+00027ea0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+00027eb0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+00027ec0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00027ed0: 636c 6965 6e74 2e63 6f70 795f 6d65 7373  client.copy_mess
+00027ee0: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
+00027ef0: 2020 2020 2063 6861 745f 6964 3d63 6861       chat_id=cha
+00027f00: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+00027f10: 2020 2020 2020 6672 6f6d 5f63 6861 745f        from_chat_
+00027f20: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
+00027f30: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00027f40: 2020 2020 6d65 7373 6167 655f 6964 3d6d      message_id=m
+00027f50: 6573 7361 6765 2e69 640a 2020 2020 2020  essage.id.      
+00027f60: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00027f70: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00027f80: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+00027f90: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+00027fa0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00027fb0: 6169 7420 6d65 7373 6167 652e 636f 7079  ait message.copy
+00027fc0: 2863 6861 745f 6964 290a 0a20 2020 2020  (chat_id)..     
+00027fd0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+00027fe0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00027ff0: 6964 2028 6060 696e 7460 6020 7c20 6060  id (``int`` | ``
+00028000: 7374 7260 6029 3a0a 2020 2020 2020 2020  str``):.        
+00028010: 2020 2020 2020 2020 556e 6971 7565 2069          Unique i
+00028020: 6465 6e74 6966 6965 7220 2869 6e74 2920  dentifier (int) 
+00028030: 6f72 2075 7365 726e 616d 6520 2873 7472  or username (str
+00028040: 2920 6f66 2074 6865 2074 6172 6765 7420  ) of the target 
+00028050: 6368 6174 2e0a 2020 2020 2020 2020 2020  chat..          
+00028060: 2020 2020 2020 466f 7220 796f 7572 2070        For your p
+00028070: 6572 736f 6e61 6c20 636c 6f75 6420 2853  ersonal cloud (S
+00028080: 6176 6564 204d 6573 7361 6765 7329 2079  aved Messages) y
+00028090: 6f75 2063 616e 2073 696d 706c 7920 7573  ou can simply us
+000280a0: 6520 226d 6522 206f 7220 2273 656c 6622  e "me" or "self"
+000280b0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000280c0: 2020 466f 7220 6120 636f 6e74 6163 7420    For a contact 
+000280d0: 7468 6174 2065 7869 7374 7320 696e 2079  that exists in y
+000280e0: 6f75 7220 5465 6c65 6772 616d 2061 6464  our Telegram add
+000280f0: 7265 7373 2062 6f6f 6b20 796f 7520 6361  ress book you ca
+00028100: 6e20 7573 6520 6869 7320 7068 6f6e 6520  n use his phone 
+00028110: 6e75 6d62 6572 2028 7374 7229 2e0a 0a20  number (str)... 
+00028120: 2020 2020 2020 2020 2020 2063 6170 7469             capti
+00028130: 6f6e 2028 6060 7374 7269 6e67 6060 2c20  on (``string``, 
+00028140: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+00028150: 2020 2020 2020 2020 2020 2020 204e 6577               New
+00028160: 2063 6170 7469 6f6e 2066 6f72 206d 6564   caption for med
+00028170: 6961 2c20 302d 3130 3234 2063 6861 7261  ia, 0-1024 chara
+00028180: 6374 6572 7320 6166 7465 7220 656e 7469  cters after enti
+00028190: 7469 6573 2070 6172 7369 6e67 2e0a 2020  ties parsing..  
+000281a0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+000281b0: 206e 6f74 2073 7065 6369 6669 6564 2c20   not specified, 
+000281c0: 7468 6520 6f72 6967 696e 616c 2063 6170  the original cap
+000281d0: 7469 6f6e 2069 7320 6b65 7074 2e0a 2020  tion is kept..  
+000281e0: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+000281f0: 7373 2022 2220 2865 6d70 7479 2073 7472  ss "" (empty str
+00028200: 696e 6729 2074 6f20 7265 6d6f 7665 2074  ing) to remove t
+00028210: 6865 2063 6170 7469 6f6e 2e0a 0a20 2020  he caption...   
+00028220: 2020 2020 2020 2020 2070 6172 7365 5f6d           parse_m
+00028230: 6f64 6520 283a 6f62 6a3a 607e 7079 726f  ode (:obj:`~pyro
+00028240: 6772 616d 2e65 6e75 6d73 2e50 6172 7365  gram.enums.Parse
+00028250: 4d6f 6465 602c 202a 6f70 7469 6f6e 616c  Mode`, *optional
+00028260: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
+00028270: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
+00028280: 7465 7874 7320 6172 6520 7061 7273 6564  texts are parsed
+00028290: 2075 7369 6e67 2062 6f74 6820 4d61 726b   using both Mark
+000282a0: 646f 776e 2061 6e64 2048 544d 4c20 7374  down and HTML st
+000282b0: 796c 6573 2e0a 2020 2020 2020 2020 2020  yles..          
+000282c0: 2020 2020 2020 596f 7520 6361 6e20 636f        You can co
+000282d0: 6d62 696e 6520 626f 7468 2073 796e 7461  mbine both synta
+000282e0: 7865 7320 746f 6765 7468 6572 2e0a 0a20  xes together... 
+000282f0: 2020 2020 2020 2020 2020 2063 6170 7469             capti
+00028300: 6f6e 5f65 6e74 6974 6965 7320 284c 6973  on_entities (Lis
+00028310: 7420 6f66 203a 6f62 6a3a 607e 7079 726f  t of :obj:`~pyro
+00028320: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
+00028330: 6765 456e 7469 7479 6029 3a0a 2020 2020  geEntity`):.    
+00028340: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00028350: 206f 6620 7370 6563 6961 6c20 656e 7469   of special enti
+00028360: 7469 6573 2074 6861 7420 6170 7065 6172  ties that appear
+00028370: 2069 6e20 7468 6520 6e65 7720 6361 7074   in the new capt
+00028380: 696f 6e2c 2077 6869 6368 2063 616e 2062  ion, which can b
+00028390: 6520 7370 6563 6966 6965 6420 696e 7374  e specified inst
+000283a0: 6561 6420 6f66 202a 7061 7273 655f 6d6f  ead of *parse_mo
+000283b0: 6465 2a2e 0a0a 2020 2020 2020 2020 2020  de*...          
+000283c0: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+000283d0: 6361 7469 6f6e 2028 6060 626f 6f6c 6060  cation (``bool``
+000283e0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+000283f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00028400: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
+00028410: 2073 696c 656e 746c 792e 0a20 2020 2020   silently..     
+00028420: 2020 2020 2020 2020 2020 2055 7365 7273             Users
+00028430: 2077 696c 6c20 7265 6365 6976 6520 6120   will receive a 
+00028440: 6e6f 7469 6669 6361 7469 6f6e 2077 6974  notification wit
+00028450: 6820 6e6f 2073 6f75 6e64 2e0a 0a20 2020  h no sound...   
+00028460: 2020 2020 2020 2020 2072 6570 6c79 5f70           reply_p
+00028470: 6172 616d 6574 6572 7320 283a 6f62 6a3a  arameters (:obj:
+00028480: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
+00028490: 2e52 6570 6c79 5061 7261 6d65 7465 7273  .ReplyParameters
+000284a0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+000284b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000284c0: 4465 7363 7269 7074 696f 6e20 6f66 2074  Description of t
+000284d0: 6865 206d 6573 7361 6765 2074 6f20 7265  he message to re
+000284e0: 706c 7920 746f 0a0a 2020 2020 2020 2020  ply to..        
+000284f0: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
+00028500: 2028 3a6f 626a 3a60 7e70 7972 6f67 7261   (:obj:`~pyrogra
+00028510: 6d2e 7479 7065 732e 496e 6c69 6e65 4b65  m.types.InlineKe
+00028520: 7962 6f61 7264 4d61 726b 7570 6020 7c20  yboardMarkup` | 
+00028530: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00028540: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
+00028550: 6172 644d 6172 6b75 7060 207c 203a 6f62  ardMarkup` | :ob
+00028560: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+00028570: 6573 2e52 6570 6c79 4b65 7962 6f61 7264  es.ReplyKeyboard
+00028580: 5265 6d6f 7665 6020 7c20 3a6f 626a 3a60  Remove` | :obj:`
+00028590: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+000285a0: 466f 7263 6552 6570 6c79 602c 202a 6f70  ForceReply`, *op
+000285b0: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+000285c0: 2020 2020 2020 2020 2020 4164 6469 7469            Additi
+000285d0: 6f6e 616c 2069 6e74 6572 6661 6365 206f  onal interface o
+000285e0: 7074 696f 6e73 2e20 416e 206f 626a 6563  ptions. An objec
+000285f0: 7420 666f 7220 616e 2069 6e6c 696e 6520  t for an inline 
+00028600: 6b65 7962 6f61 7264 2c20 6375 7374 6f6d  keyboard, custom
+00028610: 2072 6570 6c79 206b 6579 626f 6172 642c   reply keyboard,
+00028620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028630: 2069 6e73 7472 7563 7469 6f6e 7320 746f   instructions to
+00028640: 2072 656d 6f76 6520 7265 706c 7920 6b65   remove reply ke
+00028650: 7962 6f61 7264 206f 7220 746f 2066 6f72  yboard or to for
+00028660: 6365 2061 2072 6570 6c79 2066 726f 6d20  ce a reply from 
+00028670: 7468 6520 7573 6572 2e0a 2020 2020 2020  the user..      
+00028680: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
+00028690: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
+000286a0: 6f72 6967 696e 616c 2072 6570 6c79 206d  original reply m
+000286b0: 6172 6b75 7020 6973 206b 6570 742e 0a20  arkup is kept.. 
+000286c0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+000286d0: 6173 7320 4e6f 6e65 2074 6f20 7265 6d6f  ass None to remo
+000286e0: 7665 2074 6865 2072 6570 6c79 206d 6172  ve the reply mar
+000286f0: 6b75 702e 0a0a 2020 2020 2020 2020 2020  kup...          
+00028700: 2020 7363 6865 6475 6c65 5f64 6174 6520    schedule_date 
+00028710: 283a 7079 3a6f 626a 3a60 7e64 6174 6574  (:py:obj:`~datet
+00028720: 696d 652e 6461 7465 7469 6d65 602c 202a  ime.datetime`, *
+00028730: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+00028740: 2020 2020 2020 2020 2020 2020 4461 7465              Date
+00028750: 2077 6865 6e20 7468 6520 6d65 7373 6167   when the messag
+00028760: 6520 7769 6c6c 2062 6520 6175 746f 6d61  e will be automa
+00028770: 7469 6361 6c6c 7920 7365 6e74 2e0a 0a20  tically sent... 
+00028780: 2020 2020 2020 2020 2020 2062 7573 696e             busin
+00028790: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
+000287a0: 6420 2860 6073 7472 6060 2c20 2a6f 7074  d (``str``, *opt
+000287b0: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+000287c0: 2020 2020 2020 2020 2055 6e69 7175 6520           Unique 
+000287d0: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
+000287e0: 6520 6275 7369 6e65 7373 2063 6f6e 6e65  e business conne
+000287f0: 6374 696f 6e20 6f6e 2062 6568 616c 6620  ction on behalf 
+00028800: 6f66 2077 6869 6368 2074 6865 206d 6573  of which the mes
+00028810: 7361 6765 2077 696c 6c20 6265 2073 656e  sage will be sen
+00028820: 740a 0a20 2020 2020 2020 2020 2020 2070  t..            p
+00028830: 726f 7465 6374 5f63 6f6e 7465 6e74 2028  rotect_content (
+00028840: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
+00028850: 6e61 6c2a 293a 0a20 2020 2020 2020 2020  nal*):.         
+00028860: 2020 2020 2020 2050 726f 7465 6374 7320         Protects 
+00028870: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+00028880: 7468 6520 7365 6e74 206d 6573 7361 6765  the sent message
+00028890: 2066 726f 6d20 666f 7277 6172 6469 6e67   from forwarding
+000288a0: 2061 6e64 2073 6176 696e 670a 0a20 2020   and saving..   
+000288b0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000288c0: 5f74 6872 6561 645f 6964 2028 6060 696e  _thread_id (``in
+000288d0: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+000288e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000288f0: 2020 556e 6971 7565 2069 6465 6e74 6966    Unique identif
+00028900: 6965 7220 666f 7220 7468 6520 7461 7267  ier for the targ
+00028910: 6574 206d 6573 7361 6765 2074 6872 6561  et message threa
+00028920: 6420 2874 6f70 6963 2920 6f66 2074 6865  d (topic) of the
+00028930: 2066 6f72 756d 3b20 666f 7220 666f 7275   forum; for foru
+00028940: 6d20 7375 7065 7267 726f 7570 7320 6f6e  m supergroups on
+00028950: 6c79 0a0a 2020 2020 2020 2020 5265 7475  ly..        Retu
+00028960: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00028970: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+00028980: 2e74 7970 6573 2e4d 6573 7361 6765 603a  .types.Message`:
+00028990: 204f 6e20 7375 6363 6573 732c 2074 6865   On success, the
+000289a0: 2063 6f70 6965 6420 6d65 7373 6167 6520   copied message 
+000289b0: 6973 2072 6574 7572 6e65 642e 0a0a 2020  is returned...  
+000289c0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+000289d0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+000289e0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+000289f0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+00028a00: 726f 722e 0a20 2020 2020 2020 2022 2222  ror..        """
+00028a10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028a20: 2e73 6572 7669 6365 3a0a 2020 2020 2020  .service:.      
+00028a30: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+00028a40: 6728 2253 6572 7669 6365 206d 6573 7361  g("Service messa
+00028a50: 6765 7320 6361 6e6e 6f74 2062 6520 636f  ges cannot be co
+00028a60: 7069 6564 2e20 6368 6174 5f69 643a 2025  pied. chat_id: %
+00028a70: 732c 206d 6573 7361 6765 5f69 643a 2025  s, message_id: %
+00028a80: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00028a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00028aa0: 2e63 6861 742e 6964 2c20 7365 6c66 2e69  .chat.id, self.i
+00028ab0: 6429 0a20 2020 2020 2020 2065 6c69 6620  d).        elif 
+00028ac0: 7365 6c66 2e67 616d 6520 616e 6420 6e6f  self.game and no
+00028ad0: 7420 7365 6c66 2e5f 636c 6965 6e74 2e6d  t self._client.m
+00028ae0: 652e 6973 5f62 6f74 3a0a 2020 2020 2020  e.is_bot:.      
+00028af0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+00028b00: 6728 2255 7365 7273 2063 616e 6e6f 7420  g("Users cannot 
+00028b10: 7365 6e64 206d 6573 7361 6765 7320 7769  send messages wi
+00028b20: 7468 2047 616d 6520 6d65 6469 6120 7479  th Game media ty
+00028b30: 7065 2e20 6368 6174 5f69 643a 2025 732c  pe. chat_id: %s,
+00028b40: 206d 6573 7361 6765 5f69 643a 2025 7322   message_id: %s"
+00028b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00028b60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00028b70: 6861 742e 6964 2c20 7365 6c66 2e69 6429  hat.id, self.id)
+00028b80: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+00028b90: 6c66 2e65 6d70 7479 3a0a 2020 2020 2020  lf.empty:.      
+00028ba0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+00028bb0: 6728 2245 6d70 7479 206d 6573 7361 6765  g("Empty message
+00028bc0: 7320 6361 6e6e 6f74 2062 6520 636f 7069  s cannot be copi
+00028bd0: 6564 2e22 290a 2020 2020 2020 2020 656c  ed.").        el
+00028be0: 6966 2073 656c 662e 7465 7874 3a0a 2020  if self.text:.  
+00028bf0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00028c00: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+00028c10: 656e 742e 7365 6e64 5f6d 6573 7361 6765  ent.send_message
+00028c20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00028c30: 2020 6368 6174 5f69 643d 6368 6174 5f69    chat_id=chat_i
+00028c40: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00028c50: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+00028c60: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
+00028c70: 6561 645f 6964 206f 7220 7365 6c66 2e6d  ead_id or self.m
+00028c80: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00028c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00028ca0: 2020 6275 7369 6e65 7373 5f63 6f6e 6e65    business_conne
+00028cb0: 6374 696f 6e5f 6964 3d62 7573 696e 6573  ction_id=busines
+00028cc0: 735f 636f 6e6e 6563 7469 6f6e 5f69 6420  s_connection_id 
+00028cd0: 6f72 2073 656c 662e 6275 7369 6e65 7373  or self.business
+00028ce0: 5f63 6f6e 6e65 6374 696f 6e5f 6964 2c0a  _connection_id,.
+00028cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d00: 7465 7874 3d73 656c 662e 7465 7874 2c0a  text=self.text,.
+00028d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d20: 7061 7273 655f 6d6f 6465 3d65 6e75 6d73  parse_mode=enums
+00028d30: 2e50 6172 7365 4d6f 6465 2e44 4953 4142  .ParseMode.DISAB
+00028d40: 4c45 442c 0a20 2020 2020 2020 2020 2020  LED,.           
+00028d50: 2020 2020 2065 6e74 6974 6965 733d 7365       entities=se
+00028d60: 6c66 2e65 6e74 6974 6965 732c 0a20 2020  lf.entities,.   
+00028d70: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+00028d80: 6b5f 7072 6576 6965 775f 6f70 7469 6f6e  k_preview_option
+00028d90: 733d 7365 6c66 2e6c 696e 6b5f 7072 6576  s=self.link_prev
+00028da0: 6965 775f 6f70 7469 6f6e 732c 0a20 2020  iew_options,.   
+00028db0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00028dc0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00028dd0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+00028de0: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
+00028df0: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
+00028e00: 636f 6e74 656e 743d 7072 6f74 6563 745f  content=protect_
+00028e10: 636f 6e74 656e 7420 6f72 2073 656c 662e  content or self.
+00028e20: 6861 735f 7072 6f74 6563 7465 645f 636f  has_protected_co
+00028e30: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
+00028e40: 2020 2020 2020 2072 6570 6c79 5f70 6172         reply_par
+00028e50: 616d 6574 6572 733d 7265 706c 795f 7061  ameters=reply_pa
+00028e60: 7261 6d65 7465 7273 2c0a 2020 2020 2020  rameters,.      
+00028e70: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00028e80: 6d61 726b 7570 3d73 656c 662e 7265 706c  markup=self.repl
+00028e90: 795f 6d61 726b 7570 2069 6620 7265 706c  y_markup if repl
+00028ea0: 795f 6d61 726b 7570 2069 7320 6f62 6a65  y_markup is obje
+00028eb0: 6374 2065 6c73 6520 7265 706c 795f 6d61  ct else reply_ma
+00028ec0: 726b 7570 2c0a 2020 2020 2020 2020 2020  rkup,.          
+00028ed0: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
+00028ee0: 6573 7361 6765 5f69 643d 7265 706c 795f  essage_id=reply_
+00028ef0: 746f 5f6d 6573 7361 6765 5f69 642c 0a20  to_message_id,. 
+00028f00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00028f10: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
+00028f20: 6564 756c 655f 6461 7465 0a20 2020 2020  edule_date.     
+00028f30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00028f40: 2065 6c69 6620 7365 6c66 2e6d 6564 6961   elif self.media
+00028f50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00028f60: 6e64 5f6d 6564 6961 203d 2070 6172 7469  nd_media = parti
+00028f70: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00028f80: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
+00028f90: 2e73 656e 645f 6361 6368 6564 5f6d 6564  .send_cached_med
+00028fa0: 6961 2c0a 2020 2020 2020 2020 2020 2020  ia,.            
+00028fb0: 2020 2020 6368 6174 5f69 643d 6368 6174      chat_id=chat
+00028fc0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00028fd0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00028fe0: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
+00028ff0: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0a  e_notification,.
+00029000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029010: 7265 706c 795f 7061 7261 6d65 7465 7273  reply_parameters
+00029020: 3d72 6570 6c79 5f70 6172 616d 6574 6572  =reply_parameter
+00029030: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00029040: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+00029050: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
+00029060: 6561 645f 6964 206f 7220 7365 6c66 2e6d  ead_id or self.m
+00029070: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00029080: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029090: 2020 6275 7369 6e65 7373 5f63 6f6e 6e65    business_conne
+000290a0: 6374 696f 6e5f 6964 3d62 7573 696e 6573  ction_id=busines
+000290b0: 735f 636f 6e6e 6563 7469 6f6e 5f69 6420  s_connection_id 
+000290c0: 6f72 2073 656c 662e 6275 7369 6e65 7373  or self.business
+000290d0: 5f63 6f6e 6e65 6374 696f 6e5f 6964 2c0a  _connection_id,.
+000290e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000290f0: 7363 6865 6475 6c65 5f64 6174 653d 7363  schedule_date=sc
+00029100: 6865 6475 6c65 5f64 6174 652c 0a20 2020  hedule_date,.   
+00029110: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+00029120: 7465 6374 5f63 6f6e 7465 6e74 3d70 726f  tect_content=pro
+00029130: 7465 6374 5f63 6f6e 7465 6e74 206f 7220  tect_content or 
+00029140: 7365 6c66 2e68 6173 5f70 726f 7465 6374  self.has_protect
+00029150: 6564 5f63 6f6e 7465 6e74 2c0a 2020 2020  ed_content,.    
+00029160: 2020 2020 2020 2020 2020 2020 6861 735f              has_
+00029170: 7370 6f69 6c65 723d 7365 6c66 2e68 6173  spoiler=self.has
+00029180: 5f6d 6564 6961 5f73 706f 696c 6572 2c0a  _media_spoiler,.
+00029190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000291a0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+000291b0: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
+000291c0: 7361 6765 5f69 642c 0a20 2020 2020 2020  sage_id,.       
+000291d0: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+000291e0: 6172 6b75 703d 7365 6c66 2e72 6570 6c79  arkup=self.reply
+000291f0: 5f6d 6172 6b75 7020 6966 2072 6570 6c79  _markup if reply
+00029200: 5f6d 6172 6b75 7020 6973 206f 626a 6563  _markup is objec
+00029210: 7420 656c 7365 2072 6570 6c79 5f6d 6172  t else reply_mar
+00029220: 6b75 700a 2020 2020 2020 2020 2020 2020  kup.            
+00029230: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00029240: 6620 7365 6c66 2e70 686f 746f 3a0a 2020  f self.photo:.  
+00029250: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00029260: 6c65 5f69 6420 3d20 7365 6c66 2e70 686f  le_id = self.pho
+00029270: 746f 2e66 696c 655f 6964 0a20 2020 2020  to.file_id.     
+00029280: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00029290: 2e61 7564 696f 3a0a 2020 2020 2020 2020  .audio:.        
+000292a0: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
+000292b0: 3d20 7365 6c66 2e61 7564 696f 2e66 696c  = self.audio.fil
+000292c0: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
+000292d0: 2065 6c69 6620 7365 6c66 2e64 6f63 756d   elif self.docum
+000292e0: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+000292f0: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
+00029300: 656c 662e 646f 6375 6d65 6e74 2e66 696c  elf.document.fil
+00029310: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
+00029320: 2065 6c69 6620 7365 6c66 2e76 6964 656f   elif self.video
+00029330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00029340: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
+00029350: 2e76 6964 656f 2e66 696c 655f 6964 0a20  .video.file_id. 
+00029360: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00029370: 7365 6c66 2e61 6e69 6d61 7469 6f6e 3a0a  self.animation:.
+00029380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029390: 6669 6c65 5f69 6420 3d20 7365 6c66 2e61  file_id = self.a
+000293a0: 6e69 6d61 7469 6f6e 2e66 696c 655f 6964  nimation.file_id
+000293b0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000293c0: 6620 7365 6c66 2e76 6f69 6365 3a0a 2020  f self.voice:.  
+000293d0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000293e0: 6c65 5f69 6420 3d20 7365 6c66 2e76 6f69  le_id = self.voi
+000293f0: 6365 2e66 696c 655f 6964 0a20 2020 2020  ce.file_id.     
+00029400: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00029410: 2e73 7469 636b 6572 3a0a 2020 2020 2020  .sticker:.      
+00029420: 2020 2020 2020 2020 2020 6669 6c65 5f69            file_i
+00029430: 6420 3d20 7365 6c66 2e73 7469 636b 6572  d = self.sticker
+00029440: 2e66 696c 655f 6964 0a20 2020 2020 2020  .file_id.       
+00029450: 2020 2020 2065 6c69 6620 7365 6c66 2e76       elif self.v
+00029460: 6964 656f 5f6e 6f74 653a 0a20 2020 2020  ideo_note:.     
+00029470: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00029480: 6964 203d 2073 656c 662e 7669 6465 6f5f  id = self.video_
+00029490: 6e6f 7465 2e66 696c 655f 6964 0a20 2020  note.file_id.   
+000294a0: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+000294b0: 6c66 2e63 6f6e 7461 6374 3a0a 2020 2020  lf.contact:.    
+000294c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000294d0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
+000294e0: 6c69 656e 742e 7365 6e64 5f63 6f6e 7461  lient.send_conta
+000294f0: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+00029500: 2020 2020 2020 2020 6368 6174 5f69 642c          chat_id,
+00029510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029520: 2020 2020 2070 686f 6e65 5f6e 756d 6265       phone_numbe
+00029530: 723d 7365 6c66 2e63 6f6e 7461 6374 2e70  r=self.contact.p
+00029540: 686f 6e65 5f6e 756d 6265 722c 0a20 2020  hone_number,.   
+00029550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029560: 2066 6972 7374 5f6e 616d 653d 7365 6c66   first_name=self
+00029570: 2e63 6f6e 7461 6374 2e66 6972 7374 5f6e  .contact.first_n
+00029580: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00029590: 2020 2020 2020 2020 206c 6173 745f 6e61           last_na
+000295a0: 6d65 3d73 656c 662e 636f 6e74 6163 742e  me=self.contact.
+000295b0: 6c61 7374 5f6e 616d 652c 0a20 2020 2020  last_name,.     
+000295c0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000295d0: 6361 7264 3d73 656c 662e 636f 6e74 6163  card=self.contac
+000295e0: 742e 7663 6172 642c 0a20 2020 2020 2020  t.vcard,.       
+000295f0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00029600: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00029610: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+00029620: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
+00029630: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00029640: 795f 7061 7261 6d65 7465 7273 3d72 6570  y_parameters=rep
+00029650: 6c79 5f70 6172 616d 6574 6572 732c 0a20  ly_parameters,. 
+00029660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029670: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+00029680: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
+00029690: 6561 645f 6964 206f 7220 7365 6c66 2e6d  ead_id or self.m
+000296a0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000296b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000296c0: 2020 2020 2020 6275 7369 6e65 7373 5f63        business_c
+000296d0: 6f6e 6e65 6374 696f 6e5f 6964 3d62 7573  onnection_id=bus
+000296e0: 696e 6573 735f 636f 6e6e 6563 7469 6f6e  iness_connection
+000296f0: 5f69 6420 6f72 2073 656c 662e 6275 7369  _id or self.busi
+00029700: 6e65 7373 5f63 6f6e 6e65 6374 696f 6e5f  ness_connection_
+00029710: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00029720: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+00029730: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+00029740: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+00029750: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+00029760: 5f63 6f6e 7465 6e74 3d70 726f 7465 6374  _content=protect
+00029770: 5f63 6f6e 7465 6e74 206f 7220 7365 6c66  _content or self
+00029780: 2e68 6173 5f70 726f 7465 6374 6564 5f63  .has_protected_c
+00029790: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
+000297a0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+000297b0: 795f 746f 5f6d 6573 7361 6765 5f69 643d  y_to_message_id=
+000297c0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+000297d0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000297e0: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+000297f0: 6172 6b75 703d 7365 6c66 2e72 6570 6c79  arkup=self.reply
+00029800: 5f6d 6172 6b75 7020 6966 2072 6570 6c79  _markup if reply
+00029810: 5f6d 6172 6b75 7020 6973 206f 626a 6563  _markup is objec
+00029820: 7420 656c 7365 2072 6570 6c79 5f6d 6172  t else reply_mar
+00029830: 6b75 700a 2020 2020 2020 2020 2020 2020  kup.            
+00029840: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00029850: 2020 656c 6966 2073 656c 662e 6c6f 6361    elif self.loca
+00029860: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00029870: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00029880: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+00029890: 7365 6e64 5f6c 6f63 6174 696f 6e28 0a20  send_location(. 
 000298a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298b0: 2020 206c 6174 6974 7564 653d 7365 6c66     latitude=self
-000298c0: 2e76 656e 7565 2e6c 6f63 6174 696f 6e2e  .venue.location.
-000298d0: 6c61 7469 7475 6465 2c0a 2020 2020 2020  latitude,.      
-000298e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000298f0: 6e67 6974 7564 653d 7365 6c66 2e76 656e  ngitude=self.ven
-00029900: 7565 2e6c 6f63 6174 696f 6e2e 6c6f 6e67  ue.location.long
-00029910: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
-00029920: 2020 2020 2020 2020 2020 2074 6974 6c65             title
-00029930: 3d73 656c 662e 7665 6e75 652e 7469 746c  =self.venue.titl
-00029940: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00029950: 2020 2020 2020 2061 6464 7265 7373 3d73         address=s
-00029960: 656c 662e 7665 6e75 652e 6164 6472 6573  elf.venue.addres
-00029970: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00029980: 2020 2020 2020 2066 6f75 7273 7175 6172         foursquar
-00029990: 655f 6964 3d73 656c 662e 7665 6e75 652e  e_id=self.venue.
-000299a0: 666f 7572 7371 7561 7265 5f69 642c 0a20  foursquare_id,. 
-000299b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299c0: 2020 2066 6f75 7273 7175 6172 655f 7479     foursquare_ty
-000299d0: 7065 3d73 656c 662e 7665 6e75 652e 666f  pe=self.venue.fo
-000299e0: 7572 7371 7561 7265 5f74 7970 652c 0a20  ursquare_type,. 
-000299f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a00: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00029a10: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
-00029a20: 6e6f 7469 6669 6361 7469 6f6e 2c0a 2020  notification,.  
-00029a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a40: 2020 7265 706c 795f 7061 7261 6d65 7465    reply_paramete
-00029a50: 7273 3d72 6570 6c79 5f70 6172 616d 6574  rs=reply_paramet
-00029a60: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
-00029a70: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00029a80: 5f74 6872 6561 645f 6964 3d73 656c 662e  _thread_id=self.
-00029a90: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
-00029aa0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00029ab0: 2020 2020 2020 2062 7573 696e 6573 735f         business_
-00029ac0: 636f 6e6e 6563 7469 6f6e 5f69 643d 7365  connection_id=se
-00029ad0: 6c66 2e62 7573 696e 6573 735f 636f 6e6e  lf.business_conn
-00029ae0: 6563 7469 6f6e 5f69 642c 0a20 2020 2020  ection_id,.     
-00029af0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00029b00: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
-00029b10: 6564 756c 655f 6461 7465 2c0a 2020 2020  edule_date,.    
-00029b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b30: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
-00029b40: 7365 6c66 2e68 6173 5f70 726f 7465 6374  self.has_protect
-00029b50: 6564 5f63 6f6e 7465 6e74 2c0a 2020 2020  ed_content,.    
-00029b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b70: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00029b80: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
-00029b90: 7361 6765 5f69 642c 0a20 2020 2020 2020  sage_id,.       
-00029ba0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00029bb0: 6c79 5f6d 6172 6b75 703d 7365 6c66 2e72  ly_markup=self.r
-00029bc0: 6570 6c79 5f6d 6172 6b75 7020 6966 2072  eply_markup if r
-00029bd0: 6570 6c79 5f6d 6172 6b75 7020 6973 206f  eply_markup is o
-00029be0: 626a 6563 7420 656c 7365 2072 6570 6c79  bject else reply
-00029bf0: 5f6d 6172 6b75 700a 2020 2020 2020 2020  _markup.        
-00029c00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00029c10: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00029c20: 706f 6c6c 3a0a 2020 2020 2020 2020 2020  poll:.          
-00029c30: 2020 2020 2020 6f6c 6470 6d20 3d20 7365        oldpm = se
-00029c40: 6c66 2e5f 636c 6965 6e74 2e70 6172 7365  lf._client.parse
-00029c50: 5f6d 6f64 650a 2020 2020 2020 2020 2020  _mode.          
-00029c60: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
-00029c70: 6e74 2e73 6574 5f70 6172 7365 5f6d 6f64  nt.set_parse_mod
-00029c80: 6528 656e 756d 732e 5061 7273 654d 6f64  e(enums.ParseMod
-00029c90: 652e 4854 4d4c 290a 2020 2020 2020 2020  e.HTML).        
-00029ca0: 2020 2020 2020 2020 636d 203d 2061 7761          cm = awa
-00029cb0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00029cc0: 7365 6e64 5f70 6f6c 6c28 0a20 2020 2020  send_poll(.     
-00029cd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00029ce0: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
-00029cf0: 2020 2020 2020 2020 2020 2020 7175 6573              ques
-00029d00: 7469 6f6e 3d73 656c 662e 706f 6c6c 2e71  tion=self.poll.q
-00029d10: 7565 7374 696f 6e2e 6874 6d6c 2c0a 2020  uestion.html,.  
-00029d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029d30: 2020 6f70 7469 6f6e 733d 5b6f 7074 2e74    options=[opt.t
-00029d40: 6578 742e 6874 6d6c 2066 6f72 206f 7074  ext.html for opt
-00029d50: 2069 6e20 7365 6c66 2e70 6f6c 6c2e 6f70   in self.poll.op
-00029d60: 7469 6f6e 735d 2c0a 2020 2020 2020 2020  tions],.        
-00029d70: 2020 2020 2020 2020 2020 2020 6973 5f61              is_a
-00029d80: 6e6f 6e79 6d6f 7573 3d73 656c 662e 706f  nonymous=self.po
-00029d90: 6c6c 2e69 735f 616e 6f6e 796d 6f75 732c  ll.is_anonymous,
-00029da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029db0: 2020 2020 2074 7970 653d 7365 6c66 2e70       type=self.p
-00029dc0: 6f6c 6c2e 7479 7065 2c0a 2020 2020 2020  oll.type,.      
-00029dd0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00029de0: 6c6f 7773 5f6d 756c 7469 706c 655f 616e  lows_multiple_an
-00029df0: 7377 6572 733d 7365 6c66 2e70 6f6c 6c2e  swers=self.poll.
-00029e00: 616c 6c6f 7773 5f6d 756c 7469 706c 655f  allows_multiple_
-00029e10: 616e 7377 6572 732c 0a20 2020 2020 2020  answers,.       
-00029e20: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
-00029e30: 7265 6374 5f6f 7074 696f 6e5f 6964 3d73  rect_option_id=s
-00029e40: 656c 662e 706f 6c6c 2e63 6f72 7265 6374  elf.poll.correct
-00029e50: 5f6f 7074 696f 6e5f 6964 2c0a 2020 2020  _option_id,.    
-00029e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029e70: 6578 706c 616e 6174 696f 6e3d 7365 6c66  explanation=self
-00029e80: 2e70 6f6c 6c2e 6578 706c 616e 6174 696f  .poll.explanatio
-00029e90: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00029ea0: 2020 2020 2020 2065 7870 6c61 6e61 7469         explanati
-00029eb0: 6f6e 5f65 6e74 6974 6965 733d 7365 6c66  on_entities=self
-00029ec0: 2e70 6f6c 6c2e 6578 706c 616e 6174 696f  .poll.explanatio
-00029ed0: 6e5f 656e 7469 7469 6573 2c0a 2020 2020  n_entities,.    
-00029ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ef0: 6f70 656e 5f70 6572 696f 643d 7365 6c66  open_period=self
-00029f00: 2e70 6f6c 6c2e 6f70 656e 5f70 6572 696f  .poll.open_perio
-00029f10: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00029f20: 2020 2020 2020 2063 6c6f 7365 5f64 6174         close_dat
-00029f30: 653d 7365 6c66 2e70 6f6c 6c2e 636c 6f73  e=self.poll.clos
-00029f40: 655f 6461 7465 2c0a 2020 2020 2020 2020  e_date,.        
-00029f50: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00029f60: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00029f70: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00029f80: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-00029f90: 2020 2020 2020 2020 2020 2070 726f 7465             prote
-00029fa0: 6374 5f63 6f6e 7465 6e74 3d73 656c 662e  ct_content=self.
-00029fb0: 6861 735f 7072 6f74 6563 7465 645f 636f  has_protected_co
-00029fc0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
-00029fd0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00029fe0: 5f70 6172 616d 6574 6572 733d 7265 706c  _parameters=repl
-00029ff0: 795f 7061 7261 6d65 7465 7273 2c0a 2020  y_parameters,.  
-0002a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a010: 2020 6d65 7373 6167 655f 7468 7265 6164    message_thread
-0002a020: 5f69 643d 7365 6c66 2e6d 6573 7361 6765  _id=self.message
-0002a030: 5f74 6872 6561 645f 6964 2c0a 2020 2020  _thread_id,.    
-0002a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a050: 6275 7369 6e65 7373 5f63 6f6e 6e65 6374  business_connect
-0002a060: 696f 6e5f 6964 3d73 656c 662e 6275 7369  ion_id=self.busi
-0002a070: 6e65 7373 5f63 6f6e 6e65 6374 696f 6e5f  ness_connection_
-0002a080: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002a090: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
-0002a0a0: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
-0002a0b0: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
-0002a0c0: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
-0002a0d0: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
-0002a0e0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-0002a0f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002a100: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-0002a110: 7570 3d73 656c 662e 7265 706c 795f 6d61  up=self.reply_ma
-0002a120: 726b 7570 2069 6620 7265 706c 795f 6d61  rkup if reply_ma
-0002a130: 726b 7570 2069 7320 6f62 6a65 6374 2065  rkup is object e
-0002a140: 6c73 6520 7265 706c 795f 6d61 726b 7570  lse reply_markup
-0002a150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a160: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0002a170: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
-0002a180: 7365 745f 7061 7273 655f 6d6f 6465 286f  set_parse_mode(o
-0002a190: 6c64 706d 290a 2020 2020 2020 2020 2020  ldpm).          
-0002a1a0: 2020 2020 2020 7265 7475 726e 2063 6d0a        return cm.
-0002a1b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0002a1c0: 2073 656c 662e 6761 6d65 3a0a 2020 2020   self.game:.    
-0002a1d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0002a1e0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-0002a1f0: 6c69 656e 742e 7365 6e64 5f67 616d 6528  lient.send_game(
-0002a200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a210: 2020 2020 2063 6861 745f 6964 2c0a 2020       chat_id,.  
-0002a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a230: 2020 6761 6d65 5f73 686f 7274 5f6e 616d    game_short_nam
-0002a240: 653d 7365 6c66 2e67 616d 652e 7368 6f72  e=self.game.shor
-0002a250: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
-0002a260: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-0002a270: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-0002a280: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-0002a290: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-0002a2a0: 2020 2020 2020 2020 2020 2070 726f 7465             prote
-0002a2b0: 6374 5f63 6f6e 7465 6e74 3d73 656c 662e  ct_content=self.
-0002a2c0: 6861 735f 7072 6f74 6563 7465 645f 636f  has_protected_co
-0002a2d0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
-0002a2e0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0002a2f0: 6765 5f74 6872 6561 645f 6964 3d73 656c  ge_thread_id=sel
-0002a300: 662e 6d65 7373 6167 655f 7468 7265 6164  f.message_thread
-0002a310: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0002a320: 2020 2020 2020 2020 2062 7573 696e 6573           busines
-0002a330: 735f 636f 6e6e 6563 7469 6f6e 5f69 643d  s_connection_id=
-0002a340: 7365 6c66 2e62 7573 696e 6573 735f 636f  self.business_co
-0002a350: 6e6e 6563 7469 6f6e 5f69 642c 0a20 2020  nnection_id,.   
-0002a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a370: 2072 6570 6c79 5f70 6172 616d 6574 6572   reply_parameter
-0002a380: 733d 7265 706c 795f 7061 7261 6d65 7465  s=reply_paramete
-0002a390: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-0002a3a0: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-0002a3b0: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
-0002a3c0: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
-0002a3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a3e0: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
-0002a3f0: 703d 7365 6c66 2e72 6570 6c79 5f6d 6172  p=self.reply_mar
-0002a400: 6b75 7020 6966 2072 6570 6c79 5f6d 6172  kup if reply_mar
-0002a410: 6b75 7020 6973 206f 626a 6563 7420 656c  kup is object el
-0002a420: 7365 2072 6570 6c79 5f6d 6172 6b75 700a  se reply_markup.
+000298b0: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
+000298c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298d0: 6c61 7469 7475 6465 3d73 656c 662e 6c6f  latitude=self.lo
+000298e0: 6361 7469 6f6e 2e6c 6174 6974 7564 652c  cation.latitude,
+000298f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029900: 2020 2020 206c 6f6e 6769 7475 6465 3d73       longitude=s
+00029910: 656c 662e 6c6f 6361 7469 6f6e 2e6c 6f6e  elf.location.lon
+00029920: 6769 7475 6465 2c0a 2020 2020 2020 2020  gitude,.        
+00029930: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00029940: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00029950: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
+00029960: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+00029970: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00029980: 5f70 6172 616d 6574 6572 733d 7265 706c  _parameters=repl
+00029990: 795f 7061 7261 6d65 7465 7273 2c0a 2020  y_parameters,.  
+000299a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000299b0: 2020 6d65 7373 6167 655f 7468 7265 6164    message_thread
+000299c0: 5f69 643d 6d65 7373 6167 655f 7468 7265  _id=message_thre
+000299d0: 6164 5f69 6420 6f72 2073 656c 662e 6d65  ad_id or self.me
+000299e0: 7373 6167 655f 7468 7265 6164 5f69 642c  ssage_thread_id,
+000299f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029a00: 2020 2020 2062 7573 696e 6573 735f 636f       business_co
+00029a10: 6e6e 6563 7469 6f6e 5f69 643d 6275 7369  nnection_id=busi
+00029a20: 6e65 7373 5f63 6f6e 6e65 6374 696f 6e5f  ness_connection_
+00029a30: 6964 206f 7220 7365 6c66 2e62 7573 696e  id or self.busin
+00029a40: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
+00029a50: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00029a60: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
+00029a70: 6461 7465 3d73 6368 6564 756c 655f 6461  date=schedule_da
+00029a80: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
+00029a90: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
+00029aa0: 636f 6e74 656e 743d 7072 6f74 6563 745f  content=protect_
+00029ab0: 636f 6e74 656e 7420 6f72 2073 656c 662e  content or self.
+00029ac0: 6861 735f 7072 6f74 6563 7465 645f 636f  has_protected_co
+00029ad0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
+00029ae0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00029af0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d72  _to_message_id=r
+00029b00: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00029b10: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00029b20: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
+00029b30: 726b 7570 3d73 656c 662e 7265 706c 795f  rkup=self.reply_
+00029b40: 6d61 726b 7570 2069 6620 7265 706c 795f  markup if reply_
+00029b50: 6d61 726b 7570 2069 7320 6f62 6a65 6374  markup is object
+00029b60: 2065 6c73 6520 7265 706c 795f 6d61 726b   else reply_mark
+00029b70: 7570 0a20 2020 2020 2020 2020 2020 2020  up.             
+00029b80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00029b90: 2065 6c69 6620 7365 6c66 2e76 656e 7565   elif self.venue
+00029ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00029bb0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+00029bc0: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
+00029bd0: 5f76 656e 7565 280a 2020 2020 2020 2020  _venue(.        
+00029be0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+00029bf0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00029c00: 2020 2020 2020 2020 206c 6174 6974 7564           latitud
+00029c10: 653d 7365 6c66 2e76 656e 7565 2e6c 6f63  e=self.venue.loc
+00029c20: 6174 696f 6e2e 6c61 7469 7475 6465 2c0a  ation.latitude,.
+00029c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c40: 2020 2020 6c6f 6e67 6974 7564 653d 7365      longitude=se
+00029c50: 6c66 2e76 656e 7565 2e6c 6f63 6174 696f  lf.venue.locatio
+00029c60: 6e2e 6c6f 6e67 6974 7564 652c 0a20 2020  n.longitude,.   
+00029c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c80: 2074 6974 6c65 3d73 656c 662e 7665 6e75   title=self.venu
+00029c90: 652e 7469 746c 652c 0a20 2020 2020 2020  e.title,.       
+00029ca0: 2020 2020 2020 2020 2020 2020 2061 6464               add
+00029cb0: 7265 7373 3d73 656c 662e 7665 6e75 652e  ress=self.venue.
+00029cc0: 6164 6472 6573 732c 0a20 2020 2020 2020  address,.       
+00029cd0: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
+00029ce0: 7273 7175 6172 655f 6964 3d73 656c 662e  rsquare_id=self.
+00029cf0: 7665 6e75 652e 666f 7572 7371 7561 7265  venue.foursquare
+00029d00: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00029d10: 2020 2020 2020 2020 2066 6f75 7273 7175           foursqu
+00029d20: 6172 655f 7479 7065 3d73 656c 662e 7665  are_type=self.ve
+00029d30: 6e75 652e 666f 7572 7371 7561 7265 5f74  nue.foursquare_t
+00029d40: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00029d50: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
+00029d60: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
+00029d70: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00029d80: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00029d90: 2020 2020 2020 2020 7265 706c 795f 7061          reply_pa
+00029da0: 7261 6d65 7465 7273 3d72 6570 6c79 5f70  rameters=reply_p
+00029db0: 6172 616d 6574 6572 732c 0a20 2020 2020  arameters,.     
+00029dc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00029dd0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00029de0: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
+00029df0: 6964 206f 7220 7365 6c66 2e6d 6573 7361  id or self.messa
+00029e00: 6765 5f74 6872 6561 645f 6964 2c0a 2020  ge_thread_id,.  
+00029e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e20: 2020 6275 7369 6e65 7373 5f63 6f6e 6e65    business_conne
+00029e30: 6374 696f 6e5f 6964 3d62 7573 696e 6573  ction_id=busines
+00029e40: 735f 636f 6e6e 6563 7469 6f6e 5f69 6420  s_connection_id 
+00029e50: 6f72 2073 656c 662e 6275 7369 6e65 7373  or self.business
+00029e60: 5f63 6f6e 6e65 6374 696f 6e5f 6964 2c0a  _connection_id,.
+00029e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029e80: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
+00029e90: 653d 7363 6865 6475 6c65 5f64 6174 652c  e=schedule_date,
+00029ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029eb0: 2020 2020 2070 726f 7465 6374 5f63 6f6e       protect_con
+00029ec0: 7465 6e74 3d70 726f 7465 6374 5f63 6f6e  tent=protect_con
+00029ed0: 7465 6e74 206f 7220 7365 6c66 2e68 6173  tent or self.has
+00029ee0: 5f70 726f 7465 6374 6564 5f63 6f6e 7465  _protected_conte
+00029ef0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00029f00: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+00029f10: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
+00029f20: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
+00029f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029f40: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
+00029f50: 703d 7365 6c66 2e72 6570 6c79 5f6d 6172  p=self.reply_mar
+00029f60: 6b75 7020 6966 2072 6570 6c79 5f6d 6172  kup if reply_mar
+00029f70: 6b75 7020 6973 206f 626a 6563 7420 656c  kup is object el
+00029f80: 7365 2072 6570 6c79 5f6d 6172 6b75 700a  se reply_markup.
+00029f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fa0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00029fb0: 6966 2073 656c 662e 706f 6c6c 3a0a 2020  if self.poll:.  
+00029fc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00029fd0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00029fe0: 5f63 6c69 656e 742e 7365 6e64 5f70 6f6c  _client.send_pol
+00029ff0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+0002a000: 2020 2020 2020 2063 6861 745f 6964 2c0a         chat_id,.
+0002a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a020: 2020 2020 7175 6573 7469 6f6e 3d73 656c      question=sel
+0002a030: 662e 706f 6c6c 2e71 7565 7374 696f 6e2c  f.poll.question,
+0002a040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a050: 2020 2020 2071 7565 7374 696f 6e5f 656e       question_en
+0002a060: 7469 7469 6573 3d73 656c 662e 706f 6c6c  tities=self.poll
+0002a070: 2e71 7565 7374 696f 6e5f 656e 7469 7469  .question_entiti
+0002a080: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0002a090: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
+0002a0a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0002a0b0: 2020 2020 2020 2020 2020 7479 7065 732e            types.
+0002a0c0: 496e 7075 7450 6f6c 6c4f 7074 696f 6e28  InputPollOption(
+0002a0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a0e0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0002a0f0: 743d 6f70 742e 7465 7874 2c0a 2020 2020  t=opt.text,.    
+0002a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a110: 2020 2020 2020 2020 7465 7874 5f65 6e74          text_ent
+0002a120: 6974 6965 733d 6f70 742e 7465 7874 5f65  ities=opt.text_e
+0002a130: 6e74 6974 6965 730a 2020 2020 2020 2020  ntities.        
+0002a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a150: 2920 666f 7220 6f70 7420 696e 2073 656c  ) for opt in sel
+0002a160: 662e 706f 6c6c 2e6f 7074 696f 6e73 0a20  f.poll.options. 
+0002a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a180: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+0002a190: 2020 2020 2020 2020 2020 6973 5f61 6e6f            is_ano
+0002a1a0: 6e79 6d6f 7573 3d73 656c 662e 706f 6c6c  nymous=self.poll
+0002a1b0: 2e69 735f 616e 6f6e 796d 6f75 732c 0a20  .is_anonymous,. 
+0002a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a1d0: 2020 2074 7970 653d 7365 6c66 2e70 6f6c     type=self.pol
+0002a1e0: 6c2e 7479 7065 2c0a 2020 2020 2020 2020  l.type,.        
+0002a1f0: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
+0002a200: 7773 5f6d 756c 7469 706c 655f 616e 7377  ws_multiple_answ
+0002a210: 6572 733d 7365 6c66 2e70 6f6c 6c2e 616c  ers=self.poll.al
+0002a220: 6c6f 7773 5f6d 756c 7469 706c 655f 616e  lows_multiple_an
+0002a230: 7377 6572 732c 0a20 2020 2020 2020 2020  swers,.         
+0002a240: 2020 2020 2020 2020 2020 2063 6f72 7265             corre
+0002a250: 6374 5f6f 7074 696f 6e5f 6964 3d73 656c  ct_option_id=sel
+0002a260: 662e 706f 6c6c 2e63 6f72 7265 6374 5f6f  f.poll.correct_o
+0002a270: 7074 696f 6e5f 6964 2c0a 2020 2020 2020  ption_id,.      
+0002a280: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0002a290: 706c 616e 6174 696f 6e3d 7365 6c66 2e70  planation=self.p
+0002a2a0: 6f6c 6c2e 6578 706c 616e 6174 696f 6e2c  oll.explanation,
+0002a2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a2c0: 2020 2020 2065 7870 6c61 6e61 7469 6f6e       explanation
+0002a2d0: 5f65 6e74 6974 6965 733d 7365 6c66 2e70  _entities=self.p
+0002a2e0: 6f6c 6c2e 6578 706c 616e 6174 696f 6e5f  oll.explanation_
+0002a2f0: 656e 7469 7469 6573 2c0a 2020 2020 2020  entities,.      
+0002a300: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+0002a310: 656e 5f70 6572 696f 643d 7365 6c66 2e70  en_period=self.p
+0002a320: 6f6c 6c2e 6f70 656e 5f70 6572 696f 642c  oll.open_period,
+0002a330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a340: 2020 2020 2063 6c6f 7365 5f64 6174 653d       close_date=
+0002a350: 7365 6c66 2e70 6f6c 6c2e 636c 6f73 655f  self.poll.close_
+0002a360: 6461 7465 2c0a 2020 2020 2020 2020 2020  date,.          
+0002a370: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+0002a380: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
+0002a390: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+0002a3a0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0002a3b0: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+0002a3c0: 5f63 6f6e 7465 6e74 3d70 726f 7465 6374  _content=protect
+0002a3d0: 5f63 6f6e 7465 6e74 206f 7220 7365 6c66  _content or self
+0002a3e0: 2e68 6173 5f70 726f 7465 6374 6564 5f63  .has_protected_c
+0002a3f0: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
+0002a400: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+0002a410: 795f 7061 7261 6d65 7465 7273 3d72 6570  y_parameters=rep
+0002a420: 6c79 5f70 6172 616d 6574 6572 732c 0a20  ly_parameters,. 
 0002a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a440: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0002a450: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0002a460: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0002a470: 7272 6f72 2822 556e 6b6e 6f77 6e20 6d65  rror("Unknown me
-0002a480: 6469 6120 7479 7065 2229 0a0a 2020 2020  dia type")..    
-0002a490: 2020 2020 2020 2020 6966 2063 6170 7469          if capti
-0002a4a0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-0002a4b0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-0002a4c0: 696f 6e20 3d20 7365 6c66 2e63 6170 7469  ion = self.capti
-0002a4d0: 6f6e 206f 7220 2222 0a20 2020 2020 2020  on or "".       
-0002a4e0: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
-0002a4f0: 5f65 6e74 6974 6965 7320 3d20 7365 6c66  _entities = self
-0002a500: 2e63 6170 7469 6f6e 5f65 6e74 6974 6965  .caption_entitie
-0002a510: 730a 0a20 2020 2020 2020 2020 2020 2072  s..            r
-0002a520: 6574 7572 6e20 6177 6169 7420 7365 6e64  eturn await send
-0002a530: 5f6d 6564 6961 280a 2020 2020 2020 2020  _media(.        
-0002a540: 2020 2020 2020 2020 6669 6c65 5f69 643d          file_id=
-0002a550: 6669 6c65 5f69 642c 0a20 2020 2020 2020  file_id,.       
-0002a560: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
-0002a570: 3d63 6170 7469 6f6e 2c0a 2020 2020 2020  =caption,.      
-0002a580: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
-0002a590: 6d6f 6465 3d70 6172 7365 5f6d 6f64 652c  mode=parse_mode,
-0002a5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a5b0: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
-0002a5c0: 733d 6361 7074 696f 6e5f 656e 7469 7469  s=caption_entiti
-0002a5d0: 6573 0a20 2020 2020 2020 2020 2020 2029  es.            )
-0002a5e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0002a5f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0002a600: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
-0002a610: 2774 2063 6f70 7920 7468 6973 206d 6573  't copy this mes
-0002a620: 7361 6765 2229 0a0a 2020 2020 6173 796e  sage")..    asyn
-0002a630: 6320 6465 6620 6465 6c65 7465 2873 656c  c def delete(sel
-0002a640: 662c 2072 6576 6f6b 653a 2062 6f6f 6c20  f, revoke: bool 
-0002a650: 3d20 5472 7565 293a 0a20 2020 2020 2020  = True):.       
-0002a660: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
-0002a670: 202a 6465 6c65 7465 2a20 6f66 203a 6f62   *delete* of :ob
-0002a680: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
-0002a690: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
-0002a6a0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
-0002a6b0: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
-0002a6c0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-0002a6d0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-0002a6e0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0002a6f0: 636c 6965 6e74 2e64 656c 6574 655f 6d65  client.delete_me
-0002a700: 7373 6167 6573 280a 2020 2020 2020 2020  ssages(.        
-0002a710: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0002a720: 6368 6174 5f69 642c 0a20 2020 2020 2020  chat_id,.       
-0002a730: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0002a740: 5f69 6473 3d6d 6573 7361 6765 2e69 640a  _ids=message.id.
-0002a750: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0002a760: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-0002a770: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0002a780: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0002a790: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0002a7a0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-0002a7b0: 652e 6465 6c65 7465 2829 0a0a 2020 2020  e.delete()..    
-0002a7c0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-0002a7d0: 2020 2020 2020 2020 2020 2020 7265 766f              revo
-0002a7e0: 6b65 2028 6060 626f 6f6c 6060 2c20 2a6f  ke (``bool``, *o
-0002a7f0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0002a800: 2020 2020 2020 2020 2020 2044 656c 6574             Delet
-0002a810: 6573 206d 6573 7361 6765 7320 6f6e 2062  es messages on b
-0002a820: 6f74 6820 7061 7274 732e 0a20 2020 2020  oth parts..     
-0002a830: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0002a840: 6973 206f 6e6c 7920 666f 7220 7072 6976  is only for priv
-0002a850: 6174 6520 636c 6f75 6420 6368 6174 7320  ate cloud chats 
-0002a860: 616e 6420 6e6f 726d 616c 2067 726f 7570  and normal group
-0002a870: 732c 206d 6573 7361 6765 7320 6f6e 0a20  s, messages on. 
-0002a880: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002a890: 6861 6e6e 656c 7320 616e 6420 7375 7065  hannels and supe
-0002a8a0: 7267 726f 7570 7320 6172 6520 616c 7761  rgroups are alwa
-0002a8b0: 7973 2072 6576 6f6b 6564 2028 692e 652e  ys revoked (i.e.
-0002a8c0: 3a20 6465 6c65 7465 6420 666f 7220 6576  : deleted for ev
-0002a8d0: 6572 796f 6e65 292e 0a20 2020 2020 2020  eryone)..       
-0002a8e0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0002a8f0: 7320 746f 2054 7275 652e 0a0a 2020 2020  s to True...    
-0002a900: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0002a910: 2020 2020 2020 2020 2060 6069 6e74 6060           ``int``
-0002a920: 3a20 416d 6f75 6e74 206f 6620 6166 6665  : Amount of affe
-0002a930: 6374 6564 206d 6573 7361 6765 730a 0a20  cted messages.. 
-0002a940: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-0002a950: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
-0002a960: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
-0002a970: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
-0002a980: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
-0002a990: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0002a9a0: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
-0002a9b0: 656e 742e 6465 6c65 7465 5f6d 6573 7361  ent.delete_messa
-0002a9c0: 6765 7328 0a20 2020 2020 2020 2020 2020  ges(.           
-0002a9d0: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
-0002a9e0: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
-0002a9f0: 2020 206d 6573 7361 6765 5f69 6473 3d73     message_ids=s
-0002aa00: 656c 662e 6964 2c0a 2020 2020 2020 2020  elf.id,.        
-0002aa10: 2020 2020 7265 766f 6b65 3d72 6576 6f6b      revoke=revok
-0002aa20: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
-0002aa30: 735f 7363 6865 6475 6c65 643d 7365 6c66  s_scheduled=self
-0002aa40: 2e73 6368 6564 756c 6564 0a20 2020 2020  .scheduled.     
-0002aa50: 2020 2029 0a0a 2020 2020 6173 796e 6320     )..    async 
-0002aa60: 6465 6620 636c 6963 6b28 0a20 2020 2020  def click(.     
-0002aa70: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0002aa80: 2078 3a20 556e 696f 6e5b 696e 742c 2073   x: Union[int, s
-0002aa90: 7472 5d20 3d20 302c 0a20 2020 2020 2020  tr] = 0,.       
-0002aaa0: 2079 3a20 696e 7420 3d20 4e6f 6e65 2c0a   y: int = None,.
-0002aab0: 2020 2020 2020 2020 7175 6f74 653a 2062          quote: b
-0002aac0: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-0002aad0: 2020 2020 7469 6d65 6f75 743a 2069 6e74      timeout: int
-0002aae0: 203d 2031 302c 0a20 2020 2020 2020 2072   = 10,.        r
-0002aaf0: 6571 7565 7374 5f77 7269 7465 5f61 6363  equest_write_acc
-0002ab00: 6573 733a 2062 6f6f 6c20 3d20 5472 7565  ess: bool = True
-0002ab10: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
-0002ab20: 7264 3a20 7374 7220 3d20 4e6f 6e65 0a20  rd: str = None. 
-0002ab30: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0002ab40: 2242 6f75 6e64 206d 6574 686f 6420 2a63  "Bound method *c
-0002ab50: 6c69 636b 2a20 6f66 203a 6f62 6a3a 607e  lick* of :obj:`~
-0002ab60: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
-0002ab70: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
-0002ab80: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-0002ab90: 6375 7420 666f 7220 636c 6963 6b69 6e67  cut for clicking
-0002aba0: 2061 2062 7574 746f 6e20 6174 7461 6368   a button attach
-0002abb0: 6564 2074 6f20 7468 6520 6d65 7373 6167  ed to the messag
-0002abc0: 6520 696e 7374 6561 6420 6f66 3a0a 0a20  e instead of:.. 
-0002abd0: 2020 2020 2020 202d 2043 6c69 636b 696e         - Clickin
-0002abe0: 6720 696e 6c69 6e65 2062 7574 746f 6e73  g inline buttons
-0002abf0: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
-0002ac00: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-0002ac10: 6e0a 0a20 2020 2020 2020 2020 2020 2061  n..            a
-0002ac20: 7761 6974 2063 6c69 656e 742e 7265 7175  wait client.requ
-0002ac30: 6573 745f 6361 6c6c 6261 636b 5f61 6e73  est_callback_ans
-0002ac40: 7765 7228 0a20 2020 2020 2020 2020 2020  wer(.           
-0002ac50: 2020 2020 2063 6861 745f 6964 3d6d 6573       chat_id=mes
-0002ac60: 7361 6765 2e63 6861 742e 6964 2c0a 2020  sage.chat.id,.  
-0002ac70: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0002ac80: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
-0002ac90: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
-0002aca0: 2020 2020 2063 616c 6c62 6163 6b5f 6461       callback_da
-0002acb0: 7461 3d6d 6573 7361 6765 2e72 6570 6c79  ta=message.reply
-0002acc0: 5f6d 6172 6b75 705b 695d 5b6a 5d2e 6361  _markup[i][j].ca
-0002acd0: 6c6c 6261 636b 5f64 6174 610a 2020 2020  llback_data.    
-0002ace0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0002acf0: 2020 202d 2043 6c69 636b 696e 6720 6e6f     - Clicking no
-0002ad00: 726d 616c 2062 7574 746f 6e73 3a0a 0a20  rmal buttons:.. 
-0002ad10: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-0002ad20: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
-0002ad30: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0002ad40: 2063 6c69 656e 742e 7365 6e64 5f6d 6573   client.send_mes
-0002ad50: 7361 6765 280a 2020 2020 2020 2020 2020  sage(.          
-0002ad60: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
-0002ad70: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
-0002ad80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002ad90: 6578 743d 6d65 7373 6167 652e 7265 706c  ext=message.repl
-0002ada0: 795f 6d61 726b 7570 5b69 5d5b 6a5d 2e74  y_markup[i][j].t
-0002adb0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-0002adc0: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
-0002add0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-0002ade0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-0002adf0: 6265 2075 7365 6420 696e 2074 6872 6565  be used in three
-0002ae00: 2064 6966 6665 7265 6e74 2077 6179 733a   different ways:
-0002ae10: 0a0a 2020 2020 2020 2020 2020 2020 312e  ..            1.
-0002ae20: 2020 5061 7373 206f 6e65 2069 6e74 6567    Pass one integ
-0002ae30: 6572 2061 7267 756d 656e 7420 6f6e 6c79  er argument only
-0002ae40: 2028 652e 672e 3a20 6060 2e63 6c69 636b   (e.g.: ``.click
-0002ae50: 2832 2960 602c 2074 6f20 636c 6963 6b20  (2)``, to click 
-0002ae60: 6120 6275 7474 6f6e 2061 7420 696e 6465  a button at inde
-0002ae70: 7820 3229 2e0a 2020 2020 2020 2020 2020  x 2)..          
-0002ae80: 2020 2020 2020 4275 7474 6f6e 7320 6172        Buttons ar
-0002ae90: 6520 636f 756e 7465 6420 6c65 6674 2074  e counted left t
-0002aea0: 6f20 7269 6768 742c 2073 7461 7274 696e  o right, startin
-0002aeb0: 6720 6672 6f6d 2074 6865 2074 6f70 2e0a  g from the top..
-0002aec0: 0a20 2020 2020 2020 2020 2020 2032 2e20  .            2. 
-0002aed0: 2050 6173 7320 7477 6f20 696e 7465 6765   Pass two intege
-0002aee0: 7220 6172 6775 6d65 6e74 7320 2865 2e67  r arguments (e.g
-0002aef0: 2e3a 2060 602e 636c 6963 6b28 312c 2030  .: ``.click(1, 0
-0002af00: 2960 602c 2074 6f20 636c 6963 6b20 6120  )``, to click a 
-0002af10: 6275 7474 6f6e 2061 7420 706f 7369 7469  button at positi
-0002af20: 6f6e 2028 312c 2030 2929 2e0a 2020 2020  on (1, 0))..    
-0002af30: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0002af40: 6f72 6967 696e 2028 302c 2030 2920 6973  origin (0, 0) is
-0002af50: 2074 6f70 2d6c 6566 742e 0a0a 2020 2020   top-left...    
-0002af60: 2020 2020 2020 2020 332e 2020 5061 7373          3.  Pass
-0002af70: 206f 6e65 2073 7472 696e 6720 6172 6775   one string argu
-0002af80: 6d65 6e74 206f 6e6c 7920 2865 2e67 2e3a  ment only (e.g.:
-0002af90: 2060 602e 636c 6963 6b28 2253 6574 7469   ``.click("Setti
-0002afa0: 6e67 7322 2960 602c 2074 6f20 636c 6963  ngs")``, to clic
-0002afb0: 6b20 6120 6275 7474 6f6e 2062 7920 7573  k a button by us
-0002afc0: 696e 6720 6974 7320 6c61 6265 6c29 2e0a  ing its label)..
-0002afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002afe0: 4f6e 6c79 2074 6865 2066 6972 7374 206d  Only the first m
-0002aff0: 6174 6368 696e 6720 6275 7474 6f6e 2077  atching button w
-0002b000: 696c 6c20 6265 2070 7265 7373 6564 2e0a  ill be pressed..
-0002b010: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0002b020: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-0002b030: 2078 2028 6060 696e 7460 6020 7c20 6060   x (``int`` | ``
-0002b040: 7374 7260 6029 3a0a 2020 2020 2020 2020  str``):.        
-0002b050: 2020 2020 2020 2020 5573 6564 2061 7320          Used as 
-0002b060: 696e 7465 6765 7220 696e 6465 782c 2069  integer index, i
-0002b070: 6e74 6567 6572 2061 6273 6369 7373 6120  nteger abscissa 
-0002b080: 2869 6e20 7061 6972 2077 6974 6820 7929  (in pair with y)
-0002b090: 206f 7220 6173 2073 7472 696e 6720 6c61   or as string la
-0002b0a0: 6265 6c2e 0a20 2020 2020 2020 2020 2020  bel..           
-0002b0b0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-0002b0c0: 2030 2028 6669 7273 7420 6275 7474 6f6e   0 (first button
-0002b0d0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
-0002b0e0: 7920 2860 6069 6e74 6060 2c20 2a6f 7074  y (``int``, *opt
-0002b0f0: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-0002b100: 2020 2020 2020 2020 2055 7365 6420 6173           Used as
-0002b110: 206f 7264 696e 6174 6520 6f6e 6c79 2028   ordinate only (
-0002b120: 696e 2070 6169 7220 7769 7468 2078 292e  in pair with x).
-0002b130: 0a0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
-0002b140: 6f74 6520 2860 6062 6f6f 6c60 602c 202a  ote (``bool``, *
-0002b150: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
-0002b160: 2020 2020 2020 2020 2020 2020 5573 6566              Usef
-0002b170: 756c 2066 6f72 206e 6f72 6d61 6c20 6275  ul for normal bu
-0002b180: 7474 6f6e 7320 6f6e 6c79 2c20 7768 6572  ttons only, wher
-0002b190: 6520 7072 6573 7369 6e67 2069 7420 7769  e pressing it wi
-0002b1a0: 6c6c 2072 6573 756c 7420 696e 2061 206e  ll result in a n
-0002b1b0: 6577 206d 6573 7361 6765 2073 656e 742e  ew message sent.
-0002b1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b1d0: 2049 6620 6060 5472 7565 6060 2c20 7468   If ``True``, th
-0002b1e0: 6520 6d65 7373 6167 6520 7769 6c6c 2062  e message will b
-0002b1f0: 6520 7365 6e74 2061 7320 6120 7265 706c  e sent as a repl
-0002b200: 7920 746f 2074 6869 7320 6d65 7373 6167  y to this messag
-0002b210: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002b220: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
-0002b230: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
-0002b240: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
-0002b250: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
-0002b260: 6368 6174 732e 0a0a 2020 2020 2020 2020  chats...        
-0002b270: 2020 2020 7469 6d65 6f75 7420 2860 6069      timeout (``i
-0002b280: 6e74 6060 2c20 2a6f 7074 696f 6e61 6c2a  nt``, *optional*
-0002b290: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002b2a0: 2020 2054 696d 656f 7574 2069 6e20 7365     Timeout in se
-0002b2b0: 636f 6e64 732e 0a0a 2020 2020 2020 2020  conds...        
-0002b2c0: 2020 2020 7265 7175 6573 745f 7772 6974      request_writ
-0002b2d0: 655f 6163 6365 7373 2028 6060 626f 6f6c  e_access (``bool
-0002b2e0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-0002b2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b300: 204f 6e6c 7920 7573 6564 2069 6e20 6361   Only used in ca
-0002b310: 7365 206f 6620 3a6f 626a 3a60 7e70 7972  se of :obj:`~pyr
-0002b320: 6f67 7261 6d2e 7479 7065 732e 4c6f 6769  ogram.types.Logi
-0002b330: 6e55 726c 6020 6275 7474 6f6e 2e0a 2020  nUrl` button..  
-0002b340: 2020 2020 2020 2020 2020 2020 2020 5472                Tr
-0002b350: 7565 2c20 6966 2074 6865 2062 6f74 2063  ue, if the bot c
-0002b360: 616e 2073 656e 6420 6d65 7373 6167 6573  an send messages
-0002b370: 2074 6f20 7468 6520 7573 6572 2e0a 2020   to the user..  
-0002b380: 2020 2020 2020 2020 2020 2020 2020 4465                De
-0002b390: 6661 756c 7473 2074 6f20 6060 5472 7565  faults to ``True
-0002b3a0: 6060 2e0a 0a20 2020 2020 2020 2020 2020  ``...           
-0002b3b0: 2070 6173 7377 6f72 6420 2860 6073 7472   password (``str
-0002b3c0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-0002b3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b3e0: 2057 6865 6e20 636c 6963 6b69 6e67 2063   When clicking c
-0002b3f0: 6572 7461 696e 2062 7574 746f 6e73 2028  ertain buttons (
-0002b400: 7375 6368 2061 7320 426f 7446 6174 6865  such as BotFathe
-0002b410: 7227 7320 636f 6e66 6972 6d61 7469 6f6e  r's confirmation
-0002b420: 2062 7574 746f 6e20 746f 2074 7261 6e73   button to trans
-0002b430: 6665 7220 6f77 6e65 7273 6869 7029 2c20  fer ownership), 
-0002b440: 6966 2079 6f75 7220 6163 636f 756e 7420  if your account 
-0002b450: 6861 7320 3246 4120 656e 6162 6c65 642c  has 2FA enabled,
-0002b460: 2079 6f75 206e 6565 6420 746f 2070 726f   you need to pro
-0002b470: 7669 6465 2079 6f75 7220 6163 636f 756e  vide your accoun
-0002b480: 7427 7320 7061 7373 776f 7264 2e20 0a20  t's password. . 
-0002b490: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0002b4a0: 6865 2032 2d73 7465 7020 7665 7269 6669  he 2-step verifi
-0002b4b0: 6361 7469 6f6e 2070 6173 7377 6f72 6420  cation password 
-0002b4c0: 666f 7220 7468 6520 6375 7272 656e 7420  for the current 
-0002b4d0: 7573 6572 2e20 4f6e 6c79 2061 7070 6c69  user. Only appli
-0002b4e0: 6361 626c 652c 2069 6620 7468 6520 3a6f  cable, if the :o
-0002b4f0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-0002b500: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
-0002b510: 7264 4275 7474 6f6e 6020 636f 6e74 6169  rdButton` contai
-0002b520: 6e73 2060 6063 616c 6c62 6163 6b5f 6461  ns ``callback_da
-0002b530: 7461 5f77 6974 685f 7061 7373 776f 7264  ta_with_password
-0002b540: 6060 2e0a 0a20 2020 2020 2020 2052 6574  ``...        Ret
-0002b550: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0002b560: 2020 2d20 2020 5468 6520 7265 7375 6c74    -   The result
-0002b570: 206f 6620 3a6d 6574 683a 607e 7079 726f   of :meth:`~pyro
-0002b580: 6772 616d 2e43 6c69 656e 742e 7265 7175  gram.Client.requ
-0002b590: 6573 745f 6361 6c6c 6261 636b 5f61 6e73  est_callback_ans
-0002b5a0: 7765 7260 2069 6e20 6361 7365 206f 6620  wer` in case of 
-0002b5b0: 696e 6c69 6e65 2063 616c 6c62 6163 6b20  inline callback 
-0002b5c0: 6275 7474 6f6e 2063 6c69 636b 732e 0a20  button clicks.. 
-0002b5d0: 2020 2020 2020 2020 2020 202d 2020 2054             -   T
-0002b5e0: 6865 2072 6573 756c 7420 6f66 203a 6d65  he result of :me
-0002b5f0: 7468 3a60 7e4d 6573 7361 6765 2e72 6570  th:`~Message.rep
-0002b600: 6c79 2829 6020 696e 2063 6173 6520 6f66  ly()` in case of
-0002b610: 206e 6f72 6d61 6c20 6275 7474 6f6e 2063   normal button c
-0002b620: 6c69 636b 732e 0a20 2020 2020 2020 2020  licks..         
-0002b630: 2020 202d 2020 2041 2073 7472 696e 6720     -   A string 
-0002b640: 696e 2063 6173 6520 7468 6520 696e 6c69  in case the inli
-0002b650: 6e65 2062 7574 746f 6e20 6973 2061 2055  ne button is a U
-0002b660: 524c 2c20 6120 2a73 7769 7463 685f 696e  RL, a *switch_in
-0002b670: 6c69 6e65 5f71 7565 7279 2a20 6f72 2061  line_query* or a
-0002b680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b690: 202a 7377 6974 6368 5f69 6e6c 696e 655f   *switch_inline_
-0002b6a0: 7175 6572 795f 6375 7272 656e 745f 6368  query_current_ch
-0002b6b0: 6174 2a20 6275 7474 6f6e 2e0a 2020 2020  at* button..    
-0002b6c0: 2020 2020 2020 2020 2d20 2020 4120 7374          -   A st
-0002b6d0: 7269 6e67 2055 524c 2077 6974 6820 7468  ring URL with th
-0002b6e0: 6520 7573 6572 2064 6574 6169 6c73 2c20  e user details, 
-0002b6f0: 696e 2063 6173 6520 6f66 2061 204c 6f67  in case of a Log
-0002b700: 696e 5572 6c20 6275 7474 6f6e 2e0a 2020  inUrl button..  
-0002b710: 2020 2020 2020 2020 2020 2d20 2020 4120            -   A 
-0002b720: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-0002b730: 7479 7065 732e 5377 6974 6368 496e 6c69  types.SwitchInli
-0002b740: 6e65 5175 6572 7943 686f 7365 6e43 6861  neQueryChosenCha
-0002b750: 7460 206f 626a 6563 7420 696e 2063 6173  t` object in cas
-0002b760: 6520 6f66 2061 2060 6073 7769 7463 685f  e of a ``switch_
-0002b770: 696e 6c69 6e65 5f71 7565 7279 5f63 686f  inline_query_cho
-0002b780: 7365 6e5f 6368 6174 6060 2e0a 2020 2020  sen_chat``..    
-0002b790: 2020 2020 2020 2020 2d20 2020 4120 3a6f          -   A :o
-0002b7a0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
-0002b7b0: 7065 732e 5573 6572 6020 6f62 6a65 6374  pes.User` object
-0002b7c0: 2069 6e20 6361 7365 206f 6620 6120 6060   in case of a ``
-0002b7d0: 4b65 7962 6f61 7264 4275 7474 6f6e 5573  KeyboardButtonUs
-0002b7e0: 6572 5072 6f66 696c 6560 6020 6275 7474  erProfile`` butt
-0002b7f0: 6f6e 2e0a 0a20 2020 2020 2020 2052 6169  on...        Rai
-0002b800: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-0002b810: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
-0002b820: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
-0002b830: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
-0002b840: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-0002b850: 6f72 3a20 496e 2063 6173 6520 7468 6520  or: In case the 
-0002b860: 7072 6f76 6964 6564 2069 6e64 6578 206f  provided index o
-0002b870: 7220 706f 7369 7469 6f6e 2069 7320 6f75  r position is ou
-0002b880: 7420 6f66 2072 616e 6765 206f 7220 7468  t of range or th
-0002b890: 6520 6275 7474 6f6e 206c 6162 656c 2077  e button label w
-0002b8a0: 6173 206e 6f74 2066 6f75 6e64 2e0a 2020  as not found..  
-0002b8b0: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
-0002b8c0: 7445 7272 6f72 3a20 496e 2063 6173 652c  tError: In case,
-0002b8d0: 2061 6674 6572 2063 6c69 636b 696e 6720   after clicking 
-0002b8e0: 616e 2069 6e6c 696e 6520 6275 7474 6f6e  an inline button
-0002b8f0: 2c20 7468 6520 626f 7420 6661 696c 7320  , the bot fails 
-0002b900: 746f 2061 6e73 7765 7220 7769 7468 696e  to answer within
-0002b910: 2074 6865 2074 696d 656f 7574 2e0a 2020   the timeout..  
-0002b920: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0002b930: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0002b940: 2873 656c 662e 7265 706c 795f 6d61 726b  (self.reply_mark
-0002b950: 7570 2c20 7479 7065 732e 5265 706c 794b  up, types.ReplyK
-0002b960: 6579 626f 6172 644d 6172 6b75 7029 3a0a  eyboardMarkup):.
-0002b970: 2020 2020 2020 2020 2020 2020 6b65 7962              keyb
-0002b980: 6f61 7264 203d 2073 656c 662e 7265 706c  oard = self.repl
-0002b990: 795f 6d61 726b 7570 2e6b 6579 626f 6172  y_markup.keyboar
-0002b9a0: 640a 2020 2020 2020 2020 2020 2020 6973  d.            is
-0002b9b0: 5f69 6e6c 696e 6520 3d20 4661 6c73 650a  _inline = False.
-0002b9c0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-0002b9d0: 6e73 7461 6e63 6528 7365 6c66 2e72 6570  nstance(self.rep
-0002b9e0: 6c79 5f6d 6172 6b75 702c 2074 7970 6573  ly_markup, types
-0002b9f0: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-0002ba00: 6172 6b75 7029 3a0a 2020 2020 2020 2020  arkup):.        
-0002ba10: 2020 2020 6b65 7962 6f61 7264 203d 2073      keyboard = s
-0002ba20: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-0002ba30: 2e69 6e6c 696e 655f 6b65 7962 6f61 7264  .inline_keyboard
-0002ba40: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
-0002ba50: 696e 6c69 6e65 203d 2054 7275 650a 2020  inline = True.  
-0002ba60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002ba70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0002ba80: 6c75 6545 7272 6f72 2822 5468 6520 6d65  lueError("The me
-0002ba90: 7373 6167 6520 646f 6573 6e27 7420 636f  ssage doesn't co
-0002baa0: 6e74 6169 6e20 616e 7920 6b65 7962 6f61  ntain any keyboa
-0002bab0: 7264 2229 0a0a 2020 2020 2020 2020 6966  rd")..        if
-0002bac0: 2069 7369 6e73 7461 6e63 6528 782c 2069   isinstance(x, i
-0002bad0: 6e74 2920 616e 6420 7920 6973 204e 6f6e  nt) and y is Non
-0002bae0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0002baf0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0002bb00: 2020 2020 6275 7474 6f6e 203d 205b 0a20      button = [. 
-0002bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bb20: 2020 2062 7574 746f 6e0a 2020 2020 2020     button.      
-0002bb30: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002bb40: 7220 726f 7720 696e 206b 6579 626f 6172  r row in keyboar
-0002bb50: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0002bb60: 2020 2020 2020 666f 7220 6275 7474 6f6e        for button
-0002bb70: 2069 6e20 726f 770a 2020 2020 2020 2020   in row.        
-0002bb80: 2020 2020 2020 2020 5d5b 785d 0a20 2020          ][x].   
-0002bb90: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0002bba0: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
-0002bbb0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0002bbc0: 6520 5661 6c75 6545 7272 6f72 2866 2254  e ValueError(f"T
-0002bbd0: 6865 2062 7574 746f 6e20 6174 2069 6e64  he button at ind
-0002bbe0: 6578 207b 787d 2064 6f65 736e 2774 2065  ex {x} doesn't e
-0002bbf0: 7869 7374 2229 0a20 2020 2020 2020 2065  xist").        e
-0002bc00: 6c69 6620 6973 696e 7374 616e 6365 2878  lif isinstance(x
-0002bc10: 2c20 696e 7429 2061 6e64 2069 7369 6e73  , int) and isins
-0002bc20: 7461 6e63 6528 792c 2069 6e74 293a 0a20  tance(y, int):. 
-0002bc30: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0002bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bc50: 6275 7474 6f6e 203d 206b 6579 626f 6172  button = keyboar
-0002bc60: 645b 795d 5b78 5d0a 2020 2020 2020 2020  d[y][x].        
-0002bc70: 2020 2020 6578 6365 7074 2049 6e64 6578      except Index
-0002bc80: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-0002bc90: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0002bca0: 7565 4572 726f 7228 6622 5468 6520 6275  ueError(f"The bu
-0002bcb0: 7474 6f6e 2061 7420 706f 7369 7469 6f6e  tton at position
-0002bcc0: 2028 7b78 7d2c 207b 797d 2920 646f 6573   ({x}, {y}) does
-0002bcd0: 6e27 7420 6578 6973 7422 290a 2020 2020  n't exist").    
-0002bce0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-0002bcf0: 6e63 6528 782c 2073 7472 2920 616e 6420  nce(x, str) and 
-0002bd00: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-0002bd10: 2020 2020 2020 206c 6162 656c 203d 2078         label = x
-0002bd20: 2e65 6e63 6f64 6528 2275 7466 2d31 3622  .encode("utf-16"
-0002bd30: 2c20 2273 7572 726f 6761 7465 7061 7373  , "surrogatepass
-0002bd40: 2229 2e64 6563 6f64 6528 2275 7466 2d31  ").decode("utf-1
-0002bd50: 3622 290a 0a20 2020 2020 2020 2020 2020  6")..           
-0002bd60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0002bd70: 2020 2020 2020 6275 7474 6f6e 203d 205b        button = [
-0002bd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002bd90: 2020 2020 2062 7574 746f 6e0a 2020 2020       button.    
-0002bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bdb0: 666f 7220 726f 7720 696e 206b 6579 626f  for row in keybo
-0002bdc0: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
-0002bdd0: 2020 2020 2020 2020 666f 7220 6275 7474          for butt
-0002bde0: 6f6e 2069 6e20 726f 770a 2020 2020 2020  on in row.      
-0002bdf0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002be00: 206c 6162 656c 203d 3d20 6275 7474 6f6e   label == button
-0002be10: 2e74 6578 740a 2020 2020 2020 2020 2020  .text.          
-0002be20: 2020 2020 2020 5d5b 305d 0a20 2020 2020        ][0].     
-0002be30: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-0002be40: 6465 7845 7272 6f72 3a0a 2020 2020 2020  dexError:.      
-0002be50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002be60: 5661 6c75 6545 7272 6f72 2866 2254 6865  ValueError(f"The
-0002be70: 2062 7574 746f 6e20 7769 7468 206c 6162   button with lab
-0002be80: 656c 2027 7b78 7d27 2064 6f65 736e 2774  el '{x}' doesn't
-0002be90: 2065 7869 7374 7322 290a 2020 2020 2020   exists").      
-0002bea0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002beb0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0002bec0: 7272 6f72 2822 496e 7661 6c69 6420 6172  rror("Invalid ar
-0002bed0: 6775 6d65 6e74 7322 290a 0a20 2020 2020  guments")..     
-0002bee0: 2020 2069 6620 6973 5f69 6e6c 696e 653a     if is_inline:
-0002bef0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002bf00: 6275 7474 6f6e 2e63 616c 6c62 6163 6b5f  button.callback_
-0002bf10: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-0002bf20: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0002bf30: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0002bf40: 7265 7175 6573 745f 6361 6c6c 6261 636b  request_callback
-0002bf50: 5f61 6e73 7765 7228 0a20 2020 2020 2020  _answer(.       
-0002bf60: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0002bf70: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
-0002bf80: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002bf90: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0002bfa0: 643d 7365 6c66 2e69 642c 0a20 2020 2020  d=self.id,.     
-0002bfb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002bfc0: 616c 6c62 6163 6b5f 6461 7461 3d62 7574  allback_data=but
-0002bfd0: 746f 6e2e 6361 6c6c 6261 636b 5f64 6174  ton.callback_dat
-0002bfe0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-0002bff0: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-0002c000: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-0002c010: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002c020: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
-0002c030: 2e63 616c 6c62 6163 6b5f 6461 7461 5f77  .callback_data_w
-0002c040: 6974 685f 7061 7373 776f 7264 3a0a 2020  ith_password:.  
-0002c050: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002c060: 2070 6173 7377 6f72 6420 6973 204e 6f6e   password is Non
-0002c070: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002c080: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0002c090: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-0002c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c0b0: 2022 496e 7661 6c69 6420 6172 6775 6d65   "Invalid argume
-0002c0c0: 6e74 2070 6173 7365 6422 0a20 2020 2020  nt passed".     
-0002c0d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0002c0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c0f0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0002c100: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-0002c110: 7374 5f63 616c 6c62 6163 6b5f 616e 7377  st_callback_answ
-0002c120: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-0002c130: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0002c140: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
-0002c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c160: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
-0002c170: 662e 6964 2c0a 2020 2020 2020 2020 2020  f.id,.          
-0002c180: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-0002c190: 636b 5f64 6174 613d 6275 7474 6f6e 2e63  ck_data=button.c
-0002c1a0: 616c 6c62 6163 6b5f 6461 7461 5f77 6974  allback_data_wit
-0002c1b0: 685f 7061 7373 776f 7264 2c0a 2020 2020  h_password,.    
-0002c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c1d0: 7061 7373 776f 7264 3d70 6173 7377 6f72  password=passwor
-0002c1e0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002c1f0: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-0002c200: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-0002c210: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002c220: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
-0002c230: 2e75 726c 3a0a 2020 2020 2020 2020 2020  .url:.          
-0002c240: 2020 2020 2020 7265 7475 726e 2062 7574        return but
-0002c250: 746f 6e2e 7572 6c0a 2020 2020 2020 2020  ton.url.        
-0002c260: 2020 2020 656c 6966 2062 7574 746f 6e2e      elif button.
-0002c270: 6c6f 6769 6e5f 7572 6c3a 0a20 2020 2020  login_url:.     
-0002c280: 2020 2020 2020 2020 2020 2074 6c75 203d             tlu =
-0002c290: 2062 7574 746f 6e2e 6c6f 6769 6e5f 7572   button.login_ur
-0002c2a0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-0002c2b0: 2020 7269 6565 7020 3d20 6177 6169 7420    rieep = await 
-0002c2c0: 7365 6c66 2e5f 636c 6965 6e74 2e72 6573  self._client.res
-0002c2d0: 6f6c 7665 5f70 6565 7228 0a20 2020 2020  olve_peer(.     
-0002c2e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002c2f0: 656c 662e 6368 6174 2e69 640a 2020 2020  elf.chat.id.    
-0002c300: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0002c310: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
-0002c320: 6475 6974 203d 2061 7761 6974 2073 656c  duit = await sel
-0002c330: 662e 5f63 6c69 656e 742e 696e 766f 6b65  f._client.invoke
-0002c340: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c350: 2020 2020 2020 7261 772e 6675 6e63 7469        raw.functi
-0002c360: 6f6e 732e 6d65 7373 6167 6573 2e52 6571  ons.messages.Req
-0002c370: 7565 7374 5572 6c41 7574 6828 0a20 2020  uestUrlAuth(.   
-0002c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c390: 2020 2020 2070 6565 723d 7269 6565 702c       peer=rieep,
-0002c3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c3b0: 2020 2020 2020 2020 206d 7367 5f69 643d           msg_id=
-0002c3c0: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
-0002c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c3e0: 2062 7574 746f 6e5f 6964 3d74 6c75 2e62   button_id=tlu.b
-0002c3f0: 7574 746f 6e5f 6964 2c0a 2020 2020 2020  utton_id,.      
+0002a440: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+0002a450: 645f 6964 3d6d 6573 7361 6765 5f74 6872  d_id=message_thr
+0002a460: 6561 645f 6964 206f 7220 7365 6c66 2e6d  ead_id or self.m
+0002a470: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+0002a480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002a490: 2020 2020 2020 6275 7369 6e65 7373 5f63        business_c
+0002a4a0: 6f6e 6e65 6374 696f 6e5f 6964 3d62 7573  onnection_id=bus
+0002a4b0: 696e 6573 735f 636f 6e6e 6563 7469 6f6e  iness_connection
+0002a4c0: 5f69 6420 6f72 2073 656c 662e 6275 7369  _id or self.busi
+0002a4d0: 6e65 7373 5f63 6f6e 6e65 6374 696f 6e5f  ness_connection_
+0002a4e0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002a4f0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+0002a500: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+0002a510: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+0002a520: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
+0002a530: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
+0002a540: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+0002a550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002a560: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+0002a570: 7570 3d73 656c 662e 7265 706c 795f 6d61  up=self.reply_ma
+0002a580: 726b 7570 2069 6620 7265 706c 795f 6d61  rkup if reply_ma
+0002a590: 726b 7570 2069 7320 6f62 6a65 6374 2065  rkup is object e
+0002a5a0: 6c73 6520 7265 706c 795f 6d61 726b 7570  lse reply_markup
+0002a5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a5c0: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+0002a5d0: 6c69 6620 7365 6c66 2e67 616d 653a 0a20  lif self.game:. 
+0002a5e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002a5f0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+0002a600: 2e5f 636c 6965 6e74 2e73 656e 645f 6761  ._client.send_ga
+0002a610: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0002a620: 2020 2020 2020 2020 6368 6174 5f69 642c          chat_id,
+0002a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a640: 2020 2020 2067 616d 655f 7368 6f72 745f       game_short_
+0002a650: 6e61 6d65 3d73 656c 662e 6761 6d65 2e73  name=self.game.s
+0002a660: 686f 7274 5f6e 616d 652c 0a20 2020 2020  hort_name,.     
+0002a670: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0002a680: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+0002a690: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
+0002a6a0: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
+0002a6b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0002a6c0: 6f74 6563 745f 636f 6e74 656e 743d 7072  otect_content=pr
+0002a6d0: 6f74 6563 745f 636f 6e74 656e 7420 6f72  otect_content or
+0002a6e0: 2073 656c 662e 6861 735f 7072 6f74 6563   self.has_protec
+0002a6f0: 7465 645f 636f 6e74 656e 742c 0a20 2020  ted_content,.   
+0002a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a710: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+0002a720: 6964 3d6d 6573 7361 6765 5f74 6872 6561  id=message_threa
+0002a730: 645f 6964 206f 7220 7365 6c66 2e6d 6573  d_id or self.mes
+0002a740: 7361 6765 5f74 6872 6561 645f 6964 2c0a  sage_thread_id,.
+0002a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a760: 2020 2020 6275 7369 6e65 7373 5f63 6f6e      business_con
+0002a770: 6e65 6374 696f 6e5f 6964 3d62 7573 696e  nection_id=busin
+0002a780: 6573 735f 636f 6e6e 6563 7469 6f6e 5f69  ess_connection_i
+0002a790: 6420 6f72 2073 656c 662e 6275 7369 6e65  d or self.busine
+0002a7a0: 7373 5f63 6f6e 6e65 6374 696f 6e5f 6964  ss_connection_id
+0002a7b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002a7c0: 2020 2020 2020 7265 706c 795f 7061 7261        reply_para
+0002a7d0: 6d65 7465 7273 3d72 6570 6c79 5f70 6172  meters=reply_par
+0002a7e0: 616d 6574 6572 732c 0a20 2020 2020 2020  ameters,.       
+0002a7f0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+0002a800: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+0002a810: 3d72 6570 6c79 5f74 6f5f 6d65 7373 6167  =reply_to_messag
+0002a820: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+0002a830: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+0002a840: 6d61 726b 7570 3d73 656c 662e 7265 706c  markup=self.repl
+0002a850: 795f 6d61 726b 7570 2069 6620 7265 706c  y_markup if repl
+0002a860: 795f 6d61 726b 7570 2069 7320 6f62 6a65  y_markup is obje
+0002a870: 6374 2065 6c73 6520 7265 706c 795f 6d61  ct else reply_ma
+0002a880: 726b 7570 0a20 2020 2020 2020 2020 2020  rkup.           
+0002a890: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0002a8a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002a8b0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0002a8c0: 616c 7565 4572 726f 7228 2255 6e6b 6e6f  alueError("Unkno
+0002a8d0: 776e 206d 6564 6961 2074 7970 6522 290a  wn media type").
+0002a8e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0002a8f0: 6361 7074 696f 6e20 6973 204e 6f6e 653a  caption is None:
+0002a900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a910: 2063 6170 7469 6f6e 203d 2073 656c 662e   caption = self.
+0002a920: 6361 7074 696f 6e20 6f72 2022 220a 2020  caption or "".  
+0002a930: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+0002a940: 7074 696f 6e5f 656e 7469 7469 6573 203d  ption_entities =
+0002a950: 2073 656c 662e 6361 7074 696f 6e5f 656e   self.caption_en
+0002a960: 7469 7469 6573 0a0a 2020 2020 2020 2020  tities..        
+0002a970: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0002a980: 2073 656e 645f 6d65 6469 6128 0a20 2020   send_media(.   
+0002a990: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0002a9a0: 655f 6964 3d66 696c 655f 6964 2c0a 2020  e_id=file_id,.  
+0002a9b0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+0002a9c0: 7074 696f 6e3d 6361 7074 696f 6e2c 0a20  ption=caption,. 
+0002a9d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002a9e0: 6172 7365 5f6d 6f64 653d 7061 7273 655f  arse_mode=parse_
+0002a9f0: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
+0002aa00: 2020 2020 2020 6361 7074 696f 6e5f 656e        caption_en
+0002aa10: 7469 7469 6573 3d63 6170 7469 6f6e 5f65  tities=caption_e
+0002aa20: 6e74 6974 6965 730a 2020 2020 2020 2020  ntities.        
+0002aa30: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+0002aa40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002aa50: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0002aa60: 2822 4361 6e27 7420 636f 7079 2074 6869  ("Can't copy thi
+0002aa70: 7320 6d65 7373 6167 6522 290a 0a20 2020  s message")..   
+0002aa80: 2061 7379 6e63 2064 6566 2064 656c 6574   async def delet
+0002aa90: 6528 7365 6c66 2c20 7265 766f 6b65 3a20  e(self, revoke: 
+0002aaa0: 626f 6f6c 203d 2054 7275 6529 3a0a 2020  bool = True):.  
+0002aab0: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+0002aac0: 6574 686f 6420 2a64 656c 6574 652a 206f  ethod *delete* o
+0002aad0: 6620 3a6f 626a 3a60 7e70 7972 6f67 7261  f :obj:`~pyrogra
+0002aae0: 6d2e 7479 7065 732e 4d65 7373 6167 6560  m.types.Message`
+0002aaf0: 2e0a 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
+0002ab00: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
+0002ab10: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
+0002ab20: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+0002ab30: 6e0a 0a20 2020 2020 2020 2020 2020 2061  n..            a
+0002ab40: 7761 6974 2063 6c69 656e 742e 6465 6c65  wait client.dele
+0002ab50: 7465 5f6d 6573 7361 6765 7328 0a20 2020  te_messages(.   
+0002ab60: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0002ab70: 745f 6964 3d63 6861 745f 6964 2c0a 2020  t_id=chat_id,.  
+0002ab80: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0002ab90: 7373 6167 655f 6964 733d 6d65 7373 6167  ssage_ids=messag
+0002aba0: 652e 6964 0a20 2020 2020 2020 2020 2020  e.id.           
+0002abb0: 2029 0a0a 2020 2020 2020 2020 4578 616d   )..        Exam
+0002abc0: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+0002abd0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0002abe0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0002abf0: 2020 2020 2020 2020 2061 7761 6974 206d           await m
+0002ac00: 6573 7361 6765 2e64 656c 6574 6528 290a  essage.delete().
+0002ac10: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0002ac20: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0002ac30: 2072 6576 6f6b 6520 2860 6062 6f6f 6c60   revoke (``bool`
+0002ac40: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+0002ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ac60: 4465 6c65 7465 7320 6d65 7373 6167 6573  Deletes messages
+0002ac70: 206f 6e20 626f 7468 2070 6172 7473 2e0a   on both parts..
+0002ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ac90: 5468 6973 2069 7320 6f6e 6c79 2066 6f72  This is only for
+0002aca0: 2070 7269 7661 7465 2063 6c6f 7564 2063   private cloud c
+0002acb0: 6861 7473 2061 6e64 206e 6f72 6d61 6c20  hats and normal 
+0002acc0: 6772 6f75 7073 2c20 6d65 7373 6167 6573  groups, messages
+0002acd0: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+0002ace0: 2020 2020 6368 616e 6e65 6c73 2061 6e64      channels and
+0002acf0: 2073 7570 6572 6772 6f75 7073 2061 7265   supergroups are
+0002ad00: 2061 6c77 6179 7320 7265 766f 6b65 6420   always revoked 
+0002ad10: 2869 2e65 2e3a 2064 656c 6574 6564 2066  (i.e.: deleted f
+0002ad20: 6f72 2065 7665 7279 6f6e 6529 2e0a 2020  or everyone)..  
+0002ad30: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0002ad40: 6661 756c 7473 2074 6f20 5472 7565 2e0a  faults to True..
+0002ad50: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0002ad60: 3a0a 2020 2020 2020 2020 2020 2020 6060  :.            ``
+0002ad70: 696e 7460 603a 2041 6d6f 756e 7420 6f66  int``: Amount of
+0002ad80: 2061 6666 6563 7465 6420 6d65 7373 6167   affected messag
+0002ad90: 6573 0a0a 2020 2020 2020 2020 5261 6973  es..        Rais
+0002ada0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0002adb0: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+0002adc0: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+0002add0: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+0002ade0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0002adf0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+0002ae00: 2e5f 636c 6965 6e74 2e64 656c 6574 655f  ._client.delete_
+0002ae10: 6d65 7373 6167 6573 280a 2020 2020 2020  messages(.      
+0002ae20: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+0002ae30: 6c66 2e63 6861 742e 6964 2c0a 2020 2020  lf.chat.id,.    
+0002ae40: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+0002ae50: 6964 733d 7365 6c66 2e69 642c 0a20 2020  ids=self.id,.   
+0002ae60: 2020 2020 2020 2020 2072 6576 6f6b 653d           revoke=
+0002ae70: 7265 766f 6b65 2c0a 2020 2020 2020 2020  revoke,.        
+0002ae80: 2020 2020 6973 5f73 6368 6564 756c 6564      is_scheduled
+0002ae90: 3d73 656c 662e 7363 6865 6475 6c65 640a  =self.scheduled.
+0002aea0: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
+0002aeb0: 7379 6e63 2064 6566 2063 6c69 636b 280a  sync def click(.
+0002aec0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002aed0: 2020 2020 2020 783a 2055 6e69 6f6e 5b69        x: Union[i
+0002aee0: 6e74 2c20 7374 725d 203d 2030 2c0a 2020  nt, str] = 0,.  
+0002aef0: 2020 2020 2020 793a 2069 6e74 203d 204e        y: int = N
+0002af00: 6f6e 652c 0a20 2020 2020 2020 2071 756f  one,.        quo
+0002af10: 7465 3a20 626f 6f6c 203d 204e 6f6e 652c  te: bool = None,
+0002af20: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
+0002af30: 3a20 696e 7420 3d20 3130 2c0a 2020 2020  : int = 10,.    
+0002af40: 2020 2020 7265 7175 6573 745f 7772 6974      request_writ
+0002af50: 655f 6163 6365 7373 3a20 626f 6f6c 203d  e_access: bool =
+0002af60: 2054 7275 652c 0a20 2020 2020 2020 2070   True,.        p
+0002af70: 6173 7377 6f72 643a 2073 7472 203d 204e  assword: str = N
+0002af80: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
+0002af90: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0002afa0: 6f64 202a 636c 6963 6b2a 206f 6620 3a6f  od *click* of :o
+0002afb0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+0002afc0: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
+0002afd0: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+0002afe0: 7368 6f72 7463 7574 2066 6f72 2063 6c69  shortcut for cli
+0002aff0: 636b 696e 6720 6120 6275 7474 6f6e 2061  cking a button a
+0002b000: 7474 6163 6865 6420 746f 2074 6865 206d  ttached to the m
+0002b010: 6573 7361 6765 2069 6e73 7465 6164 206f  essage instead o
+0002b020: 663a 0a0a 2020 2020 2020 2020 2d20 436c  f:..        - Cl
+0002b030: 6963 6b69 6e67 2069 6e6c 696e 6520 6275  icking inline bu
+0002b040: 7474 6f6e 733a 0a0a 2020 2020 2020 2020  ttons:..        
+0002b050: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+0002b060: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+0002b070: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+0002b080: 2e72 6571 7565 7374 5f63 616c 6c62 6163  .request_callbac
+0002b090: 6b5f 616e 7377 6572 280a 2020 2020 2020  k_answer(.      
+0002b0a0: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+0002b0b0: 643d 6d65 7373 6167 652e 6368 6174 2e69  d=message.chat.i
+0002b0c0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0002b0d0: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
+0002b0e0: 7373 6167 652e 6964 2c0a 2020 2020 2020  ssage.id,.      
+0002b0f0: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
+0002b100: 636b 5f64 6174 613d 6d65 7373 6167 652e  ck_data=message.
+0002b110: 7265 706c 795f 6d61 726b 7570 5b69 5d5b  reply_markup[i][
+0002b120: 6a5d 2e63 616c 6c62 6163 6b5f 6461 7461  j].callback_data
+0002b130: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0002b140: 2020 2020 2020 2020 2d20 436c 6963 6b69          - Clicki
+0002b150: 6e67 206e 6f72 6d61 6c20 6275 7474 6f6e  ng normal button
+0002b160: 733a 0a0a 2020 2020 2020 2020 2e2e 2063  s:..        .. c
+0002b170: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+0002b180: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+0002b190: 6177 6169 7420 636c 6965 6e74 2e73 656e  await client.sen
+0002b1a0: 645f 6d65 7373 6167 6528 0a20 2020 2020  d_message(.     
+0002b1b0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+0002b1c0: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
+0002b1d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002b1e0: 2020 2020 7465 7874 3d6d 6573 7361 6765      text=message
+0002b1f0: 2e72 6570 6c79 5f6d 6172 6b75 705b 695d  .reply_markup[i]
+0002b200: 5b6a 5d2e 7465 7874 0a20 2020 2020 2020  [j].text.       
+0002b210: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0002b220: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
+0002b230: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
+0002b240: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
+0002b250: 7468 7265 6520 6469 6666 6572 656e 7420  three different 
+0002b260: 7761 7973 3a0a 0a20 2020 2020 2020 2020  ways:..         
+0002b270: 2020 2031 2e20 2050 6173 7320 6f6e 6520     1.  Pass one 
+0002b280: 696e 7465 6765 7220 6172 6775 6d65 6e74  integer argument
+0002b290: 206f 6e6c 7920 2865 2e67 2e3a 2060 602e   only (e.g.: ``.
+0002b2a0: 636c 6963 6b28 3229 6060 2c20 746f 2063  click(2)``, to c
+0002b2b0: 6c69 636b 2061 2062 7574 746f 6e20 6174  lick a button at
+0002b2c0: 2069 6e64 6578 2032 292e 0a20 2020 2020   index 2)..     
+0002b2d0: 2020 2020 2020 2020 2020 2042 7574 746f             Butto
+0002b2e0: 6e73 2061 7265 2063 6f75 6e74 6564 206c  ns are counted l
+0002b2f0: 6566 7420 746f 2072 6967 6874 2c20 7374  eft to right, st
+0002b300: 6172 7469 6e67 2066 726f 6d20 7468 6520  arting from the 
+0002b310: 746f 702e 0a0a 2020 2020 2020 2020 2020  top...          
+0002b320: 2020 322e 2020 5061 7373 2074 776f 2069    2.  Pass two i
+0002b330: 6e74 6567 6572 2061 7267 756d 656e 7473  nteger arguments
+0002b340: 2028 652e 672e 3a20 6060 2e63 6c69 636b   (e.g.: ``.click
+0002b350: 2831 2c20 3029 6060 2c20 746f 2063 6c69  (1, 0)``, to cli
+0002b360: 636b 2061 2062 7574 746f 6e20 6174 2070  ck a button at p
+0002b370: 6f73 6974 696f 6e20 2831 2c20 3029 292e  osition (1, 0)).
+0002b380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b390: 2054 6865 206f 7269 6769 6e20 2830 2c20   The origin (0, 
+0002b3a0: 3029 2069 7320 746f 702d 6c65 6674 2e0a  0) is top-left..
+0002b3b0: 0a20 2020 2020 2020 2020 2020 2033 2e20  .            3. 
+0002b3c0: 2050 6173 7320 6f6e 6520 7374 7269 6e67   Pass one string
+0002b3d0: 2061 7267 756d 656e 7420 6f6e 6c79 2028   argument only (
+0002b3e0: 652e 672e 3a20 6060 2e63 6c69 636b 2822  e.g.: ``.click("
+0002b3f0: 5365 7474 696e 6773 2229 6060 2c20 746f  Settings")``, to
+0002b400: 2063 6c69 636b 2061 2062 7574 746f 6e20   click a button 
+0002b410: 6279 2075 7369 6e67 2069 7473 206c 6162  by using its lab
+0002b420: 656c 292e 0a20 2020 2020 2020 2020 2020  el)..           
+0002b430: 2020 2020 204f 6e6c 7920 7468 6520 6669       Only the fi
+0002b440: 7273 7420 6d61 7463 6869 6e67 2062 7574  rst matching but
+0002b450: 746f 6e20 7769 6c6c 2062 6520 7072 6573  ton will be pres
+0002b460: 7365 642e 0a0a 2020 2020 2020 2020 5061  sed...        Pa
+0002b470: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+0002b480: 2020 2020 2020 7820 2860 6069 6e74 6060        x (``int``
+0002b490: 207c 2060 6073 7472 6060 293a 0a20 2020   | ``str``):.   
+0002b4a0: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+0002b4b0: 6420 6173 2069 6e74 6567 6572 2069 6e64  d as integer ind
+0002b4c0: 6578 2c20 696e 7465 6765 7220 6162 7363  ex, integer absc
+0002b4d0: 6973 7361 2028 696e 2070 6169 7220 7769  issa (in pair wi
+0002b4e0: 7468 2079 2920 6f72 2061 7320 7374 7269  th y) or as stri
+0002b4f0: 6e67 206c 6162 656c 2e0a 2020 2020 2020  ng label..      
+0002b500: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0002b510: 7473 2074 6f20 3020 2866 6972 7374 2062  ts to 0 (first b
+0002b520: 7574 746f 6e29 2e0a 0a20 2020 2020 2020  utton)...       
+0002b530: 2020 2020 2079 2028 6060 696e 7460 602c       y (``int``,
+0002b540: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
+0002b550: 2020 2020 2020 2020 2020 2020 2020 5573                Us
+0002b560: 6564 2061 7320 6f72 6469 6e61 7465 206f  ed as ordinate o
+0002b570: 6e6c 7920 2869 6e20 7061 6972 2077 6974  nly (in pair wit
+0002b580: 6820 7829 2e0a 0a20 2020 2020 2020 2020  h x)...         
+0002b590: 2020 2071 756f 7465 2028 6060 626f 6f6c     quote (``bool
+0002b5a0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+0002b5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b5c0: 2055 7365 6675 6c20 666f 7220 6e6f 726d   Useful for norm
+0002b5d0: 616c 2062 7574 746f 6e73 206f 6e6c 792c  al buttons only,
+0002b5e0: 2077 6865 7265 2070 7265 7373 696e 6720   where pressing 
+0002b5f0: 6974 2077 696c 6c20 7265 7375 6c74 2069  it will result i
+0002b600: 6e20 6120 6e65 7720 6d65 7373 6167 6520  n a new message 
+0002b610: 7365 6e74 2e0a 2020 2020 2020 2020 2020  sent..          
+0002b620: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
+0002b630: 602c 2074 6865 206d 6573 7361 6765 2077  `, the message w
+0002b640: 696c 6c20 6265 2073 656e 7420 6173 2061  ill be sent as a
+0002b650: 2072 6570 6c79 2074 6f20 7468 6973 206d   reply to this m
+0002b660: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
+0002b670: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+0002b680: 2074 6f20 6060 5472 7565 6060 2069 6e20   to ``True`` in 
+0002b690: 6772 6f75 7020 6368 6174 7320 616e 6420  group chats and 
+0002b6a0: 6060 4661 6c73 6560 6020 696e 2070 7269  ``False`` in pri
+0002b6b0: 7661 7465 2063 6861 7473 2e0a 0a20 2020  vate chats...   
+0002b6c0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0002b6d0: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
+0002b6e0: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+0002b6f0: 2020 2020 2020 2020 5469 6d65 6f75 7420          Timeout 
+0002b700: 696e 2073 6563 6f6e 6473 2e0a 0a20 2020  in seconds...   
+0002b710: 2020 2020 2020 2020 2072 6571 7565 7374           request
+0002b720: 5f77 7269 7465 5f61 6363 6573 7320 2860  _write_access (`
+0002b730: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+0002b740: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+0002b750: 2020 2020 2020 4f6e 6c79 2075 7365 6420        Only used 
+0002b760: 696e 2063 6173 6520 6f66 203a 6f62 6a3a  in case of :obj:
+0002b770: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
+0002b780: 2e4c 6f67 696e 5572 6c60 2062 7574 746f  .LoginUrl` butto
+0002b790: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+0002b7a0: 2020 2054 7275 652c 2069 6620 7468 6520     True, if the 
+0002b7b0: 626f 7420 6361 6e20 7365 6e64 206d 6573  bot can send mes
+0002b7c0: 7361 6765 7320 746f 2074 6865 2075 7365  sages to the use
+0002b7d0: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
+0002b7e0: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
+0002b7f0: 6054 7275 6560 602e 0a0a 2020 2020 2020  `True``...      
+0002b800: 2020 2020 2020 7061 7373 776f 7264 2028        password (
+0002b810: 6060 7374 7260 602c 202a 6f70 7469 6f6e  ``str``, *option
+0002b820: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+0002b830: 2020 2020 2020 5768 656e 2063 6c69 636b        When click
+0002b840: 696e 6720 6365 7274 6169 6e20 6275 7474  ing certain butt
+0002b850: 6f6e 7320 2873 7563 6820 6173 2042 6f74  ons (such as Bot
+0002b860: 4661 7468 6572 2773 2063 6f6e 6669 726d  Father's confirm
+0002b870: 6174 696f 6e20 6275 7474 6f6e 2074 6f20  ation button to 
+0002b880: 7472 616e 7366 6572 206f 776e 6572 7368  transfer ownersh
+0002b890: 6970 292c 2069 6620 796f 7572 2061 6363  ip), if your acc
+0002b8a0: 6f75 6e74 2068 6173 2032 4641 2065 6e61  ount has 2FA ena
+0002b8b0: 626c 6564 2c20 796f 7520 6e65 6564 2074  bled, you need t
+0002b8c0: 6f20 7072 6f76 6964 6520 796f 7572 2061  o provide your a
+0002b8d0: 6363 6f75 6e74 2773 2070 6173 7377 6f72  ccount's passwor
+0002b8e0: 642e 200a 2020 2020 2020 2020 2020 2020  d. .            
+0002b8f0: 2020 2020 5468 6520 322d 7374 6570 2076      The 2-step v
+0002b900: 6572 6966 6963 6174 696f 6e20 7061 7373  erification pass
+0002b910: 776f 7264 2066 6f72 2074 6865 2063 7572  word for the cur
+0002b920: 7265 6e74 2075 7365 722e 204f 6e6c 7920  rent user. Only 
+0002b930: 6170 706c 6963 6162 6c65 2c20 6966 2074  applicable, if t
+0002b940: 6865 203a 6f62 6a3a 607e 7079 726f 6772  he :obj:`~pyrogr
+0002b950: 616d 2e74 7970 6573 2e49 6e6c 696e 654b  am.types.InlineK
+0002b960: 6579 626f 6172 6442 7574 746f 6e60 2063  eyboardButton` c
+0002b970: 6f6e 7461 696e 7320 6060 6361 6c6c 6261  ontains ``callba
+0002b980: 636b 5f64 6174 615f 7769 7468 5f70 6173  ck_data_with_pas
+0002b990: 7377 6f72 6460 602e 0a0a 2020 2020 2020  sword``...      
+0002b9a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0002b9b0: 2020 2020 2020 202d 2020 2054 6865 2072         -   The r
+0002b9c0: 6573 756c 7420 6f66 203a 6d65 7468 3a60  esult of :meth:`
+0002b9d0: 7e70 7972 6f67 7261 6d2e 436c 6965 6e74  ~pyrogram.Client
+0002b9e0: 2e72 6571 7565 7374 5f63 616c 6c62 6163  .request_callbac
+0002b9f0: 6b5f 616e 7377 6572 6020 696e 2063 6173  k_answer` in cas
+0002ba00: 6520 6f66 2069 6e6c 696e 6520 6361 6c6c  e of inline call
+0002ba10: 6261 636b 2062 7574 746f 6e20 636c 6963  back button clic
+0002ba20: 6b73 2e0a 2020 2020 2020 2020 2020 2020  ks..            
+0002ba30: 2d20 2020 5468 6520 7265 7375 6c74 206f  -   The result o
+0002ba40: 6620 3a6d 6574 683a 607e 4d65 7373 6167  f :meth:`~Messag
+0002ba50: 652e 7265 706c 7928 2960 2069 6e20 6361  e.reply()` in ca
+0002ba60: 7365 206f 6620 6e6f 726d 616c 2062 7574  se of normal but
+0002ba70: 746f 6e20 636c 6963 6b73 2e0a 2020 2020  ton clicks..    
+0002ba80: 2020 2020 2020 2020 2d20 2020 4120 7374          -   A st
+0002ba90: 7269 6e67 2069 6e20 6361 7365 2074 6865  ring in case the
+0002baa0: 2069 6e6c 696e 6520 6275 7474 6f6e 2069   inline button i
+0002bab0: 7320 6120 5552 4c2c 2061 202a 7377 6974  s a URL, a *swit
+0002bac0: 6368 5f69 6e6c 696e 655f 7175 6572 792a  ch_inline_query*
+0002bad0: 206f 7220 610a 2020 2020 2020 2020 2020   or a.          
+0002bae0: 2020 2020 2020 2a73 7769 7463 685f 696e        *switch_in
+0002baf0: 6c69 6e65 5f71 7565 7279 5f63 7572 7265  line_query_curre
+0002bb00: 6e74 5f63 6861 742a 2062 7574 746f 6e2e  nt_chat* button.
+0002bb10: 0a20 2020 2020 2020 2020 2020 202d 2020  .            -  
+0002bb20: 2041 2073 7472 696e 6720 5552 4c20 7769   A string URL wi
+0002bb30: 7468 2074 6865 2075 7365 7220 6465 7461  th the user deta
+0002bb40: 696c 732c 2069 6e20 6361 7365 206f 6620  ils, in case of 
+0002bb50: 6120 4c6f 6769 6e55 726c 2062 7574 746f  a LoginUrl butto
+0002bb60: 6e2e 0a20 2020 2020 2020 2020 2020 202d  n..            -
+0002bb70: 2020 2041 203a 6f62 6a3a 607e 7079 726f     A :obj:`~pyro
+0002bb80: 6772 616d 2e74 7970 6573 2e53 7769 7463  gram.types.Switc
+0002bb90: 6849 6e6c 696e 6551 7565 7279 4368 6f73  hInlineQueryChos
+0002bba0: 656e 4368 6174 6020 6f62 6a65 6374 2069  enChat` object i
+0002bbb0: 6e20 6361 7365 206f 6620 6120 6060 7377  n case of a ``sw
+0002bbc0: 6974 6368 5f69 6e6c 696e 655f 7175 6572  itch_inline_quer
+0002bbd0: 795f 6368 6f73 656e 5f63 6861 7460 602e  y_chosen_chat``.
+0002bbe0: 0a20 2020 2020 2020 2020 2020 202d 2020  .            -  
+0002bbf0: 2041 203a 6f62 6a3a 607e 7079 726f 6772   A :obj:`~pyrogr
+0002bc00: 616d 2e74 7970 6573 2e55 7365 7260 206f  am.types.User` o
+0002bc10: 626a 6563 7420 696e 2063 6173 6520 6f66  bject in case of
+0002bc20: 2061 2060 604b 6579 626f 6172 6442 7574   a ``KeyboardBut
+0002bc30: 746f 6e55 7365 7250 726f 6669 6c65 6060  tonUserProfile``
+0002bc40: 2062 7574 746f 6e2e 0a0a 2020 2020 2020   button...      
+0002bc50: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+0002bc60: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
+0002bc70: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
+0002bc80: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
+0002bc90: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+0002bca0: 7565 4572 726f 723a 2049 6e20 6361 7365  ueError: In case
+0002bcb0: 2074 6865 2070 726f 7669 6465 6420 696e   the provided in
+0002bcc0: 6465 7820 6f72 2070 6f73 6974 696f 6e20  dex or position 
+0002bcd0: 6973 206f 7574 206f 6620 7261 6e67 6520  is out of range 
+0002bce0: 6f72 2074 6865 2062 7574 746f 6e20 6c61  or the button la
+0002bcf0: 6265 6c20 7761 7320 6e6f 7420 666f 756e  bel was not foun
+0002bd00: 642e 0a20 2020 2020 2020 2020 2020 2054  d..            T
+0002bd10: 696d 656f 7574 4572 726f 723a 2049 6e20  imeoutError: In 
+0002bd20: 6361 7365 2c20 6166 7465 7220 636c 6963  case, after clic
+0002bd30: 6b69 6e67 2061 6e20 696e 6c69 6e65 2062  king an inline b
+0002bd40: 7574 746f 6e2c 2074 6865 2062 6f74 2066  utton, the bot f
+0002bd50: 6169 6c73 2074 6f20 616e 7377 6572 2077  ails to answer w
+0002bd60: 6974 6869 6e20 7468 6520 7469 6d65 6f75  ithin the timeou
+0002bd70: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
+0002bd80: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0002bd90: 7461 6e63 6528 7365 6c66 2e72 6570 6c79  tance(self.reply
+0002bda0: 5f6d 6172 6b75 702c 2074 7970 6573 2e52  _markup, types.R
+0002bdb0: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
+0002bdc0: 7570 293a 0a20 2020 2020 2020 2020 2020  up):.           
+0002bdd0: 206b 6579 626f 6172 6420 3d20 7365 6c66   keyboard = self
+0002bde0: 2e72 6570 6c79 5f6d 6172 6b75 702e 6b65  .reply_markup.ke
+0002bdf0: 7962 6f61 7264 0a20 2020 2020 2020 2020  yboard.         
+0002be00: 2020 2069 735f 696e 6c69 6e65 203d 2046     is_inline = F
+0002be10: 616c 7365 0a20 2020 2020 2020 2065 6c69  alse.        eli
+0002be20: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
+0002be30: 662e 7265 706c 795f 6d61 726b 7570 2c20  f.reply_markup, 
+0002be40: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
+0002be50: 6f61 7264 4d61 726b 7570 293a 0a20 2020  oardMarkup):.   
+0002be60: 2020 2020 2020 2020 206b 6579 626f 6172           keyboar
+0002be70: 6420 3d20 7365 6c66 2e72 6570 6c79 5f6d  d = self.reply_m
+0002be80: 6172 6b75 702e 696e 6c69 6e65 5f6b 6579  arkup.inline_key
+0002be90: 626f 6172 640a 2020 2020 2020 2020 2020  board.          
+0002bea0: 2020 6973 5f69 6e6c 696e 6520 3d20 5472    is_inline = Tr
+0002beb0: 7565 0a20 2020 2020 2020 2065 6c73 653a  ue.        else:
+0002bec0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0002bed0: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
+0002bee0: 6865 206d 6573 7361 6765 2064 6f65 736e  he message doesn
+0002bef0: 2774 2063 6f6e 7461 696e 2061 6e79 206b  't contain any k
+0002bf00: 6579 626f 6172 6422 290a 0a20 2020 2020  eyboard")..     
+0002bf10: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0002bf20: 2878 2c20 696e 7429 2061 6e64 2079 2069  (x, int) and y i
+0002bf30: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0002bf40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0002bf50: 2020 2020 2020 2020 2062 7574 746f 6e20           button 
+0002bf60: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0002bf70: 2020 2020 2020 2020 6275 7474 6f6e 0a20          button. 
+0002bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bf90: 2020 2066 6f72 2072 6f77 2069 6e20 6b65     for row in ke
+0002bfa0: 7962 6f61 7264 0a20 2020 2020 2020 2020  yboard.         
+0002bfb0: 2020 2020 2020 2020 2020 2066 6f72 2062             for b
+0002bfc0: 7574 746f 6e20 696e 2072 6f77 0a20 2020  utton in row.   
+0002bfd0: 2020 2020 2020 2020 2020 2020 205d 5b78               ][x
+0002bfe0: 5d0a 2020 2020 2020 2020 2020 2020 6578  ].            ex
+0002bff0: 6365 7074 2049 6e64 6578 4572 726f 723a  cept IndexError:
+0002c000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c010: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0002c020: 7228 6622 5468 6520 6275 7474 6f6e 2061  r(f"The button a
+0002c030: 7420 696e 6465 7820 7b78 7d20 646f 6573  t index {x} does
+0002c040: 6e27 7420 6578 6973 7422 290a 2020 2020  n't exist").    
+0002c050: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0002c060: 6e63 6528 782c 2069 6e74 2920 616e 6420  nce(x, int) and 
+0002c070: 6973 696e 7374 616e 6365 2879 2c20 696e  isinstance(y, in
+0002c080: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0002c090: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0002c0a0: 2020 2020 2062 7574 746f 6e20 3d20 6b65       button = ke
+0002c0b0: 7962 6f61 7264 5b79 5d5b 785d 0a20 2020  yboard[y][x].   
+0002c0c0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0002c0d0: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
+0002c0e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002c0f0: 6520 5661 6c75 6545 7272 6f72 2866 2254  e ValueError(f"T
+0002c100: 6865 2062 7574 746f 6e20 6174 2070 6f73  he button at pos
+0002c110: 6974 696f 6e20 287b 787d 2c20 7b79 7d29  ition ({x}, {y})
+0002c120: 2064 6f65 736e 2774 2065 7869 7374 2229   doesn't exist")
+0002c130: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+0002c140: 696e 7374 616e 6365 2878 2c20 7374 7229  instance(x, str)
+0002c150: 2061 6e64 2079 2069 7320 4e6f 6e65 3a0a   and y is None:.
+0002c160: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0002c170: 6c20 3d20 782e 656e 636f 6465 2822 7574  l = x.encode("ut
+0002c180: 662d 3136 222c 2022 7375 7272 6f67 6174  f-16", "surrogat
+0002c190: 6570 6173 7322 292e 6465 636f 6465 2822  epass").decode("
+0002c1a0: 7574 662d 3136 2229 0a0a 2020 2020 2020  utf-16")..      
+0002c1b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0002c1c0: 2020 2020 2020 2020 2020 2062 7574 746f             butto
+0002c1d0: 6e20 3d20 5b0a 2020 2020 2020 2020 2020  n = [.          
+0002c1e0: 2020 2020 2020 2020 2020 6275 7474 6f6e            button
+0002c1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c200: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
+0002c210: 6b65 7962 6f61 7264 0a20 2020 2020 2020  keyboard.       
+0002c220: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0002c230: 2062 7574 746f 6e20 696e 2072 6f77 0a20   button in row. 
+0002c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c250: 2020 2069 6620 6c61 6265 6c20 3d3d 2062     if label == b
+0002c260: 7574 746f 6e2e 7465 7874 0a20 2020 2020  utton.text.     
+0002c270: 2020 2020 2020 2020 2020 205d 5b30 5d0a             ][0].
+0002c280: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0002c290: 7074 2049 6e64 6578 4572 726f 723a 0a20  pt IndexError:. 
+0002c2a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002c2b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0002c2c0: 6622 5468 6520 6275 7474 6f6e 2077 6974  f"The button wit
+0002c2d0: 6820 6c61 6265 6c20 277b 787d 2720 646f  h label '{x}' do
+0002c2e0: 6573 6e27 7420 6578 6973 7473 2229 0a20  esn't exists"). 
+0002c2f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0002c300: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0002c310: 616c 7565 4572 726f 7228 2249 6e76 616c  alueError("Inval
+0002c320: 6964 2061 7267 756d 656e 7473 2229 0a0a  id arguments")..
+0002c330: 2020 2020 2020 2020 6966 2069 735f 696e          if is_in
+0002c340: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
+0002c350: 2020 6966 2062 7574 746f 6e2e 6361 6c6c    if button.call
+0002c360: 6261 636b 5f64 6174 613a 0a20 2020 2020  back_data:.     
+0002c370: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002c380: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
+0002c390: 6965 6e74 2e72 6571 7565 7374 5f63 616c  ient.request_cal
+0002c3a0: 6c62 6163 6b5f 616e 7377 6572 280a 2020  lback_answer(.  
+0002c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c3c0: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
+0002c3d0: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+0002c3e0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+0002c3f0: 6167 655f 6964 3d73 656c 662e 6964 2c0a  age_id=self.id,.
 0002c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c410: 2020 7572 6c3d 746c 752e 7572 6c0a 2020    url=tlu.url.  
-0002c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c430: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0002c440: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0002c450: 2020 2020 2020 7469 7564 6b6f 203d 2061        tiudko = a
-0002c460: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-0002c470: 742e 696e 766f 6b65 280a 2020 2020 2020  t.invoke(.      
-0002c480: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0002c490: 772e 6675 6e63 7469 6f6e 732e 6d65 7373  w.functions.mess
-0002c4a0: 6167 6573 2e41 6363 6570 7455 726c 4175  ages.AcceptUrlAu
-0002c4b0: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-0002c4c0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-0002c4d0: 655f 616c 6c6f 7765 643d 7265 7175 6573  e_allowed=reques
-0002c4e0: 745f 7772 6974 655f 6163 6365 7373 2c0a  t_write_access,.
+0002c410: 2020 2020 6361 6c6c 6261 636b 5f64 6174      callback_dat
+0002c420: 613d 6275 7474 6f6e 2e63 616c 6c62 6163  a=button.callbac
+0002c430: 6b5f 6461 7461 2c0a 2020 2020 2020 2020  k_data,.        
+0002c440: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0002c450: 6f75 743d 7469 6d65 6f75 740a 2020 2020  out=timeout.    
+0002c460: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002c470: 2020 2020 2020 2020 2020 656c 6966 2062            elif b
+0002c480: 7574 746f 6e2e 6361 6c6c 6261 636b 5f64  utton.callback_d
+0002c490: 6174 615f 7769 7468 5f70 6173 7377 6f72  ata_with_passwor
+0002c4a0: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+0002c4b0: 2020 2069 6620 7061 7373 776f 7264 2069     if password i
+0002c4c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0002c4d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002c4e0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
 0002c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c500: 2020 2020 2020 2020 7065 6572 3d72 6965          peer=rie
-0002c510: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
-0002c520: 2020 2020 2020 2020 2020 2020 6d73 675f              msg_
-0002c530: 6964 3d73 656c 662e 6964 2c0a 2020 2020  id=self.id,.    
-0002c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c550: 2020 2020 6275 7474 6f6e 5f69 643d 746c      button_id=tl
-0002c560: 752e 6275 7474 6f6e 5f69 642c 0a20 2020  u.button_id,.   
-0002c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c580: 2020 2020 2075 726c 3d74 6c75 2e75 726c       url=tlu.url
-0002c590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c5a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0002c5b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002c5c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002c5d0: 7469 7564 6b6f 2e75 726c 0a20 2020 2020  tiudko.url.     
-0002c5e0: 2020 2020 2020 2065 6c69 6620 6275 7474         elif butt
-0002c5f0: 6f6e 2e77 6562 5f61 7070 3a0a 2020 2020  on.web_app:.    
-0002c600: 2020 2020 2020 2020 2020 2020 746c 7520              tlu 
-0002c610: 3d20 6275 7474 6f6e 2e77 6562 5f61 7070  = button.web_app
-0002c620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c630: 2077 6869 6368 626f 7463 6861 7420 3d20   whichbotchat = 
-0002c640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c650: 2020 2020 2020 7365 6c66 2e76 6961 5f62        self.via_b
-0002c660: 6f74 2061 6e64 0a20 2020 2020 2020 2020  ot and.         
-0002c670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002c680: 7669 615f 626f 742e 6964 0a20 2020 2020  via_bot.id.     
-0002c690: 2020 2020 2020 2020 2020 2029 206f 7220             ) or 
-0002c6a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c6b0: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-0002c6c0: 7573 6572 2061 6e64 0a20 2020 2020 2020  user and.       
-0002c6d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0002c6e0: 662e 6672 6f6d 5f75 7365 722e 6973 5f62  f.from_user.is_b
-0002c6f0: 6f74 2061 6e64 0a20 2020 2020 2020 2020  ot and.         
-0002c700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002c710: 6672 6f6d 5f75 7365 722e 6964 0a20 2020  from_user.id.   
-0002c720: 2020 2020 2020 2020 2020 2020 2029 206f               ) o
-0002c730: 7220 4e6f 6e65 0a20 2020 2020 2020 2020  r None.         
-0002c740: 2020 2020 2020 2069 6620 6e6f 7420 7768         if not wh
-0002c750: 6963 6862 6f74 6368 6174 3a0a 2020 2020  ichbotchat:.    
-0002c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c770: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0002c780: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c790: 2020 2020 2020 2020 2020 2249 6e76 616c            "Inval
-0002c7a0: 6964 2043 6861 7442 6f74 5479 7065 220a  id ChatBotType".
-0002c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c7c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0002c7d0: 2020 2020 2020 7269 6565 7020 3d20 6177        rieep = aw
-0002c7e0: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-0002c7f0: 2e72 6573 6f6c 7665 5f70 6565 7228 0a20  .resolve_peer(. 
-0002c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c810: 2020 2073 656c 662e 6368 6174 2e69 640a     self.chat.id.
+0002c500: 2020 2020 2020 2249 6e76 616c 6964 2061        "Invalid a
+0002c510: 7267 756d 656e 7420 7061 7373 6564 220a  rgument passed".
+0002c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c530: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0002c540: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0002c550: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+0002c560: 7265 7175 6573 745f 6361 6c6c 6261 636b  request_callback
+0002c570: 5f61 6e73 7765 7228 0a20 2020 2020 2020  _answer(.       
+0002c580: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0002c590: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+0002c5a0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0002c5b0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
+0002c5c0: 643d 7365 6c66 2e69 642c 0a20 2020 2020  d=self.id,.     
+0002c5d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0002c5e0: 616c 6c62 6163 6b5f 6461 7461 3d62 7574  allback_data=but
+0002c5f0: 746f 6e2e 6361 6c6c 6261 636b 5f64 6174  ton.callback_dat
+0002c600: 615f 7769 7468 5f70 6173 7377 6f72 642c  a_with_password,
+0002c610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c620: 2020 2020 2070 6173 7377 6f72 643d 7061       password=pa
+0002c630: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+0002c640: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0002c650: 6f75 743d 7469 6d65 6f75 740a 2020 2020  out=timeout.    
+0002c660: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002c670: 2020 2020 2020 2020 2020 656c 6966 2062            elif b
+0002c680: 7574 746f 6e2e 7572 6c3a 0a20 2020 2020  utton.url:.     
+0002c690: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002c6a0: 6e20 6275 7474 6f6e 2e75 726c 0a20 2020  n button.url.   
+0002c6b0: 2020 2020 2020 2020 2065 6c69 6620 6275           elif bu
+0002c6c0: 7474 6f6e 2e6c 6f67 696e 5f75 726c 3a0a  tton.login_url:.
+0002c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c6e0: 746c 7520 3d20 6275 7474 6f6e 2e6c 6f67  tlu = button.log
+0002c6f0: 696e 5f75 726c 0a20 2020 2020 2020 2020  in_url.         
+0002c700: 2020 2020 2020 2072 6965 6570 203d 2061         rieep = a
+0002c710: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+0002c720: 742e 7265 736f 6c76 655f 7065 6572 280a  t.resolve_peer(.
+0002c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c740: 2020 2020 7365 6c66 2e63 6861 742e 6964      self.chat.id
+0002c750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c760: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0002c770: 2020 206f 6b64 7569 7420 3d20 6177 6169     okduit = awai
+0002c780: 7420 7365 6c66 2e5f 636c 6965 6e74 2e69  t self._client.i
+0002c790: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
+0002c7a0: 2020 2020 2020 2020 2020 2072 6177 2e66             raw.f
+0002c7b0: 756e 6374 696f 6e73 2e6d 6573 7361 6765  unctions.message
+0002c7c0: 732e 5265 7175 6573 7455 726c 4175 7468  s.RequestUrlAuth
+0002c7d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002c7e0: 2020 2020 2020 2020 2020 7065 6572 3d72            peer=r
+0002c7f0: 6965 6570 2c0a 2020 2020 2020 2020 2020  ieep,.          
+0002c800: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+0002c810: 675f 6964 3d73 656c 662e 6964 2c0a 2020  g_id=self.id,.  
 0002c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c830: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002c840: 2020 6965 6570 7220 3d20 6177 6169 7420    ieepr = await 
-0002c850: 7365 6c66 2e5f 636c 6965 6e74 2e72 6573  self._client.res
-0002c860: 6f6c 7665 5f70 6565 7228 0a20 2020 2020  olve_peer(.     
-0002c870: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0002c880: 6869 6368 626f 7463 6861 740a 2020 2020  hichbotchat.    
-0002c890: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0002c8a0: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
-0002c8b0: 6475 6974 203d 2061 7761 6974 2073 656c  duit = await sel
-0002c8c0: 662e 5f63 6c69 656e 742e 696e 766f 6b65  f._client.invoke
-0002c8d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002c8e0: 2020 2020 2020 7261 772e 6675 6e63 7469        raw.functi
-0002c8f0: 6f6e 732e 6d65 7373 6167 6573 2e52 6571  ons.messages.Req
-0002c900: 7565 7374 5765 6256 6965 7728 0a20 2020  uestWebView(.   
+0002c830: 2020 2020 2020 6275 7474 6f6e 5f69 643d        button_id=
+0002c840: 746c 752e 6275 7474 6f6e 5f69 642c 0a20  tlu.button_id,. 
+0002c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c860: 2020 2020 2020 2075 726c 3d74 6c75 2e75         url=tlu.u
+0002c870: 726c 0a20 2020 2020 2020 2020 2020 2020  rl.             
+0002c880: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002c890: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0002c8a0: 2020 2020 2020 2020 2020 2074 6975 646b             tiudk
+0002c8b0: 6f20 3d20 6177 6169 7420 7365 6c66 2e5f  o = await self._
+0002c8c0: 636c 6965 6e74 2e69 6e76 6f6b 6528 0a20  client.invoke(. 
+0002c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c8e0: 2020 2072 6177 2e66 756e 6374 696f 6e73     raw.functions
+0002c8f0: 2e6d 6573 7361 6765 732e 4163 6365 7074  .messages.Accept
+0002c900: 5572 6c41 7574 6828 0a20 2020 2020 2020  UrlAuth(.       
 0002c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c920: 2020 2020 2070 6565 723d 7269 6565 702c       peer=rieep,
-0002c930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c940: 2020 2020 2020 2020 2062 6f74 3d69 6565           bot=iee
-0002c950: 7072 2c0a 2020 2020 2020 2020 2020 2020  pr,.            
-0002c960: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-0002c970: 746c 752e 7572 6c2c 0a20 2020 2020 2020  tlu.url,.       
-0002c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c990: 2070 6c61 7466 6f72 6d3d 7365 6c66 2e5f   platform=self._
-0002c9a0: 636c 6965 6e74 2e63 6c69 656e 745f 706c  client.client_pl
-0002c9b0: 6174 666f 726d 2e76 616c 7565 2c0a 2020  atform.value,.  
-0002c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c9d0: 2020 2020 2020 2320 544f 444f 0a20 2020        # TODO.   
-0002c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c9f0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0002ca00: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002ca10: 2020 2020 2072 6574 7572 6e20 6f6b 6475       return okdu
-0002ca20: 6974 2e75 726c 0a20 2020 2020 2020 2020  it.url.         
-0002ca30: 2020 2065 6c69 6620 6275 7474 6f6e 2e75     elif button.u
-0002ca40: 7365 725f 6964 3a0a 2020 2020 2020 2020  ser_id:.        
-0002ca50: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0002ca60: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-0002ca70: 742e 6765 745f 6368 6174 280a 2020 2020  t.get_chat(.    
-0002ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca90: 6275 7474 6f6e 2e75 7365 725f 6964 2c0a  button.user_id,.
-0002caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cab0: 2020 2020 4661 6c73 650a 2020 2020 2020      False.      
-0002cac0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0002cad0: 2020 2020 2020 2020 656c 6966 2062 7574          elif but
-0002cae0: 746f 6e2e 7377 6974 6368 5f69 6e6c 696e  ton.switch_inlin
-0002caf0: 655f 7175 6572 793a 0a20 2020 2020 2020  e_query:.       
-0002cb00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002cb10: 6275 7474 6f6e 2e73 7769 7463 685f 696e  button.switch_in
-0002cb20: 6c69 6e65 5f71 7565 7279 0a20 2020 2020  line_query.     
-0002cb30: 2020 2020 2020 2065 6c69 6620 6275 7474         elif butt
-0002cb40: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
-0002cb50: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
-0002cb60: 6861 743a 0a20 2020 2020 2020 2020 2020  hat:.           
-0002cb70: 2020 2020 2072 6574 7572 6e20 6275 7474       return butt
-0002cb80: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
-0002cb90: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
-0002cba0: 6861 740a 2020 2020 2020 2020 2020 2020  hat.            
-0002cbb0: 656c 6966 2062 7574 746f 6e2e 7377 6974  elif button.swit
-0002cbc0: 6368 5f69 6e6c 696e 655f 7175 6572 795f  ch_inline_query_
-0002cbd0: 6368 6f73 656e 5f63 6861 743a 0a20 2020  chosen_chat:.   
-0002cbe0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0002cbf0: 7572 6e20 6275 7474 6f6e 2e73 7769 7463  urn button.switc
-0002cc00: 685f 696e 6c69 6e65 5f71 7565 7279 5f63  h_inline_query_c
-0002cc10: 686f 7365 6e5f 6368 6174 0a20 2020 2020  hosen_chat.     
-0002cc20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0002cc30: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0002cc40: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-0002cc50: 6869 7320 6275 7474 6f6e 2069 7320 6e6f  his button is no
-0002cc60: 7420 7375 7070 6f72 7465 6420 7965 7422  t supported yet"
-0002cc70: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0002cc80: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0002cc90: 7420 7365 6c66 2e72 6570 6c79 2874 6578  t self.reply(tex
-0002cca0: 743d 6275 7474 6f6e 2c20 7175 6f74 653d  t=button, quote=
-0002ccb0: 7175 6f74 6529 0a0a 2020 2020 6173 796e  quote)..    asyn
-0002ccc0: 6320 6465 6620 7265 6163 7428 0a20 2020  c def react(.   
-0002ccd0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002cce0: 2020 2072 6561 6374 696f 6e3a 2055 6e69     reaction: Uni
-0002ccf0: 6f6e 5b0a 2020 2020 2020 2020 2020 2020  on[.            
-0002cd00: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-0002cd10: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-0002cd20: 2020 4c69 7374 5b55 6e69 6f6e 5b69 6e74    List[Union[int
-0002cd30: 2c20 7374 722c 2022 7479 7065 732e 5265  , str, "types.Re
-0002cd40: 6163 7469 6f6e 5479 7065 225d 5d0a 2020  actionType"]].  
-0002cd50: 2020 2020 2020 5d20 3d20 4e6f 6e65 2c0a        ] = None,.
-0002cd60: 2020 2020 2020 2020 6973 5f62 6967 3a20          is_big: 
-0002cd70: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0002cd80: 2020 2020 2020 6164 645f 746f 5f72 6563        add_to_rec
-0002cd90: 656e 743a 2062 6f6f 6c20 3d20 5472 7565  ent: bool = True
-0002cda0: 0a20 2020 2029 202d 3e20 2274 7970 6573  .    ) -> "types
-0002cdb0: 2e4d 6573 7361 6765 5265 6163 7469 6f6e  .MessageReaction
-0002cdc0: 7322 3a0a 2020 2020 2020 2020 2222 2242  s":.        """B
-0002cdd0: 6f75 6e64 206d 6574 686f 6420 2a72 6561  ound method *rea
-0002cde0: 6374 2a20 6f66 203a 6f62 6a3a 607e 7079  ct* of :obj:`~py
-0002cdf0: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
-0002ce00: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
-0002ce10: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-0002ce20: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
-0002ce30: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-0002ce40: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-0002ce50: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-0002ce60: 2e73 6574 5f72 6561 6374 696f 6e28 0a20  .set_reaction(. 
-0002ce70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002ce80: 6861 745f 6964 3d63 6861 745f 6964 2c0a  hat_id=chat_id,.
-0002ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cea0: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-0002ceb0: 6765 2e69 642c 0a20 2020 2020 2020 2020  ge.id,.         
-0002cec0: 2020 2020 2020 2072 6561 6374 696f 6e3d         reaction=
-0002ced0: 5b52 6561 6374 696f 6e54 7970 6545 6d6f  [ReactionTypeEmo
-0002cee0: 6a69 2865 6d6f 6a69 3d22 f09f 918d 2229  ji(emoji="....")
-0002cef0: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-0002cf00: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002cf10: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-0002cf20: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002cf30: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002cf40: 2020 2020 2020 2320 5365 6e64 2061 2072        # Send a r
-0002cf50: 6561 6374 696f 6e0a 2020 2020 2020 2020  eaction.        
-0002cf60: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-0002cf70: 7373 6167 652e 7265 6163 7428 5b52 6561  ssage.react([Rea
-0002cf80: 6374 696f 6e54 7970 6545 6d6f 6a69 2865  ctionTypeEmoji(e
-0002cf90: 6d6f 6a69 3d22 f09f 918d 2229 5d29 0a0a  moji="....")])..
-0002cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cfb0: 2320 5265 7472 6163 7420 6120 7265 6163  # Retract a reac
-0002cfc0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0002cfd0: 2020 2020 2061 7761 6974 206d 6573 7361       await messa
-0002cfe0: 6765 2e72 6561 6374 2829 0a0a 2020 2020  ge.react()..    
-0002cff0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-0002d000: 2020 2020 2020 2020 2020 2020 7265 6163              reac
-0002d010: 7469 6f6e 2028 6060 696e 7460 6020 7c20  tion (``int`` | 
-0002d020: 6060 7374 7260 6020 7c20 4c69 7374 206f  ``str`` | List o
-0002d030: 6620 6060 696e 7460 6020 4f52 2060 6073  f ``int`` OR ``s
-0002d040: 7472 6060 207c 204c 6973 7420 6f66 203a  tr`` | List of :
-0002d050: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
-0002d060: 7970 6573 2e52 6561 6374 696f 6e54 7970  ypes.ReactionTyp
-0002d070: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
-0002d080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d090: 204e 6577 206c 6973 7420 6f66 2072 6561   New list of rea
-0002d0a0: 6374 696f 6e20 7479 7065 7320 746f 2073  ction types to s
-0002d0b0: 6574 206f 6e20 7468 6520 6d65 7373 6167  et on the messag
-0002d0c0: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002d0d0: 2020 2050 6173 7320 4e6f 6e65 2061 7320     Pass None as 
-0002d0e0: 656d 6f6a 6920 2864 6566 6175 6c74 2920  emoji (default) 
-0002d0f0: 746f 2072 6574 7261 6374 2074 6865 2072  to retract the r
-0002d100: 6561 6374 696f 6e2e 0a0a 2020 2020 2020  eaction...      
-0002d110: 2020 2020 2020 6973 5f62 6967 2028 6060        is_big (``
-0002d120: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-0002d130: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-0002d140: 2020 2020 2050 6173 7320 5472 7565 2074       Pass True t
-0002d150: 6f20 7365 7420 7468 6520 7265 6163 7469  o set the reacti
-0002d160: 6f6e 2077 6974 6820 6120 6269 6720 616e  on with a big an
-0002d170: 696d 6174 696f 6e2e 0a20 2020 2020 2020  imation..       
-0002d180: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0002d190: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
-0002d1a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002d1b0: 2020 2020 2061 6464 5f74 6f5f 7265 6365       add_to_rece
-0002d1c0: 6e74 2028 6060 626f 6f6c 6060 2c20 2a6f  nt (``bool``, *o
-0002d1d0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0002d1e0: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-0002d1f0: 5472 7565 2069 6620 7468 6520 7265 6163  True if the reac
-0002d200: 7469 6f6e 2073 686f 756c 6420 6170 7065  tion should appe
-0002d210: 6172 2069 6e20 7468 6520 7265 6365 6e74  ar in the recent
-0002d220: 6c79 2075 7365 6420 7265 6163 7469 6f6e  ly used reaction
-0002d230: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-0002d240: 2020 2054 6869 7320 6f70 7469 6f6e 2069     This option i
-0002d250: 7320 6170 706c 6963 6162 6c65 206f 6e6c  s applicable onl
-0002d260: 7920 666f 7220 7573 6572 732e 0a20 2020  y for users..   
-0002d270: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-0002d280: 6175 6c74 7320 746f 2054 7275 652e 0a20  aults to True.. 
-0002d290: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0002d2a0: 2020 2020 2020 2020 2020 2020 4f6e 2073              On s
-0002d2b0: 7563 6365 7373 2c20 3a6f 626a 3a60 7e70  uccess, :obj:`~p
-0002d2c0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-0002d2d0: 7373 6167 6552 6561 6374 696f 6e73 603a  ssageReactions`:
-0002d2e0: 2069 7320 7265 7475 726e 6564 2e0a 0a20   is returned... 
-0002d2f0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-0002d300: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
-0002d310: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
-0002d320: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
-0002d330: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
-0002d340: 220a 2020 2020 2020 2020 7372 203d 204e  ".        sr = N
-0002d350: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-0002d360: 6973 696e 7374 616e 6365 2872 6561 6374  isinstance(react
-0002d370: 696f 6e2c 204c 6973 7429 3a0a 2020 2020  ion, List):.    
-0002d380: 2020 2020 2020 2020 7372 203d 205b 5d0a          sr = [].
-0002d390: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0002d3a0: 6920 696e 2072 6561 6374 696f 6e3a 0a20  i in reaction:. 
-0002d3b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002d3c0: 6620 6973 696e 7374 616e 6365 2869 2c20  f isinstance(i, 
-0002d3d0: 7479 7065 732e 5265 6163 7469 6f6e 5479  types.ReactionTy
-0002d3e0: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
-0002d3f0: 2020 2020 2020 2020 2073 722e 6170 7065           sr.appe
-0002d400: 6e64 2869 290a 2020 2020 2020 2020 2020  nd(i).          
-0002d410: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0002d420: 7461 6e63 6528 692c 2069 6e74 293a 0a20  tance(i, int):. 
-0002d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d440: 2020 2073 722e 6170 7065 6e64 2874 7970     sr.append(typ
-0002d450: 6573 2e52 6561 6374 696f 6e54 7970 6543  es.ReactionTypeC
-0002d460: 7573 746f 6d45 6d6f 6a69 280a 2020 2020  ustomEmoji(.    
-0002d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d480: 2020 2020 6375 7374 6f6d 5f65 6d6f 6a69      custom_emoji
-0002d490: 5f69 643d 7374 7228 6929 0a20 2020 2020  _id=str(i).     
-0002d4a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0002d4b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002d4c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002d4d0: 2020 2020 2020 2020 2020 2020 7372 2e61              sr.a
-0002d4e0: 7070 656e 6428 7479 7065 732e 5265 6163  ppend(types.Reac
-0002d4f0: 7469 6f6e 5479 7065 456d 6f6a 6928 0a20  tionTypeEmoji(. 
-0002d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d510: 2020 2020 2020 2065 6d6f 6a69 3d69 0a20         emoji=i. 
-0002d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d530: 2020 2029 290a 0a20 2020 2020 2020 2065     ))..        e
-0002d540: 6c69 6620 6973 696e 7374 616e 6365 2872  lif isinstance(r
-0002d550: 6561 6374 696f 6e2c 2069 6e74 293a 0a20  eaction, int):. 
-0002d560: 2020 2020 2020 2020 2020 2073 7220 3d20             sr = 
-0002d570: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0002d580: 2020 7479 7065 732e 5265 6163 7469 6f6e    types.Reaction
-0002d590: 5479 7065 4375 7374 6f6d 456d 6f6a 6928  TypeCustomEmoji(
-0002d5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d5b0: 2020 2020 2063 7573 746f 6d5f 656d 6f6a       custom_emoj
-0002d5c0: 695f 6964 3d73 7472 2872 6561 6374 696f  i_id=str(reactio
-0002d5d0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-0002d5e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0002d5f0: 205d 0a0a 2020 2020 2020 2020 656c 6966   ]..        elif
-0002d600: 2069 7369 6e73 7461 6e63 6528 7265 6163   isinstance(reac
-0002d610: 7469 6f6e 2c20 7374 7229 3a0a 2020 2020  tion, str):.    
-0002d620: 2020 2020 2020 2020 7372 203d 205b 0a20          sr = [. 
-0002d630: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002d640: 7970 6573 2e52 6561 6374 696f 6e54 7970  ypes.ReactionTyp
-0002d650: 6545 6d6f 6a69 280a 2020 2020 2020 2020  eEmoji(.        
-0002d660: 2020 2020 2020 2020 2020 2020 656d 6f6a              emoj
-0002d670: 693d 7265 6163 7469 6f6e 0a20 2020 2020  i=reaction.     
-0002d680: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002d690: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
-0002d6a0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0002d6b0: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
-0002d6c0: 745f 7265 6163 7469 6f6e 280a 2020 2020  t_reaction(.    
-0002d6d0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0002d6e0: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
-0002d6f0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0002d700: 655f 6964 3d73 656c 662e 6964 2c0a 2020  e_id=self.id,.  
-0002d710: 2020 2020 2020 2020 2020 7265 6163 7469            reacti
-0002d720: 6f6e 3d73 722c 0a20 2020 2020 2020 2020  on=sr,.         
-0002d730: 2020 2069 735f 6269 673d 6973 5f62 6967     is_big=is_big
-0002d740: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
-0002d750: 645f 746f 5f72 6563 656e 743d 6164 645f  d_to_recent=add_
-0002d760: 746f 5f72 6563 656e 740a 2020 2020 2020  to_recent.      
-0002d770: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-0002d780: 6566 2072 6574 7261 6374 5f76 6f74 6528  ef retract_vote(
-0002d790: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002d7a0: 2020 2029 202d 3e20 2274 7970 6573 2e50     ) -> "types.P
-0002d7b0: 6f6c 6c22 3a0a 2020 2020 2020 2020 2222  oll":.        ""
-0002d7c0: 2242 6f75 6e64 206d 6574 686f 6420 2a72  "Bound method *r
-0002d7d0: 6574 7261 6374 5f76 6f74 652a 206f 6620  etract_vote* of 
-0002d7e0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-0002d7f0: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
-0002d800: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
-0002d810: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
-0002d820: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-0002d830: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-0002d840: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-0002d850: 656e 742e 7265 7472 6163 745f 766f 7465  ent.retract_vote
-0002d860: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002d870: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
-0002d880: 652e 6368 6174 2e69 642c 0a20 2020 2020  e.chat.id,.     
-0002d890: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0002d8a0: 6765 5f69 643d 6d65 7373 6167 655f 6964  ge_id=message_id
-0002d8b0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0002d8c0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002d8d0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-0002d8e0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002d8f0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002d900: 2020 2020 2020 6d65 7373 6167 652e 7265        message.re
-0002d910: 7472 6163 745f 766f 7465 2829 0a0a 2020  tract_vote()..  
-0002d920: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0002d930: 2020 2020 2020 2020 2020 203a 6f62 6a3a             :obj:
-0002d940: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
-0002d950: 2e50 6f6c 6c60 3a20 4f6e 2073 7563 6365  .Poll`: On succe
-0002d960: 7373 2c20 7468 6520 706f 6c6c 2077 6974  ss, the poll wit
-0002d970: 6820 7468 6520 7265 7472 6163 7465 6420  h the retracted 
-0002d980: 766f 7465 2069 7320 7265 7475 726e 6564  vote is returned
-0002d990: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-0002d9a0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-0002d9b0: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-0002d9c0: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-0002d9d0: 5043 2065 7272 6f72 2e0a 2020 2020 2020  PC error..      
-0002d9e0: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-0002d9f0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0002da00: 2e5f 636c 6965 6e74 2e72 6574 7261 6374  ._client.retract
-0002da10: 5f76 6f74 6528 0a20 2020 2020 2020 2020  _vote(.         
-0002da20: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
-0002da30: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
-0002da40: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
-0002da50: 7365 6c66 2e69 640a 2020 2020 2020 2020  self.id.        
-0002da60: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0002da70: 2064 6f77 6e6c 6f61 6428 0a20 2020 2020   download(.     
-0002da80: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0002da90: 2066 696c 655f 6e61 6d65 3a20 7374 7220   file_name: str 
-0002daa0: 3d20 2222 2c0a 2020 2020 2020 2020 696e  = "",.        in
-0002dab0: 5f6d 656d 6f72 793a 2062 6f6f 6c20 3d20  _memory: bool = 
-0002dac0: 4661 6c73 652c 0a20 2020 2020 2020 2062  False,.        b
-0002dad0: 6c6f 636b 3a20 626f 6f6c 203d 2054 7275  lock: bool = Tru
-0002dae0: 652c 0a20 2020 2020 2020 2070 726f 6772  e,.        progr
-0002daf0: 6573 733a 2043 616c 6c61 626c 6520 3d20  ess: Callable = 
-0002db00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-0002db10: 6f67 7265 7373 5f61 7267 733a 2074 7570  ogress_args: tup
-0002db20: 6c65 203d 2028 290a 2020 2020 2920 2d3e  le = ().    ) ->
-0002db30: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-0002db40: 2242 6f75 6e64 206d 6574 686f 6420 2a64  "Bound method *d
-0002db50: 6f77 6e6c 6f61 642a 206f 6620 3a6f 626a  ownload* of :obj
-0002db60: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-0002db70: 732e 4d65 7373 6167 6560 2e0a 0a20 2020  s.Message`...   
-0002db80: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-0002db90: 6f72 7463 7574 2066 6f72 3a0a 0a20 2020  ortcut for:..   
-0002dba0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-0002dbb0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-0002dbc0: 2020 2020 2020 2020 2061 7761 6974 2063           await c
-0002dbd0: 6c69 656e 742e 646f 776e 6c6f 6164 5f6d  lient.download_m
-0002dbe0: 6564 6961 286d 6573 7361 6765 290a 0a20  edia(message).. 
-0002dbf0: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-0002dc00: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0002dc10: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0002dc20: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0002dc30: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-0002dc40: 652e 646f 776e 6c6f 6164 2829 0a0a 2020  e.download()..  
-0002dc50: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0002dc60: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-0002dc70: 6c65 5f6e 616d 6520 2860 6073 7472 6060  le_name (``str``
-0002dc80: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
-0002dc90: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0002dca0: 2063 7573 746f 6d20 2a66 696c 655f 6e61   custom *file_na
-0002dcb0: 6d65 2a20 746f 2062 6520 7573 6564 2069  me* to be used i
-0002dcc0: 6e73 7465 6164 206f 6620 7468 6520 6f6e  nstead of the on
-0002dcd0: 6520 7072 6f76 6964 6564 2062 7920 5465  e provided by Te
-0002dce0: 6c65 6772 616d 2e0a 2020 2020 2020 2020  legram..        
-0002dcf0: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
-0002dd00: 6c74 2c20 616c 6c20 6669 6c65 7320 6172  lt, all files ar
-0002dd10: 6520 646f 776e 6c6f 6164 6564 2069 6e20  e downloaded in 
-0002dd20: 7468 6520 2a64 6f77 6e6c 6f61 6473 2a20  the *downloads* 
-0002dd30: 666f 6c64 6572 2069 6e20 796f 7572 2077  folder in your w
-0002dd40: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
-0002dd50: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002dd60: 2020 596f 7520 6361 6e20 616c 736f 2073    You can also s
-0002dd70: 7065 6369 6679 2061 2070 6174 6820 666f  pecify a path fo
-0002dd80: 7220 646f 776e 6c6f 6164 696e 6720 6669  r downloading fi
-0002dd90: 6c65 7320 696e 2061 2063 7573 746f 6d20  les in a custom 
-0002dda0: 6c6f 6361 7469 6f6e 3a20 7061 7468 7320  location: paths 
-0002ddb0: 7468 6174 2065 6e64 2077 6974 6820 222f  that end with "/
-0002ddc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0002ddd0: 2020 6172 6520 636f 6e73 6964 6572 6564    are considered
-0002dde0: 2064 6972 6563 746f 7269 6573 2e20 416c   directories. Al
-0002ddf0: 6c20 6e6f 6e2d 6578 6973 7465 6e74 2066  l non-existent f
-0002de00: 6f6c 6465 7273 2077 696c 6c20 6265 2063  olders will be c
-0002de10: 7265 6174 6564 2061 7574 6f6d 6174 6963  reated automatic
-0002de20: 616c 6c79 2e0a 0a20 2020 2020 2020 2020  ally...         
-0002de30: 2020 2069 6e5f 6d65 6d6f 7279 2028 6060     in_memory (``
-0002de40: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-0002de50: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-0002de60: 2020 2020 2050 6173 7320 5472 7565 2074       Pass True t
-0002de70: 6f20 646f 776e 6c6f 6164 2074 6865 206d  o download the m
-0002de80: 6564 6961 2069 6e2d 6d65 6d6f 7279 2e0a  edia in-memory..
-0002de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002dea0: 4120 6269 6e61 7279 2066 696c 652d 6c69  A binary file-li
-0002deb0: 6b65 206f 626a 6563 7420 7769 7468 2069  ke object with i
-0002dec0: 7473 2061 7474 7269 6275 7465 2022 2e6e  ts attribute ".n
-0002ded0: 616d 6522 2073 6574 2077 696c 6c20 6265  ame" set will be
-0002dee0: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-0002def0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-0002df00: 6c74 7320 746f 2046 616c 7365 2e0a 0a20  lts to False... 
-0002df10: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
-0002df20: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-0002df30: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-0002df40: 2020 2020 2020 2020 2042 6c6f 636b 7320           Blocks 
-0002df50: 7468 6520 636f 6465 2065 7865 6375 7469  the code executi
-0002df60: 6f6e 2075 6e74 696c 2074 6865 2066 696c  on until the fil
-0002df70: 6520 6861 7320 6265 656e 2064 6f77 6e6c  e has been downl
-0002df80: 6f61 6465 642e 0a20 2020 2020 2020 2020  oaded..         
-0002df90: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-0002dfa0: 746f 2054 7275 652e 0a0a 2020 2020 2020  to True...      
-0002dfb0: 2020 2020 2020 7072 6f67 7265 7373 2028        progress (
-0002dfc0: 6060 4361 6c6c 6162 6c65 6060 2c20 2a6f  ``Callable``, *o
-0002dfd0: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-0002dfe0: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-0002dff0: 6120 6361 6c6c 6261 636b 2066 756e 6374  a callback funct
-0002e000: 696f 6e20 746f 2076 6965 7720 7468 6520  ion to view the 
-0002e010: 6669 6c65 2074 7261 6e73 6d69 7373 696f  file transmissio
-0002e020: 6e20 7072 6f67 7265 7373 2e0a 2020 2020  n progress..    
-0002e030: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0002e040: 6675 6e63 7469 6f6e 206d 7573 7420 7461  function must ta
-0002e050: 6b65 202a 2863 7572 7265 6e74 2c20 746f  ke *(current, to
-0002e060: 7461 6c29 2a20 6173 2070 6f73 6974 696f  tal)* as positio
-0002e070: 6e61 6c20 6172 6775 6d65 6e74 7320 286c  nal arguments (l
-0002e080: 6f6f 6b20 6174 204f 7468 6572 2050 6172  ook at Other Par
-0002e090: 616d 6574 6572 7320 6265 6c6f 7720 666f  ameters below fo
-0002e0a0: 7220 610a 2020 2020 2020 2020 2020 2020  r a.            
-0002e0b0: 2020 2020 6465 7461 696c 6564 2064 6573      detailed des
-0002e0c0: 6372 6970 7469 6f6e 2920 616e 6420 7769  cription) and wi
-0002e0d0: 6c6c 2062 6520 6361 6c6c 6564 2062 6163  ll be called bac
-0002e0e0: 6b20 6561 6368 2074 696d 6520 6120 6e65  k each time a ne
-0002e0f0: 7720 6669 6c65 2063 6875 6e6b 2068 6173  w file chunk has
-0002e100: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
-0002e110: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-0002e120: 2020 2074 7261 6e73 6d69 7474 6564 2e0a     transmitted..
-0002e130: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0002e140: 6772 6573 735f 6172 6773 2028 6060 7475  gress_args (``tu
-0002e150: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
-0002e160: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-0002e170: 2020 2020 4578 7472 6120 6375 7374 6f6d      Extra custom
-0002e180: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-0002e190: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
-0002e1a0: 6261 636b 2066 756e 6374 696f 6e2e 0a20  back function.. 
-0002e1b0: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
-0002e1c0: 6f75 2063 616e 2070 6173 7320 616e 7974  ou can pass anyt
-0002e1d0: 6869 6e67 2079 6f75 206e 6565 6420 746f  hing you need to
-0002e1e0: 2062 6520 6176 6169 6c61 626c 6520 696e   be available in
-0002e1f0: 2074 6865 2070 726f 6772 6573 7320 6361   the progress ca
-0002e200: 6c6c 6261 636b 2073 636f 7065 3b20 666f  llback scope; fo
-0002e210: 7220 6578 616d 706c 652c 2061 204d 6573  r example, a Mes
-0002e220: 7361 6765 0a20 2020 2020 2020 2020 2020  sage.           
-0002e230: 2020 2020 206f 626a 6563 7420 6f72 2061       object or a
-0002e240: 2043 6c69 656e 7420 696e 7374 616e 6365   Client instance
-0002e250: 2069 6e20 6f72 6465 7220 746f 2065 6469   in order to edi
-0002e260: 7420 7468 6520 6d65 7373 6167 6520 7769  t the message wi
-0002e270: 7468 2074 6865 2075 7064 6174 6564 2070  th the updated p
-0002e280: 726f 6772 6573 7320 7374 6174 7573 2e0a  rogress status..
-0002e290: 0a20 2020 2020 2020 204f 7468 6572 2050  .        Other P
-0002e2a0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-0002e2b0: 2020 2020 2020 2063 7572 7265 6e74 2028         current (
-0002e2c0: 6060 696e 7460 6029 3a0a 2020 2020 2020  ``int``):.      
-0002e2d0: 2020 2020 2020 2020 2020 5468 6520 616d            The am
-0002e2e0: 6f75 6e74 206f 6620 6279 7465 7320 7472  ount of bytes tr
-0002e2f0: 616e 736d 6974 7465 6420 736f 2066 6172  ansmitted so far
-0002e300: 2e0a 0a20 2020 2020 2020 2020 2020 2074  ...            t
-0002e310: 6f74 616c 2028 6060 696e 7460 6029 3a0a  otal (``int``):.
-0002e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e330: 5468 6520 746f 7461 6c20 7369 7a65 206f  The total size o
-0002e340: 6620 7468 6520 6669 6c65 2e0a 0a20 2020  f the file...   
-0002e350: 2020 2020 2020 2020 202a 6172 6773 2028           *args (
-0002e360: 6060 7475 706c 6560 602c 202a 6f70 7469  ``tuple``, *opti
-0002e370: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
-0002e380: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
-0002e390: 7374 6f6d 2061 7267 756d 656e 7473 2061  stom arguments a
-0002e3a0: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-0002e3b0: 2060 6070 726f 6772 6573 735f 6172 6773   ``progress_args
-0002e3c0: 6060 2070 6172 616d 6574 6572 2e0a 2020  `` parameter..  
-0002e3d0: 2020 2020 2020 2020 2020 2020 2020 596f                Yo
-0002e3e0: 7520 6361 6e20 6569 7468 6572 206b 6565  u can either kee
-0002e3f0: 7020 6060 2a61 7267 7360 6020 6f72 2061  p ``*args`` or a
-0002e400: 6464 2065 7665 7279 2073 696e 676c 6520  dd every single 
-0002e410: 6578 7472 6120 6172 6775 6d65 6e74 2069  extra argument i
-0002e420: 6e20 796f 7572 2066 756e 6374 696f 6e20  n your function 
-0002e430: 7369 676e 6174 7572 652e 0a0a 2020 2020  signature...    
-0002e440: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0002e450: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-0002e460: 6573 732c 2074 6865 2061 6273 6f6c 7574  ess, the absolut
-0002e470: 6520 7061 7468 206f 6620 7468 6520 646f  e path of the do
-0002e480: 776e 6c6f 6164 6564 2066 696c 6520 6173  wnloaded file as
-0002e490: 2073 7472 696e 6720 6973 2072 6574 7572   string is retur
-0002e4a0: 6e65 642c 204e 6f6e 6520 6f74 6865 7277  ned, None otherw
-0002e4b0: 6973 652e 0a0a 2020 2020 2020 2020 5261  ise...        Ra
-0002e4c0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-0002e4d0: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-0002e4e0: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-0002e4f0: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-0002e500: 2020 2020 2020 2020 2060 6056 616c 7565           ``Value
-0002e510: 4572 726f 7260 603a 2049 6620 7468 6520  Error``: If the 
-0002e520: 6d65 7373 6167 6520 646f 6573 6e27 7420  message doesn't 
-0002e530: 636f 6e74 6169 6e20 616e 7920 646f 776e  contain any down
-0002e540: 6c6f 6164 6162 6c65 206d 6564 6961 0a20  loadable media. 
-0002e550: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002e560: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0002e570: 7365 6c66 2e5f 636c 6965 6e74 2e64 6f77  self._client.dow
-0002e580: 6e6c 6f61 645f 6d65 6469 6128 0a20 2020  nload_media(.   
-0002e590: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0002e5a0: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
-0002e5b0: 2020 2066 696c 655f 6e61 6d65 3d66 696c     file_name=fil
-0002e5c0: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
-0002e5d0: 2020 2020 696e 5f6d 656d 6f72 793d 696e      in_memory=in
-0002e5e0: 5f6d 656d 6f72 792c 0a20 2020 2020 2020  _memory,.       
-0002e5f0: 2020 2020 2062 6c6f 636b 3d62 6c6f 636b       block=block
-0002e600: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
-0002e610: 6f67 7265 7373 3d70 726f 6772 6573 732c  ogress=progress,
-0002e620: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0002e630: 6772 6573 735f 6172 6773 3d70 726f 6772  gress_args=progr
-0002e640: 6573 735f 6172 6773 2c0a 2020 2020 2020  ess_args,.      
-0002e650: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-0002e660: 6566 2076 6f74 6528 0a20 2020 2020 2020  ef vote(.       
-0002e670: 2073 656c 662c 0a20 2020 2020 2020 206f   self,.        o
-0002e680: 7074 696f 6e3a 2069 6e74 2c0a 2020 2020  ption: int,.    
-0002e690: 2920 2d3e 2022 7479 7065 732e 506f 6c6c  ) -> "types.Poll
-0002e6a0: 223a 0a20 2020 2020 2020 2022 2222 426f  ":.        """Bo
-0002e6b0: 756e 6420 6d65 7468 6f64 202a 766f 7465  und method *vote
-0002e6c0: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-0002e6d0: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-0002e6e0: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-0002e6f0: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0002e700: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-0002e710: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002e720: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002e730: 2020 636c 6965 6e74 2e76 6f74 655f 706f    client.vote_po
-0002e740: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-0002e750: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-0002e760: 6167 652e 6368 6174 2e69 642c 0a20 2020  age.chat.id,.   
-0002e770: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-0002e780: 7361 6765 5f69 643d 6d65 7373 6167 652e  sage_id=message.
-0002e790: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002e7a0: 2020 2020 6f70 7469 6f6e 3d31 0a20 2020      option=1.   
-0002e7b0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0002e7c0: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-0002e7d0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
-0002e7e0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-0002e7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e800: 206d 6573 7361 6765 2e76 6f74 6528 3629   message.vote(6)
-0002e810: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0002e820: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-0002e830: 2020 6f70 7469 6f6e 2028 6060 696e 7460    option (``int`
-0002e840: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-0002e850: 2020 2020 496e 6465 7820 6f66 2074 6865      Index of the
-0002e860: 2070 6f6c 6c20 6f70 7469 6f6e 2079 6f75   poll option you
-0002e870: 2077 616e 7420 746f 2076 6f74 6520 666f   want to vote fo
-0002e880: 7220 2830 2074 6f20 3929 2e0a 0a20 2020  r (0 to 9)...   
-0002e890: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0002e8a0: 2020 2020 2020 2020 2020 3a6f 626a 3a60            :obj:`
-0002e8b0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
-0002e8c0: 506f 6c6c 603a 204f 6e20 7375 6363 6573  Poll`: On succes
-0002e8d0: 732c 2074 6865 2070 6f6c 6c20 7769 7468  s, the poll with
-0002e8e0: 2074 6865 2063 686f 7365 6e20 6f70 7469   the chosen opti
-0002e8f0: 6f6e 2069 7320 7265 7475 726e 6564 2e0a  on is returned..
-0002e900: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-0002e910: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
-0002e920: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
-0002e930: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
-0002e940: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
-0002e950: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0002e960: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-0002e970: 636c 6965 6e74 2e76 6f74 655f 706f 6c6c  client.vote_poll
-0002e980: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-0002e990: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
-0002e9a0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002e9b0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
-0002e9c0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0002e9d0: 6f70 7469 6f6e 733d 6f70 7469 6f6e 0a20  options=option. 
-0002e9e0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
-0002e9f0: 796e 6320 6465 6620 7069 6e28 7365 6c66  ync def pin(self
-0002ea00: 2c20 6469 7361 626c 655f 6e6f 7469 6669  , disable_notifi
-0002ea10: 6361 7469 6f6e 3a20 626f 6f6c 203d 2046  cation: bool = F
-0002ea20: 616c 7365 2c20 626f 7468 5f73 6964 6573  alse, both_sides
-0002ea30: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-0002ea40: 2d3e 2022 7479 7065 732e 4d65 7373 6167  -> "types.Messag
-0002ea50: 6522 3a0a 2020 2020 2020 2020 2222 2242  e":.        """B
-0002ea60: 6f75 6e64 206d 6574 686f 6420 2a70 696e  ound method *pin
-0002ea70: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-0002ea80: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-0002ea90: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-0002eaa0: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0002eab0: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-0002eac0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0002ead0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-0002eae0: 2020 6177 6169 7420 636c 6965 6e74 2e70    await client.p
-0002eaf0: 696e 5f63 6861 745f 6d65 7373 6167 6528  in_chat_message(
-0002eb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002eb10: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
-0002eb20: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
-0002eb30: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0002eb40: 655f 6964 3d6d 6573 7361 6765 5f69 640a  e_id=message_id.
-0002eb50: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0002eb60: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-0002eb70: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0002eb80: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0002eb90: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0002eba0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-0002ebb0: 652e 7069 6e28 290a 0a20 2020 2020 2020  e.pin()..       
-0002ebc0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-0002ebd0: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-0002ebe0: 5f6e 6f74 6966 6963 6174 696f 6e20 2860  _notification (`
-0002ebf0: 6062 6f6f 6c60 6029 3a0a 2020 2020 2020  `bool``):.      
-0002ec00: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
-0002ec10: 7275 652c 2069 6620 6974 2069 7320 6e6f  rue, if it is no
-0002ec20: 7420 6e65 6365 7373 6172 7920 746f 2073  t necessary to s
-0002ec30: 656e 6420 6120 6e6f 7469 6669 6361 7469  end a notificati
-0002ec40: 6f6e 2074 6f20 616c 6c20 6368 6174 206d  on to all chat m
-0002ec50: 656d 6265 7273 2061 626f 7574 2074 6865  embers about the
-0002ec60: 206e 6577 2070 696e 6e65 640a 2020 2020   new pinned.    
-0002ec70: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-0002ec80: 6167 652e 204e 6f74 6966 6963 6174 696f  age. Notificatio
-0002ec90: 6e73 2061 7265 2061 6c77 6179 7320 6469  ns are always di
-0002eca0: 7361 626c 6564 2069 6e20 6368 616e 6e65  sabled in channe
-0002ecb0: 6c73 2e0a 0a20 2020 2020 2020 2020 2020  ls...           
-0002ecc0: 2062 6f74 685f 7369 6465 7320 2860 6062   both_sides (``b
-0002ecd0: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
-0002ece0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-0002ecf0: 2020 2020 5061 7373 2054 7275 6520 746f      Pass True to
-0002ed00: 2070 696e 2074 6865 206d 6573 7361 6765   pin the message
-0002ed10: 2066 6f72 2062 6f74 6820 7369 6465 7320   for both sides 
-0002ed20: 2879 6f75 2061 6e64 2072 6563 6970 6965  (you and recipie
-0002ed30: 6e74 292e 0a20 2020 2020 2020 2020 2020  nt)..           
-0002ed40: 2020 2020 2041 7070 6c69 6361 626c 6520       Applicable 
-0002ed50: 746f 2070 7269 7661 7465 2063 6861 7473  to private chats
-0002ed60: 206f 6e6c 792e 2044 6566 6175 6c74 7320   only. Defaults 
-0002ed70: 746f 2046 616c 7365 2e0a 0a20 2020 2020  to False...     
-0002ed80: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0002ed90: 2020 2020 2020 2020 3a6f 626a 3a60 7e70          :obj:`~p
-0002eda0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-0002edb0: 7373 6167 6560 3a20 4f6e 2073 7563 6365  ssage`: On succe
-0002edc0: 7373 2c20 7468 6520 7365 7276 6963 6520  ss, the service 
-0002edd0: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
-0002ede0: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
-0002edf0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-0002ee00: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-0002ee10: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-0002ee20: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-0002ee30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002ee40: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0002ee50: 6c66 2e5f 636c 6965 6e74 2e70 696e 5f63  lf._client.pin_c
-0002ee60: 6861 745f 6d65 7373 6167 6528 0a20 2020  hat_message(.   
-0002ee70: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-0002ee80: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
-0002ee90: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0002eea0: 6765 5f69 643d 7365 6c66 2e69 642c 0a20  ge_id=self.id,. 
-0002eeb0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0002eec0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-0002eed0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-0002eee0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-0002eef0: 2020 626f 7468 5f73 6964 6573 3d62 6f74    both_sides=bot
-0002ef00: 685f 7369 6465 730a 2020 2020 2020 2020  h_sides.        
-0002ef10: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0002ef20: 2075 6e70 696e 2873 656c 6629 202d 3e20   unpin(self) -> 
-0002ef30: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0002ef40: 2242 6f75 6e64 206d 6574 686f 6420 2a75  "Bound method *u
-0002ef50: 6e70 696e 2a20 6f66 203a 6f62 6a3a 607e  npin* of :obj:`~
-0002ef60: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
-0002ef70: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
-0002ef80: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-0002ef90: 6375 7420 666f 723a 0a0a 2020 2020 2020  cut for:..      
-0002efa0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0002efb0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-0002efc0: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
-0002efd0: 6e74 2e75 6e70 696e 5f63 6861 745f 6d65  nt.unpin_chat_me
-0002efe0: 7373 6167 6528 0a20 2020 2020 2020 2020  ssage(.         
-0002eff0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-0002f000: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
-0002f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f020: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-0002f030: 6765 5f69 640a 2020 2020 2020 2020 2020  ge_id.          
-0002f040: 2020 290a 0a20 2020 2020 2020 2045 7861    )..        Exa
-0002f050: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-0002f060: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0002f070: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-0002f080: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-0002f090: 6d65 7373 6167 652e 756e 7069 6e28 290a  message.unpin().
-0002f0a0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0002f0b0: 3a0a 2020 2020 2020 2020 2020 2020 5472  :.            Tr
-0002f0c0: 7565 206f 6e20 7375 6363 6573 732e 0a0a  ue on success...
-0002f0d0: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-0002f0e0: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-0002f0f0: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-0002f100: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-0002f110: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
-0002f120: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0002f130: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-0002f140: 6965 6e74 2e75 6e70 696e 5f63 6861 745f  ient.unpin_chat_
-0002f150: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
-0002f160: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
-0002f170: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
-0002f180: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0002f190: 643d 7365 6c66 2e69 640a 2020 2020 2020  d=self.id.      
-0002f1a0: 2020 290a 0a20 2020 2023 2042 4547 494e    )..    # BEGIN
-0002f1b0: 3a20 7468 6520 6265 6c6f 7720 7072 6f70  : the below prop
-0002f1c0: 6572 7469 6573 2077 6572 6520 7265 6d6f  erties were remo
-0002f1d0: 7665 6420 696e 2060 424f 5420 4150 4920  ved in `BOT API 
-0002f1e0: 372e 3020 3c68 7474 7073 3a2f 2f63 6f72  7.0 <https://cor
-0002f1f0: 652e 7465 6c65 6772 616d 2e6f 7267 2f62  e.telegram.org/b
-0002f200: 6f74 732f 6170 692d 6368 616e 6765 6c6f  ots/api-changelo
-0002f210: 6723 6465 6365 6d62 6572 2d32 392d 3230  g#december-29-20
-0002f220: 3233 3e60 5f0a 0a20 2020 2040 7072 6f70  23>`_..    @prop
-0002f230: 6572 7479 0a20 2020 2064 6566 2066 6f72  erty.    def for
-0002f240: 7761 7264 5f66 726f 6d28 7365 6c66 2920  ward_from(self) 
-0002f250: 2d3e 2022 7479 7065 732e 5573 6572 223a  -> "types.User":
-0002f260: 0a20 2020 2020 2020 206c 6f67 2e77 6172  .        log.war
-0002f270: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-0002f280: 2020 2254 6869 7320 7072 6f70 6572 7479    "This property
-0002f290: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-0002f2a0: 220a 2020 2020 2020 2020 2020 2020 2250  ".            "P
-0002f2b0: 6c65 6173 6520 7573 6520 666f 7277 6172  lease use forwar
-0002f2c0: 645f 6f72 6967 696e 2069 6e73 7465 6164  d_origin instead
-0002f2d0: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-0002f2e0: 2020 2020 7265 7475 726e 2067 6574 6174      return getat
-0002f2f0: 7472 2873 656c 662e 666f 7277 6172 645f  tr(self.forward_
-0002f300: 6f72 6967 696e 2c20 2273 656e 6465 725f  origin, "sender_
-0002f310: 7573 6572 222c 204e 6f6e 6529 0a20 2020  user", None).   
-0002f320: 200a 2020 2020 4070 726f 7065 7274 790a   .    @property.
-0002f330: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002f340: 7365 6e64 6572 5f6e 616d 6528 7365 6c66  sender_name(self
-0002f350: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0002f360: 2020 6c6f 672e 7761 726e 696e 6728 0a20    log.warning(. 
-0002f370: 2020 2020 2020 2020 2020 2022 5468 6973             "This
-0002f380: 2070 726f 7065 7274 7920 6973 2064 6570   property is dep
-0002f390: 7265 6361 7465 642e 2022 0a20 2020 2020  recated. ".     
-0002f3a0: 2020 2020 2020 2022 506c 6561 7365 2075         "Please u
-0002f3b0: 7365 2066 6f72 7761 7264 5f6f 7269 6769  se forward_origi
-0002f3c0: 6e20 696e 7374 6561 6422 0a20 2020 2020  n instead".     
-0002f3d0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-0002f3e0: 7572 6e20 6765 7461 7474 7228 7365 6c66  urn getattr(self
-0002f3f0: 2e66 6f72 7761 7264 5f6f 7269 6769 6e2c  .forward_origin,
-0002f400: 2022 7365 6e64 6572 5f75 7365 725f 6e61   "sender_user_na
-0002f410: 6d65 222c 204e 6f6e 6529 0a0a 2020 2020  me", None)..    
-0002f420: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0002f430: 6620 666f 7277 6172 645f 6672 6f6d 5f63  f forward_from_c
-0002f440: 6861 7428 7365 6c66 2920 2d3e 2022 7479  hat(self) -> "ty
-0002f450: 7065 732e 4368 6174 223a 0a20 2020 2020  pes.Chat":.     
-0002f460: 2020 206c 6f67 2e77 6172 6e69 6e67 280a     log.warning(.
-0002f470: 2020 2020 2020 2020 2020 2020 2254 6869              "Thi
-0002f480: 7320 7072 6f70 6572 7479 2069 7320 6465  s property is de
-0002f490: 7072 6563 6174 6564 2e20 220a 2020 2020  precated. ".    
-0002f4a0: 2020 2020 2020 2020 2250 6c65 6173 6520          "Please 
-0002f4b0: 7573 6520 666f 7277 6172 645f 6f72 6967  use forward_orig
-0002f4c0: 696e 2069 6e73 7465 6164 220a 2020 2020  in instead".    
-0002f4d0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-0002f4e0: 7475 726e 2067 6574 6174 7472 280a 2020  turn getattr(.  
-0002f4f0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0002f500: 6f72 7761 7264 5f6f 7269 6769 6e2c 0a20  orward_origin,. 
-0002f510: 2020 2020 2020 2020 2020 2022 6368 6174             "chat
-0002f520: 222c 0a20 2020 2020 2020 2020 2020 2067  ",.            g
-0002f530: 6574 6174 7472 280a 2020 2020 2020 2020  etattr(.        
-0002f540: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-0002f550: 7761 7264 5f6f 7269 6769 6e2c 0a20 2020  ward_origin,.   
-0002f560: 2020 2020 2020 2020 2020 2020 2022 7365               "se
-0002f570: 6e64 6572 5f63 6861 7422 2c0a 2020 2020  nder_chat",.    
-0002f580: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-0002f590: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0002f5a0: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
-0002f5b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0002f5c0: 666f 7277 6172 645f 6672 6f6d 5f6d 6573  forward_from_mes
-0002f5d0: 7361 6765 5f69 6428 7365 6c66 2920 2d3e  sage_id(self) ->
-0002f5e0: 2069 6e74 3a0a 2020 2020 2020 2020 6c6f   int:.        lo
-0002f5f0: 672e 7761 726e 696e 6728 0a20 2020 2020  g.warning(.     
-0002f600: 2020 2020 2020 2022 5468 6973 2070 726f         "This pro
-0002f610: 7065 7274 7920 6973 2064 6570 7265 6361  perty is depreca
-0002f620: 7465 642e 2022 0a20 2020 2020 2020 2020  ted. ".         
-0002f630: 2020 2022 506c 6561 7365 2075 7365 2066     "Please use f
-0002f640: 6f72 7761 7264 5f6f 7269 6769 6e20 696e  orward_origin in
-0002f650: 7374 6561 6422 0a20 2020 2020 2020 2029  stead".        )
-0002f660: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002f670: 6765 7461 7474 7228 7365 6c66 2e66 6f72  getattr(self.for
-0002f680: 7761 7264 5f6f 7269 6769 6e2c 2022 6d65  ward_origin, "me
-0002f690: 7373 6167 655f 6964 222c 204e 6f6e 6529  ssage_id", None)
-0002f6a0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0002f6b0: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002f6c0: 7369 676e 6174 7572 6528 7365 6c66 2920  signature(self) 
-0002f6d0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0002f6e0: 6c6f 672e 7761 726e 696e 6728 0a20 2020  log.warning(.   
-0002f6f0: 2020 2020 2020 2020 2022 5468 6973 2070           "This p
-0002f700: 726f 7065 7274 7920 6973 2064 6570 7265  roperty is depre
-0002f710: 6361 7465 642e 2022 0a20 2020 2020 2020  cated. ".       
-0002f720: 2020 2020 2022 506c 6561 7365 2075 7365       "Please use
-0002f730: 2066 6f72 7761 7264 5f6f 7269 6769 6e20   forward_origin 
-0002f740: 696e 7374 6561 6422 0a20 2020 2020 2020  instead".       
-0002f750: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0002f760: 6e20 6765 7461 7474 7228 7365 6c66 2e66  n getattr(self.f
-0002f770: 6f72 7761 7264 5f6f 7269 6769 6e2c 2022  orward_origin, "
-0002f780: 6175 7468 6f72 5f73 6967 6e61 7475 7265  author_signature
-0002f790: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-0002f7a0: 200a 2020 2020 4070 726f 7065 7274 790a   .    @property.
-0002f7b0: 2020 2020 6465 6620 666f 7277 6172 645f      def forward_
-0002f7c0: 6461 7465 2873 656c 6629 202d 3e20 6461  date(self) -> da
-0002f7d0: 7465 7469 6d65 3a0a 2020 2020 2020 2020  tetime:.        
-0002f7e0: 6c6f 672e 7761 726e 696e 6728 0a20 2020  log.warning(.   
-0002f7f0: 2020 2020 2020 2020 2022 5468 6973 2070           "This p
-0002f800: 726f 7065 7274 7920 6973 2064 6570 7265  roperty is depre
-0002f810: 6361 7465 642e 2022 0a20 2020 2020 2020  cated. ".       
-0002f820: 2020 2020 2022 506c 6561 7365 2075 7365       "Please use
-0002f830: 2066 6f72 7761 7264 5f6f 7269 6769 6e20   forward_origin 
-0002f840: 696e 7374 6561 6422 0a20 2020 2020 2020  instead".       
-0002f850: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0002f860: 6e20 6765 7461 7474 7228 7365 6c66 2e66  n getattr(self.f
-0002f870: 6f72 7761 7264 5f6f 7269 6769 6e2c 2022  orward_origin, "
-0002f880: 6461 7465 222c 204e 6f6e 6529 0a0a 2020  date", None)..  
-0002f890: 2020 2320 454e 443a 2074 6865 2062 656c    # END: the bel
-0002f8a0: 6f77 2070 726f 7065 7274 6965 7320 7765  ow properties we
-0002f8b0: 7265 2072 656d 6f76 6564 2069 6e20 6042  re removed in `B
-0002f8c0: 4f54 2041 5049 2037 2e30 203c 6874 7470  OT API 7.0 <http
-0002f8d0: 733a 2f2f 636f 7265 2e74 656c 6567 7261  s://core.telegra
-0002f8e0: 6d2e 6f72 672f 626f 7473 2f61 7069 2d63  m.org/bots/api-c
-0002f8f0: 6861 6e67 656c 6f67 2364 6563 656d 6265  hangelog#decembe
-0002f900: 722d 3239 2d32 3032 333e 605f 0a         r-29-2023>`_.
+0002c920: 2077 7269 7465 5f61 6c6c 6f77 6564 3d72   write_allowed=r
+0002c930: 6571 7565 7374 5f77 7269 7465 5f61 6363  equest_write_acc
+0002c940: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
+0002c950: 2020 2020 2020 2020 2020 2020 2070 6565               pee
+0002c960: 723d 7269 6565 702c 0a20 2020 2020 2020  r=rieep,.       
+0002c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c980: 206d 7367 5f69 643d 7365 6c66 2e69 642c   msg_id=self.id,
+0002c990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c9a0: 2020 2020 2020 2020 2062 7574 746f 6e5f           button_
+0002c9b0: 6964 3d74 6c75 2e62 7574 746f 6e5f 6964  id=tlu.button_id
+0002c9c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c9d0: 2020 2020 2020 2020 2020 7572 6c3d 746c            url=tl
+0002c9e0: 752e 7572 6c0a 2020 2020 2020 2020 2020  u.url.          
+0002c9f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0002ca00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0002ca10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0002ca20: 7475 726e 2074 6975 646b 6f2e 7572 6c0a  turn tiudko.url.
+0002ca30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0002ca40: 2062 7574 746f 6e2e 7765 625f 6170 703a   button.web_app:
+0002ca50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ca60: 2074 6c75 203d 2062 7574 746f 6e2e 7765   tlu = button.we
+0002ca70: 625f 6170 700a 2020 2020 2020 2020 2020  b_app.          
+0002ca80: 2020 2020 2020 7768 6963 6862 6f74 6368        whichbotch
+0002ca90: 6174 203d 2028 0a20 2020 2020 2020 2020  at = (.         
+0002caa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002cab0: 7669 615f 626f 7420 616e 640a 2020 2020  via_bot and.    
+0002cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cad0: 7365 6c66 2e76 6961 5f62 6f74 2e69 640a  self.via_bot.id.
+0002cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002caf0: 2920 6f72 2028 0a20 2020 2020 2020 2020  ) or (.         
+0002cb00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002cb10: 6672 6f6d 5f75 7365 7220 616e 640a 2020  from_user and.  
+0002cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cb30: 2020 7365 6c66 2e66 726f 6d5f 7573 6572    self.from_user
+0002cb40: 2e69 735f 626f 7420 616e 640a 2020 2020  .is_bot and.    
+0002cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cb60: 7365 6c66 2e66 726f 6d5f 7573 6572 2e69  self.from_user.i
+0002cb70: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0002cb80: 2020 2920 6f72 204e 6f6e 650a 2020 2020    ) or None.    
+0002cb90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0002cba0: 6f74 2077 6869 6368 626f 7463 6861 743a  ot whichbotchat:
+0002cbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cbc0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0002cbd0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0002cbe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0002cbf0: 496e 7661 6c69 6420 4368 6174 426f 7454  Invalid ChatBotT
+0002cc00: 7970 6522 0a20 2020 2020 2020 2020 2020  ype".           
+0002cc10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0002cc20: 2020 2020 2020 2020 2020 2072 6965 6570             rieep
+0002cc30: 203d 2061 7761 6974 2073 656c 662e 5f63   = await self._c
+0002cc40: 6c69 656e 742e 7265 736f 6c76 655f 7065  lient.resolve_pe
+0002cc50: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+0002cc60: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+0002cc70: 742e 6964 0a20 2020 2020 2020 2020 2020  t.id.           
+0002cc80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0002cc90: 2020 2020 2020 2069 6565 7072 203d 2061         ieepr = a
+0002cca0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+0002ccb0: 742e 7265 736f 6c76 655f 7065 6572 280a  t.resolve_peer(.
+0002ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ccd0: 2020 2020 7768 6963 6862 6f74 6368 6174      whichbotchat
+0002cce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ccf0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0002cd00: 2020 206f 6b64 7569 7420 3d20 6177 6169     okduit = awai
+0002cd10: 7420 7365 6c66 2e5f 636c 6965 6e74 2e69  t self._client.i
+0002cd20: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
+0002cd30: 2020 2020 2020 2020 2020 2072 6177 2e66             raw.f
+0002cd40: 756e 6374 696f 6e73 2e6d 6573 7361 6765  unctions.message
+0002cd50: 732e 5265 7175 6573 7457 6562 5669 6577  s.RequestWebView
+0002cd60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002cd70: 2020 2020 2020 2020 2020 7065 6572 3d72            peer=r
+0002cd80: 6965 6570 2c0a 2020 2020 2020 2020 2020  ieep,.          
+0002cd90: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0002cda0: 743d 6965 6570 722c 0a20 2020 2020 2020  t=ieepr,.       
+0002cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cdc0: 2075 726c 3d74 6c75 2e75 726c 2c0a 2020   url=tlu.url,.  
+0002cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cde0: 2020 2020 2020 706c 6174 666f 726d 3d73        platform=s
+0002cdf0: 656c 662e 5f63 6c69 656e 742e 636c 6965  elf._client.clie
+0002ce00: 6e74 5f70 6c61 7466 6f72 6d2e 7661 6c75  nt_platform.valu
+0002ce10: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002ce20: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+0002ce30: 4f0a 2020 2020 2020 2020 2020 2020 2020  O.              
+0002ce40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002ce50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002ce60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002ce70: 206f 6b64 7569 742e 7572 6c0a 2020 2020   okduit.url.    
+0002ce80: 2020 2020 2020 2020 656c 6966 2062 7574          elif but
+0002ce90: 746f 6e2e 7573 6572 5f69 643a 0a20 2020  ton.user_id:.   
+0002cea0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0002ceb0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
+0002cec0: 636c 6965 6e74 2e67 6574 5f63 6861 7428  client.get_chat(
+0002ced0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cee0: 2020 2020 2062 7574 746f 6e2e 7573 6572       button.user
+0002cef0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0002cf00: 2020 2020 2020 2020 2046 616c 7365 0a20           False. 
+0002cf10: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0002cf20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0002cf30: 6620 6275 7474 6f6e 2e73 7769 7463 685f  f button.switch_
+0002cf40: 696e 6c69 6e65 5f71 7565 7279 3a0a 2020  inline_query:.  
+0002cf50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0002cf60: 7475 726e 2062 7574 746f 6e2e 7377 6974  turn button.swit
+0002cf70: 6368 5f69 6e6c 696e 655f 7175 6572 790a  ch_inline_query.
+0002cf80: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0002cf90: 2062 7574 746f 6e2e 7377 6974 6368 5f69   button.switch_i
+0002cfa0: 6e6c 696e 655f 7175 6572 795f 6375 7272  nline_query_curr
+0002cfb0: 656e 745f 6368 6174 3a0a 2020 2020 2020  ent_chat:.      
+0002cfc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002cfd0: 2062 7574 746f 6e2e 7377 6974 6368 5f69   button.switch_i
+0002cfe0: 6e6c 696e 655f 7175 6572 795f 6375 7272  nline_query_curr
+0002cff0: 656e 745f 6368 6174 0a20 2020 2020 2020  ent_chat.       
+0002d000: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
+0002d010: 2e73 7769 7463 685f 696e 6c69 6e65 5f71  .switch_inline_q
+0002d020: 7565 7279 5f63 686f 7365 6e5f 6368 6174  uery_chosen_chat
+0002d030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002d040: 2020 7265 7475 726e 2062 7574 746f 6e2e    return button.
+0002d050: 7377 6974 6368 5f69 6e6c 696e 655f 7175  switch_inline_qu
+0002d060: 6572 795f 6368 6f73 656e 5f63 6861 740a  ery_chosen_chat.
+0002d070: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0002d080: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002d090: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0002d0a0: 6f72 2822 5468 6973 2062 7574 746f 6e20  or("This button 
+0002d0b0: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+0002d0c0: 2079 6574 2229 0a20 2020 2020 2020 2065   yet").        e
+0002d0d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002d0e0: 2061 7761 6974 2073 656c 662e 7265 706c   await self.repl
+0002d0f0: 7928 7465 7874 3d62 7574 746f 6e2c 2071  y(text=button, q
+0002d100: 756f 7465 3d71 756f 7465 290a 0a20 2020  uote=quote)..   
+0002d110: 2061 7379 6e63 2064 6566 2072 6561 6374   async def react
+0002d120: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002d130: 2020 2020 2020 2020 7265 6163 7469 6f6e          reaction
+0002d140: 3a20 556e 696f 6e5b 0a20 2020 2020 2020  : Union[.       
+0002d150: 2020 2020 2069 6e74 2c0a 2020 2020 2020       int,.      
+0002d160: 2020 2020 2020 7374 722c 0a20 2020 2020        str,.     
+0002d170: 2020 2020 2020 204c 6973 745b 556e 696f         List[Unio
+0002d180: 6e5b 696e 742c 2073 7472 2c20 2274 7970  n[int, str, "typ
+0002d190: 6573 2e52 6561 6374 696f 6e54 7970 6522  es.ReactionType"
+0002d1a0: 5d5d 0a20 2020 2020 2020 205d 203d 204e  ]].        ] = N
+0002d1b0: 6f6e 652c 0a20 2020 2020 2020 2069 735f  one,.        is_
+0002d1c0: 6269 673a 2062 6f6f 6c20 3d20 4661 6c73  big: bool = Fals
+0002d1d0: 652c 0a20 2020 2020 2020 2061 6464 5f74  e,.        add_t
+0002d1e0: 6f5f 7265 6365 6e74 3a20 626f 6f6c 203d  o_recent: bool =
+0002d1f0: 2054 7275 650a 2020 2020 2920 2d3e 2022   True.    ) -> "
+0002d200: 7479 7065 732e 4d65 7373 6167 6552 6561  types.MessageRea
+0002d210: 6374 696f 6e73 223a 0a20 2020 2020 2020  ctions":.       
+0002d220: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
+0002d230: 202a 7265 6163 742a 206f 6620 3a6f 626a   *react* of :obj
+0002d240: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
+0002d250: 732e 4d65 7373 6167 6560 2e0a 0a20 2020  s.Message`...   
+0002d260: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
+0002d270: 6f72 7463 7574 2066 6f72 3a0a 0a20 2020  ortcut for:..   
+0002d280: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
+0002d290: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
+0002d2a0: 2020 2020 2020 2020 2061 7761 6974 2063           await c
+0002d2b0: 6c69 656e 742e 7365 745f 7265 6163 7469  lient.set_reacti
+0002d2c0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0002d2d0: 2020 2020 6368 6174 5f69 643d 6368 6174      chat_id=chat
+0002d2e0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0002d2f0: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+0002d300: 6d65 7373 6167 652e 6964 2c0a 2020 2020  message.id,.    
+0002d310: 2020 2020 2020 2020 2020 2020 7265 6163              reac
+0002d320: 7469 6f6e 3d5b 5265 6163 7469 6f6e 5479  tion=[ReactionTy
+0002d330: 7065 456d 6f6a 6928 656d 6f6a 693d 22f0  peEmoji(emoji=".
+0002d340: 9f91 8d22 295d 0a20 2020 2020 2020 2020  ...")].         
+0002d350: 2020 2029 0a0a 2020 2020 2020 2020 4578     )..        Ex
+0002d360: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+0002d370: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0002d380: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0002d390: 2020 2020 2020 2020 2020 2023 2053 656e             # Sen
+0002d3a0: 6420 6120 7265 6163 7469 6f6e 0a20 2020  d a reaction.   
+0002d3b0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0002d3c0: 6974 206d 6573 7361 6765 2e72 6561 6374  it message.react
+0002d3d0: 285b 5265 6163 7469 6f6e 5479 7065 456d  ([ReactionTypeEm
+0002d3e0: 6f6a 6928 656d 6f6a 693d 22f0 9f91 8d22  oji(emoji="...."
+0002d3f0: 295d 290a 0a20 2020 2020 2020 2020 2020  )])..           
+0002d400: 2020 2020 2023 2052 6574 7261 6374 2061       # Retract a
+0002d410: 2072 6561 6374 696f 6e0a 2020 2020 2020   reaction.      
+0002d420: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0002d430: 6d65 7373 6167 652e 7265 6163 7428 290a  message.react().
+0002d440: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0002d450: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0002d460: 2072 6561 6374 696f 6e20 2860 6069 6e74   reaction (``int
+0002d470: 6060 207c 2060 6073 7472 6060 207c 204c  `` | ``str`` | L
+0002d480: 6973 7420 6f66 2060 6069 6e74 6060 204f  ist of ``int`` O
+0002d490: 5220 6060 7374 7260 6020 7c20 4c69 7374  R ``str`` | List
+0002d4a0: 206f 6620 3a6f 626a 3a60 7e70 7972 6f67   of :obj:`~pyrog
+0002d4b0: 7261 6d2e 7479 7065 732e 5265 6163 7469  ram.types.Reacti
+0002d4c0: 6f6e 5479 7065 602c 202a 6f70 7469 6f6e  onType`, *option
+0002d4d0: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+0002d4e0: 2020 2020 2020 4e65 7720 6c69 7374 206f        New list o
+0002d4f0: 6620 7265 6163 7469 6f6e 2074 7970 6573  f reaction types
+0002d500: 2074 6f20 7365 7420 6f6e 2074 6865 206d   to set on the m
+0002d510: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
+0002d520: 2020 2020 2020 2020 5061 7373 204e 6f6e          Pass Non
+0002d530: 6520 6173 2065 6d6f 6a69 2028 6465 6661  e as emoji (defa
+0002d540: 756c 7429 2074 6f20 7265 7472 6163 7420  ult) to retract 
+0002d550: 7468 6520 7265 6163 7469 6f6e 2e0a 0a20  the reaction... 
+0002d560: 2020 2020 2020 2020 2020 2069 735f 6269             is_bi
+0002d570: 6720 2860 6062 6f6f 6c60 602c 202a 6f70  g (``bool``, *op
+0002d580: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+0002d590: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
+0002d5a0: 7275 6520 746f 2073 6574 2074 6865 2072  rue to set the r
+0002d5b0: 6561 6374 696f 6e20 7769 7468 2061 2062  eaction with a b
+0002d5c0: 6967 2061 6e69 6d61 7469 6f6e 2e0a 2020  ig animation..  
+0002d5d0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0002d5e0: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
+0002d5f0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+0002d600: 2020 2020 2020 2020 2020 6164 645f 746f            add_to
+0002d610: 5f72 6563 656e 7420 2860 6062 6f6f 6c60  _recent (``bool`
+0002d620: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+0002d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d640: 5061 7373 2054 7275 6520 6966 2074 6865  Pass True if the
+0002d650: 2072 6561 6374 696f 6e20 7368 6f75 6c64   reaction should
+0002d660: 2061 7070 6561 7220 696e 2074 6865 2072   appear in the r
+0002d670: 6563 656e 746c 7920 7573 6564 2072 6561  ecently used rea
+0002d680: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
+0002d690: 2020 2020 2020 2020 5468 6973 206f 7074          This opt
+0002d6a0: 696f 6e20 6973 2061 7070 6c69 6361 626c  ion is applicabl
+0002d6b0: 6520 6f6e 6c79 2066 6f72 2075 7365 7273  e only for users
+0002d6c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002d6d0: 2020 4465 6661 756c 7473 2074 6f20 5472    Defaults to Tr
+0002d6e0: 7565 2e0a 2020 2020 2020 2020 5265 7475  ue..        Retu
+0002d6f0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0002d700: 204f 6e20 7375 6363 6573 732c 203a 6f62   On success, :ob
+0002d710: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+0002d720: 6573 2e4d 6573 7361 6765 5265 6163 7469  es.MessageReacti
+0002d730: 6f6e 7360 3a20 6973 2072 6574 7572 6e65  ons`: is returne
+0002d740: 642e 0a0a 2020 2020 2020 2020 5261 6973  d...        Rais
+0002d750: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0002d760: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+0002d770: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+0002d780: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+0002d790: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0002d7a0: 7220 3d20 4e6f 6e65 0a0a 2020 2020 2020  r = None..      
+0002d7b0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0002d7c0: 7265 6163 7469 6f6e 2c20 4c69 7374 293a  reaction, List):
+0002d7d0: 0a20 2020 2020 2020 2020 2020 2073 7220  .            sr 
+0002d7e0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+0002d7f0: 2066 6f72 2069 2069 6e20 7265 6163 7469   for i in reacti
+0002d800: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+0002d810: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0002d820: 6528 692c 2074 7970 6573 2e52 6561 6374  e(i, types.React
+0002d830: 696f 6e54 7970 6529 3a0a 2020 2020 2020  ionType):.      
+0002d840: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+0002d850: 2e61 7070 656e 6428 6929 0a20 2020 2020  .append(i).     
+0002d860: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0002d870: 6973 696e 7374 616e 6365 2869 2c20 696e  isinstance(i, in
+0002d880: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0002d890: 2020 2020 2020 2020 7372 2e61 7070 656e          sr.appen
+0002d8a0: 6428 7479 7065 732e 5265 6163 7469 6f6e  d(types.Reaction
+0002d8b0: 5479 7065 4375 7374 6f6d 456d 6f6a 6928  TypeCustomEmoji(
+0002d8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d8d0: 2020 2020 2020 2020 2063 7573 746f 6d5f           custom_
+0002d8e0: 656d 6f6a 695f 6964 3d73 7472 2869 290a  emoji_id=str(i).
+0002d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d900: 2020 2020 2929 0a20 2020 2020 2020 2020      )).         
+0002d910: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0002d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d930: 2073 722e 6170 7065 6e64 2874 7970 6573   sr.append(types
+0002d940: 2e52 6561 6374 696f 6e54 7970 6545 6d6f  .ReactionTypeEmo
+0002d950: 6a69 280a 2020 2020 2020 2020 2020 2020  ji(.            
+0002d960: 2020 2020 2020 2020 2020 2020 656d 6f6a              emoj
+0002d970: 693d 690a 2020 2020 2020 2020 2020 2020  i=i.            
+0002d980: 2020 2020 2020 2020 2929 0a0a 2020 2020          ))..    
+0002d990: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0002d9a0: 6e63 6528 7265 6163 7469 6f6e 2c20 696e  nce(reaction, in
+0002d9b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0002d9c0: 7372 203d 205b 0a20 2020 2020 2020 2020  sr = [.         
+0002d9d0: 2020 2020 2020 2074 7970 6573 2e52 6561         types.Rea
+0002d9e0: 6374 696f 6e54 7970 6543 7573 746f 6d45  ctionTypeCustomE
+0002d9f0: 6d6f 6a69 280a 2020 2020 2020 2020 2020  moji(.          
+0002da00: 2020 2020 2020 2020 2020 6375 7374 6f6d            custom
+0002da10: 5f65 6d6f 6a69 5f69 643d 7374 7228 7265  _emoji_id=str(re
+0002da20: 6163 7469 6f6e 290a 2020 2020 2020 2020  action).        
+0002da30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002da40: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+0002da50: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0002da60: 2872 6561 6374 696f 6e2c 2073 7472 293a  (reaction, str):
+0002da70: 0a20 2020 2020 2020 2020 2020 2073 7220  .            sr 
+0002da80: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0002da90: 2020 2020 7479 7065 732e 5265 6163 7469      types.Reacti
+0002daa0: 6f6e 5479 7065 456d 6f6a 6928 0a20 2020  onTypeEmoji(.   
+0002dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dac0: 2065 6d6f 6a69 3d72 6561 6374 696f 6e0a   emoji=reaction.
+0002dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dae0: 290a 2020 2020 2020 2020 2020 2020 5d0a  ).            ].
+0002daf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002db00: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+0002db10: 6e74 2e73 6574 5f72 6561 6374 696f 6e28  nt.set_reaction(
+0002db20: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+0002db30: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+0002db40: 642c 0a20 2020 2020 2020 2020 2020 206d  d,.            m
+0002db50: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
+0002db60: 642c 0a20 2020 2020 2020 2020 2020 2072  d,.            r
+0002db70: 6561 6374 696f 6e3d 7372 2c0a 2020 2020  eaction=sr,.    
+0002db80: 2020 2020 2020 2020 6973 5f62 6967 3d69          is_big=i
+0002db90: 735f 6269 672c 0a20 2020 2020 2020 2020  s_big,.         
+0002dba0: 2020 2061 6464 5f74 6f5f 7265 6365 6e74     add_to_recent
+0002dbb0: 3d61 6464 5f74 6f5f 7265 6365 6e74 0a20  =add_to_recent. 
+0002dbc0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
+0002dbd0: 796e 6320 6465 6620 7265 7472 6163 745f  ync def retract_
+0002dbe0: 766f 7465 280a 2020 2020 2020 2020 7365  vote(.        se
+0002dbf0: 6c66 2c0a 2020 2020 2920 2d3e 2022 7479  lf,.    ) -> "ty
+0002dc00: 7065 732e 506f 6c6c 223a 0a20 2020 2020  pes.Poll":.     
+0002dc10: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0002dc20: 6f64 202a 7265 7472 6163 745f 766f 7465  od *retract_vote
+0002dc30: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
+0002dc40: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
+0002dc50: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
+0002dc60: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
+0002dc70: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
+0002dc80: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+0002dc90: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+0002dca0: 2020 636c 6965 6e74 2e72 6574 7261 6374    client.retract
+0002dcb0: 5f76 6f74 6528 0a20 2020 2020 2020 2020  _vote(.         
+0002dcc0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
+0002dcd0: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
+0002dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002dcf0: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
+0002dd00: 6765 5f69 642c 0a20 2020 2020 2020 2020  ge_id,.         
+0002dd10: 2020 2029 0a0a 2020 2020 2020 2020 4578     )..        Ex
+0002dd20: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
+0002dd30: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0002dd40: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0002dd50: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+0002dd60: 6765 2e72 6574 7261 6374 5f76 6f74 6528  ge.retract_vote(
+0002dd70: 290a 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
+0002dd80: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0002dd90: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+0002dda0: 7479 7065 732e 506f 6c6c 603a 204f 6e20  types.Poll`: On 
+0002ddb0: 7375 6363 6573 732c 2074 6865 2070 6f6c  success, the pol
+0002ddc0: 6c20 7769 7468 2074 6865 2072 6574 7261  l with the retra
+0002ddd0: 6374 6564 2076 6f74 6520 6973 2072 6574  cted vote is ret
+0002dde0: 7572 6e65 642e 0a0a 2020 2020 2020 2020  urned...        
+0002ddf0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0002de00: 2020 2020 5250 4345 7272 6f72 3a20 496e      RPCError: In
+0002de10: 2063 6173 6520 6f66 2061 2054 656c 6567   case of a Teleg
+0002de20: 7261 6d20 5250 4320 6572 726f 722e 0a20  ram RPC error.. 
+0002de30: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0002de40: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0002de50: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
+0002de60: 7472 6163 745f 766f 7465 280a 2020 2020  tract_vote(.    
+0002de70: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+0002de80: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
+0002de90: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+0002dea0: 655f 6964 3d73 656c 662e 6964 0a20 2020  e_id=self.id.   
+0002deb0: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
+0002dec0: 6320 6465 6620 646f 776e 6c6f 6164 280a  c def download(.
+0002ded0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002dee0: 2020 2020 2020 6669 6c65 5f6e 616d 653a        file_name:
+0002def0: 2073 7472 203d 2022 222c 0a20 2020 2020   str = "",.     
+0002df00: 2020 2069 6e5f 6d65 6d6f 7279 3a20 626f     in_memory: bo
+0002df10: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0002df20: 2020 2020 626c 6f63 6b3a 2062 6f6f 6c20      block: bool 
+0002df30: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+0002df40: 7072 6f67 7265 7373 3a20 4361 6c6c 6162  progress: Callab
+0002df50: 6c65 203d 204e 6f6e 652c 0a20 2020 2020  le = None,.     
+0002df60: 2020 2070 726f 6772 6573 735f 6172 6773     progress_args
+0002df70: 3a20 7475 706c 6520 3d20 2829 0a20 2020  : tuple = ().   
+0002df80: 2029 202d 3e20 7374 723a 0a20 2020 2020   ) -> str:.     
+0002df90: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0002dfa0: 6f64 202a 646f 776e 6c6f 6164 2a20 6f66  od *download* of
+0002dfb0: 203a 6f62 6a3a 607e 7079 726f 6772 616d   :obj:`~pyrogram
+0002dfc0: 2e74 7970 6573 2e4d 6573 7361 6765 602e  .types.Message`.
+0002dfd0: 0a0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
+0002dfe0: 2061 2073 686f 7274 6375 7420 666f 723a   a shortcut for:
+0002dff0: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+0002e000: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0002e010: 0a0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+0002e020: 6169 7420 636c 6965 6e74 2e64 6f77 6e6c  ait client.downl
+0002e030: 6f61 645f 6d65 6469 6128 6d65 7373 6167  oad_media(messag
+0002e040: 6529 0a0a 2020 2020 2020 2020 4578 616d  e)..        Exam
+0002e050: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+0002e060: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0002e070: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0002e080: 2020 2020 2020 2020 2061 7761 6974 206d           await m
+0002e090: 6573 7361 6765 2e64 6f77 6e6c 6f61 6428  essage.download(
+0002e0a0: 290a 0a20 2020 2020 2020 2050 6172 616d  )..        Param
+0002e0b0: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+0002e0c0: 2020 2066 696c 655f 6e61 6d65 2028 6060     file_name (``
+0002e0d0: 7374 7260 602c 202a 6f70 7469 6f6e 616c  str``, *optional
+0002e0e0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
+0002e0f0: 2020 2020 4120 6375 7374 6f6d 202a 6669      A custom *fi
+0002e100: 6c65 5f6e 616d 652a 2074 6f20 6265 2075  le_name* to be u
+0002e110: 7365 6420 696e 7374 6561 6420 6f66 2074  sed instead of t
+0002e120: 6865 206f 6e65 2070 726f 7669 6465 6420  he one provided 
+0002e130: 6279 2054 656c 6567 7261 6d2e 0a20 2020  by Telegram..   
+0002e140: 2020 2020 2020 2020 2020 2020 2042 7920               By 
+0002e150: 6465 6661 756c 742c 2061 6c6c 2066 696c  default, all fil
+0002e160: 6573 2061 7265 2064 6f77 6e6c 6f61 6465  es are downloade
+0002e170: 6420 696e 2074 6865 202a 646f 776e 6c6f  d in the *downlo
+0002e180: 6164 732a 2066 6f6c 6465 7220 696e 2079  ads* folder in y
+0002e190: 6f75 7220 776f 726b 696e 6720 6469 7265  our working dire
+0002e1a0: 6374 6f72 792e 0a20 2020 2020 2020 2020  ctory..         
+0002e1b0: 2020 2020 2020 2059 6f75 2063 616e 2061         You can a
+0002e1c0: 6c73 6f20 7370 6563 6966 7920 6120 7061  lso specify a pa
+0002e1d0: 7468 2066 6f72 2064 6f77 6e6c 6f61 6469  th for downloadi
+0002e1e0: 6e67 2066 696c 6573 2069 6e20 6120 6375  ng files in a cu
+0002e1f0: 7374 6f6d 206c 6f63 6174 696f 6e3a 2070  stom location: p
+0002e200: 6174 6873 2074 6861 7420 656e 6420 7769  aths that end wi
+0002e210: 7468 2022 2f22 0a20 2020 2020 2020 2020  th "/".         
+0002e220: 2020 2020 2020 2061 7265 2063 6f6e 7369         are consi
+0002e230: 6465 7265 6420 6469 7265 6374 6f72 6965  dered directorie
+0002e240: 732e 2041 6c6c 206e 6f6e 2d65 7869 7374  s. All non-exist
+0002e250: 656e 7420 666f 6c64 6572 7320 7769 6c6c  ent folders will
+0002e260: 2062 6520 6372 6561 7465 6420 6175 746f   be created auto
+0002e270: 6d61 7469 6361 6c6c 792e 0a0a 2020 2020  matically...    
+0002e280: 2020 2020 2020 2020 696e 5f6d 656d 6f72          in_memor
+0002e290: 7920 2860 6062 6f6f 6c60 602c 202a 6f70  y (``bool``, *op
+0002e2a0: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+0002e2b0: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
+0002e2c0: 7275 6520 746f 2064 6f77 6e6c 6f61 6420  rue to download 
+0002e2d0: 7468 6520 6d65 6469 6120 696e 2d6d 656d  the media in-mem
+0002e2e0: 6f72 792e 0a20 2020 2020 2020 2020 2020  ory..           
+0002e2f0: 2020 2020 2041 2062 696e 6172 7920 6669       A binary fi
+0002e300: 6c65 2d6c 696b 6520 6f62 6a65 6374 2077  le-like object w
+0002e310: 6974 6820 6974 7320 6174 7472 6962 7574  ith its attribut
+0002e320: 6520 222e 6e61 6d65 2220 7365 7420 7769  e ".name" set wi
+0002e330: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0002e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e350: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
+0002e360: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+0002e370: 626c 6f63 6b20 2860 6062 6f6f 6c60 602c  block (``bool``,
+0002e380: 202a 6f70 7469 6f6e 616c 2a29 3a0a 2020   *optional*):.  
+0002e390: 2020 2020 2020 2020 2020 2020 2020 426c                Bl
+0002e3a0: 6f63 6b73 2074 6865 2063 6f64 6520 6578  ocks the code ex
+0002e3b0: 6563 7574 696f 6e20 756e 7469 6c20 7468  ecution until th
+0002e3c0: 6520 6669 6c65 2068 6173 2062 6565 6e20  e file has been 
+0002e3d0: 646f 776e 6c6f 6164 6564 2e0a 2020 2020  downloaded..    
+0002e3e0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0002e3f0: 756c 7473 2074 6f20 5472 7565 2e0a 0a20  ults to True... 
+0002e400: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+0002e410: 6573 7320 2860 6043 616c 6c61 626c 6560  ess (``Callable`
+0002e420: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+0002e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e440: 5061 7373 2061 2063 616c 6c62 6163 6b20  Pass a callback 
+0002e450: 6675 6e63 7469 6f6e 2074 6f20 7669 6577  function to view
+0002e460: 2074 6865 2066 696c 6520 7472 616e 736d   the file transm
+0002e470: 6973 7369 6f6e 2070 726f 6772 6573 732e  ission progress.
+0002e480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002e490: 2054 6865 2066 756e 6374 696f 6e20 6d75   The function mu
+0002e4a0: 7374 2074 616b 6520 2a28 6375 7272 656e  st take *(curren
+0002e4b0: 742c 2074 6f74 616c 292a 2061 7320 706f  t, total)* as po
+0002e4c0: 7369 7469 6f6e 616c 2061 7267 756d 656e  sitional argumen
+0002e4d0: 7473 2028 6c6f 6f6b 2061 7420 4f74 6865  ts (look at Othe
+0002e4e0: 7220 5061 7261 6d65 7465 7273 2062 656c  r Parameters bel
+0002e4f0: 6f77 2066 6f72 2061 0a20 2020 2020 2020  ow for a.       
+0002e500: 2020 2020 2020 2020 2064 6574 6169 6c65           detaile
+0002e510: 6420 6465 7363 7269 7074 696f 6e29 2061  d description) a
+0002e520: 6e64 2077 696c 6c20 6265 2063 616c 6c65  nd will be calle
+0002e530: 6420 6261 636b 2065 6163 6820 7469 6d65  d back each time
+0002e540: 2061 206e 6577 2066 696c 6520 6368 756e   a new file chun
+0002e550: 6b20 6861 7320 6265 656e 2073 7563 6365  k has been succe
+0002e560: 7373 6675 6c6c 790a 2020 2020 2020 2020  ssfully.        
+0002e570: 2020 2020 2020 2020 7472 616e 736d 6974          transmit
+0002e580: 7465 642e 0a0a 2020 2020 2020 2020 2020  ted...          
+0002e590: 2020 7072 6f67 7265 7373 5f61 7267 7320    progress_args 
+0002e5a0: 2860 6074 7570 6c65 6060 2c20 2a6f 7074  (``tuple``, *opt
+0002e5b0: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+0002e5c0: 2020 2020 2020 2020 2045 7874 7261 2063           Extra c
+0002e5d0: 7573 746f 6d20 6172 6775 6d65 6e74 7320  ustom arguments 
+0002e5e0: 666f 7220 7468 6520 7072 6f67 7265 7373  for the progress
+0002e5f0: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+0002e600: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0002e610: 2020 2020 596f 7520 6361 6e20 7061 7373      You can pass
+0002e620: 2061 6e79 7468 696e 6720 796f 7520 6e65   anything you ne
+0002e630: 6564 2074 6f20 6265 2061 7661 696c 6162  ed to be availab
+0002e640: 6c65 2069 6e20 7468 6520 7072 6f67 7265  le in the progre
+0002e650: 7373 2063 616c 6c62 6163 6b20 7363 6f70  ss callback scop
+0002e660: 653b 2066 6f72 2065 7861 6d70 6c65 2c20  e; for example, 
+0002e670: 6120 4d65 7373 6167 650a 2020 2020 2020  a Message.      
+0002e680: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+0002e690: 206f 7220 6120 436c 6965 6e74 2069 6e73   or a Client ins
+0002e6a0: 7461 6e63 6520 696e 206f 7264 6572 2074  tance in order t
+0002e6b0: 6f20 6564 6974 2074 6865 206d 6573 7361  o edit the messa
+0002e6c0: 6765 2077 6974 6820 7468 6520 7570 6461  ge with the upda
+0002e6d0: 7465 6420 7072 6f67 7265 7373 2073 7461  ted progress sta
+0002e6e0: 7475 732e 0a0a 2020 2020 2020 2020 4f74  tus...        Ot
+0002e6f0: 6865 7220 5061 7261 6d65 7465 7273 3a0a  her Parameters:.
+0002e700: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+0002e710: 656e 7420 2860 6069 6e74 6060 293a 0a20  ent (``int``):. 
+0002e720: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0002e730: 6865 2061 6d6f 756e 7420 6f66 2062 7974  he amount of byt
+0002e740: 6573 2074 7261 6e73 6d69 7474 6564 2073  es transmitted s
+0002e750: 6f20 6661 722e 0a0a 2020 2020 2020 2020  o far...        
+0002e760: 2020 2020 746f 7461 6c20 2860 6069 6e74      total (``int
+0002e770: 6060 293a 0a20 2020 2020 2020 2020 2020  ``):.           
+0002e780: 2020 2020 2054 6865 2074 6f74 616c 2073       The total s
+0002e790: 697a 6520 6f66 2074 6865 2066 696c 652e  ize of the file.
+0002e7a0: 0a0a 2020 2020 2020 2020 2020 2020 2a61  ..            *a
+0002e7b0: 7267 7320 2860 6074 7570 6c65 6060 2c20  rgs (``tuple``, 
+0002e7c0: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+0002e7d0: 2020 2020 2020 2020 2020 2020 2045 7874               Ext
+0002e7e0: 7261 2063 7573 746f 6d20 6172 6775 6d65  ra custom argume
+0002e7f0: 6e74 7320 6173 2064 6566 696e 6564 2069  nts as defined i
+0002e800: 6e20 7468 6520 6060 7072 6f67 7265 7373  n the ``progress
+0002e810: 5f61 7267 7360 6020 7061 7261 6d65 7465  _args`` paramete
+0002e820: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
+0002e830: 2020 2059 6f75 2063 616e 2065 6974 6865     You can eithe
+0002e840: 7220 6b65 6570 2060 602a 6172 6773 6060  r keep ``*args``
+0002e850: 206f 7220 6164 6420 6576 6572 7920 7369   or add every si
+0002e860: 6e67 6c65 2065 7874 7261 2061 7267 756d  ngle extra argum
+0002e870: 656e 7420 696e 2079 6f75 7220 6675 6e63  ent in your func
+0002e880: 7469 6f6e 2073 6967 6e61 7475 7265 2e0a  tion signature..
+0002e890: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0002e8a0: 3a0a 2020 2020 2020 2020 2020 2020 4f6e  :.            On
+0002e8b0: 2073 7563 6365 7373 2c20 7468 6520 6162   success, the ab
+0002e8c0: 736f 6c75 7465 2070 6174 6820 6f66 2074  solute path of t
+0002e8d0: 6865 2064 6f77 6e6c 6f61 6465 6420 6669  he downloaded fi
+0002e8e0: 6c65 2061 7320 7374 7269 6e67 2069 7320  le as string is 
+0002e8f0: 7265 7475 726e 6564 2c20 4e6f 6e65 206f  returned, None o
+0002e900: 7468 6572 7769 7365 2e0a 0a20 2020 2020  therwise...     
+0002e910: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+0002e920: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+0002e930: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+0002e940: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+0002e950: 2e0a 2020 2020 2020 2020 2020 2020 6060  ..            ``
+0002e960: 5661 6c75 6545 7272 6f72 6060 3a20 4966  ValueError``: If
+0002e970: 2074 6865 206d 6573 7361 6765 2064 6f65   the message doe
+0002e980: 736e 2774 2063 6f6e 7461 696e 2061 6e79  sn't contain any
+0002e990: 2064 6f77 6e6c 6f61 6461 626c 6520 6d65   downloadable me
+0002e9a0: 6469 610a 2020 2020 2020 2020 2222 220a  dia.        """.
+0002e9b0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0002e9c0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+0002e9d0: 742e 646f 776e 6c6f 6164 5f6d 6564 6961  t.download_media
+0002e9e0: 280a 2020 2020 2020 2020 2020 2020 6d65  (.            me
+0002e9f0: 7373 6167 653d 7365 6c66 2c0a 2020 2020  ssage=self,.    
+0002ea00: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
+0002ea10: 653d 6669 6c65 5f6e 616d 652c 0a20 2020  e=file_name,.   
+0002ea20: 2020 2020 2020 2020 2069 6e5f 6d65 6d6f           in_memo
+0002ea30: 7279 3d69 6e5f 6d65 6d6f 7279 2c0a 2020  ry=in_memory,.  
+0002ea40: 2020 2020 2020 2020 2020 626c 6f63 6b3d            block=
+0002ea50: 626c 6f63 6b2c 0a20 2020 2020 2020 2020  block,.         
+0002ea60: 2020 2070 726f 6772 6573 733d 7072 6f67     progress=prog
+0002ea70: 7265 7373 2c0a 2020 2020 2020 2020 2020  ress,.          
+0002ea80: 2020 7072 6f67 7265 7373 5f61 7267 733d    progress_args=
+0002ea90: 7072 6f67 7265 7373 5f61 7267 732c 0a20  progress_args,. 
+0002eaa0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
+0002eab0: 796e 6320 6465 6620 766f 7465 280a 2020  ync def vote(.  
+0002eac0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002ead0: 2020 2020 6f70 7469 6f6e 3a20 696e 742c      option: int,
+0002eae0: 0a20 2020 2029 202d 3e20 2274 7970 6573  .    ) -> "types
+0002eaf0: 2e50 6f6c 6c22 3a0a 2020 2020 2020 2020  .Poll":.        
+0002eb00: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
+0002eb10: 2a76 6f74 652a 206f 6620 3a6f 626a 3a60  *vote* of :obj:`
+0002eb20: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+0002eb30: 4d65 7373 6167 6560 2e0a 0a20 2020 2020  Message`...     
+0002eb40: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
+0002eb50: 7463 7574 2066 6f72 3a0a 0a20 2020 2020  tcut for:..     
+0002eb60: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0002eb70: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0002eb80: 2020 2020 2020 2063 6c69 656e 742e 766f         client.vo
+0002eb90: 7465 5f70 6f6c 6c28 0a20 2020 2020 2020  te_poll(.       
+0002eba0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+0002ebb0: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
+0002ebc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002ebd0: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
+0002ebe0: 7361 6765 2e69 642c 0a20 2020 2020 2020  sage.id,.       
+0002ebf0: 2020 2020 2020 2020 206f 7074 696f 6e3d           option=
+0002ec00: 310a 2020 2020 2020 2020 2020 2020 290a  1.            ).
+0002ec10: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+0002ec20: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
+0002ec30: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+0002ec40: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+0002ec50: 2020 2020 2020 6d65 7373 6167 652e 766f        message.vo
+0002ec60: 7465 2836 290a 0a20 2020 2020 2020 2050  te(6)..        P
+0002ec70: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+0002ec80: 2020 2020 2020 206f 7074 696f 6e20 2860         option (`
+0002ec90: 6069 6e74 6060 293a 0a20 2020 2020 2020  `int``):.       
+0002eca0: 2020 2020 2020 2020 2049 6e64 6578 206f           Index o
+0002ecb0: 6620 7468 6520 706f 6c6c 206f 7074 696f  f the poll optio
+0002ecc0: 6e20 796f 7520 7761 6e74 2074 6f20 766f  n you want to vo
+0002ecd0: 7465 2066 6f72 2028 3020 746f 2039 292e  te for (0 to 9).
+0002ece0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0002ecf0: 733a 0a20 2020 2020 2020 2020 2020 203a  s:.            :
+0002ed00: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
+0002ed10: 7970 6573 2e50 6f6c 6c60 3a20 4f6e 2073  ypes.Poll`: On s
+0002ed20: 7563 6365 7373 2c20 7468 6520 706f 6c6c  uccess, the poll
+0002ed30: 2077 6974 6820 7468 6520 6368 6f73 656e   with the chosen
+0002ed40: 206f 7074 696f 6e20 6973 2072 6574 7572   option is retur
+0002ed50: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
+0002ed60: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+0002ed70: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
+0002ed80: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
+0002ed90: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
+0002eda0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0002edb0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+0002edc0: 656c 662e 5f63 6c69 656e 742e 766f 7465  elf._client.vote
+0002edd0: 5f70 6f6c 6c28 0a20 2020 2020 2020 2020  _poll(.         
+0002ede0: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
+0002edf0: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
+0002ee00: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+0002ee10: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
+0002ee20: 2020 2020 206f 7074 696f 6e73 3d6f 7074       options=opt
+0002ee30: 696f 6e0a 2020 2020 2020 2020 290a 0a20  ion.        ).. 
+0002ee40: 2020 2061 7379 6e63 2064 6566 2070 696e     async def pin
+0002ee50: 2873 656c 662c 2064 6973 6162 6c65 5f6e  (self, disable_n
+0002ee60: 6f74 6966 6963 6174 696f 6e3a 2062 6f6f  otification: boo
+0002ee70: 6c20 3d20 4661 6c73 652c 2062 6f74 685f  l = False, both_
+0002ee80: 7369 6465 733a 2062 6f6f 6c20 3d20 4661  sides: bool = Fa
+0002ee90: 6c73 6529 202d 3e20 2274 7970 6573 2e4d  lse) -> "types.M
+0002eea0: 6573 7361 6765 223a 0a20 2020 2020 2020  essage":.       
+0002eeb0: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
+0002eec0: 202a 7069 6e2a 206f 6620 3a6f 626a 3a60   *pin* of :obj:`
+0002eed0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
+0002eee0: 4d65 7373 6167 6560 2e0a 0a20 2020 2020  Message`...     
+0002eef0: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
+0002ef00: 7463 7574 2066 6f72 3a0a 0a20 2020 2020  tcut for:..     
+0002ef10: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0002ef20: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0002ef30: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+0002ef40: 656e 742e 7069 6e5f 6368 6174 5f6d 6573  ent.pin_chat_mes
+0002ef50: 7361 6765 280a 2020 2020 2020 2020 2020  sage(.          
+0002ef60: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
+0002ef70: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
+0002ef80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002ef90: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
+0002efa0: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
+0002efb0: 2029 0a0a 2020 2020 2020 2020 4578 616d   )..        Exam
+0002efc0: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+0002efd0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0002efe0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+0002eff0: 2020 2020 2020 2020 2061 7761 6974 206d           await m
+0002f000: 6573 7361 6765 2e70 696e 2829 0a0a 2020  essage.pin()..  
+0002f010: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0002f020: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+0002f030: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+0002f040: 6f6e 2028 6060 626f 6f6c 6060 293a 0a20  on (``bool``):. 
+0002f050: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+0002f060: 6173 7320 5472 7565 2c20 6966 2069 7420  ass True, if it 
+0002f070: 6973 206e 6f74 206e 6563 6573 7361 7279  is not necessary
+0002f080: 2074 6f20 7365 6e64 2061 206e 6f74 6966   to send a notif
+0002f090: 6963 6174 696f 6e20 746f 2061 6c6c 2063  ication to all c
+0002f0a0: 6861 7420 6d65 6d62 6572 7320 6162 6f75  hat members abou
+0002f0b0: 7420 7468 6520 6e65 7720 7069 6e6e 6564  t the new pinned
+0002f0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002f0d0: 206d 6573 7361 6765 2e20 4e6f 7469 6669   message. Notifi
+0002f0e0: 6361 7469 6f6e 7320 6172 6520 616c 7761  cations are alwa
+0002f0f0: 7973 2064 6973 6162 6c65 6420 696e 2063  ys disabled in c
+0002f100: 6861 6e6e 656c 732e 0a0a 2020 2020 2020  hannels...      
+0002f110: 2020 2020 2020 626f 7468 5f73 6964 6573        both_sides
+0002f120: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+0002f130: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+0002f140: 2020 2020 2020 2020 2050 6173 7320 5472           Pass Tr
+0002f150: 7565 2074 6f20 7069 6e20 7468 6520 6d65  ue to pin the me
+0002f160: 7373 6167 6520 666f 7220 626f 7468 2073  ssage for both s
+0002f170: 6964 6573 2028 796f 7520 616e 6420 7265  ides (you and re
+0002f180: 6369 7069 656e 7429 2e0a 2020 2020 2020  cipient)..      
+0002f190: 2020 2020 2020 2020 2020 4170 706c 6963            Applic
+0002f1a0: 6162 6c65 2074 6f20 7072 6976 6174 6520  able to private 
+0002f1b0: 6368 6174 7320 6f6e 6c79 2e20 4465 6661  chats only. Defa
+0002f1c0: 756c 7473 2074 6f20 4661 6c73 652e 0a0a  ults to False...
+0002f1d0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0002f1e0: 0a20 2020 2020 2020 2020 2020 203a 6f62  .            :ob
+0002f1f0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+0002f200: 6573 2e4d 6573 7361 6765 603a 204f 6e20  es.Message`: On 
+0002f210: 7375 6363 6573 732c 2074 6865 2073 6572  success, the ser
+0002f220: 7669 6365 206d 6573 7361 6765 2069 7320  vice message is 
+0002f230: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
+0002f240: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+0002f250: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+0002f260: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+0002f270: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+0002f280: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0002f290: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0002f2a0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+0002f2b0: 7069 6e5f 6368 6174 5f6d 6573 7361 6765  pin_chat_message
+0002f2c0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
+0002f2d0: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
+0002f2e0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002f2f0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
+0002f300: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002f310: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+0002f320: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
+0002f330: 6966 6963 6174 696f 6e2c 0a20 2020 2020  ification,.     
+0002f340: 2020 2020 2020 2062 6f74 685f 7369 6465         both_side
+0002f350: 733d 626f 7468 5f73 6964 6573 0a20 2020  s=both_sides.   
+0002f360: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
+0002f370: 6320 6465 6620 756e 7069 6e28 7365 6c66  c def unpin(self
+0002f380: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0002f390: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0002f3a0: 6f64 202a 756e 7069 6e2a 206f 6620 3a6f  od *unpin* of :o
+0002f3b0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+0002f3c0: 7065 732e 4d65 7373 6167 6560 2e0a 0a20  pes.Message`... 
+0002f3d0: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+0002f3e0: 7368 6f72 7463 7574 2066 6f72 3a0a 0a20  shortcut for:.. 
+0002f3f0: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0002f400: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+0002f410: 2020 2020 2020 2020 2020 2061 7761 6974             await
+0002f420: 2063 6c69 656e 742e 756e 7069 6e5f 6368   client.unpin_ch
+0002f430: 6174 5f6d 6573 7361 6765 280a 2020 2020  at_message(.    
+0002f440: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+0002f450: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
+0002f460: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
+0002f470: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+0002f480: 6d65 7373 6167 655f 6964 0a20 2020 2020  message_id.     
+0002f490: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0002f4a0: 2020 4578 616d 706c 653a 0a20 2020 2020    Example:.     
+0002f4b0: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0002f4c0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+0002f4d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0002f4e0: 7761 6974 206d 6573 7361 6765 2e75 6e70  wait message.unp
+0002f4f0: 696e 2829 0a0a 2020 2020 2020 2020 5265  in()..        Re
+0002f500: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002f510: 2020 2054 7275 6520 6f6e 2073 7563 6365     True on succe
+0002f520: 7373 2e0a 0a20 2020 2020 2020 2052 6169  ss...        Rai
+0002f530: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+0002f540: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
+0002f550: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
+0002f560: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
+0002f570: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002f580: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+0002f590: 662e 5f63 6c69 656e 742e 756e 7069 6e5f  f._client.unpin_
+0002f5a0: 6368 6174 5f6d 6573 7361 6765 280a 2020  chat_message(.  
+0002f5b0: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+0002f5c0: 643d 7365 6c66 2e63 6861 742e 6964 2c0a  d=self.chat.id,.
+0002f5d0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+0002f5e0: 6167 655f 6964 3d73 656c 662e 6964 0a20  age_id=self.id. 
+0002f5f0: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+0002f600: 4245 4749 4e3a 2074 6865 2062 656c 6f77  BEGIN: the below
+0002f610: 2070 726f 7065 7274 6965 7320 7765 7265   properties were
+0002f620: 2072 656d 6f76 6564 2069 6e20 6042 4f54   removed in `BOT
+0002f630: 2041 5049 2037 2e30 203c 6874 7470 733a   API 7.0 <https:
+0002f640: 2f2f 636f 7265 2e74 656c 6567 7261 6d2e  //core.telegram.
+0002f650: 6f72 672f 626f 7473 2f61 7069 2d63 6861  org/bots/api-cha
+0002f660: 6e67 656c 6f67 2364 6563 656d 6265 722d  ngelog#december-
+0002f670: 3239 2d32 3032 333e 605f 0a0a 2020 2020  29-2023>`_..    
+0002f680: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0002f690: 6620 666f 7277 6172 645f 6672 6f6d 2873  f forward_from(s
+0002f6a0: 656c 6629 202d 3e20 2274 7970 6573 2e55  elf) -> "types.U
+0002f6b0: 7365 7222 3a0a 2020 2020 2020 2020 6c6f  ser":.        lo
+0002f6c0: 672e 7761 726e 696e 6728 0a20 2020 2020  g.warning(.     
+0002f6d0: 2020 2020 2020 2022 5468 6973 2070 726f         "This pro
+0002f6e0: 7065 7274 7920 6973 2064 6570 7265 6361  perty is depreca
+0002f6f0: 7465 642e 2022 0a20 2020 2020 2020 2020  ted. ".         
+0002f700: 2020 2022 506c 6561 7365 2075 7365 2066     "Please use f
+0002f710: 6f72 7761 7264 5f6f 7269 6769 6e20 696e  orward_origin in
+0002f720: 7374 6561 6422 0a20 2020 2020 2020 2029  stead".        )
+0002f730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002f740: 6765 7461 7474 7228 7365 6c66 2e66 6f72  getattr(self.for
+0002f750: 7761 7264 5f6f 7269 6769 6e2c 2022 7365  ward_origin, "se
+0002f760: 6e64 6572 5f75 7365 7222 2c20 4e6f 6e65  nder_user", None
+0002f770: 290a 2020 2020 0a20 2020 2040 7072 6f70  ).    .    @prop
+0002f780: 6572 7479 0a20 2020 2064 6566 2066 6f72  erty.    def for
+0002f790: 7761 7264 5f73 656e 6465 725f 6e61 6d65  ward_sender_name
+0002f7a0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+0002f7b0: 2020 2020 2020 206c 6f67 2e77 6172 6e69         log.warni
+0002f7c0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0002f7d0: 2254 6869 7320 7072 6f70 6572 7479 2069  "This property i
+0002f7e0: 7320 6465 7072 6563 6174 6564 2e20 220a  s deprecated. ".
+0002f7f0: 2020 2020 2020 2020 2020 2020 2250 6c65              "Ple
+0002f800: 6173 6520 7573 6520 666f 7277 6172 645f  ase use forward_
+0002f810: 6f72 6967 696e 2069 6e73 7465 6164 220a  origin instead".
+0002f820: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002f830: 2020 7265 7475 726e 2067 6574 6174 7472    return getattr
+0002f840: 2873 656c 662e 666f 7277 6172 645f 6f72  (self.forward_or
+0002f850: 6967 696e 2c20 2273 656e 6465 725f 7573  igin, "sender_us
+0002f860: 6572 5f6e 616d 6522 2c20 4e6f 6e65 290a  er_name", None).
+0002f870: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0002f880: 2020 2064 6566 2066 6f72 7761 7264 5f66     def forward_f
+0002f890: 726f 6d5f 6368 6174 2873 656c 6629 202d  rom_chat(self) -
+0002f8a0: 3e20 2274 7970 6573 2e43 6861 7422 3a0a  > "types.Chat":.
+0002f8b0: 2020 2020 2020 2020 6c6f 672e 7761 726e          log.warn
+0002f8c0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0002f8d0: 2022 5468 6973 2070 726f 7065 7274 7920   "This property 
+0002f8e0: 6973 2064 6570 7265 6361 7465 642e 2022  is deprecated. "
+0002f8f0: 0a20 2020 2020 2020 2020 2020 2022 506c  .            "Pl
+0002f900: 6561 7365 2075 7365 2066 6f72 7761 7264  ease use forward
+0002f910: 5f6f 7269 6769 6e20 696e 7374 6561 6422  _origin instead"
+0002f920: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002f930: 2020 2072 6574 7572 6e20 6765 7461 7474     return getatt
+0002f940: 7228 0a20 2020 2020 2020 2020 2020 2073  r(.            s
+0002f950: 656c 662e 666f 7277 6172 645f 6f72 6967  elf.forward_orig
+0002f960: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0002f970: 2263 6861 7422 2c0a 2020 2020 2020 2020  "chat",.        
+0002f980: 2020 2020 6765 7461 7474 7228 0a20 2020      getattr(.   
+0002f990: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0002f9a0: 662e 666f 7277 6172 645f 6f72 6967 696e  f.forward_origin
+0002f9b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002f9c0: 2020 2273 656e 6465 725f 6368 6174 222c    "sender_chat",
+0002f9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002f9e0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0002f9f0: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+0002fa00: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0002fa10: 2064 6566 2066 6f72 7761 7264 5f66 726f   def forward_fro
+0002fa20: 6d5f 6d65 7373 6167 655f 6964 2873 656c  m_message_id(sel
+0002fa30: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+0002fa40: 2020 206c 6f67 2e77 6172 6e69 6e67 280a     log.warning(.
+0002fa50: 2020 2020 2020 2020 2020 2020 2254 6869              "Thi
+0002fa60: 7320 7072 6f70 6572 7479 2069 7320 6465  s property is de
+0002fa70: 7072 6563 6174 6564 2e20 220a 2020 2020  precated. ".    
+0002fa80: 2020 2020 2020 2020 2250 6c65 6173 6520          "Please 
+0002fa90: 7573 6520 666f 7277 6172 645f 6f72 6967  use forward_orig
+0002faa0: 696e 2069 6e73 7465 6164 220a 2020 2020  in instead".    
+0002fab0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0002fac0: 7475 726e 2067 6574 6174 7472 2873 656c  turn getattr(sel
+0002fad0: 662e 666f 7277 6172 645f 6f72 6967 696e  f.forward_origin
+0002fae0: 2c20 226d 6573 7361 6765 5f69 6422 2c20  , "message_id", 
+0002faf0: 4e6f 6e65 290a 0a20 2020 2040 7072 6f70  None)..    @prop
+0002fb00: 6572 7479 0a20 2020 2064 6566 2066 6f72  erty.    def for
+0002fb10: 7761 7264 5f73 6967 6e61 7475 7265 2873  ward_signature(s
+0002fb20: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+0002fb30: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+0002fb40: 280a 2020 2020 2020 2020 2020 2020 2254  (.            "T
+0002fb50: 6869 7320 7072 6f70 6572 7479 2069 7320  his property is 
+0002fb60: 6465 7072 6563 6174 6564 2e20 220a 2020  deprecated. ".  
+0002fb70: 2020 2020 2020 2020 2020 2250 6c65 6173            "Pleas
+0002fb80: 6520 7573 6520 666f 7277 6172 645f 6f72  e use forward_or
+0002fb90: 6967 696e 2069 6e73 7465 6164 220a 2020  igin instead".  
+0002fba0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002fbb0: 7265 7475 726e 2067 6574 6174 7472 2873  return getattr(s
+0002fbc0: 656c 662e 666f 7277 6172 645f 6f72 6967  elf.forward_orig
+0002fbd0: 696e 2c20 2261 7574 686f 725f 7369 676e  in, "author_sign
+0002fbe0: 6174 7572 6522 2c20 4e6f 6e65 290a 2020  ature", None).  
+0002fbf0: 2020 2020 2020 0a20 2020 2040 7072 6f70        .    @prop
+0002fc00: 6572 7479 0a20 2020 2064 6566 2066 6f72  erty.    def for
+0002fc10: 7761 7264 5f64 6174 6528 7365 6c66 2920  ward_date(self) 
+0002fc20: 2d3e 2064 6174 6574 696d 653a 0a20 2020  -> datetime:.   
+0002fc30: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+0002fc40: 280a 2020 2020 2020 2020 2020 2020 2254  (.            "T
+0002fc50: 6869 7320 7072 6f70 6572 7479 2069 7320  his property is 
+0002fc60: 6465 7072 6563 6174 6564 2e20 220a 2020  deprecated. ".  
+0002fc70: 2020 2020 2020 2020 2020 2250 6c65 6173            "Pleas
+0002fc80: 6520 7573 6520 666f 7277 6172 645f 6f72  e use forward_or
+0002fc90: 6967 696e 2069 6e73 7465 6164 220a 2020  igin instead".  
+0002fca0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002fcb0: 7265 7475 726e 2067 6574 6174 7472 2873  return getattr(s
+0002fcc0: 656c 662e 666f 7277 6172 645f 6f72 6967  elf.forward_orig
+0002fcd0: 696e 2c20 2264 6174 6522 2c20 4e6f 6e65  in, "date", None
+0002fce0: 290a 0a20 2020 2023 2045 4e44 3a20 7468  )..    # END: th
+0002fcf0: 6520 6265 6c6f 7720 7072 6f70 6572 7469  e below properti
+0002fd00: 6573 2077 6572 6520 7265 6d6f 7665 6420  es were removed 
+0002fd10: 696e 2060 424f 5420 4150 4920 372e 3020  in `BOT API 7.0 
+0002fd20: 3c68 7474 7073 3a2f 2f63 6f72 652e 7465  <https://core.te
+0002fd30: 6c65 6772 616d 2e6f 7267 2f62 6f74 732f  legram.org/bots/
+0002fd40: 6170 692d 6368 616e 6765 6c6f 6723 6465  api-changelog#de
+0002fd50: 6365 6d62 6572 2d32 392d 3230 3233 3e60  cember-29-2023>`
+0002fd60: 5f0a 0a20 2020 2061 7379 6e63 2064 6566  _..    async def
+0002fd70: 2072 6561 6428 7365 6c66 2920 2d3e 2062   read(self) -> b
+0002fd80: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0002fd90: 426f 756e 6420 6d65 7468 6f64 202a 7265  Bound method *re
+0002fda0: 6164 2a20 6f66 203a 6f62 6a3a 607e 7079  ad* of :obj:`~py
+0002fdb0: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
+0002fdc0: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
+0002fdd0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+0002fde0: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
+0002fdf0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+0002fe00: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+0002fe10: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+0002fe20: 2e72 6561 645f 6368 6174 5f68 6973 746f  .read_chat_histo
+0002fe30: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+0002fe40: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
+0002fe50: 6167 652e 6368 6174 2e69 642c 0a20 2020  age.chat.id,.   
+0002fe60: 2020 2020 2020 2020 2020 2020 206d 6178               max
+0002fe70: 5f69 643d 6d65 7373 6167 655f 6964 0a20  _id=message_id. 
+0002fe80: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0002fe90: 2020 2020 2020 4578 616d 706c 653a 0a0a        Example:..
+0002fea0: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+0002feb0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+0002fec0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+0002fed0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+0002fee0: 652e 7265 6164 2829 0a0a 2020 2020 2020  e.read()..      
+0002fef0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0002ff00: 2020 2020 2020 2054 7275 6520 6f6e 2073         True on s
+0002ff10: 7563 6365 7373 2e0a 0a20 2020 2020 2020  uccess...       
+0002ff20: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+0002ff30: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+0002ff40: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+0002ff50: 6772 616d 2052 5043 2065 7272 6f72 2e0a  gram RPC error..
+0002ff60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0002ff70: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+0002ff80: 7420 7365 6c66 2e5f 636c 6965 6e74 2e72  t self._client.r
+0002ff90: 6561 645f 6368 6174 5f68 6973 746f 7279  ead_chat_history
+0002ffa0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
+0002ffb0: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
+0002ffc0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002ffd0: 6d61 785f 6964 3d73 656c 662e 6964 0a20  max_id=self.id. 
+0002ffe0: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
+0002fff0: 796e 6320 6465 6620 7669 6577 2873 656c  ync def view(sel
+00030000: 662c 2066 6f72 6365 5f72 6561 643a 2062  f, force_read: b
+00030010: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2062  ool = True) -> b
+00030020: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00030030: 426f 756e 6420 6d65 7468 6f64 202a 7669  Bound method *vi
+00030040: 6577 2a20 6f66 203a 6f62 6a3a 607e 7079  ew* of :obj:`~py
+00030050: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
+00030060: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
+00030070: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+00030080: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
+00030090: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000300a0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+000300b0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+000300c0: 2e76 6965 775f 6d65 7373 6167 6573 280a  .view_messages(.
+000300d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000300e0: 6368 6174 5f69 643d 6d65 7373 6167 652e  chat_id=message.
+000300f0: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
+00030100: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00030110: 5f69 6473 3d6d 6573 7361 6765 5f69 640a  _ids=message_id.
+00030120: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00030130: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+00030140: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+00030150: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00030160: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+00030170: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+00030180: 652e 7669 6577 2829 0a0a 2020 2020 2020  e.view()..      
+00030190: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+000301a0: 2020 2020 2020 2020 2020 666f 7263 655f            force_
+000301b0: 7265 6164 2028 6060 626f 6f6c 6060 2c20  read (``bool``, 
+000301c0: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+000301d0: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
+000301e0: 7320 5472 7565 2074 6f20 6d61 726b 2061  s True to mark a
+000301f0: 7320 7265 6164 2074 6865 2073 7065 6369  s read the speci
+00030200: 6669 6564 206d 6573 7361 6765 7320 616e  fied messages an
+00030210: 6420 616c 736f 2069 6e63 7265 6d65 6e74  d also increment
+00030220: 2074 6865 2076 6965 7720 636f 756e 7465   the view counte
+00030230: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
+00030240: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00030250: 2054 7275 6520 6f6e 2073 7563 6365 7373   True on success
+00030260: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00030270: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+00030280: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
+00030290: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
+000302a0: 5043 2065 7272 6f72 2e0a 0a20 2020 2020  PC error...     
+000302b0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+000302c0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+000302d0: 2e5f 636c 6965 6e74 2e76 6965 775f 6d65  ._client.view_me
+000302e0: 7373 6167 6573 280a 2020 2020 2020 2020  ssages(.        
+000302f0: 2020 2020 6368 6174 5f69 643d 7365 6c66      chat_id=self
+00030300: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
+00030310: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
+00030320: 733d 7365 6c66 2e69 642c 0a20 2020 2020  s=self.id,.     
+00030330: 2020 2020 2020 2066 6f72 6365 5f72 6561         force_rea
+00030340: 643d 666f 7263 655f 7265 6164 0a20 2020  d=force_read.   
+00030350: 2020 2020 2029 0a                             ).
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_entity.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     ) -> "MessageReactionUpdated":
         chat = None
         peer_id = utils.get_peer_id(update.peer)
         raw_peer_id = utils.get_raw_peer_id(update.peer)
         if peer_id > 0:
             chat = types.Chat._parse_user_chat(client, users[raw_peer_id])
         else:
-            chat = types.Chat._parse_chat_chat(client, chats[raw_peer_id])
+            chat = types.Chat._parse_chat(client, chats[raw_peer_id])
 
         return MessageReactionCountUpdated(
             client=client,
             chat=chat,
             message_id=update.msg_id,
             date=utils.timestamp_to_datetime(update.date),
             reactions=[
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     ) -> "MessageReactionUpdated":
         chat = None
         peer_id = utils.get_peer_id(update.peer)
         raw_peer_id = utils.get_raw_peer_id(update.peer)
         if peer_id > 0:
             chat = types.Chat._parse_user_chat(client, users[raw_peer_id])
         else:
-            chat = types.Chat._parse_chat_chat(client, chats[raw_peer_id])
+            chat = types.Chat._parse_chat(client, chats[raw_peer_id])
 
         user = None
         actor_chat = None
 
         raw_actor_peer_id = utils.get_raw_peer_id(update.actor)
         actor_peer_id = utils.get_peer_id(update.actor)
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/message_reactions.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/photo.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/poll_option.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/reaction.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/sticker.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/story.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/thumbnail.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/venue.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/video_note.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/voice.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_app_data.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/messages_and_media/web_page.py` & `pyrotgfork-2.1.31/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/__init__.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .chat_permissions import ChatPermissions
 from .chat_photo import ChatPhoto
 from .chat_privileges import ChatPrivileges
 from .chat_reactions import ChatReactions
 from .chat_shared import ChatShared
 from .dialog import Dialog
 from .emoji_status import EmojiStatus
+from .group_call_participant import GroupCallParticipant
 from .invite_link_importer import InviteLinkImporter
 from .restriction import Restriction
 from .user import User
 from .username import Username
 from .users_shared import UsersShared
 from .video_chat_ended import VideoChatEnded
 from .video_chat_participants_invited import VideoChatParticipantsInvited
@@ -59,14 +60,15 @@
     "ChatPermissions",
     "ChatPhoto",
     "ChatPrivileges",
     "ChatReactions",
     "ChatShared",
     "Dialog",
     "EmojiStatus",
+    "GroupCallParticipant",
     "InviteLinkImporter",
     "Restriction",
     "User",
     "Username",
     "UsersShared",
     "VideoChatEnded",
     "VideoChatParticipantsInvited",
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/birthdate.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_color.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_photo.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,51 +31,51 @@
 
         allow_custom_emoji (``bool``, *optional*):
             Whether custom emoji are allowed or not.
 
         reactions (List of :obj:`~pyrogram.types.Reaction`, *optional*):
             Reactions available.
         
-        limit (``int``, *optional*):
+        max_reaction_count (``int``, *optional*):
             Limit of the number of different unique reactions that can be added to a message, including already published ones. Can have values between 1 and 11. Defaults to 11, if not specified. Only applicable for :obj:`~pyrogram.enums.ChatType.CHANNEL`.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         all_are_enabled: Optional[bool] = None,
         allow_custom_emoji: Optional[bool] = None,
         reactions: Optional[List["types.Reaction"]] = None,
-        limit: int = 11,
+        max_reaction_count: int = 11,
     ):
         super().__init__(client)
 
         self.all_are_enabled = all_are_enabled
         self.allow_custom_emoji = allow_custom_emoji
         self.reactions = reactions
-        self.limit = limit
+        self.max_reaction_count = max_reaction_count
 
     @staticmethod
     def _parse(client, chat_reactions: "raw.base.ChatReactions", reactions_limit: int = 11) -> Optional["ChatReactions"]:
         if isinstance(chat_reactions, raw.types.ChatReactionsAll):
             return ChatReactions(
                 client=client,
                 all_are_enabled=True,
                 allow_custom_emoji=chat_reactions.allow_custom,
-                limit=reactions_limit
+                max_reaction_count=reactions_limit
             )
 
         if isinstance(chat_reactions, raw.types.ChatReactionsSome):
             return ChatReactions(
                 client=client,
                 reactions=[
                     types.ReactionType._parse(client, reaction)
                     for reaction in chat_reactions.reactions
                 ],
-                limit=reactions_limit
+                max_reaction_count=reactions_limit
             )
 
         if isinstance(chat_reactions, raw.types.ChatReactionsNone):
             return None
 
         return None
```

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/chat_shared.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/chat_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/dialog.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/emoji_status.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/restriction.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/user.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/username.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/users_shared.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/users_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_participants_invited.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrotgfork-2.1.31/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/.gitignore` & `pyrotgfork-2.1.31/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/COPYING` & `pyrotgfork-2.1.31/COPYING`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/COPYING.lesser` & `pyrotgfork-2.1.31/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/NOTICE` & `pyrotgfork-2.1.31/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/README.md` & `pyrotgfork-2.1.31/README.md`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/hatch_build.py` & `pyrotgfork-2.1.31/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.30/pyproject.toml` & `pyrotgfork-2.1.31/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
 # Used to call hatch_build.py
 [tool.hatch.build.hooks.custom]
 
 [project.urls]
 Homepage = "https://telegramplayground.github.io/pyrogram/releases/"
 Tracker = "https://github.com/TelegramPlayGround/Pyrogram/issues"
-Community = "https://t.me/PyroTGFork"
 Source = "https://github.com/TelegramPlayGround/Pyrogram"
 Documentation = "https://telegramplayground.github.io/pyrogram/"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
@@ -95,10 +94,10 @@
     "furo<=2023.9.10",
     "sphinx-autobuild<=2021.3.14",
     "sphinx-copybutton<=0.5.2",
     "pygments<=2.17.2"
 ]
 
 fast = [
-    "TgCrypto==1.2.5",
+    "PyTgCrypto==1.2.6",
     "uvloop>0.18.0,<=0.19.0"
 ]
```

### Comparing `pyrotgfork-2.1.30/PKG-INFO` & `pyrotgfork-2.1.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.3
 Name: pyrotgfork
-Version: 2.1.30
+Version: 2.1.31
 Summary: Fork of Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Homepage, https://telegramplayground.github.io/pyrogram/releases/
 Project-URL: Tracker, https://github.com/TelegramPlayGround/Pyrogram/issues
-Project-URL: Community, https://t.me/PyroTGFork
 Project-URL: Source, https://github.com/TelegramPlayGround/Pyrogram
 Project-URL: Documentation, https://telegramplayground.github.io/pyrogram/
 Author-email: SpEcHIDe <pyrogram@iamidiotareyoutoo.com>
 License-Expression: LGPL-3.0-or-later
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
@@ -48,15 +47,15 @@
 Provides-Extra: docs
 Requires-Dist: furo<=2023.9.10; extra == 'docs'
 Requires-Dist: pygments<=2.17.2; extra == 'docs'
 Requires-Dist: sphinx-autobuild<=2021.3.14; extra == 'docs'
 Requires-Dist: sphinx-copybutton<=0.5.2; extra == 'docs'
 Requires-Dist: sphinx<=7.2.6; extra == 'docs'
 Provides-Extra: fast
-Requires-Dist: tgcrypto==1.2.5; extra == 'fast'
+Requires-Dist: pytgcrypto==1.2.6; extra == 'fast'
 Requires-Dist: uvloop<=0.19.0,>0.18.0; extra == 'fast'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://github.com/pyrogram/pyrogram">
         <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="Pyrogram" width="128">
     </a>
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.30 Summary: Fork of
+Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.31 Summary: Fork of
 Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Homepage, https://
 telegramplayground.github.io/pyrogram/releases/ Project-URL: Tracker, https://
-github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Community, https://
-t.me/PyroTGFork Project-URL: Source, https://github.com/TelegramPlayGround/
-Pyrogram Project-URL: Documentation, https://telegramplayground.github.io/
-pyrogram/ Author-email: SpEcHIDe
+github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Source, https://
+github.com/TelegramPlayGround/Pyrogram Project-URL: Documentation, https://
+telegramplayground.github.io/pyrogram/ Author-email: SpEcHIDe
 iamidiotareyoutoo.com> License-Expression: LGPL-3.0-or-later License-File:
 COPYING License-File: COPYING.lesser License-File: NOTICE Keywords: telegram
 chat messenger mtproto api client library python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
@@ -29,15 +28,15 @@
 hatch<=1.7.0; extra == 'dev' Requires-Dist: keyring<=25.1.0; extra == 'dev'
 Requires-Dist: pytest-asyncio<=0.21.1; extra == 'dev' Requires-Dist: pytest-
 cov<=4.1.0; extra == 'dev' Requires-Dist: pytest<=7.4.3; extra == 'dev'
 Requires-Dist: twine<=4.0.2; extra == 'dev' Provides-Extra: docs Requires-Dist:
 furo<=2023.9.10; extra == 'docs' Requires-Dist: pygments<=2.17.2; extra ==
 'docs' Requires-Dist: sphinx-autobuild<=2021.3.14; extra == 'docs' Requires-
 Dist: sphinx-copybutton<=0.5.2; extra == 'docs' Requires-Dist: sphinx<=7.2.6;
-extra == 'docs' Provides-Extra: fast Requires-Dist: tgcrypto==1.2.5; extra ==
+extra == 'docs' Provides-Extra: fast Requires-Dist: pytgcrypto==1.2.6; extra ==
 'fast' Requires-Dist: uvloop<=0.19.0,>0.18.0; extra == 'fast' Description-
 Content-Type: text/markdown
                                   _[_P_y_r_o_g_r_a_m_]
                   TTeelleeggrraamm MMTTPPrroottoo AAPPII FFrraammeewwoorrkk ffoorr PPyytthhoonn
                _H_o_m_e_p_a_g_e_ â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n_ â¢ _R_e_l_e_a_s_e_s_ â¢ _N_e_w_s
 ## Pyrogram > Elegant, modern and asynchronous Telegram MTProto API framework
 in Python for users and bots ``` python from pyrogram import Client, filters
```

