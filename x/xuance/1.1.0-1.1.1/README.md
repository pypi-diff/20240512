# Comparing `tmp/xuance-1.1.0.tar.gz` & `tmp/xuance-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xuance-1.1.0.tar", last modified: Wed May  1 15:42:23 2024, max compression
+gzip compressed data, was "dist/xuance-1.1.1.tar", last modified: Sun May 12 09:32:27 2024, max compression
```

## Comparing `xuance-1.1.0.tar` & `xuance-1.1.1.tar`

### file list

```diff
@@ -1,833 +1,843 @@
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-12-25 08:46:35.000000 xuance-1.1.0/LICENSE.txt
--rw-r--r--   0 wzliu     (1000) wzliu     (1000)     2693 2024-05-01 15:42:23.196396 xuance-1.1.0/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    19574 2024-04-14 03:11:12.000000 xuance-1.1.0/README.md
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       38 2024-05-01 15:42:23.196396 xuance-1.1.0/setup.cfg
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3603 2024-05-01 15:40:41.000000 xuance-1.1.0/setup.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      185 2024-04-11 09:02:57.000000 xuance-1.1.0/xuance/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/common/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      213 2023-12-18 07:52:17.000000 xuance-1.1.0/xuance/common/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13861 2024-05-01 08:19:43.000000 xuance-1.1.0/xuance/common/common_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    25239 2023-12-21 05:26:17.000000 xuance-1.1.0/xuance/common/memory_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    36896 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/common/memory_tools_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-12-19 13:13:16.000000 xuance-1.1.0/xuance/common/segtree_tool.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4606 2023-12-19 11:27:23.000000 xuance-1.1.0/xuance/common/statistic_tools.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1426 2023-12-18 07:52:53.000000 xuance-1.1.0/xuance/configs/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      749 2024-05-01 14:59:33.000000 xuance-1.1.0/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      726 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      747 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      750 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      751 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      770 2024-05-01 15:18:11.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      764 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/a2c/mujoco.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/configs/basic.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1110 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/c51/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      811 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      667 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      673 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      674 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      677 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/coma/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/coma/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/coma/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1153 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1158 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1154 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1151 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/coma/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/coma/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1152 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/dcg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/dcg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dcg/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1679 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1681 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1677 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1680 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      683 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      715 2024-05-01 15:18:41.000000 xuance-1.1.0/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      832 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/ddpg/drones.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      824 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/ddpg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      784 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      637 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      645 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      646 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1078 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      781 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      634 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      633 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1145 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      870 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/drqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      794 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iddpg/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1038 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/drones.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1044 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1039 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1037 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/ippo/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2014 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1474 2024-05-01 14:03:25.000000 xuance-1.1.0/xuance/configs/ippo/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1532 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1551 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1590 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1528 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ippo/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1553 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ippo/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/iql/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      927 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/iql/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1079 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1076 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/iql/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1101 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1077 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/iql/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/iql/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/isac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/isac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1041 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1043 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/maddpg/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1035 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/drones.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/maddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1007 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1029 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_spread_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      976 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/new_env_mas.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mappo/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2002 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/football/1v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2017 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1525 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1535 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1524 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1543 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1592 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1522 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1520 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1557 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1542 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1545 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/masac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/masac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1050 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1045 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1048 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/matd3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/matd3/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      990 2024-05-01 14:14:07.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      985 2024-05-01 14:14:07.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      987 2024-05-01 14:14:06.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mfac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1642 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/mfac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mfq/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfq/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfq/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mfq/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mpdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      725 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/mpdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      796 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      656 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      720 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/pdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1118 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      821 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      680 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      681 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      721 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/pg/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      692 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/pg/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      701 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/pg/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/pg/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/pg/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      731 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/pg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      730 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/pg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      722 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      691 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ppg/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      703 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      698 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      707 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      727 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      734 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1285 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ppo/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      807 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      983 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ppo/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      782 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      790 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      813 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1074 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/drones.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1102 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/metadrive.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      937 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/ppo/minigrid.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      887 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/qmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1667 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1216 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1215 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1218 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1214 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1212 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1213 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1219 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1098 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      801 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      663 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      666 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/qtran/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qtran/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1121 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qtran/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/random/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/random/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      121 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_adversary.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      116 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_push.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      118 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1034 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/sac/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      696 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/sac/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/sac/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      935 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/metadrive.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      728 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/spdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      656 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/spdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      689 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/td3/box2d/BipedalWalker-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      727 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/td3/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      813 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/td3/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/vdac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/vdac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2024-05-01 14:19:34.000000 xuance-1.1.0/xuance/configs/vdac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdac/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1664 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1721 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1665 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdac/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1662 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1464 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1719 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1723 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdac/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1560 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      940 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/mpe/simple_spread_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      977 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/new_env_mas.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1092 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdn/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdn/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/wqmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/wqmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1287 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/wqmix/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1277 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1276 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1279 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1275 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1278 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6407 2024-04-24 07:21:56.000000 xuance-1.1.0/xuance/environment/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/drones/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      336 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/drones/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/drones/customized/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3983 2024-02-23 12:32:58.000000 xuance-1.1.0/xuance/environment/drones/customized/HoverAviary.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6687 2024-04-16 12:40:23.000000 xuance-1.1.0/xuance/environment/drones/customized/MultiHoverAviary.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2024-02-23 12:27:09.000000 xuance-1.1.0/xuance/environment/drones/customized/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4266 2024-04-23 05:11:00.000000 xuance-1.1.0/xuance/environment/drones/drones_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4437 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/drones/drones_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9817 2024-03-01 08:07:09.000000 xuance-1.1.0/xuance/environment/drones/drones_vec_env_mas.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2357 2024-04-23 04:42:48.000000 xuance-1.1.0/xuance/environment/football/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3526 2024-04-22 07:53:14.000000 xuance-1.1.0/xuance/environment/football/gfootball_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11382 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/football/gfootball_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4850 2024-04-22 07:54:05.000000 xuance-1.1.0/xuance/environment/football/raw_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      233 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/gym/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10151 2023-12-14 05:19:51.000000 xuance-1.1.0/xuance/environment/gym/gym_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10348 2024-03-01 07:44:31.000000 xuance-1.1.0/xuance/environment/gym/gym_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym_platform/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      239 2019-05-17 10:11:51.000000 xuance-1.1.0/xuance/environment/gym_platform/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym_platform/envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       74 2023-12-14 06:11:08.000000 xuance-1.1.0/xuance/environment/gym_platform/envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21868 2023-12-14 05:45:17.000000 xuance-1.1.0/xuance/environment/gym_platform/envs/platform_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      742 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/magent2/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/builtin/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/builtin/config/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/battle.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1372 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/double_attack.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1150 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/forest.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1015 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/pursuit.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1229 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/c_lib.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environment.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      155 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       60 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7541 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       91 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit_v4.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/battle/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8888 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle/battle.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle_v4.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       52 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8882 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/battlefield.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       66 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield_v5.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       54 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12397 2023-10-20 05:41:15.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/combined_arms.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       68 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms_v6.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/gather/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9543 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather/gather.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather_v5.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10576 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/magent_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       51 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7817 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       65 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer_v4.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    31405 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/gridworld.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   166808 2023-12-12 04:50:11.000000 xuance-1.1.0/xuance/environment/magent2/libmagent.dylib
--rwxrwxr-x   0 wzliu     (1000) wzliu     (1000)  2945728 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/libmagent.so
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   126464 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/magent.dll
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3247 2024-02-20 07:58:49.000000 xuance-1.1.0/xuance/environment/magent2/magent_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      984 2024-01-08 03:46:25.000000 xuance-1.1.0/xuance/environment/magent2/magent_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11270 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/render.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3233 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/utility.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/metadrive/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       83 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/metadrive/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1401 2024-04-23 05:11:00.000000 xuance-1.1.0/xuance/environment/metadrive/metadrive_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      826 2024-04-18 04:02:14.000000 xuance-1.1.0/xuance/environment/metadrive/metadrive_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/minigrid/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      109 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/minigrid/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2712 2023-12-27 02:21:08.000000 xuance-1.1.0/xuance/environment/minigrid/minigrid_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1242 2024-03-01 03:02:51.000000 xuance-1.1.0/xuance/environment/minigrid/minigrid_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/new_env/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       86 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/new_env/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2142 2024-05-01 08:48:40.000000 xuance-1.1.0/xuance/environment/new_env/new_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1230 2023-12-02 04:54:59.000000 xuance-1.1.0/xuance/environment/new_env/new_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/new_env_mas/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      102 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/new_env_mas/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3273 2024-03-28 11:11:38.000000 xuance-1.1.0/xuance/environment/new_env_mas/new_env_mas.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9939 2024-03-23 08:28:32.000000 xuance-1.1.0/xuance/environment/new_env_mas/new_vec_env_mas.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/pettingzoo/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      186 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/pettingzoo/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5672 2024-04-22 07:52:00.000000 xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18308 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/robotic_warehouse/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2024-02-21 11:20:19.000000 xuance-1.1.0/xuance/environment/robotic_warehouse/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2387 2024-02-21 12:24:01.000000 xuance-1.1.0/xuance/environment/robotic_warehouse/robotic_warehouse_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/starcraft2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      103 2024-04-23 04:42:01.000000 xuance-1.1.0/xuance/environment/starcraft2/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2079 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/starcraft2/sc2_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12562 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/starcraft2/sc2_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/vector_envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      448 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3990 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/env_utils.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4649 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/subproc_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2198 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/vector_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/mindspore/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/mindspore/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4007 2023-12-12 07:20:21.000000 xuance-1.1.0/xuance/mindspore/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5252 2024-01-18 07:03:28.000000 xuance-1.1.0/xuance/mindspore/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2640 2023-12-11 07:21:42.000000 xuance-1.1.0/xuance/mindspore/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7347 2023-12-10 06:30:07.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5758 2023-12-27 08:59:15.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2776 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6168 2023-12-12 05:44:12.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4743 2023-12-27 09:00:15.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2721 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2779 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6454 2023-12-13 03:46:25.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2769 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3045 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4653 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5055 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4910 2023-12-27 09:00:48.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5237 2023-12-27 09:01:17.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5479 2023-12-14 15:09:07.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4777 2023-12-27 09:01:49.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5068 2023-12-27 08:49:17.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7507 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6427 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8389 2023-12-14 08:59:31.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7622 2023-12-14 08:59:31.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6786 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8517 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7431 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6552 2023-12-25 08:01:55.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5832 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6167 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8054 2023-12-14 08:59:32.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6261 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/C51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6351 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7569 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6376 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6382 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6775 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6360 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2445 2023-12-14 07:33:46.000000 xuance-1.1.0/xuance/mindspore/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3773 2023-12-12 05:18:55.000000 xuance-1.1.0/xuance/mindspore/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5469 2023-12-10 07:25:06.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9850 2023-12-11 05:36:13.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3696 2023-12-12 04:28:24.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6130 2023-12-13 03:59:31.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2847 2023-12-12 07:23:31.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4341 2023-12-13 04:22:33.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4010 2023-12-12 12:04:11.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6260 2023-12-13 04:02:46.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4346 2023-12-13 05:38:16.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5292 2023-12-13 05:53:16.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3566 2023-12-13 09:58:44.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3448 2023-12-14 04:59:30.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-12-14 12:28:36.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6262 2023-12-14 13:33:25.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3483 2023-12-14 15:09:41.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3184 2023-12-14 15:17:55.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4808 2023-12-14 15:23:28.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2422 2023-12-09 11:20:09.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2707 2023-12-11 08:46:06.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4558 2023-12-14 06:37:27.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3227 2023-12-14 08:11:30.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2101 2023-12-14 11:00:21.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4400 2023-12-14 11:29:33.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2747 2023-12-14 11:47:36.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2798 2023-12-15 02:16:25.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2738 2023-12-14 14:03:37.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3166 2023-12-14 13:57:10.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4570 2023-12-14 08:16:36.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3100 2023-12-14 14:11:09.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3599 2023-12-10 02:53:02.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2380 2023-12-11 14:44:06.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2367 2023-12-11 14:52:23.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2750 2023-12-11 16:09:42.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2239 2023-12-12 02:46:31.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2440 2023-12-14 07:36:25.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2624 2023-12-14 10:42:40.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-14 12:42:12.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8887 2023-12-13 02:58:26.000000 xuance-1.1.0/xuance/mindspore/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14094 2023-12-14 13:56:24.000000 xuance-1.1.0/xuance/mindspore/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16181 2023-12-27 08:44:15.000000 xuance-1.1.0/xuance/mindspore/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4460 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/mindspore/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    40243 2023-12-22 09:37:01.000000 xuance-1.1.0/xuance/mindspore/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29574 2023-12-27 08:39:23.000000 xuance-1.1.0/xuance/mindspore/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10536 2023-12-23 04:26:37.000000 xuance-1.1.0/xuance/mindspore/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16781 2023-12-27 08:43:51.000000 xuance-1.1.0/xuance/mindspore/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6926 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/mindspore/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      939 2023-12-15 05:03:25.000000 xuance-1.1.0/xuance/mindspore/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3706 2023-12-15 04:57:29.000000 xuance-1.1.0/xuance/mindspore/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1570 2023-12-15 04:57:29.000000 xuance-1.1.0/xuance/mindspore/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3600 2023-12-15 05:05:10.000000 xuance-1.1.0/xuance/mindspore/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      198 2023-12-10 03:30:31.000000 xuance-1.1.0/xuance/mindspore/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      376 2023-12-08 14:07:56.000000 xuance-1.1.0/xuance/mindspore/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7274 2023-12-09 11:58:58.000000 xuance-1.1.0/xuance/mindspore/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21371 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/mindspore/runners/runner_pettingzoo.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      555 2023-12-10 05:41:45.000000 xuance-1.1.0/xuance/mindspore/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4934 2023-12-15 06:04:32.000000 xuance-1.1.0/xuance/mindspore/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3930 2023-12-15 05:03:25.000000 xuance-1.1.0/xuance/mindspore/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2421 2023-12-08 14:09:42.000000 xuance-1.1.0/xuance/mindspore/utils/operations.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/utils/set_trainer.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4028 2023-12-18 09:17:36.000000 xuance-1.1.0/xuance/tensorflow/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5342 2024-01-18 07:03:28.000000 xuance-1.1.0/xuance/tensorflow/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2688 2023-12-15 14:37:25.000000 xuance-1.1.0/xuance/tensorflow/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7409 2023-12-15 14:01:47.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5903 2023-12-27 11:01:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4844 2023-12-18 09:48:22.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5143 2023-12-15 15:11:06.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2809 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2974 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5487 2023-12-18 10:42:02.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2813 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4789 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4323 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5133 2023-12-15 15:32:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5415 2023-12-15 16:17:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5602 2023-12-18 11:20:47.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4991 2023-12-15 15:22:26.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5291 2023-12-15 16:12:55.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7251 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6212 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7961 2023-12-18 08:14:46.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7930 2023-12-15 09:02:49.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6780 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8848 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7501 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7564 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5893 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6194 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7557 2023-12-15 09:13:28.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6267 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6221 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6373 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6366 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7533 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6398 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6353 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6797 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6383 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2319 2023-12-18 09:16:20.000000 xuance-1.1.0/xuance/tensorflow/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3451 2023-12-18 11:10:06.000000 xuance-1.1.0/xuance/tensorflow/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4782 2023-12-18 06:50:12.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8735 2023-12-18 14:51:09.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3740 2023-12-18 06:53:36.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5340 2023-12-18 10:15:58.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2023-12-15 15:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4039 2023-12-18 06:55:07.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3870 2023-12-18 06:57:53.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5534 2023-12-18 10:49:48.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4042 2023-12-18 06:59:18.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3949 2023-12-18 08:51:07.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3461 2023-12-18 09:07:01.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3657 2023-12-18 07:00:35.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3768 2023-12-15 15:34:24.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6452 2023-12-15 16:20:03.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3612 2023-12-18 11:33:04.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3498 2023-12-15 15:30:10.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5335 2023-12-15 16:15:19.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2067 2023-12-15 02:16:24.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2580 2023-12-18 08:04:47.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2911 2023-12-18 08:14:00.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2865 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1725 2023-12-15 11:08:41.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4673 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2411 2023-12-15 11:58:35.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2770 2023-12-15 02:16:24.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3169 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2867 2023-12-18 08:15:19.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3039 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2535 2023-12-15 05:11:09.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 05:50:16.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2062 2023-12-15 07:32:39.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-12-15 07:40:07.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2078 2023-12-15 08:02:34.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 08:11:57.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2320 2023-12-15 08:16:49.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10285 2023-12-27 10:44:41.000000 xuance-1.1.0/xuance/tensorflow/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11117 2023-12-15 13:41:09.000000 xuance-1.1.0/xuance/tensorflow/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    17686 2023-12-27 10:46:13.000000 xuance-1.1.0/xuance/tensorflow/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4383 2023-12-23 09:08:24.000000 xuance-1.1.0/xuance/tensorflow/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42293 2023-12-22 09:37:01.000000 xuance-1.1.0/xuance/tensorflow/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    32883 2023-12-27 13:06:20.000000 xuance-1.1.0/xuance/tensorflow/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11288 2023-12-15 11:31:24.000000 xuance-1.1.0/xuance/tensorflow/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16441 2023-12-27 10:46:13.000000 xuance-1.1.0/xuance/tensorflow/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8074 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/tensorflow/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      906 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2023-12-15 07:51:58.000000 xuance-1.1.0/xuance/tensorflow/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       49 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      195 2023-12-15 02:02:01.000000 xuance-1.1.0/xuance/tensorflow/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1009 2023-12-15 08:54:19.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6832 2023-12-15 06:06:26.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21509 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_pettingzoo.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      618 2023-12-15 12:49:56.000000 xuance-1.1.0/xuance/tensorflow/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2023-12-15 13:25:10.000000 xuance-1.1.0/xuance/tensorflow/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4128 2023-12-15 06:51:54.000000 xuance-1.1.0/xuance/tensorflow/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3859 2023-12-15 11:37:34.000000 xuance-1.1.0/xuance/tensorflow/utils/operations.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2678 2024-05-01 10:42:19.000000 xuance-1.1.0/xuance/torch/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5897 2024-05-01 10:20:05.000000 xuance-1.1.0/xuance/torch/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3425 2024-05-01 09:48:01.000000 xuance-1.1.0/xuance/torch/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      638 2024-04-22 13:08:14.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7853 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6327 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3328 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6649 2024-01-30 07:07:08.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5188 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3181 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3279 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7007 2024-03-30 09:29:07.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3176 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2024-05-01 14:32:15.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5111 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5443 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5378 2024-05-01 10:42:14.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5770 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5858 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5234 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5555 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      424 2024-04-22 13:07:06.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8083 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6855 2024-01-30 08:04:24.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8203 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8391 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7355 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8951 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8254 2024-04-17 04:33:18.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8045 2024-04-14 06:51:57.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6487 2024-04-25 12:16:23.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6819 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7767 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6874 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.188396 xuance-1.1.0/xuance/torch/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      296 2024-04-22 13:07:15.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6959 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7012 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6956 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8193 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7040 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6994 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7437 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7018 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.188396 xuance-1.1.0/xuance/torch/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1064 2024-04-22 13:00:21.000000 xuance-1.1.0/xuance/torch/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2024-05-01 10:21:47.000000 xuance-1.1.0/xuance/torch/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      640 2024-04-22 13:02:22.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8825 2023-11-04 11:24:47.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11559 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9879 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6037 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3761 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3606 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10946 2024-01-29 04:09:10.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3764 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3415 2024-05-01 14:31:15.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3290 2023-12-13 08:47:10.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3145 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6656 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5382 2023-12-14 13:10:44.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6097 2023-12-14 14:54:20.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6440 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10661 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      472 2024-04-22 13:01:54.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1887 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2056 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 06:23:29.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2298 2023-12-14 06:01:04.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3555 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2681 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2416 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2141 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2570 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 07:59:27.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2432 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      281 2024-04-22 13:02:07.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2256 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1881 2023-12-11 14:43:00.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1810 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2151 2023-10-20 05:41:15.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1818 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1903 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1907 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/ssl_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/learners/ssl_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/learners/ssl_rl/curl_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10442 2024-05-01 15:26:37.000000 xuance-1.1.0/xuance/torch/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11695 2024-04-22 13:06:16.000000 xuance-1.1.0/xuance/torch/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15749 2024-01-31 09:53:33.000000 xuance-1.1.0/xuance/torch/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3964 2023-12-18 12:16:47.000000 xuance-1.1.0/xuance/torch/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42041 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29895 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12014 2024-05-01 15:29:30.000000 xuance-1.1.0/xuance/torch/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13728 2024-05-01 14:00:37.000000 xuance-1.1.0/xuance/torch/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6646 2023-11-04 15:22:56.000000 xuance-1.1.0/xuance/torch/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1268 2023-12-15 05:00:06.000000 xuance-1.1.0/xuance/torch/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4150 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2066 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3944 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/xuance/torch/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-02-22 11:27:05.000000 xuance-1.1.0/xuance/torch/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      372 2023-11-08 08:20:22.000000 xuance-1.1.0/xuance/torch/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7016 2024-05-01 15:10:48.000000 xuance-1.1.0/xuance/torch/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9455 2023-11-09 12:03:08.000000 xuance-1.1.0/xuance/torch/runners/runner_football.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      171 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/torch/runners/runner_magent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16013 2024-05-01 10:20:05.000000 xuance-1.1.0/xuance/torch/runners/runner_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21469 2024-05-01 14:34:22.000000 xuance-1.1.0/xuance/torch/runners/runner_pettingzoo.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21193 2024-05-01 10:46:01.000000 xuance-1.1.0/xuance/torch/runners/runner_sc2.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/xuance/torch/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      935 2024-05-01 13:27:29.000000 xuance-1.1.0/xuance/torch/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-10-27 12:18:06.000000 xuance-1.1.0/xuance/torch/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5748 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4412 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3826 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/operations.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3098 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/value_norm.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance.egg-info/
--rw-r--r--   0 wzliu     (1000) wzliu     (1000)     2693 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    30714 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/SOURCES.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/dependency_links.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      451 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/requires.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        7 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/top_level.txt
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-12-25 08:46:35.000000 xuance-1.1.1/LICENSE.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1748 2024-05-12 09:32:27.000000 xuance-1.1.1/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    19604 2024-05-09 01:00:24.000000 xuance-1.1.1/README.md
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       38 2024-05-12 09:32:27.000000 xuance-1.1.1/setup.cfg
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3567 2024-05-12 09:29:43.000000 xuance-1.1.1/setup.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      185 2024-04-11 09:02:57.000000 xuance-1.1.1/xuance/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/common/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      213 2023-12-18 07:52:17.000000 xuance-1.1.1/xuance/common/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13799 2024-05-08 06:28:00.000000 xuance-1.1.1/xuance/common/common_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    25456 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/common/memory_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    36883 2024-05-06 02:01:30.000000 xuance-1.1.1/xuance/common/memory_tools_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-12-19 13:13:16.000000 xuance-1.1.1/xuance/common/segtree_tool.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4606 2023-12-19 11:27:23.000000 xuance-1.1.1/xuance/common/statistic_tools.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1426 2023-12-18 07:52:53.000000 xuance-1.1.1/xuance/configs/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/a2c/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1218 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/a2c/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/a2c/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      834 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      811 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/a2c/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/a2c/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      832 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/a2c/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      835 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/a2c/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      836 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/a2c/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      855 2024-05-09 14:40:37.000000 xuance-1.1.1/xuance/configs/a2c/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      849 2024-05-09 14:41:58.000000 xuance-1.1.1/xuance/configs/a2c/mujoco.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-05-06 06:17:14.000000 xuance-1.1.1/xuance/configs/basic.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/c51/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1115 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/c51/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/c51/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      816 2024-05-06 02:02:51.000000 xuance-1.1.1/xuance/configs/c51/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      673 2024-05-06 02:02:51.000000 xuance-1.1.1/xuance/configs/c51/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/c51/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      679 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/c51/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      680 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/c51/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      683 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/c51/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/coma/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/coma/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-09 14:24:53.000000 xuance-1.1.1/xuance/configs/coma/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/coma/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1161 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1158 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1163 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1159 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1165 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1157 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1165 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1161 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1165 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/coma/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dcg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dcg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/dcg/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dcg/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1679 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/dcg/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/dcg/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1681 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/dcg/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1677 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/dcg/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/dcg/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/dcg/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/dcg/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/dcg/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1680 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/dcg/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/dcg/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddpg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddpg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      735 2024-05-07 09:05:48.000000 xuance-1.1.1/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddpg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      700 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      837 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddpg/drones.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      830 2024-05-10 08:33:20.000000 xuance-1.1.1/xuance/configs/ddpg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      643 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ddqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      651 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      652 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1083 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      786 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      640 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      639 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/drqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1150 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/drqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      875 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      766 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/drqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      766 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      767 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      803 2024-05-06 03:27:56.000000 xuance-1.1.1/xuance/configs/drqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dueldqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1102 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dueldqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      798 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/dueldqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      660 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      661 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      665 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iddpg/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1038 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/iddpg/drones.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1044 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1039 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/iddpg/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1037 2024-05-09 06:18:04.000000 xuance-1.1.1/xuance/configs/iddpg/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ippo/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ippo/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2019 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ippo/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ippo/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1537 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1556 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1595 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1535 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1533 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1566 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1555 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1566 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1563 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/ippo/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      927 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/iql/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      930 2024-05-08 06:01:06.000000 xuance-1.1.1/xuance/configs/iql/robotic_warehouse/rware-tiny-2ag-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/iql/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1079 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1076 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/iql/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1101 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1077 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/iql/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/iql/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/iql/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/isac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/isac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1081 2024-05-08 10:04:31.000000 xuance-1.1.1/xuance/configs/isac/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1076 2024-05-08 10:04:31.000000 xuance-1.1.1/xuance/configs/isac/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1078 2024-05-08 09:08:04.000000 xuance-1.1.1/xuance/configs/isac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/maddpg/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1035 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/maddpg/drones.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/maddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1007 2024-05-01 13:26:43.000000 xuance-1.1.1/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1029 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/maddpg/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/maddpg/mpe/simple_spread_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      976 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/maddpg/new_env_mas.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mappo/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mappo/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2007 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/football/1v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mappo/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1535 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1533 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mappo/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1542 2024-05-10 15:12:40.000000 xuance-1.1.1/xuance/configs/mappo/robotic_warehouse/rware-tiny-2ag-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mappo/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1529 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1548 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1597 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1527 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1525 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1562 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1547 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1563 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1555 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/mappo/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/masac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/masac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1085 2024-05-08 10:04:31.000000 xuance-1.1.1/xuance/configs/masac/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2024-05-08 10:04:31.000000 xuance-1.1.1/xuance/configs/masac/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1083 2024-05-08 10:04:31.000000 xuance-1.1.1/xuance/configs/masac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/matd3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/matd3/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      990 2024-05-01 14:14:07.000000 xuance-1.1.1/xuance/configs/matd3/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      985 2024-05-01 14:14:07.000000 xuance-1.1.1/xuance/configs/matd3/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      996 2024-05-09 14:10:11.000000 xuance-1.1.1/xuance/configs/matd3/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mfac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mfac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1642 2024-05-01 13:26:44.000000 xuance-1.1.1/xuance/configs/mfac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mfq/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mfq/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mfq/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/mfq/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/mpdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      730 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/mpdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/noisydqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1098 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/noisydqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/noisydqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      801 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/noisydqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      661 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2024-05-07 06:31:06.000000 xuance-1.1.1/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      665 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/pdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      725 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/pdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/perdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1123 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/perdqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      826 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/perdqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      686 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      687 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/pg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/pg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      806 2024-05-09 14:41:58.000000 xuance-1.1.1/xuance/configs/pg/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      780 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/pg/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/pg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2024-05-06 03:08:48.000000 xuance-1.1.1/xuance/configs/pg/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      787 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/pg/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      791 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/pg/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      816 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/pg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      815 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/pg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      807 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      776 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppg/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      788 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppg/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      783 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppg/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      792 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppg/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      812 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      819 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppo/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1370 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/ppo/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppo/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      892 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1068 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppo/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      867 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppo/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/ppo/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      874 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppo/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      875 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppo/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      878 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppo/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      898 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppo/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1159 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppo/drones.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1187 2024-05-09 14:40:18.000000 xuance-1.1.1/xuance/configs/ppo/metadrive.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1022 2024-05-09 14:39:55.000000 xuance-1.1.1/xuance/configs/ppo/minigrid.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      972 2024-05-09 14:39:54.000000 xuance-1.1.1/xuance/configs/ppo/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qmix/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1667 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/qmix/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qmix/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1051 2024-05-10 15:10:50.000000 xuance-1.1.1/xuance/configs/qmix/robotic_warehouse/rware-tiny-2ag-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qmix/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1216 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/qmix/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1215 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1218 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1214 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1212 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/qmix/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1213 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/qmix/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/qmix/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1219 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/qmix/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/qmix/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qrdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1103 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qrdqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      806 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      660 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qrdqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      668 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      669 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      672 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qtran/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/qtran/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1121 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/qtran/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/random/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/random/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      121 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/configs/random/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      116 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/configs/random/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      118 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/configs/random/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/sac/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1019 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/sac/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      749 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/sac/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      689 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      692 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      713 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      859 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/drones.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      922 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/metadrive.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      740 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/sac/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/spdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      661 2024-05-06 02:17:51.000000 xuance-1.1.1/xuance/configs/spdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/td3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/td3/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      730 2024-05-07 09:01:54.000000 xuance-1.1.1/xuance/configs/td3/box2d/BipedalWalker-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/td3/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      733 2024-05-06 02:23:59.000000 xuance-1.1.1/xuance/configs/td3/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      819 2024-05-10 14:21:42.000000 xuance-1.1.1/xuance/configs/td3/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1681 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdac/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1669 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1670 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1667 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1469 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1735 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1724 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1735 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1733 2024-05-09 14:29:18.000000 xuance-1.1.1/xuance/configs/vdac/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdn/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1560 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdn/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      940 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/mpe/simple_spread_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      977 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/new_env_mas.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdn/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      928 2024-05-10 15:09:37.000000 xuance-1.1.1/xuance/configs/vdn/robotic_warehouse/rware-tiny-2ag-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/vdn/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/vdn/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1092 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/vdn/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/vdn/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/vdn/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/vdn/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/vdn/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/vdn/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/wqmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/wqmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1287 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1277 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1276 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1279 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1275 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:17.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1278 2024-05-01 13:26:16.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.1/xuance/configs/wqmix/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6678 2024-05-08 02:38:01.000000 xuance-1.1.1/xuance/environment/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/drones/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      336 2024-04-23 04:44:07.000000 xuance-1.1.1/xuance/environment/drones/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/drones/customized/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3983 2024-02-23 12:32:58.000000 xuance-1.1.1/xuance/environment/drones/customized/HoverAviary.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6687 2024-04-16 12:40:23.000000 xuance-1.1.1/xuance/environment/drones/customized/MultiHoverAviary.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2024-02-23 12:27:09.000000 xuance-1.1.1/xuance/environment/drones/customized/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4266 2024-04-23 05:11:00.000000 xuance-1.1.1/xuance/environment/drones/drones_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4437 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/environment/drones/drones_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9817 2024-03-01 08:07:09.000000 xuance-1.1.1/xuance/environment/drones/drones_vec_env_mas.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2357 2024-04-23 04:42:48.000000 xuance-1.1.1/xuance/environment/football/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3526 2024-04-22 07:53:14.000000 xuance-1.1.1/xuance/environment/football/gfootball_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11382 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/environment/football/gfootball_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4850 2024-04-22 07:54:05.000000 xuance-1.1.1/xuance/environment/football/raw_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/gym/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      233 2024-04-22 07:42:41.000000 xuance-1.1.1/xuance/environment/gym/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10151 2023-12-14 05:19:51.000000 xuance-1.1.1/xuance/environment/gym/gym_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10348 2024-03-01 07:44:31.000000 xuance-1.1.1/xuance/environment/gym/gym_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/gym_platform/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      239 2019-05-17 10:11:51.000000 xuance-1.1.1/xuance/environment/gym_platform/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/gym_platform/envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       74 2023-12-14 06:11:08.000000 xuance-1.1.1/xuance/environment/gym_platform/envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21868 2023-12-14 05:45:17.000000 xuance-1.1.1/xuance/environment/gym_platform/envs/platform_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      742 2024-04-23 04:44:07.000000 xuance-1.1.1/xuance/environment/magent2/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/builtin/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/battle.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1372 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/double_attack.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1150 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/forest.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1015 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/builtin/config/pursuit.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1229 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/c_lib.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environment.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      155 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/adversarial_pursuit/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       60 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/adversarial_pursuit/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7541 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       91 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/adversarial_pursuit_v4.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/battle/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/battle/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8888 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/environment/magent2/environments/battle/battle.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/battle_v4.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/battlefield/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       52 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/battlefield/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8882 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/environment/magent2/environments/battlefield/battlefield.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       66 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/battlefield_v5.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/combined_arms/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       54 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/combined_arms/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12397 2023-10-20 05:41:15.000000 xuance-1.1.1/xuance/environment/magent2/environments/combined_arms/combined_arms.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       68 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/combined_arms_v6.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/gather/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/gather/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9543 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/environment/magent2/environments/gather/gather.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/gather_v5.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10576 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/magent_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/magent2/environments/tiger_deer/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       51 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/tiger_deer/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7817 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       65 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/environments/tiger_deer_v4.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    31405 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/gridworld.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   166808 2023-12-12 04:50:11.000000 xuance-1.1.1/xuance/environment/magent2/libmagent.dylib
+-rwxrwxr-x   0 wzliu     (1000) wzliu     (1000)  2945728 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/libmagent.so
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   126464 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/magent.dll
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3247 2024-02-20 07:58:49.000000 xuance-1.1.1/xuance/environment/magent2/magent_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      984 2024-01-08 03:46:25.000000 xuance-1.1.1/xuance/environment/magent2/magent_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11270 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/render.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3233 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/environment/magent2/utility.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/metadrive/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       83 2024-04-23 04:44:07.000000 xuance-1.1.1/xuance/environment/metadrive/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1401 2024-04-23 05:11:00.000000 xuance-1.1.1/xuance/environment/metadrive/metadrive_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      826 2024-04-18 04:02:14.000000 xuance-1.1.1/xuance/environment/metadrive/metadrive_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/minigrid/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      109 2024-04-23 04:44:07.000000 xuance-1.1.1/xuance/environment/minigrid/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2712 2023-12-27 02:21:08.000000 xuance-1.1.1/xuance/environment/minigrid/minigrid_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1242 2024-03-01 03:02:51.000000 xuance-1.1.1/xuance/environment/minigrid/minigrid_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/new_env/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       86 2024-04-23 04:44:50.000000 xuance-1.1.1/xuance/environment/new_env/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2142 2024-05-01 08:48:40.000000 xuance-1.1.1/xuance/environment/new_env/new_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1230 2023-12-02 04:54:59.000000 xuance-1.1.1/xuance/environment/new_env/new_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/new_env_mas/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      102 2024-04-23 04:44:50.000000 xuance-1.1.1/xuance/environment/new_env_mas/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3273 2024-03-28 11:11:38.000000 xuance-1.1.1/xuance/environment/new_env_mas/new_env_mas.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9939 2024-03-23 08:28:32.000000 xuance-1.1.1/xuance/environment/new_env_mas/new_vec_env_mas.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/pettingzoo/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      186 2024-04-23 04:44:50.000000 xuance-1.1.1/xuance/environment/pettingzoo/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5672 2024-04-22 07:52:00.000000 xuance-1.1.1/xuance/environment/pettingzoo/pettingzoo_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18308 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/environment/pettingzoo/pettingzoo_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      280 2024-05-08 05:34:07.000000 xuance-1.1.1/xuance/environment/robotic_warehouse/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2981 2024-05-08 06:22:33.000000 xuance-1.1.1/xuance/environment/robotic_warehouse/robotic_warehouse_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      462 2024-05-08 02:29:52.000000 xuance-1.1.1/xuance/environment/robotic_warehouse/robotic_warehouse_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/starcraft2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      103 2024-04-23 04:42:01.000000 xuance-1.1.1/xuance/environment/starcraft2/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2079 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/environment/starcraft2/sc2_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12562 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/environment/starcraft2/sc2_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/environment/vector_envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      448 2024-04-22 07:42:41.000000 xuance-1.1.1/xuance/environment/vector_envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3990 2024-04-22 07:42:41.000000 xuance-1.1.1/xuance/environment/vector_envs/env_utils.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4649 2024-04-22 07:42:41.000000 xuance-1.1.1/xuance/environment/vector_envs/subproc_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2198 2024-04-22 07:42:41.000000 xuance-1.1.1/xuance/environment/vector_envs/vector_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4007 2023-12-12 07:20:21.000000 xuance-1.1.1/xuance/mindspore/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5252 2024-01-18 07:03:28.000000 xuance-1.1.1/xuance/mindspore/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2640 2023-12-11 07:21:42.000000 xuance-1.1.1/xuance/mindspore/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7347 2023-12-10 06:30:07.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5758 2023-12-27 08:59:15.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2776 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6168 2023-12-12 05:44:12.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4743 2023-12-27 09:00:15.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2721 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2779 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6454 2023-12-13 03:46:25.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2769 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3045 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4653 2024-02-22 12:18:39.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5055 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4910 2023-12-27 09:00:48.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5237 2023-12-27 09:01:17.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5479 2023-12-14 15:09:07.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4777 2023-12-27 09:01:49.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5068 2023-12-27 08:49:17.000000 xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7507 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6427 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8389 2023-12-14 08:59:31.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7622 2023-12-14 08:59:31.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6786 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8517 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7431 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6552 2023-12-25 08:01:55.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5832 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6167 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8054 2023-12-14 08:59:32.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6261 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/C51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6351 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7569 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6376 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6382 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6775 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6360 2024-01-18 07:02:49.000000 xuance-1.1.1/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2445 2023-12-14 07:33:46.000000 xuance-1.1.1/xuance/mindspore/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3773 2023-12-12 05:18:55.000000 xuance-1.1.1/xuance/mindspore/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5469 2023-12-10 07:25:06.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9850 2023-12-11 05:36:13.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3696 2023-12-12 04:28:24.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6130 2023-12-13 03:59:31.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2847 2023-12-12 07:23:31.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4341 2023-12-13 04:22:33.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4010 2023-12-12 12:04:11.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6260 2023-12-13 04:02:46.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4346 2023-12-13 05:38:16.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5292 2023-12-13 05:53:16.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3566 2023-12-13 09:58:44.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3448 2023-12-14 04:59:30.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-12-14 12:28:36.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6262 2023-12-14 13:33:25.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3483 2023-12-14 15:09:41.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3184 2023-12-14 15:17:55.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4808 2023-12-14 15:23:28.000000 xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2422 2023-12-09 11:20:09.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2707 2023-12-11 08:46:06.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4558 2023-12-14 06:37:27.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3227 2023-12-14 08:11:30.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2101 2023-12-14 11:00:21.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4400 2023-12-14 11:29:33.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2747 2023-12-14 11:47:36.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2798 2023-12-15 02:16:25.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2738 2023-12-14 14:03:37.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3166 2023-12-14 13:57:10.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4570 2023-12-14 08:16:36.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3100 2023-12-14 14:11:09.000000 xuance-1.1.1/xuance/mindspore/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3599 2023-12-10 02:53:02.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2380 2023-12-11 14:44:06.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2367 2023-12-11 14:52:23.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2750 2023-12-11 16:09:42.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2239 2023-12-12 02:46:31.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2440 2023-12-14 07:36:25.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2624 2023-12-14 10:42:40.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-14 12:42:12.000000 xuance-1.1.1/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8887 2023-12-13 02:58:26.000000 xuance-1.1.1/xuance/mindspore/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14094 2023-12-14 13:56:24.000000 xuance-1.1.1/xuance/mindspore/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16181 2023-12-27 08:44:15.000000 xuance-1.1.1/xuance/mindspore/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4460 2023-12-23 08:58:45.000000 xuance-1.1.1/xuance/mindspore/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    40243 2023-12-22 09:37:01.000000 xuance-1.1.1/xuance/mindspore/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29574 2023-12-27 08:39:23.000000 xuance-1.1.1/xuance/mindspore/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10536 2023-12-23 04:26:37.000000 xuance-1.1.1/xuance/mindspore/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16781 2023-12-27 08:43:51.000000 xuance-1.1.1/xuance/mindspore/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6926 2023-12-23 08:58:45.000000 xuance-1.1.1/xuance/mindspore/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      939 2023-12-15 05:03:25.000000 xuance-1.1.1/xuance/mindspore/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3706 2023-12-15 04:57:29.000000 xuance-1.1.1/xuance/mindspore/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1570 2023-12-15 04:57:29.000000 xuance-1.1.1/xuance/mindspore/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3600 2023-12-15 05:05:10.000000 xuance-1.1.1/xuance/mindspore/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      198 2023-12-10 03:30:31.000000 xuance-1.1.1/xuance/mindspore/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      376 2023-12-08 14:07:56.000000 xuance-1.1.1/xuance/mindspore/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7274 2023-12-09 11:58:58.000000 xuance-1.1.1/xuance/mindspore/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21371 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/mindspore/runners/runner_pettingzoo.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/mindspore/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      555 2023-12-10 05:41:45.000000 xuance-1.1.1/xuance/mindspore/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4934 2023-12-15 06:04:32.000000 xuance-1.1.1/xuance/mindspore/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3930 2023-12-15 05:03:25.000000 xuance-1.1.1/xuance/mindspore/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2421 2023-12-08 14:09:42.000000 xuance-1.1.1/xuance/mindspore/utils/operations.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/mindspore/utils/set_trainer.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4028 2023-12-18 09:17:36.000000 xuance-1.1.1/xuance/tensorflow/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5342 2024-01-18 07:03:28.000000 xuance-1.1.1/xuance/tensorflow/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2688 2023-12-15 14:37:25.000000 xuance-1.1.1/xuance/tensorflow/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7409 2023-12-15 14:01:47.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5903 2023-12-27 11:01:48.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:39.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4844 2023-12-18 09:48:22.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5143 2023-12-15 15:11:06.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2809 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2974 2024-02-22 12:18:39.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5487 2023-12-18 10:42:02.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2813 2024-02-22 12:18:39.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4789 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4323 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5133 2023-12-15 15:32:48.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5415 2023-12-15 16:17:48.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5602 2023-12-18 11:20:47.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4991 2023-12-15 15:22:26.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5291 2023-12-15 16:12:55.000000 xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7251 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6212 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7961 2023-12-18 08:14:46.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7930 2023-12-15 09:02:49.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6780 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8848 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7501 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7564 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5893 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6194 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7557 2023-12-15 09:13:28.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6267 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6221 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6373 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6366 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7533 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6398 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6353 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6797 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6383 2024-01-18 07:02:30.000000 xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2319 2023-12-18 09:16:20.000000 xuance-1.1.1/xuance/tensorflow/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3451 2023-12-18 11:10:06.000000 xuance-1.1.1/xuance/tensorflow/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4782 2023-12-18 06:50:12.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8735 2023-12-18 14:51:09.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3740 2023-12-18 06:53:36.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5340 2023-12-18 10:15:58.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2023-12-15 15:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4039 2023-12-18 06:55:07.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3870 2023-12-18 06:57:53.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5534 2023-12-18 10:49:48.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4042 2023-12-18 06:59:18.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3949 2023-12-18 08:51:07.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3461 2023-12-18 09:07:01.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3657 2023-12-18 07:00:35.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3768 2023-12-15 15:34:24.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6452 2023-12-15 16:20:03.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3612 2023-12-18 11:33:04.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3498 2023-12-15 15:30:10.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5335 2023-12-15 16:15:19.000000 xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2067 2023-12-15 02:16:24.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2580 2023-12-18 08:04:47.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2911 2023-12-18 08:14:00.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2865 2023-12-18 08:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1725 2023-12-15 11:08:41.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4673 2023-12-18 08:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2411 2023-12-15 11:58:35.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2770 2023-12-15 02:16:24.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-12-18 08:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3169 2023-12-18 08:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2867 2023-12-18 08:15:19.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3039 2023-12-18 08:18:11.000000 xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2535 2023-12-15 05:11:09.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 05:50:16.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2062 2023-12-15 07:32:39.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-12-15 07:40:07.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2078 2023-12-15 08:02:34.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 08:11:57.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2320 2023-12-15 08:16:49.000000 xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10285 2023-12-27 10:44:41.000000 xuance-1.1.1/xuance/tensorflow/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11117 2023-12-15 13:41:09.000000 xuance-1.1.1/xuance/tensorflow/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    17686 2023-12-27 10:46:13.000000 xuance-1.1.1/xuance/tensorflow/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4383 2023-12-23 09:08:24.000000 xuance-1.1.1/xuance/tensorflow/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42293 2023-12-22 09:37:01.000000 xuance-1.1.1/xuance/tensorflow/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    32883 2023-12-27 13:06:20.000000 xuance-1.1.1/xuance/tensorflow/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11288 2023-12-15 11:31:24.000000 xuance-1.1.1/xuance/tensorflow/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16441 2023-12-27 10:46:13.000000 xuance-1.1.1/xuance/tensorflow/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8074 2023-12-23 08:58:45.000000 xuance-1.1.1/xuance/tensorflow/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      906 2023-12-15 06:57:56.000000 xuance-1.1.1/xuance/tensorflow/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2023-12-15 06:57:56.000000 xuance-1.1.1/xuance/tensorflow/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2023-12-15 07:51:58.000000 xuance-1.1.1/xuance/tensorflow/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       49 2023-12-15 06:57:56.000000 xuance-1.1.1/xuance/tensorflow/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      195 2023-12-15 02:02:01.000000 xuance-1.1.1/xuance/tensorflow/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1009 2023-12-15 08:54:19.000000 xuance-1.1.1/xuance/tensorflow/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6832 2023-12-15 06:06:26.000000 xuance-1.1.1/xuance/tensorflow/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21509 2024-02-22 12:36:38.000000 xuance-1.1.1/xuance/tensorflow/runners/runner_pettingzoo.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/tensorflow/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      618 2023-12-15 12:49:56.000000 xuance-1.1.1/xuance/tensorflow/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/tensorflow/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2023-12-15 13:25:10.000000 xuance-1.1.1/xuance/tensorflow/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4128 2023-12-15 06:51:54.000000 xuance-1.1.1/xuance/tensorflow/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3859 2023-12-15 11:37:34.000000 xuance-1.1.1/xuance/tensorflow/utils/operations.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/torch/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2678 2024-05-01 10:42:19.000000 xuance-1.1.1/xuance/torch/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6962 2024-05-06 07:15:02.000000 xuance-1.1.1/xuance/torch/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3425 2024-05-01 09:48:01.000000 xuance-1.1.1/xuance/torch/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      638 2024-04-22 13:08:14.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7822 2024-05-09 14:24:53.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6327 2023-12-20 02:55:43.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3325 2024-05-09 03:43:53.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6574 2024-05-09 14:24:53.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5188 2023-12-20 02:55:42.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3298 2024-05-08 09:08:38.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3276 2024-05-09 03:56:03.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7012 2024-05-09 14:24:53.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3295 2024-05-08 10:24:54.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3334 2024-05-09 13:41:57.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5111 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5443 2024-02-22 12:18:38.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5378 2024-05-01 10:42:14.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5770 2023-12-20 02:55:43.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5970 2024-05-10 14:43:12.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5234 2023-12-20 02:55:42.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5555 2023-12-20 02:55:42.000000 xuance-1.1.1/xuance/torch/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      424 2024-04-22 13:07:06.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8103 2024-05-06 03:04:25.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6860 2024-05-10 06:56:33.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8208 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8396 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7375 2024-05-06 03:05:42.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8971 2024-05-06 03:05:42.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8274 2024-05-06 03:05:42.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8065 2024-05-06 03:05:42.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6487 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6794 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7772 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6872 2024-05-10 08:55:15.000000 xuance-1.1.1/xuance/torch/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      296 2024-04-22 13:07:15.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6964 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7017 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6961 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8198 2024-05-06 03:28:10.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7045 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6999 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7442 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7023 2024-05-06 02:26:51.000000 xuance-1.1.1/xuance/torch/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1064 2024-04-22 13:00:21.000000 xuance-1.1.1/xuance/torch/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5139 2024-05-06 07:09:03.000000 xuance-1.1.1/xuance/torch/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      640 2024-04-22 13:02:22.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8825 2023-11-04 11:24:47.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11559 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3285 2024-05-09 03:44:34.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10383 2024-05-08 15:06:37.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6037 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4453 2024-05-08 09:47:54.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3597 2024-05-09 03:57:00.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10948 2024-05-09 02:39:43.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      710 2024-05-08 10:24:32.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3428 2024-05-09 13:17:26.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3290 2023-12-13 08:47:10.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3145 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6656 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5382 2023-12-14 13:10:44.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6290 2024-05-10 14:58:51.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6440 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10661 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      472 2024-04-22 13:01:54.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1887 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2053 2024-05-10 03:36:25.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 06:23:29.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2298 2023-12-14 06:01:04.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3555 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2681 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2416 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3194 2024-05-05 14:26:33.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3436 2024-05-05 14:29:30.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 07:59:27.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2587 2024-05-10 10:33:17.000000 xuance-1.1.1/xuance/torch/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      281 2024-04-22 13:02:07.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2256 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1881 2023-12-11 14:43:00.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1810 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2151 2023-10-20 05:41:15.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1818 2023-10-20 05:41:18.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1903 2023-10-20 05:41:17.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1907 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/torch/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/learners/ssl_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/torch/learners/ssl_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/torch/learners/ssl_rl/curl_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10505 2024-05-07 05:51:11.000000 xuance-1.1.1/xuance/torch/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12674 2024-05-05 14:36:23.000000 xuance-1.1.1/xuance/torch/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15470 2024-05-10 14:47:25.000000 xuance-1.1.1/xuance/torch/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3964 2023-12-18 12:16:47.000000 xuance-1.1.1/xuance/torch/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42059 2024-05-10 14:09:04.000000 xuance-1.1.1/xuance/torch/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    33217 2024-05-09 06:47:45.000000 xuance-1.1.1/xuance/torch/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13665 2024-05-05 13:04:50.000000 xuance-1.1.1/xuance/torch/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18493 2024-05-09 03:40:41.000000 xuance-1.1.1/xuance/torch/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6646 2023-11-04 15:22:56.000000 xuance-1.1.1/xuance/torch/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1268 2023-12-15 05:00:06.000000 xuance-1.1.1/xuance/torch/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4150 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/torch/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2029 2024-05-10 14:04:20.000000 xuance-1.1.1/xuance/torch/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3944 2023-10-20 05:41:16.000000 xuance-1.1.1/xuance/torch/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-02-22 11:27:05.000000 xuance-1.1.1/xuance/torch/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      372 2023-11-08 08:20:22.000000 xuance-1.1.1/xuance/torch/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7016 2024-05-01 15:10:48.000000 xuance-1.1.1/xuance/torch/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9455 2023-11-09 12:03:08.000000 xuance-1.1.1/xuance/torch/runners/runner_football.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      171 2024-01-18 07:00:38.000000 xuance-1.1.1/xuance/torch/runners/runner_magent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15974 2024-05-08 06:25:17.000000 xuance-1.1.1/xuance/torch/runners/runner_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21469 2024-05-01 14:34:22.000000 xuance-1.1.1/xuance/torch/runners/runner_pettingzoo.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21193 2024-05-01 10:46:01.000000 xuance-1.1.1/xuance/torch/runners/runner_sc2.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance/torch/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      974 2024-05-05 05:17:57.000000 xuance-1.1.1/xuance/torch/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4089 2024-05-07 07:42:06.000000 xuance-1.1.1/xuance/torch/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5748 2024-05-01 14:57:14.000000 xuance-1.1.1/xuance/torch/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4412 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/torch/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3847 2024-05-07 07:43:37.000000 xuance-1.1.1/xuance/torch/utils/operations.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3098 2023-10-20 05:39:12.000000 xuance-1.1.1/xuance/torch/utils/value_norm.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1748 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    31054 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/SOURCES.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/dependency_links.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      437 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/requires.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        7 2024-05-12 09:32:27.000000 xuance-1.1.1/xuance.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xuance-1.1.0/LICENSE.txt` & `xuance-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/README.md` & `xuance-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 ### [Classic Control](https://www.gymlibrary.dev/environments/classic_control/)
 
 <details open>
 <summary>(Click to hide)</summary>
 
 <table rules="none" align="center"><tr>
 <td> <center>
-<img src="./docs/source/figures/toy/cart_pole.gif" height=100" /><br/><font color="AAAAAA">CartPole</font>
+<img src="./docs/source/figures/toy/cart_pole.gif" height=100" /><br/><font color="AAAAAA">Cart Pole</font>
 </center></td>
 <td> <center>
 <img src="./docs/source/figures/toy/pendulum.gif" height=100" /> <br/> <font color="AAAAAA">Pendulum</font>
 </center> </td>
 <td> <center>
 <img src="./docs/source/figures/toy/acrobot.gif" height=100" /> <br/> <font color="AAAAAA">Acrobot</font>
 </center> </td>
@@ -157,21 +157,21 @@
 ### [Box2D](https://www.gymlibrary.dev/environments/box2d/)
 
 <details open>
 <summary>(Click to hide)</summary>
 
 <table rules="none" align="center"><tr>
 <td> <center>
-<img src="./docs/source/figures/box2d/bipedal_walker.gif" height=100" /><br/><font color="AAAAAA">CartPole</font>
+<img src="./docs/source/figures/box2d/bipedal_walker.gif" height=100" /><br/><font color="AAAAAA">Bipedal Walker</font>
 </center></td>
 <td> <center>
-<img src="./docs/source/figures/box2d/car_racing.gif" height=100" /> <br/> <font color="AAAAAA">Pendulum</font>
+<img src="./docs/source/figures/box2d/car_racing.gif" height=100" /> <br/> <font color="AAAAAA">Car Racing</font>
 </center> </td>
 <td> <center>
-<img src="./docs/source/figures/box2d/lunar_lander.gif" height=100" /> <br/> <font color="AAAAAA">Acrobot</font>
+<img src="./docs/source/figures/box2d/lunar_lander.gif" height=100" /> <br/> <font color="AAAAAA">Lunar Lander</font>
 </center> </td>
 </tr>
 </table>
 
 </details>
 
 ### [MuJoCo Environments](https://www.gymlibrary.dev/environments/mujoco/)
@@ -435,22 +435,22 @@
 You can put your questions, advices, or the bugs you have found in the [Issues](https://github.com/agi-brain/xuance/issues). 
 
 ### Social Accounts.
 
 Welcome to join the official communication group with QQ app (Group number: 552432695), and the official account ("玄策 RLlib") on WeChat.
 
 <details open>
-<summary>(QR code for QQ group and official account)</summary>
+<summary>(QR code for QQ group and WeChat official account)</summary>
 
 <table rules="none" align="center"><tr>
 <td> <center>
 <img src="docs/source/figures/QQ_group.jpeg" width="200" height="auto" /><br/><font color="AAAAAA">QQ group</font>
 </center></td>
 <td> <center>
-<img src="docs/source/figures/Official_Account.jpg" width="200" height="auto" /> <br/> <font color="AAAAAA">Official account</font>
+<img src="docs/source/figures/Official_Account.jpg" width="200" height="auto" /> <br/> <font color="AAAAAA">Official account (WeChat)</font>
 </center> </td>
 </tr>
 </table>
 
 </details>
 
 [@TFBestPractices](https://twitter.com/TFBestPractices/status/1665770204398223361)
```

### Comparing `xuance-1.1.0/setup.py` & `xuance-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                 "configs/*/*.yaml",
                 "configs/*/*/*.yaml",
                 "environment/magent2/libmagent.so",  # for magent2 environment on linux
                 "environment/magent2/magent.dll",  # for magent2 environment on Windows
                 "environment/magent2/libmagent.dylib"  # for magent2 environment on MacOS (for Intel CPU)
             ]
     },
-    version="1.1.0",
+    version="1.1.1",
     description='XuanCe: A Comprehensive and Unified Deep Reinforcement Learning Library.',
     long_description='XuanCe is an open-source ensemble of Deep Reinforcement Learning (DRL) algorithm implementations. We call it as Xuan-Ce (玄策) in Chinese. "Xuan (玄)" means incredible and magic box, "Ce (策)" means policy. DRL algorithms are sensitive to hyper-parameters tuning, varying in performance with different tricks, and suffering from unstable training processes, therefore, sometimes DRL algorithms seems elusive and "Xuan". This project gives a thorough, high-quality and easy-to-understand implementation of DRL algorithms, and hope this implementation can give a hint on the magics of reinforcement learning. We expect it to be compatible with multiple deep learning toolboxes( PyTorch, TensorFlow, and MindSpore), and hope it can really become a zoo full of DRL algorithms.',
     author='Wenzhang Liu, et al.',
     author_email='liu_wzh@foxmail.com',
     license='MIT',
     url='',
     download_url='https://github.com/agi-brain/xuance.git',
@@ -32,28 +32,27 @@
         'Programming Language :: Python :: 3.6',  # Specify which python versions that you want to support
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     extras_require={
-        "torch": ["torch==1.13.0"],  # default
+        "torch": ["torch==1.13.0"],
         "tensorflow": ["tensorflow==2.6.0"],
         "mindspore": ["mindspore==2.2.0"],
         "all": [
             "torch==1.13.0",
             "tensorflow==2.6.0",
             "mindspore==2.2.0"  # mindspore might be installed manually.
         ],
         "atari": ["atari-py==0.2.9",  # for Atari
                   "ale-py==0.7.5"],
         "box2d": ["box2d-py==2.3.5"],  # for box2d
     },
     install_requires=[
-        "torch==1.13.0",
         "numpy>=1.21.6",
         "scipy==1.7.3",
         "PyYAML",  # default version is 6.0
         "gym==0.26.2",
         "gymnasium==0.28.1",
         "gym-notices==0.0.8",
         "pygame==2.1.0",
```

### Comparing `xuance-1.1.0/xuance/common/common_tools.py` & `xuance-1.1.1/xuance/common/common_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                 raise RuntimeError(f"The environment named '{args.env}' is currently not supported for {args.method}.")
             else:
                 print("Failed to load arguments for the implementation!")
 
         print("Algorithm:", args.agent)
         print("Environment:", args.env_name)
         print("Scenario:", args.env_id)
-        runner = run_REGISTRY[args[0].runner](args) if type(args) == list else run_REGISTRY[args.runner](args)
+        runner = run_REGISTRY[args.runner](args)
         return runner
 
 
 def create_directory(path):
     """Create an empty directory.
     Args:
         path: the path of the directory
```

### Comparing `xuance-1.1.0/xuance/common/memory_tools.py` & `xuance-1.1.1/xuance/common/memory_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,32 +162,33 @@
     Replay buffer for on-policy DRL algorithms.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
+        horizon_size: max length of steps to store for one environment.
         use_gae: if use GAE trick.
         use_advnorm: if use Advantage normalization trick.
         gamma: discount factor.
         gae_lam: gae lambda.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 horizon_size: int,
                  use_gae: bool = True,
                  use_advnorm: bool = True,
                  gamma: float = 0.99,
                  gae_lam: float = 0.95):
         super(DummyOnPolicyBuffer, self).__init__(observation_space, action_space, auxiliary_shape)
-        self.n_envs, self.n_size = n_envs, n_size
+        self.n_envs, self.horizon_size = n_envs, horizon_size
+        self.n_size = self.horizon_size
         self.buffer_size = self.n_size * self.n_envs
         self.use_gae, self.use_advnorm = use_gae, use_advnorm
         self.gamma, self.gae_lam = gamma, gae_lam
         self.start_ids = np.zeros(self.n_envs, np.int64)
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size)
         self.actions = create_memory(space2shape(self.action_space), self.n_envs, self.n_size)
         self.rewards = create_memory((), self.n_envs, self.n_size)
@@ -269,32 +270,32 @@
     Replay buffer for on-policy DRL algorithms and Atari tasks.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
+        horizon_size: max length of steps to store for one environment.
         use_gae: if use GAE trick.
         use_advnorm: if use Advantage normalization trick.
         gamma: discount factor.
         gae_lam: gae lambda.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 horizon_size: int,
                  use_gae: bool = True,
                  use_advnorm: bool = True,
                  gamma: float = 0.99,
                  gae_lam: float = 0.95):
         super(DummyOnPolicyBuffer_Atari, self).__init__(observation_space, action_space, auxiliary_shape,
-                                                        n_envs, n_size, use_gae, use_advnorm, gamma, gae_lam)
+                                                        n_envs, horizon_size, use_gae, use_advnorm, gamma, gae_lam)
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
 
     def clear(self):
         self.ptr, self.size = 0, 0
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
         self.actions = create_memory(space2shape(self.action_space), self.n_envs, self.n_size)
         self.auxiliary_infos = create_memory(self.auxiliary_shape, self.n_envs, self.n_size)
@@ -308,26 +309,27 @@
     Replay buffer for off-policy DRL algorithms.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
-        batch_size: batch size of transition data for a sample.
+        buffer_size: the total size of the replay buffer.
+        batch_size: size of transition data for a batch of sample.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 buffer_size: int,
                  batch_size: int):
         super(DummyOffPolicyBuffer, self).__init__(observation_space, action_space, auxiliary_shape)
-        self.n_envs, self.n_size, self.batch_size = n_envs, n_size, batch_size
+        self.n_envs, self.batch_size = n_envs, batch_size
+        self.n_size = buffer_size // self.n_envs
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size)
         self.next_observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size)
         self.actions = create_memory(space2shape(self.action_space), self.n_envs, self.n_size)
         self.auxiliary_infos = create_memory(self.auxiliary_shape, self.n_envs, self.n_size)
         self.rewards = create_memory((), self.n_envs, self.n_size)
         self.terminals = create_memory((), self.n_envs, self.n_size)
 
@@ -363,30 +365,31 @@
     Replay buffer for DRQN-based algorithms.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
+        buffer_size: the size of replay buffer that stores episodes of data.
         batch_size: batch size of transition data for a sample.
         episode_length: data length for an episode.
         lookup_length: the length of history data.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 buffer_size: int,
                  batch_size: int,
                  episode_length: int,
                  lookup_length: int):
         super(RecurrentOffPolicyBuffer, self).__init__(observation_space, action_space, auxiliary_shape)
-        self.n_envs, self.n_size, self.episode_length, self.batch_size = n_envs, n_size, episode_length, batch_size
+        self.n_envs, self.buffer_size, self.episode_length, self.batch_size = n_envs, buffer_size, episode_length, batch_size
+        self.n_size = self.buffer_size // self.n_envs
         self.lookup_length = lookup_length
         self.memory = deque(maxlen=self.n_size)
 
     @property
     def full(self):
         return self.size >= self.n_size
 
@@ -433,28 +436,29 @@
     Prioritized Replay Buffer.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
+        buffer_size: the total size of the replay buffer.
         batch_size: batch size of transition data for a sample.
         alpha: prioritized factor.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 buffer_size: int,
                  batch_size: int,
                  alpha: float = 0.6):
         super(PerOffPolicyBuffer, self).__init__(observation_space, action_space, auxiliary_shape)
-        self.n_envs, self.n_size, self.batch_size = n_envs, n_size, batch_size
+        self.n_envs, self.batch_size = n_envs, batch_size
+        self.n_size = buffer_size // self.n_envs
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size)
         self.next_observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size)
         self.actions = create_memory(space2shape(self.action_space), self.n_envs, self.n_size)
         self.rewards = create_memory((), self.n_envs, self.n_size)
         self.terminals = create_memory((), self.n_envs, self.n_size)
 
         self._alpha = alpha
@@ -561,26 +565,26 @@
     Replay buffer for off-policy DRL algorithms and Atari tasks.
 
     Args:
         observation_space: the observation space of the environment.
         action_space: the action space of the environment.
         auxiliary_shape: data shape of auxiliary information (if exists).
         n_envs: number of parallel environments.
-        n_size: max length of steps to store for one environment.
+        buffer_size: the total size of the replay buffer.
         batch_size: batch size of transition data for a sample.
     """
     def __init__(self,
                  observation_space: Space,
                  action_space: Space,
                  auxiliary_shape: Optional[dict],
                  n_envs: int,
-                 n_size: int,
+                 buffer_size: int,
                  batch_size: int):
         super(DummyOffPolicyBuffer_Atari, self).__init__(observation_space, action_space, auxiliary_shape,
-                                                         n_envs, n_size, batch_size)
+                                                         n_envs, buffer_size, batch_size)
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
         self.next_observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
 
     def clear(self):
         self.observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
         self.next_observations = create_memory(space2shape(self.observation_space), self.n_envs, self.n_size, np.uint8)
         self.actions = create_memory(space2shape(self.action_space), self.n_envs, self.n_size)
```

### Comparing `xuance-1.1.0/xuance/common/memory_tools_marl.py` & `xuance-1.1.1/xuance/common/memory_tools_marl.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         n_agents: number of agents.
         state_space: global state space, type: Discrete, Box.
         obs_space: observation space for one agent (suppose same obs space for group agents).
         act_space: action space for one agent (suppose same actions space for group agents).
         rew_space: reward space.
         done_space: terminal variable space.
         n_envs: number of parallel environments.
-        buffer_size: buffer size of transition data for one environment.
+        buffer_size: buffer size of total experience data.
         use_gae: whether to use GAE trick.
         use_advnorm: whether to use Advantage normalization trick.
         gamma: discount factor.
         gae_lam: gae lambda.
     """
 
     def __init__(self, n_agents, state_space, obs_space, act_space, rew_space, done_space, n_envs, buffer_size,
@@ -159,15 +159,15 @@
         n_agents: number of agents.
         state_space: global state space, type: Discrete, Box.
         obs_space: observation space for one agent (suppose same obs space for group agents).
         act_space: action space for one agent (suppose same actions space for group agents).
         rew_space: reward space.
         done_space: terminal variable space.
         n_envs: number of parallel environments.
-        buffer_size: buffer size of trajectory data for one environment.
+        buffer_size: buffer size of total experience data.
         use_gae: whether to use GAE trick.
         use_advnorm: whether to use Advantage normalization trick.
         gamma: discount factor.
         gae_lam: gae lambda.
         max_episode_length: maximum length of data for one episode trajectory.
     """
 
@@ -524,15 +524,15 @@
         n_agents: number of agents.
         state_space: global state space, type: Discrete, Box.
         obs_space: observation space for one agent (suppose same obs space for group agents).
         act_space: action space for one agent (suppose same actions space for group agents).
         rew_space: reward space.
         done_space: terminal variable space.
         n_envs: number of parallel environments.
-        buffer_size: buffer size for one environment.
+        buffer_size: buffer size of total experience data.
         batch_size: batch size of transition data for a sample.
         **kwargs: other arguments.
     """
 
     def __init__(self, n_agents, state_space, obs_space, act_space, rew_space, done_space,
                  n_envs, buffer_size, batch_size, **kwargs):
         super(MARL_OffPolicyBuffer, self).__init__(n_agents, state_space, obs_space, act_space, rew_space, done_space,
@@ -582,15 +582,15 @@
         n_agents: number of agents.
         state_space: global state space, type: Discrete, Box.
         obs_space: observation space for one agent (suppose same obs space for group agents).
         act_space: action space for one agent (suppose same actions space for group agents).
         rew_space: reward space.
         done_space: terminal variable space.
         n_envs: number of parallel environments.
-        buffer_size: buffer size for one environment.
+        buffer_size: buffer size of total experience data.
         batch_size: batch size of episodes for a sample.
         kwargs: other arguments.
     """
 
     def __init__(self, n_agents, state_space, obs_space, act_space, rew_space, done_space,
                  n_envs, buffer_size, batch_size, **kwargs):
         self.max_eps_len = kwargs['max_episode_length']
@@ -669,15 +669,15 @@
         state_space: global state space, type: Discrete, Box.
         obs_space: observation space for one agent (suppose same obs space for group agents).
         act_space: action space for one agent (suppose same actions space for group agents).
         prob_shape: the data shape of the action probabilities.
         rew_space: reward space.
         done_space: terminal variable space.
         n_envs: number of parallel environments.
-        buffer_size: buffer size for one environment.
+        buffer_size: buffer size of total experience data.
         batch_size: batch size of transition data for a sample.
     """
 
     def __init__(self, n_agents, state_space, obs_space, act_space, prob_shape, rew_space, done_space,
                  n_envs, buffer_size, batch_size):
         self.prob_shape = prob_shape
         super(MeanField_OffPolicyBuffer, self).__init__(n_agents, state_space, obs_space, act_space, rew_space,
```

### Comparing `xuance-1.1.0/xuance/common/segtree_tool.py` & `xuance-1.1.1/xuance/common/segtree_tool.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/common/statistic_tools.py` & `xuance-1.1.1/xuance/common/statistic_tools.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/__init__.py` & `xuance-1.1.1/xuance/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/a2c/atari.yaml` & `xuance-1.1.1/xuance/configs/a2c/atari.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 actor_hidden_size: [128, 128]
 critic_hidden_size: [128, 128]
 activation: "leaky_relu"
 
 seed: 1
 parallels: 5
 running_steps: 10000000  # 10M
-n_steps: 256  #
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.  #
 n_epoch: 4
 n_minibatch: 8
 learning_rate: 0.0007
 
 vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.2
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 critic_hidden_size: [64,]
 activation: 'leaky_relu'
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 1000000
-n_steps: 128
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 5
 learning_rate: 0.0004
 
 vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/a2c/classic_control/MountainCar-v0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 agent: "A2C"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
 activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 128
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
+n_minibatch: 1
 learning_rate: 0.0004
 
 vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/a2c/mujoco.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 agent: "A2C"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
-policy: "Categorical_AC"
+policy: "Gaussian_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: 'leaky_relu'
+activation: "leaky_relu"
+activation_action: 'tanh'
 
-seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 128
+seed: 6782
+parallels: 16
+running_steps: 1000000  # 1M
+horizon_size: 16  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
 n_minibatch: 1
-learning_rate: 0.0004
+learning_rate: 0.0007
 
 vf_coef: 0.25
-ent_coef: 0.01
+ent_coef: 0.0
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.98
+gamma: 0.99
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 3
+eval_interval: 5000
+test_episode: 5
 log_dir: "./logs/a2c/"
 model_dir: "./models/a2c/"
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/pg/classic_control/MountainCar-v0.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "A2C"
+agent: "PG"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
-vectorize: "Subproc_Gym"
-policy: "Categorical_AC"
+env_id: "MountainCar-v0"
 representation: "Basic_MLP"
+vectorize: "Dummy_Gym"
+policy: "Categorical_Actor"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: 'leaky_relu'
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 128
-n_epoch: 1
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 3
 n_minibatch: 1
 learning_rate: 0.0004
 
-vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
-use_gae: True
+use_gae: False
 gae_lambda: 0.95
-use_advnorm: True
+use_advnorm: False
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/a2c/"
-model_dir: "./models/a2c/"
+test_episode: 1
+log_dir: "./logs/pg/"
+model_dir: "./models/pg/"
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/ppg/classic_control/Acrobot-v1.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-agent: "A2C"
+agent: "PPG"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Categorical_AC"
 representation: "Basic_MLP"
+policy: "Categorical_PPG"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: 'leaky_relu'
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
+activation: "leaky_relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 128
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
+policy_nepoch: 4
+value_nepoch: 8 
+aux_nepoch: 8
 n_minibatch: 1
-learning_rate: 0.0004
+learning_rate: 0.001
 
-vf_coef: 0.25
 ent_coef: 0.01
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
+clip_range: 0.2
+kl_beta: 1.0
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/a2c/"
-model_dir: "./models/a2c/"
+test_episode: 1
+log_dir: "./logs/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/a2c/classic_control/Acrobot-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 agent: "A2C"
 env_name: "Classic Control"
-env_id: "Pendulum-v1"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_AC"
+policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
 activation: 'leaky_relu'
-activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-running_steps: 500000
-n_steps: 64
-n_epoch: 1
-n_minibatch: 1
+running_steps: 300000
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 8
+n_minibatch: 8
 learning_rate: 0.0004
 
 vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
```

### Comparing `xuance-1.1.0/xuance/configs/a2c/mujoco.yaml` & `xuance-1.1.1/xuance/configs/a2c/box2d/LunarLander-v2.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 agent: "A2C"
-env_name: "MuJoCo"
-env_id: "Ant-v4"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_AC"
+policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "leaky_relu"
-activation_action: 'tanh'
+activation: 'leaky_relu'
 
-seed: 6782
-parallels: 16
-running_steps: 1000000  # 1M
-n_steps: 16
+seed: 1
+parallels: 10
+running_steps: 300000
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
-n_minibatch: 1
-learning_rate: 0.0007
+learning_rate: 0.0004
 
 vf_coef: 0.25
-ent_coef: 0.0
+ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.99
+gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 5000
-test_episode: 5
+eval_interval: 50000
+test_episode: 3
 log_dir: "./logs/a2c/"
 model_dir: "./models/a2c/"
```

### Comparing `xuance-1.1.0/xuance/configs/c51/atari.yaml` & `xuance-1.1.1/xuance/configs/dqn/atari.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-agent: "C51DQN"
+agent: "DQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
 noop_max: 30  # Do no-op action for a number of steps in [1, noop_max].
-policy: "C51_Q_network"
+policy: "Basic_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
+buffer_size: 500000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
-vmin: 0
-vmax: 200
-atom_num: 51
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
 training_frequency: 1
 running_steps: 50000000  # 50M
@@ -40,10 +37,10 @@
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 500000
-test_episode: 3
-log_dir: "./logs/c51/"
-model_dir: "./models/c51/"
+test_episode: 5
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/c51/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/c51/box2d/CarRacing-v2.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 vmin: 0
 vmax: 200
 atom_num: 51
```

### Comparing `xuance-1.1.0/xuance/configs/c51/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/c51/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 vmin: 0
 vmax: 200
 atom_num: 51
```

### Comparing `xuance-1.1.0/xuance/configs/c51/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "C51DQN"
+agent: "QRDQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "C51_Q_network"
+policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
-vmin: 0
-vmax: 200
-atom_num: 51
+quantile_num: 20
 
-start_greedy: 0.5
+start_greedy: 0.25
 end_greedy: 0.01
-decay_step_greedy: 10000
+decay_step_greedy: 30000
 sync_frequency: 100
 training_frequency: 1
 running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/c51/"
-model_dir: "./models/c51/"
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/c51/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "C51DQN"
+agent: "QRDQN"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
-policy: "C51_Q_network"
+policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
-vmin: 0
-vmax: 200
-atom_num: 51
+quantile_num: 20
 
-start_greedy: 0.5
+start_greedy: 0.25
 end_greedy: 0.01
-decay_step_greedy: 10000
+decay_step_greedy: 30000
 sync_frequency: 100
 training_frequency: 1
-running_steps: 200000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/c51/"
-model_dir: "./models/c51/"
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/c51/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/c51/classic_control/MountainCar-v0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 vmin: 0
 vmax: 200
 atom_num: 51
```

### Comparing `xuance-1.1.0/xuance/configs/coma/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/coma/mpe/simple_spread_v3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 actor_hidden_size: [128, ]
 critic_hidden_size: [128, ]
 activation: "relu"
 
 seed: 1
 parallels: 10
-n_size: 250
+buffer_size: 250
 n_epoch: 10
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/1c3s5z.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/25m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/2m_vs_1z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/2s3z.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/3m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/5m_vs_6m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/8m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/8m_vs_9m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/MMM2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/coma/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/coma/sc2/corridor.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
 learning_rate_critic: 0.0007
 
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.1.0/xuance/configs/dcg/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/dcg/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/1c3s5z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/25m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/2s3z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/3m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/5m_vs_6m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/8m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/8m_vs_9m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/MMM2.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/dcg/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/dcg/sc2/corridor.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 agent: "DDPG"
-env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+env_name: "Classic Control"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
 policy: "DDPG_Policy"
-representation: "Basic_Identical"
+representation: "Basic_MLP"
 runner: "DRL"
 
+representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
 activation: "relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-n_size: 200000
+buffer_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
 gamma: 0.98
 tau: 0.005
-learning_rate: 0.0007
 
 start_noise: 0.1
 end_noise: 0.1
 training_frequency: 1
 running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
+test_episode: 3
 log_dir: "./logs/ddpg/"
 model_dir: "./models/ddpg/"
```

### Comparing `xuance-1.1.0/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/td3/classic_control/Pendulum-v1.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-agent: "DDPG"
+agent: "TD3"
 env_name: "Classic Control"
 env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "DDPG_Policy"
-representation: "Basic_MLP"
+representation: "Basic_Identical"
+policy: "TD3_Policy"
 runner: "DRL"
 
 representation_hidden_size: [64]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: "relu"
+actor_hidden_size: [256, ]
+critic_hidden_size: [256, ]
+activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-n_size: 200000
+buffer_size: 200000
 batch_size: 256
-actor_learning_rate: 0.001
+actor_learning_rate: 0.0005
 critic_learning_rate: 0.001
 gamma: 0.98
 tau: 0.005
-learning_rate: 0.0007
+actor_update_delay: 3
 
-start_noise: 0.1
-end_noise: 0.1
-training_frequency: 1
+start_noise: 0.25
+end_noise: 0.05
+training_frequency: 2
 running_steps: 500000
-start_training: 1000
+start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/ddpg/"
-model_dir: "./models/ddpg/"
+test_episode: 1
+log_dir: "./logs/td3/"
+model_dir: "./models/td3/"
```

### Comparing `xuance-1.1.0/xuance/configs/ddpg/drones.yaml` & `xuance-1.1.1/xuance/configs/ddpg/drones.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-n_size: 1000000  # buffer
+buffer_size: 1000000  # buffer
 batch_size: 1024
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
 
 start_noise: 0.1
```

### Comparing `xuance-1.1.0/xuance/configs/ddpg/mujoco.yaml` & `xuance-1.1.1/xuance/configs/ddpg/mujoco.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 actor_hidden_size: [400, 300]
 critic_hidden_size: [400, 300]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 19089
 parallels: 4  # number of environments
-n_size: 50000  # replay buffer size
+buffer_size: 200000  # replay buffer size
 batch_size: 100
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
 
 start_noise: 0.5
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/atari.yaml` & `xuance-1.1.1/xuance/configs/perdqn/atari.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DDQN"
+agent: "PerDQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -17,16 +17,16 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
-batch_size: 32
+buffer_size: 500000
+batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
@@ -35,12 +35,15 @@
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
+PER_alpha: 0.5
+PER_beta0: 0.4
+
 test_steps: 10000
 eval_interval: 500000
-test_episode: 3
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
+test_episode: 1
+log_dir: "./logs/perdqn/"
+model_dir: "./models/perdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/dqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DDQN"
+agent: "DQN"
 env_name: "Box2D"
 env_id: "CarRacing-v2"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
@@ -12,15 +12,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
@@ -33,9 +33,9 @@
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 100000
 test_episode: 1
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/ddqn/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 100000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/ddqn/classic_control/CartPole-v1.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/dqn/classic_control/CartPole-v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-agent: "DDQN"
+agent: "DQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 128
+buffer_size: 100000
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
-sync_frequency: 100
+sync_frequency: 50
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000  # 200k
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 1
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
-
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/atari.yaml` & `xuance-1.1.1/xuance/configs/ddqn/atari.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DQN"
+agent: "DDQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -17,16 +17,16 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
-batch_size: 32  # 64
+buffer_size: 500000
+batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
@@ -37,10 +37,10 @@
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 500000
-test_episode: 5
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+test_episode: 3
+log_dir: "./logs/ddqn/"
+model_dir: "./models/ddqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/ddqn/box2d/CarRacing-v2.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DQN"
+agent: "DDQN"
 env_name: "Box2D"
 env_id: "CarRacing-v2"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
@@ -12,15 +12,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
@@ -33,9 +33,9 @@
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 100000
 test_episode: 1
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+log_dir: "./logs/ddqn/"
+model_dir: "./models/ddqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/dqn/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 100000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/dqn/classic_control/MountainCar-v0.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 agent: "DQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'relu'
+representation_hidden_size: [256, ]
+q_hidden_size: [256, ]
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 200000
 batch_size: 256
-learning_rate: 0.001
+learning_rate: 0.1
 gamma: 0.99
 
-start_greedy: 0.5
+start_greedy: 1.0
 end_greedy: 0.01
-decay_step_greedy: 10000
-sync_frequency: 50
-training_frequency: 1
-running_steps: 200000  # 200k
+sync_frequency: 200
+training_frequency: 2
+running_steps: 2000000  # 2M
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 20000
-test_episode: 1
+eval_interval: 50000
+test_episode: 5
 log_dir: "./logs/dqn/"
 model_dir: "./models/dqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/perdqn/classic_control/CartPole-v1.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-agent: "DQN"
+agent: "PerDQN"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
-batch_size: 256
+buffer_size: 200000
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
-end_greedy: 0.01
-decay_step_greedy: 10000
-sync_frequency: 50
-training_frequency: 1
-running_steps: 200000  # 200k
+end_greedy: 0.1
+decay_step_greedy: 20000
+sync_frequency: 100
+training_frequency: 4
+running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
+PER_alpha: 0.5
+PER_beta0: 0.4
+
 test_steps: 10000
-eval_interval: 20000
+eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+log_dir: "./logs/perdqn/"
+model_dir: "./models/perdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-agent: "DQN"
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
+agent: "DDPG"
+env_name: "Box2D"
+env_id: "BipedalWalker-v3"
 vectorize: "Dummy_Gym"
-policy: "Basic_Q_network"
-representation: "Basic_MLP"
+representation: "Basic_Identical"
+policy: "DDPG_Policy"
 runner: "DRL"
 
-representation_hidden_size: [256, ]
-q_hidden_size: [256, ]
-activation: 'leaky_relu'
+representation_hidden_size:
+actor_hidden_size: [256, 256]
+critic_hidden_size: [256, 256]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-n_size: 20000
+parallels: 10  # number of environments
+buffer_size: 200000
 batch_size: 256
-learning_rate: 0.1
+actor_learning_rate: 0.001
+critic_learning_rate: 0.001
 gamma: 0.99
+tau: 0.005
 
-start_greedy: 1.0
-end_greedy: 0.01
-sync_frequency: 200
-training_frequency: 2
-running_steps: 2000000  # 2M
+start_noise: 0.5
+end_noise: 0.1
+training_frequency: 1
+running_steps: 2000000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 5
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+log_dir: "./logs/ddpg/"
+model_dir: "./models/ddpg/"
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/atari.yaml` & `xuance-1.1.1/xuance/configs/drqn/atari.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 recurrent_hidden_size: 512
 recurrent_layer_N: 1
 dropout: 0
 activation: 'relu'
 
 seed: 1
 parallels: 5
-n_size: 1000
+buffer_size: 5000
 batch_size: 8  # batch size for training
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/drqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 recurrent_hidden_size: 512
 recurrent_layer_N: 1
 dropout: 0
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 100
+buffer_size: 200
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/drqn/box2d/LunarLander-v2.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 50  # memory size for each parallel
+buffer_size: 500
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 5000
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/drqn/classic_control/MountainCar-v0.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 agent: "DRQN"  # deep recurrent Q-networks
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "DRQN_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
 rnn: "LSTM"
 
 representation_hidden_size: [128,]
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000  # memory size for each parallel
+buffer_size: 100000  # memory size for each parallel
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/drqn/classic_control/CartPole-v1.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000  # memory size for each parallel
+buffer_size: 100000
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
```

### Comparing `xuance-1.1.0/xuance/configs/drqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "DRQN"  # deep recurrent Q-networks
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
+agent: "QRDQN"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "DRQN_Policy"
+policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
-rnn: "LSTM"
 
 representation_hidden_size: [128,]
-recurrent_hidden_size: 128
-recurrent_layer_N: 1
-dropout: 0
+q_hidden_size: [128,]
 activation: 'relu'
 
+seed: 1
 parallels: 10
-n_size: 10000  # memory size for each parallel
-batch_size: 8  # batch size for training
+buffer_size: 100000
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
+quantile_num: 20
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
 sync_frequency: 50
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000
 start_training: 1000
-lookup_length: 50
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/drqn/"
-model_dir: "./models/drqn/"
+test_episode: 1
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/atari.yaml` & `xuance-1.1.1/xuance/configs/dueldqn/atari.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
+buffer_size: 500000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-agent: "Duel_DQN"
+agent: "QRDQN"
 env_name: "Box2D"
 env_id: "CarRacing-v2"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "QR_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
+quantile_num: 20
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
 sync_frequency: 500
 training_frequency: 1
 running_steps: 2000000
@@ -33,9 +34,9 @@
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 100000
 test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/c51/classic_control/Acrobot-v1.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-agent: "Duel_DQN"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+agent: "C51DQN"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "C51_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128, ]
-q_hidden_size: [128, ]
+representation_hidden_size: [128,]
+q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
+vmin: 0
+vmax: 200
+atom_num: 51
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 20000
-sync_frequency: 50
+decay_step_greedy: 10000
+sync_frequency: 100
 training_frequency: 1
-running_steps: 500000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+log_dir: "./logs/c51/"
+model_dir: "./models/c51/"
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-agent: "Duel_DQN"
+agent: "PerDQN"
 env_name: "Classic Control"
 env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128, ]
-q_hidden_size: [128, ]
+representation_hidden_size: [128,]
+q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
-batch_size: 256
+buffer_size: 200000
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
-end_greedy: 0.01
+end_greedy: 0.1
 decay_step_greedy: 20000
-sync_frequency: 50
-training_frequency: 1
+sync_frequency: 100
+training_frequency: 4
 running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
+PER_alpha: 0.5
+PER_beta0: 0.4
+
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+log_dir: "./logs/perdqn/"
+model_dir: "./models/perdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agent: "Duel_DQN"
-env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
 policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 100000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 20000
```

### Comparing `xuance-1.1.0/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 100000
 batch_size: 256
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 20000
```

### Comparing `xuance-1.1.0/xuance/configs/iddpg/drones.yaml` & `xuance-1.1.1/xuance/configs/iddpg/drones.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/iddpg/mpe/simple_push_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/iddpg/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/ippo/football/3v1.yaml` & `xuance-1.1.1/xuance/configs/ippo/football/3v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "relu"
 
 seed: 1
 parallels: 50
-n_size: 400
+buffer_size: 400
 n_epoch: 15
 n_minibatch: 2
 learning_rate: 5.0e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/ippo/mpe/simple_spread_v3.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 env_id: "simple_spread_v3"
 continuous_action: True
 policy: "Gaussian_MAAC_Policy"
 representation: "Basic_MLP"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
+# recurrent settings for Basic_RNN representation
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
 activation: "relu"
 activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
-n_size: 3200
+buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
 weight_decay: 0
 
 vf_coef: 0.5
 ent_coef: 0.01
@@ -36,15 +37,15 @@
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace merged observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
-use_value_norm: True  # use running mean and std to normalize rewards.
+use_value_norm: False  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True
 use_gae: True
 gae_lambda: 0.95
 
 start_training: 1
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/1c3s5z.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/25m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/2m_vs_1z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/2s3z.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/8m.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "8m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
+on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
@@ -21,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
@@ -50,14 +51,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000
+running_steps: 1000000  # 1M
 training_frequency: 1
 
 eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/ippo/"
 model_dir: "./models/ippo/"
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/5m_vs_6m.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/8m_vs_9m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "8m_vs_9m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -22,43 +22,43 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.2
+clip_range: 0.05
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.2
+value_clip_range: 0.05
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/ippo/"
 model_dir: "./models/ippo/"
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/corridor.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "8m_vs_9m"
+env_id: "corridor"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -22,35 +22,35 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 15
+buffer_size: 128
+n_epoch: 5
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.05
+clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.05
+value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/MMM2.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 5
 n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/ippo/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/corridor.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "IPPO"
+agent: "MAPPO"
 env_name: "StarCraft2"
 env_id: "corridor"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 5
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
@@ -38,15 +38,15 @@
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: False  # if use global state to replace joint observations
+use_global_state: True  # if use global state to calculate values
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -56,9 +56,9 @@
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/ippo/"
-model_dir: "./models/ippo/"
+log_dir: "./logs/mappo/"
+model_dir: "./models/mappo/"
```

### Comparing `xuance-1.1.0/xuance/configs/iql/football/3v1.yaml` & `xuance-1.1.1/xuance/configs/iql/football/3v1.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml` & `xuance-1.1.1/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/iql/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/1c3s5z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/25m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/2s3z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/3m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/5m_vs_6m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/8m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/8m_vs_9m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/MMM2.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/iql/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/iql/sc2/corridor.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/isac/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/isac/mpe/simple_adversary_v3.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/isac/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/isac/mpe/simple_push_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/isac/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/isac/mpe/simple_spread_v3.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/maddpg/drones.yaml` & `xuance-1.1.1/xuance/configs/maddpg/drones.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/maddpg/mpe/simple_push_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/maddpg/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/maddpg/new_env_mas.yaml` & `xuance-1.1.1/xuance/configs/maddpg/new_env_mas.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/mappo/football/1v1.yaml` & `xuance-1.1.1/xuance/configs/mappo/football/1v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "relu"
 
 seed: 1
 parallels: 50
-n_size: 100
+buffer_size: 100
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 5.0e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/football/3v1.yaml` & `xuance-1.1.1/xuance/configs/mappo/football/3v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "relu"
 
 seed: 1
 parallels: 50
-n_size: 400
+buffer_size: 400
 n_epoch: 15
 n_minibatch: 2
 learning_rate: 5.0e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/mappo/mpe/simple_adversary_v3.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
 activation: "relu"
 activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
-n_size: 3200
+buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
 weight_decay: 0
 
 vf_coef: 0.5
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/mappo/mpe/simple_push_v3.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
 activation: "relu"
 activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
-n_size: 3200
+buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
 weight_decay: 0
 
 vf_coef: 0.5
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/mappo/mpe/simple_spread_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
-actor_hidden_size: [64, 64]
-critic_hidden_size: [64, 64]
+actor_hidden_size: [64, ]
+critic_hidden_size: [256, ]
 activation: "relu"
 activation_action: "sigmoid"
 
 seed: 1
-parallels: 8  # 128
-n_size: 3200
+parallels: 128
+buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
 weight_decay: 0
 
 vf_coef: 0.5
 ent_coef: 0.01
@@ -37,15 +37,15 @@
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace merged observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
-use_value_norm: True  # use running mean and std to normalize rewards.
+use_value_norm: False  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True
 use_gae: True
 gae_lambda: 0.95
 
 start_training: 1
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/25m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/2m_vs_1z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/8m.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 agent: "MAPPO"
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "8m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
+on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
@@ -21,15 +22,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
@@ -50,14 +51,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 2000000
+running_steps: 1000000  # 1M
 training_frequency: 1
 
-eval_interval: 20000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/mappo/"
 model_dir: "./models/mappo/"
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/MMM2.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 agent: "MAPPO"
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "MMM2"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
+on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 0.01
+gain: 1.0
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 15
-n_minibatch: 1
+buffer_size: 128
+n_epoch: 5
+n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -50,14 +51,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000
+running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/mappo/"
 model_dir: "./models/mappo/"
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/5m_vs_6m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/2s3z.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 agent: "MAPPO"
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "2s3z"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
-on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
@@ -22,15 +21,15 @@
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
@@ -51,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000  # 1M
+running_steps: 2000000
 training_frequency: 1
 
-eval_interval: 10000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/mappo/"
 model_dir: "./models/mappo/"
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/8m_vs_9m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
+buffer_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/mappo/sc2/3m.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 agent: "MAPPO"
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "3m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
-on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 1.0
+gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 5
-n_minibatch: 2
+buffer_size: 128
+n_epoch: 15
+n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -51,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000  # 10M
+running_steps: 1000000
 training_frequency: 1
 
-eval_interval: 100000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/mappo/"
 model_dir: "./models/mappo/"
```

### Comparing `xuance-1.1.0/xuance/configs/mappo/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/corridor.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-agent: "MAPPO"
+agent: "VDAC"
 env_name: "StarCraft2"
 env_id: "corridor"
 fps: 15
-policy: "Categorical_MAAC_Policy"
+policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, 64, 64]
+fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
+mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
+hidden_dim_mixing_net: 32  # hidden units of mixing network
+hidden_dim_hyper_net: 64  # hidden units of hyper network
+
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 5
+buffer_size: 8
+n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: True  # if use global state to calculate values
+use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -54,11 +58,11 @@
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 100000
+eval_interval: 50000
 test_episode: 16
-log_dir: "./logs/mappo/"
-model_dir: "./models/mappo/"
+log_dir: "./logs/vdac/"
+model_dir: "./models/vdac/"
```

### Comparing `xuance-1.1.0/xuance/configs/masac/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/masac/mpe/simple_adversary_v3.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/masac/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/masac/mpe/simple_push_v3.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/masac/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/masac/mpe/simple_spread_v3.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
 alpha: 0.01
+use_automatic_entropy_tuning: True
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1  # random noise for continuous actions
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/matd3/mpe/simple_adversary_v3.yaml` & `xuance-1.1.1/xuance/configs/matd3/mpe/simple_adversary_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/matd3/mpe/simple_push_v3.yaml` & `xuance-1.1.1/xuance/configs/matd3/mpe/simple_push_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/matd3/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/matd3/mpe/simple_spread_v3.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
+delay: 3
 
 start_noise: 1.0
 end_noise: 0.01
 sigma: 0.1
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
```

### Comparing `xuance-1.1.0/xuance/configs/mfac/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/mfac/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml` & `xuance-1.1.1/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/mfq/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/mfq/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/mpdqn/Platform.yaml` & `xuance-1.1.1/xuance/configs/mpdqn/Platform.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
 activation: "relu"
 activation_action: 'tanh'
 
-n_size: 20000
+buffer_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
 
 start_greedy: 0.5
 end_greedy: 0.05
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/atari.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/atari.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
+buffer_size: 500000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_greedy: 1000000  # 1M
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_noise: 200000
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_noise: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_noise: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_noise: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_noise: 0.05
 end_noise: 0.0
 decay_step_noise: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/pdqn/Platform.yaml` & `xuance-1.1.1/xuance/configs/pdqn/Platform.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
 activation: "relu"
 activation_action: 'tanh'
 
-n_size: 20000
+buffer_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
 
 start_greedy: 0.5
 end_greedy: 0.05
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/atari.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/atari.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-agent: "PerDQN"
+agent: "QRDQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
 noop_max: 30  # Do no-op action for a number of steps in [1, noop_max].
-policy: "Basic_Q_network"
+policy: "QR_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
 activation: "relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
+buffer_size: 500000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
+quantile_num: 20
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
 training_frequency: 1
 running_steps: 50000000  # 50M
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-PER_alpha: 0.5
-PER_beta0: 0.4
-
 test_steps: 10000
 eval_interval: 500000
 test_episode: 1
-log_dir: "./logs/perdqn/"
-model_dir: "./models/perdqn/"
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/perdqn/box2d/CarRacing-v2.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/perdqn/box2d/LunarLander-v2.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.1
 decay_step_greedy: 20000
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agent: "PerDQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.1
 decay_step_greedy: 20000
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/sac/classic_control/CartPole-v1.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "PerDQN"
+agent: "SACDIS"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "Basic_Q_network"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'relu'
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
+activation: "relu"
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 128
-learning_rate: 0.001
+buffer_size: 200000
+batch_size: 256
+actor_learning_rate: 0.001
+critic_learning_rate: 0.001
 gamma: 0.99
+alpha: 0.2
+use_automatic_entropy_tuning: True
+tau: 0.005
 
-start_greedy: 0.5
-end_greedy: 0.1
-decay_step_greedy: 20000
-sync_frequency: 100
-training_frequency: 4
+training_frequency: 2
 running_steps: 500000
-start_training: 1000
+start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-PER_alpha: 0.5
-PER_beta0: 0.4
-
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/perdqn/"
-model_dir: "./models/perdqn/"
+test_episode: 5
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml` & `xuance-1.1.1/xuance/configs/dqn/classic_control/Acrobot-v1.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-agent: "PerDQN"
+agent: "DQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 128
+buffer_size: 100000
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
-end_greedy: 0.1
-decay_step_greedy: 20000
-sync_frequency: 100
-training_frequency: 4
-running_steps: 500000
+end_greedy: 0.01
+decay_step_greedy: 10000
+sync_frequency: 50
+training_frequency: 1
+running_steps: 200000  # 200k
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-PER_alpha: 0.5
-PER_beta0: 0.4
-
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 1
-log_dir: "./logs/perdqn/"
-model_dir: "./models/perdqn/"
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/pg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-agent: "PG"
+agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Box2D"
 env_id: "BipedalWalker-v3"
-representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_Actor"
+representation: "Basic_MLP"
+policy: "Gaussian_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
-activation: 'relu'
+critic_hidden_size: [128,]
+activation: 'leaky_relu'
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-running_steps: 100000
-n_steps: 1024
-n_epoch: 3
-n_minibatch: 1
+running_steps: 300000
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 8
+n_minibatch: 8
 learning_rate: 0.0004
 
+use_grad_clip: True
+
+vf_coef: 0.25
 ent_coef: 0.01
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
+target_kl: 0.001  # for PPO_KL agent
+clip_range: 0.2  # for PPO_Clip agent
+clip_grad_norm: 0.5
 gamma: 0.98
-use_gae: False
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 10000
-test_episode: 1
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+eval_interval: 50000
+test_episode: 3
+log_dir: "./logs/ppo/"
+model_dir: "./models/ppo/"
```

### Comparing `xuance-1.1.0/xuance/configs/pg/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/pg/classic_control/Acrobot-v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 agent: "PG"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
 policy: "Categorical_Actor"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-nsteps: 128
-nepoch: 3
-nminibatch: 1
+horizon_size: 500
+n_epoch: 1
+n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
 use_gae: False
```

### Comparing `xuance-1.1.0/xuance/configs/pg/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/pg/box2d/BipedalWalker-v3.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 agent: "PG"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_name: "Box2D"
+env_id: "BipedalWalker-v3"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
-policy: "Categorical_Actor"
+policy: "Gaussian_Actor"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 activation: 'relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-running_steps: 300000
-n_steps: 500
-n_epoch: 1
+running_steps: 100000
+horizon_size: 1024  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 3
 n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
@@ -28,11 +29,11 @@
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 10000
 test_episode: 1
 log_dir: "./logs/pg/"
 model_dir: "./models/pg/"
```

### Comparing `xuance-1.1.0/xuance/configs/pg/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/pg/box2d/LunarLander-v2.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 agent: "PG"
-env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
 policy: "Categorical_Actor"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 128
-n_epoch: 1
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 3
 n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
```

### Comparing `xuance-1.1.0/xuance/configs/pg/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/pg/classic_control/Pendulum-v1.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 agent: "PG"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Pendulum-v1"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
-policy: "Categorical_Actor"
+policy: "Gaussian_Actor"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-activation: 'relu'
+representation_hidden_size: [256,]
+actor_hidden_size: [256,]
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 128
-n_epoch: 3
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
@@ -31,8 +32,8 @@
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
 log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+model_dir: "./models/pg/"
```

### Comparing `xuance-1.1.0/xuance/configs/pg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/ppo/mujoco.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-agent: "PG"
-env_name: "Classic Control"
-env_id: "Pendulum-v1"
-representation: "Basic_MLP"
+agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_Actor"
+policy: "Gaussian_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
+representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
-activation: 'leaky_relu'
+critic_hidden_size: [256,]
+activation: "leaky_relu"
 activation_action: 'tanh'
 
-seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 128
-n_epoch: 1
-n_minibatch: 1
+seed: 79811
+parallels: 16
+running_steps: 1000000
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_epoch: 16
+n_minibatch: 8
 learning_rate: 0.0004
 
-ent_coef: 0.01
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.98
-use_gae: False
+use_grad_clip: True
+
+vf_coef: 0.25
+ent_coef: 0.0
+target_kl: 0.001  # for PPO_KL agent
+clip_range: 0.2  # for PPO_Clip agent
+clip_grad_norm: 0.5
+gamma: 0.99
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+eval_interval: 5000
+test_episode: 5
+log_dir: "./logs/ppo/"
+model_dir: "./models/ppo/"
```

### Comparing `xuance-1.1.0/xuance/configs/pg/mujoco.yaml` & `xuance-1.1.1/xuance/configs/ppg/mujoco.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-agent: "PG"
+agent: "PPG"
 env_name: "MuJoCo"
-env_id: "Ant-v4"
+env_id: "InvertedPendulum-v2"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_Actor"
 representation: "Basic_MLP"
+policy: "Gaussian_PPG"
 runner: "DRL"
 
-representation_hidden_size: [256, 256]
-actor_hidden_size: []
+representation_hidden_size: [256,]
+actor_hidden_size: [256,]
+critic_hidden_size: [256,]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 16
 running_steps: 1000000  # 1M
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
+n_minibatch: 4
 n_epoch: 1
-n_minibatch: 1
-learning_rate: 0.0007  # 7e-4
+policy_nepoch: 2
+value_nepoch: 4
+aux_nepoch: 8
+
+learning_rate: 0.0007
 
 ent_coef: 0.0
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.99
-use_gae: False
+clip_range: 0.25
+kl_beta: 2.0
+gamma: 0.98
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 5000
+eval_interval: 10000
 test_episode: 5
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+log_dir: "./logs/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/ppg/classic_control/Pendulum-v1.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 agent: "PPG"
-env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+env_name: "Classic Control"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Gaussian_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
 policy_nepoch: 4
 value_nepoch: 8 
 aux_nepoch: 8
 n_minibatch: 1
 learning_rate: 0.001
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/ppg/box2d/LunarLander-v2.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: "relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
 policy_nepoch: 4
 value_nepoch: 8 
 aux_nepoch: 8
 n_minibatch: 1
 learning_rate: 0.0004
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/sac/box2d/BipedalWalker-v3.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-agent: "PPG"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
+agent: "SAC"
+env_name: "Box2D"
+env_id: "BipedalWalker-v3"
 vectorize: "Dummy_Gym"
-representation: "Basic_MLP"
-policy: "Categorical_PPG"
+policy: "Gaussian_SAC"
+representation: "Basic_Identical"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-critic_hidden_size: [128,]
+representation_hidden_size:
+actor_hidden_size: [256, 256]
+critic_hidden_size: [256, 256]
 activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 256
-n_epoch: 1
-policy_nepoch: 4
-value_nepoch: 8 
-aux_nepoch: 8
-n_minibatch: 1
-learning_rate: 0.001
+parallels: 10  # number of environments
+buffer_size: 200000
+batch_size: 256
+actor_learning_rate: 0.001
+critic_learning_rate: 0.001
+gamma: 0.99
+alpha: 0.2
+use_automatic_entropy_tuning: True
+tau: 0.005
 
-ent_coef: 0.01
-clip_range: 0.2
-kl_beta: 1.0
-gamma: 0.98
-use_gae: True
-gae_lambda: 0.95
-use_advnorm: True
+training_frequency: 1
+running_steps: 5000000
+start_training: 2000
 
-use_obsnorm: True
-use_rewnorm: True
+use_obsnorm: False
+use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+eval_interval: 500000
+test_episode: 5
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/a2c/classic_control/CartPole-v1.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-agent: "PPG"
+agent: "A2C"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
-vectorize: "Dummy_Gym"
+vectorize: "Subproc_Gym"
+policy: "Categorical_AC"
 representation: "Basic_MLP"
-policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "relu"
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
-policy_nepoch: 4
-value_nepoch: 8 
-aux_nepoch: 8
-n_minibatch: 1
+n_minibatch: 8
 learning_rate: 0.0004
 
+vf_coef: 0.25
 ent_coef: 0.01
-clip_range: 0.2
-kl_beta: 1.0
+clip_grad: 0.5
+clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+test_episode: 3
+log_dir: "./logs/a2c/"
+model_dir: "./models/a2c/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/ppg/classic_control/CartPole-v1.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 agent: "PPG"
 env_name: "Classic Control"
-env_id: "Pendulum-v1"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Gaussian_PPG"
+policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "leaky_relu"
-activation_action: 'tanh'
+activation: "relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
 policy_nepoch: 4
 value_nepoch: 8 
 aux_nepoch: 8
 n_minibatch: 1
-learning_rate: 0.001
+learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_range: 0.2
 kl_beta: 1.0
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
@@ -36,8 +35,8 @@
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
 log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppg/mujoco.yaml` & `xuance-1.1.1/xuance/configs/ppg/classic_control/MountainCar-v0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 agent: "PPG"
-env_name: "MuJoCo"
-env_id: "InvertedPendulum-v2"
+env_name: "Classic Control"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Gaussian_PPG"
+policy: "Categorical_PPG"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
 activation: "leaky_relu"
-activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-running_steps: 1000000  # 1M
-n_steps: 256
-n_minibatch: 4
+parallels: 10
+running_steps: 300000
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 1
-policy_nepoch: 2
-value_nepoch: 4
+policy_nepoch: 4
+value_nepoch: 8 
 aux_nepoch: 8
+n_minibatch: 1
+learning_rate: 0.001
 
-learning_rate: 0.0007
-
-ent_coef: 0.0
-clip_range: 0.25
-kl_beta: 2.0
+ent_coef: 0.01
+clip_range: 0.2
+kl_beta: 1.0
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 10000
-test_episode: 5
+eval_interval: 50000
+test_episode: 1
 log_dir: "./logs/ppg/"
 model_dir: "./models/ppg/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/atari.yaml` & `xuance-1.1.1/xuance/configs/ppo/atari.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 8
 running_steps: 10000000  # 10M
-n_steps: 128
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 4
 n_minibatch: 4
 learning_rate: 0.00025
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/ppo/box2d/LunarLander-v2.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Gaussian_AC"
+policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: 'leaky_relu'
-activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 8
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/ppo/box2d/CarRacing-v2.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 seed: 1
 parallels: 2
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 8
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/sac/box2d/LunarLander-v2.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,38 @@
-agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
+agent: "SACDIS"
 env_name: "Box2D"
 env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
-policy: "Categorical_AC"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-critic_hidden_size: [128,]
-activation: 'leaky_relu'
+representation_hidden_size: [256,]
+actor_hidden_size: [128,128,]
+critic_hidden_size: [128,128,]
+activation: "relu"
 
 seed: 1
 parallels: 10
-running_steps: 300000
-n_steps: 256
-n_epoch: 8
-n_minibatch: 8
-learning_rate: 0.0004
+buffer_size: 200000
+batch_size: 256
+actor_learning_rate: 0.001
+critic_learning_rate: 0.01
+gamma: 0.99
+alpha: 0.2
+use_automatic_entropy_tuning: True
+tau: 0.005
+
+training_frequency: 1
+running_steps: 500000
+start_training: 2000
 
-use_grad_clip: True
-
-vf_coef: 0.25
-ent_coef: 0.01
-target_kl: 0.001  # for PPO_KL agent
-clip_range: 0.2  # for PPO_Clip agent
-clip_grad_norm: 0.5
-gamma: 0.98
-use_gae: True
-gae_lambda: 0.95
-use_advnorm: True
-
-use_obsnorm: True
-use_rewnorm: True
+use_obsnorm: False
+use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/ppo/"
-model_dir: "./models/ppo/"
+test_episode: 1
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/ppo/classic_control/MountainCar-v0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 8
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/ppo/classic_control/Pendulum-v1.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Categorical_AC"
+policy: "Gaussian_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 8
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/ppo/classic_control/CartPole-v1.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
 activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
-running_steps: 300000
-n_steps: 256
+running_steps: 120000
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 8
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/drones.yaml` & `xuance-1.1.1/xuance/configs/ppo/drones.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 critic_hidden_size: [512,]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 79811
 parallels: 10
 running_steps: 1000000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 16
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/metadrive.yaml` & `xuance-1.1.1/xuance/configs/ppo/metadrive.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 critic_hidden_size: [512, 512]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 500000
-n_steps: 128
+horizon_size: 128  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 4
 n_minibatch: 4
 learning_rate: 0.00025
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/ppo/minigrid.yaml` & `xuance-1.1.1/xuance/configs/ppo/minigrid.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
 activation: "leaky_relu"
 
 seed: 79811
 parallels: 16
 running_steps: 100000
-n_steps: 256
+horizon_size: 256  # the horizon size for an environment, buffer_size = horizon_size * parallels.
 n_epoch: 16
 n_minibatch: 8
 learning_rate: 0.0001
 
 use_grad_clip: True
 
 vf_coef: 0.25
```

### Comparing `xuance-1.1.0/xuance/configs/qmix/football/3v1.yaml` & `xuance-1.1.1/xuance/configs/qmix/football/3v1.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/qmix/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/1c3s5z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/25m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/2s3z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/3m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/5m_vs_6m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/8m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/8m_vs_9m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/MMM2.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qmix/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/qmix/sc2/corridor.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/atari.yaml` & `xuance-1.1.1/xuance/configs/sac/atari.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-agent: "QRDQN"
+agent: "SACDIS"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
 noop_max: 30  # Do no-op action for a number of steps in [1, noop_max].
-policy: "QR_Q_network"
 representation: "Basic_CNN"
+policy: "Discrete_SAC"
 runner: "DRL"
 
-# the following three arguments are for "Basic_CNN" representation.
-filters: [32, 64, 64]  #  [16, 16, 32, 32]
-kernels: [8, 4, 3]  # [8, 6, 4, 4]
-strides: [4, 2, 1]  # [2, 2, 2, 2]
-
-q_hidden_size: [512, ]
-activation: "relu"
+filters: [32, 32, 64, 64]
+kernels: [8, 4, 4, 4]
+strides: [4, 2, 2, 2]
+actor_hidden_size: [128, 128]
+critic_hidden_size: [128, 128]
+activation: "leaky_relu"
 
 seed: 1069
 parallels: 5
-n_size: 100000
+buffer_size: 500000
 batch_size: 32  # 64
-learning_rate: 0.0001
+actor_learning_rate: 0.001
+critic_learning_rate: 0.001
 gamma: 0.99
-quantile_num: 20
+alpha: 0.01
+use_automatic_entropy_tuning: False
+tau: 0.005
 
-start_greedy: 0.5
-end_greedy: 0.05
-decay_step_greedy: 1000000  # 1M
-sync_frequency: 500
 training_frequency: 1
 running_steps: 50000000  # 50M
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 500000
 test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.1/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-agent: "QRDQN"
+agent: "Duel_DQN"
 env_name: "Box2D"
 env_id: "CarRacing-v2"
 vectorize: "Dummy_Gym"
-policy: "QR_Q_network"
+policy: "Duel_Q_network"
 representation: "Basic_CNN"
 runner: "DRL"
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
 activation: 'relu'
 
 seed: 1
 parallels: 2
-n_size: 10000
+buffer_size: 20000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
-quantile_num: 20
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 50000
 sync_frequency: 500
 training_frequency: 1
 running_steps: 2000000
@@ -34,9 +33,9 @@
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 100000
 test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+log_dir: "./logs/dueldqn/"
+model_dir: "./models/dueldqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 agent: "QRDQN"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
 policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 quantile_num: 20
 
-start_greedy: 0.5
+start_greedy: 0.25
 end_greedy: 0.01
-decay_step_greedy: 10000
-sync_frequency: 50
+decay_step_greedy: 30000
+sync_frequency: 100
 training_frequency: 1
-running_steps: 200000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
```

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/spdqn/Platform.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-agent: "QRDQN"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
-vectorize: "Dummy_Gym"
-policy: "QR_Q_network"
+agent: "SPDQN"
+env_name: "Platform"
+env_id: "Platform-v0"
+vectorize: "NOREQUIRED"
+policy: "SPDQN_Policy"
+render: False
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'relu'
+conactor_hidden_size: [128,]
+qnetwork_hidden_size: [128, ]
+activation: "relu"
+activation_action: 'tanh'
 
-seed: 1
-parallels: 10
-n_size: 20000
-batch_size: 256
+buffer_size: 20000
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
-quantile_num: 20
+tau: 0.005
 
-start_greedy: 0.25
-end_greedy: 0.01
-decay_step_greedy: 30000
-sync_frequency: 100
+start_noise: 0.1
+end_noise: 0.1
 training_frequency: 1
-running_steps: 300000
+running_steps: 30000
 start_training: 1000
 
+test_steps: 10000
+eval_interval: 1000
+test_episode: 5
+
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+log_dir: "./logs/spdqn/"
+model_dir: "./models/spdqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/c51/classic_control/CartPole-v1.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-agent: "QRDQN"
+agent: "C51DQN"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "QR_Q_network"
+policy: "C51_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
 activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
-quantile_num: 20
+vmin: 0
+vmax: 200
+atom_num: 51
 
-start_greedy: 0.25
+start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 30000
+decay_step_greedy: 10000
 sync_frequency: 100
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+log_dir: "./logs/c51/"
+model_dir: "./models/c51/"
```

### Comparing `xuance-1.1.0/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.1/xuance/configs/sac/metadrive.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-agent: "QRDQN"
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
-vectorize: "Dummy_Gym"
-policy: "QR_Q_network"
-representation: "Basic_MLP"
+agent: "SAC"
+env_name: "MetaDrive"
+env_id: "metadrive"
+env_config:  # the configs for MetaDrive environment
+  map: "C"  # see https://metadrive-simulator.readthedocs.io/en/latest/rl_environments.html#generalization-environment for choices
+render: False
+vectorize: "Subproc_MetaDrive"
+policy: "Gaussian_SAC"
+representation: "Basic_Identical"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'relu'
+representation_hidden_size:
+actor_hidden_size: [512, 512]
+critic_hidden_size: [512, 512]
+activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-n_size: 20000
+parallels: 4
+buffer_size: 1000000
 batch_size: 256
-learning_rate: 0.001
+actor_learning_rate: 0.0003
+critic_learning_rate: 0.0003
 gamma: 0.99
-quantile_num: 20
+alpha: 0.2
+use_automatic_entropy_tuning: True
+tau: 0.005
 
-start_greedy: 0.25
-end_greedy: 0.01
-decay_step_greedy: 30000
-sync_frequency: 100
 training_frequency: 1
-running_steps: 300000
-start_training: 1000
+running_steps: 1000000
+start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+eval_interval: 10000
+test_episode: 5
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/qtran/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/qtran/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/sac/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.1/xuance/configs/sac/classic_control/Acrobot-v1.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-agent: "SAC"
-env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+agent: "SACDIS"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_SAC"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
 activation: "relu"
-activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+buffer_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
-gamma: 0.98
+gamma: 0.99
+alpha: 0.2
+use_automatic_entropy_tuning: True
 tau: 0.005
 
-start_noise: 0.25
-end_noise: 0.05
 training_frequency: 2
 running_steps: 500000
 start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
+test_episode: 5
 log_dir: "./logs/sac/"
 model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/box2d/LunarLander-v2.yaml` & `xuance-1.1.1/xuance/configs/sac/classic_control/MountainCar-v0.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 agent: "SACDIS"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [128,128,]
-critic_hidden_size: [128,128,]
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
 activation: "relu"
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+buffer_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.01
 gamma: 0.98
+alpha: 0.2
+use_automatic_entropy_tuning: True
 tau: 0.005
 
-start_noise: 0.25
-end_noise: 0.05
 training_frequency: 2
 running_steps: 500000
 start_training: 2000
-action_type: "DISCRETE"
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
+test_episode: 5
 log_dir: "./logs/sac/"
 model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/classic_control/Acrobot-v1.yaml` & `xuance-1.1.1/xuance/configs/sac/classic_control/Pendulum-v1.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-agent: "SACDIS"
+agent: "SAC"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "Discrete_SAC"
+policy: "Gaussian_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
-actor_hidden_size: [128,128,]
-critic_hidden_size: [128,128,]
+actor_hidden_size: [256,]
+critic_hidden_size: [256,]
 activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+buffer_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
-critic_learning_rate: 0.01
+critic_learning_rate: 0.001
 gamma: 0.98
+alpha: 0.2
+use_automatic_entropy_tuning: True
 tau: 0.005
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
+training_frequency: 1
 running_steps: 500000
-start_training: 2000
-action_type: "DISCRETE"
+start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
+test_episode: 5
 log_dir: "./logs/sac/"
 model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/classic_control/CartPole-v1.yaml` & `xuance-1.1.1/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-agent: "SACDIS"
+agent: "Duel_DQN"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Discrete_SAC"
+policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-critic_hidden_size: [128,]
-activation: "relu"
+representation_hidden_size: [128, ]
+q_hidden_size: [128, ]
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+buffer_size: 100000
 batch_size: 256
-actor_learning_rate: 0.001
-critic_learning_rate: 0.01
-gamma: 0.98
-tau: 0.005
+learning_rate: 0.001
+gamma: 0.99
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
+start_greedy: 0.5
+end_greedy: 0.01
+decay_step_greedy: 20000
+sync_frequency: 50
+training_frequency: 1
 running_steps: 500000
-start_training: 2000
-action_type: "DISCRETE"
+start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+log_dir: "./logs/dueldqn/"
+model_dir: "./models/dueldqn/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/td3/box2d/BipedalWalker-v3.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-agent: "SAC"
-env_name: "Classic Control"
-env_id: "Pendulum-v1"
+agent: "TD3"
+env_name: "Box2D"
+env_id: "BipedalWalker-v3"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_SAC"
-representation: "Basic_MLP"
+representation: "Basic_Identical"
+policy: "TD3_Policy"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: "relu"
+representation_hidden_size:
+actor_hidden_size: [256, 256]
+critic_hidden_size: [256, 256]
+activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+buffer_size: 200000
 batch_size: 256
-actor_learning_rate: 0.001
+actor_learning_rate: 0.0005
 critic_learning_rate: 0.001
-gamma: 0.98
+gamma: 0.99
 tau: 0.005
+actor_update_delay: 3
 
 start_noise: 0.25
 end_noise: 0.05
 training_frequency: 2
-running_steps: 500000
+running_steps: 2000000
 start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+test_episode: 5
+log_dir: "./logs/td3/"
+model_dir: "./models/td3/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/metadrive.yaml` & `xuance-1.1.1/xuance/configs/td3/mujoco.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-agent: "SAC"
-env_name: "MetaDrive"
-env_id: "metadrive"
-env_config:  # the configs for MetaDrive environment
-  map: "C"  # see https://metadrive-simulator.readthedocs.io/en/latest/rl_environments.html#generalization-environment for choices
-render: False
-vectorize: "Subproc_MetaDrive"
-policy: "Gaussian_SAC"
+agent: "TD3"
+env_name: "MuJoCo"
+env_id: "Ant-v4"
+vectorize: "Dummy_Gym"
 representation: "Basic_Identical"
+policy: "TD3_Policy"
 runner: "DRL"
 
-representation_hidden_size:
-actor_hidden_size: [512, 512]
-critic_hidden_size: [512, 512]
-activation: "relu"
+representation_hidden_size:  # If you choose Basic_Identical representation, then ignore this value
+actor_hidden_size: [400, 300]
+critic_hidden_size: [400, 300]
+activation: "leaky_relu"
 activation_action: 'tanh'
 
-seed: 1
-parallels: 10
-n_size: 250000
+seed: 6782
+parallels: 4  # number of environments
+buffer_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
+actor_update_delay: 2
 critic_learning_rate: 0.001
 gamma: 0.99
-alpha: 0.2
 tau: 0.005
-learning_rate: 0.0003
 
-start_noise: 0.25
-end_noise: 0.01
+start_noise: 0.1
+end_noise: 0.1
 training_frequency: 1
 running_steps: 1000000
-start_training: 1000
+start_training: 25000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 10000
+eval_interval: 5000
 test_episode: 5
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+log_dir: "./logs/td3/"
+model_dir: "./models/td3/"
```

### Comparing `xuance-1.1.0/xuance/configs/sac/mujoco.yaml` & `xuance-1.1.1/xuance/configs/sac/drones.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 agent: "SAC"
-env_name: "MuJoCo"
-env_id: "Ant-v4"
-vectorize: "Dummy_Gym"
+env_name: "Drones"
+env_id: "HoverAviary"
+obs_type: 'kin'
+act_type: 'one_d_rpm'
+num_drones: 1
+record: False
+obstacles: True
+max_episode_steps: 2000  #
+render: False
+sleep: 0.01
+vectorize: "Dummy_Drone"
 policy: "Gaussian_SAC"
 representation: "Basic_Identical"
 runner: "DRL"
 
 representation_hidden_size:
-actor_hidden_size: [256, 256]
-critic_hidden_size: [256, 256]
+actor_hidden_size: [512, 512]
+critic_hidden_size: [512, 512]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
-parallels: 4
-n_size: 250000
+parallels: 10
+buffer_size: 1000000
 batch_size: 256
-actor_learning_rate: 0.001
-critic_learning_rate: 0.001
+actor_learning_rate: 0.0003
+critic_learning_rate: 0.0003
 gamma: 0.99
 alpha: 0.2
+use_automatic_entropy_tuning: True
 tau: 0.005
-learning_rate: 0.0003
 
-start_noise: 0.25
-end_noise: 0.01
 training_frequency: 1
 running_steps: 1000000
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 5000
+eval_interval: 10000
 test_episode: 5
 log_dir: "./logs/sac/"
 model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/td3/classic_control/Pendulum-v1.yaml` & `xuance-1.1.1/xuance/configs/sac/mujoco.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-agent: "TD3"
-env_name: "Classic Control"
-env_id: "Pendulum-v1"
+agent: "SAC"
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
+policy: "Gaussian_SAC"
 representation: "Basic_Identical"
-policy: "TD3_Policy"
 runner: "DRL"
 
-representation_hidden_size: [64]
-actor_hidden_size: [256, ]
-critic_hidden_size: [256, ]
+representation_hidden_size:
+actor_hidden_size: [256, 256]
+critic_hidden_size: [256, 256]
 activation: "leaky_relu"
 activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-n_size: 20000
+parallels: 4  # number of environments
+buffer_size: 1000000
 batch_size: 256
-actor_learning_rate: 0.0005
+actor_learning_rate: 0.001
 critic_learning_rate: 0.001
-gamma: 0.98
+gamma: 0.99
+alpha: 0.2
+use_automatic_entropy_tuning: True
 tau: 0.005
-actor_update_delay: 3
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
-running_steps: 500000
-start_training: 2000
+training_frequency: 1
+running_steps: 1000000
+start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/td3/"
-model_dir: "./models/td3/"
+eval_interval: 10000
+test_episode: 5
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/vdac/mpe/simple_spread_v3.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 mixer: "VDN"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 128
-n_size: 3200
+buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
 weight_decay: 0
 
 vf_coef: 0.5
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/1c3s5z.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/25m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/2m_vs_1z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/5m_vs_6m.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "5m_vs_6m"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
+on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
@@ -25,44 +26,43 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.2
+clip_range: 0.05
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
+use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.2
+value_clip_range: 0.05
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 2000000
-train_per_step: True
+running_steps: 10000000  # 10M
 training_frequency: 1
 
-test_steps: 10000
-eval_interval: 10000
+eval_interval: 50000
 test_episode: 16
 log_dir: "./logs/vdac/"
 model_dir: "./models/vdac/"
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/3m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 mixer: "QMIX"  # choices: Independent, VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.0
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/MMM2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "5m_vs_6m"
+env_id: "MMM2"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -14,47 +14,47 @@
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 0.01
+gain: 1.0
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
-n_minibatch: 1
+n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.05
+clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.05
+value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/8m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/8m_vs_9m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/ippo/sc2/3m.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-agent: "VDAC"
+agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "3m"
 fps: 15
-policy: "Categorical_MAAC_Policy_Share"
+policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
-on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, ]
+fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 1.0
+gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
 activation: "relu"
 
-mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
-hidden_dim_mixing_net: 32  # hidden units of mixing network
-hidden_dim_hyper_net: 64  # hidden units of hyper network
-
 seed: 1
 parallels: 8
-n_size: 8
-n_epoch: 1
-n_minibatch: 2
+buffer_size: 128
+n_epoch: 15
+n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -55,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000  # 10M
+running_steps: 1000000
 training_frequency: 1
 
-eval_interval: 50000
+eval_interval: 10000
 test_episode: 16
-log_dir: "./logs/vdac/"
-model_dir: "./models/vdac/"
+log_dir: "./logs/ippo/"
+model_dir: "./models/ippo/"
```

### Comparing `xuance-1.1.0/xuance/configs/vdac/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/vdac/sc2/2s3z.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "corridor"
+env_id: "2s3z"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
-on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
@@ -26,15 +25,15 @@
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 8
+buffer_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
@@ -42,27 +41,28 @@
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000  # 10M
+running_steps: 2000000
+train_per_step: True
 training_frequency: 1
 
-eval_interval: 50000
+test_steps: 10000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/vdac/"
 model_dir: "./models/vdac/"
```

### Comparing `xuance-1.1.0/xuance/configs/vdn/football/3v1.yaml` & `xuance-1.1.1/xuance/configs/vdn/football/3v1.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/vdn/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/new_env_mas.yaml` & `xuance-1.1.1/xuance/configs/vdn/new_env_mas.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/1c3s5z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/25m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/2s3z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/3m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/5m_vs_6m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/8m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/8m_vs_9m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/MMM2.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/vdn/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/vdn/sc2/corridor.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/mpe/simple_spread_v3.yaml` & `xuance-1.1.1/xuance/configs/wqmix/mpe/simple_spread_v3.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/1c3s5z.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/1c3s5z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/25m.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/25m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/2m_vs_1z.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/2s3z.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/2s3z.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/3m.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/3m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/5m_vs_6m.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/5m_vs_6m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/8m.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/8m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/8m_vs_9m.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/8m_vs_9m.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/MMM2.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/MMM2.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/configs/wqmix/sc2/corridor.yaml` & `xuance-1.1.1/xuance/configs/wqmix/sc2/corridor.yaml`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/__init__.py` & `xuance-1.1.1/xuance/environment/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,44 @@
 from xuance.environment.pettingzoo import DummyVecEnv_Pettingzoo, SubprocVecEnv_Pettingzoo
 from xuance.environment.starcraft2 import DummyVecEnv_StarCraft2, SubprocVecEnv_StarCraft2
 from xuance.environment.football import DummyVecEnv_GFootball, SubprocVecEnv_GFootball
 from xuance.environment.minigrid import DummyVecEnv_MiniGrid, SubprocVecEnv_MiniGrid
 from xuance.environment.drones import DummyVecEnv_Drones, SubprocVecEnv_Drones
 from xuance.environment.drones import DummyVecEnv_Drones_MAS, SubprocVecEnv_Drones_MAS
 from xuance.environment.metadrive import SubprocVecEnv_MetaDrive
+from xuance.environment.robotic_warehouse import DummyVecEnv_RoboticWarehouse, SubprocVecEnv_RoboticWarehouse
 from xuance.environment.new_env import DummyVecEnv_New, SubprocVecEnv_New
 from xuance.environment.new_env_mas import DummyVecEnv_New_MAS, SubprocVecEnv_New_MAS
 
 from .vector_envs.subproc_vec_env import SubprocVecEnv
 
 REGISTRY_VEC_ENV = {
     "Dummy_Gym": DummyVecEnv_Gym,
     "Dummy_Pettingzoo": DummyVecEnv_Pettingzoo,
     "Dummy_StarCraft2": DummyVecEnv_StarCraft2,
     "Dummy_Football": DummyVecEnv_GFootball,
     "Dummy_Atari": DummyVecEnv_Atari,
     "Dummy_MiniGrid": DummyVecEnv_MiniGrid,
     "Dummy_Drone": DummyVecEnv_Drones,
     "Dummy_Drone_MAS": DummyVecEnv_Drones_MAS,
+    "Dummy_RoboticWarehouse": DummyVecEnv_RoboticWarehouse,
     "Dummy_NewEnv": DummyVecEnv_New,  # Add the newly defined vectorized environment
     "Dummy_NewEnv_MAS": DummyVecEnv_New_MAS,  # Add the newly defined vectorized environment for multi-agent systems
 
     # multiprocess #
     "Subproc_Gym": SubprocVecEnv_Gym,
     "Subproc_Pettingzoo": SubprocVecEnv_Pettingzoo,
     "Subproc_StarCraft2": SubprocVecEnv_StarCraft2,
     "Subproc_Football": SubprocVecEnv_GFootball,
     "Subproc_Atari": SubprocVecEnv_Atari,
     "Subproc_MiniGrid": SubprocVecEnv_MiniGrid,
     "Subproc_Drone": SubprocVecEnv_Drones,
     "Subproc_Drone_MAS": SubprocVecEnv_Drones_MAS,
     "Subproc_MetaDrive": SubprocVecEnv_MetaDrive,
+    "Subproc_RoboticWarehouse": SubprocVecEnv_RoboticWarehouse,
     "Subproc_NewEnv": SubprocVecEnv_New,  # Add the newly defined vectorized environment
     "Subproc_NewEnv_MAS": SubprocVecEnv_New_MAS,  # Add the newly defined vectorized environment for multi-agent systems
 }
 
 
 def make_envs(config: Namespace):
     def _thunk():
@@ -66,17 +69,17 @@
             env = MAgent_Env(config.env_id, config.seed,
                              minimap_mode=config.minimap_mode,
                              max_cycles=config.max_cycles,
                              extra_features=config.extra_features,
                              map_size=config.map_size,
                              render_mode=config.render_mode)
 
-        elif config.env_name == "Robotic_WareHouse":
+        elif config.env_name == "RoboticWarehouse":
             from xuance.environment.robotic_warehouse.robotic_warehouse_env import RoboticWarehouseEnv
-            env = RoboticWarehouseEnv()
+            env = RoboticWarehouseEnv(config, render_mode=config.render_mode)
 
         elif config.env_name == "Atari":
             from xuance.environment.gym.gym_env import Atari_Env
             env = Atari_Env(config.env_id, config.seed, config.render_mode,
                             config.obs_type, config.frame_skip, config.num_stack, config.img_size, config.noop_max)
 
         elif config.env_id.__contains__("MountainCar"):
```

### Comparing `xuance-1.1.0/xuance/environment/drones/customized/HoverAviary.py` & `xuance-1.1.1/xuance/environment/drones/customized/HoverAviary.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/drones/customized/MultiHoverAviary.py` & `xuance-1.1.1/xuance/environment/drones/customized/MultiHoverAviary.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/drones/drones_env.py` & `xuance-1.1.1/xuance/environment/drones/drones_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/drones/drones_vec_env.py` & `xuance-1.1.1/xuance/environment/drones/drones_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/drones/drones_vec_env_mas.py` & `xuance-1.1.1/xuance/environment/drones/drones_vec_env_mas.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/football/__init__.py` & `xuance-1.1.1/xuance/environment/football/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/football/gfootball_env.py` & `xuance-1.1.1/xuance/environment/football/gfootball_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/football/gfootball_vec_env.py` & `xuance-1.1.1/xuance/environment/football/gfootball_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/football/raw_env.py` & `xuance-1.1.1/xuance/environment/football/raw_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/gym/gym_env.py` & `xuance-1.1.1/xuance/environment/gym/gym_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/gym/gym_vec_env.py` & `xuance-1.1.1/xuance/environment/gym/gym_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/gym_platform/envs/platform_env.py` & `xuance-1.1.1/xuance/environment/gym_platform/envs/platform_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/__init__.py` & `xuance-1.1.1/xuance/environment/magent2/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/builtin/config/battle.py` & `xuance-1.1.1/xuance/environment/magent2/builtin/config/battle.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/builtin/config/double_attack.py` & `xuance-1.1.1/xuance/environment/magent2/builtin/config/double_attack.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/builtin/config/forest.py` & `xuance-1.1.1/xuance/environment/magent2/builtin/config/forest.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/builtin/config/pursuit.py` & `xuance-1.1.1/xuance/environment/magent2/builtin/config/pursuit.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/c_lib.py` & `xuance-1.1.1/xuance/environment/magent2/c_lib.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environment.py` & `xuance-1.1.1/xuance/environment/magent2/environment.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py` & `xuance-1.1.1/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/battle/battle.py` & `xuance-1.1.1/xuance/environment/magent2/environments/battle/battle.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/battlefield/battlefield.py` & `xuance-1.1.1/xuance/environment/magent2/environments/battlefield/battlefield.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/combined_arms.py` & `xuance-1.1.1/xuance/environment/magent2/environments/combined_arms/combined_arms.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/gather/gather.py` & `xuance-1.1.1/xuance/environment/magent2/environments/gather/gather.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/magent_env.py` & `xuance-1.1.1/xuance/environment/magent2/environments/magent_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py` & `xuance-1.1.1/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/gridworld.py` & `xuance-1.1.1/xuance/environment/magent2/gridworld.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/libmagent.dylib` & `xuance-1.1.1/xuance/environment/magent2/libmagent.dylib`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/libmagent.so` & `xuance-1.1.1/xuance/environment/magent2/libmagent.so`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/magent.dll` & `xuance-1.1.1/xuance/environment/magent2/magent.dll`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/magent_env.py` & `xuance-1.1.1/xuance/environment/magent2/magent_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/magent_vec_env.py` & `xuance-1.1.1/xuance/environment/magent2/magent_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/render.py` & `xuance-1.1.1/xuance/environment/magent2/render.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/magent2/utility.py` & `xuance-1.1.1/xuance/environment/magent2/utility.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/metadrive/metadrive_env.py` & `xuance-1.1.1/xuance/environment/metadrive/metadrive_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/metadrive/metadrive_vec_env.py` & `xuance-1.1.1/xuance/environment/metadrive/metadrive_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/minigrid/minigrid_env.py` & `xuance-1.1.1/xuance/environment/minigrid/minigrid_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/minigrid/minigrid_vec_env.py` & `xuance-1.1.1/xuance/environment/minigrid/minigrid_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/new_env/new_env.py` & `xuance-1.1.1/xuance/environment/new_env/new_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/new_env/new_vec_env.py` & `xuance-1.1.1/xuance/environment/new_env/new_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/new_env_mas/new_env_mas.py` & `xuance-1.1.1/xuance/environment/new_env_mas/new_env_mas.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/new_env_mas/new_vec_env_mas.py` & `xuance-1.1.1/xuance/environment/new_env_mas/new_vec_env_mas.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_env.py` & `xuance-1.1.1/xuance/environment/pettingzoo/pettingzoo_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_vec_env.py` & `xuance-1.1.1/xuance/environment/pettingzoo/pettingzoo_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/robotic_warehouse/robotic_warehouse_env.py` & `xuance-1.1.1/xuance/environment/starcraft2/sc2_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-import gymnasium as gym
-from gym.spaces import Box, Discrete
-import numpy as np
+import copy
 
+from smac.env import StarCraft2Env
+import numpy as np
 
-class RoboticWarehouseEnv():
-    """
-    The wrapper of minigrid environment.
-
-    Args:
-        env_id: The environment id of minigrid.
-        seed: random seed.
-        render_mode: "rgb_array", "human".
-        rgb_img_partial_wrapper: whether to apply the RGB image's partial observation wrapper.
-        img_obs_wrapper:  whether to apply the image observation wrapper.
-    """
-    def __init__(self, env_id: str, seed: int, render_mode: str):
-        self.env = gym.make(env_id, render_mode=render_mode)
 
-        self.env_id = env_id
-        self.render_mode = render_mode
+class StarCraft2_Env:
+    def __init__(self, map_name):
+        self.env = StarCraft2Env(map_name=map_name)
+        self.env_info = self.env.get_env_info()
+
+        self.n_agents = self.env_info["n_agents"]
+        self.n_enemies = self.env.n_enemies
+        self.dim_state = self.env_info["state_shape"]
+        self.dim_obs = self.env_info["obs_shape"]
+        self.dim_act = self.n_actions = self.env_info["n_actions"]
+        self.dim_reward = self.n_agents
+
+        self.observation_space = (self.dim_obs,)
+        self.action_space = (self.dim_act, )
+        self.max_cycles = self.env_info["episode_limit"]
         self._episode_step = 0
-        self._episode_score = 0.0
-        self.image_size = np.prod(self.env.observation_space['image'].shape)  # height * width * channels
-        self.dim_obs = self.image_size + 1  # direction
-        self.observation_space = Box(low=0, high=255, shape=[self.dim_obs, ], dtype=np.uint8, seed=seed)
-        self.action_space = self.env.action_space
-        self.max_episode_steps = self.env.env.env.max_steps
+        self._episode_score = 0
+        self.filled = np.zeros([self.max_cycles, 1], np.bool_)
+        self.env.reset()
+        self.buf_info = {
+            'battle_won': 0,
+            'dead_allies': 0,
+            'dead_enemies': 0,
+        }
 
     def close(self):
-        """Close the environment."""
         self.env.close()
 
-    def render(self, *args):
-        """Return the rendering result"""
-        return self.env.render()
+    def render(self, mode):
+        return self.env.render(mode)
 
     def reset(self):
-        """Reset the environment."""
-        obs_raw, info = self.env.reset()
-        obs = self.flatten_obs(obs_raw)
+        obs, state = self.env.reset()
         self._episode_step = 0
         self._episode_score = 0.0
-        info["episode_step"] = self._episode_step
-        return obs, info
+        info = {
+            "episode_step": self._episode_step,
+            "episode_score": self._episode_score,
+        }
+        return obs, state, info
 
     def step(self, actions):
-        """Execute the actions and get next observations, rewards, and other information."""
-        obs_raw, reward, terminated, truncated, info = self.env.step(actions)
-        observation = self.flatten_obs(obs_raw)
-
-        reward *= 10
-
+        reward, terminated, info = self.env.step(actions)
+        if info == {}:
+            info = self.buf_info
+        obs = self.env.get_obs()
+        state = self.env.get_state()
         self._episode_step += 1
         self._episode_score += reward
-        info["episode_step"] = self._episode_step  # current episode step
-        info["episode_score"] = self._episode_score  # the accumulated rewards
-        return observation, reward, terminated, truncated, info
-
-    def flatten_obs(self, obs_raw):
-        """Convert image observation to vectors"""
-        image = obs_raw['image']
-        direction = obs_raw['direction']
-        observations = np.append(image.reshape(-1), direction)
-        return observations
-
+        reward_n = np.array([[reward] for _ in range(self.n_agents)])
+        self.buf_info = copy.deepcopy(info)
+        info["episode_step"] = self._episode_step
+        info["episode_score"] = self._episode_score
+        truncated = True if self._episode_step >= self.max_cycles else False
+        return obs, state, reward_n, [terminated], [truncated], info
 
+    def get_avail_actions(self):
+        return self.env.get_avail_actions()
```

### Comparing `xuance-1.1.0/xuance/environment/starcraft2/sc2_vec_env.py` & `xuance-1.1.1/xuance/environment/starcraft2/sc2_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/vector_envs/env_utils.py` & `xuance-1.1.1/xuance/environment/vector_envs/env_utils.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/vector_envs/subproc_vec_env.py` & `xuance-1.1.1/xuance/environment/vector_envs/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/environment/vector_envs/vector_env.py` & `xuance-1.1.1/xuance/environment/vector_envs/vector_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/__init__.py` & `xuance-1.1.1/xuance/mindspore/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/agent.py` & `xuance-1.1.1/xuance/mindspore/agents/agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/agents_marl.py` & `xuance-1.1.1/xuance/mindspore/agents/agents_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/coma_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/isac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/masac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.1/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/a2c_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ddpg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/pdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pg_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/pg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/ppokl_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sac_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/sac_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/sacdis_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/spdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/td3_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/policy_gradient/td3_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/C51_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/C51_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/ddqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/drqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/perdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py` & `xuance-1.1.1/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/__init__.py` & `xuance-1.1.1/xuance/mindspore/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/learner.py` & `xuance-1.1.1/xuance/mindspore/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/isac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/masac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sac_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/sac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/sacdis_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/spdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/td3_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/policy_gradient/td3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/c51_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/ddqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/dqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/perdqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/perdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py` & `xuance-1.1.1/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/__init__.py` & `xuance-1.1.1/xuance/mindspore/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/categorical.py` & `xuance-1.1.1/xuance/mindspore/policies/categorical.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/categorical_marl.py` & `xuance-1.1.1/xuance/mindspore/policies/categorical_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/coordination_graph.py` & `xuance-1.1.1/xuance/mindspore/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/deterministic.py` & `xuance-1.1.1/xuance/mindspore/policies/deterministic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/deterministic_marl.py` & `xuance-1.1.1/xuance/mindspore/policies/deterministic_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/gaussian.py` & `xuance-1.1.1/xuance/mindspore/policies/gaussian.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/gaussian_marl.py` & `xuance-1.1.1/xuance/mindspore/policies/gaussian_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/policies/mixers.py` & `xuance-1.1.1/xuance/mindspore/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/representations/__init__.py` & `xuance-1.1.1/xuance/mindspore/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/representations/cnn.py` & `xuance-1.1.1/xuance/mindspore/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/representations/mlp.py` & `xuance-1.1.1/xuance/mindspore/representations/mlp.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/representations/rnn.py` & `xuance-1.1.1/xuance/mindspore/representations/rnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/runners/runner_drl.py` & `xuance-1.1.1/xuance/mindspore/runners/runner_drl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/runners/runner_pettingzoo.py` & `xuance-1.1.1/xuance/mindspore/runners/runner_pettingzoo.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/__init__.py` & `xuance-1.1.1/xuance/mindspore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/distributions.py` & `xuance-1.1.1/xuance/mindspore/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/input_reformat.py` & `xuance-1.1.1/xuance/mindspore/utils/input_reformat.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/layers.py` & `xuance-1.1.1/xuance/mindspore/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/operations.py` & `xuance-1.1.1/xuance/mindspore/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/mindspore/utils/set_trainer.py` & `xuance-1.1.1/xuance/mindspore/utils/set_trainer.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/__init__.py` & `xuance-1.1.1/xuance/tensorflow/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/agents_marl.py` & `xuance-1.1.1/xuance/tensorflow/agents/agents_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.1/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/a2c_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pg_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/pg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppg_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sac_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/sac_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/td3_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/policy_gradient/td3_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/c51_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/c51_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/drqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py` & `xuance-1.1.1/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/__init__.py` & `xuance-1.1.1/xuance/tensorflow/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sac_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/sac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/td3_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/policy_gradient/td3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/c51_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/dqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py` & `xuance-1.1.1/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/__init__.py` & `xuance-1.1.1/xuance/tensorflow/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/categorical.py` & `xuance-1.1.1/xuance/tensorflow/policies/categorical.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/categorical_marl.py` & `xuance-1.1.1/xuance/tensorflow/policies/categorical_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/coordination_graph.py` & `xuance-1.1.1/xuance/tensorflow/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/deterministic.py` & `xuance-1.1.1/xuance/tensorflow/policies/deterministic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/deterministic_marl.py` & `xuance-1.1.1/xuance/tensorflow/policies/deterministic_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/gaussian.py` & `xuance-1.1.1/xuance/tensorflow/policies/gaussian.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/gaussian_marl.py` & `xuance-1.1.1/xuance/tensorflow/policies/gaussian_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/policies/mixers.py` & `xuance-1.1.1/xuance/tensorflow/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/representations/__init__.py` & `xuance-1.1.1/xuance/tensorflow/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/representations/cnn.py` & `xuance-1.1.1/xuance/tensorflow/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/representations/mlp.py` & `xuance-1.1.1/xuance/tensorflow/representations/mlp.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/runners/runner_basic.py` & `xuance-1.1.1/xuance/tensorflow/runners/runner_basic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/runners/runner_drl.py` & `xuance-1.1.1/xuance/tensorflow/runners/runner_drl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/runners/runner_pettingzoo.py` & `xuance-1.1.1/xuance/tensorflow/runners/runner_pettingzoo.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/utils/__init__.py` & `xuance-1.1.1/xuance/tensorflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/utils/distributions.py` & `xuance-1.1.1/xuance/tensorflow/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/utils/input_reformat.py` & `xuance-1.1.1/xuance/tensorflow/utils/input_reformat.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/utils/layers.py` & `xuance-1.1.1/xuance/tensorflow/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/tensorflow/utils/operations.py` & `xuance-1.1.1/xuance/tensorflow/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/__init__.py` & `xuance-1.1.1/xuance/torch/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/agents_marl.py` & `xuance-1.1.1/xuance/torch/agents/agents_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/__init__.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/coma_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
         self.start_greedy, self.end_greedy = config.start_greedy, config.end_greedy
         self.egreedy = self.start_greedy
         self.delta_egreedy = (self.start_greedy - self.end_greedy) / config.decay_step_greedy
 
         self.n_envs = envs.num_envs
-        self.n_size = config.n_size
         self.n_epoch = config.n_epoch
         self.n_minibatch = config.n_minibatch
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape[0], config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
@@ -58,15 +57,15 @@
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         config.act_onehot_shape = config.act_shape + tuple([config.dim_act])
 
         buffer = COMA_Buffer_RNN if self.use_recurrent else COMA_Buffer
         input_buffer = (config.n_agents, config.state_space.shape, config.obs_shape, config.act_shape, config.rew_shape,
-                        config.done_shape, envs.num_envs, config.n_size,
+                        config.done_shape, envs.num_envs, config.buffer_size,
                         config.use_gae, config.use_advnorm, config.gamma, config.gae_lambda)
         memory = buffer(*input_buffer, max_episode_length=envs.max_episode_length,
                         dim_act=config.dim_act, td_lambda=config.td_lambda)
         self.buffer_size = memory.buffer_size
         self.batch_size = self.buffer_size // self.n_minibatch
 
         learner = COMA_Learner(config, policy, optimizer, scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
+        self.representation_info_shape = policy.representation_info_shape
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(config.n_agents,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/ippo_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     """
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
         self.n_envs = envs.num_envs
-        self.n_size = config.n_size
         self.n_epoch = config.n_epoch
         self.n_minibatch = config.n_minibatch
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape[0], config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
@@ -49,15 +48,15 @@
                                      weight_decay=config.weight_decay)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
         buffer = MARL_OnPolicyBuffer_RNN if self.use_recurrent else MARL_OnPolicyBuffer
         input_buffer = (config.n_agents, config.state_space.shape, config.obs_shape, config.act_shape, config.rew_shape,
-                        config.done_shape, envs.num_envs, config.n_size,
+                        config.done_shape, envs.num_envs, config.buffer_size,
                         config.use_gae, config.use_advnorm, config.gamma, config.gae_lambda)
         memory = buffer(*input_buffer, max_episode_length=envs.max_episode_length, dim_act=config.dim_act)
         self.buffer_size = memory.buffer_size
         self.batch_size = self.buffer_size // self.n_minibatch
 
         learner = IPPO_Learner(config, policy, optimizer, None, config.device, config.model_dir, config.gamma)
         super(IPPO_Agents, self).__init__(config, envs, policy, memory, learner, device,
@@ -103,25 +102,23 @@
             values_n = values_n.squeeze(2)
         else:
             hidden_state, values_n = self.policy.get_values(critic_in, agents_id)
 
         return hidden_state, values_n.detach().cpu().numpy()
 
     def train(self, i_step, **kwargs):
+        info_train = {}
         if self.memory.full:
-            info_train = {}
             indexes = np.arange(self.buffer_size)
             for _ in range(self.n_epoch):
                 np.random.shuffle(indexes)
                 for start in range(0, self.buffer_size, self.batch_size):
                     end = start + self.batch_size
                     sample_idx = indexes[start:end]
                     sample = self.memory.sample(sample_idx)
                     if self.use_recurrent:
                         info_train = self.learner.update_recurrent(sample)
                     else:
                         info_train = self.learner.update(sample)
             self.learner.lr_decay(i_step)
             self.memory.clear()
-            return info_train
-        else:
-            return {}
+        return info_train
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/matd3_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class ISAC_Agents(MARLAgents):
-    """The implementation of Independent SAC agents.
+class MATD3_Agents(MARLAgents):
+    """The implementation of MATD3 agents.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         device: the calculating device of the model, such as CPU or GPU.
     """
     def __init__(self,
@@ -23,15 +23,15 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
+        self.representation_info_shape = policy.representation_info_shape
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(config.n_agents,
@@ -39,25 +39,28 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = ISAC_Learner(config, policy, optimizer, scheduler,
-                               config.device, config.model_dir, config.gamma)
-        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
-                                          config.log_dir, config.model_dir)
+        learner = MATD3_Learner(config, policy, optimizer, scheduler,
+                                config.device, config.model_dir, config.gamma, delay=config.delay)
+        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, device,
+                                           config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, dists = self.policy(obs_n, agents_id)
-        acts = dists.rsample()
-        actions = acts.cpu().detach().numpy()
-        return None, actions
+        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
+        actions = actions.cpu().detach().numpy()
+        if test_mode:
+            return None, actions
+        else:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=config.running_steps),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=config.running_steps)]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
+        self.representation_info_shape = policy.representation_info_shape
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(config.n_agents,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mappo_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                                      weight_decay=config.weight_decay)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
         buffer = MARL_OnPolicyBuffer_RNN if self.use_recurrent else MARL_OnPolicyBuffer
         input_buffer = (config.n_agents, config.state_space.shape, config.obs_shape, config.act_shape, config.rew_shape,
-                        config.done_shape, envs.num_envs, config.n_size,
+                        config.done_shape, envs.num_envs, config.buffer_size,
                         config.use_gae, config.use_advnorm, config.gamma, config.gae_lambda)
         memory = buffer(*input_buffer, max_episode_length=envs.max_episode_length, dim_act=config.dim_act)
         self.buffer_size = memory.buffer_size
         self.batch_size = self.buffer_size // self.n_minibatch
 
         learner = MAPPO_Clip_Learner(config, policy, optimizer, None, config.device, config.model_dir, config.gamma)
         super(MAPPO_Agents, self).__init__(config, envs, policy, memory, learner, device,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/masac_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
+        self.representation_info_shape = policy.representation_info_shape
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(config.n_agents,
@@ -39,25 +39,25 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, scheduler,
-                                config.device, config.model_dir, config.gamma)
+        learner = MASAC_Learner(config, policy, optimizer, scheduler, config.device, config.model_dir,
+                                use_automatic_entropy_tuning=config.use_automatic_entropy_tuning,
+                                target_entropy=-policy.action_dim,
+                                lr_policy=config.lr_a)
         super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
                                            config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, dists = self.policy(obs_n, agents_id)
-        acts = dists.rsample()
-        actions = acts.cpu().detach().numpy()
-        return None, actions
+        _, actions = self.policy(obs_n, agents_id)
+        return None, actions.cpu().detach().numpy()
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/isac_agents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class MATD3_Agents(MARLAgents):
-    """The implementation of MATD3 agents.
+class ISAC_Agents(MARLAgents):
+    """The implementation of Independent SAC agents.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         device: the calculating device of the model, such as CPU or GPU.
     """
     def __init__(self,
@@ -23,15 +23,15 @@
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
+        self.representation_info_shape = policy.representation_info_shape
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
         memory = MARL_OffPolicyBuffer(config.n_agents,
@@ -39,28 +39,25 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MATD3_Learner(config, policy, optimizer, scheduler,
-                                config.device, config.model_dir, config.gamma)
-        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, device,
-                                           config.log_dir, config.model_dir)
+        learner = ISAC_Learner(config, policy, optimizer, scheduler, config.device, config.model_dir,
+                               use_automatic_entropy_tuning=config.use_automatic_entropy_tuning,
+                               target_entropy=-policy.action_dim,
+                               lr_policy=config.lr_a)
+        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
+                                          config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        _, actions = self.policy(torch.Tensor(obs_n), agents_id)
-        actions = actions.cpu().detach().numpy()
-        if test_mode:
-            return None, actions
-        else:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-            return None, actions
+        _, actions = self.policy(obs_n, agents_id)
+        return None, actions.cpu().detach().numpy()
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mfac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/mfq_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/vdac_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     """
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
         self.n_envs = envs.num_envs
-        self.n_size = config.n_size
         self.n_epoch = config.n_epoch
         self.n_minibatch = config.n_minibatch
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
@@ -50,38 +49,40 @@
                                      weight_decay=config.weight_decay)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
         buffer = MARL_OnPolicyBuffer_RNN if self.use_recurrent else MARL_OnPolicyBuffer
         input_buffer = (config.n_agents, config.state_space.shape, config.obs_shape, config.act_shape, config.rew_shape,
-                        config.done_shape, envs.num_envs, config.n_size,
+                        config.done_shape, envs.num_envs, config.buffer_size,
                         config.use_gae, config.use_advnorm, config.gamma, config.gae_lambda)
         memory = buffer(*input_buffer, max_episode_length=envs.max_episode_length, dim_act=config.dim_act)
         self.buffer_size = memory.buffer_size
         self.batch_size = self.buffer_size // self.n_minibatch
 
         learner = VDAC_Learner(config, policy, optimizer, None, config.device, config.model_dir, config.gamma)
         super(VDAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
                                           config.log_dir, config.model_dir)
         self.share_values = True if config.rew_shape[0] == 1 else False
         self.on_policy = True
 
     def act(self, obs_n, *rnn_hidden, avail_actions=None, state=None, test_mode=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        obs_in = torch.Tensor(obs_n).view([batch_size, self.n_agents, -1]).to(self.device)
+        obs_in = torch.Tensor(obs_n).reshape([batch_size, self.n_agents, -1]).to(self.device)
         if state is not None:
             state = torch.Tensor(state).to(self.device)
+        if avail_actions is not None:
+            avail_actions = torch.Tensor(avail_actions).to(self.device)
         if self.use_recurrent:
             batch_agents = batch_size * self.n_agents
-            hidden_state, dists, values_tot = self.policy(obs_in.view(batch_agents, 1, -1),
-                                                          agents_id.unsqueeze(2),
+            hidden_state, dists, values_tot = self.policy(obs_in.reshape(batch_agents, 1, -1),
+                                                          agents_id.reshape(batch_agents, 1, -1),
                                                           *rnn_hidden,
-                                                          avail_actions=avail_actions[:, :, np.newaxis],
+                                                          avail_actions=avail_actions.reshape(batch_agents, 1, -1),
                                                           state=state.unsqueeze(2))
             actions = dists.stochastic_sample()
             actions = actions.reshape(batch_size, self.n_agents)
             values_tot = values_tot.reshape([batch_size, self.n_agents, 1])
         else:
             hidden_state, dists, values_tot = self.policy(obs_in, agents_id,
                                                           avail_actions=avail_actions,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.1/xuance/torch/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/a2c_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,34 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
+        self.horizon_size = config.horizon_size
         self.n_epoch = config.n_epoch
         self.n_minibatch = config.n_minibatch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.clip_grad = config.clip_grad
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
-        self.buffer_size = self.n_envs * self.n_steps
+        self.buffer_size = self.n_envs * self.horizon_size
         self.batch_size = self.buffer_size // self.n_minibatch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        self.n_steps,
+                        self.horizon_size,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = A2C_Learner(policy,
                               optimizer,
                               scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/ddpg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.action_space,
                                       self.auxiliary_info_shape,
                                       self.n_envs,
-                                      config.n_size,
+                                      config.buffer_size,
                                       config.batch_size)
         learner = DDPG_Learner(policy,
                                optimizer,
                                scheduler,
                                config.device,
                                config.model_dir,
                                config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/mpdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.epsilon_final = 0.1
         self.buffer_action_space = spaces.Box(np.zeros(4), np.ones(4), dtype=np.float64)
 
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.buffer_action_space,
                                       self.auxiliary_info_shape,
                                       self.n_envs,
-                                      config.n_size,
+                                      config.buffer_size,
                                       config.batch_size)
         learner = MPDQN_Learner(policy,
                                 optimizer,
                                 scheduler,
                                 config.device,
                                 config.model_dir,
                                 config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/pdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.epsilon_final = 0.1
         self.buffer_action_space = spaces.Box(np.zeros(4), np.ones(4), dtype=np.float64)
 
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.buffer_action_space,
                                       self.auxiliary_info_shape,
                                       self.n_envs,
-                                      config.n_size,
+                                      config.buffer_size,
                                       config.batch_size)
         learner = PDQN_Learner(policy,
                                optimizer,
                                scheduler,
                                config.device,
                                config.model_dir,
                                config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/pg_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/pg_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,34 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
+        self.horizon_size = config.horizon_size
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.clip_grad = config.clip_grad
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
-        self.buffer_size = self.n_envs * self.n_steps
+        self.buffer_size = self.n_envs * self.horizon_size
         self.batch_size = self.buffer_size // self.n_epoch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        self.n_steps,
+                        self.horizon_size,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = PG_Learner(policy,
                              optimizer,
                              scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/ppg_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,35 +17,35 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
+        self.horizon_size = config.horizon_size
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
         self.policy_nepoch = config.policy_nepoch
         self.value_nepoch = config.value_nepoch
         self.aux_nepoch = config.aux_nepoch
         
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.actor_representation.output_shapes
         self.auxiliary_info_shape = {"old_dist": None}
 
-        self.buffer_size = self.n_envs * self.n_steps
+        self.buffer_size = self.n_envs * self.horizon_size
         self.batch_size = self.buffer_size // self.n_epoch
         memory = DummyOnPolicyBuffer(self.observation_space,
                                      self.action_space,
                                      self.auxiliary_info_shape,
                                      self.n_envs,
-                                     self.n_steps,
+                                     self.horizon_size,
                                      config.use_gae,
                                      config.use_advnorm,
                                      self.gamma,
                                      self.gae_lam)
         learner = PPG_Learner(policy,
                               optimizer,
                               scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/ppoclip_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,33 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
+        self.horizon_size = config.horizon_size
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {"old_logp": ()}
 
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
-        self.buffer_size = self.n_envs * self.n_steps
+        self.buffer_size = self.n_envs * self.horizon_size
         self.batch_size = self.buffer_size // self.n_minibatch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        self.n_steps,
+                        self.horizon_size,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = PPOCLIP_Learner(policy,
                                   optimizer,
                                   scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/ppokl_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,33 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
+        self.horizon_size = config.horizon_size
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {"old_dist": None}
 
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer_Atari
-        self.buffer_size = self.n_envs * self.n_steps
+        self.buffer_size = self.n_envs * self.horizon_size
         self.batch_size = self.buffer_size // self.n_minibatch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        self.n_steps,
+                        self.horizon_size,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = PPOKL_Learner(policy,
                                 optimizer,
                                 scheduler,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/sac_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/qrdqn_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,105 @@
 from xuance.torch.agents import *
 
 
-class SAC_Agent(Agent):
-    """The implementation of SAC agent.
+class QRDQN_Agent(Agent):
+    """The implementation of QRDQN agent.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
         device: the calculating device of the model, such as CPU or GPU.
     """
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
-                 optimizer: Sequence[torch.optim.Optimizer],
-                 scheduler: Optional[Sequence[torch.optim.lr_scheduler._LRScheduler]] = None,
+                 optimizer: torch.optim.Optimizer,
+                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
 
         self.gamma = config.gamma
         self.train_frequency = config.training_frequency
         self.start_training = config.start_training
-        self.start_noise = config.start_noise
-        self.end_noise = config.end_noise
-        self.noise_scale = config.start_noise
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
-        memory = DummyOffPolicyBuffer(self.observation_space,
-                                      self.action_space,
-                                      self.auxiliary_info_shape,
-                                      self.n_envs,
-                                      config.n_size,
-                                      config.batch_size)
-        learner = SAC_Learner(policy,
-                              optimizer,
-                              scheduler,
-                              config.device,
-                              config.model_dir,
-                              config.gamma,
-                              config.tau)
-        super(SAC_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
-
-    def _action(self, obs):
-        _, act_dist = self.policy(obs)
-        action = act_dist.rsample()
-        action = action.detach().cpu().numpy()
+        self.atari = True if config.env_name == "Atari" else False
+        Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
+        memory = Buffer(self.observation_space,
+                        self.action_space,
+                        self.auxiliary_info_shape,
+                        self.n_envs,
+                        config.buffer_size,
+                        config.batch_size)
+        learner = QRDQN_Learner(policy,
+                                optimizer,
+                                scheduler,
+                                config.device,
+                                config.model_dir,
+                                config.gamma,
+                                config.sync_frequency)
+        super(QRDQN_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                          config.log_dir, config.model_dir)
+
+    def _action(self, obs, egreedy=0.0):
+        _, argmax_action, _ = self.policy(obs)
+        random_action = np.random.choice(self.action_space.n, self.n_envs)
+        if np.random.rand() < egreedy:
+            action = random_action
+        else:
+            action = argmax_action.detach().cpu().numpy()
         return action
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs)
-            if self.current_step < self.start_training:
-                acts = [self.action_space.sample() for _ in range(self.n_envs)]
-
+            acts = self._action(obs, self.egreedy)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
+
             self.memory.store(obs, acts, self._process_reward(rewards), terminals, self._process_observation(next_obs))
-            if (self.current_step > self.start_training) and (self.current_step % self.train_frequency == 0):
+            if self.current_step > self.start_training and self.current_step % self.train_frequency == 0:
+                # training
                 obs_batch, act_batch, rew_batch, terminal_batch, next_batch = self.memory.sample()
                 step_info = self.learner.update(obs_batch, act_batch, rew_batch, next_batch, terminal_batch)
+                step_info["epsilon-greedy"] = self.egreedy
                 self.log_infos(step_info, self.current_step)
 
-            self.returns = self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
-                    obs[i] = infos[i]["reset_obs"]
-                    self.ret_rms.update(self.returns[i:i + 1])
-                    self.returns[i] = 0.0
-                    self.current_episode[i] += 1
-                    if self.use_wandb:
-                        step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
-                        step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
+                    if self.atari and (~trunctions[i]):
+                        pass
                     else:
-                        step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
-                        step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
-                    self.log_infos(step_info, self.current_step)
+                        obs[i] = infos[i]["reset_obs"]
+                        self.current_episode[i] += 1
+                        if self.use_wandb:
+                            step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
+                            step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
+                        else:
+                            step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
+                            step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
+                        self.log_infos(step_info, self.current_step)
 
             self.current_step += self.n_envs
+            if self.egreedy > self.end_greedy:
+                self.egreedy = self.egreedy - (self.start_greedy - self.end_greedy) / self.config.decay_step_greedy
 
     def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
         obs, infos = test_envs.reset()
@@ -99,32 +107,35 @@
             images = test_envs.render(self.config.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
 
         while current_episode < test_episodes:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs)
+            acts = self._action(obs, egreedy=0.0)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
-            if self.config.render and self.config.render_mode == "rgb_array":
+            if self.config.render_mode == "rgb_array" and self.render:
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
             for i in range(num_envs):
                 if terminals[i] or trunctions[i]:
-                    obs[i] = infos[i]["reset_obs"]
-                    scores.append(infos[i]["episode_score"])
-                    current_episode += 1
-                    if best_score < infos[i]["episode_score"]:
-                        best_score = infos[i]["episode_score"]
-                        episode_videos = videos[i].copy()
-                    if self.config.test_mode:
-                        print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
+                    if self.atari and (~trunctions[i]):
+                        pass
+                    else:
+                        obs[i] = infos[i]["reset_obs"]
+                        scores.append(infos[i]["episode_score"])
+                        current_episode += 1
+                        if best_score < infos[i]["episode_score"]:
+                            best_score = infos[i]["episode_score"]
+                            episode_videos = videos[i].copy()
+                        if self.config.test_mode:
+                            print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
             self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/sac_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class SACDIS_Agent(Agent):
-    """The implementation of SAC agent with discrete actions.
+class SAC_Agent(Agent):
+    """The implementation of SAC agent.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
@@ -21,77 +21,71 @@
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
 
         self.gamma = config.gamma
         self.train_frequency = config.training_frequency
         self.start_training = config.start_training
-        self.start_noise = config.start_noise
-        self.end_noise = config.end_noise
-        self.noise_scale = config.start_noise
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
-        self.atari = True if config.env_name == "Atari" else False
-        Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
-        memory = Buffer(self.observation_space,
-                        self.action_space,
-                        self.auxiliary_info_shape,
-                        self.n_envs,
-                        config.n_size,
-                        config.batch_size)
-        learner = SACDIS_Learner(policy,
-                                 optimizer,
-                                 scheduler,
-                                 config.device,
-                                 config.model_dir,
-                                 config.gamma,
-                                 config.tau)
-        super(SACDIS_Agent, self).__init__(config, envs, policy, memory, learner, device,
-                                           config.log_dir, config.model_dir)
+
+        memory = DummyOffPolicyBuffer(self.observation_space,
+                                      self.action_space,
+                                      self.auxiliary_info_shape,
+                                      self.n_envs,
+                                      config.buffer_size,
+                                      config.batch_size)
+        learner = SAC_Learner(policy, optimizer, scheduler, config.device, config.model_dir,
+                              gamma=config.gamma,
+                              tau=config.tau,
+                              alpha=config.alpha,
+                              use_automatic_entropy_tuning=config.use_automatic_entropy_tuning,
+                              target_entropy=-np.prod(self.action_space.shape).item(),
+                              lr_policy=config.actor_learning_rate)
+        super(SAC_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
 
     def _action(self, obs):
-        _, act_prob, act_distribution = self.policy(obs)
-        action = act_distribution.sample()
-        action = action.detach().cpu().numpy()
-        return action
+        _, action = self.policy(obs)
+        return action.detach().cpu().numpy()
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
             acts = self._action(obs)
+            if self.current_step < self.start_training:
+                acts = [self.action_space.sample() for _ in range(self.n_envs)]
+
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
             self.memory.store(obs, acts, self._process_reward(rewards), terminals, self._process_observation(next_obs))
-            if self.current_step > self.start_training and self.current_step % self.train_frequency == 0:
+            if (self.current_step > self.start_training) and (self.current_step % self.train_frequency == 0):
                 obs_batch, act_batch, rew_batch, terminal_batch, next_batch = self.memory.sample()
                 step_info = self.learner.update(obs_batch, act_batch, rew_batch, next_batch, terminal_batch)
                 self.log_infos(step_info, self.current_step)
 
             self.returns = self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
-                    if self.atari and (~trunctions[i]):
-                        pass
+                    obs[i] = infos[i]["reset_obs"]
+                    self.ret_rms.update(self.returns[i:i + 1])
+                    self.returns[i] = 0.0
+                    self.current_episode[i] += 1
+                    if self.use_wandb:
+                        step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
+                        step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                     else:
-                        obs[i] = infos[i]["reset_obs"]
-                        self.ret_rms.update(self.returns[i:i + 1])
-                        self.returns[i] = 0.0
-                        self.current_episode[i] += 1
-                        if self.use_wandb:
-                            step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
-                            step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
-                        else:
-                            step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
-                            step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
-                        self.log_infos(step_info, self.current_step)
+                        step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
+                        step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
+                    self.log_infos(step_info, self.current_step)
+
             self.current_step += self.n_envs
 
     def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
@@ -102,33 +96,30 @@
                 videos[idx].append(img)
 
         while current_episode < test_episodes:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
             acts = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
-            if self.config.render_mode == "rgb_array" and self.render:
+            if self.config.render and self.config.render_mode == "rgb_array":
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
             for i in range(num_envs):
                 if terminals[i] or trunctions[i]:
-                    if self.atari and (~trunctions[i]):
-                        pass
-                    else:
-                        obs[i] = infos[i]["reset_obs"]
-                        scores.append(infos[i]["episode_score"])
-                        current_episode += 1
-                        if best_score < infos[i]["episode_score"]:
-                            best_score = infos[i]["episode_score"]
-                            episode_videos = videos[i].copy()
-                        if self.config.test_mode:
-                            print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
+                    obs[i] = infos[i]["reset_obs"]
+                    scores.append(infos[i]["episode_score"])
+                    current_episode += 1
+                    if best_score < infos[i]["episode_score"]:
+                        best_score = infos[i]["episode_score"]
+                        episode_videos = videos[i].copy()
+                    if self.config.test_mode:
+                        print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
             self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/spdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.epsilon_final = 0.1
         self.buffer_action_space = spaces.Box(np.zeros(4), np.ones(4), dtype=np.float64)
 
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.buffer_action_space,
                                       self.auxiliary_info_shape,
                                       self.n_envs,
-                                      config.n_size,
+                                      config.buffer_size,
                                       config.batch_size)
         learner = SPDQN_Learner(policy,
                                 optimizer,
                                 scheduler,
                                 config.device,
                                 config.model_dir,
                                 config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/policy_gradient/td3_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/td3_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,28 +33,28 @@
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
 
         memory = DummyOffPolicyBuffer(self.observation_space,
                                       self.action_space,
                                       self.auxiliary_info_shape,
                                       self.n_envs,
-                                      config.n_size,
+                                      config.buffer_size,
                                       config.batch_size)
         learner = TD3_Learner(policy,
                               optimizer,
                               scheduler,
                               config.device,
                               config.model_dir,
                               config.gamma,
                               config.tau,
                               config.actor_update_delay)
         super(TD3_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
 
     def _action(self, obs, noise_scale=0.0):
-        _, action = self.policy.action(obs)
+        _, action = self.policy(obs)
         action = action.detach().cpu().numpy()
         action = action + np.random.normal(size=action.shape) * noise_scale
         return np.clip(action, -1, 1)
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/c51_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/c51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
         learner = C51_Learner(policy,
                               optimizer,
                               scheduler,
                               config.device,
                               config.model_dir,
                               config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/ddqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.auxiliary_info_shape = {}
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
         learner = DDQN_Learner(policy,
                                optimizer,
                                scheduler,
                                config.device,
                                config.model_dir,
                                config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/dqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.auxiliary_info_shape = {}
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
         learner = DQN_Learner(policy,
                               optimizer,
                               scheduler,
                               config.device,
                               config.model_dir,
                               config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/drqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.auxiliary_info_shape = {}
 
         self.atari = True if config.env_name == "Atari" else False
         memory = RecurrentOffPolicyBuffer(self.observation_space,
                                           self.action_space,
                                           self.auxiliary_info_shape,
                                           self.n_envs,
-                                          config.n_size,
+                                          config.buffer_size,
                                           config.batch_size,
                                           episode_length=envs.max_episode_length,
                                           lookup_length=config.lookup_length)
         learner = DRQN_Learner(policy,
                                optimizer,
                                scheduler,
                                config.device,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/dueldqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
         learner = DuelDQN_Learner(policy,
                                   optimizer,
                                   scheduler,
                                   config.device,
                                   config.model_dir,
                                   config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/noisydqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
         learner = DQN_Learner(policy,
                               optimizer,
                               scheduler,
                               config.device,
                               config.model_dir,
                               config.gamma,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/qlearning_family/perdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.PER_beta = config.PER_beta0
 
         self.atari = True if config.env_name == "Atari" else False
         memory = PerOffPolicyBuffer(self.observation_space,
                                     self.action_space,
                                     self.auxiliary_info_shape,
                                     self.n_envs,
-                                    config.n_size,
+                                    config.buffer_size,
                                     config.batch_size,
                                     config.PER_alpha)
         learner = PerDQN_Learner(policy,
                                  optimizer,
                                  scheduler,
                                  config.device,
                                  config.model_dir,
```

### Comparing `xuance-1.1.0/xuance/torch/agents/qlearning_family/qrdqn_agent.py` & `xuance-1.1.1/xuance/torch/agents/policy_gradient/sacdis_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,93 @@
 from xuance.torch.agents import *
 
 
-class QRDQN_Agent(Agent):
-    """The implementation of QRDQN agent.
+class SACDIS_Agent(Agent):
+    """The implementation of SAC agent with discrete actions.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
         device: the calculating device of the model, such as CPU or GPU.
     """
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
-                 optimizer: torch.optim.Optimizer,
-                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
+                 optimizer: Sequence[torch.optim.Optimizer],
+                 scheduler: Optional[Sequence[torch.optim.lr_scheduler._LRScheduler]] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
 
         self.gamma = config.gamma
         self.train_frequency = config.training_frequency
         self.start_training = config.start_training
-        self.start_greedy = config.start_greedy
-        self.end_greedy = config.end_greedy
-        self.egreedy = config.start_greedy
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
-
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
-                        config.n_size,
+                        config.buffer_size,
                         config.batch_size)
-        learner = QRDQN_Learner(policy,
-                                optimizer,
-                                scheduler,
-                                config.device,
-                                config.model_dir,
-                                config.gamma,
-                                config.sync_frequency)
-        super(QRDQN_Agent, self).__init__(config, envs, policy, memory, learner, device,
-                                          config.log_dir, config.model_dir)
-
-    def _action(self, obs, egreedy=0.0):
-        _, argmax_action, _ = self.policy(obs)
-        random_action = np.random.choice(self.action_space.n, self.n_envs)
-        if np.random.rand() < egreedy:
-            action = random_action
-        else:
-            action = argmax_action.detach().cpu().numpy()
-        return action
+        learner = SACDIS_Learner(policy, optimizer, scheduler, config.device, config.model_dir,
+                                 gamma=config.gamma,
+                                 tau=config.tau,
+                                 alpha=config.alpha,
+                                 use_automatic_entropy_tuning=config.use_automatic_entropy_tuning,
+                                 target_entropy=-np.prod(self.action_space.shape).item(),
+                                 lr_policy=config.actor_learning_rate)
+        super(SACDIS_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                           config.log_dir, config.model_dir)
+
+    def _action(self, obs):
+        _, action = self.policy(obs)
+        return action.detach().cpu().numpy()
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs, self.egreedy)
+            acts = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
-
             self.memory.store(obs, acts, self._process_reward(rewards), terminals, self._process_observation(next_obs))
             if self.current_step > self.start_training and self.current_step % self.train_frequency == 0:
-                # training
                 obs_batch, act_batch, rew_batch, terminal_batch, next_batch = self.memory.sample()
                 step_info = self.learner.update(obs_batch, act_batch, rew_batch, next_batch, terminal_batch)
-                step_info["epsilon-greedy"] = self.egreedy
                 self.log_infos(step_info, self.current_step)
 
+            self.returns = self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
                         obs[i] = infos[i]["reset_obs"]
+                        self.ret_rms.update(self.returns[i:i + 1])
+                        self.returns[i] = 0.0
                         self.current_episode[i] += 1
                         if self.use_wandb:
                             step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
                             step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                         else:
                             step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
                             step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
                         self.log_infos(step_info, self.current_step)
-
             self.current_step += self.n_envs
-            if self.egreedy > self.end_greedy:
-                self.egreedy = self.egreedy - (self.start_greedy - self.end_greedy) / self.config.decay_step_greedy
 
     def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
         obs, infos = test_envs.reset()
@@ -107,15 +95,15 @@
             images = test_envs.render(self.config.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
 
         while current_episode < test_episodes:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs, egreedy=0.0)
+            acts = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
             if self.config.render_mode == "rgb_array" and self.render:
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
```

### Comparing `xuance-1.1.0/xuance/torch/learners/__init__.py` & `xuance-1.1.1/xuance/torch/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/learner.py` & `xuance-1.1.1/xuance/torch/learners/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             "cuda:3": self.device,
             "cuda:4": self.device,
             "cuda:5": self.device,
             "cuda:6": self.device,
             "cuda:7": self.device
         }))
         print(f"Successfully load model from '{path}'.")
+        return path
 
     @abstractmethod
     def update(self, *args):
         raise NotImplementedError
 
 
 class LearnerMAS(ABC):
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/__init__.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/iddpg_learner.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,21 @@
         actions = torch.Tensor(sample['actions']).to(self.device)
         obs_next = torch.Tensor(sample['obs_next']).to(self.device)
         rewards = torch.Tensor(sample['rewards']).to(self.device)
         terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
         agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
         IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
 
-        q_eval = self.policy.critic(obs, actions, IDs)
-        q_next = self.policy.target_critic(obs_next, self.policy.target_actor(obs_next, IDs), IDs)
+        q_eval = self.policy.Qpolicy(obs, actions, IDs)
+        q_next = self.policy.Qtarget(obs_next, self.policy.Atarget(obs_next, IDs), IDs)
         q_target = rewards + (1-terminals) * self.args.gamma * q_next
 
         # calculate the loss function
         _, actions_eval = self.policy(obs, IDs)
-        loss_a = -(self.policy.critic(obs, actions_eval, IDs) * agent_mask).sum() / agent_mask.sum()
+        loss_a = -(self.policy.Qpolicy(obs, actions_eval, IDs) * agent_mask).sum() / agent_mask.sum()
         self.optimizer['actor'].zero_grad()
         loss_a.backward()
         torch.nn.utils.clip_grad_norm_(self.policy.parameters_actor, self.args.grad_clip_norm)
         self.optimizer['actor'].step()
         if self.scheduler['actor'] is not None:
             self.scheduler['actor'].step()
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/ippo_learner.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,31 +66,39 @@
 
         # entropy loss
         entropy = pi_dist.entropy().reshape(agent_mask.shape) * agent_mask
         loss_e = entropy.mean()
 
         # critic loss
         _, value_pred = self.policy.get_values(obs, IDs)
-        value_pred = value_pred
-        value_target = returns
+        value_pred = value_pred.reshape(-1, 1)
+        value_target = returns.reshape(-1, 1)
+        values = values.reshape(-1, 1)
+        agent_mask_flatten = agent_mask.reshape(-1, 1)
         if self.use_value_clip:
             value_clipped = values + (value_pred - values).clamp(-self.value_clip_range, self.value_clip_range)
+            if self.use_value_norm:
+                self.value_normalizer.update(value_target)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
                 loss_v = self.huber_loss(value_pred, value_target)
                 loss_v_clipped = self.huber_loss(value_clipped, value_target)
             else:
                 loss_v = (value_pred - value_target) ** 2
                 loss_v_clipped = (value_clipped - value_target) ** 2
-            loss_c = torch.max(loss_v, loss_v_clipped) * agent_mask
-            loss_c = loss_c.sum() / agent_mask.sum()
+            loss_c = torch.max(loss_v, loss_v_clipped) * agent_mask_flatten
+            loss_c = loss_c.sum() / agent_mask_flatten.sum()
         else:
+            if self.use_value_norm:
+                self.value_normalizer.update(value_target)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
-                loss_v = self.huber_loss(value_pred, value_target) * agent_mask
+                loss_v = self.huber_loss(value_pred, value_target) * agent_mask_flatten
             else:
-                loss_v = ((value_pred - value_target) ** 2) * agent_mask
+                loss_v = ((value_pred - value_target) ** 2) * agent_mask_flatten
             loss_c = loss_v.sum() / agent_mask.sum()
 
         loss = loss_a + self.vf_coef * loss_c - self.ent_coef * loss_e
         self.optimizer.zero_grad()
         loss.backward()
         if self.use_grad_norm:
             grad_norm = torch.nn.utils.clip_grad_norm_(self.policy.parameters(), self.max_grad_norm)
@@ -172,15 +180,15 @@
                 loss_v = (value_pred - value_target) ** 2
                 loss_v_clipped = (value_clipped - value_target) ** 2
             loss_c = torch.max(loss_v, loss_v_clipped) * filled_all
             loss_c = loss_c.sum() / filled_all.sum()
         else:
             if self.use_value_norm:
                 self.value_normalizer.update(value_target)
-                value_pred = self.value_normalizer.normalize(value_pred)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
                 loss_v = self.huber_loss(value_pred, value_target)
             else:
                 loss_v = (value_pred - value_target) ** 2
             loss_c = (loss_v * filled_all).sum() / filled_all.sum()
 
         loss = loss_a + self.vf_coef * loss_c - self.ent_coef * loss_e
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/matd3_learner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
-Independent Soft Actor-critic (ISAC)
-Implementation: Pytorch
+Multi-Agent TD3
 """
 from xuance.torch.learners import *
 
 
-class ISAC_Learner(LearnerMAS):
+class MATD3_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
                  optimizer: Sequence[torch.optim.Optimizer],
                  scheduler: Sequence[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
-                 sync_frequency: int = 100
+                 sync_frequency: int = 100,
+                 delay: int = 3
                  ):
         self.gamma = gamma
         self.tau = config.tau
-        self.alpha = config.alpha
+        self.delay = delay
         self.sync_frequency = sync_frequency
         self.mse_loss = nn.MSELoss()
-        super(ISAC_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
+        super(MATD3_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
         self.optimizer = {
             'actor': optimizer[0],
             'critic': optimizer[1]
         }
         self.scheduler = {
             'actor': scheduler[0],
             'critic': scheduler[1]
@@ -37,50 +37,46 @@
         actions = torch.Tensor(sample['actions']).to(self.device)
         obs_next = torch.Tensor(sample['obs_next']).to(self.device)
         rewards = torch.Tensor(sample['rewards']).to(self.device)
         terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
         agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
         IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
 
-        q_eval = self.policy.critic(obs, actions, IDs)
-        actions_next_dist = self.policy.target_actor(obs_next, IDs)
-        actions_next = actions_next_dist.rsample()
-        log_pi_a_next = actions_next_dist.log_prob(actions_next)
-        q_next = self.policy.target_critic(obs_next, actions_next, IDs)
-        q_target = rewards + (1-terminals) * self.args.gamma * (q_next - self.alpha * log_pi_a_next.unsqueeze(dim=-1))
-
-        # calculate the loss function
-        _, actions_dist = self.policy(obs, IDs)
-        actions_eval = actions_dist.rsample()
-        log_pi_a = actions_dist.log_prob(actions_eval)
-        loss_a = -(self.policy.critic(obs, actions_eval, IDs) - self.alpha * log_pi_a.unsqueeze(dim=-1) * agent_mask).sum() / agent_mask.sum()
-        # loss_a = (- self.policy.critic(obs, actions_eval, IDs)) * agent_mask.sum() / agent_mask.sum()
-        self.optimizer['actor'].zero_grad()
-        loss_a.backward()
-        torch.nn.utils.clip_grad_norm_(self.policy.parameters_actor, self.args.grad_clip_norm)
-        self.optimizer['actor'].step()
-        if self.scheduler['actor'] is not None:
-            self.scheduler['actor'].step()
-
-        td_error = (q_eval - q_target.detach()) * agent_mask
+        # actor update
+        if self.iterations % self.delay == 0:
+            _, actions_eval = self.policy(obs, IDs)
+            policy_q = self.policy.Qpolicy(obs, actions_eval, IDs) * agent_mask
+            p_loss = -policy_q.sum() / agent_mask.sum()
+            self.optimizer['actor'].zero_grad()
+            p_loss.backward()
+            self.optimizer['actor'].step()
+            if self.scheduler['actor'] is not None:
+                self.scheduler['actor'].step()
+            self.policy.soft_update(self.tau)
+
+        # train critic
+        action_q = self.policy.Qaction(obs, actions, IDs)
+        actions_next = self.policy.Atarget(obs_next, IDs)
+        q_next = self.policy.Qtarget(obs_next, actions_next, IDs)
+        q_target = rewards + (1 - terminals) * self.args.gamma * q_next
+        td_error = (action_q - q_target.detach()) * agent_mask
         loss_c = (td_error ** 2).sum() / agent_mask.sum()
+        # loss_c = F.mse_loss(torch.tile(q_target.detach(), (1, 2)), action_q)
         self.optimizer['critic'].zero_grad()
         loss_c.backward()
         torch.nn.utils.clip_grad_norm_(self.policy.parameters_critic, self.args.grad_clip_norm)
         self.optimizer['critic'].step()
         if self.scheduler['critic'] is not None:
             self.scheduler['critic'].step()
 
-        self.policy.soft_update(self.tau)
-
         lr_a = self.optimizer['actor'].state_dict()['param_groups'][0]['lr']
         lr_c = self.optimizer['critic'].state_dict()['param_groups'][0]['lr']
 
         info = {
             "learning_rate_actor": lr_a,
             "learning_rate_critic": lr_c,
-            "loss_actor": loss_a.item(),
-            "loss_critic": loss_c.item(),
-            "predictQ": q_eval.mean().item()
+            "loss_critic": loss_c.item()
         }
+        if self.iterations % self.delay == 0:
+            info["loss_actor"] = p_loss.item()
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/maddpg_learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,27 +41,27 @@
         rewards = torch.Tensor(sample['rewards']).to(self.device)
         terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
         agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
         IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
 
         # train actor
         _, actions_eval = self.policy(obs, IDs)
-        loss_a = -(self.policy.critic(obs, actions_eval, IDs) * agent_mask).sum() / agent_mask.sum()
+        loss_a = -(self.policy.Qpolicy(obs, actions_eval, IDs) * agent_mask).sum() / agent_mask.sum()
         self.optimizer['actor'].zero_grad()
         loss_a.backward()
         if self.args.use_grad_clip:
             torch.nn.utils.clip_grad_norm_(self.policy.parameters_actor, self.args.grad_clip_norm)
         self.optimizer['actor'].step()
         if self.scheduler['actor'] is not None:
             self.scheduler['actor'].step()
 
         # train critic
-        actions_next = self.policy.target_actor(obs_next, IDs)
-        q_eval = self.policy.critic(obs, actions, IDs)
-        q_next = self.policy.target_critic(obs_next, actions_next, IDs)
+        actions_next = self.policy.Atarget(obs_next, IDs)
+        q_eval = self.policy.Qpolicy(obs, actions, IDs)
+        q_next = self.policy.Qtarget(obs_next, actions_next, IDs)
         q_target = rewards + (1 - terminals) * self.args.gamma * q_next
         td_error = (q_eval - q_target.detach()) * agent_mask
         loss_c = (td_error ** 2).sum() / agent_mask.sum()
         self.optimizer['critic'].zero_grad()
         loss_c.backward()
         if self.args.use_grad_clip:
             torch.nn.utils.clip_grad_norm_(self.policy.parameters_critic, self.args.grad_clip_norm)
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mappo_learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                 loss_v = (value_pred - value_target) ** 2
                 loss_v_clipped = (value_clipped - value_target) ** 2
             loss_c = torch.max(loss_v, loss_v_clipped) * filled_all
             loss_c = loss_c.sum() / filled_all.sum()
         else:
             if self.use_value_norm:
                 self.value_normalizer.update(value_target)
-                value_pred = self.value_normalizer.normalize(value_target)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
                 loss_v = self.huber_loss(value_pred, value_target)
             else:
                 loss_v = (value_pred - value_target) ** 2
             loss_c = (loss_v * filled_all).sum() / filled_all.sum()
 
         loss = loss_a + self.vf_coef * loss_c - self.ent_coef * loss_e
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mfq_learner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,74 @@
 """
-Multi-agent Soft Actor-critic (MASAC)
+MFQ: Mean Field Q-Learning
+Paper link:
+http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
 Implementation: Pytorch
 """
 from xuance.torch.learners import *
 
 
-class MASAC_Learner(LearnerMAS):
+class MFQ_Learner(LearnerMAS):
     def __init__(self,
                  config: Namespace,
                  policy: nn.Module,
-                 optimizer: Sequence[torch.optim.Optimizer],
-                 scheduler: Sequence[torch.optim.lr_scheduler._LRScheduler] = None,
+                 optimizer: torch.optim.Optimizer,
+                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100
                  ):
         self.gamma = gamma
-        self.tau = config.tau
-        self.alpha = config.alpha
+        self.temperature = config.temperature
         self.sync_frequency = sync_frequency
         self.mse_loss = nn.MSELoss()
-        super(MASAC_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
-        self.optimizer = {
-            'actor': optimizer[0],
-            'critic': optimizer[1]
-        }
-        self.scheduler = {
-            'actor': scheduler[0],
-            'critic': scheduler[1]
-        }
+        self.softmax = torch.nn.Softmax(dim=-1)
+        super(MFQ_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
+
+    def get_boltzmann_policy(self, q):
+        return self.softmax(q / self.temperature)
 
     def update(self, sample):
         self.iterations += 1
         obs = torch.Tensor(sample['obs']).to(self.device)
         actions = torch.Tensor(sample['actions']).to(self.device)
         obs_next = torch.Tensor(sample['obs_next']).to(self.device)
+        act_mean = torch.Tensor(sample['act_mean']).to(self.device)
+        act_mean_next = torch.Tensor(sample['act_mean_next']).to(self.device)
         rewards = torch.Tensor(sample['rewards']).to(self.device)
         terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
         agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
         IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
 
-        q_eval = self.policy.critic(obs, actions, IDs)
-        actions_next_dist = self.policy.target_actor(obs_next, IDs)
-        actions_next = actions_next_dist.rsample()
-        log_pi_a_next = actions_next_dist.log_prob(actions_next)
-        q_next = self.policy.target_critic(obs_next, actions_next, IDs)
-        q_target = rewards + (1-terminals) * self.args.gamma * (q_next - self.alpha * log_pi_a_next.unsqueeze(dim=-1))
+        act_mean = act_mean.unsqueeze(1).repeat([1, self.n_agents, 1])
+        act_mean_next = act_mean_next.unsqueeze(1).repeat([1, self.n_agents, 1])
+        _, _, q_eval = self.policy(obs, act_mean, IDs)
+        q_eval_a = q_eval.gather(-1, actions.long().reshape([self.args.batch_size, self.n_agents, 1]))
+        q_next = self.policy.target_Q(obs_next, act_mean_next, IDs)
+        shape = q_next.shape
+        pi = self.get_boltzmann_policy(q_next)
+        v_mf = torch.bmm(q_next.reshape(-1, 1, shape[-1]), pi.unsqueeze(-1).reshape(-1, shape[-1], 1))
+        v_mf = v_mf.reshape(*(list(shape[0:-1]) + [1]))
+        q_target = rewards + (1 - terminals) * self.args.gamma * v_mf
 
         # calculate the loss function
-        _, actions_dist = self.policy(obs, IDs)
-        actions_eval = actions_dist.rsample()
-        log_pi_a = actions_dist.log_prob(actions_eval)
-        loss_a = -(self.policy.critic(obs, actions_eval, IDs) - self.alpha * log_pi_a.unsqueeze(dim=-1) * agent_mask).sum() / agent_mask.sum()
-        # loss_a = (- self.policy.critic(obs, actions_eval, IDs)) * agent_mask.sum() / agent_mask.sum()
-        self.optimizer['actor'].zero_grad()
-        loss_a.backward()
-        torch.nn.utils.clip_grad_norm_(self.policy.parameters_actor, self.args.grad_clip_norm)
-        self.optimizer['actor'].step()
-        if self.scheduler['actor'] is not None:
-            self.scheduler['actor'].step()
-
-        td_error = (q_eval - q_target.detach()) * agent_mask
-        loss_c = (td_error ** 2).sum() / agent_mask.sum()
-        self.optimizer['critic'].zero_grad()
-        loss_c.backward()
-        torch.nn.utils.clip_grad_norm_(self.policy.parameters_critic, self.args.grad_clip_norm)
-        self.optimizer['critic'].step()
-        if self.scheduler['critic'] is not None:
-            self.scheduler['critic'].step()
+        td_error = (q_eval_a - q_target.detach()) * agent_mask
+        loss = (td_error ** 2).sum() / agent_mask.sum()
+        self.optimizer.zero_grad()
+        loss.backward()
+        self.optimizer.step()
+        if self.scheduler is not None:
+            self.scheduler.step()
 
-        self.policy.soft_update(self.tau)
+        if self.iterations % self.sync_frequency == 0:
+            self.policy.copy_target()
 
-        lr_a = self.optimizer['actor'].state_dict()['param_groups'][0]['lr']
-        lr_c = self.optimizer['critic'].state_dict()['param_groups'][0]['lr']
+        lr = self.optimizer.state_dict()['param_groups'][0]['lr']
 
         info = {
-            "learning_rate_actor": lr_a,
-            "learning_rate_critic": lr_c,
-            "loss_actor": loss_a.item(),
-            "loss_critic": loss_c.item(),
-            "predictQ": q_eval.mean().item()
+            "learning_rate": lr,
+            "loss_Q": loss.item(),
+            "predictQ": q_eval_a.mean().item()
         }
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/sacdis_learner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-"""
-Multi-Agent TD3
-"""
 from xuance.torch.learners import *
 
 
-class MATD3_Learner(LearnerMAS):
+class SACDIS_Learner(Learner):
     def __init__(self,
-                 config: Namespace,
                  policy: nn.Module,
-                 optimizer: Sequence[torch.optim.Optimizer],
-                 scheduler: Sequence[torch.optim.lr_scheduler._LRScheduler] = None,
+                 optimizers: Sequence[torch.optim.Optimizer],
+                 schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
-                 gamma: float = 0.99,
-                 sync_frequency: int = 100,
-                 delay: int = 3
-                 ):
-        self.gamma = gamma
-        self.tau = config.tau
-        self.delay = delay
-        self.sync_frequency = sync_frequency
-        self.mse_loss = nn.MSELoss()
-        super(MATD3_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
-        self.optimizer = {
-            'actor': optimizer[0],
-            'critic': optimizer[1]
-        }
-        self.scheduler = {
-            'actor': scheduler[0],
-            'critic': scheduler[1]
-        }
+                 **kwargs):
+        self.tau = kwargs['tau']
+        self.gamma = kwargs['gamma']
+        self.alpha = kwargs['alpha']
+        self.use_automatic_entropy_tuning = kwargs['use_automatic_entropy_tuning']
+        super(SACDIS_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
+        if self.use_automatic_entropy_tuning:
+            self.target_entropy = kwargs['target_entropy']
+            self.log_alpha = nn.Parameter(torch.zeros(1, requires_grad=True, device=device))
+            self.alpha = self.log_alpha.exp()
+            self.alpha_optimizer = torch.optim.Adam([self.log_alpha], lr=kwargs['lr_policy'])
 
-    def update(self, sample):
+    def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
-        obs = torch.Tensor(sample['obs']).to(self.device)
-        actions = torch.Tensor(sample['actions']).to(self.device)
-        obs_next = torch.Tensor(sample['obs_next']).to(self.device)
-        rewards = torch.Tensor(sample['rewards']).to(self.device)
-        terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
-        agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
-        IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
-
-        # train critic
-        _, action_q = self.policy.Qaction(obs, actions, IDs)
-        actions_next = self.policy.target_actor(obs_next, IDs)
-        _, target_q = self.policy.Qtarget(obs_next, actions_next, IDs)
-        q_target = rewards + (1 - terminals) * self.args.gamma * target_q
-        td_error = (action_q - q_target.detach()) * agent_mask
-        loss_c = (td_error ** 2).sum() / agent_mask.sum()
-        # loss_c = F.mse_loss(torch.tile(q_target.detach(), (1, 2)), action_q)
-        self.optimizer['critic'].zero_grad()
-        loss_c.backward()
-        torch.nn.utils.clip_grad_norm_(self.policy.parameters_critic, self.args.grad_clip_norm)
-        self.optimizer['critic'].step()
-        if self.scheduler['critic'] is not None:
-            self.scheduler['critic'].step()
+        act_batch = torch.as_tensor(act_batch, device=self.device).unsqueeze(-1)
+        rew_batch = torch.as_tensor(rew_batch, device=self.device).unsqueeze(-1)
+        ter_batch = torch.as_tensor(terminal_batch, device=self.device).reshape([-1, 1])
 
         # actor update
-        if self.iterations % self.delay == 0:
-            _, actions_eval = self.policy(obs, IDs)
-            _, policy_q = self.policy.Qpolicy(obs, actions_eval, IDs)
-            p_loss = -policy_q.mean()
-            self.optimizer['actor'].zero_grad()
-            p_loss.backward()
-            self.optimizer['actor'].step()
-            if self.scheduler['actor'] is not None:
-                self.scheduler['actor'].step()
-            self.policy.soft_update(self.tau)
+        action_prob, log_pi, policy_q_1, policy_q_2 = self.policy.Qpolicy(obs_batch)
+        policy_q = torch.min(policy_q_1, policy_q_2)
+        p_loss = (action_prob * (self.alpha * log_pi - policy_q)).sum(dim=1).mean()
+        self.optimizer[0].zero_grad()
+        p_loss.backward()
+        self.optimizer[0].step()
+
+        # critic update
+        action_q_1, action_q_2 = self.policy.Qaction(obs_batch)
+        action_q_1 = action_q_1.gather(1, act_batch.long())
+        action_q_2 = action_q_2.gather(1, act_batch.long())
+        action_prob_next, log_pi_next, target_q = self.policy.Qtarget(next_batch)
+        target_q = action_prob_next * (target_q - self.alpha * log_pi_next)
+        target_q = target_q.sum(dim=1).unsqueeze(-1)
+        backup = rew_batch + (1 - ter_batch) * self.gamma * target_q
+        q_loss = F.mse_loss(action_q_1, backup.detach()) + F.mse_loss(action_q_2, backup.detach())
+        self.optimizer[1].zero_grad()
+        q_loss.backward()
+        self.optimizer[1].step()
+
+        # automatic entropy tuning
+        if self.use_automatic_entropy_tuning:
+            alpha_loss = -(self.log_alpha * (log_pi + self.target_entropy).detach()).mean()
+            self.alpha_optimizer.zero_grad()
+            alpha_loss.backward()
+            self.alpha_optimizer.step()
+            self.alpha = self.log_alpha.exp()
+        else:
+            alpha_loss = 0
+
+        if self.scheduler is not None:
+            self.scheduler[0].step()
+            self.scheduler[1].step()
+
+        self.policy.soft_update(self.tau)
 
-        lr_a = self.optimizer['actor'].state_dict()['param_groups'][0]['lr']
-        lr_c = self.optimizer['critic'].state_dict()['param_groups'][0]['lr']
+        actor_lr = self.optimizer[0].state_dict()['param_groups'][0]['lr']
+        critic_lr = self.optimizer[1].state_dict()['param_groups'][0]['lr']
 
         info = {
-            "learning_rate_actor": lr_a,
-            "learning_rate_critic": lr_c,
-            "loss_critic": loss_c.item()
+            "Qloss": q_loss.item(),
+            "Ploss": p_loss.item(),
+            "Qvalue": policy_q.mean().item(),
+            "actor_lr": actor_lr,
+            "critic_lr": critic_lr,
+            "alpha_loss": alpha_loss.item(),
+            "alpha": self.alpha.item(),
         }
-        if self.iterations % self.delay == 0:
-            info["loss_actor"] = p_loss.item()
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/qrdqn_learner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,45 @@
-"""
-MFQ: Mean Field Q-Learning
-Paper link:
-http://proceedings.mlr.press/v80/yang18d/yang18d.pdf
-Implementation: Pytorch
-"""
 from xuance.torch.learners import *
 
 
-class MFQ_Learner(LearnerMAS):
+class QRDQN_Learner(Learner):
     def __init__(self,
-                 config: Namespace,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
-                 sync_frequency: int = 100
-                 ):
+                 sync_frequency: int = 100):
         self.gamma = gamma
-        self.temperature = config.temperature
         self.sync_frequency = sync_frequency
-        self.mse_loss = nn.MSELoss()
-        self.softmax = torch.nn.Softmax(dim=-1)
-        super(MFQ_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
+        super(QRDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
 
-    def get_boltzmann_policy(self, q):
-        return self.softmax(q / self.temperature)
-
-    def update(self, sample):
+    def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
-        obs = torch.Tensor(sample['obs']).to(self.device)
-        actions = torch.Tensor(sample['actions']).to(self.device)
-        obs_next = torch.Tensor(sample['obs_next']).to(self.device)
-        act_mean = torch.Tensor(sample['act_mean']).to(self.device)
-        act_mean_next = torch.Tensor(sample['act_mean_next']).to(self.device)
-        rewards = torch.Tensor(sample['rewards']).to(self.device)
-        terminals = torch.Tensor(sample['terminals']).float().reshape(-1, self.n_agents, 1).to(self.device)
-        agent_mask = torch.Tensor(sample['agent_mask']).float().reshape(-1, self.n_agents, 1).to(self.device)
-        IDs = torch.eye(self.n_agents).unsqueeze(0).expand(self.args.batch_size, -1, -1).to(self.device)
-
-        act_mean = act_mean.unsqueeze(1).repeat([1, self.n_agents, 1])
-        act_mean_next = act_mean_next.unsqueeze(1).repeat([1, self.n_agents, 1])
-        _, _, q_eval = self.policy(obs, act_mean, IDs)
-        q_eval_a = q_eval.gather(-1, actions.long().reshape([self.args.batch_size, self.n_agents, 1]))
-        q_next = self.policy.target_Q(obs_next, act_mean_next, IDs)
-        shape = q_next.shape
-        pi = self.get_boltzmann_policy(q_next)
-        v_mf = torch.bmm(q_next.reshape(-1, 1, shape[-1]), pi.unsqueeze(-1).reshape(-1, shape[-1], 1))
-        v_mf = v_mf.reshape(*(list(shape[0:-1]) + [1]))
-        q_target = rewards + (1 - terminals) * self.args.gamma * v_mf
-
-        # calculate the loss function
-        td_error = (q_eval_a - q_target.detach()) * agent_mask
-        loss = (td_error ** 2).sum() / agent_mask.sum()
+        act_batch = torch.as_tensor(act_batch, device=self.device).long()
+        rew_batch = torch.as_tensor(rew_batch, device=self.device)
+        ter_batch = torch.as_tensor(terminal_batch, device=self.device)
+        _, _, evalZ = self.policy(obs_batch)
+        _, targetA, targetZ = self.policy(next_batch)
+
+        current_quantile = (evalZ * F.one_hot(act_batch, evalZ.shape[1]).unsqueeze(-1)).sum(1)
+        target_quantile = (targetZ * F.one_hot(targetA.detach(), evalZ.shape[1]).unsqueeze(-1)).sum(1).detach()
+        target_quantile = rew_batch.unsqueeze(1) + self.gamma * target_quantile * (1 - ter_batch.unsqueeze(1))
+
+        loss = F.mse_loss(target_quantile, current_quantile)
         self.optimizer.zero_grad()
         loss.backward()
         self.optimizer.step()
         if self.scheduler is not None:
             self.scheduler.step()
-
+        # hard update for target network
         if self.iterations % self.sync_frequency == 0:
             self.policy.copy_target()
-
         lr = self.optimizer.state_dict()['param_groups'][0]['lr']
 
         info = {
+            "Qloss": loss.item(),
             "learning_rate": lr,
-            "loss_Q": loss.item(),
-            "predictQ": q_eval_a.mean().item()
         }
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/vdac_learner.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,20 +100,20 @@
             self.device)
 
         filled_n = filled.unsqueeze(1).expand(batch_size, self.n_agents, episode_length, 1)
 
         # actor loss
         rnn_hidden = self.policy.representation.init_hidden(batch_size * self.n_agents)
         _, pi_dist, value_pred = self.policy(obs[:, :, :-1].reshape(-1, episode_length, self.dim_obs),
-                                             IDs[:, :, :-1],
+                                             IDs[:, :, :-1].reshape(-1, episode_length, self.n_agents),
                                              *rnn_hidden,
-                                             avail_actions=avail_actions[:, :, :-1],
+                                             avail_actions=avail_actions[:, :, :-1].reshape(-1, episode_length, self.dim_act),
                                              state=state[:, :-1])
-        log_pi = pi_dist.log_prob(actions).unsqueeze(-1)
-        entropy = pi_dist.entropy().unsqueeze(-1)
+        log_pi = pi_dist.log_prob(actions.reshape(-1, episode_length)).reshape(batch_size, self.n_agents, episode_length, 1)
+        entropy = pi_dist.entropy().reshape(batch_size, self.n_agents, episode_length, 1)
 
         targets = returns
         advantages = targets - value_pred
         td_error = value_pred - targets.detach()
 
         pg_loss = -((advantages.detach() * log_pi) * filled_n).sum() / filled_n.sum()
         vf_loss = ((td_error ** 2) * filled_n).sum() / filled_n.sum()
```

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.1/xuance/torch/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/ddpg_learner.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,20 +15,20 @@
         super(DDPG_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
+
         # critic update
-        action_q = self.policy.Qaction(obs_batch, act_batch)
-        # with torch.no_grad():
-        target_q = self.policy.Qtarget(next_batch)
-        backup = rew_batch + (1 - ter_batch) * self.gamma * target_q
-        q_loss = F.mse_loss(action_q, backup.detach())
+        action_q = self.policy.Qaction(obs_batch, act_batch).reshape([-1])
+        next_q = self.policy.Qtarget(next_batch).reshape([-1])
+        target_q = rew_batch + (1 - ter_batch) * self.gamma * next_q
+        q_loss = F.mse_loss(action_q, target_q.detach())
         self.optimizer[1].zero_grad()
         q_loss.backward()
         self.optimizer[1].step()
 
         # actor update
         policy_q = self.policy.Qpolicy(obs_batch)
         p_loss = -policy_q.mean()
```

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/pg_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/sac_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/spdqn_learner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 from xuance.torch.learners import *
 
 
-class SAC_Learner(Learner):
+class SPDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
                  tau: float = 0.01):
         self.tau = tau
         self.gamma = gamma
-        super(SAC_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
+        super(SPDQN_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
-        act_batch = torch.as_tensor(act_batch, device=self.device)
+        obs_batch = torch.as_tensor(obs_batch, device=self.device)
+        hyact_batch = torch.as_tensor(act_batch, device=self.device)
+        disact_batch = hyact_batch[:, 0].long()
+        conact_batch = hyact_batch[:, 1:]
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
+        next_batch = torch.as_tensor(next_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
-        # critic update
-        action_q = self.policy.Qaction(obs_batch, act_batch)
-        # with torch.no_grad():
-        log_pi_next, target_q = self.policy.Qtarget(next_batch)
-        backup = rew_batch + (1-ter_batch) * self.gamma * (target_q - 0.01 * log_pi_next.reshape([-1]))
-        q_loss = F.mse_loss(action_q, backup.detach())
+
+        # optimize Q-network
+        with torch.no_grad():
+            target_conact = self.policy.Atarget(next_batch)
+            target_q = self.policy.Qtarget(next_batch, target_conact)
+            target_q = torch.max(target_q, 1, keepdim=True)[0].squeeze()
+
+            target_q = rew_batch + (1 - ter_batch) * self.gamma * target_q
+
+        eval_qs = self.policy.Qeval(obs_batch, conact_batch)
+        eval_q = eval_qs.gather(1, disact_batch.view(-1, 1)).squeeze()
+        q_loss = F.mse_loss(eval_q, target_q)
+
         self.optimizer[1].zero_grad()
         q_loss.backward()
         self.optimizer[1].step()
 
-        # actor update
-        log_pi, policy_q = self.policy.Qpolicy(obs_batch)
-        p_loss = (0.01 * log_pi.reshape([-1]) - policy_q).mean()
+        # optimize actor network
+        policy_q = self.policy.Qpolicy(obs_batch)
+        p_loss = - policy_q.mean()
         self.optimizer[0].zero_grad()
         p_loss.backward()
         self.optimizer[0].step()
 
         if self.scheduler is not None:
             self.scheduler[0].step()
             self.scheduler[1].step()
 
         self.policy.soft_update(self.tau)
 
-        actor_lr = self.optimizer[0].state_dict()['param_groups'][0]['lr']
-        critic_lr = self.optimizer[1].state_dict()['param_groups'][0]['lr']
-
         info = {
-            "Qloss": q_loss.item(),
-            "Ploss": p_loss.item(),
-            "Qvalue": action_q.mean().item(),
-            "actor_lr": actor_lr,
-            "critic_lr": critic_lr
+            "Q_loss": q_loss.item(),
+            "P_loss": q_loss.item(),
+            'Qvalue': eval_q.mean().item()
         }
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/sac_learner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 from xuance.torch.learners import *
 
 
-class SACDIS_Learner(Learner):
+class SAC_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizers: Sequence[torch.optim.Optimizer],
                  schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
-                 gamma: float = 0.99,
-                 tau: float = 0.01):
-        self.tau = tau
-        self.gamma = gamma
-        super(SACDIS_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
+                 **kwargs):
+        self.tau = kwargs['tau']
+        self.gamma = kwargs['gamma']
+        self.alpha = kwargs['alpha']
+        self.use_automatic_entropy_tuning = kwargs['use_automatic_entropy_tuning']
+        super(SAC_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
+        if self.use_automatic_entropy_tuning:
+            self.target_entropy = kwargs['target_entropy']
+            self.log_alpha = nn.Parameter(torch.zeros(1, requires_grad=True, device=device))
+            self.alpha = self.log_alpha.exp()
+            self.alpha_optimizer = torch.optim.Adam([self.log_alpha], lr=kwargs['lr_policy'])
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
-        ter_batch = torch.as_tensor(terminal_batch, device=self.device).reshape([-1, 1])
-        act_batch = torch.unsqueeze(act_batch, -1)
-        # critic update
-        _, action_q = self.policy.Qaction(obs_batch)
-        action_q = action_q.gather(1, act_batch.long())
-        # with torch.no_grad():
-        action_prob_next, log_pi_next, target_q = self.policy.Qtarget(next_batch)
-        target_q = action_prob_next * (target_q - 0.01 * log_pi_next)
-        target_q = target_q.sum(dim=1).unsqueeze(-1)
-        rew = torch.unsqueeze(rew_batch, -1)
-        backup = rew + (1 - ter_batch) * self.gamma * target_q
-        q_loss = F.mse_loss(action_q, backup.detach())
-        self.optimizer[1].zero_grad()
-        q_loss.backward()
-        self.optimizer[1].step()
+        ter_batch = torch.as_tensor(terminal_batch, device=self.device)
 
         # actor update
-        action_prob, log_pi, policy_q = self.policy.Qpolicy(obs_batch)
-        inside_term = 0.01 * log_pi - policy_q
-        p_loss = (action_prob * inside_term).sum(dim=1).mean()
-        # p_loss = (inside_term).sum(dim=1).mean()
-        # p_loss = (0.01 * log_pi - policy_q).mean()
+        log_pi, policy_q_1, policy_q_2 = self.policy.Qpolicy(obs_batch)
+        policy_q = torch.min(policy_q_1, policy_q_2).reshape([-1])
+        p_loss = (self.alpha * log_pi.reshape([-1]) - policy_q).mean()
         self.optimizer[0].zero_grad()
         p_loss.backward()
         self.optimizer[0].step()
 
+        # critic update
+        action_q_1, action_q_2 = self.policy.Qaction(obs_batch, act_batch)
+        log_pi_next, target_q = self.policy.Qtarget(next_batch)
+        target_value = target_q - self.alpha * log_pi_next.reshape([-1])
+        backup = rew_batch + (1 - ter_batch) * self.gamma * target_value
+        q_loss = F.mse_loss(action_q_1, backup.detach()) + F.mse_loss(action_q_2, backup.detach())
+        self.optimizer[1].zero_grad()
+        q_loss.backward()
+        self.optimizer[1].step()
+
+        # automatic entropy tuning
+        if self.use_automatic_entropy_tuning:
+            alpha_loss = -(self.log_alpha * (log_pi + self.target_entropy).detach()).mean()
+            self.alpha_optimizer.zero_grad()
+            alpha_loss.backward()
+            self.alpha_optimizer.step()
+            self.alpha = self.log_alpha.exp()
+        else:
+            alpha_loss = 0
+
         if self.scheduler is not None:
             self.scheduler[0].step()
             self.scheduler[1].step()
 
         self.policy.soft_update(self.tau)
 
         actor_lr = self.optimizer[0].state_dict()['param_groups'][0]['lr']
         critic_lr = self.optimizer[1].state_dict()['param_groups'][0]['lr']
 
         info = {
             "Qloss": q_loss.item(),
             "Ploss": p_loss.item(),
-            "Qvalue": action_q.mean().item(),
+            "Qvalue": policy_q.mean().item(),
             "actor_lr": actor_lr,
-            "critic_lr": critic_lr
+            "critic_lr": critic_lr,
+            "alpha_loss": alpha_loss.item(),
+            "alpha": self.alpha.item(),
         }
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/ddqn_learner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 from xuance.torch.learners import *
 
 
-class SPDQN_Learner(Learner):
+class DDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
-                 optimizers: Sequence[torch.optim.Optimizer],
-                 schedulers: Sequence[torch.optim.lr_scheduler._LRScheduler],
+                 optimizer: torch.optim.Optimizer,
+                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
-                 tau: float = 0.01):
-        self.tau = tau
+                 sync_frequency: int = 100):
         self.gamma = gamma
-        super(SPDQN_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
+        self.sync_frequency = sync_frequency
+        super(DDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
-        obs_batch = torch.as_tensor(obs_batch, device=self.device)
-        hyact_batch = torch.as_tensor(act_batch, device=self.device)
-        disact_batch = hyact_batch[:, 0].long()
-        conact_batch = hyact_batch[:, 1:]
+        act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
-        next_batch = torch.as_tensor(next_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
 
-        # optimize Q-network
-        with torch.no_grad():
-            target_conact = self.policy.Atarget(next_batch)
-            target_q = self.policy.Qtarget(next_batch, target_conact)
-            target_q = torch.max(target_q, 1, keepdim=True)[0].squeeze()
-
-            target_q = rew_batch + (1 - ter_batch) * self.gamma * target_q
-
-        eval_qs = self.policy.Qeval(obs_batch, conact_batch)
-        eval_q = eval_qs.gather(1, disact_batch.view(-1, 1)).squeeze()
-        q_loss = F.mse_loss(eval_q, target_q)
-
-        self.optimizer[1].zero_grad()
-        q_loss.backward()
-        self.optimizer[1].step()
-
-        # optimize actor network
-        policy_q = self.policy.Qpolicy(obs_batch)
-        p_loss = - policy_q.mean()
-        self.optimizer[0].zero_grad()
-        p_loss.backward()
-        self.optimizer[0].step()
+        _, _, evalQ = self.policy(obs_batch)
+        _, targetA, targetQ = self.policy.target(next_batch)
 
+        targetA = F.one_hot(targetA, targetQ.shape[-1])
+        targetQ = (targetQ * targetA).sum(dim=-1)
+        targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
+        predictQ = (evalQ * F.one_hot(act_batch.long(), evalQ.shape[1])).sum(dim=-1)
+
+        loss = F.mse_loss(predictQ, targetQ)
+        self.optimizer.zero_grad()
+        loss.backward()
+        self.optimizer.step()
         if self.scheduler is not None:
-            self.scheduler[0].step()
-            self.scheduler[1].step()
+            self.scheduler.step()
 
-        self.policy.soft_update(self.tau)
+        # hard update for target network
+        if self.iterations % self.sync_frequency == 0:
+            self.policy.copy_target()
+
+        lr = self.optimizer.state_dict()['param_groups'][0]['lr']
 
         info = {
-            "Q_loss": q_loss.item(),
-            "P_loss": q_loss.item(),
-            'Qvalue': eval_q.mean().item()
+            "Qloss": loss.item(),
+            "learning_rate": lr,
+            "predictQ": predictQ.mean().item()
         }
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/policy_gradient/td3_learner.py` & `xuance-1.1.1/xuance/torch/learners/policy_gradient/td3_learner.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,45 +19,48 @@
         self.gamma = gamma
         self.delay = delay
         super(TD3_Learner, self).__init__(policy, optimizers, schedulers, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
-        rew_batch = torch.as_tensor(rew_batch, device=self.device).unsqueeze(dim=1)
-        ter_batch = torch.as_tensor(terminal_batch, device=self.device).unsqueeze(dim=1)
+        rew_batch = torch.as_tensor(rew_batch, device=self.device)
+        ter_batch = torch.as_tensor(terminal_batch, device=self.device)
 
         # critic update
-        _, action_q = self.policy.Qaction(obs_batch, act_batch)
-        _, target_q = self.policy.Qtarget(next_batch)
-        backup = rew_batch + self.gamma * (1 - ter_batch) * target_q
-        q_loss = F.mse_loss(torch.tile(backup.detach(), (1, 2)), action_q)
+        action_q_A, action_q_B = self.policy.Qaction(obs_batch, act_batch)
+        action_q_A = action_q_A.reshape([-1])
+        action_q_B = action_q_B.reshape([-1])
+        next_q = self.policy.Qtarget(next_batch).reshape([-1])
+        target_q = rew_batch + self.gamma * (1 - ter_batch) * next_q
+        q_loss = F.mse_loss(action_q_A, target_q.detach()) + F.mse_loss(action_q_B, target_q.detach())
         self.optimizer[1].zero_grad()
         q_loss.backward()
         self.optimizer[1].step()
         if self.scheduler is not None:
             self.scheduler[1].step()
 
         # actor update
         if self.iterations % self.delay == 0:
-            _, policy_q = self.policy.Qpolicy(obs_batch)
+            policy_q = self.policy.Qpolicy(obs_batch)
             p_loss = -policy_q.mean()
             self.optimizer[0].zero_grad()
             p_loss.backward()
             self.optimizer[0].step()
             if self.scheduler is not None:
                 self.scheduler[0].step()
             self.policy.soft_update(self.tau)
 
         actor_lr = self.optimizer[0].state_dict()['param_groups'][0]['lr']
         critic_lr = self.optimizer[1].state_dict()['param_groups'][0]['lr']
 
         info = {
             "Qloss": q_loss.item(),
-            "Qvalue": action_q.mean().item(),
+            "QvalueA": action_q_A.mean().item(),
+            "QvalueB": action_q_B.mean().item(),
             "actor_lr": actor_lr,
             "critic_lr": critic_lr
         }
         if self.iterations % self.delay == 0:
             info["Ploss"] = p_loss.item()
 
         return info
```

### Comparing `xuance-1.1.0/xuance/torch/learners/qlearning_family/c51_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/dqn_learner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 from xuance.torch.learners import *
 
 
-class DDQN_Learner(Learner):
+class DQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(DDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
+        super(DQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
 
         _, _, evalQ = self.policy(obs_batch)
-        _, targetA, targetQ = self.policy.target(next_batch)
-
-        targetA = F.one_hot(targetA, targetQ.shape[-1])
-        targetQ = (targetQ * targetA).sum(dim=-1)
+        _, _, targetQ = self.policy.target(next_batch)
+        targetQ = targetQ.max(dim=-1).values
         targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
         predictQ = (evalQ * F.one_hot(act_batch.long(), evalQ.shape[1])).sum(dim=-1)
 
         loss = F.mse_loss(predictQ, targetQ)
         self.optimizer.zero_grad()
         loss.backward()
         self.optimizer.step()
         if self.scheduler is not None:
             self.scheduler.step()
 
         # hard update for target network
         if self.iterations % self.sync_frequency == 0:
             self.policy.copy_target()
-
         lr = self.optimizer.state_dict()['param_groups'][0]['lr']
 
         info = {
             "Qloss": loss.item(),
             "learning_rate": lr,
             "predictQ": predictQ.mean().item()
         }
```

### Comparing `xuance-1.1.0/xuance/torch/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/dueldqn_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from xuance.torch.learners import *
 
 
-class DQN_Learner(Learner):
+class DuelDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(DQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
+        super(DuelDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
```

### Comparing `xuance-1.1.0/xuance/torch/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.1/xuance/torch/learners/qlearning_family/perdqn_learner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from xuance.torch.learners import *
 
 
-class DuelDQN_Learner(Learner):
+class PerDQN_Learner(Learner):
     def __init__(self,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None,
                  model_dir: str = "./",
                  gamma: float = 0.99,
                  sync_frequency: int = 100):
         self.gamma = gamma
         self.sync_frequency = sync_frequency
-        super(DuelDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
+        super(PerDQN_Learner, self).__init__(policy, optimizer, scheduler, device, model_dir)
 
     def update(self, obs_batch, act_batch, rew_batch, next_batch, terminal_batch):
         self.iterations += 1
         act_batch = torch.as_tensor(act_batch, device=self.device)
         rew_batch = torch.as_tensor(rew_batch, device=self.device)
         ter_batch = torch.as_tensor(terminal_batch, device=self.device)
 
         _, _, evalQ = self.policy(obs_batch)
         _, _, targetQ = self.policy.target(next_batch)
         targetQ = targetQ.max(dim=-1).values
         targetQ = rew_batch + self.gamma * (1 - ter_batch) * targetQ
         predictQ = (evalQ * F.one_hot(act_batch.long(), evalQ.shape[1])).sum(dim=-1)
 
+        td_error = targetQ - predictQ
         loss = F.mse_loss(predictQ, targetQ)
         self.optimizer.zero_grad()
         loss.backward()
         self.optimizer.step()
         if self.scheduler is not None:
             self.scheduler.step()
 
@@ -39,9 +40,9 @@
         lr = self.optimizer.state_dict()['param_groups'][0]['lr']
 
         info = {
             "Qloss": loss.item(),
             "learning_rate": lr,
             "predictQ": predictQ.mean().item()
         }
-
-        return info
+        
+        return np.abs(td_error.cpu().detach().numpy()), info
```

### Comparing `xuance-1.1.0/xuance/torch/policies/__init__.py` & `xuance-1.1.1/xuance/torch/policies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,19 +110,19 @@
                     "initialize", "activation", "activation_action", "device"],
     "SAC_Policy": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
                    "normalize", "initialize", "activation", "activation_action", "device"],
     "TD3_Policy": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
                    "normalize", "initialize", "activation", "activation_action", "device"],
     # DRL (hybrid action spaces) #
     "PDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                    'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
+                    'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'activation_action', 'device'],
     "MPDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
+                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'activation_action', 'device'],
     "SPDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
+                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'activation_action', 'device'],
     #  MARL policies (discrete action spaces) #
     "Basic_Q_network_marl": ["action_space", "n_agents", "representation", "hidden_sizes",
                              "normalize", "initialize", "activation", "device"],
     "Mixing_Q_network": ["action_space", "n_agents", "representation", "mixer", "hidden_sizes",
                          "normalize", "initialize", "activation", "device"],
     "Weighted_Mixing_Q_network": ["action_space", "n_agents", "representation", "mixer", "ff_mixer", "hidden_sizes",
                                   "normalize", "initialize", "activation", "device"],
```

### Comparing `xuance-1.1.0/xuance/torch/policies/categorical.py` & `xuance-1.1.1/xuance/torch/policies/categorical.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import torch.distributions
+import torch
+
 from xuance.torch.policies import *
 from xuance.torch.utils import *
 import numpy as np
 
 
 def _init_layer(layer, gain=np.sqrt(2), bias=0.0):
     nn.init.orthogonal_(layer.weight, gain=gain)
@@ -26,15 +27,15 @@
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
         layers.extend(mlp_block(input_shape[0], action_dim, None, None, initialize, device)[0])
         self.model = nn.Sequential(*layers)
         self.dist = CategoricalDistribution(action_dim)
 
     def forward(self, x: torch.Tensor):
-        self.dist.set_param(self.model(x))
+        self.dist.set_param(logits=self.model(x))
         return self.dist
 
 
 class CriticNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  hidden_sizes: Sequence[int],
@@ -134,61 +135,50 @@
         aux_critic_outputs = self.aux_critic_representation(observation)
         a = self.actor(policy_outputs['state'])
         v = self.critic(critic_outputs['state'])
         aux_v = self.aux_critic(aux_critic_outputs['state'])
         return policy_outputs, a, v, aux_v
 
 
-class CriticNet_SACDIS(nn.Module):
+class Actor_SAC(ActorNet):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
+                 normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
-        super(CriticNet_SACDIS, self).__init__()
-        layers = []
-        input_shape = (state_dim,)
-        for h in hidden_sizes:
-            mlp, input_shape = mlp_block(input_shape[0], h, None, activation, initialize, device)
-            layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, None, initialize, device)[0])
-        self.model = nn.Sequential(*layers)
+        super(Actor_SAC, self).__init__(state_dim, action_dim, hidden_sizes, normalize, initialize, activation, device)
+        self.output = nn.Softmax(dim=-1)
 
-    def forward(self, x: torch.tensor):
-        return self.model(x)
+    def forward(self, x: torch.Tensor):
+        self.dist.set_param(probs=self.output(self.model(x)))
+        return self.dist
 
 
-class ActorNet_SACDIS(nn.Module):
+class Critic_SAC(CriticNet, nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
-                 normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
-        super(ActorNet_SACDIS, self).__init__()
+        nn.Module.__init__(self)
         layers = []
         input_shape = (state_dim,)
         for h in hidden_sizes:
-            mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
+            mlp, input_shape = mlp_block(input_shape[0], h, None, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, None, None, device)[0])
-        self.output = nn.Sequential(*layers)
-        self.model = nn.Softmax(dim=-1)
+        layers.extend(mlp_block(input_shape[0], action_dim, None, None, initialize, device)[0])
+        self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor):
-        action_prob = self.model(self.output(x))
-        dist = torch.distributions.Categorical(probs=action_prob)
-        # action_logits = self.output(x)
-        # dist = torch.distributions.Categorical(logits=action_logits)
-        # action_prob = dist.probs
-        return action_prob, dist
+        return self.model(x)
 
 
 class SACDISPolicy(nn.Module):
     def __init__(self,
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
@@ -198,53 +188,83 @@
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(SACDISPolicy, self).__init__()
         self.action_dim = action_space.n
         self.representation_info_shape = representation.output_shapes
 
         self.actor_representation = representation
-        self.critic_representation = copy.deepcopy(representation)
-        self.target_critic_representation = copy.deepcopy(representation)
+        self.actor = Actor_SAC(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
+                               normalize, initialize, activation, device)
 
-        self.actor = ActorNet_SACDIS(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                                     normalize, initialize, activation, device)
-        self.critic = CriticNet_SACDIS(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
-                                       initialize, activation, device)
-        self.target_critic = copy.deepcopy(self.critic)
+        self.critic_1_representation = copy.deepcopy(representation)
+        self.critic_1 = Critic_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                   initialize, activation, device)
+        self.critic_2_representation = copy.deepcopy(representation)
+        self.critic_2 = Critic_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                   initialize, activation, device)
+        self.target_critic_1_representation = copy.deepcopy(self.critic_1_representation)
+        self.target_critic_1 = copy.deepcopy(self.critic_1)
+        self.target_critic_2_representation = copy.deepcopy(self.critic_2_representation)
+        self.target_critic_2 = copy.deepcopy(self.critic_2)
 
         self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
-        self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
+        self.critic_parameters = list(self.critic_1_representation.parameters()) + list(
+            self.critic_1.parameters()) + list(self.critic_2_representation.parameters()) + list(
+            self.critic_2.parameters())
 
     def forward(self, observation: Union[np.ndarray, dict]):
         outputs = self.actor_representation(observation)
-        act_prob, act_distribution = self.actor(outputs['state'])
-        return outputs, act_prob, act_distribution
+        act_dist = self.actor(outputs['state'])
+        act_samples = act_dist.stochastic_sample()
+        return outputs, act_samples
 
-    def Qtarget(self, observation: Union[np.ndarray, dict]):
+    def Qpolicy(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
-        outputs_critic = self.target_critic_representation(observation)
-        act_prob, act_distribution = self.actor(outputs_actor['state'])
-        # z = act_prob == 0.0
-        # z = z.float() * 1e-8
-        log_action_prob = torch.log(act_prob + 1e-5)
-        return act_prob, log_action_prob, self.target_critic(outputs_critic['state'])
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
 
-    def Qaction(self, observation: Union[np.ndarray, dict]):
-        outputs_critic = self.critic_representation(observation)
-        return outputs_critic, self.critic(outputs_critic['state'])
+        act_dist = self.actor(outputs_actor['state'])
+        act_prob = act_dist.probs
+        z = act_prob == 0.0
+        z = z.float() * 1e-8
+        log_action_prob = torch.log(act_prob + z)
+
+        q_1 = self.critic_1(outputs_critic_1['state'])
+        q_2 = self.critic_2(outputs_critic_2['state'])
+        return act_prob, log_action_prob, q_1, q_2
 
-    def Qpolicy(self, observation: Union[np.ndarray, dict]):
+    def Qtarget(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
-        outputs_critic = self.critic_representation(observation)
-        act_prob, act_distribution = self.actor(outputs_actor['state'])
-        # z = act_prob == 0.0
-        # z = z.float() * 1e-8
-        log_action_prob = torch.log(act_prob + 1e-5)
-        return act_prob, log_action_prob, self.critic(outputs_critic['state'])
+        outputs_critic_1 = self.target_critic_1_representation(observation)
+        outputs_critic_2 = self.target_critic_2_representation(observation)
+
+        new_act_dist = self.actor(outputs_actor['state'])
+        new_act_prob = new_act_dist.probs
+        z = new_act_prob == 0.0
+        z = z.float() * 1e-8  # avoid log(0)
+        log_action_prob = torch.log(new_act_prob + z)
+
+        target_q_1 = self.target_critic_1(outputs_critic_1['state'])
+        target_q_2 = self.target_critic_2(outputs_critic_2['state'])
+        target_q = torch.min(target_q_1, target_q_2)
+        return new_act_prob, log_action_prob, target_q
+
+    def Qaction(self, observation: Union[np.ndarray, dict]):
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+        q_1 = self.critic_1(outputs_critic_1['state'])
+        q_2 = self.critic_2(outputs_critic_2['state'])
+        return q_1, q_2
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
+        for ep, tp in zip(self.critic_1_representation.parameters(), self.target_critic_1_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_2_representation.parameters(), self.target_critic_2_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_1.parameters(), self.target_critic_1.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
+        for ep, tp in zip(self.critic_2.parameters(), self.target_critic_2.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
```

### Comparing `xuance-1.1.0/xuance/torch/policies/categorical_marl.py` & `xuance-1.1.1/xuance/torch/policies/categorical_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,40 +180,37 @@
         self.mixer = mixer
         self.pi_dist = CategoricalDistribution(self.action_dim)
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
                 *rnn_hidden: torch.Tensor, avail_actions=None, state=None):
         batch_size = len(observation)
         if self.use_rnn:
-            sequence_length = observation.shape[1]
             outputs = self.representation(observation, *rnn_hidden)
             rnn_hidden = (outputs['rnn_hidden'], outputs['rnn_cell'])
-            representated_state = outputs['state'].view(batch_size, self.n_agents, sequence_length, -1)
-            actor_critic_input = torch.concat([representated_state, agent_ids], dim=-1)
         else:
             outputs = self.representation(observation)
             rnn_hidden = None
-            actor_critic_input = torch.concat([outputs['state'], agent_ids], dim=-1)
+        actor_critic_input = torch.concat([outputs['state'], agent_ids], dim=-1)
         act_logits = self.actor(actor_critic_input)
         if avail_actions is not None:
             avail_actions = torch.Tensor(avail_actions)
             act_logits[avail_actions == 0] = -1e10
             self.pi_dist.set_param(logits=act_logits)
         else:
             self.pi_dist.set_param(logits=act_logits)
 
         values_independent = self.critic(actor_critic_input)
         if self.use_rnn:
             if self.mixer is None:
                 values_tot = values_independent
             else:
                 sequence_length = observation.shape[1]
-                values_independent = values_independent.transpose(1, 2).reshape(batch_size*sequence_length, self.n_agents)
+                values_independent = values_independent.transpose(1, 2).reshape(-1, self.n_agents)
                 values_tot = self.value_tot(values_independent, global_state=state)
-                values_tot = values_tot.reshape([batch_size, sequence_length, 1])
+                values_tot = values_tot.reshape([-1, sequence_length, 1])
                 values_tot = values_tot.unsqueeze(1).expand(-1, self.n_agents, -1, -1)
         else:
             values_tot = values_independent if self.mixer is None else self.value_tot(values_independent, global_state=state)
             values_tot = values_tot.unsqueeze(1).expand(-1, self.n_agents, -1)
 
         return rnn_hidden, self.pi_dist, values_tot
```

### Comparing `xuance-1.1.0/xuance/torch/policies/coordination_graph.py` & `xuance-1.1.1/xuance/torch/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/policies/deterministic.py` & `xuance-1.1.1/xuance/torch/policies/deterministic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import torch
+
 from xuance.torch.policies import *
 from xuance.torch.utils import *
 import numpy as np
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
@@ -43,15 +45,16 @@
                                    kwargs["recurrent_layer_N"],
                                    kwargs["dropout"],
                                    kwargs["initialize"],
                                    kwargs["device"])
         else:
             raise "Unknown recurrent module!"
         self.rnn_layer = output
-        fc_layer = mlp_block(kwargs["recurrent_hidden_size"], kwargs["action_dim"], None, None, None, kwargs["device"])[0]
+        fc_layer = mlp_block(kwargs["recurrent_hidden_size"], kwargs["action_dim"], None, None, None, kwargs["device"])[
+            0]
         self.model = nn.Sequential(*fc_layer)
 
     def forward(self, x: torch.Tensor, h: torch.Tensor, c: torch.Tensor = None):
         self.rnn_layer.flatten_parameters()
         if self.lstm:
             output, (hn, cn) = self.rnn_layer(x, (h, c))
             return hn, cn, self.model(output)
@@ -397,15 +400,15 @@
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, None, activation, initialize, device)
             layers.extend(mlp)
         layers.extend(mlp_block(input_shape[0], 1, None, None, initialize, device)[0])
         self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor, a: torch.tensor):
-        return self.model(torch.concat((x, a), dim=-1))[:, 0]
+        return self.model(torch.concat((x, a), dim=-1))
 
 
 class DDPGPolicy(nn.Module):
     def __init__(self,
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
@@ -413,50 +416,52 @@
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(DDPGPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation_info_shape = representation.output_shapes
+        # create networks
         self.actor_representation = representation
+        self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
+                              initialize, activation, activation_action, device)
         self.critic_representation = copy.deepcopy(representation)
-        self.target_actor_representation = copy.deepcopy(representation)
-        self.target_critic_representation = copy.deepcopy(representation)
-        self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size, initialize,
-                              activation, activation_action, device)
         self.critic = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                 initialize, activation, device)
+        # create target networks
+        self.target_actor_representation = copy.deepcopy(self.actor_representation)
         self.target_actor = copy.deepcopy(self.actor)
+        self.target_critic_representation = copy.deepcopy(self.critic_representation)
         self.target_critic = copy.deepcopy(self.critic)
-        
+
         # parameters
         self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
         self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
 
     def forward(self, observation: Union[np.ndarray, dict]):
         outputs = self.actor_representation(observation)
         act = self.actor(outputs['state'])
         return outputs, act
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.target_actor_representation(observation)
-        outputs_critic = self.target_critic_representation(observation) 
+        outputs_critic = self.target_critic_representation(observation)
         act = self.target_actor(outputs_actor['state'])
-        # noise = torch.randn_like(act).clamp(-1, 1) * 0.1
-        # act = (act + noise).clamp(-1, 1)
         return self.target_critic(outputs_critic['state'], act)
 
     def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
         outputs = self.critic_representation(observation)
         return self.critic(outputs['state'], action)
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
+        act = self.actor(outputs_actor['state'])
         outputs_critic = self.critic_representation(observation)
-        return self.critic(outputs_critic['state'], self.actor(outputs_actor['state']))
+        q_eval = self.critic(outputs_critic['state'], act)
+        return q_eval
 
     def soft_update(self, tau=0.005):
         for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
             tp.data.mul_(1 - tau)
@@ -481,86 +486,88 @@
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(TD3Policy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation_info_shape = representation.output_shapes
 
         self.actor_representation = representation
-        self.criticA_representation = copy.deepcopy(representation)
-        self.criticB_representation = copy.deepcopy(representation)
+        self.critic_A_representation = copy.deepcopy(representation)
+        self.critic_B_representation = copy.deepcopy(representation)
 
         self.target_actor_representation = copy.deepcopy(representation)
-        self.target_criticA_representation = copy.deepcopy(representation)
-        self.target_criticB_representation = copy.deepcopy(representation)
+        self.target_critic_A_representation = copy.deepcopy(representation)
+        self.target_critic_B_representation = copy.deepcopy(representation)
 
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
                               initialize, activation, activation_action, device)
-        self.criticA = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
-                                 initialize, activation, device)
-        self.criticB = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
-                                 initialize, activation, device)
+        self.critic_A = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                  initialize, activation, device)
+        self.critic_B = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                  initialize, activation, device)
         self.target_actor = copy.deepcopy(self.actor)
-        self.target_criticA = copy.deepcopy(self.criticA)
-        self.target_criticB = copy.deepcopy(self.criticB)
+        self.target_critic_A = copy.deepcopy(self.critic_A)
+        self.target_critic_B = copy.deepcopy(self.critic_B)
 
         # parameters
         self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
-        self.critic_parameters = list(self.criticA_representation.parameters()) + list(self.criticA.parameters()) + list(self.criticB_representation.parameters()) + list(self.criticB.parameters())
+        self.critic_parameters = list(self.critic_A_representation.parameters()) + list(
+            self.critic_A.parameters()) + list(self.critic_B_representation.parameters()) + list(
+            self.critic_B.parameters())
 
-    def action(self, observation: Union[np.ndarray, dict]):
+    def forward(self, observation: Union[np.ndarray, dict]):
         outputs = self.actor_representation(observation)
         act = self.actor(outputs['state'])
         return outputs, act
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.target_actor_representation(observation)
-        outputs_criticA = self.target_criticA_representation(observation)
-        outputs_criticB = self.target_criticB_representation(observation)
+        outputs_critic_A = self.target_critic_A_representation(observation)
+        outputs_critic_B = self.target_critic_B_representation(observation)
         act = self.target_actor(outputs_actor['state'])
-        noise = torch.randn_like(act).clamp(-0.1, 0.1) * 0.1
+        noise = (torch.randn_like(act) * 0.2).clamp(-0.5, 0.5)
         act = (act + noise).clamp(-1, 1)
 
-        qa = self.target_criticA(outputs_criticA['state'], act).unsqueeze(dim=1)
-        qb = self.target_criticB(outputs_criticB['state'], act).unsqueeze(dim=1)
-        mim_q = torch.minimum(qa, qb)
-        return outputs_actor, mim_q
+        qa = self.target_critic_A(outputs_critic_A['state'], act)
+        qb = self.target_critic_B(outputs_critic_B['state'], act)
+        min_q = torch.min(qa, qb)
+        return min_q
 
     def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
-        outputs_criticA = self.criticA_representation(observation)
-        outputs_criticB = self.criticB_representation(observation)
-        qa = self.criticA(outputs_criticA['state'], action).unsqueeze(dim=1)
-        qb = self.criticB(outputs_criticB['state'], action).unsqueeze(dim=1)
-        return outputs_criticA, torch.cat((qa, qb), axis=-1)
+        outputs_critic_A = self.critic_A_representation(observation)
+        outputs_critic_B = self.critic_B_representation(observation)
+        q_eval_a = self.critic_A(outputs_critic_A['state'], action)
+        q_eval_b = self.critic_B(outputs_critic_B['state'], action)
+        return q_eval_a, q_eval_b
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
-        outputs_criticA = self.criticA_representation(observation)
-        outputs_criticB = self.criticB_representation(observation)
+        outputs_critic_A = self.critic_A_representation(observation)
+        outputs_critic_B = self.critic_B_representation(observation)
         act = self.actor(outputs_actor['state'])
-        qa = self.criticA(outputs_criticA['state'], act).unsqueeze(dim=1)
-        qb = self.criticB(outputs_criticB['state'], act).unsqueeze(dim=1)
-        return outputs_actor, (qa + qb) / 2.0
+        q_eval_a = self.critic_A(outputs_critic_A['state'], act).unsqueeze(dim=1)
+        q_eval_b = self.critic_B(outputs_critic_B['state'], act).unsqueeze(dim=1)
+        return (q_eval_a + q_eval_b) / 2.0
 
     def soft_update(self, tau=0.005):
         for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.criticA_representation.parameters(), self.target_criticA_representation.parameters()):
+        for ep, tp in zip(self.critic_A_representation.parameters(), self.target_critic_A_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.criticA.parameters(), self.target_criticA.parameters()):
+        for ep, tp in zip(self.critic_A.parameters(), self.target_critic_A.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.criticB_representation.parameters(), self.target_criticB_representation.parameters()):
+        for ep, tp in zip(self.critic_B_representation.parameters(), self.target_critic_B_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.criticB.parameters(), self.target_criticB.parameters()):
+        for ep, tp in zip(self.critic_B.parameters(), self.target_critic_B.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
 class PDQNPolicy(nn.Module):
     def __init__(self,
                  observation_space,
```

### Comparing `xuance-1.1.0/xuance/torch/policies/deterministic_marl.py` & `xuance-1.1.1/xuance/torch/policies/deterministic_marl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import copy
+
 from xuance.torch.policies import *
 from xuance.torch.utils import *
 from torch.distributions import Categorical
-from gymnasium import spaces as spaces_pettingzoo
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
                  n_actions: int,
                  n_agents: int,
@@ -397,30 +398,25 @@
 
     def forward(self, x: torch.tensor):
         return self.model(x)
 
 
 class CriticNet(nn.Module):
     def __init__(self,
-                 independent: bool,
                  state_dim: int,
                  n_agents: int,
-                 action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         super(CriticNet, self).__init__()
         layers = []
-        if independent:
-            input_shape = (state_dim + action_dim + n_agents,)
-        else:
-            input_shape = (state_dim * n_agents + action_dim * n_agents + n_agents,)
+        input_shape = (state_dim + n_agents,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
         layers.extend(mlp_block(input_shape[0], 1, None, None, initialize, device)[0])
         self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor):
@@ -439,90 +435,119 @@
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  ):
         super(Basic_DDPG_policy, self).__init__()
         self.action_dim = action_space.shape[-1]
         self.n_agents = n_agents
-        self.representation = representation
-        self.representation_info_shape = self.representation.output_shapes
+        self.representation_info_shape = representation.output_shapes
+        dim_input_actor = representation.output_shapes['state'][0]
+        dim_input_critic = representation.output_shapes['state'][0] + self.action_dim
+
+        self.actor_representation = representation
+        self.actor = ActorNet(dim_input_actor, n_agents, self.action_dim, actor_hidden_size,
+                              normalize, initialize, activation, activation_action, device)
+        self.critic_representation = copy.deepcopy(representation)
+        self.critic = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                normalize, initialize, activation, device)
+
+        self.target_actor_representation = copy.deepcopy(self.actor_representation)
+        self.target_actor = copy.deepcopy(self.actor)
+        self.target_critic_representation = copy.deepcopy(self.critic_representation)
+        self.target_critic = copy.deepcopy(self.critic)
 
-        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
-        self.critic_net = CriticNet(True, representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                    critic_hidden_size, normalize, initialize, activation, device)
-        self.target_actor_net = copy.deepcopy(self.actor_net)
-        self.target_critic_net = copy.deepcopy(self.critic_net)
-        self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
-        self.parameters_critic = self.critic_net.parameters()
+        self.parameters_actor = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.parameters_critic = list(self.critic_representation.parameters()) + list(self.critic.parameters())
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
+        outputs = self.actor_representation(observation)
         actor_in = torch.concat([outputs['state'], agent_ids], dim=-1)
-        act = self.actor_net(actor_in)
+        act = self.actor(actor_in)
         return outputs, act
 
-    def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
+    def Qpolicy(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+        outputs = self.critic_representation(observation)
         critic_in = torch.concat([outputs['state'], actions, agent_ids], dim=-1)
-        return self.critic_net(critic_in)
+        return self.critic(critic_in)
 
-    def target_critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
+    def Qtarget(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+        outputs = self.target_critic_representation(observation)
         critic_in = torch.concat([outputs['state'], actions, agent_ids], dim=-1)
-        return self.target_critic_net(critic_in)
+        return self.target_critic(critic_in)
 
-    def target_actor(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
+    def Atarget(self, observation: torch.Tensor, agent_ids: torch.Tensor):
+        outputs = self.target_actor_representation(observation)
         actor_in = torch.concat([outputs['state'], agent_ids], dim=-1)
-        return self.target_actor_net(actor_in)
+        return self.target_actor(actor_in)
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.actor_net.parameters(), self.target_actor_net.parameters()):
+        for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic_net.parameters(), self.target_critic_net.parameters()):
+        for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
-class MADDPG_policy(Basic_DDPG_policy):
+class MADDPG_policy(Basic_DDPG_policy, nn.Module):
     def __init__(self,
                  action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
-        super(MADDPG_policy, self).__init__(action_space, n_agents, representation,
-                                            actor_hidden_size, critic_hidden_size,
-                                            normalize, initialize, activation, activation_action, device)
-        self.critic_net = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                    critic_hidden_size, normalize, initialize, activation, device)
-        self.target_critic_net = copy.deepcopy(self.critic_net)
-        self.parameters_critic = self.critic_net.parameters()
+        nn.Module.__init__(self)
+        self.action_dim = action_space.shape[-1]
+        self.n_agents = n_agents
+        self.representation_info_shape = representation.output_shapes
+        dim_input_actor = representation.output_shapes['state'][0]
+        dim_input_critic = (representation.output_shapes['state'][0] + self.action_dim) * self.n_agents
+
+        self.actor_representation = representation
+        self.actor = ActorNet(dim_input_actor, n_agents, self.action_dim, actor_hidden_size,
+                              normalize, initialize, activation, activation_action, device)
+        self.critic_representation = copy.deepcopy(representation)
+        self.critic = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                normalize, initialize, activation, device)
+
+        self.target_actor_representation = copy.deepcopy(self.actor_representation)
+        self.target_actor = copy.deepcopy(self.actor)
+        self.target_critic_representation = copy.deepcopy(self.critic_representation)
+        self.target_critic = copy.deepcopy(self.critic)
+
+        self.parameters_actor = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.parameters_critic = list(self.critic_representation.parameters()) + list(self.critic.parameters())
 
-    def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+    def Qpolicy(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        return self.critic_net(critic_in)
+        outputs = self.critic_representation(observation)
+        critic_in = torch.concat([outputs['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                  actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                  agent_ids], dim=-1)
+        return self.critic(critic_in)
 
-    def target_critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+    def Qtarget(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        return self.target_critic_net(critic_in)
+        outputs = self.target_critic_representation(observation)
+        critic_in = torch.concat([outputs['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                  actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                  agent_ids], dim=-1)
+        return self.target_critic(critic_in)
 
 
 class MATD3_policy(Basic_DDPG_policy, nn.Module):
     def __init__(self,
                  action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
@@ -533,65 +558,91 @@
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         nn.Module.__init__(self)
         self.action_dim = action_space.shape[-1]
         self.n_agents = n_agents
-        self.representation = representation
-        self.representation_info_shape = self.representation.output_shapes
-
-        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
-        self.target_actor_net = copy.deepcopy(self.actor_net)
-
-        self.critic_net_A = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                      critic_hidden_size, normalize, initialize, activation, device)
-        self.critic_net_B = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                      critic_hidden_size, normalize, initialize, activation, device)
-        self.target_critic_net_A = copy.deepcopy(self.critic_net_A)
-        self.target_critic_net_B = copy.deepcopy(self.critic_net_B)
-
-        self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
-        self.parameters_critic = list(self.critic_net_A.parameters()) + list(self.critic_net_B.parameters())
+        self.representation_info_shape = representation.output_shapes
+        dim_input_actor = representation.output_shapes['state'][0]
+        dim_input_critic = (representation.output_shapes['state'][0] + self.action_dim) * self.n_agents
+
+        self.actor_representation = representation
+        self.actor = ActorNet(dim_input_actor, n_agents, self.action_dim, actor_hidden_size,
+                              normalize, initialize, activation, activation_action, device)
+        self.critic_A_representation = copy.deepcopy(representation)
+        self.critic_A = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.critic_B_representation = copy.deepcopy(representation)
+        self.critic_B = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.target_actor_representation = copy.deepcopy(self.actor_representation)
+        self.target_actor = copy.deepcopy(self.actor)
+        self.target_critic_A_representation = copy.deepcopy(self.critic_A_representation)
+        self.target_critic_A = copy.deepcopy(self.critic_A)
+        self.target_critic_B_representation = copy.deepcopy(self.critic_B_representation)
+        self.target_critic_B = copy.deepcopy(self.critic_B)
+
+        self.parameters_actor = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.parameters_critic = list(self.critic_A_representation.parameters()) + list(
+            self.critic_A.parameters()) + list(self.critic_B_representation.parameters()) + list(
+            self.critic_B.parameters())
 
     def Qpolicy(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        qa = self.critic_net_A(critic_in)
-        qb = self.critic_net_B(critic_in)
-        return outputs_n, (qa + qb) / 2.0
+        outputs_critic_A = self.critic_A_representation(observation)
+        outputs_critic_B = self.critic_B_representation(observation)
+        critic_A_in = torch.concat([outputs_critic_A['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_B_in = torch.concat([outputs_critic_B['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        qa, qb = self.critic_A(critic_A_in), self.critic_B(critic_B_in)
+        return (qa + qb) / 2.0
 
     def Qtarget(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        # noise = torch.randn_like(actions).clamp(-1, 1) * 0.1
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        # noise = noise.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        # actions_n = (actions_n + noise).clamp(-1, 1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        qa = self.target_critic_net_A(critic_in)
-        qb = self.target_critic_net_B(critic_in)
+        outputs_critic_A = self.target_critic_A_representation(observation)
+        outputs_critic_B = self.target_critic_B_representation(observation)
+        critic_A_in = torch.concat([outputs_critic_A['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_B_in = torch.concat([outputs_critic_B['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        qa, qb = self.target_critic_A(critic_A_in), self.target_critic_B(critic_B_in)
         min_q = torch.minimum(qa, qb)
-        return outputs_n, min_q
+        return min_q
 
     def Qaction(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        qa = self.critic_net_A(critic_in)
-        qb = self.critic_net_B(critic_in)
-        return outputs_n, torch.cat((qa, qb), dim=-1)
+        outputs_critic_A = self.critic_A_representation(observation)
+        outputs_critic_B = self.critic_B_representation(observation)
+        critic_A_in = torch.concat([outputs_critic_A['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_B_in = torch.concat([outputs_critic_B['state'].reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.reshape(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        qa, qb = self.critic_A(critic_A_in), self.critic_B(critic_B_in)
+        return torch.cat((qa, qb), dim=-1)
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.actor_net.parameters(), self.target_actor_net.parameters()):
+        for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_A_representation.parameters(), self.target_critic_A_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_A.parameters(), self.target_critic_A.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic_net_A.parameters(), self.target_critic_net_A.parameters()):
+        for ep, tp in zip(self.critic_B_representation.parameters(), self.target_critic_B_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic_net_B.parameters(), self.target_critic_net_B.parameters()):
+        for ep, tp in zip(self.critic_B.parameters(), self.target_critic_B.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
```

### Comparing `xuance-1.1.0/xuance/torch/policies/gaussian.py` & `xuance-1.1.1/xuance/torch/policies/gaussian.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import torch.nn.functional
 from xuance.torch.policies import *
 from xuance.torch.utils import *
-from torch.distributions import Normal
 import numpy as np
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
@@ -148,24 +148,25 @@
         layers = []
         input_shape = (state_dim,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
         self.device = device
         self.output = nn.Sequential(*layers)
-        self.out_mu = nn.Sequential(*mlp_block(hidden_sizes[-1], action_dim, normalize, activation_action, initialize, device)[0])
-        self.out_std = nn.Linear(hidden_sizes[-1], action_dim, device=device)
+        self.out_mu = nn.Linear(hidden_sizes[-1], action_dim, device=device)
+        self.out_log_std = nn.Linear(hidden_sizes[-1], action_dim, device=device)
+        self.dist = ActivatedDiagGaussianDistribution(action_dim, activation_action, device)
 
     def forward(self, x: torch.tensor):
         output = self.output(x)
         mu = self.out_mu(output)
-        std = torch.clamp(self.out_std(output), -20, 2)
-        std = std.exp()
-        dist = Normal(mu, std)
-        return dist
+        log_std = torch.clamp(self.out_log_std(output), -20, 2)
+        std = log_std.exp()
+        self.dist.set_param(mu, std)
+        return self.dist
 
 
 class CriticNet_SAC(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
@@ -195,55 +196,81 @@
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(SACPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
+        self.activation_action = activation_action()
         self.representation_info_shape = representation.output_shapes
-        
-        # representations
-        self.actor_representation = representation
-        self.critic_representation = copy.deepcopy(representation)
-        self.target_critic_representation = copy.deepcopy(representation)
 
+        self.actor_representation = representation
         self.actor = ActorNet_SAC(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
                                   normalize, initialize, activation, activation_action, device)
-        self.critic = CriticNet_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
-                                    normalize, initialize, activation, device)
-        self.target_critic = copy.deepcopy(self.critic)
+
+        self.critic_1_representation = copy.deepcopy(representation)
+        self.critic_1 = CriticNet_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                      normalize, initialize, activation, device)
+        self.critic_2_representation = copy.deepcopy(representation)
+        self.critic_2 = CriticNet_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
+                                      normalize, initialize, activation, device)
+        self.target_critic_1_representation = copy.deepcopy(self.critic_1_representation)
+        self.target_critic_1 = copy.deepcopy(self.critic_1)
+        self.target_critic_2_representation = copy.deepcopy(self.critic_2_representation)
+        self.target_critic_2 = copy.deepcopy(self.critic_2)
 
         self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
-        self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
+        self.critic_parameters = list(self.critic_1_representation.parameters()) + list(
+            self.critic_1.parameters()) + list(self.critic_2_representation.parameters()) + list(
+            self.critic_2.parameters())
 
     def forward(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
         act_dist = self.actor(outputs_actor['state'])
-        return outputs_actor, act_dist
+        act_sample = act_dist.activated_rsample()
+        return outputs_actor, act_sample
 
-    def Qtarget(self, observation: Union[np.ndarray, dict]):
+    def Qpolicy(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
-        outputs_critic = self.target_critic_representation(observation)
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+
         act_dist = self.actor(outputs_actor['state'])
-        act = act_dist.rsample()
-        act_log = act_dist.log_prob(act).sum(-1)
-        return act_log, self.target_critic(outputs_critic['state'], act)
+        act_sample, act_log = act_dist.activated_rsample_and_logprob()
 
-    def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
-        outputs_critic = self.critic_representation(observation)
-        return self.critic(outputs_critic['state'], action)
+        q_1 = self.critic_1(outputs_critic_1['state'], act_sample)
+        q_2 = self.critic_2(outputs_critic_2['state'], act_sample)
+        return act_log, q_1, q_2
 
-    def Qpolicy(self, observation: Union[np.ndarray, dict]):
+    def Qtarget(self, observation: Union[np.ndarray, dict]):
         outputs_actor = self.actor_representation(observation)
-        outputs_critic = self.critic_representation(observation)
-        act_dist = self.actor(outputs_actor['state'])
-        act = act_dist.rsample()
-        act_log = act_dist.log_prob(act).sum(-1)
-        return act_log, self.critic(outputs_critic['state'], act)
+        outputs_critic_1 = self.target_critic_1_representation(observation)
+        outputs_critic_2 = self.target_critic_2_representation(observation)
+
+        new_act_dist = self.actor(outputs_actor['state'])
+        new_act_sample, new_act_log = new_act_dist.activated_rsample_and_logprob()
+
+        target_q_1 = self.target_critic_1(outputs_critic_1['state'], new_act_sample)
+        target_q_2 = self.target_critic_2(outputs_critic_2['state'], new_act_sample)
+        target_q = torch.min(target_q_1, target_q_2)
+        return new_act_log, target_q
+
+    def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+        q_1 = self.critic_1(outputs_critic_1['state'], action)
+        q_2 = self.critic_2(outputs_critic_2['state'], action)
+        return q_1, q_2
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
+        for ep, tp in zip(self.critic_1_representation.parameters(), self.target_critic_1_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_2_representation.parameters(), self.target_critic_2_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_1.parameters(), self.target_critic_1.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
+        for ep, tp in zip(self.critic_2.parameters(), self.target_critic_2.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
```

### Comparing `xuance-1.1.0/xuance/torch/policies/gaussian_marl.py` & `xuance-1.1.1/xuance/torch/policies/gaussian_marl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,70 @@
-import torch.distributions
+import copy
 
 from xuance.torch.policies import *
 from xuance.torch.utils import *
 
 
-class BasicQhead(nn.Module):
+class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
-                 action_dim: int,
                  n_agents: int,
+                 action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
-        super(BasicQhead, self).__init__()
-        layers_ = []
+        super(ActorNet, self).__init__()
+        self.device = device
+        layers = []
         input_shape = (state_dim + n_agents,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
-            layers_.extend(mlp)
-        layers_.extend(mlp_block(input_shape[0], action_dim, None, None, None, device)[0])
-        self.model = nn.Sequential(*layers_)
+            layers.extend(mlp)
+        layers.extend(mlp_block(input_shape[0], action_dim, activation=activation_action, device=device)[0])
+        self.mu = nn.Sequential(*layers)
+        self.log_std = nn.Parameter(-torch.ones((action_dim,), device=device))
+        self.dist = DiagGaussianDistribution(action_dim)
 
     def forward(self, x: torch.Tensor):
-        return self.model(x)
-
-
-class BasicQnetwork(nn.Module):
-    def __init__(self,
-                 action_space: Discrete,
-                 n_agents: int,
-                 representation: nn.Module,
-                 hidden_size: Sequence[int] = None,
-                 normalize: Optional[ModuleType] = None,
-                 initialize: Optional[Callable[..., torch.Tensor]] = None,
-                 activation: Optional[ModuleType] = None,
-                 device: Optional[Union[str, int, torch.device]] = None):
-        super(BasicQnetwork, self).__init__()
-        self.action_dim = action_space.n
-        self.representation = representation
-        self.representation_info_shape = self.representation.output_shapes
-
-        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.action_dim, n_agents,
-                                     hidden_size, normalize, initialize, activation, device)
-        self.target_Qhead = copy.deepcopy(self.eval_Qhead)
-
-    def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        q_inputs = torch.concat([outputs['state'], agent_ids], dim=-1)
-        evalQ = self.eval_Qhead(q_inputs)
-        argmax_action = evalQ.argmax(dim=-1, keepdim=False)
-        return outputs, argmax_action, evalQ
-
-    def target_Q(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        q_inputs = torch.concat([outputs['state'], agent_ids], dim=-1)
-        return self.target_Qhead(q_inputs)
-
-    def copy_target(self):
-        for ep, tp in zip(self.eval_Qhead.parameters(), self.target_Qhead.parameters()):
-            tp.data.copy_(ep)
+        self.dist.set_param(self.mu(x), self.log_std.exp())
+        return self.dist
 
 
-class ActorNet(nn.Module):
+class ActorNet_SAC(nn.Module):
     def __init__(self,
                  state_dim: int,
                  n_agents: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
-        super(ActorNet, self).__init__()
+        super(ActorNet_SAC, self).__init__()
         self.device = device
         layers = []
         input_shape = (state_dim + n_agents,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, activation=activation_action, device=device)[0])
-        self.mu = nn.Sequential(*layers)
-        self.log_std = nn.Parameter(-torch.ones((action_dim,), device=device))
-        self.dist = DiagGaussianDistribution(action_dim)
+        self.output = nn.Sequential(*layers)
+        self.mu = nn.Linear(input_shape[0], action_dim, device=device)
+        self.log_std = nn.Linear(input_shape[0], action_dim, device=device)
+        self.dist = ActivatedDiagGaussianDistribution(action_dim, activation_action, device)
 
     def forward(self, x: torch.Tensor):
-        self.dist.set_param(self.mu(x), self.log_std.exp())
+        output = self.output(x)
+        mu = self.mu(output)
+        log_std = torch.clamp(self.log_std(output), -20, 2)
+        std = log_std.exp()
+        self.dist.set_param(mu, std)
         return self.dist
 
 
 class CriticNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  n_agents: int,
@@ -159,25 +132,25 @@
             rnn_hidden = None
         actor_input = torch.concat([outputs['state'], agent_ids], dim=-1)
         self.pi_dist = self.actor(actor_input)
         return rnn_hidden, self.pi_dist
 
     def get_values(self, critic_in: torch.Tensor, agent_ids: torch.Tensor,
                    *rnn_hidden: torch.Tensor, **kwargs):
-        shape_obs = critic_in.shape
+        shape_input = critic_in.shape
         # get representation features
         if self.use_rnn:
-            batch_size, n_agent, episode_length, dim_obs = tuple(shape_obs)
-            outputs = self.representation_critic(critic_in.reshape(-1, episode_length, dim_obs), *rnn_hidden)
-            outputs['state'] = outputs['state'].view(batch_size, n_agent, episode_length, -1)
+            batch_size, n_agent, episode_length, dim_input = tuple(shape_input)
+            outputs = self.representation_critic(critic_in.reshape(-1, episode_length, dim_input), *rnn_hidden)
+            outputs['state'] = outputs['state'].reshape(batch_size, n_agent, episode_length, -1)
             rnn_hidden = (outputs['rnn_hidden'], outputs['rnn_cell'])
         else:
-            batch_size, n_agent, dim_obs = tuple(shape_obs)
-            outputs = self.representation_critic(critic_in.reshape(-1, dim_obs))
-            outputs['state'] = outputs['state'].view(batch_size, n_agent, -1)
+            batch_size, n_agent, dim_input = tuple(shape_input)
+            outputs = self.representation_critic(critic_in.reshape(-1, dim_input))
+            outputs['state'] = outputs['state'].reshape(batch_size, n_agent, -1)
             rnn_hidden = None
         # get critic values
         critic_in = torch.concat([outputs['state'], agent_ids], dim=-1)
         v = self.critic(critic_in)
         return rnn_hidden, v
 
     def value_tot(self, values_n: torch.Tensor, global_state=None):
@@ -197,86 +170,185 @@
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         super(Basic_ISAC_policy, self).__init__()
         self.action_dim = action_space.shape[0]
+        self.activation_action = activation_action
         self.n_agents = n_agents
-        self.representation = representation
-        self.representation_info_shape = self.representation.output_shapes
-
-        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
+        self.representation_info_shape = representation.output_shapes
+        dim_input_actor = representation.output_shapes['state'][0]
         dim_input_critic = representation.output_shapes['state'][0] + self.action_dim
-        self.critic_net = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
-                                    normalize, initialize, activation, device)
-        self.target_actor_net = copy.deepcopy(self.actor_net)
-        self.target_critic_net = copy.deepcopy(self.critic_net)
-        self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
-        self.parameters_critic = self.critic_net.parameters()
+
+        self.actor_representation = representation
+        self.actor = ActorNet_SAC(dim_input_actor, n_agents, self.action_dim, actor_hidden_size,
+                                  normalize, initialize, activation, activation_action, device)
+
+        self.critic_1_representation = copy.deepcopy(representation)
+        self.critic_1 = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.critic_2_representation = copy.deepcopy(representation)
+        self.critic_2 = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.target_critic_1_representation = copy.deepcopy(self.critic_1_representation)
+        self.target_critic_1 = copy.deepcopy(self.critic_1)
+        self.target_critic_2_representation = copy.deepcopy(self.critic_2_representation)
+        self.target_critic_2 = copy.deepcopy(self.critic_2)
+
+        self.parameters_actor = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.parameters_critic = list(self.critic_1_representation.parameters()) + list(
+            self.critic_1.parameters()) + list(self.critic_2_representation.parameters()) + list(
+            self.critic_2.parameters())
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        actor_in = torch.concat([outputs['state'], agent_ids], dim=-1)
-        act = self.actor_net(actor_in)
-        return outputs, act
-
-    def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        critic_in = torch.concat([outputs['state'], actions, agent_ids], dim=-1)
-        return self.critic_net(critic_in)
-
-    def target_critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        critic_in = torch.concat([outputs['state'], actions, agent_ids], dim=-1)
-        return self.target_critic_net(critic_in)
-
-    def target_actor(self, observation: torch.Tensor, agent_ids: torch.Tensor):
-        outputs = self.representation(observation)
-        actor_in = torch.concat([outputs['state'], agent_ids], dim=-1)
-        return self.target_actor_net(actor_in)
+        outputs_actor = self.actor_representation(observation)
+        actor_in = torch.concat([outputs_actor['state'], agent_ids], dim=-1)
+        act_dist = self.actor(actor_in)
+        act_sample = act_dist.activated_rsample()
+        return outputs_actor, act_sample
+
+    def Qpolicy(self, observation: torch.Tensor, agent_ids: torch.Tensor):
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+
+        actor_in = torch.concat([outputs_actor['state'], agent_ids], dim=-1)
+        act_dist = self.actor(actor_in)
+        act_sample, act_log = act_dist.activated_rsample_and_logprob()
+
+        critic_1_in = torch.concat([outputs_critic_1['state'], act_sample, agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'], act_sample, agent_ids], dim=-1)
+        q_1, q_2 = self.critic_1(critic_1_in), self.critic_2(critic_2_in)
+        return act_log, q_1, q_2
+
+    def Qtarget(self, observation: torch.Tensor, agent_ids: torch.Tensor):
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic_1 = self.target_critic_1_representation(observation)
+        outputs_critic_2 = self.target_critic_2_representation(observation)
+
+        actor_in = torch.concat([outputs_actor['state'], agent_ids], dim=-1)
+        new_act_dist = self.actor(actor_in)
+        new_act_sample, new_act_log = new_act_dist.activated_rsample_and_logprob()
+
+        critic_1_in = torch.concat([outputs_critic_1['state'], new_act_sample, agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'], new_act_sample, agent_ids], dim=-1)
+        target_q_1, target_q_2 = self.target_critic_1(critic_1_in), self.target_critic_2(critic_2_in)
+        target_q = torch.min(target_q_1, target_q_2)
+        return new_act_log, target_q
+
+    def Qaction(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+        critic_1_in = torch.concat([outputs_critic_1['state'], actions, agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'], actions, agent_ids], dim=-1)
+        q_1, q_2 = self.critic_1(critic_1_in), self.critic_2(critic_2_in)
+        return q_1, q_2
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.actor_net.parameters(), self.target_actor_net.parameters()):
+        for ep, tp in zip(self.critic_1_representation.parameters(), self.target_critic_1_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_1.parameters(), self.target_critic_1.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_2_representation.parameters(), self.target_critic_2_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.critic_net.parameters(), self.target_critic_net.parameters()):
+        for ep, tp in zip(self.critic_2.parameters(), self.target_critic_2.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
-class MASAC_policy(Basic_ISAC_policy):
+class MASAC_policy(Basic_ISAC_policy, nn.Module):
     def __init__(self,
                  action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
-        super(MASAC_policy, self).__init__(action_space, n_agents, representation,
-                                           actor_hidden_size, critic_hidden_size,
-                                           normalize, initialize, activation, activation_action, device)
+        nn.Module.__init__(self)
+        self.action_dim = action_space.shape[0]
+        self.activation_action = activation_action
+        self.n_agents = n_agents
+        self.representation_info_shape = representation.output_shapes
+        dim_input_actor = representation.output_shapes['state'][0]
         dim_input_critic = (representation.output_shapes['state'][0] + self.action_dim) * self.n_agents
-        self.critic_net = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
-                                    normalize, initialize, activation, device)
-        self.target_critic_net = copy.deepcopy(self.critic_net)
-        self.parameters_critic = self.critic_net.parameters()
 
-    def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+        self.actor_representation = representation
+        self.actor = ActorNet_SAC(dim_input_actor, n_agents, self.action_dim, actor_hidden_size,
+                                  normalize, initialize, activation, activation_action, device)
+
+        self.critic_1_representation = copy.deepcopy(representation)
+        self.critic_1 = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.critic_2_representation = copy.deepcopy(representation)
+        self.critic_2 = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
+                                  normalize, initialize, activation, device)
+        self.target_critic_1_representation = copy.deepcopy(self.critic_1_representation)
+        self.target_critic_1 = copy.deepcopy(self.critic_1)
+        self.target_critic_2_representation = copy.deepcopy(self.critic_2_representation)
+        self.target_critic_2 = copy.deepcopy(self.critic_2)
+
+        self.parameters_actor = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.parameters_critic = list(self.critic_1_representation.parameters()) + list(
+            self.critic_1.parameters()) + list(self.critic_2_representation.parameters()) + list(
+            self.critic_2.parameters())
+
+    def Qpolicy(self, observation: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        return self.critic_net(critic_in)
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+
+        actor_in = torch.concat([outputs_actor['state'], agent_ids], dim=-1)
+        act_dist = self.actor(actor_in)
+        act_sample, act_log = act_dist.activated_rsample_and_logprob()
+
+        critic_1_in = torch.concat([outputs_critic_1['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    act_sample.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    act_sample.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        q_1, q_2 = self.critic_1(critic_1_in), self.critic_2(critic_2_in)
+        return act_log, q_1, q_2
 
-    def target_critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+    def Qtarget(self, observation: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
-        outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
-        critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
-        return self.target_critic_net(critic_in)
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic_1 = self.target_critic_1_representation(observation)
+        outputs_critic_2 = self.target_critic_2_representation(observation)
+
+        actor_in = torch.concat([outputs_actor['state'], agent_ids], dim=-1)
+        new_act_dist = self.actor(actor_in)
+        new_act_sample, new_act_log = new_act_dist.activated_rsample_and_logprob()
+
+        critic_1_in = torch.concat([outputs_critic_1['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    new_act_sample.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    new_act_sample.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        target_q_1, target_q_2 = self.target_critic_1(critic_1_in), self.target_critic_2(critic_2_in)
+        target_q = torch.min(target_q_1, target_q_2)
+        return new_act_log, target_q
+
+    def Qaction(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
+        bs = observation.shape[0]
+        outputs_critic_1 = self.critic_1_representation(observation)
+        outputs_critic_2 = self.critic_2_representation(observation)
+
+        critic_1_in = torch.concat([outputs_critic_1['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        critic_2_in = torch.concat([outputs_critic_2['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    actions.view(bs, 1, -1).expand(-1, self.n_agents, -1),
+                                    agent_ids], dim=-1)
+        q_1, q_2 = self.critic_1(critic_1_in), self.critic_2(critic_2_in)
+        return q_1, q_2
```

### Comparing `xuance-1.1.0/xuance/torch/policies/mixers.py` & `xuance-1.1.1/xuance/torch/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/representations/__init__.py` & `xuance-1.1.1/xuance/torch/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/representations/cnn.py` & `xuance-1.1.1/xuance/torch/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/representations/mlp.py` & `xuance-1.1.1/xuance/torch/representations/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     def __init__(self,
                  input_shape: Sequence[int],
                  device: Optional[Union[str, int, torch.device]] = None):
         super(Basic_Identical, self).__init__()
         assert len(input_shape) == 1
         self.output_shapes = {'state': (input_shape[0],)}
         self.device = device
-        self.model = nn.Sequential()
 
     def forward(self, observations: np.ndarray):
         state = torch.as_tensor(observations, dtype=torch.float32, device=self.device)
         return {'state': state}
 
 
 # process the input observations with stacks of MLP layers
```

### Comparing `xuance-1.1.0/xuance/torch/representations/rnn.py` & `xuance-1.1.1/xuance/torch/representations/rnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/runners/runner_drl.py` & `xuance-1.1.1/xuance/torch/runners/runner_drl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/runners/runner_football.py` & `xuance-1.1.1/xuance/torch/runners/runner_football.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/runners/runner_marl.py` & `xuance-1.1.1/xuance/torch/runners/runner_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class Runner_MARL(Runner_Base):
     def __init__(self, args):
         super(Runner_MARL, self).__init__(args)
         self.args = args
         self.render = args.render
-        self.fps = args[0].fps if type(args) == list else args.fps
+        self.fps = args.fps
 
         time_string = get_time_string()
         seed = f"seed_{self.args.seed}_"
         self.args.model_dir_load = args.model_dir
         self.args.model_dir_save = os.path.join(os.getcwd(), args.model_dir, seed + time_string)
 
         if args.logger == "tensorboard":
```

### Comparing `xuance-1.1.0/xuance/torch/runners/runner_pettingzoo.py` & `xuance-1.1.1/xuance/torch/runners/runner_pettingzoo.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/runners/runner_sc2.py` & `xuance-1.1.1/xuance/torch/runners/runner_sc2.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/utils/__init__.py` & `xuance-1.1.1/xuance/torch/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,16 @@
     torch, nn,
     ModuleType,
     mlp_block, cnn_block, pooling_block, gru_block, lstm_block
 )
 from .distributions import (
     Distribution,
     CategoricalDistribution,
-    DiagGaussianDistribution
+    DiagGaussianDistribution,
+    ActivatedDiagGaussianDistribution
 )
 from .operations import (update_linear_decay, set_seed, get_flat_grad, get_flat_params, assign_from_flat_grads,
                          assign_from_flat_params, split_distributions, merge_distributions)
 from .value_norm import ValueNorm
 
 ActivationFunctions = {
     "relu": nn.ReLU,
```

### Comparing `xuance-1.1.0/xuance/torch/utils/input_reformat.py` & `xuance-1.1.1/xuance/torch/utils/input_reformat.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/utils/layers.py` & `xuance-1.1.1/xuance/torch/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance/torch/utils/operations.py` & `xuance-1.1.1/xuance/torch/utils/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def split_distributions(distribution):
     return_list = []
     if isinstance(distribution, CategoricalDistribution):
         shape = distribution.logits.shape
         logits = distribution.logits.view(-1, shape[-1])
         for logit in logits:
             dist = CategoricalDistribution(logits.shape[-1])
-            dist.set_param(logit.unsqueeze(0).detach())
+            dist.set_param(logits=logit.unsqueeze(0).detach())
             return_list.append(dist)
     elif isinstance(distribution, DiagGaussianDistribution):
         shape = distribution.mu.shape
         means = distribution.mu.view(-1, shape[-1])
         std = distribution.std
         for mu in means:
             dist = DiagGaussianDistribution(shape[-1])
@@ -73,15 +73,15 @@
 
 
 def merge_distributions(distribution_list):
     if isinstance(distribution_list[0], CategoricalDistribution):
         logits = torch.cat([dist.logits for dist in distribution_list], dim=0)
         action_dim = logits.shape[-1]
         dist = CategoricalDistribution(action_dim)
-        dist.set_param(logits.detach())
+        dist.set_param(logits=logits.detach())
         return dist
     elif isinstance(distribution_list[0], DiagGaussianDistribution):
         shape = distribution_list.shape
         distribution_list = distribution_list.reshape([-1])
         mu = torch.cat([dist.mu for dist in distribution_list], dim=0)
         std = torch.cat([dist.std for dist in distribution_list], dim=0)
         action_dim = distribution_list[0].mu.shape[-1]
@@ -93,11 +93,11 @@
     elif isinstance(distribution_list[0, 0], CategoricalDistribution):
         shape = distribution_list.shape
         distribution_list = distribution_list.reshape([-1])
         logits = torch.cat([dist.logits for dist in distribution_list], dim=0)
         action_dim = logits.shape[-1]
         dist = CategoricalDistribution(action_dim)
         logits = logits.view(shape + (action_dim, ))
-        dist.set_param(logits.detach())
+        dist.set_param(logits=logits.detach())
         return dist
     else:
         pass
```

### Comparing `xuance-1.1.0/xuance/torch/utils/value_norm.py` & `xuance-1.1.1/xuance/torch/utils/value_norm.py`

 * *Files identical despite different names*

### Comparing `xuance-1.1.0/xuance.egg-info/SOURCES.txt` & `xuance-1.1.1/xuance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 xuance/configs/ippo/sc2/8m.yaml
 xuance/configs/ippo/sc2/8m_vs_9m.yaml
 xuance/configs/ippo/sc2/MMM2.yaml
 xuance/configs/ippo/sc2/corridor.yaml
 xuance/configs/iql/football/3v1.yaml
 xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml
 xuance/configs/iql/mpe/simple_spread_v3.yaml
+xuance/configs/iql/robotic_warehouse/rware-tiny-2ag-v1.yaml
 xuance/configs/iql/sc2/1c3s5z.yaml
 xuance/configs/iql/sc2/25m.yaml
 xuance/configs/iql/sc2/2m_vs_1z.yaml
 xuance/configs/iql/sc2/2s3z.yaml
 xuance/configs/iql/sc2/3m.yaml
 xuance/configs/iql/sc2/5m_vs_6m.yaml
 xuance/configs/iql/sc2/8m.yaml
@@ -117,14 +118,15 @@
 xuance/configs/maddpg/mpe/simple_push_v3.yaml
 xuance/configs/maddpg/mpe/simple_spread_v3.yaml
 xuance/configs/mappo/football/1v1.yaml
 xuance/configs/mappo/football/3v1.yaml
 xuance/configs/mappo/mpe/simple_adversary_v3.yaml
 xuance/configs/mappo/mpe/simple_push_v3.yaml
 xuance/configs/mappo/mpe/simple_spread_v3.yaml
+xuance/configs/mappo/robotic_warehouse/rware-tiny-2ag-v1.yaml
 xuance/configs/mappo/sc2/1c3s5z.yaml
 xuance/configs/mappo/sc2/25m.yaml
 xuance/configs/mappo/sc2/2m_vs_1z.yaml
 xuance/configs/mappo/sc2/2s3z.yaml
 xuance/configs/mappo/sc2/3m.yaml
 xuance/configs/mappo/sc2/5m_vs_6m.yaml
 xuance/configs/mappo/sc2/8m.yaml
@@ -178,14 +180,15 @@
 xuance/configs/ppo/box2d/LunarLander-v2.yaml
 xuance/configs/ppo/classic_control/Acrobot-v1.yaml
 xuance/configs/ppo/classic_control/CartPole-v1.yaml
 xuance/configs/ppo/classic_control/MountainCar-v0.yaml
 xuance/configs/ppo/classic_control/Pendulum-v1.yaml
 xuance/configs/qmix/football/3v1.yaml
 xuance/configs/qmix/mpe/simple_spread_v3.yaml
+xuance/configs/qmix/robotic_warehouse/rware-tiny-2ag-v1.yaml
 xuance/configs/qmix/sc2/1c3s5z.yaml
 xuance/configs/qmix/sc2/25m.yaml
 xuance/configs/qmix/sc2/2m_vs_1z.yaml
 xuance/configs/qmix/sc2/2s3z.yaml
 xuance/configs/qmix/sc2/3m.yaml
 xuance/configs/qmix/sc2/5m_vs_6m.yaml
 xuance/configs/qmix/sc2/8m.yaml
@@ -199,14 +202,15 @@
 xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
 xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
 xuance/configs/qtran/mpe/simple_spread_v3.yaml
 xuance/configs/random/mpe/simple_adversary.yaml
 xuance/configs/random/mpe/simple_push.yaml
 xuance/configs/random/mpe/simple_spread.yaml
 xuance/configs/sac/atari.yaml
+xuance/configs/sac/drones.yaml
 xuance/configs/sac/metadrive.yaml
 xuance/configs/sac/mujoco.yaml
 xuance/configs/sac/box2d/BipedalWalker-v3.yaml
 xuance/configs/sac/box2d/LunarLander-v2.yaml
 xuance/configs/sac/classic_control/Acrobot-v1.yaml
 xuance/configs/sac/classic_control/CartPole-v1.yaml
 xuance/configs/sac/classic_control/MountainCar-v0.yaml
@@ -225,14 +229,15 @@
 xuance/configs/vdac/sc2/8m.yaml
 xuance/configs/vdac/sc2/8m_vs_9m.yaml
 xuance/configs/vdac/sc2/MMM2.yaml
 xuance/configs/vdac/sc2/corridor.yaml
 xuance/configs/vdn/new_env_mas.yaml
 xuance/configs/vdn/football/3v1.yaml
 xuance/configs/vdn/mpe/simple_spread_v3.yaml
+xuance/configs/vdn/robotic_warehouse/rware-tiny-2ag-v1.yaml
 xuance/configs/vdn/sc2/1c3s5z.yaml
 xuance/configs/vdn/sc2/25m.yaml
 xuance/configs/vdn/sc2/2m_vs_1z.yaml
 xuance/configs/vdn/sc2/2s3z.yaml
 xuance/configs/vdn/sc2/3m.yaml
 xuance/configs/vdn/sc2/5m_vs_6m.yaml
 xuance/configs/vdn/sc2/8m.yaml
@@ -318,14 +323,15 @@
 xuance/environment/new_env_mas/new_env_mas.py
 xuance/environment/new_env_mas/new_vec_env_mas.py
 xuance/environment/pettingzoo/__init__.py
 xuance/environment/pettingzoo/pettingzoo_env.py
 xuance/environment/pettingzoo/pettingzoo_vec_env.py
 xuance/environment/robotic_warehouse/__init__.py
 xuance/environment/robotic_warehouse/robotic_warehouse_env.py
+xuance/environment/robotic_warehouse/robotic_warehouse_vec_env.py
 xuance/environment/starcraft2/__init__.py
 xuance/environment/starcraft2/sc2_env.py
 xuance/environment/starcraft2/sc2_vec_env.py
 xuance/environment/vector_envs/__init__.py
 xuance/environment/vector_envs/env_utils.py
 xuance/environment/vector_envs/subproc_vec_env.py
 xuance/environment/vector_envs/vector_env.py
```

