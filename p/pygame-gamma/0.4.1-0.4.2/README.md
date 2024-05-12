# Comparing `tmp/pygame_gamma-0.4.1.tar.gz` & `tmp/pygame_gamma-0.4.2.tar.gz`

## Comparing `pygame_gamma-0.4.1.tar` & `pygame_gamma-0.4.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/0.example_renderable.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/1.example_entities_images_animations.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/10.example_particle_system.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/11.example_trauma_system.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/12.example_triggers.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/13.example_cutscene.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/14.example_inventory.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/15.example_world_images.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/16.example_crafting.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/2.example_cameras.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/3.example_map.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/4.example_menu.py
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/5.example_scenes_transitions.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/6.example_button.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/7.example_input_movement.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/8.example_text_system.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/9.example_emote_system.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/collect_the_coins.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/component_score.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/factory_coin.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/input_context_player.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/scene_game.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/scene_game_over.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/scene_info.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/scene_menu.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/system_coin.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/trigger_coin.py
--rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_0.png
--rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_1.png
--rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_2.png
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_3.png
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_4.png
--rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_5.png
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/images/player/player.png
--rw-r--r--   0        0        0  2219087 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/music/before_the_dawn.ogg
--rw-r--r--   0        0        0   915612 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/music/solace.ogg
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/collect_the_coins/sounds/coin.ogg
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/heart.png
--rw-r--r--   0        0        0    97117 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/light.png
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/x_n.png
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/x_y1.png
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/x_y2.png
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/layers/back.png
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/layers/foreground.png
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/layers/front.png
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/layers/middle.png
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_00.png
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_01.png
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_02.png
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_03.png
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_04.png
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_05.png
--rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_06.png
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_07.png
--rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_08.png
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_09.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_10.png
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_11.png
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_12.png
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_13.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_14.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_15.png
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_16.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_17.png
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_18.png
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_19.png
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_20.png
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_21.png
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_22.png
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/player/vita_23.png
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/textures/dirt.png
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/textures/grass.png
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/examples/images/textures/water.png
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/gamma.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_battle.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_camera.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_collider.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_crafting.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_emote.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_input.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_inventory.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_motion.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_particle_emitter.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_position.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_sprites.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_tags.py
--rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_text.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_trauma.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/components/component_triggers.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/colours.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/component.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/crafting_recipe.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/cutscene.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/entity.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/entity_factory.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/hitbox.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/hurtbox.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/map.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/particle.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/renderable.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/renderer.py
--rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/scene.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/sprite.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/system.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/tile.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/core/transition.py
--rwxr-xr-x   0        0        0     9592 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/fonts/munro.ttf
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/images/emote_box.png
--rw-r--r--   0        0        0    10731 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/images/gamma.png
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/images/tile_outline.png
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/input/controller.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/input/keyboard.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_entity.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_input.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_resource.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_scene.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_sound.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_system.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_tile.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/renderables/circle.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/renderables/image.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/renderables/rectangle.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/renderables/text.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_animation.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_battle.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_camera.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_collision.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_crafting.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_emote.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_image.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_input.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_inventory.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_particle.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_physics.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_text.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_trauma.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/systems/system_trigger.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_black.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyinleft.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyinright.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyoutleft.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyoutright.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_moveleft.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_moveright.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_none.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_wipeleft.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_wiperight.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/keyboard_layouts.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_action_listener.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_button.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_menu.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text_input.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text_menu_item.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/utils/utils.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/src/pygame-gamma/utils/utils_draw.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/LICENSE
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 pygame_gamma-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/0.example_renderable.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/1.example_entities_images_animations.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/10.example_particle_system.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/11.example_trauma_system.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/12.example_triggers.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/13.example_cutscene.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/14.example_inventory.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/15.example_world_images.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/16.example_crafting.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/2.example_cameras.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/3.example_map.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/4.example_menu.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/5.example_scenes_transitions.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/6.example_button.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/7.example_input_movement.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/8.example_text_system.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/9.example_emote_system.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/collect_the_coins.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/component_score.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/factory_coin.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/input_context_player.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/scene_game.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/scene_game_over.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/scene_info.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/scene_menu.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/system_coin.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/trigger_coin.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_0.png
+-rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_1.png
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_2.png
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_3.png
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_4.png
+-rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_5.png
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/images/player/player.png
+-rw-r--r--   0        0        0  2219087 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/music/before_the_dawn.ogg
+-rw-r--r--   0        0        0   915612 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/music/solace.ogg
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/collect_the_coins/sounds/coin.ogg
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/heart.png
+-rw-r--r--   0        0        0    97117 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/light.png
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/x_n.png
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/x_y1.png
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/x_y2.png
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/layers/back.png
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/layers/foreground.png
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/layers/front.png
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/layers/middle.png
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_00.png
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_01.png
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_02.png
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_03.png
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_04.png
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_05.png
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_06.png
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_07.png
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_08.png
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_09.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_10.png
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_11.png
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_12.png
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_13.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_14.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_15.png
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_16.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_17.png
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_18.png
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_19.png
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_20.png
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_21.png
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_22.png
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/player/vita_23.png
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/textures/dirt.png
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/textures/grass.png
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/examples/images/textures/water.png
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/gamma.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_battle.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_camera.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_collider.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_crafting.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_emote.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_input.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_inventory.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_motion.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_particle_emitter.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_position.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_sprites.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_tags.py
+-rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_text.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_trauma.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/components/component_triggers.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/colours.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/component.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/crafting_recipe.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/cutscene.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/entity.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/entity_factory.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/hitbox.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/hurtbox.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/map.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/particle.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/renderable.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/renderer.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/scene.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/sprite.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/system.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/tile.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/core/transition.py
+-rwxr-xr-x   0        0        0     9592 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/fonts/munro.ttf
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/images/emote_box.png
+-rw-r--r--   0        0        0    10731 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/images/gamma.png
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/images/tile_outline.png
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/input/controller.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/input/keyboard.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_entity.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_input.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_resource.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_scene.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_sound.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_system.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/managers/manager_tile.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/renderables/circle.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/renderables/image.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/renderables/rectangle.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/renderables/text.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_animation.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_battle.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_camera.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_collision.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_crafting.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_emote.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_image.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_input.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_inventory.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_particle.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_physics.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_text.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_trauma.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/systems/system_trigger.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_black.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_flyinleft.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_flyinright.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_flyoutleft.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_flyoutright.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_moveleft.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_moveright.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_none.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_wipeleft.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/transitions/transition_wiperight.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/keyboard_layouts.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_action_listener.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_button.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_menu.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_text.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_text_input.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/ui/ui_text_menu_item.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/utils/utils.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/src/gamma/utils/utils_draw.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 pygame_gamma-0.4.2/PKG-INFO
```

### Comparing `pygame_gamma-0.4.1/examples/0.example_renderable.py` & `pygame_gamma-0.4.2/examples/0.example_renderable.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/1.example_entities_images_animations.py` & `pygame_gamma-0.4.2/examples/1.example_entities_images_animations.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/10.example_particle_system.py` & `pygame_gamma-0.4.2/examples/10.example_particle_system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/11.example_trauma_system.py` & `pygame_gamma-0.4.2/examples/11.example_trauma_system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/12.example_triggers.py` & `pygame_gamma-0.4.2/examples/12.example_triggers.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/13.example_cutscene.py` & `pygame_gamma-0.4.2/examples/13.example_cutscene.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/14.example_inventory.py` & `pygame_gamma-0.4.2/examples/14.example_inventory.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/15.example_world_images.py` & `pygame_gamma-0.4.2/examples/15.example_world_images.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/16.example_crafting.py` & `pygame_gamma-0.4.2/examples/16.example_crafting.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/2.example_cameras.py` & `pygame_gamma-0.4.2/examples/2.example_cameras.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/3.example_map.py` & `pygame_gamma-0.4.2/examples/3.example_map.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/4.example_menu.py` & `pygame_gamma-0.4.2/examples/4.example_menu.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/5.example_scenes_transitions.py` & `pygame_gamma-0.4.2/examples/5.example_scenes_transitions.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/6.example_button.py` & `pygame_gamma-0.4.2/examples/6.example_button.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/7.example_input_movement.py` & `pygame_gamma-0.4.2/examples/7.example_input_movement.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/8.example_text_system.py` & `pygame_gamma-0.4.2/examples/8.example_text_system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/9.example_emote_system.py` & `pygame_gamma-0.4.2/examples/9.example_emote_system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/collect_the_coins.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/collect_the_coins.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/factory_coin.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/factory_coin.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/input_context_player.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/input_context_player.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/scene_game.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/scene_game.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/scene_game_over.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/scene_game_over.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/scene_info.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/scene_info.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/scene_menu.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/scene_menu.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/system_coin.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/system_coin.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/trigger_coin.py` & `pygame_gamma-0.4.2/examples/collect_the_coins/trigger_coin.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_0.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_0.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_1.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_1.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_2.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_2.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_3.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_3.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_4.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_4.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/coin/coin_5.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/coin/coin_5.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/images/player/player.png` & `pygame_gamma-0.4.2/examples/collect_the_coins/images/player/player.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/music/before_the_dawn.ogg` & `pygame_gamma-0.4.2/examples/collect_the_coins/music/before_the_dawn.ogg`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/music/solace.ogg` & `pygame_gamma-0.4.2/examples/collect_the_coins/music/solace.ogg`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/collect_the_coins/sounds/coin.ogg` & `pygame_gamma-0.4.2/examples/collect_the_coins/sounds/coin.ogg`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/heart.png` & `pygame_gamma-0.4.2/examples/images/heart.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/light.png` & `pygame_gamma-0.4.2/examples/images/light.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/x_n.png` & `pygame_gamma-0.4.2/examples/images/x_n.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/x_y1.png` & `pygame_gamma-0.4.2/examples/images/x_y1.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/x_y2.png` & `pygame_gamma-0.4.2/examples/images/x_y2.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/layers/back.png` & `pygame_gamma-0.4.2/examples/images/layers/back.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/layers/foreground.png` & `pygame_gamma-0.4.2/examples/images/layers/foreground.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/layers/front.png` & `pygame_gamma-0.4.2/examples/images/layers/front.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/layers/middle.png` & `pygame_gamma-0.4.2/examples/images/layers/middle.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_00.png` & `pygame_gamma-0.4.2/examples/images/player/vita_00.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_01.png` & `pygame_gamma-0.4.2/examples/images/player/vita_01.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_02.png` & `pygame_gamma-0.4.2/examples/images/player/vita_02.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_03.png` & `pygame_gamma-0.4.2/examples/images/player/vita_03.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_04.png` & `pygame_gamma-0.4.2/examples/images/player/vita_04.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_05.png` & `pygame_gamma-0.4.2/examples/images/player/vita_05.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_06.png` & `pygame_gamma-0.4.2/examples/images/player/vita_06.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_07.png` & `pygame_gamma-0.4.2/examples/images/player/vita_07.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_08.png` & `pygame_gamma-0.4.2/examples/images/player/vita_08.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_09.png` & `pygame_gamma-0.4.2/examples/images/player/vita_09.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/player/vita_11.png` & `pygame_gamma-0.4.2/examples/images/player/vita_11.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/textures/dirt.png` & `pygame_gamma-0.4.2/examples/images/textures/dirt.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/textures/grass.png` & `pygame_gamma-0.4.2/examples/images/textures/grass.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/examples/images/textures/water.png` & `pygame_gamma-0.4.2/examples/images/textures/water.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/__init__.py` & `pygame_gamma-0.4.2/src/gamma/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = 'Rik Cross'
 __license__ = 'MIT'
 
 from .gamma import *
 
 from .core.scene import *
```

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/gamma.py` & `pygame_gamma-0.4.2/src/gamma/gamma.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_battle.py` & `pygame_gamma-0.4.2/src/gamma/components/component_battle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_camera.py` & `pygame_gamma-0.4.2/src/gamma/components/component_camera.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_crafting.py` & `pygame_gamma-0.4.2/src/gamma/components/component_crafting.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_emote.py` & `pygame_gamma-0.4.2/src/gamma/components/component_emote.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_input.py` & `pygame_gamma-0.4.2/src/gamma/components/component_input.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_inventory.py` & `pygame_gamma-0.4.2/src/gamma/components/component_inventory.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_motion.py` & `pygame_gamma-0.4.2/src/gamma/components/component_motion.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_particle_emitter.py` & `pygame_gamma-0.4.2/src/gamma/components/component_particle_emitter.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_position.py` & `pygame_gamma-0.4.2/src/gamma/components/component_position.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_sprites.py` & `pygame_gamma-0.4.2/src/gamma/components/component_sprites.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_tags.py` & `pygame_gamma-0.4.2/src/gamma/components/component_tags.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_text.py` & `pygame_gamma-0.4.2/src/gamma/components/component_text.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_trauma.py` & `pygame_gamma-0.4.2/src/gamma/components/component_trauma.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/components/component_triggers.py` & `pygame_gamma-0.4.2/src/gamma/components/component_triggers.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/colours.py` & `pygame_gamma-0.4.2/src/gamma/core/colours.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/cutscene.py` & `pygame_gamma-0.4.2/src/gamma/core/cutscene.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/entity.py` & `pygame_gamma-0.4.2/src/gamma/core/entity.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/map.py` & `pygame_gamma-0.4.2/src/gamma/core/map.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/particle.py` & `pygame_gamma-0.4.2/src/gamma/core/particle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/renderable.py` & `pygame_gamma-0.4.2/src/gamma/core/renderable.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/renderer.py` & `pygame_gamma-0.4.2/src/gamma/core/renderer.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/scene.py` & `pygame_gamma-0.4.2/src/gamma/core/scene.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/sprite.py` & `pygame_gamma-0.4.2/src/gamma/core/sprite.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/system.py` & `pygame_gamma-0.4.2/src/gamma/core/system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/tile.py` & `pygame_gamma-0.4.2/src/gamma/core/tile.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/core/transition.py` & `pygame_gamma-0.4.2/src/gamma/core/transition.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/fonts/munro.ttf` & `pygame_gamma-0.4.2/src/gamma/fonts/munro.ttf`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/images/emote_box.png` & `pygame_gamma-0.4.2/src/gamma/images/emote_box.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/images/gamma.png` & `pygame_gamma-0.4.2/src/gamma/images/gamma.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/images/tile_outline.png` & `pygame_gamma-0.4.2/src/gamma/images/tile_outline.png`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/input/controller.py` & `pygame_gamma-0.4.2/src/gamma/input/controller.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/input/keyboard.py` & `pygame_gamma-0.4.2/src/gamma/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_entity.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_entity.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_input.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_input.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_resource.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_resource.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_scene.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_scene.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_sound.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_sound.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/managers/manager_system.py` & `pygame_gamma-0.4.2/src/gamma/managers/manager_system.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/renderables/circle.py` & `pygame_gamma-0.4.2/src/gamma/renderables/circle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/renderables/image.py` & `pygame_gamma-0.4.2/src/gamma/renderables/image.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/renderables/rectangle.py` & `pygame_gamma-0.4.2/src/gamma/renderables/rectangle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/renderables/text.py` & `pygame_gamma-0.4.2/src/gamma/renderables/text.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_animation.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_animation.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_battle.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_battle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_camera.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_camera.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_collision.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_collision.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_emote.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_emote.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_image.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_image.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_input.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_input.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_particle.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_particle.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_physics.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_physics.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_text.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_text.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/systems/system_trigger.py` & `pygame_gamma-0.4.2/src/gamma/systems/system_trigger.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_black.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_black.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyinleft.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_flyinleft.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyinright.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_flyinright.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyoutleft.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_flyoutleft.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_flyoutright.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_flyoutright.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_moveleft.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_moveleft.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_moveright.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_moveright.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_wipeleft.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_wipeleft.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/transitions/transition_wiperight.py` & `pygame_gamma-0.4.2/src/gamma/transitions/transition_wiperight.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_button.py` & `pygame_gamma-0.4.2/src/gamma/ui/ui_button.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_menu.py` & `pygame_gamma-0.4.2/src/gamma/ui/ui_menu.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text.py` & `pygame_gamma-0.4.2/src/gamma/ui/ui_text.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text_input.py` & `pygame_gamma-0.4.2/src/gamma/ui/ui_text_input.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/ui/ui_text_menu_item.py` & `pygame_gamma-0.4.2/src/gamma/ui/ui_text_menu_item.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/utils/utils.py` & `pygame_gamma-0.4.2/src/gamma/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/src/pygame-gamma/utils/utils_draw.py` & `pygame_gamma-0.4.2/src/gamma/utils/utils_draw.py`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/LICENSE` & `pygame_gamma-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/README.md` & `pygame_gamma-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pygame_gamma-0.4.1/pyproject.toml` & `pygame_gamma-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/gamma"]
+packages = ["src/pygame-gamma"]
 
 [project]
 name = "pygame-gamma"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Rik Cross", email="rik.j.cross@gmail.com" },
 ]
 description = "A simple ECS game engine for Python, built on Pygame, with an emphasis on ease of use"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygame_gamma-0.4.1/PKG-INFO` & `pygame_gamma-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pygame-gamma
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple ECS game engine for Python, built on Pygame, with an emphasis on ease of use
 Project-URL: Homepage, https://github.com/rik-cross/gamma
 Project-URL: Suggestions and bugs, https://github.com/rik-cross/gamma/issues
 Author-email: Rik Cross <rik.j.cross@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

