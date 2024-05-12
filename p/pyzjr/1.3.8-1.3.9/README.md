# Comparing `tmp/pyzjr-1.3.8.tar.gz` & `tmp/pyzjr-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.3.8.tar", last modified: Mon Apr 29 16:07:47 2024, max compression
+gzip compressed data, was "dist\pyzjr-1.3.9.tar", last modified: Sun May 12 03:18:57 2024, max compression
```

## Comparing `pyzjr-1.3.8.tar` & `pyzjr-1.3.9.tar`

### file list

```diff
@@ -1,220 +1,234 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/
--rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     2931 2024-04-29 16:07:47.000000 pyzjr-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/models_img/
--rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.8/models_img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Math/
--rw-rw-rw-   0        0        0      689 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/Numpy.py
--rw-rw-rw-   0        0        0      212 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/__init__.py
--rw-rw-rw-   0        0        0     3438 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/arithmetic.py
--rw-rw-rw-   0        0        0      134 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/constant.py
--rw-rw-rw-   0        0        0     7362 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/function.py
--rw-rw-rw-   0        0        0    19620 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Math/point_line.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/Attention/
--rw-rw-rw-   0        0        0     2271 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/A2.py
--rw-rw-rw-   0        0        0     1927 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/AFT.py
--rw-rw-rw-   0        0        0     1911 2024-04-29 07:40:57.000000 pyzjr-1.3.8/pyzjr/Models/Attention/DANet.py
--rw-rw-rw-   0        0        0     5412 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/MobileViT.py
--rw-rw-rw-   0        0        0     3105 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/SE.py
--rw-rw-rw-   0        0        0     1933 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/ViP.py
--rw-rw-rw-   0        0        0     1589 2024-04-29 07:40:19.000000 pyzjr-1.3.8/pyzjr/Models/Attention/__init__.py
--rw-rw-rw-   0        0        0     4795 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/acmix.py
--rw-rw-rw-   0        0        0    12705 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/axial.py
--rw-rw-rw-   0        0        0     3180 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/bam.py
--rw-rw-rw-   0        0        0     3729 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/cbam.py
--rw-rw-rw-   0        0        0     1635 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/coord.py
--rw-rw-rw-   0        0        0     2175 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/cot.py
--rw-rw-rw-   0        0        0     2688 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/crisscross.py
--rw-rw-rw-   0        0        0    26854 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/crossformer.py
--rw-rw-rw-   0        0        0    23025 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/dat.py
--rw-rw-rw-   0        0        0     1340 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/eca.py
--rw-rw-rw-   0        0        0     3752 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/emsa.py
--rw-rw-rw-   0        0        0     1341 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/external.py
--rw-rw-rw-   0        0        0     4161 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/gfnet.py
--rw-rw-rw-   0        0        0     5444 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/halo.py
--rw-rw-rw-   0        0        0    30578 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/moat.py
--rw-rw-rw-   0        0        0     3670 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/muse.py
--rw-rw-rw-   0        0        0     2281 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/outlook.py
--rw-rw-rw-   0        0        0      985 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/parnet.py
--rw-rw-rw-   0        0        0     4087 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/polarized.py
--rw-rw-rw-   0        0        0     2296 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/psa.py
--rw-rw-rw-   0        0        0      930 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/residual.py
--rw-rw-rw-   0        0        0     2355 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/s2.py
--rw-rw-rw-   0        0        0     3084 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/self_att.py
--rw-rw-rw-   0        0        0     1784 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/sge.py
--rw-rw-rw-   0        0        0     2637 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/shuffle.py
--rw-rw-rw-   0        0        0      909 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/simam.py
--rw-rw-rw-   0        0        0     2933 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/simplified_self_att.py
--rw-rw-rw-   0        0        0     1863 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/sk.py
--rw-rw-rw-   0        0        0     2349 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/triplet.py
--rw-rw-rw-   0        0        0     2234 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/Attention/ufo.py
--rw-rw-rw-   0        0        0      220 2024-04-29 07:38:52.000000 pyzjr-1.3.8/pyzjr/Models/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/backbone/
--rw-rw-rw-   0        0        0     5692 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/Darknet.py
--rw-rw-rw-   0        0        0    25919 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/Ghostnet.py
--rw-rw-rw-   0        0        0     1953 2024-04-29 07:42:05.000000 pyzjr-1.3.8/pyzjr/Models/backbone/__init__.py
--rw-rw-rw-   0        0        0     1935 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/alexnet.py
--rw-rw-rw-   0        0        0     7560 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/conv2former.py
--rw-rw-rw-   0        0        0     6278 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/densenet.py
--rw-rw-rw-   0        0        0    12866 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/drn.py
--rw-rw-rw-   0        0        0    17934 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/efficientnet.py
--rw-rw-rw-   0        0        0     7210 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/fasternet.py
--rw-rw-rw-   0        0        0     5623 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/googlenet.py
--rw-rw-rw-   0        0        0     1869 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/lenet.py
--rw-rw-rw-   0        0        0     7048 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/mnasnet.py
--rw-rw-rw-   0        0        0    16395 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/mobilenet.py
--rw-rw-rw-   0        0        0     9972 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/nasnet.py
--rw-rw-rw-   0        0        0     7217 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/regnet.py
--rw-rw-rw-   0        0        0     8910 2024-04-29 07:41:16.000000 pyzjr-1.3.8/pyzjr/Models/backbone/resnet.py
--rw-rw-rw-   0        0        0    11356 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/shufflenet.py
--rw-rw-rw-   0        0        0     4392 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/squeezenet.py
--rw-rw-rw-   0        0        0     3996 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/vgg.py
--rw-rw-rw-   0        0        0     5866 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/xception.py
--rw-rw-rw-   0        0        0     2705 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/backbone/zfnet.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/bricks/
--rw-rw-rw-   0        0        0     5577 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/Initer.py
--rw-rw-rw-   0        0        0      426 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/__init__.py
--rw-rw-rw-   0        0        0     1577 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/classfier.py
--rw-rw-rw-   0        0        0    22575 2024-04-29 07:40:36.000000 pyzjr-1.3.8/pyzjr/Models/bricks/comblock.py
--rw-rw-rw-   0        0        0     2646 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/conv_norm_act.py
--rw-rw-rw-   0        0        0     6828 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/drop.py
--rw-rw-rw-   0        0        0     6669 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/bricks/mlp.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/conv/
--rw-rw-rw-   0        0        0     1974 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/Depthwise_Conv.py
--rw-rw-rw-   0        0        0      508 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/Dilated_Conv.py
--rw-rw-rw-   0        0        0     1862 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/Partial_Conv.py
--rw-rw-rw-   0        0        0     2660 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/Ref_Conv.py
--rw-rw-rw-   0        0        0    11456 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/Snake_Conv.py
--rw-rw-rw-   0        0        0      295 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/conv/__init__.py
--rw-rw-rw-   0        0        0     3029 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/networks.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/sampling/
--rw-rw-rw-   0        0        0      754 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/__init__.py
--rw-rw-rw-   0        0        0     4857 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/adaptivepooling.py
--rw-rw-rw-   0        0        0     1393 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/haarwavelet.py
--rw-rw-rw-   0        0        0     1828 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/medianpooling.py
--rw-rw-rw-   0        0        0     4792 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/standardpooling.py
--rw-rw-rw-   0        0        0      854 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/strideconv.py
--rw-rw-rw-   0        0        0     3692 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/sampling/strippooling.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/Models/segmentation/
--rw-rw-rw-   0        0        0       70 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/segmentation/__init__.py
--rw-rw-rw-   0        0        0    24988 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/segmentation/fcn.py
--rw-rw-rw-   0        0        0     3289 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Models/segmentation/unet.py
--rw-rw-rw-   0        0        0     6328 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/PIC.py
--rw-rw-rw-   0        0        0    10349 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/Z.py
--rw-rw-rw-   0        0        0      896 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/augmentation/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/
--rw-rw-rw-   0        0        0    13180 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/Crack.py
--rw-rw-rw-   0        0        0     8307 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/_Steger.py
--rw-rw-rw-   0        0        0      366 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/__init__.py
--rw-rw-rw-   0        0        0     7681 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/definition.py
--rw-rw-rw-   0        0        0     4835 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/pixel.py
--rw-rw-rw-   0        0        0     1685 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/Pixel/utils.py
--rw-rw-rw-   0        0        0      116 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/__init__.py
--rw-rw-rw-   0        0        0    28649 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/augments.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/
--rw-rw-rw-   0        0        0      306 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/_utils.py
--rw-rw-rw-   0        0        0     3413 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/normal.py
--rw-rw-rw-   0        0        0    10459 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/opencv.py
--rw-rw-rw-   0        0        0    40685 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/pillow.py
--rw-rw-rw-   0        0        0     6139 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/transforms/tvision.py
--rw-rw-rw-   0        0        0     1084 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/augmentation/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/core/
--rw-rw-rw-   0        0        0     1136 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/__init__.py
--rw-rw-rw-   0        0        0     6991 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/__tensor.py
--rw-rw-rw-   0        0        0      680 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/_utils.py
--rw-rw-rw-   0        0        0      982 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/decorator.py
--rw-rw-rw-   0        0        0     2123 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/error.py
--rw-rw-rw-   0        0        0     2692 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/general.py
--rw-rw-rw-   0        0        0      671 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/helpers.py
--rw-rw-rw-   0        0        0     7254 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/lr_scheduler.py
--rw-rw-rw-   0        0        0    15534 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/core/utils_pytorch_numpy_unification.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/data/
--rw-rw-rw-   0        0        0     1486 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/Dataloader.py
--rw-rw-rw-   0        0        0     9590 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/Dataset.py
--rw-rw-rw-   0        0        0    12147 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/FM.py
--rw-rw-rw-   0        0        0      215 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/basedataset.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/data/data_set/
--rw-rw-rw-   0        0        0     9436 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/data_set/Pascal_voc.py
--rw-rw-rw-   0        0        0        0 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/data_set/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/data_set/config.py
--rw-rw-rw-   0        0        0    15340 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/reader.py
--rw-rw-rw-   0        0        0      934 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/data/txt_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/devices/
--rw-rw-rw-   0        0        0      523 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/devices/__init__.py
--rw-rw-rw-   0        0        0     1572 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/devices/get_device.py
--rw-rw-rw-   0        0        0     3032 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/devices/measures.py
--rw-rw-rw-   0        0        0     1202 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/devices/systeminfo.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/dlearn/
--rw-rw-rw-   0        0        0      949 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/__init__.py
--rw-rw-rw-   0        0        0     8571 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/callbacklog.py
--rw-rw-rw-   0        0        0     8379 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/callbacks.py
--rw-rw-rw-   0        0        0     1051 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/savemodels.py
--rw-rw-rw-   0        0        0     5603 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/strategy.py
--rw-rw-rw-   0        0        0     5955 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/tools.py
--rw-rw-rw-   0        0        0     7356 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/dlearn/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/nn/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/
--rw-rw-rw-   0        0        0      768 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/__init__.py
--rw-rw-rw-   0        0        0    16268 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/classification.py
--rw-rw-rw-   0        0        0     3822 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/indexutils.py
--rw-rw-rw-   0        0        0     9779 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/medical_index.py
--rw-rw-rw-   0        0        0     5837 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/segment3d.py
--rw-rw-rw-   0        0        0    11847 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Metrics/semantic.py
--rw-rw-rw-   0        0        0     9459 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/Summary.py
--rw-rw-rw-   0        0        0      123 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/__init__.py
--rw-rw-rw-   0        0        0    84332 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/functional.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/
--rw-rw-rw-   0        0        0     3262 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/OneHot.py
--rw-rw-rw-   0        0        0      835 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/__init__.py
--rw-rw-rw-   0        0        0     7197 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/avgweight.py
--rw-rw-rw-   0        0        0    15225 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/learnrate.py
--rw-rw-rw-   0        0        0    27275 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/loss_function.py
--rw-rw-rw-   0        0        0     5217 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/nn/torchutils/loss_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/torch3D/
--rw-rw-rw-   0        0        0       57 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/
--rw-rw-rw-   0        0        0      266 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/basic_unet.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/block/
--rw-rw-rw-   0        0        0    22077 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/block/DSConv.py
--rw-rw-rw-   0        0        0       28 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/block/__init__.py
--rw-rw-rw-   0        0        0     7909 2024-04-29 08:00:13.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/dscnet.py
--rw-rw-rw-   0        0        0     5755 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/networks/vent.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/torch3D/nii/
--rw-rw-rw-   0        0        0      306 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/nii/__init__.py
--rw-rw-rw-   0        0        0     4420 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/nii/mri.py
--rw-rw-rw-   0        0        0     4363 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/nii/nifti_dataset.py
--rw-rw-rw-   0        0        0     3373 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/torch3D/nii/nii_utils.py
--rw-rw-rw-   0        0        0       21 2024-04-29 16:07:44.000000 pyzjr-1.3.8/pyzjr/version.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/visualize/
--rw-rw-rw-   0        0        0      410 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/visualize/color/
--rw-rw-rw-   0        0        0     1418 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/__init__.py
--rw-rw-rw-   0        0        0     4848 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/colormap.py
--rw-rw-rw-   0        0        0     3339 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/colorspace.py
--rw-rw-rw-   0        0        0     7471 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/cvplot.py
--rw-rw-rw-   0        0        0     7937 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/findcolor.py
--rw-rw-rw-   0        0        0     1066 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/color/hex.py
--rw-rw-rw-   0        0        0    10972 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/io.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:47.000000 pyzjr-1.3.8/pyzjr/visualize/mediapipe/
--rw-rw-rw-   0        0        0     6556 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/mediapipe/HandTrack.py
--rw-rw-rw-   0        0        0      376 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/mediapipe/__init__.py
--rw-rw-rw-   0        0        0      631 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/mediapipe/const.py
--rw-rw-rw-   0        0        0     4327 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/printf.py
--rw-rw-rw-   0        0        0     3367 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/utils.py
--rw-rw-rw-   0        0        0     3796 2024-04-29 07:37:02.000000 pyzjr-1.3.8/pyzjr/visualize/video_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2931 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7154 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 16:07:46.000000 pyzjr-1.3.8/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 16:07:47.000000 pyzjr-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2187 2024-04-29 16:07:44.000000 pyzjr-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/
+-rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-05-12 03:18:57.000000 pyzjr-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/models_img/
+-rw-rw-rw-   0        0        0    13179 2024-05-11 10:42:51.000000 pyzjr-1.3.9/models_img/Crack.py
+-rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.9/models_img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/models_img/test_crack_measure/
+-rw-rw-rw-   0        0        0        0 2024-05-11 15:43:43.000000 pyzjr-1.3.9/models_img/test_crack_measure/__init__.py
+-rw-rw-rw-   0        0        0     4626 2024-05-11 15:46:11.000000 pyzjr-1.3.9/models_img/test_crack_measure/crack_type.py
+-rw-rw-rw-   0        0        0     8886 2024-05-11 15:56:59.000000 pyzjr-1.3.9/models_img/test_crack_measure/pixel.py
+-rw-rw-rw-   0        0        0     2941 2024-05-11 15:46:11.000000 pyzjr-1.3.9/models_img/test_crack_measure/skeleton_extraction.py
+-rw-rw-rw-   0        0        0     3015 2024-05-11 15:46:11.000000 pyzjr-1.3.9/models_img/test_crack_measure/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Math/
+-rw-rw-rw-   0        0        0      689 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/Numpy.py
+-rw-rw-rw-   0        0        0      212 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/__init__.py
+-rw-rw-rw-   0        0        0     3438 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/arithmetic.py
+-rw-rw-rw-   0        0        0      134 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/constant.py
+-rw-rw-rw-   0        0        0     7362 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/function.py
+-rw-rw-rw-   0        0        0    19620 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Math/point_line.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/Attention/
+-rw-rw-rw-   0        0        0     2271 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/A2.py
+-rw-rw-rw-   0        0        0     1927 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/AFT.py
+-rw-rw-rw-   0        0        0     1911 2024-04-29 07:40:57.000000 pyzjr-1.3.9/pyzjr/Models/Attention/DANet.py
+-rw-rw-rw-   0        0        0     5412 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/MobileViT.py
+-rw-rw-rw-   0        0        0     3105 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/SE.py
+-rw-rw-rw-   0        0        0     1933 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/ViP.py
+-rw-rw-rw-   0        0        0     1589 2024-04-29 07:40:19.000000 pyzjr-1.3.9/pyzjr/Models/Attention/__init__.py
+-rw-rw-rw-   0        0        0     4795 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/acmix.py
+-rw-rw-rw-   0        0        0    12705 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/axial.py
+-rw-rw-rw-   0        0        0     3180 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/bam.py
+-rw-rw-rw-   0        0        0     3729 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/cbam.py
+-rw-rw-rw-   0        0        0     1635 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/coord.py
+-rw-rw-rw-   0        0        0     2175 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/cot.py
+-rw-rw-rw-   0        0        0     2688 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/crisscross.py
+-rw-rw-rw-   0        0        0    26854 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/crossformer.py
+-rw-rw-rw-   0        0        0    23025 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/dat.py
+-rw-rw-rw-   0        0        0     1340 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/eca.py
+-rw-rw-rw-   0        0        0     3752 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/emsa.py
+-rw-rw-rw-   0        0        0     1341 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/external.py
+-rw-rw-rw-   0        0        0     4161 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/gfnet.py
+-rw-rw-rw-   0        0        0     5444 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/halo.py
+-rw-rw-rw-   0        0        0    30578 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/moat.py
+-rw-rw-rw-   0        0        0     3670 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/muse.py
+-rw-rw-rw-   0        0        0     2281 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/outlook.py
+-rw-rw-rw-   0        0        0      985 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/parnet.py
+-rw-rw-rw-   0        0        0     4087 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/polarized.py
+-rw-rw-rw-   0        0        0     2296 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/psa.py
+-rw-rw-rw-   0        0        0      930 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/residual.py
+-rw-rw-rw-   0        0        0     2355 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/s2.py
+-rw-rw-rw-   0        0        0     3084 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/self_att.py
+-rw-rw-rw-   0        0        0     1784 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/sge.py
+-rw-rw-rw-   0        0        0     2637 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/shuffle.py
+-rw-rw-rw-   0        0        0      909 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/simam.py
+-rw-rw-rw-   0        0        0     2933 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/simplified_self_att.py
+-rw-rw-rw-   0        0        0     1863 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/sk.py
+-rw-rw-rw-   0        0        0     2349 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/triplet.py
+-rw-rw-rw-   0        0        0     2234 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/Attention/ufo.py
+-rw-rw-rw-   0        0        0      220 2024-04-29 07:38:52.000000 pyzjr-1.3.9/pyzjr/Models/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/backbone/
+-rw-rw-rw-   0        0        0     5692 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/Darknet.py
+-rw-rw-rw-   0        0        0    25919 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/Ghostnet.py
+-rw-rw-rw-   0        0        0     1953 2024-04-29 07:42:05.000000 pyzjr-1.3.9/pyzjr/Models/backbone/__init__.py
+-rw-rw-rw-   0        0        0     1935 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/alexnet.py
+-rw-rw-rw-   0        0        0     7560 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/conv2former.py
+-rw-rw-rw-   0        0        0     6278 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/densenet.py
+-rw-rw-rw-   0        0        0    12866 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/drn.py
+-rw-rw-rw-   0        0        0    17934 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/efficientnet.py
+-rw-rw-rw-   0        0        0     7210 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/fasternet.py
+-rw-rw-rw-   0        0        0     5623 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/googlenet.py
+-rw-rw-rw-   0        0        0     1869 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/lenet.py
+-rw-rw-rw-   0        0        0     7048 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/mnasnet.py
+-rw-rw-rw-   0        0        0    16395 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/mobilenet.py
+-rw-rw-rw-   0        0        0     9972 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/nasnet.py
+-rw-rw-rw-   0        0        0     7217 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/regnet.py
+-rw-rw-rw-   0        0        0     8910 2024-04-29 07:41:16.000000 pyzjr-1.3.9/pyzjr/Models/backbone/resnet.py
+-rw-rw-rw-   0        0        0    11356 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/shufflenet.py
+-rw-rw-rw-   0        0        0     4392 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/squeezenet.py
+-rw-rw-rw-   0        0        0     3996 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/vgg.py
+-rw-rw-rw-   0        0        0     5866 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/xception.py
+-rw-rw-rw-   0        0        0     2705 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/backbone/zfnet.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/bricks/
+-rw-rw-rw-   0        0        0     5577 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/bricks/Initer.py
+-rw-rw-rw-   0        0        0      487 2024-05-04 09:16:09.000000 pyzjr-1.3.9/pyzjr/Models/bricks/__init__.py
+-rw-rw-rw-   0        0        0     1577 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/bricks/classfier.py
+-rw-rw-rw-   0        0        0    22038 2024-05-04 09:16:09.000000 pyzjr-1.3.9/pyzjr/Models/bricks/comblock.py
+-rw-rw-rw-   0        0        0     3099 2024-05-06 14:21:54.000000 pyzjr-1.3.9/pyzjr/Models/bricks/conv_norm_act.py
+-rw-rw-rw-   0        0        0     6828 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/bricks/drop.py
+-rw-rw-rw-   0        0        0     6669 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/bricks/mlp.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/conv/
+-rw-rw-rw-   0        0        0     1974 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/Depthwise_Conv.py
+-rw-rw-rw-   0        0        0      508 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/Dilated_Conv.py
+-rw-rw-rw-   0        0        0     1862 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/Partial_Conv.py
+-rw-rw-rw-   0        0        0     2660 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/Ref_Conv.py
+-rw-rw-rw-   0        0        0    11456 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/Snake_Conv.py
+-rw-rw-rw-   0        0        0      295 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/conv/__init__.py
+-rw-rw-rw-   0        0        0     3029 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/networks.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/sampling/
+-rw-rw-rw-   0        0        0      754 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/__init__.py
+-rw-rw-rw-   0        0        0     4857 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/adaptivepooling.py
+-rw-rw-rw-   0        0        0     1393 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/haarwavelet.py
+-rw-rw-rw-   0        0        0     1828 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/medianpooling.py
+-rw-rw-rw-   0        0        0     4792 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/standardpooling.py
+-rw-rw-rw-   0        0        0      854 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/strideconv.py
+-rw-rw-rw-   0        0        0     3692 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/Models/sampling/strippooling.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/Models/segmentation/
+-rw-rw-rw-   0        0        0      181 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/Models/segmentation/__init__.py
+-rw-rw-rw-   0        0        0    24917 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/Models/segmentation/fcn.py
+-rw-rw-rw-   0        0        0     3281 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/Models/segmentation/unet.py
+-rw-rw-rw-   0        0        0    10316 2024-05-11 08:54:26.000000 pyzjr-1.3.9/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      864 2024-05-11 16:15:32.000000 pyzjr-1.3.9/pyzjr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/augmentation/
+-rw-rw-rw-   0        0        0     3780 2024-05-11 16:19:09.000000 pyzjr-1.3.9/pyzjr/augmentation/PIC.py
+-rw-rw-rw-   0        0        0     1149 2024-05-11 16:38:16.000000 pyzjr-1.3.9/pyzjr/augmentation/__init__.py
+-rw-rw-rw-   0        0        0    21827 2024-05-11 16:38:16.000000 pyzjr-1.3.9/pyzjr/augmentation/augments.py
+-rw-rw-rw-   0        0        0     4479 2024-05-11 16:38:15.000000 pyzjr-1.3.9/pyzjr/augmentation/blur.py
+-rw-rw-rw-   0        0        0     8860 2024-05-11 12:10:14.000000 pyzjr-1.3.9/pyzjr/augmentation/mask_ops.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/
+-rw-rw-rw-   0        0        0     1741 2024-05-11 16:38:16.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/__init__.py
+-rw-rw-rw-   0        0        0     4224 2024-05-10 15:43:50.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/_utils.py
+-rw-rw-rw-   0        0        0     4164 2024-05-11 16:38:15.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/normal.py
+-rw-rw-rw-   0        0        0    10523 2024-05-11 16:38:16.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/opencv.py
+-rw-rw-rw-   0        0        0    40681 2024-05-10 16:31:02.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/pillow.py
+-rw-rw-rw-   0        0        0     6270 2024-05-11 16:38:16.000000 pyzjr-1.3.9/pyzjr/augmentation/transforms/tvision.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/core/
+-rw-rw-rw-   0        0        0     1034 2024-05-11 08:34:49.000000 pyzjr-1.3.9/pyzjr/core/__init__.py
+-rw-rw-rw-   0        0        0     6991 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/core/__tensor.py
+-rw-rw-rw-   0        0        0      863 2024-05-10 16:27:29.000000 pyzjr-1.3.9/pyzjr/core/_utils.py
+-rw-rw-rw-   0        0        0      982 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/core/decorator.py
+-rw-rw-rw-   0        0        0     2071 2024-05-10 16:09:23.000000 pyzjr-1.3.9/pyzjr/core/error.py
+-rw-rw-rw-   0        0        0     3040 2024-05-11 08:39:17.000000 pyzjr-1.3.9/pyzjr/core/general.py
+-rw-rw-rw-   0        0        0      671 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/core/helpers.py
+-rw-rw-rw-   0        0        0     7254 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/core/lr_scheduler.py
+-rw-rw-rw-   0        0        0    15534 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/core/utils_pytorch_numpy_unification.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/data/
+-rw-rw-rw-   0        0        0     1486 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/Dataloader.py
+-rw-rw-rw-   0        0        0     9590 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/Dataset.py
+-rw-rw-rw-   0        0        0    12148 2024-05-02 16:02:08.000000 pyzjr-1.3.9/pyzjr/data/FM.py
+-rw-rw-rw-   0        0        0      247 2024-05-11 16:38:15.000000 pyzjr-1.3.9/pyzjr/data/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/basedataset.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/data/data_set/
+-rw-rw-rw-   0        0        0     9436 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/data_set/Pascal_voc.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/data_set/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/data_set/config.py
+-rw-rw-rw-   0        0        0    15340 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/data/reader.py
+-rw-rw-rw-   0        0        0      974 2024-05-02 16:49:01.000000 pyzjr-1.3.9/pyzjr/data/txt_utils.py
+-rw-rw-rw-   0        0        0      250 2024-05-04 09:04:32.000000 pyzjr-1.3.9/pyzjr/data/yaml_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/devices/
+-rw-rw-rw-   0        0        0      574 2024-05-10 16:50:18.000000 pyzjr-1.3.9/pyzjr/devices/__init__.py
+-rw-rw-rw-   0        0        0     2022 2024-05-11 06:49:37.000000 pyzjr-1.3.9/pyzjr/devices/get_device.py
+-rw-rw-rw-   0        0        0     3422 2024-05-04 08:38:51.000000 pyzjr-1.3.9/pyzjr/devices/measures.py
+-rw-rw-rw-   0        0        0     1204 2024-05-04 08:42:43.000000 pyzjr-1.3.9/pyzjr/devices/systeminfo.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/dlearn/
+-rw-rw-rw-   0        0        0     1023 2024-05-02 14:43:13.000000 pyzjr-1.3.9/pyzjr/dlearn/__init__.py
+-rw-rw-rw-   0        0        0     8571 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/dlearn/callbacklog.py
+-rw-rw-rw-   0        0        0     8379 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/dlearn/callbacks.py
+-rw-rw-rw-   0        0        0     1930 2024-05-11 06:57:55.000000 pyzjr-1.3.9/pyzjr/dlearn/save_pth.py
+-rw-rw-rw-   0        0        0     4925 2024-05-11 06:49:37.000000 pyzjr-1.3.9/pyzjr/dlearn/strategy.py
+-rw-rw-rw-   0        0        0     5781 2024-05-02 14:21:27.000000 pyzjr-1.3.9/pyzjr/dlearn/tools.py
+-rw-rw-rw-   0        0        0     7356 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/dlearn/trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/measure/
+-rw-rw-rw-   0        0        0      394 2024-05-11 16:15:32.000000 pyzjr-1.3.9/pyzjr/measure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/measure/crack/
+-rw-rw-rw-   0        0        0      296 2024-05-11 15:56:59.000000 pyzjr-1.3.9/pyzjr/measure/crack/__init__.py
+-rw-rw-rw-   0        0        0     3082 2024-05-11 15:56:59.000000 pyzjr-1.3.9/pyzjr/measure/crack/attribute.py
+-rw-rw-rw-   0        0        0     4712 2024-05-12 01:40:37.000000 pyzjr-1.3.9/pyzjr/measure/crack/crack_type.py
+-rw-rw-rw-   0        0        0     2955 2024-05-11 12:36:35.000000 pyzjr-1.3.9/pyzjr/measure/crack/skeleton_extraction.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/measure/dehaze/
+-rw-rw-rw-   0        0        0      189 2024-05-11 16:15:32.000000 pyzjr-1.3.9/pyzjr/measure/dehaze/__init__.py
+-rw-rw-rw-   0        0        0     3349 2024-05-11 16:01:15.000000 pyzjr-1.3.9/pyzjr/measure/dehaze/eval_definition.py
+-rw-rw-rw-   0        0        0     3339 2024-05-11 16:15:32.000000 pyzjr-1.3.9/pyzjr/measure/dehaze/vague.py
+-rw-rw-rw-   0        0        0     5438 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/measure/pixel.py
+-rw-rw-rw-   0        0        0     8029 2024-05-11 11:42:15.000000 pyzjr-1.3.9/pyzjr/measure/steger.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/nn/
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/
+-rw-rw-rw-   0        0        0      857 2024-05-02 12:54:19.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/__init__.py
+-rw-rw-rw-   0        0        0    16274 2024-05-02 12:54:19.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/classification.py
+-rw-rw-rw-   0        0        0    13011 2024-05-02 12:56:38.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/indexutils.py
+-rw-rw-rw-   0        0        0     9773 2024-05-02 15:41:09.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/medical_index.py
+-rw-rw-rw-   0        0        0     6273 2024-05-02 14:02:12.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/segment3d.py
+-rw-rw-rw-   0        0        0    11847 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/Metrics/semantic.py
+-rw-rw-rw-   0        0        0     9506 2024-05-02 14:02:24.000000 pyzjr-1.3.9/pyzjr/nn/Summary.py
+-rw-rw-rw-   0        0        0      123 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/__init__.py
+-rw-rw-rw-   0        0        0    84332 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/functional.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/
+-rw-rw-rw-   0        0        0     3262 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/OneHot.py
+-rw-rw-rw-   0        0        0      835 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/__init__.py
+-rw-rw-rw-   0        0        0     7197 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/avgweight.py
+-rw-rw-rw-   0        0        0    15225 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/learnrate.py
+-rw-rw-rw-   0        0        0    27275 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/loss_function.py
+-rw-rw-rw-   0        0        0     5217 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/nn/torchutils/loss_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/torch3D/
+-rw-rw-rw-   0        0        0       57 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/
+-rw-rw-rw-   0        0        0      319 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/basic_unet.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/block/
+-rw-rw-rw-   0        0        0    22077 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/block/DSConv.py
+-rw-rw-rw-   0        0        0       28 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/block/__init__.py
+-rw-rw-rw-   0        0        0     7895 2024-05-12 03:15:49.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/dscnet.py
+-rw-rw-rw-   0        0        0     5755 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/networks/vnet.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/torch3D/nii/
+-rw-rw-rw-   0        0        0      306 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/nii/__init__.py
+-rw-rw-rw-   0        0        0     4420 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/nii/mri.py
+-rw-rw-rw-   0        0        0     4197 2024-05-02 14:09:27.000000 pyzjr-1.3.9/pyzjr/torch3D/nii/nifti_dataset.py
+-rw-rw-rw-   0        0        0     3373 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/torch3D/nii/nii_utils.py
+-rw-rw-rw-   0        0        0       21 2024-05-12 03:18:52.000000 pyzjr-1.3.9/pyzjr/version.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/visualize/
+-rw-rw-rw-   0        0        0      340 2024-05-11 10:07:16.000000 pyzjr-1.3.9/pyzjr/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/visualize/color/
+-rw-rw-rw-   0        0        0     1418 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/colormap.py
+-rw-rw-rw-   0        0        0     3339 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/colorspace.py
+-rw-rw-rw-   0        0        0     7471 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/cvplot.py
+-rw-rw-rw-   0        0        0     7937 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/findcolor.py
+-rw-rw-rw-   0        0        0     1066 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/color/hex.py
+-rw-rw-rw-   0        0        0    10970 2024-05-11 10:15:19.000000 pyzjr-1.3.9/pyzjr/visualize/io.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr/visualize/mediapipe/
+-rw-rw-rw-   0        0        0     6556 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/mediapipe/HandTrack.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/mediapipe/__init__.py
+-rw-rw-rw-   0        0        0      631 2024-04-29 07:37:02.000000 pyzjr-1.3.9/pyzjr/visualize/mediapipe/const.py
+-rw-rw-rw-   0        0        0     4325 2024-05-04 08:34:26.000000 pyzjr-1.3.9/pyzjr/visualize/printf.py
+-rw-rw-rw-   0        0        0     3769 2024-05-02 14:18:08.000000 pyzjr-1.3.9/pyzjr/visualize/video_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7535 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 03:18:57.000000 pyzjr-1.3.9/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 03:18:57.000000 pyzjr-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2024-05-12 03:18:52.000000 pyzjr-1.3.9/setup.py
```

### Comparing `pyzjr-1.3.8/LICENSE` & `pyzjr-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/PKG-INFO` & `pyzjr-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.8
+Version: 1.3.9
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.8/README.md` & `pyzjr-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Math/Numpy.py` & `pyzjr-1.3.9/pyzjr/Math/Numpy.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Math/arithmetic.py` & `pyzjr-1.3.9/pyzjr/Math/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Math/function.py` & `pyzjr-1.3.9/pyzjr/Math/function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Math/point_line.py` & `pyzjr-1.3.9/pyzjr/Math/point_line.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/A2.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/A2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/AFT.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/AFT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/DANet.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/DANet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/MobileViT.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/MobileViT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/SE.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/SE.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/ViP.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/ViP.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/__init__.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/acmix.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/acmix.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/axial.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/axial.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/bam.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/bam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/cbam.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/cbam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/coord.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/coord.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/cot.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/cot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/crisscross.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/crisscross.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/crossformer.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/crossformer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/dat.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/dat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/eca.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/eca.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/emsa.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/emsa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/external.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/external.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/gfnet.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/gfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/halo.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/halo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/moat.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/moat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/muse.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/muse.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/outlook.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/outlook.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/parnet.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/parnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/polarized.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/polarized.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/psa.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/psa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/residual.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/residual.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/s2.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/s2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/self_att.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/sge.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/sge.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/shuffle.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/shuffle.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/simam.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/simam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/simplified_self_att.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/simplified_self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/sk.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/sk.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/triplet.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/triplet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/Attention/ufo.py` & `pyzjr-1.3.9/pyzjr/Models/Attention/ufo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/_utils.py` & `pyzjr-1.3.9/pyzjr/Models/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/Darknet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/Darknet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/Ghostnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/Ghostnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/__init__.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/alexnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/alexnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/conv2former.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/conv2former.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/densenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/densenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/drn.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/drn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/efficientnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/fasternet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/fasternet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/googlenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/googlenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/lenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/lenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/mnasnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/mnasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/mobilenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/nasnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/nasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/regnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/resnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/shufflenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/shufflenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/squeezenet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/vgg.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/xception.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/xception.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/backbone/zfnet.py` & `pyzjr-1.3.9/pyzjr/Models/backbone/zfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/Initer.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/Initer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/classfier.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/classfier.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/comblock.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/comblock.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,16 @@
 Time: 2024-01-28 0:59
 """
 import torch
 import math
 import torch.nn as nn
 import torch.nn.functional as F
 from pyzjr.Models.Attention import BAMAttention, SEAttention
+from pyzjr.Models.bricks.conv_norm_act import conv1x1, conv3x3
 
-def conv3x3(in_channels, out_channels, stride=1, groups=1, dilation=1):
-    """3x3 convolution with padding:捕捉局部特征和空间相关性，学习更复杂的特征和抽象表示"""
-    return nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=stride,
-                     padding=dilation, groups=groups, bias=False, dilation=dilation)
-
-def conv1x1(in_channels, out_channels, stride=1):
-    """1x1 convolution:实现降维或升维，调整通道数和执行通道间的线性变换"""
-    return nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=False)
 
 class ConvBNReLU(nn.Module):
     def __init__(self, in_channels, out_channels, stride=1,  kernel_size=3, padding=1,
                  **kwargs):
         super(ConvBNReLU, self).__init__()
         self.conv = nn.Conv2d(in_channels=in_channels, out_channels=out_channels,
                               kernel_size=kernel_size, stride=stride, padding=padding,
```

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/conv_norm_act.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/conv_norm_act.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,27 +49,26 @@
                  kernel_size=3,
                  stride=1,
                  padding=1,
                  dilation=1,
                  groups=1,
                  bias=False,
                  norm_layer=nn.BatchNorm2d,
-                 act_layer=nn.ReLU(inplace=True),
                  **kwargs,):
         super().__init__(in_channels=in_channels,
                          out_channels=out_channels,
                          kernel_size=kernel_size,
                          stride=stride,
                          padding=padding,
                          dilation=dilation,
                          groups=groups,
                          bias=bias,
                          apply_act=False,
                          norm_layer=norm_layer,
-                         act_layer=act_layer,
+                         act_layer=nn.ReLU(inplace=True),  # ignore, actually not working
                          **kwargs,)
 
 class NormAct(nn.Module):
     def __init__(self,
                  out_channels,
                  norm_layer=nn.BatchNorm2d,
                  act_layer=nn.ReLU(inplace=True),
@@ -79,11 +78,20 @@
         self.act_layer = act_layer
 
     def forward(self, x):
         x = self.norm_layer(x)
         x = self.act_layer(x)
         return x
 
+def conv3x3(in_channels, out_channels, stride=1, groups=1, dilation=1, bias=False):
+    """3x3 convolution"""
+    return nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=stride,
+                     padding=dilation, groups=groups, bias=bias, dilation=dilation)
+
+def conv1x1(in_channels, out_channels, stride=1, bias=False):
+    """1x1 convolution"""
+    return nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, bias=bias)
+
 
 ConvBnReLU = ConvNormAct
 ConvBn = ConvNorm
 BnReLU = NormAct
```

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/drop.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/bricks/mlp.py` & `pyzjr-1.3.9/pyzjr/Models/bricks/mlp.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/conv/Depthwise_Conv.py` & `pyzjr-1.3.9/pyzjr/Models/conv/Depthwise_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/conv/Partial_Conv.py` & `pyzjr-1.3.9/pyzjr/Models/conv/Partial_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/conv/Ref_Conv.py` & `pyzjr-1.3.9/pyzjr/Models/conv/Ref_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/conv/Snake_Conv.py` & `pyzjr-1.3.9/pyzjr/Models/conv/Snake_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/networks.py` & `pyzjr-1.3.9/pyzjr/Models/networks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/__init__.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/adaptivepooling.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/adaptivepooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/haarwavelet.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/haarwavelet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/medianpooling.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/medianpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/standardpooling.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/standardpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/strideconv.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/strideconv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/sampling/strippooling.py` & `pyzjr-1.3.9/pyzjr/Models/sampling/strippooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/Models/segmentation/fcn.py` & `pyzjr-1.3.9/pyzjr/Models/segmentation/fcn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import torch
 import torch.nn as nn
 from torchvision.models import vgg16_bn, vgg19_bn, vgg13_bn, vgg11_bn, \
                                resnet50, resnet101, resnet152
 from pyzjr.Models.bricks.comblock import _DenseBlock
 from pyzjr.Models.bricks.conv_norm_act import ConvBnReLU
 
-__all__ = ["VggFCN8s", "VggFCN16s", "VggFCN32s", "VggFCNs", "VggFCN", "ResFCN", "DenseFCN"]
-
 class FCN32s(nn.Module):
     def __init__(self, num_classes=21):
         super(FCN32s, self).__init__()
         self.block1 = nn.Sequential(
             nn.Conv2d(3, 64, 3),
             nn.BatchNorm2d(64),
             nn.ReLU(),
@@ -398,15 +396,15 @@
         x = self.deconv4(x)
         x = self.deconv5(x)
 
         return x
 
 
 class MobileFCN(nn.Module):
-    def __init__(self, ch_in=3, num_classes=21):
+    def __init__(self, in_channels=3, num_classes=21):
         super(MobileFCN, self).__init__()
 
         # 标准卷积
         def conv_bn(inp, oup, stride):
             return nn.Sequential(
                 nn.Conv2d(inp, oup, 3, stride, 1, bias=False),
                 nn.BatchNorm2d(oup),
@@ -420,15 +418,15 @@
                 nn.ReLU(inplace=True),
 
                 nn.Conv2d(inp, oup, 1, 1, 0, bias=False),
                 nn.BatchNorm2d(oup),
                 nn.ReLU(inplace=True))
 
         # 网络模型声明
-        self.encoder1 = conv_bn(ch_in, 32, 2)                                                              # 240,240,32
+        self.encoder1 = conv_bn(in_channels, 32, 2)                                                              # 240,240,32
         self.encoder2 = nn.Sequential(conv_dw(32, 64, 1), conv_dw(64, 128, 2))                             # 120,120,128
         self.encoder3 = nn.Sequential(conv_dw(128, 128, 1), conv_dw(128, 256, 2))                          # 60,60,256
         self.encoder4 = nn.Sequential(conv_dw(256, 256, 1), conv_dw(256, 512, 2))                          # 30,30,512
         self.encoder5 = nn.Sequential(conv_dw(512, 512, 1), conv_dw(512, 512, 1), conv_dw(512, 512, 1),
                                       conv_dw(512, 512, 1), conv_dw(512, 512, 1), conv_dw(512, 1024, 2),
                                       conv_dw(1024, 1024, 1))                                              # 15,15,1024
         self.relu = nn.ReLU(inplace=True)
@@ -460,15 +458,15 @@
         x = self.bn5(self.relu(self.decoder5(x)))
         x = self.classifier(x)
 
         return x
 
 
 class MobileFCN1(nn.Module):
-    def __init__(self, ch_in=3, num_classes=21):
+    def __init__(self, in_channels=3, num_classes=21):
         super(MobileFCN1, self).__init__()
 
         # 标准卷积
         def conv_bn(inp, oup, stride):
             return nn.Sequential(
                 nn.Conv2d(inp, oup, 3, stride, 1, bias=False),
                 nn.BatchNorm2d(oup),
@@ -489,15 +487,15 @@
             return nn.Sequential(
                 nn.Upsample(scale_factor=2),
                 nn.Conv2d(ch_in, ch_out, kernel_size=3, stride=1, padding=1, bias=True),
                 nn.BatchNorm2d(ch_out),
                 nn.ReLU(inplace=True)
             )
 
-        self.encoder1 = conv_bn(ch_in, 32, 2)                                                              # 240,240,32
+        self.encoder1 = conv_bn(in_channels, 32, 2)                                                              # 240,240,32
         self.encoder2 = nn.Sequential(conv_dw(32, 64, 1), conv_dw(64, 128, 2))                             # 120,120,128
         self.encoder3 = nn.Sequential(conv_dw(128, 128, 1), conv_dw(128, 256, 2))                          # 60,60,256
         self.encoder4 = nn.Sequential(conv_dw(256, 256, 1), conv_dw(256, 512, 2))                          # 30,30,512
         self.encoder5 = nn.Sequential(conv_dw(512, 512, 1), conv_dw(512, 512, 1), conv_dw(512, 512, 1),
                                       conv_dw(512, 512, 1), conv_dw(512, 512, 1), conv_dw(512, 1024, 2),
                                       conv_dw(1024, 1024, 1))                                              # 15,15,1024
```

### Comparing `pyzjr-1.3.8/pyzjr/Models/segmentation/unet.py` & `pyzjr-1.3.9/pyzjr/Models/segmentation/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,21 @@
             nn.BatchNorm2d(mid_channels),
             nn.ReLU(inplace=True),
             nn.Conv2d(mid_channels, out_channels, kernel_size=3, padding=1, bias=False),
             nn.BatchNorm2d(out_channels),
             nn.ReLU(inplace=True)
         )
 
-
 class Down(nn.Sequential):
     def __init__(self, in_channels, out_channels):
         super(Down, self).__init__(
             nn.MaxPool2d(2, stride=2),
             DoubleConv(in_channels, out_channels)
         )
 
-
 class Up(nn.Module):
     def __init__(self, in_channels, out_channels, bilinear=True):
         super(Up, self).__init__()
         if bilinear:
             self.up = nn.Upsample(scale_factor=2, mode='bilinear', align_corners=True)
             self.conv = DoubleConv(in_channels, out_channels, in_channels // 2)
         else:
@@ -44,22 +42,20 @@
         x1 = F.pad(x1, [diff_x // 2, diff_x - diff_x // 2,
                         diff_y // 2, diff_y - diff_y // 2])
 
         x = torch.cat([x2, x1], dim=1)
         x = self.conv(x)
         return x
 
-
 class OutConv(nn.Sequential):
     def __init__(self, in_channels, num_classes):
         super(OutConv, self).__init__(
             nn.Conv2d(in_channels, num_classes, kernel_size=1)
         )
 
-
 class UNet(nn.Module):
     def __init__(self, in_channels=1, num_classes=2, bilinear=True, base_c=64):
         super(UNet, self).__init__()
         self.in_channels = in_channels
         self.num_classes = num_classes
         self.bilinear = bilinear
```

### Comparing `pyzjr-1.3.8/pyzjr/PIC.py` & `pyzjr-1.3.9/models_img/test_crack_measure/pixel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,218 @@
+import numpy as np
 import cv2
-from pylab import *
-import pyzjr.Z as Z
-from pyzjr.Math import *
-from skimage.morphology import disk
-from skimage.filters import rank
-from skimage import measure
-from torchvision import transforms
-
-
-def getContours(img, cThr=(100, 100), minArea=1000, filter=0, draw=True):
-    """
-    :param img: 输入图像
-    :param cThr: 阈值
-    :param minArea: 更改大小
-    :param filter: 过滤
-    :param draw: 绘制边缘
-    :return: 返回图像轮廓
-    """
-    imgGray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-    imgBlur = cv2.GaussianBlur(imgGray, (5, 5), 1)
-    imgCanny = cv2.Canny(imgBlur, cThr[0], cThr[1])
-    kernel = np.ones((5, 5))
-    imgDial = cv2.dilate(imgCanny, kernel, iterations=3)
-    imgThre = cv2.erode(imgDial, kernel, iterations=2)
-    contours, _ = cv2.findContours(imgThre, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-    finalCountours = []
-    for i in contours:
-        area = cv2.contourArea(i)
-        if area > minArea:
-            peri = cv2.arcLength(i, True)
-            approx = cv2.approxPolyDP(i, 0.02 * peri, True)
-            bbox = cv2.boundingRect(approx)
-            if filter > 0:
-                if len(approx) == filter:
-                    finalCountours.append([len(approx), area, approx, bbox, i])
-            else:
-                finalCountours.append([len(approx), area, approx, bbox, i])
-    finalCountours = sorted(finalCountours, key=lambda x: x[1], reverse=True)
-    if draw:
-        for con in finalCountours:
-            cv2.drawContours(img, con[4], -1, (0, 0, 255), 3)
-    return img, finalCountours
-
-
-def labelpoint(im, click=4):
-    """
-    交互式标注
-    :param im: 图像,采用im = Image.open(?)的方式打开，颜色空间才是正常的
-    :param click: 点击次数、默认为4
-    :return: 返回点的坐标
-    """
-    imshow(im)
-    print(f'please click {click} points')
-    x = ginput(click)
-    print('you clicked:',x)
-    return x
-
-
-def transImg(img, targetWH):
-    """
-    标注方式按照先上后下，先左后右的顺序
-    :param img: 图像
-    :param targetWH: 已知目标物体的宽度,长度
-    :return: 修正后的图像
-    """
-    width, height = targetWH
-    pts1 = np.float32(labelpoint(img))
-    pts2 = np.float32([[0, 0], [width, 0], [0, height], [width, height]])
-    matrix = cv2.getPerspectiveTransform(pts1, pts2)
-    imgOutput = cv2.warpPerspective(img, matrix, (width, height))
-    return imgOutput
-
-
-def BinaryImg(img, min_value=127, max_value=255):
-    """
-    将OpenCV读取的图像转换为二值图像
-    :param img: 输入的图像,必须是OpenCV读取的图像对象(BGR格式)
-    :param min_value: 最小阈值
-    :param max_value: 最大阈值
-    :return: 转换后的二值图像
+import string
+from skimage.filters import threshold_otsu
+from skimage.morphology import skeletonize
+from skimage import morphology, measure
+from skimage.morphology import medial_axis
+
+def is_bool(param):
+    return param.dtype == np.bool_
+
+def bool2mask(matrix):
+    """
+    Convert Boolean matrix to 8-bit unsigned integer mask image
+    """
+    if is_bool(matrix):
+        result_int = matrix.astype(int)
+        _mask = result_int * 255
+        return _mask.astype(np.uint8)
+    else:
+        raise ValueError("Input matrix must be of bool dtype.")
+
+def medial_axis_mask(image):
     """
-    gray_image = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+    The input must be a binary graph to obtain the axis image within it
+    """
+    result = medial_axis(image)
+    return bool2mask(result)
+
+def BinaryImg(image, min_value=127, max_value=255):
+    """
+    Convert image to binary image
+    :param image: Original image. --- (BGR format)
+    :param min_value: Minimum threshold, default to 127
+    :param max_value: Maximum threshold, default to 225
+    """
+    gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     _, binary_image = cv2.threshold(gray_image, min_value, max_value, cv2.THRESH_BINARY)
     return binary_image
 
+def count_nonzero(thresh):
+    """计算矩阵非0值"""
+    nonzero_pixels = np.count_nonzero(thresh)
+    return nonzero_pixels
+
+def putBoxText(background_image, bbox, text, mode=1, rect=False, bboxcolor=(0, 255, 0), textcolor=(0, 0, 255),
+               fontsize=1, thickness=2, bboxthickness=2,font=cv2.FONT_HERSHEY_SIMPLEX):
+    """
+    在给定的背景图像上绘制一个框，并在框的中心位置添加文本。获取文本的text_size，使文本居中。
+
+    :param background_image: 背景图像，要在其上绘制框和文本的图像
+    :param bbox: 框的边界框，表示为 [x1, y1, x2, y2]
+    :param text: 要添加到框中心的文本
+    :param mode: 模式0 表示框的中心位置，1 表示框的左上角
+    :param rect: 是否绘制角标记框，导入的为 cornerRect 函数
+    :param bboxcolor: 框的颜色，以 BGR 格式表示，例如 (0, 255, 0) 表示绿色
+    :param textcolor: 文本的颜色，以 BGR 格式表示，例如 (0, 0, 255) 表示红色
+    :param fontsize: 文本的字体大小
+    :param thickness: 文本的线宽
+    :param bboxthickness: 框的线宽，默认为 2
+    :return: 绘制了框和文本的图像
+    """
+    text_x = text_y = None
+    x1, y1, x2, y2 = bbox
+    text_size, _ = cv2.getTextSize(text, font, fontsize, thickness)
+    if rect:
+        pass
+    else:
+        cv2.rectangle(background_image, (x1, y1), (x2, y2), bboxcolor, bboxthickness)
+    if mode == 0:
+        text_x = int((x1 + x2) / 2 - text_size[0] / 2)
+        text_y = int((y1 + y2) / 2 + text_size[1] / 2)
+    elif mode == 1:
+        text_x = int(x1)
+        text_y = int(y1 - text_size[1])
+    cv2.putText(background_image, text, (text_x, text_y), font, fontsize, textcolor, thickness)
 
-def SearchOutline(img):
+def SearchOutline(binary_image):
     """
     在给定图像中搜索轮廓并返回轮廓的坐标列表。
-    :param img: 要搜索轮廓的图像。
+    :param binary_image: 要搜索轮廓的图像。
     :return: 包含轮廓坐标的列表，每个坐标表示裂缝的一个点，坐标格式为 [(x, y),...]。
     """
-    binary_image = BinaryImg(img)
     contours = measure.find_contours(binary_image, level=128, fully_connected='low', positive_orientation='low')
-    contour_coordinates = []
-    for contour in contours:
-        contour_coordinates.extend([(int(coord[1]), int(coord[0])) for coord in contour])
-    return contour_coordinates
-
-
-def imtensor(image, dim=0):
-    """转化为tensor格式
-    image1 = Image.open(path).convert('L')
-    image2 = pz.imtensor(image1)
-    """
-    preprocess = transforms.ToTensor()
-    image_tensor = preprocess(image).unsqueeze(dim=dim)
-    return image_tensor
-
-def torch2pillow(input_tensor, dim=0):
-    """将tensor再转化为PIL"""
-    output_image = transforms.ToPILImage()(input_tensor.squeeze(dim=dim))
-    return output_image
-
-def addnoisy(image, n=10000):
-    """
-    :param image: 原始图像
-    :param n: 添加椒盐的次数,默认为10000
-    :return: 返回被椒盐处理后的图像
-    """
-    result = image.copy()
-    w, h = image.shape[:2]
-    for i in range(n):
-        x = np.random.randint(0, w)
-        y = np.random.randint(0, h)
-        if np.random.randint(0, 2) == 0:
-            result[x, y] = 0
-        else:
-            result[x, y] = 255
-    return result
-
-def RectMask(image,mask,boxes):
-    """
-    创建矩形蒙版
-    :param image: 原始图像。
-    :param mask: np.zeros(image.shape, dtype=np.uint8) 背景图
-    :param boxes: [x1, y1, x2, y2]
-    :return: 蒙版与应用蒙版
-    """
-    for box in boxes:
-        x1, y1, x2, y2 = box
-        mask[y1:y2, x1:x2] = 255
-    if mask.ndim == 3 and mask.shape[-1] > 1:
-        mask = mask[:, :, 0]
-    masked_image = cv2.bitwise_and(image, image, mask=mask)
-    return mask, masked_image
-
-
-def drawOutline(blackbackground,contours,mode=0,color=Z.green):
-    """
-    绘制边缘轮廓
-    :param blackbackground: 背景图
-    :param contours: [(x,y),...]
-    :param mode: 默认模式0,可选模式0或1
-    :param color: 默认绿色
-    :return: 
-    """
-    def _sort(imglist):
-        return sorted(imglist, key=lambda item: item[1])
-    if mode == 0:
-        contours = _sort(contours)
-        contour = [np.array([point], dtype=np.int32) for point in contours]
-        cv2.drawContours(blackbackground, contour, -1, color, thickness=-1)
-    elif mode==1:
-        for i in range(len(contours) - 1):
-            start = contours[i]
-            end = contours[i + 1]
-            cv2.line(blackbackground, start, end, color=color, thickness=1)
-
-
-def gradientOutline(img, radius=2):
-    """
-    对图像进行梯度边缘检测，并返回边缘强度图像。
-    
-    :param img: 输入的图像(内部有二值转化)
-    :param radius: 半径,默认为2。
-    :return: 返回经过梯度边缘检测处理后的边缘强度图像
-    """
-    image = BinaryImg(img)
-    denoised = rank.median(image, disk(radius))
-    gradient = rank.gradient(denoised, disk(radius))
-    gradient = cv2.cvtColor(gradient, cv2.COLOR_GRAY2BGR)
+    contours_xy = [np.fliplr(np.vstack(contour)).astype(np.int32) for contour in contours]
+    return contours_xy
+
+def is_gray_image(image):
+    return (len(image.shape) == 2) or (len(image.shape) == 3 and image.shape[-1] == 1)
+
+def drawOutline(blackbackground, contours, color=(255, 0, 255)):
+    cv2.drawContours(blackbackground, contours, -1, color, thickness=1)
 
-    return gradient
+
+def SkeletonMap(target):
+    """
+    获取骨架图的信息
+    :param target: 目标图
+    :return: 骨架图与一个数组，其中每一行表示一个非零元素的索引(y,x)，包括行索引和列索引
+    """
+    if target.ndim == 2 or target.shape[2] == 1:
+        gray = target
+    else:
+        gray = cv2.cvtColor(target, cv2.COLOR_RGB2GRAY)
+    thresh = threshold_otsu(target)
+    binary = gray > thresh
+    skimage = skeletonize(binary)
+    skepoints = np.argwhere(skimage)
+    skimage = skimage.astype(np.uint8)
+    return skimage, skepoints
+
+
+def incircle(img, contours_arr, color=(0, 0, 255)):
+    """
+    轮廓最大内切圆算法,所有轮廓当中的内切圆
+    :param img: 单通道图像
+    :param contours_arr: ndarry的轮廓, 建议使用cv2.findContours,
+                        contours_arr, hierarchy = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_NONE)
+                        pyzjr也有SearchOutline可用,但要转换成ndarry的格式
+    :example:
+        contour = [np.array([point], dtype=np.int32) for point in contours]
+        # 平铺的方法
+        flatten_contours = np.concatenate([cnt.flatten() for cnt in contours_arr])
+        flatten_contours = flatten_contours.reshape(-1, 2)
+    :param color: 绘制内切圆颜色
+    :return: 绘制在原图的内切圆,内切圆直径,绘制出的图像与轮廓直接差距一个像素，是因为cv2.circle的半径参数必须为int类型
+    """
+    if is_gray_image:
+        result = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+    raw_dist = np.zeros(img.shape, dtype=np.float32)
+    letters = list(string.ascii_uppercase)
+    label = {}
+    k = 0
+    for contours in contours_arr:
+        for i in range(img.shape[0]):
+            for j in range(img.shape[1]):
+                raw_dist[i, j] = cv2.pointPolygonTest(contours, (j, i), True)
+        min_val, max_val, _, max_dist_pt = cv2.minMaxLoc(raw_dist)
+        if max_val > .5:
+            label[letters[k]] = max_val * 2
+            k += 1
+        cv2.circle(result, max_dist_pt, int(max_val), color, 1, 1, 0)
+
+    return result, label
+
+
+def outcircle(img, contours_arr, color=(0, 255, 0)):
+    """
+    轮廓外切圆算法,画出所有轮廓的外切圆
+    :param img: 单通道图像
+    :param contours_arr: ndarry的轮廓, 建议使用cv2.findContours,
+                        contours_arr, hierarchy = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_NONE)
+                        pyzjr也有SearchOutline可用,但要转换成ndarry的格式
+    :example:
+        contour = [np.array([point], dtype=np.int32) for point in contours]
+    :param color: 绘制外切圆颜色
+    :return:
+    """
+    radii = []
+    result = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+    for k, cnt in enumerate(contours_arr):
+        (x, y), radius = cv2.minEnclosingCircle(cnt)
+        radii.append([(x,y),radius])
+        center = (int(x), int(y))
+        radius = int(radius)
+        cv2.circle(result, center, radius, color, 1)
+        cv2.circle(result, center, 1, color, 1)
+
+    return result, radii
+
+def foreground_contour_length(binary_img, minArea=30):
+    """
+    计算前景的轮廓长度, 返回两个值, 每个轮廓的长度和总长度
+    :param binary_img: 二值图
+    :param minArea: 最小过滤面积
+    """
+    contours_xy = SearchOutline(binary_img)
+    contour_lengths = []
+    for contour in contours_xy:
+        area = cv2.contourArea(contour)
+        if area > minArea:
+            length = cv2.arcLength(contour, False)
+            contour_lengths.append(length)
+    all_length = np.sum(contour_lengths)
+    return contour_lengths, all_length
+
+
+def each_crack_areas(mask, thresh, merge_threshold=3, area_threshold=50):
+    """每条裂缝的面积,并用大写字母来进行标记"""
+    connected_image = morphology.closing(thresh, morphology.disk(merge_threshold))
+    labeled_image = measure.label(connected_image, connectivity=2)
+    region_props = measure.regionprops(labeled_image)
+    area = {}
+    Bboxing = []
+    crack_label = ord('A')
+    for region in region_props:
+        area_value = region.area
+        if area_value >= area_threshold:
+            minr, minc, maxr, maxc = region.bbox
+            Bboxing.append([(minc, minr), (maxc, maxr)])
+            putBoxText(mask, [minc, minr, maxc, maxr], chr(crack_label), mode=0, fontsize=.5)
+            if crack_label <= ord('Z'):
+                area[chr(crack_label)] = area_value
+                crack_label += 1
+    return area, Bboxing, mask
+
+if __name__=="__main__":
+    from pyzjr.augmentation.mask_ops import BinaryImg
+    from pyzjr.measure.crack.skeleton_extraction import skeletoncv
+    path = r'/models_img/1604.png'
+    cv_image = cv2.imread(path)
+    image = skeletoncv(path)
+    # image = BinaryImg(cv_image)
+    contour_lengths, all_length = foreground_contour_length(image)
+
+    print(all_length)
+    for i, length in enumerate(contour_lengths):
+        print(f"Contour {i} length: {length}")
```

### Comparing `pyzjr-1.3.8/pyzjr/Z.py` & `pyzjr-1.3.9/pyzjr/Z.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 GRAY2BGR = 8
 GRAY2RGB = 8
 HSV2BGR = 54
 HSV2RGB = 55
 RGB2HSV = 41
 RGB2BGR = 4
 
-repair_NS = 0
-repair_TELEA = 1
 Lap_64F = 6
 # video
 Esc = 27
 # BGR
 blue = (255, 0, 0)
 green = (0, 255, 0)
 red = (0, 0, 255)
```

### Comparing `pyzjr-1.3.8/pyzjr/__init__.py` & `pyzjr-1.3.9/pyzjr/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 - WeChat: z15583909992
 - Email: zjricetea@gmail.com / 2165648225@qq.com
 - Note: Currently still being updated, please refer to the latest version for any changes that may occur
 
     https://www.pepy.tech/projects/pyzjr
     API documentation website:
 """
-from pyzjr.visualize.utils import *
 
-from pyzjr.Z import * 
+from pyzjr.Z import *
+from pyzjr.version import __version__
+
 from pyzjr.Math import *
-from pyzjr.PIC import *
 from pyzjr.data import *
 from pyzjr.devices import *
 
 from pyzjr.augmentation import *
 from pyzjr.dlearn import *
 from pyzjr.core import *
-from pyzjr.version import __version__
 from pyzjr.visualize import *
+from pyzjr.measure import *
 
 from pyzjr.nn import *
 from pyzjr.Models import *
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/Pixel/Crack.py` & `pyzjr-1.3.9/models_img/Crack.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 
 import string
 import os
 from skimage.filters import threshold_otsu, median
 from skimage.morphology import skeletonize, dilation, disk
 from skimage import io, morphology, measure
 
-from pyzjr.augmentation.Pixel import SkeletonMap, incircle
+from pyzjr.measure.pixel import SkeletonMap, incircle
 from pyzjr.visualize.color import putBoxText
 
-
 # 裂缝类型
 class CrackType():
     """直方图投影法推断裂缝类型,仅仅能区分线性裂缝和网状裂缝"""
     def __init__(self, threshold=3, HWratio=10, Histratio=0.5):
         """
         初始化分类裂缝的参数
         :param threshold: 阈值，用于分类裂缝的阈值
@@ -224,17 +223,17 @@
         kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
         binary = cv2.dilate(binary, kernel, iterations=1)
         binary = cv2.medianBlur(binary, 5)
         binary = cv2.dilate(binary, kernel, iterations=1)
         binary = cv2.medianBlur(binary, 5)
         kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
         binary = cv2.morphologyEx(binary, cv2.MORPH_CLOSE, kernel)
-        binary=cv2.cvtColor(binary,cv2.COLOR_BGR2RGB)
+        binary = cv2.cvtColor(binary,cv2.COLOR_BGR2RGB)
         skeleton = skeletonize(binary)
-        skeleton=cv2.cvtColor(skeleton,cv2.COLOR_RGB2BGR)
+        skeleton = cv2.cvtColor(skeleton,cv2.COLOR_RGB2BGR)
         return skeleton
 
     def sketionio(self,single_pic):
         image = io.imread(single_pic, as_gray=True)
         thresh = threshold_otsu(image)
         binary = image > thresh
 
@@ -252,15 +251,15 @@
     def sketions(self, input_folder='num', output_folder='output'):
         if not os.path.exists(output_folder):
             os.makedirs(output_folder)  # 如果输出文件夹不存在，就创建它
         for filename in os.listdir(input_folder):
             if filename.endswith('.jpg') or filename.endswith('.png'):
                 input_file=os.path.join(input_folder, filename)
                 output_filename = os.path.join(output_folder, filename)
-                skeleton=self.sketionio(input_file)
+                skeleton = self.sketionio(input_file)
                 io.imsave(output_filename, skeleton)
         return output_folder
 
 def DetectCracks(mask, skeimg, mode, merge_threshold=3, area_threshold=50, showcrackinformation=True):
     crack_area = Crack_areas_and_numbers(mask)
     cracktype = infertype(mask)
     if cracktype == "Mesh":
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/Pixel/_Steger.py` & `pyzjr-1.3.9/pyzjr/measure/steger.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 All rights reserved.
 
 This module is used to extract the laser centerline using the steger algorithm
 """
 import numpy as np
 import cv2
 
-__all__ = ["Steger", "threshold"]
-
 def _derivation_with_Filter(Gaussimg):
-    dx = cv2.filter2D(Gaussimg,-1, kernel=np.array([[1], [0], [-1]]))
-    dy = cv2.filter2D(Gaussimg,-1, kernel=np.array([[1, 0, -1]]))
-    dxx = cv2.filter2D(Gaussimg,-1, kernel=np.array([[1], [-2], [1]]))
-    dyy = cv2.filter2D(Gaussimg,-1, kernel=np.array([[1, -2, 1]]))
-    dxy = cv2.filter2D(Gaussimg,-1, kernel=np.array([[1, -1], [-1, 1]]))
+    dx = cv2.filter2D(Gaussimg, -1, kernel=np.array([[1], [0], [-1]]))
+    dy = cv2.filter2D(Gaussimg, -1, kernel=np.array([[1, 0, -1]]))
+    dxx = cv2.filter2D(Gaussimg, -1, kernel=np.array([[1], [-2], [1]]))
+    dyy = cv2.filter2D(Gaussimg, -1, kernel=np.array([[1, -2, 1]]))
+    dxy = cv2.filter2D(Gaussimg, -1, kernel=np.array([[1, -1], [-1, 1]]))
 
     return dx, dy, dxx, dyy, dxy
 
 def _derivation_with_Scharr(Gaussimg):
     dx = cv2.Scharr(Gaussimg, cv2.CV_32F, 1, 0)
     dy = cv2.Scharr(Gaussimg, cv2.CV_32F, 0, 1)
     dxx = cv2.Scharr(dx, cv2.CV_32F, 1, 0)
@@ -148,36 +146,17 @@
                         if np.abs(T*nx) <= threshold and np.abs(T*ny) <= threshold:
                             point.append((x,y))
                             direction.append((nx,ny))
                             value.append(np.abs(dxy[y,x]+dxy[y,x]))
         return point, direction, value
 
 
-def threshold(mask, std=127.5):
-    """阈值法"""
-    mask[mask > std] = 255
-    mask[mask < std] = 0
-    return mask.astype("uint8")
-
-def test_Steger():
-    img = cv2.imread(r"D:\PythonProject\net\line\data\Image_20230215160728679.jpg")
-
-    gray_img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-    gray_img = threshold(gray_img)
-    steger = Steger(gray_img)
-    img,newimage=steger.centerline(img,sigmaX=1.1,sigmaY=1.1,method="Sobel")
-    # point, direction, value = HessianMatrix(gray_img, 1.1, 1.1, usenonmax=True)
-
-
-    cv2.imwrite("result/main3.png", newimage)
-    cv2.imwrite("result/main3_img.png", img)
 
 
-
-def test_derivation_methods_time():
+if __name__=="__main__":
     from pyzjr.dlearn import Runcodes
     img = cv2.imread(r"D:\PythonProject\net\line\data\Image_20230215160728411.jpg")
     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
     gray_img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
     with Runcodes(description="Filter"):
         print(derivation(gray_img,1.1,1.1,"Filter"))
         # Filter: 0.01344 sec
@@ -187,11 +166,18 @@
         # Scharr: 0.00959 sec
 
     with Runcodes(description="Sobel"):
         print(derivation(gray_img, 1.1, 1.1,"Sobel"))
         # Sobel: 0.01820 sec
 
 
+    def test_Steger():
+        img = cv2.imread(r"D:\PythonProject\net\line\data\Image_20230215160728679.jpg")
 
-if __name__=="__main__":
-    # test_derivation_methods_time()
-    test_Steger()
+        gray_img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        steger = Steger(gray_img)
+        img,newimage=steger.centerline(img, sigmaX=1.1,sigmaY=1.1,method="Sobel")
+        # point, direction, value = HessianMatrix(gray_img, 1.1, 1.1, usenonmax=True)
+
+
+        cv2.imwrite("result/main3.png", newimage)
+        cv2.imwrite("result/main3_img.png", img)
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/Pixel/definition.py` & `pyzjr-1.3.9/pyzjr/augmentation/mask_ops.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,232 +1,266 @@
-"""
-Copyright (c) 2023, Auorui.
-All rights reserved.
-
-This module is used to implement clarity evaluation algorithms.
-"""
 import cv2
-import math
 import numpy as np
-import scipy.ndimage as ndi
-from skimage.filters import sobel
-
-import pyzjr.Z as Z
-from pyzjr.data.reader import getPhotopath
+from PIL import Image
+from pyzjr.core.general import is_numpy, is_bool
+from skimage.morphology import medial_axis
+from scipy.ndimage import distance_transform_edt
+
+def convert_np(image, dtype=np.uint8):
+    """Convert an image to a NumPy array with the specified dtype."""
+    return image if is_numpy(image) else np.array(image).astype(dtype)
 
-__all__ = ["ImgDefinition", "Fuzzy_image", "vagueJudge",]
+def clip(image, maxval, dtype=np.uint8):
+    """
+    Truncate the pixel values of the image to the specified range and perform data type conversion
+    """
+    np_image = convert_np(image)
+    return np.clip(np_image, 0, maxval).astype(dtype)
 
-class ImgDefinition():
-    """
-    清晰度评价函数: https://blog.csdn.net/m0_62919535/article/details/127818006
-    Laplacian与Gradientmetric最靠谱
-    """
-    def Brenner(self, img):
-        '''
-        Brenner梯度函数
-        :param img:narray 二维灰度图像
-        :return: int 图像越清晰越大
-        '''
-        shapes = np.shape(img)
-        output = 0
-        for x in range(0, shapes[0] - 2):
-            for y in range(0, shapes[1]):
-                output += (int(img[x + 2, y]) - int(img[x, y])) ** 2
-        return output
-
-    def EOG(self, img):
-        '''
-        能量梯度函数(Energy of Gradient)
-        :param img:narray 二维灰度图像
-        :return: int 图像越清晰越大
-        '''
-        shapes = np.shape(img)
-        output = 0
-        for x in range(0, shapes[0] - 1):
-            for y in range(0, shapes[1] - 1):
-                output += ((int(img[x + 1, y]) - int(img[x, y])) ** 2 + (int(img[x, y + 1]) - int(img[x, y])) ** 2)
-        return output
-
-    def Roberts(self,img):
-        '''
-        Roberts函数
-        :param img:narray 二维灰度图像
-        :return: int 图像越清晰越大
-        '''
-        shapes = np.shape(img)
-        output = 0
-        for x in range(0, shapes[0] - 1):
-            for y in range(0, shapes[1] - 1):
-                output += ((int(img[x + 1, y + 1]) - int(img[x, y])) ** 2 + (
-                        int(img[x + 1, y]) - int(img[x, y + 1])) ** 2)
-        return output
-
-    def Laplacian(self,img):
-        '''
-        Laplace
-        :param img:narray 二维灰度图像
-        :return: int 图像越清晰越大
-        '''
-        return cv2.Laplacian(img, Z.Lap_64F).var()
-
-    def SMD(self,img):
-        '''
-        SMD(灰度方差)函数
-        :param img:narray 二维灰度图像
-        :return: int 图像越清晰越大
-        '''
-        shape = np.shape(img)
-        output = 0
-        for x in range(1, shape[0] - 1):
-            for y in range(0, shape[1]):
-                output += math.fabs(int(img[x, y]) - int(img[x, y - 1]))
-                output += math.fabs(int(img[x, y] - int(img[x + 1, y])))
-        return output
-
-    def SMD2(self,img):
-        '''
-        （灰度方差乘积）函数
-        :param img:narray 二维灰度图像
-        :return: int 图像约清晰越大
-        '''
-        shape = np.shape(img)
-        output = 0
-        for x in range(0, shape[0] - 1):
-            for y in range(0, shape[1] - 1):
-                output += math.fabs(int(img[x, y]) - int(img[x + 1, y])) * math.fabs(
-                    int(img[x, y] - int(img[x, y + 1])))
-        return output
-
-    def Gradientmetric(self,img, size=11):
-        """
-        计算指示图像中模糊强度的度量(0表示无模糊, 1表示最大模糊)
-        但实际上还是要根据我们的标准图与模糊图得到模糊区间
-        :param img: 单通道进行处理,灰度图
-        :param size: 重新模糊过滤器的大小
-        :return: float,唯一不是值越大,越清晰的算法
-        """
-        image = np.array(img, dtype=np.float32) / 255
-        n_axes = image.ndim
-        shape = image.shape
-        blur_metric = []
-
-        slices = tuple([slice(2, s - 1) for s in shape])
-        for ax in range(n_axes):
-            filt_im = ndi.uniform_filter1d(image, size, axis=ax)
-            im_sharp = np.abs(sobel(image, axis=ax))
-            im_blur = np.abs(sobel(filt_im, axis=ax))
-            T = np.maximum(0, im_sharp - im_blur)
-            M1 = np.sum(im_sharp[slices])
-            M2 = np.sum(T[slices])
-            blur_metric.append(np.abs((M1 - M2)) / M1)
-
-        return np.max(blur_metric) if len(blur_metric) > 0 else 0.0
-
-    def get_method(self, mode):
-        methods = {
-            "B": self.Brenner,
-            "E": self.EOG,
-            "R": self.Roberts,
-            "L": self.Laplacian,
-            "S": self.SMD,
-            "S2": self.SMD2,
-            "G": self.Gradientmetric,
-        }
-        return methods.get(mode, None)
-
-def definemode(img, mode):
-    ti = ImgDefinition()
-    method = ti.get_method(mode)
+def unique(image):
+    """Returns a list of unique pixel values in the input image"""
+    np_image = convert_np(image)
+    return np.unique(np_image)
 
-    if method is not None:
-        return method(img)
+def RectMask(image, up_left_coord=None, lower_right_coord=None, bboxes=None):
+    """
+    Create a rectangular mask
+    :param image: Original image.
+    :param up_left_coord: [x1, y1]
+    :param lower_right_coord: [x2, y2]
+    :param bboxes: [x1, y1, x2, y2]
+    """
+    image = convert_np(image)
+    h, w = image.shape[:2]
+    mask = np.zeros((h, w, 3), dtype=np.uint8)
+    if bboxes is None:
+        x1, y1 = up_left_coord
+        x2, y2 = lower_right_coord
     else:
-        raise ValueError(f"[pyzjr]:Invalid mode: {mode}")
+        x1, y1, x2, y2 = bboxes
+    mask[y1: y2, x1: x2] = 255
 
-class Fuzzy_image():
-    def __init__(self, mode="L"):
-        """
-        模糊判定区间: https://blog.csdn.net/m0_62919535/article/details/128061017
-        :param mode: 图像清晰度算法模式,建议采用“L”或“G”算法
-        """
-        self.mode=mode
-    def getImgVar(self, image):
-        """
-        :param image: 图像
-        :return: 图片清晰度数值
-        """
-        imggray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-        imageVar = definemode(imggray,mode=self.mode)
-        return abs(imageVar)
-
-    def getReorder(self, imgfile, reverse = False):
-        """
-        :param imgfile: getPhotopath()获取图片路径的列表
-        :param reverse: 表示是否进行反转排序(从大到小)
-        :return: 模糊值排序
-        """
-        c = []
-        for i in imgfile:
-            img = cv2.imread(i)
-            image = self.getImgVar(img)
-            c.append(float(f"{image:.3f}"))
-        c.sort(reverse=reverse)
-        return c
-
-    def getInterval(self, pathVague, pathStd):
-        """
-        :param pathVague:模糊图的数据集文件夹位置
-        :param pathStd: 标准图的数据文件夹位置
-        :return: 模糊判定区间
-        """
-        imgfile1, _ = getPhotopath(pathVague,debug=False)
-        imgfile2, _ = getPhotopath(pathStd,debug=False)
-        a = self.getReorder(imgfile1)
-        b = self.getReorder(imgfile2)
-        if self.mode=="G":
-            thr = (b[-1], a[0])
-        else:
-            thr = (a[-1], b[0])
-        return thr
+    if mask.ndim == 3 and mask.shape[-1] > 1:
+        mask = mask[:, :, 0]
+    masked_image = cv2.bitwise_and(image, image, mask=mask)
+    return mask, masked_image
 
-def vagueJudge(img, pathVague, pathStd, mode="L", show_minandmax=True):
+def BinaryImg(image, min_value=127, max_value=255):
     """
-    :param img: 图片
-    :param show_minandmax:是否输出模糊未知区间
-    :return: 模糊数值打印在图片上显示,只要没有超过清晰图像的阈值，全部判断为模糊
-    """
-    Fuzzy = Fuzzy_image(mode)
-    imgVar = Fuzzy.getImgVar(img)
-    minThr, maxThr = Fuzzy.getInterval(pathVague=pathVague, pathStd=pathStd)
-    img2 = img.copy()
-    if imgVar > maxThr:
-        if mode == "G":
-            text = "Vague"
-            color = Z.red
-        else:
-            text = "Not Vague"
-            color = Z.blue
+    Convert image to binary image
+    :param image: Original image. --- (BGR format)
+    :param min_value: Minimum threshold, default to 127
+    :param max_value: Maximum threshold, default to 225
+    """
+    np_image = convert_np(image)
+    gray_image = cv2.cvtColor(np_image, cv2.COLOR_BGR2GRAY)
+    _, binary_image = cv2.threshold(gray_image, min_value, max_value, cv2.THRESH_BINARY)
+    return binary_image
+
+def up_low(image, lower, upper, dtype=np.uint8):
+    """
+    Create a binarized mask based on the given color range (lower and upper limits)
+    :param lower: Lower limit of color range, (B, G, R)
+    :param upper: Upper limit of color range, (B, G, R)
+    """
+    np_image = convert_np(image)
+    lower = np.array(lower, dtype=dtype)
+    upper = np.array(upper, dtype=dtype)
+    _mask = cv2.inRange(np_image, lower, upper)
+    return _mask
+
+def approximate(image, std=127.5, dtype=np.uint8):
+    """
+    Convert a single channel image into a binary image.
+    """
+    image[image > std] = 255
+    image[image < std] = 0
+    image = image.astype(dtype)
+    return image
+
+def ceilfloor(image, dtype=np.uint8):
+    """
+    The pixel value of the input image is limited between the maximum value of 255 and the minimum value of 0
+    """
+    image[image > 255] = 255
+    image[image < 0] = 0
+    image = image.astype(dtype)
+    return image
+
+def bool2mask(matrix):
+    """
+    Convert Boolean matrix to 8-bit unsigned integer mask image
+    """
+    if is_bool(matrix):
+        result_int = matrix.astype(int)
+        _mask = result_int * 255
+        return _mask.astype(np.uint8)
     else:
-        if mode == "G":
-            text = "Not Vague"
-            color = Z.blue
+        raise ValueError("Input matrix must be of bool dtype.")
+
+def cv_distance(image):
+    """Using distance transformation functions in OpenCV"""
+    dist_transform = cv2.distanceTransform(image, cv2.DIST_L2, 3)
+    return dist_transform
+
+def chamfer(image, weight=None):
+    """Chamfer distance transformation"""
+    if weight is None:
+        weights = np.array([[1, 1, 1],
+                            [1, 0, 1],
+                            [1, 1, 1]], dtype=np.uint8)
+    else:
+        weights = weight
+    dist_transform = cv2.filter2D(image, cv2.CV_32F, weights)
+    return dist_transform
+
+def fast_marching(image):
+    """Fast-Marching Distance Transform"""
+    _, medial_axis_image = medial_axis(image, return_distance=True)   # 使用medial_axis函数计算中轴线
+    dist_transform = distance_transform_edt(medial_axis_image)
+    return dist_transform
+
+def addnoisy(image, n=10000):
+    """
+    Add salt and pepper treatment
+    """
+    result = image.copy()
+    w, h = image.shape[:2]
+    for i in range(n):
+        x = np.random.randint(0, w)
+        y = np.random.randint(0, h)
+        if np.random.randint(0, 2) == 0:
+            result[x, y] = 0
         else:
-            text = "Vague"
-            color = Z.red
+            result[x, y] = 255
+    return result
 
-    cv2.putText(img2, f"{text}{imgVar:.2f}", (12, 70), cv2.FONT_HERSHEY_PLAIN, 3, color, 3)
+def inpaint_defect(image, mask, radius=10, flags=1):
+    """
+    Inpaint defect image
+    :param image: defect image
+    :param mask: Mask of defective parts
+    :param radius: Inpaint radius
+    :param flags: TELEA-1; NS-0
+    """
+    dst = cv2.inpaint(image, mask, radius, flags)
+    return dst
 
-    if show_minandmax:
-        print(minThr, maxThr)
+def medial_axis_mask(image):
+    """
+    The input must be a binary graph to obtain the axis image within it
+    """
+    result = medial_axis(image)
+    return bool2mask(result)
+
+def cvt8png(pngpath, bit_depth=False, target=(255, 255, 255), convert=(128, 0, 0)):
+    """
+    Voc: RGB png彩图转换
+    :param bit_depth: 默认转为8位,需要使用out_png.save可以正确保存
+    True:                      False:
+        plt.imshow(img)             cv2.imshow("img",img)
+        plt.axis('off')             cv2.waitKey(0)
+        plt.show()
+    :param pngpath: 为保证是按照cv2的方式读入, 所以传入路径即可
+    :param target: 目标颜色, RGB方式
+    :param convert: 转换颜色, 同RGB格式
+    :return:
+    """
+    png = cv2.imread(pngpath)
+    png = cv2.cvtColor(png, cv2.COLOR_BGR2RGB)
+    h, w = png.shape[:2]
+
+    mask = np.all(png == target, axis=-1)
+    out_png = np.zeros((h, w, 3), dtype=np.uint8)
+    out_png[mask] = convert
+    out_png[~mask] = png[~mask]
+
+    if bit_depth:
+        out_png_pil = Image.fromarray(out_png)
+        out_png_pil = out_png_pil.convert("P", palette=Image.ADAPTIVE, colors=256)
+        return out_png_pil
     else:
-        pass
-    return img2
+        out_png_cv = cv2.cvtColor(out_png, cv2.COLOR_RGB2BGR)
+        return out_png_cv
+
+def cvtMask(pngpath, lower ,upper, convert=(255, 255, 255)):
+    """
+    去除标签中的杂色,并对其进行颜色的转换
+
+    :param pngpath: 输入图像的文件路径
+    :param lower: 颜色范围的下限值，作为一个包含(B, G, R)值的元组
+    :param upper: 颜色范围的上限值，作为一个包含(B, G, R)值的元组
+    :param convert: 需要转换为的颜色，作为一个包含(B, G, R)值的元组
+    :return: 处理后的图像
+    """
+    image = cv2.imread(pngpath)
+    lower = np.array(lower, dtype=np.uint8)
+    upper = np.array(upper, dtype=np.uint8)
+
+    mask = cv2.inRange(image, lower, upper)
+    image[mask > 0] = convert
+
+    return image
+
+def imageContentMove(image, H_pixels=None, V_pixels=None):
+    if H_pixels is None:
+        H_pixels = 0
+    if V_pixels is None:
+        V_pixels = 0
+    h, w = image.shape[:2]
+    black = np.zeros_like(image)
+
+    start_row, end_row = max(0, V_pixels), min(h, h + V_pixels)
+    start_col, end_col = max(0, H_pixels), min(w, w + H_pixels)
+
+    fill_start_row, fill_end_row = max(0, -V_pixels), min(h, h - V_pixels)
+    fill_start_col, fill_end_col = max(0, -H_pixels), min(w, w - H_pixels)
+
+    black[start_row:end_row, start_col:end_col] = image[fill_start_row:fill_end_row, fill_start_col:fill_end_col]
+
+    return black
+
+def count_zero(thresh):
+    """计算矩阵0值"""
+    zero_count = np.sum(thresh == 0)
+    return zero_count
+
+def count_white(thresh):
+    """计算矩阵255值"""
+    white_count = np.sum(thresh == 255)
+    return white_count
+
+def count_nonzero(thresh):
+    """计算矩阵非0值"""
+    nonzero_pixels = np.count_nonzero(thresh)
+    return nonzero_pixels
 
 if __name__=="__main__":
-    path = r"ces\Standards\001.jpg"   # 需要进行测试的图片
-    path2 = r"ces\test\02.jpg"
-    pathVague = r"ces\test"           # 模糊图像数据
-    pathStd = r"ces\Standards"        # 标准图像数据
-    img = cv2.imread(path)
-    test = vagueJudge(img, pathVague, pathStd, mode="G")
-    cv2.imshow("test", test)
-    cv2.waitKey(0)
+    image = np.zeros((10, 10), dtype=np.uint8)
+    image[2:8, 2:8] = 255
+    print(image)
+
+    dist_transform = cv_distance(image)
+    chamfer_dist_transform = chamfer(image)
+    fast_marching_dist_transform = fast_marching(image)
+    # 距离变换结果
+    print("Distance Transform:")
+    print(dist_transform)
+    print("\nChamfer Distance Transform:")
+    print(chamfer_dist_transform)
+    print("\nFast-Marching Distance Transform:")
+    print(fast_marching_dist_transform)
+
+    mask_img_path = r'D:\PythonProject\pyzjrPyPi\models_img\1604.png'
+    mask_img = cv2.imread(mask_img_path)
+    img = clip(mask_img, 255)
+    # img = up_low(img, (0, 0, 100), (255, 255, 255))
+    # img = approximate(img, 130)
+    img = BinaryImg(img)
+    # img = ceilfloor(img)
+    # _, img = RectMask(img, (15, 27), (388, 300))
+    result = medial_axis_mask(img)
+    print(unique(result))
+    # print(result.shape)
+    cv2.imshow("test mask-function", result)
+    cv2.waitKey(0)
+
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/augments.py` & `pyzjr-1.3.9/pyzjr/augmentation/augments.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,32 @@
 
 __all__ = ["base_crop1", "base_crop2", "center_crop", "five_crop", "Stitcher_image",\
 
            "Centerzoom", "flip", "horizontal_flip", "vertical_flip", "resize", "adjust_brightness_cv2", "adjust_brightness_numpy",\
 
            "rotate", "adjust_gamma", "pad", "erase", "augment_Hsv","hist_equalize","random_resize_crop","random_crop",\
 
-           "random_horizontal_flip", "random_vertical_flip", "random_rotation", "random_lighting", "random_apply", "random_order",\
+           "random_horizontal_flip", "random_vertical_flip", "random_rotation", "random_lighting",\
 
-           "random_choice", "uniform_augment",
-
-           "Retinex", "blur", "median_blur", "gaussian_blur", "bilateral_blur", "Filter"]
+           "Retinex"]
 
 def base_crop1(img, x_min, y_min, x_max, y_max):
     height, width = img.shape[:2]
-    assert x_max > x_min, "[pyzjr]:Maximum value of cropping x_max cannot be less than the minimum value x_min"
-    assert y_max > y_min, "[pyzjr]:Maximum value of cropping y_max cannot be less than the minimum value y_min"
-    assert x_min >= 0, "[pyzjr]:x_min cannot be less than 0"
-    assert x_max <= width, "[pyzjr]:x_max cannot be greater than the image width"
-    assert y_min >= 0, "[pyzjr]:y_min cannot be less than 0"
-    assert y_max <= height, "[pyzjr]:y_max cannot be greater than the image height"
+    assert x_max > x_min, "Maximum value of cropping x_max cannot be less than the minimum value x_min"
+    assert y_max > y_min, "Maximum value of cropping y_max cannot be less than the minimum value y_min"
+    assert x_min >= 0, "x_min cannot be less than 0"
+    assert x_max <= width, "x_max cannot be greater than the image width"
+    assert y_min >= 0, "y_min cannot be less than 0"
+    assert y_max <= height, "y_max cannot be greater than the image height"
 
     return img[y_min:y_max, x_min:x_max]
 
 def base_crop2(img, x_start, y_start, width, height):
-    assert width > 0 and height > 0, "[pyzjr]:Width and height of cropping area must be greater than 0"
-    assert x_start >= 0 and y_start >= 0, "[pyzjr]:x_min and y_min cannot be less than 0"
+    assert width > 0 and height > 0, "Width and height of cropping area must be greater than 0"
+    assert x_start >= 0 and y_start >= 0, "x_min and y_min cannot be less than 0"
 
     return img[y_start:y_start+height, x_start:x_start+width]
 
 def center_crop(image, target_size):
     """
     Center-crops an image to the specified target size.
 
@@ -434,82 +432,14 @@
     img_arr[:, :, 0] += pca_b
     img_arr[:, :, 1] += pca_g
     img_arr[:, :, 2] += pca_r
     img_arr = np.uint8(np.minimum(np.maximum(img_arr, 0), 255))
 
     return img_arr
 
-def random_apply(img, transforms:list, prob):
-    """
-    以给定的概率随机应用一个transforms列表
-    Args:
-        img: Image to be randomly applied a list transformations.
-        transforms (list): List of transformations to be applied.
-        prob (float): The probability to apply the transformation list.
-
-    Returns:
-        Transformed image.
-    """
-    if prob < random.random():
-        return img
-    for transform in transforms:
-        img = transform(img)
-    return img
-
-def random_order(img, transforms:list):
-    """
-    以随机顺序应用transforms列表.
-    Args:
-        img: Image to be applied transformations in a random order.
-        transforms (list): List of the transformations to be applied.
-
-    Returns:
-        Transformed image.
-    """
-    random.shuffle(transforms)
-    for transform in transforms:
-        img = transform(img)
-    return img
-
-def random_choice(img, transforms:list):
-    """
-    从transforms列表中随机选择一个变换，并将其应用于图像。
-    Args:
-        img: Image to be applied transformation.
-        transforms (list): List of transformations to be chosen from to apply.
-
-    Returns:
-        Transformed image.
-    """
-    return random.choice(transforms)(img)
-
-def uniform_augment(img, transforms, num_ops):
-    """
-    Uniformly select and apply a number of transforms sequentially from
-    a list of transforms. Randomly assigns a probability to each transform for
-    each image to decide whether apply it or not.
-    All the transforms in transform list must have the same input/output data type.
-
-    Args:
-        img: Image to be applied transformation.
-        transforms (list): List of transformations to be chosen from to apply.
-        num_ops (int): number of transforms to sequentially aaply.
-
-    Returns:
-        Transformed image.
-
-    """
-    op_idx = np.random.choice(len(transforms), size=num_ops, replace=False)
-    for idx in op_idx:
-        augment_op = transforms[idx]
-        pr = random.random()
-        if random.random() < pr:
-            img = augment_op(img.copy())
-    return img
-
 class Retinex():
     """
     增强算法Retinex
     - 单尺度 : SSR
     - 多尺度 : MSR
     - 多尺度自适应增益 : MSRCR
     https://blog.csdn.net/m0_62919535/article/details/130372571
@@ -601,116 +531,7 @@
                 result[:, :, z]=result[:, :, z]*G_ratio
                 img_light[:, :, z] += cv2.resize(img_smooth, (c, r))
 
         img_msrcr = np.exp(result+img_light) - 1
         img_msrcr = np.uint8(cv2.normalize(img_msrcr, None, 0, 255, cv2.NORM_MINMAX))
         return img_msrcr
 
-def blur(img, ksize):
-    """均值滤波 """
-    blur_img = cv2.blur(img, ksize=ksize)
-    return blur_img
-
-def median_blur(img, ksize):
-    """中值滤波"""
-    if img.dtype == np.float32 and ksize not in {3, 5, 7}:
-        raise ValueError(f"Invalid ksize value {ksize}.The available values are 3, 5, and 7")
-    medblur_img = cv2.medianBlur(img, ksize=ksize)
-    return medblur_img
-
-def gaussian_blur(img, ksize):
-    """
-    高斯模糊,提供给不熟悉高斯模糊参数的用户,sigma根据ksize进行自动计算,具体可以参考下面
-    https://docs.opencv.org/master/d4/d13/tutorial_py_filtering.html
-    """
-    sigma = 0.3*((ksize-1)*0.5 - 1) + 0.8
-    gaussianblur_img = cv2.GaussianBlur(img, ksize=(ksize,ksize), sigmaX=sigma)
-    return gaussianblur_img
-
-def bilateral_blur(img, d=5, sigma_color=75, sigma_space=75):
-    """双边滤波"""
-    return cv2.bilateralFilter(img, d, sigma_color, sigma_space)
-
-class Filter():
-    """手写实现,仅供学习参考,最好还是使用cv2
-    https://blog.csdn.net/m0_62919535/category_11936595.html?spm=1001.2014.3001.5482
-    """
-    def median_filtering(self, img,ksize=3):
-        """
-        中值滤波
-        :param img:输入图像
-        :param ksize: 核大小
-        :return: 中值滤波平滑
-        """
-        h, w, c = img.shape
-        half = ksize//2
-        dst = np.zeros((h+2*half,w+2*half,c),np.uint8)
-        dst[half:half+h, half:half+w] = img.copy()
-
-        tmp=dst.copy()
-        for y in range(h):
-            for x in range(w):
-                for z in range(c):
-                    dst[half+x,half+y]=np.median(tmp[x:x+ksize,y:y+ksize])
-        output=dst[half:half+h,half:half+w]
-        return output
-
-    def Arerage_Filtering(self, img, k_size=3):
-        """
-        均值滤波函数,默认会返回灰度图，因为三个for循环实在是太耗费时间了。而且，在这里需要考虑到边界点的问题。
-        计算填充的宽度，即卷积核宽度的一半，用于处理图像边缘。使用cv2.copyMakeBorder函数进行边缘填充，将图
-        像的边缘复制并填充到周围，以防止边缘像素点无法进行卷积。
-        :param img: 原始图像，要求为灰度图
-        :param k_size: 滤波核大小,默认为3,确保滤波核大小为奇数
-        :return: 处理后的均值滤波图像
-        """
-        if k_size % 2 == 0:
-            k_size += 1
-        rows, cols = img.shape[:2]
-        # 计算需要在图像边界扩充的大小
-        pad_width = (k_size - 1) // 2
-        # 在图像边界进行扩充
-        img_pad = cv2.copyMakeBorder(img, pad_width, pad_width, pad_width, pad_width, cv2.BORDER_REPLICATE)
-        img_filter = np.zeros_like(img)
-        for i in range(rows):
-            for j in range(cols):
-                pixel_values = img_pad[i:i+k_size, j:j+k_size].flatten()
-                img_filter[i, j] = np.mean(pixel_values)
-
-        return img_filter
-
-    def gaussian_kernel(self, size, sigma):
-        """
-        生成高斯核
-        :param size: 核的大小
-        :param sigma: 标准差
-        :return:
-        """
-        kernel = np.zeros((size, size), dtype=np.float32)
-        center = size // 2
-        for i in range(size):
-            for j in range(size):
-                x, y = i - center, j - center
-                kernel[i, j] = np.exp(-(x**2 + y**2)/(2*sigma**2))
-        kernel /= 2 * np.pi * sigma**2
-        kernel /= np.sum(kernel)
-        return kernel
-
-    def Gaussian_Filtering(self, img, kernel_size, sigma):
-        """
-        生成高斯滤波
-        :param img: 输入图像
-        :param kernel_size: 核大小
-        :param sigma: 标准差
-        :return:
-        """
-        kernel = self.gaussian_kernel(kernel_size, sigma)
-        height, width, _ = img.shape
-        result = np.zeros_like(img, dtype=np.float32)
-
-        pad_size = kernel_size // 2
-        img_pad = np.pad(img, [(pad_size, pad_size), (pad_size, pad_size), (0, 0)], mode='constant')
-        for c in range(_):
-            for i in range(pad_size, height + pad_size):
-                for j in range(pad_size, width + pad_size):
-                    result[i - pad_size, j - pad_size, c] = np.sum(kernel * img_pad[i - pad_size:i + pad_size + 1, j - pad_size:j + pad_size + 1, c])
-        return np.uint8(result)
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/transforms/normal.py` & `pyzjr-1.3.9/pyzjr/augmentation/transforms/normal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,106 @@
 import torch
 import numpy as np
 
 IMAGENET_MEAN = 0.485, 0.456, 0.406  # RGB mean
 IMAGENET_STD = 0.229, 0.224, 0.225  # RGB standard deviation
 
-def IMGNET_DENORMALIZE(image):
+def imagenet_denormal(image):
     # 对RGB图像x进行ImageNet反规范化, i.e. = x * std + mean
     return image * IMAGENET_STD + IMAGENET_MEAN
 
-def IMGNET_NORMALIZE(image):
+def imagenet_normal(image):
     # 对RGB图像x进行ImageNet规范化, i.e. = (x - mean) / std
-    return (image / 255.0 - IMAGENET_MEAN) / IMAGENET_STD
+    image = image.astype('float') / 255
+    normal_image = (image - IMAGENET_MEAN) / IMAGENET_STD
+    return normal_image
 
-class Normalize():
-    def __init__(self, image):
+def min_max_normal(np_image):
+    """
+    Min-Max normalization, scales pixel values to a specific range [0, 1].
+    """
+    min_val = np.min(np_image)
+    max_val = np.max(np_image)
+    min_and_max = (np_image - min_val) / (max_val - min_val)
+    return min_and_max
+
+def z_score_normal(np_image):
+    """
+    Z-score, computes the standard scores of given data.
+    """
+    mean = np.mean(np_image)
+    std = np.std(np_image)
+    z_scores = (np_image - mean) / std
+    return z_scores
+
+def linear_normal(np_image):
+    """
+    Linear normalization
+    http://en.wikipedia.org/wiki/Normalization_%28image_processing%29
+    """
+    arr = np_image.astype('float')
+    for i in range(3):
+        minval = arr[..., i].min()
+        maxval = arr[..., i].max()
+        if minval != maxval:
+            arr[..., i] -= minval
+            arr[..., i] *= (255.0 / (maxval - minval))
+    return arr
+
+def zero_centered_normal(np_image):
+    """Zero-centered (centered)"""
+    np_image = np_image.astype('float32')
+    mean = np.mean(np_image)
+    np_image -= mean
+    return np_image
+
+class Normalizer():
+    def __init__(self, normal_type='imagenet'):
+        self.normal_type = normal_type
+
+    def __call__(self, image):
         if isinstance(image, np.ndarray):
             self.image = image
-        elif isinstance(image, torch.Tensor):
-            self.image = image.numpy()
         else:
-            raise ValueError("Unsupported input type. Only numpy arrays and torch tensors are supported.")
+            self.image = np.array(image)
+
+        if self.normal_type == 'imagenet':
+            return imagenet_normal(self.image)
+        elif self.normal_type == 'min_max':
+            return min_max_normal(self.image)
+        elif self.normal_type == 'z_score':
+            return z_score_normal(self.image)
+        elif self.normal_type == 'linear':
+            return linear_normal(self.image)
+        elif self.normal_type == 'zero_centered':
+            return zero_centered_normal(self.image)
+        else:
+            raise ValueError(f"Unsupported normalization type: {self.normal_type}, "
+                             f"You can choose to use these parameters"
+                             f"' imagenet ',' min_max ',' z_score ',' linear ', and ' zero_centered '")
 
-    @property
-    def min_max(self):
-        """
-        Min-Max normalization, scales pixel values to a specific range [0, 1].
-        """
-        min_val = np.min(self.image)
-        max_val = np.max(self.image)
-        min_and_max = (self.image - min_val) / (max_val - min_val)
-        return min_and_max
-
-    @property
-    def z_score(self):
-        """
-        Z-score, computes the standard scores of given data.
-        """
-        mean = np.mean(self.image)
-        std = np.std(self.image)
-        z_scores = (self.image - mean) / std
-        return z_scores
-
-    @property
-    def linear(self):
-        """
-        Linear normalization
-        http://en.wikipedia.org/wiki/Normalization_%28image_processing%29
-        """
-        arr = self.image.astype('float')
-        for i in range(3):
-            minval = arr[..., i].min()
-            maxval = arr[..., i].max()
-            if minval != maxval:
-                arr[..., i] -= minval
-                arr[..., i] *= (255.0 / (maxval - minval))
-        return arr
-
-    @property
-    def zero_centered(self):
-        """Zero-centered (centered)"""
-        mean = np.mean(self.image)
-        self.image -= mean
-        return self.image
 
-def denormalize(data, mean, std):
+def denormalize(image, mean, std):
     """
     Denormalization operation, converts normalized data back to the original range.
 
     Parameters:
-        - data: Input data (NumPy array or Torch tensor)
+        - image: Input data (NumPy array or Torch tensor)
         - mean: Mean used for normalization
         - std: Standard deviation used for normalization
 
     Returns:
         - Denormalized data
     """
-    if isinstance(data, np.ndarray):
+    if isinstance(image, np.ndarray):
         # NumPy arrays
-        denormalized_data = data * std + mean
-    elif torch.is_tensor(data):
+        denormalized_data = image * std + mean
+    elif torch.is_tensor(image):
         # Torch tensors
-        denormalized_data = data.clone()
+        denormalized_data = image.clone()
         for d, m, s in zip(denormalized_data, mean, std):
             d.mul_(s).add_(m)
     else:
         raise ValueError("Unsupported input type. Only NumPy arrays and Torch tensors are supported.")
 
     return denormalized_data
 
@@ -95,14 +111,19 @@
 
     image_path = r"../test.png"
     image = Image.open(image_path)
 
     to_tensor = transforms.ToTensor()
     torch_image = to_tensor(image)
 
-    normalizer = Normalize(torch_image)
+    imagenet_normalized = Normalize('imagenet')
+    min_max_normalized = Normalize('min_max')
+    z_score_normalized = Normalize('z_score')
+    linear_normalized = Normalize('linear')
+    zero_centered = Normalize('zero_centered')
+
 
-    min_max_normalized = normalizer.min_max
-    z_score_normalized = normalizer.z_score
-    linear_normalized = normalizer.linear
-    zero_centered = normalizer.zero_centered
-    print(min_max_normalized,z_score_normalized,linear_normalized,zero_centered)
+    print(imagenet_normalized(image))
+    print(min_max_normalized(image))
+    print(z_score_normalized(image))
+    print(linear_normalized(image))
+    print(zero_centered(image))
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/transforms/opencv.py` & `pyzjr-1.3.9/pyzjr/augmentation/transforms/opencv.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 This module is based on cv2 implemented transformations
 """
 import cv2
 import torch
 import random
 import numpy as np
 from pyzjr.augmentation.augments import Centerzoom, horizontal_flip, vertical_flip, adjust_brightness_cv2, \
-    adjust_gamma, augment_Hsv, hist_equalize, random_rotation, random_lighting, blur, gaussian_blur,\
-    bilateral_blur, median_blur, random_crop, random_resize_crop
-
+    adjust_gamma, augment_Hsv, hist_equalize, random_rotation, random_lighting, random_crop, random_resize_crop
+from pyzjr.augmentation.blur import (
+    meanblur,
+    medianblur,
+    gaussianblur,
+    bilateralblur,
+)
 from pyzjr.core.error import _check_img_is_opencv
 from pyzjr.core.helpers import convert_to_tuple
 from pyzjr.Math import rand
 
 __all__ = ["OpencvToTensor",
            "OpencvResize",
            "OpencvSquareResize",
@@ -180,31 +184,31 @@
         return opencv_img
 
 class OpencvRandomBlur():
     """OpencvRandomBlur类用于对图像进行随机模糊(支持四选一)"""
     def __init__(self, ksize, choice=None):
         self.ksize = ksize
         self.choice = choice
-        if self.ksize not in {1, 3, 5, 7, 9}:
-            raise ValueError(f"Invalid ksize value {ksize}.The available values are 1, 3, 5, 7, 9")
+        if self.ksize not in {1, 3, 5, 7, 9, 11}:
+            raise ValueError(f"Invalid ksize value {ksize}.The available values are 1, 3, 5, 7, 9, 11")
         if self.choice is None:
             filter_functions = ["blur", "median", "gaussian", "bilateral"]
             self.choice = random.choice(filter_functions)
 
     def __call__(self, opencv_img):
         _check_img_is_opencv(opencv_img)
         if self.choice == "blur":
             self.ksize = convert_to_tuple(self.ksize)
-            opencv_img = blur(opencv_img, self.ksize)
+            opencv_img = meanblur(opencv_img, self.ksize)
         elif self.choice == "median":
-            opencv_img = median_blur(opencv_img, self.ksize)
+            opencv_img = medianblur(opencv_img, self.ksize)
         elif self.choice == "gaussian":
-            opencv_img = gaussian_blur(opencv_img, ksize=self.ksize)
+            opencv_img = gaussianblur(opencv_img, ksize=self.ksize)
         elif self.choice == "bilateral":
-            opencv_img = bilateral_blur(opencv_img, self.ksize)
+            opencv_img = bilateralblur(opencv_img, self.ksize)
         return opencv_img
 
 class OpencvCrop():
     """OpencvCrop类用于对图像进行随机裁剪"""
     def __init__(self, size):
         self.size = convert_to_tuple(size)
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/transforms/pillow.py` & `pyzjr-1.3.9/pyzjr/augmentation/transforms/pillow.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 This module is based on PIL implemented transformations.
 """
 import torch
 from PIL import Image, ImageOps, ImageEnhance, ImageFilter
 import random
 from pyzjr.core.error import _check_img_is_plt, is_pil,_check_img_is_ndarray, _check_parameter_is_tuple_and_list_or_single_2, \
     _check_input_is_tensor
-from pyzjr.core.general import get_image_size, is_int, get_image_num_channels, is_list_or_tuple
-from ._utils import Images, Compose
+from pyzjr.core.general import is_int, is_list_or_tuple
+from pyzjr.core._utils import get_image_num_channels
+from pyzjr.augmentation.transforms._utils import Images, Compose
 import numpy as np
 
 __all__ = ["PILToTensor",
            "NdarryToPIL",
            "TensorToPIL",
            "MeanStdNormalize",
            "AdjustBrightness",
@@ -764,15 +765,15 @@
     def __init__(self, size):
         super(RandomCrop, self).__init__()
         self.size = size
 
     def get_shape(self, image, output_size):
         if isinstance(output_size, int):
             output_size = [output_size, output_size]
-        h, w = get_image_size(image)
+        w, h = image.size
         outw, outh = output_size
         if w == outw and h == outh:
             return 0, 0, h, w
 
         if h + 1 < outh or w + 1 < outw:
             raise ValueError(f"Required crop size {(outh, outw)} is larger then input image size {(h, w)}")
         i = torch.randint(0, h - outh + 1, size=(1, )).item()
@@ -1039,15 +1040,15 @@
         - box (tuple, optional): A tuple (x, y, width, height) specifying a fixed crop box. If None, a random box will be generated.
 
     Examples:
         >>> transforms = Compose([RandomResizedCrop(224, (0.2, 1.0)), PILToTensor(), TensorToPIL()])
         >>> transformed_image = transforms(image)
     """
     def __init__(self, sizes, scale=(0.2, 1.0), box=None):
-        super(RandomResizedCrop, self).__init__(sizes,box)
+        super(RandomResizedCrop, self).__init__(sizes, box)
         self.scale = scale
         self.box = box
 
     def get_random_box(self, image, scale):
         width, height = image.size
         minscale_img = (width * scale[0], height * scale[0])
         maxscale_img = (width * scale[1], height * scale[1])
@@ -1069,17 +1070,17 @@
         return super().resize_crop(img, x, y, w, h, self.sizes)
 
 if __name__ == "__main__":
     import matplotlib
     import matplotlib.pyplot as plt
 
     matplotlib.use("TkAgg")
-    image = Image.open(r'D:\PythonProject\Torchproject\classification\dataset\crack\1181.png')
+    image = Image.open(r'D:\PythonProject\pyzjrPyPi\pyzjr\augmentation\test.png')
 
-    transforms = Compose([RandomResizedCrop(224), PILToTensor(), TensorToPIL()])
+    transforms = Compose([PILToTensor(), TensorToPIL()])
     transformed_image = transforms(image)
 
     print(transformed_image.size)
     # transformed_image = torch.clamp(transformed_image, 0, 1)
     # transformed_image = transformed_image.permute(1, 2, 0)
 
     plt.imshow(transformed_image)
```

### Comparing `pyzjr-1.3.8/pyzjr/augmentation/transforms/tvision.py` & `pyzjr-1.3.9/pyzjr/augmentation/transforms/tvision.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,26 @@
 import torch
 from torchvision import transforms as T
 from torchvision.transforms import functional as F
 import cv2
 
 from pyzjr.Math import rand
 
-__all__ = ["pad_if_smaller", "ComposeWithLabel", "RandomResize", "RandomHorizontalFlip", "RandomVerticalFlip",
-           "RandomCrop", "CenterCrop", "ToTensor", "Normalize", "ToHsv", "RandomContrast", "RandomBrightness",]
+__all__ = ["pad_if_smaller",
+           "ComposeWithLabel",
+           "RandomResize",
+           "RandomHorizontal_Flip",
+           "RandomVertical_Flip",
+           "Random_Crop",
+           "Center_Crop",
+           "ToTensor",
+           "Normalize",
+           "ToHSV",
+           "RandomContrast",
+           "RandomBrightness",]
 
 def pad_if_smaller(img, size, fill=0):
     """如果图像最小边长小于给定size，则用数值fill进行padding"""
     min_size = min(img.size)
     if min_size < size:
         ow, oh = img.size
         padh = size - oh if oh < size else 0
@@ -42,47 +52,47 @@
         # 这里size传入的是int类型，所以是将图像的最小边长缩放到size大小
         image = F.resize(image, [size])
         # 这里的interpolation注意下，在torchvision(0.9.0)以后才有InterpolationMode.NEAREST
         # 如果是之前的版本需要使用PIL.Image.NEAREST
         target = F.resize(target, [size], interpolation=Image.NEAREST)
         return image, target
 
-class RandomHorizontalFlip(object):
+class RandomHorizontal_Flip(object):
     def __init__(self, flip_prob):
         self.flip_prob = flip_prob
 
     def __call__(self, image, target):
         if random.random() < self.flip_prob:
             image = F.hflip(image)
             target = F.hflip(target)
         return image, target
 
-class RandomVerticalFlip(object):
+class RandomVertical_Flip(object):
     def __init__(self, flip_prob):
         self.flip_prob = flip_prob
 
     def __call__(self, image, target):
         if random.random() < self.flip_prob:
             image = F.vflip(image)
             target = F.vflip(target)
         return image, target
 
-class RandomCrop(object):
+class Random_Crop(object):
     def __init__(self, size):
         self.size = size
 
     def __call__(self, image, target):
         image = pad_if_smaller(image, self.size)
         target = pad_if_smaller(target, self.size, fill=255)
         crop_params = T.RandomCrop.get_params(image, (self.size, self.size))
         image = F.crop(image, *crop_params)
         target = F.crop(target, *crop_params)
         return image, target
 
-class CenterCrop(object):
+class Center_Crop(object):
     def __init__(self, size):
         self.size = size
 
     def __call__(self, image, target):
         image = F.center_crop(image, self.size)
         target = F.center_crop(target, self.size)
         return image, target
@@ -98,15 +108,15 @@
         self.mean = mean
         self.std = std
 
     def __call__(self, image, target):
         image = F.normalize(image, mean=self.mean, std=self.std)
         return image, target
 
-class ToHsv(object):
+class ToHSV(object):
     def __init__(self, hue_range=(-0.1, 0.1), saturation_range=(0.6, 1.4), value_range=(0.7, 1.3)):
         self.hue_range = hue_range
         self.saturation_range = saturation_range
         self.value_range = value_range
 
     def __call__(self, image, target):
         hsv_image = cv2.cvtColor(np.array(image), cv2.COLOR_RGB2HSV)
@@ -149,18 +159,18 @@
 
     image = Image.open(r'./VOCdevkit\VOC2007\JPEGImages\2007_000032.jpg')
     target = Image.open(r'./VOCdevkit\VOC2007\SegmentationClass\2007_000032.png')
 
     # 创建数据增强操作的组合
     transforms = ComposeWithLabel([
         RandomResize(min_size=256, max_size=512),
-        RandomHorizontalFlip(flip_prob=0.5),
-        RandomCrop(size=224),
-        CenterCrop(size=200),
-        ToHsv(hue_range=(-0.1, 0.1), saturation_range=(0.6, 1.4), value_range=(0.7, 1.3)),
+        RandomHorizontal_Flip(flip_prob=0.5),
+        Random_Crop(size=224),
+        Center_Crop(size=200),
+        ToHSV(hue_range=(-0.1, 0.1), saturation_range=(0.6, 1.4), value_range=(0.7, 1.3)),
 
         ToTensor(),
 
         RandomContrast(),
         RandomBrightness(),
         Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
     ])
```

### Comparing `pyzjr-1.3.8/pyzjr/core/__init__.py` & `pyzjr-1.3.9/pyzjr/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 
 from .general import (
     is_tensor,
     is_pil,
     is_numpy,
     is_gray_image,
     is_rgb_image,
-    get_num_channels,
-    get_image_size,
-    get_image_num_channels,
+    is_str,
     is_int,
     is_float,
+    is_bool,
     is_list,
     is_tuple,
     is_list_or_tuple,
     is_None,
+    is_not_None,
     is_positive_int,
     is_nonnegative_int,
     is_parallel,
     is_ascii,
-    is_url
+    is_url,
+    is_image_extension,
+    is_video_extension,
+    is_file,
+    is_directory,
+    is_directory_not_empty,
+    is_path_exists,
+    is_Linux,
+    is_Windows
 )
 
 from ._utils import (
-    Module,
-    ModuleList,
-    Parameter,
-    Tensor,
-    arange,
-    as_tensor,
-    complex,
-    concatenate,
-    diag,
-    einsum,
-    eye,
-    linspace,
-    normalize,
-    ones,
-    ones_like,
-    pad,
-    rand,
-    softmax,
-    stack,
-    tensor,
-    where,
-    zeros,
-    zeros_like,
+    get_num_channels,
+    get_image_num_channels,
+    get_image_size
 )
+
 from .decorator import timing
 from .lr_scheduler import _LRScheduler
 from .error import *
 
 from .helpers import (
     _ntuple,
     to_1tuple,
```

### Comparing `pyzjr-1.3.8/pyzjr/core/__tensor.py` & `pyzjr-1.3.9/pyzjr/core/__tensor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/core/decorator.py` & `pyzjr-1.3.9/pyzjr/core/decorator.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/core/error.py` & `pyzjr-1.3.9/pyzjr/core/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from .general import is_pil, is_rgb_image, is_numpy, is_tensor, is_gray_image
-import numpy as np
+from pyzjr.core.general import is_pil, is_rgb_image, is_numpy, is_tensor, is_gray_image
 
 Error_flags = "[pyzjr error]:"
 Augment_Error_Message = "Image should be PIL image. Got {}. Use Decode() for encoded data or ToPIL() for decoded data."
 Ndarray_Error_Message = "The input image should be of type numpy.ndarray or PIL.Image.Image. Got {}."
 
 def not_rgb_warning(image):
     if not is_rgb_image(image):
@@ -17,17 +16,15 @@
         raise TypeError(Augment_Error_Message.format(type(img)))
 
 def _check_img_is_ndarray(img):
     if not is_numpy(img):
         raise TypeError(Ndarray_Error_Message.format(type(img)))
 
 def _check_img_is_opencv(img):
-    if isinstance(img, np.ndarray):
-        return True
-    else:
+    if not is_numpy(img):
         raise ValueError("The loaded image should conform to the format read by OpenCV!")
 
 def _check_input_is_tensor(img):
     if not is_tensor(img):
         raise TypeError('Input tensor should be a torch tensor. Got {}.'.format(type(img)))
 
 def _check_parameter_is_tuple_2(a):
```

### Comparing `pyzjr-1.3.8/pyzjr/core/general.py` & `pyzjr-1.3.9/pyzjr/core/general.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import numpy as np
 import re
-from PIL import Image
+import os
 import torch
 import torch.nn as nn
-
+import numpy as np
+from PIL import Image
+import pyzjr.Z as Z
+import platform
 
 def is_tensor(img):
     """Check if the input image is torch format."""
     return isinstance(img, torch.Tensor)
 
 def is_pil(img):
     """Check if the input image is PIL format."""
@@ -19,64 +21,45 @@
 
 def is_gray_image(image):
     return (len(image.shape) == 2) or (len(image.shape) == 3 and image.shape[-1] == 1)
 
 def is_rgb_image(image):
     return len(image.shape) == 3 and image.shape[-1] == 3
 
-def get_num_channels(image):
-    return image.shape[2] if len(image.shape) == 3 else 1
-
-def get_image_size(image):
-    if is_numpy(image):
-        h, w = image.shape[:2]
-        return h, w
-    if is_pil(image):
-        w, h = image.size
-        return h, w
-    if is_tensor(image):
-        if len(image.shape) == 4 or len(image.shape) == 3:
-            w, h = image.shape[-2:]
-            return h, w
-    else:
-        raise ValueError("[pyzjr]:Unsupported input type")
-
-def get_image_num_channels(img):
-    if is_tensor(img):
-        if img.ndim == 2:
-            return 1
-        elif img.ndim > 2:
-            return img.shape[-3]
-    if is_pil(img):
-        return 1 if img.mode == 'L' else 3
-    if is_numpy(img):
-        return 1 if is_gray_image else 3
-
 def is_parallel(model):
     # Returns True if model is of type DP or DDP
     return isinstance(model, (nn.parallel.DataParallel, nn.parallel.DistributedDataParallel))
 
+def is_str(param):
+    return isinstance(param, str)
+
 def is_int(param):
     return isinstance(param, int)
 
 def is_float(param):
     return isinstance(param, float)
 
+def is_bool(param):
+    return param.dtype == np.bool_
+
 def is_list(param):
     return isinstance(param, list)
 
 def is_tuple(param):
     return isinstance(param, tuple)
 
 def is_list_or_tuple(param):
     return isinstance(param, (list, tuple))
 
 def is_None(param):
     return True if param is None else False
 
+def is_not_None(param):
+    return not is_None(param)
+
 def is_positive_int(param):
     return is_int(param) and param > 0
 
 def is_nonnegative_int(param):
     return is_int(param) and param >= 0
 
 def is_ascii(s):
@@ -90,8 +73,40 @@
     s = str(s)
     return all(ord(c) < 128 for c in s)
 
 def is_url(filename):
     """Return True if string is an http or ftp path."""
     URL_REGEX = re.compile(r'http://|https://|ftp://|file://|file:\\')
     return (isinstance(filename, str) and
-            URL_REGEX.match(filename) is not None)
+            URL_REGEX.match(filename) is not None)
+
+def is_image_extension(image_name):
+    ext = image_name.split('.')
+    return ext[-1] in Z.IMG_FORMATS and is_str(image_name)
+
+def is_video_extension(video_name):
+    ext = video_name.split('.')
+    return ext[-1] in Z.VID_FORMATS and is_str(video_name)
+
+def is_file(path):
+    return os.path.isfile(path) and is_str(path)
+
+def is_directory(path):
+    return os.path.isdir(path) and is_str(path)
+
+def is_directory_not_empty(path):
+    return os.path.isdir(path) and len(os.listdir(path)) > 0 and is_str(path)
+
+def is_path_exists(path):
+    return os.path.exists(path) and is_str(path)
+
+def is_Windows():
+    if platform.system() == "Windows":
+        return True
+
+def is_Linux():
+    if platform.system() == "Linux":
+        return True
+
+if __name__=="__main__":
+    image_name = r'D:\PythonProject\pyzjrPyPi\pyzjr\augmentation\test.png'
+    print(is_file(image_name), is_Windows())
```

### Comparing `pyzjr-1.3.8/pyzjr/core/helpers.py` & `pyzjr-1.3.9/pyzjr/core/helpers.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/core/lr_scheduler.py` & `pyzjr-1.3.9/pyzjr/core/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/core/utils_pytorch_numpy_unification.py` & `pyzjr-1.3.9/pyzjr/core/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/Dataloader.py` & `pyzjr-1.3.9/pyzjr/data/Dataloader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/Dataset.py` & `pyzjr-1.3.9/pyzjr/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/FM.py` & `pyzjr-1.3.9/pyzjr/data/FM.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     sh = logging.StreamHandler()
     sh.setFormatter(formatter)
     logger.addHandler(sh)
 
     return logger
 
-def getFilePath(filedir,format='png'):
+def getFilePath(filedir, format='png'):
     """What is returned is a list that includes all paths under the target path that match the suffix."""
     file_list = [os.path.join(root, filespath) \
                  for root, dirs, files in os.walk(filedir) \
                  for filespath in files \
                  if str(filespath).endswith(format)
                  ]
     return file_list if file_list else []
```

### Comparing `pyzjr-1.3.8/pyzjr/data/basedataset.py` & `pyzjr-1.3.9/pyzjr/data/basedataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/data_set/Pascal_voc.py` & `pyzjr-1.3.9/pyzjr/data/data_set/Pascal_voc.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/data_set/config.py` & `pyzjr-1.3.9/pyzjr/data/data_set/config.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/reader.py` & `pyzjr-1.3.9/pyzjr/data/reader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/data/txt_utils.py` & `pyzjr-1.3.9/pyzjr/data/txt_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 
 def get_file_list(file_dir):
     files = os.listdir(file_dir)
     files_num = len(files)
     return files, files_num
 
-def generate_txt(target_path, txt_name=r'./output.txt'):
-    f = open(txt_name, "w")
+def generate_txt(target_path, onlybasename=False, txt_path=r'./output.txt'):
+    f = open(txt_path, "w")
     files, files_num = get_file_list(target_path)
     index_count = 0
     count = 0
     for file in files:
         index_count = index_count + 1
+        path = str(file) if onlybasename else os.path.join(target_path, str(file))
         if count == files_num - 1:
-            f.write(os.path.join(target_path, str(file)))
+            f.write(path)
             break
         if index_count >= 0:
-            f.write(os.path.join(target_path, str(file)) + "\n")
+            f.write(path + "\n")
             count = count + 1
     f.close()
 
 def read_file_from_txt(txt_path):
     files = []
     for line in open(txt_path, "r"):
         files.append(line.strip())
```

### Comparing `pyzjr-1.3.8/pyzjr/devices/__init__.py` & `pyzjr-1.3.9/pyzjr/devices/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .get_device import (
     Central_Processing_Unit,
     Graphics_Processing_Unit,
     use_all_gpu,
     num_workers,
-    release_memory,
+    load_owned_device,
+    load_device_on_model,
     CPU, cpu,
     GPU, gpu
 )
 
 from .measures import (
     release_gpu_memory,
+    release_memory,
     PeakCPUMemory,
     start_measure,
     end_measure,
     log_measures
 )
 
 from .systeminfo import (
```

### Comparing `pyzjr-1.3.8/pyzjr/devices/get_device.py` & `pyzjr-1.3.9/pyzjr/devices/get_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import torch
-import gc
 
 def Central_Processing_Unit():
     """
     Returns the CPU device.
 
     Returns:
         torch.device: The CPU device.
@@ -32,25 +31,35 @@
 
 def num_workers(batch_size):
     """
     Determine the number of parallel worker processes used for data loading
     """
     return min([os.cpu_count(), batch_size if batch_size > 1 else 0, 8])
 
-def release_memory(*args):
+def load_owned_device():
     """
-    Function to release memory resources, particularly useful when working with PyTorch and CUDA.
+    Return appropriate device objects based on whether the system supports CUDA.
     """
-    if torch.cuda.is_available():
-        torch.cuda.empty_cache()
-    if not isinstance(args, list):
-        args = list(args)
-    for i in range(len(args)):
-        args[i] = None
-    gc.collect()
-    return args
+    return torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
+def load_device_on_model(model, i=0):
+    """
+    Load the model onto the specified device, prioritize CUDA devices (if available),
+    otherwise load onto the CPU.
+    If the number of CUDA devices is greater than 1, use torch. nn DataParallel copies
+    the model to all available CUDA devices.
+    """
+    if torch.cuda.device_count() > 1:
+        model = torch.nn.DataParallel(model).to(f'cuda:{i}')
+    elif torch.cuda.is_available():
+        model = model.to(f'cuda:{i}')
+    else:
+        model = model.to('cpu')
+    return model
 
 CPU = cpu = Central_Processing_Unit
 GPU = gpu = Graphics_Processing_Unit
 
+if __name__=="__main__":
+    device = load_owned_device()
+    print(device)
```

### Comparing `pyzjr-1.3.8/pyzjr/devices/measures.py` & `pyzjr-1.3.9/pyzjr/devices/measures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 import gc
 import threading
 import time
 import psutil
 import torch
 
-__all__ = ["release_gpu_memory", "PeakCPUMemory", "start_measure", "end_measure",
-           "log_measures"]
+__all__ = [
+    "release_gpu_memory",
+    "release_memory",
+    "PeakCPUMemory",
+    "start_measure",
+    "end_measure",
+    "log_measures"
+]
 
 def release_gpu_memory():
     gc.collect()
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
+def release_memory(*args):
+    """
+    Function to release memory resources, particularly useful when working with PyTorch and CUDA.
+    """
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
+    if not isinstance(args, list):
+        args = list(args)
+    for i in range(len(args)):
+        args[i] = None
+    gc.collect()
+    return args
+
 class PeakCPUMemory:
     def __init__(self):
         self.process = psutil.Process()
         self.peak_monitoring = False
 
     def peak_monitor(self):
         self.cpu_memory_peak = -1
```

### Comparing `pyzjr-1.3.8/pyzjr/devices/systeminfo.py` & `pyzjr-1.3.9/pyzjr/devices/systeminfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     print("CPU型号:", CPU_MODEL_INFO())
     print("CPU核心数量:", CPU_NUMBERS_COUNT())
     print("系统信息:", System_VERSION_INFO())
     print("---------------------------")
     print("Pyzjr版本:", zjr.__version__)
 
 
-if __name__=="__main__":
+if __name__ == "__main__":
     Pyzjr_INFO()
```

### Comparing `pyzjr-1.3.8/pyzjr/dlearn/callbacklog.py` & `pyzjr-1.3.9/pyzjr/dlearn/callbacklog.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/dlearn/callbacks.py` & `pyzjr-1.3.9/pyzjr/dlearn/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/dlearn/strategy.py` & `pyzjr-1.3.9/pyzjr/dlearn/strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -82,21 +82,21 @@
     :param size: 目标尺寸，形如 (width, height)
     :param frame: 是否进行不失真的resize
     :return: 调整大小后的图像，PIL Image 对象
     """
     iw, ih = image.size
     w, h = size
     if frame:
-        scale = min(w/iw, h/ih)
-        nw = int(iw*scale)
-        nh = int(ih*scale)
-
-        image = image.resize((nw,nh), Image.BICUBIC)
-        new_image = Image.new('RGB', size, (128,128,128))
-        new_image.paste(image, ((w-nw)//2, (h-nh)//2))
+        scale = min(w / iw, h / ih)
+        nw = int(iw * scale)
+        nh = int(ih * scale)
+
+        image = image.resize((nw, nh), Image.BICUBIC)
+        new_image = Image.new('RGB', size, (128, 128, 128))
+        new_image.paste(image, ((w-nw) // 2, (h-nh) // 2))
         return new_image, nw, nh
     else:
         new_image = image.resize((w, h), Image.BICUBIC)
         return new_image
 
 def SeedEvery(seed=11, rank=0, use_deterministic_algorithms=None):
     """
@@ -125,28 +125,10 @@
             torch.use_deterministic_algorithms(True)
         elif hasattr(torch, "set_deterministic"):
             torch.set_deterministic(True)
         else:
             warnings.warn("If use_deterministic-algorithms=True is set, pytorch version "
                           "greater than 1.8 may be required to use this feature properly.")
 
-def summarys(input_shape, model):
-    """
-    打印模型的摘要信息，并计算模型的总浮点运算量和总参数数量
-    :param input_shape:
-    :param model:要进行计算的模型
-    """
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    models = model.to(device)
-    summary(models, (3, input_shape[0], input_shape[1]))
-
-    dummy_input = torch.randn(1, 3, input_shape[0], input_shape[1]).to(device)
-    flops, params = profile(models.to(device), (dummy_input, ), verbose=False)
-    flops = flops * 2
-    flops, params = clever_format([flops, params], "%.3f")
-    print('Total GFLOPS: %s' % (flops))
-    print('Total params: %s' % (params))
-
-
 def get_lr(optimizer):
     for param_group in optimizer.param_groups:
         return param_group['lr']
```

### Comparing `pyzjr-1.3.8/pyzjr/dlearn/tools.py` & `pyzjr-1.3.9/pyzjr/dlearn/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyzjr.visualize.video_utils import Timer
 from pyzjr.visualize.printf import colorstr
 try:
     import thop  # for FLOPs computation
 except ImportError:
     thop = None
 
-__all__ = ["Runcodes", "LoadingBar", "show_config", "GPU_INFO", "time_sync", "profile"]
+__all__ = ["Runcodes", "LoadingBar", "show_config", "time_sync", "profile"]
 
 class Runcodes:
     """
     Comparing the running time of different algorithms.
     example:
         with Runcodes("inference time"):
             output = ...
@@ -72,18 +72,14 @@
 
     for key, value in kwargs.items():
         counter += 1
         print(colorstr(color, f'|%5d | %45s | %55s|' % (counter, key, value)))
 
     print(colorstr(color, '-' * 113))
 
-def GPU_INFO(headColor="red",gpuColor="red"):
-    print(colorstr(headColor, 'GPU INFO:'))
-    print(colorstr(gpuColor, torch.cuda.memory_summary()), end='')
-
 def profile(input, ops, n=10, cuda=True):
     """
     Usage:
         model = MyModel().to('cuda')
         input_tensor = torch.randn(1, 3, 512, 512).to('cuda')
         profile(input_tensor, model, n=10)
     """
```

### Comparing `pyzjr-1.3.8/pyzjr/dlearn/trainer.py` & `pyzjr-1.3.9/pyzjr/dlearn/trainer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/Metrics/__init__.py` & `pyzjr-1.3.9/pyzjr/nn/Metrics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,32 +10,37 @@
 )
 
 from .classification import (
     accuracy_all_classes,
     cls_matrix,
     BinaryConfusionMatrix,
     MulticlassConfusionMatrix,
-    ConfusionMatrixs,
+    ConfusionMatrixs2D,
     ModelIndex,
     calculate_metrics,
     MultiLabelConfusionMatrix
 )
 
-from .segment3d import (
-    PPV,
-    DiceMetric3d,
-    MeanIoU3d,
-    JaccardMetric3d,
-    HausdorffDistanceMetric3d
-)
-
 from .indexutils import (
     hd, hd95,
     _surface_distances,
     ignore_background,
+    calculate_area,
+    mean_iou,
+    auc_roc,
+    accuracy,
+    dice,
+    kappa,
+    do_metric_reduction
+)
+
+from .segment3d import (
+    DiceMetric3d,
+    HausdorffDistanceMetric3d,
+    MeanIoUMetric3d
 )
 
 from .medical_index import (
     ConfusionMatrixs3D,
     get_confusion_matrix_3d,
     get_confusion_matrix_3d_np,
     get_confusion_matrix_3d_torch
```

### Comparing `pyzjr-1.3.8/pyzjr/nn/Metrics/classification.py` & `pyzjr-1.3.9/pyzjr/nn/Metrics/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import torch
 
 __all__ = [
     "accuracy_all_classes",
     "cls_matrix",
     "BinaryConfusionMatrix",
     "MulticlassConfusionMatrix",
-    "ConfusionMatrixs",
+    "ConfusionMatrixs2D",
     "ModelIndex",
     "calculate_metrics",
     "MultiLabelConfusionMatrix"
 ]
 
 def accuracy_all_classes(output, target):
     """
@@ -128,15 +128,15 @@
         if self.reduction == 'mean':
             return np.mean(TP), np.mean(FN), np.mean(FP), np.mean(TN)
         elif self.reduction == 'sum':
             return np.sum(TP), np.sum(FN), np.sum(FP), np.sum(TN)
         elif self.reduction == 'none':
             return TP, FN, FP, TN
 
-class ConfusionMatrixs(cls_matrix):
+class ConfusionMatrixs2D(cls_matrix):
     """
     结合多分类与二分类两种情况, 用法与这二者相同
     """
     def __init__(self, num_classes, reduction='mean'):
         super().__init__(num_classes)
         self.num_classes = num_classes
         self.reduction = reduction
@@ -411,15 +411,15 @@
         self.matrixs += np.array([tn, fp, fn, tp]).T.reshape(-1, 2, 2)
 
     @property
     def get_matrix(self):
         return self.matrixs
 
 if __name__=="__main__":
-    confusion_matrix = ConfusionMatrixs(num_classes=3, reduction='none')
+    confusion_matrix = ConfusionMatrixs2D(num_classes=3, reduction='none')
     true = torch.tensor([1, 1, 1, 0, 0, 0, 2, 2, 2, 2])
     pred = torch.tensor([1, 0, 0, 0, 2, 1, 0, 0, 2, 2])
     confusion_matrix.update(pred, true)
     TP, FN, FP, TN = confusion_matrix.ravel()
     print(TP, FN, FP, TN)
     print(confusion_matrix.get_matrix)
```

### Comparing `pyzjr-1.3.8/pyzjr/nn/Metrics/medical_index.py` & `pyzjr-1.3.9/pyzjr/nn/Metrics/medical_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import torch.nn as nn
 import numpy as np
 from pyzjr.core.general import is_numpy, is_tensor
-from pyzjr.nn.Metrics.indexutils import ignore_background
+from pyzjr.nn.Metrics.indexutils import ignore_background, do_metric_reduction
 
 def get_confusion_matrix_3d_torch(y_pred, y, include_background=True):
     """
     Calculate the three-dimensional confusion matrix of tensor type.
     """
     if not include_background:
         y_pred, y = ignore_background(y_pred=y_pred, y=y)
@@ -89,22 +89,23 @@
         ``"prevalence threshold"``, ``"threat score"``, ``"accuracy"``, ``"balanced accuracy"``,
         ``"f1 score"``, ``"matthews correlation coefficient"``, ``"fowlkes mallows index"``,
         ``"informedness"``, ``"markedness"``]
 
     For more names, you can refer to the "_check_confusion_matrix_metric name" function
     under this category.
     """
-    def __init__(self, metric_name, reduction='mean', eps=1e-5):
+    def __init__(self, metric_name, include_background=True, reduction='mean', eps=1e-5):
         super(ConfusionMatrixs3D, self).__init__()
         self.metric = self._check_confusion_matrix_metric_name(metric_name)
+        self.include_background = include_background
         self.reduction = reduction
         self.eps = eps
 
     def forward(self, y_pred, y):
-        confusion_matrix = get_confusion_matrix_3d_torch(y_pred, y)
+        confusion_matrix = get_confusion_matrix_3d_torch(y_pred, y, self.include_background)
         confusion_matrix = self._check_conf_matrix_format(confusion_matrix)
         tp = confusion_matrix[..., 0]
         fp = confusion_matrix[..., 1]
         tn = confusion_matrix[..., 2]
         fn = confusion_matrix[..., 3]
         p = tp + fn
         n = fp + tn
@@ -158,21 +159,17 @@
             npv = torch.where((tn + fn) > 0, tn / (tn + fn), nan_tensor)
             numerator = ppv + npv - 1.0
             denominator = 1.0
         else:
             raise NotImplementedError("the metric is not implemented.")
         index = numerator / (denominator + self.eps)
 
-        if self.reduction == 'mean':
-            index = index.mean()
-        elif self.reduction == 'sum':
-            index = index.mean()
-        elif self.reduction == 'none':
-            return index
-        return index
+        f, not_nans = do_metric_reduction(index, self.reduction)  # type: ignore
+        return f
+
 
     def _check_conf_matrix_format(self, confusion_matrix):
         input_dim = confusion_matrix.ndimension()
         if input_dim == 1:
             confusion_matrix = confusion_matrix.unsqueeze(dim=0)
         if confusion_matrix.shape[-1] != 4:
             raise ValueError("the size of the last dimension of confusion_matrix should be 4.")
```

### Comparing `pyzjr-1.3.8/pyzjr/nn/Metrics/semantic.py` & `pyzjr-1.3.9/pyzjr/nn/Metrics/semantic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/Summary.py` & `pyzjr-1.3.9/pyzjr/nn/Summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,22 +114,22 @@
     summary_logs.append("--------------------------------------------------------------------------")
 
     summary_info = "\n".join(summary_logs)
 
     print(summary_info)
     return summary_info
 
-def summary_2(model, x, *args, **kwargs):
+def summary_2(model, input_size, *args, **kwargs):
     """Summarize the given input model.
     Summarized information are 1) output shape, 2) kernel shape,
     3) number of the parameters and 4) operations (Mult-Adds)
 
     Args:
         model (Module): Model to summarize
-        x (Tensor): Input tensor of the model with [N, C, H, W] shape
+        input_size (Tensor): Input tensor of the model with [N, C, H, W] shape
                     dtype and device have to match to the model
         args, kwargs: Other argument used in `model.forward` function
     """
     def register_hook(module):
         def hook(module, inputs, outputs):
             cls_name = str(module.__class__).split(".")[-1].split("'")[0]
             module_idx = len(summary)
@@ -183,15 +183,15 @@
             hooks.append(module.register_forward_hook(hook))
 
     hooks = []
     summary = OrderedDict()
 
     model.apply(register_hook)
     with torch.no_grad():
-        model(x) if not (kwargs or args) else model(x, *args, **kwargs)
+        model(input_size) if not (kwargs or args) else model(input_size, *args, **kwargs)
 
     for hook in hooks:
         hook.remove()
 
     print("-"*100)
     print("{:<15} {:>20} {:>20} {:>20} {:>20}"
           .format("Layer", "Kernel Shape", "Output Shape",
@@ -225,8 +225,8 @@
     print("-"*100)
 
 if __name__ == "__main__":
     import torchvision.models.resnet as models
     model = models.resnet18()
     input_size = (3, 224, 224)
     summary_1(model, input_size=input_size)
-    summary_2(model, torch.ones((1, 3, 224, 224)))
+    summary_2(model, input_size=torch.ones((1, 3, 224, 224)))
```

### Comparing `pyzjr-1.3.8/pyzjr/nn/functional.py` & `pyzjr-1.3.9/pyzjr/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/OneHot.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/OneHot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/__init__.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/avgweight.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/avgweight.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/learnrate.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/learnrate.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/loss_function.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/loss_function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/nn/torchutils/loss_utils.py` & `pyzjr-1.3.9/pyzjr/nn/torchutils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/networks/basic_unet.py` & `pyzjr-1.3.9/pyzjr/torch3D/networks/basic_unet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/networks/block/DSConv.py` & `pyzjr-1.3.9/pyzjr/torch3D/networks/block/DSConv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/networks/dscnet.py` & `pyzjr-1.3.9/pyzjr/torch3D/networks/dscnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,8 @@
     # 4 x 1 x 32 x 32 x 32
     input = torch.ones(1, 1, 32, 32, 32).to(device)
     net = DSCNet3D(in_channels=1, num_classes=3, kernel_size=9, device=device,
                  extend_scope=1.0, if_offset=True, number=16)
     net = net.to(device)
     out = net(input)
     print(out.shape)
-    torchsummary.summary(net, input_size=(1, 32, 32, 32))
-
-
-
-
-
-
+    torchsummary.summary(net, input_size=(1, 32, 32, 32))
```

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/networks/vent.py` & `pyzjr-1.3.9/pyzjr/torch3D/networks/vnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/nii/mri.py` & `pyzjr-1.3.9/pyzjr/torch3D/nii/mri.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/nii/nifti_dataset.py` & `pyzjr-1.3.9/pyzjr/torch3D/nii/nifti_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,26 @@
         scale (float): 缩放因子，用于缩放图像和标签。默认为0.5.
         num_classes (int): 类别数量。
         normalize (bool): 是否对图像进行归一化。默认为True.
     """
     def __init__(self,
                  image_path,
                  label_path,
-                 target_shape,
-                 scale=.5,
+                 target_shape=(160, 160, 160),
+                 scale=.6,
                  num_classes=None,
                  normalize=True
                  ):
         super().__init__()
         self.image_paths = self.read_path2list(image_path)
         self.label_paths = self.read_path2list(label_path)
         self.num_classes = num_classes
         self.normalize = normalize
         self.scale = scale
-        self.target_crop_shape = (int(target_shape[0] // scale),
-                                 int(target_shape[1] // scale),
-                                 int(target_shape[2] // scale))
+        self.target_crop_shape = target_shape
 
     def __getitem__(self, item):
         one_image, one_label = self.read_nii_im_and_label(
             self.image_paths[item], self.label_paths[item]
         )
         one_image = center_crop_nii(one_image, self.target_crop_shape)
         one_label = center_crop_nii(one_label, self.target_crop_shape)
@@ -53,15 +51,15 @@
         self.label_trans = one_label[np.newaxis, :, :, :]  # b c d w h
 
         if isinstance(image_trans, torch.Tensor):
             image_trans = image_trans.numpy()
         if isinstance(self.label_trans, torch.Tensor):
             self.label_trans = self.label_trans.numpy()
         one_hot_label_trans = one_hot_3d(self.label_trans[0], num_classes=self.num_classes)
-        # one_hot_label_trans  b  d  y  x  c ----->  b  c  d  y  x
+        # one_hot_label_trans  d  y  x  c ----->  c  d  y  x
         return image_trans, np.transpose(one_hot_label_trans, (3, 0, 1, 2))
 
     def read_nii_im_and_label(self, image_path, label_path):
         image, _, _ = nii_load(image_path)
         label, _, _ = nii_load(label_path)
         # w, h, d  ----->  d, h, w
         return np.transpose(image, (2, 1, 0)), np.transpose(label, (2, 1, 0))
@@ -82,15 +80,15 @@
     def _get_label_unique(self):
         return np.unique(self.label_trans)
 
 if __name__=="__main__":
     image_path = r"D:\PythonProject\pytorch_segmentation_3D\DSCNet_3D\SegDataset\MRI_Hippocampus\imagesTe"
     label_path = r"D:\PythonProject\pytorch_segmentation_3D\DSCNet_3D\SegDataset\MRI_Hippocampus\labelsTe"
 
-    dataset = NiftiDataset3D(image_path, label_path, target_shape=(64, 64, 64), num_classes=3)
+    dataset = NiftiDataset3D(image_path, label_path, num_classes=3)
     dataloader = DataLoader(dataset, batch_size=2, shuffle=True)
 
     for i, (image, onehotlabel) in enumerate(dataset):
         print(f"Sample {i+1}:")
         print("Image shape:", image.shape)
         print("One Hot Label shape:", onehotlabel.shape)
         print(np.unique(onehotlabel), np.unique(onehotlabel[0]), np.unique(onehotlabel[1]),
```

### Comparing `pyzjr-1.3.8/pyzjr/torch3D/nii/nii_utils.py` & `pyzjr-1.3.9/pyzjr/torch3D/nii/nii_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/__init__.py` & `pyzjr-1.3.9/pyzjr/visualize/color/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/colormap.py` & `pyzjr-1.3.9/pyzjr/visualize/color/colormap.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/colorspace.py` & `pyzjr-1.3.9/pyzjr/visualize/color/colorspace.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/cvplot.py` & `pyzjr-1.3.9/pyzjr/visualize/color/cvplot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/findcolor.py` & `pyzjr-1.3.9/pyzjr/visualize/color/findcolor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/color/hex.py` & `pyzjr-1.3.9/pyzjr/visualize/color/hex.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/io.py` & `pyzjr-1.3.9/pyzjr/visualize/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 This module is applied to image reading and display.
 """
 import os
 import cv2
 import imghdr
 import torch
+
 import numpy as np
 from urllib import request
-
 from matplotlib import pyplot as plt
 plt.rcParams['font.sans-serif'] = ['SimHei']
 plt.rcParams['axes.unicode_minus'] = False
 from pathlib import Path
 from pyzjr.core.general import is_gray_image, is_pil, is_url
 
 __all__ = ["ImagesReader", "imwrite", "imshowplt", "StackedCV2", "StackedImages", "Stackedplt",
@@ -29,15 +29,15 @@
 RGB2HSV  = cv2.COLOR_RGB2HSV
 HSV2BGR  = cv2.COLOR_HSV2BGR
 HSV2RGB  = cv2.COLOR_HSV2RGB
 
 class ImagesReader(object):
     def __init__(self, filename, is_gray=False, flip=None):
         """
-         Initialize ImagesReader object.
+        Initialize ImagesReader object.
 
         :param filename: Path to the image file.
         :param is_gray: If True, read the image in grayscale.
         :param flip: 0: Flip vertically.
                     1: Flip horizontally.
                    -1: Flip both vertically and horizontally.
         """
@@ -97,15 +97,15 @@
         res = request.urlopen(url, timeout=3)
     else:
         raise ValueError("[url2imgcv2]:The current input parameter does not conform to the URL format")
     try:
         image = np.asarray(bytearray(res.read()), dtype="uint8")
         image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
     except:
-        print ('[url2imgcv2]: Load read - Image timeout!')
+        print('[url2imgcv2]: Load read - Image timeout!')
         image = []
     h, w, c = image.shape
     if c == 4:
         image = image[:,:,:3]
     return image
 
 def imwrite(filename: str, img: np.ndarray, params=None):
```

### Comparing `pyzjr-1.3.8/pyzjr/visualize/mediapipe/HandTrack.py` & `pyzjr-1.3.9/pyzjr/visualize/mediapipe/HandTrack.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/mediapipe/const.py` & `pyzjr-1.3.9/pyzjr/visualize/mediapipe/const.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.8/pyzjr/visualize/printf.py` & `pyzjr-1.3.9/pyzjr/visualize/printf.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         # Logging to console
         stream_handler = logging.StreamHandler()
         stream_handler.setFormatter(logging.Formatter('%(message)s'))
         logger.addHandler(stream_handler)
 
 def printlog(info):
     nowtime = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-    print("\n"+"=========="*8 + "%s"%nowtime)
+    print("\n"+"=========="*8 + "%s" % nowtime)
     print(info+'...\n\n')
 
 def colorful(obj, color="red", display_type="plain"):
     # 彩色输出格式：
     # 设置颜色开始 ：\033[显示方式;前景色;背景色m
     # 前景色            背景色           颜色
     # ---------------------------------------
@@ -108,9 +108,7 @@
     colors = ["red", "green", "blue", "yellow", "purple", "cyan", "white"]
     display_types = ["plain", "highlight", "underline", "shine", "inverse", "invisible"]
 
     for color in colors:
         for display_type in display_types:
             colored_text = colorful(text, color=color, display_type=display_type)
             print(f"Color: {color}, Display Type: {display_type} -> {colored_text}")
-
-
```

### Comparing `pyzjr-1.3.8/pyzjr/visualize/utils.py` & `pyzjr-1.3.9/pyzjr/augmentation/PIC.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,99 @@
 import cv2
-import numpy as np
+from pylab import *
 import pyzjr.Z as Z
-from PIL import Image
-
-def RemoveInboxes(boxes):
-    """
-    中心点的方法,去除重叠的框,并去掉相对较小的框
-    :param boxes: [minc, minr, maxc, maxr]
-    :return: 过滤的boxes
-    """
-    final_boxes = []
-    for box in boxes:
-        x1, y1, x2, y2 = box
-        cx = (x1 + x2) / 2
-        cy = (y1 + y2) / 2
-        box_area = (x2 - x1) * (y2 - y1)
-        is_inner = False
-        for fb in final_boxes:
-            fx1, fy1, fx2, fy2 = fb
-            if fx1 <= cx <= fx2 and fy1 <= cy <= fy2:
-                fb_area = (fx2 - fx1) * (fy2 - fy1)
-                if box_area >= fb_area:
-                    final_boxes.remove(fb)
-                else:
-                    is_inner = True
-                    break
-        if not is_inner:
-            final_boxes.append(box)
-    return final_boxes
-
-def cvt8png(pngpath, bit_depth=False, target=Z.white, convert=(128, 0, 0)):
-    """
-    Voc: RGB png彩图转换
-    :param bit_depth: 默认转为8位,需要使用out_png.save可以正确保存
-    True:                      False:
-        plt.imshow(img)             cv2.imshow("img",img)
-        plt.axis('off')             cv2.waitKey(0)
-        plt.show()
-    :param pngpath: 为保证是按照cv2的方式读入,所以传入路径即可
-    :param target: 目标颜色,RGB方式
-    :param convert: 转换颜色,同RGB格式
-    :return:
-    """
-    png = cv2.imread(pngpath)
-    png = cv2.cvtColor(png, cv2.COLOR_BGR2RGB)
-    h, w = png.shape[:2]
-
-    mask = np.all(png == target, axis=-1)
-    out_png = np.zeros((h, w, 3), dtype=np.uint8)
-    out_png[mask] = convert
-    out_png[~mask] = png[~mask]
-
-    if bit_depth:
-        out_png_pil = Image.fromarray(out_png)
-        out_png_pil = out_png_pil.convert("P", palette=Image.ADAPTIVE, colors=256)
-        return out_png_pil
-    else:
-        out_png_cv = cv2.cvtColor(out_png, cv2.COLOR_RGB2BGR)
-        return out_png_cv
-
-def cvtMask(pngpath, lower ,upper, convert=(255, 255, 255)):
-    """
-    去除标签中的杂色,并对其进行颜色的转换
-
-    :param pngpath: 输入图像的文件路径
-    :param lower: 颜色范围的下限值，作为一个包含(B, G, R)值的元组
-    :param upper: 颜色范围的上限值，作为一个包含(B, G, R)值的元组
-    :param convert: 需要转换为的颜色，作为一个包含(B, G, R)值的元组
-    :return: 处理后的图像
-    """
-    image = cv2.imread(pngpath)
-    lower = np.array(lower, dtype=np.uint8)
-    upper = np.array(upper, dtype=np.uint8)
-
-    mask = cv2.inRange(image, lower, upper)
-    image[mask > 0] = convert
-
-    return image
-
-def imageContentMove(image, H_pixels=None, V_pixels=None):
-    if H_pixels is None:
-        H_pixels = 0
-    if V_pixels is None:
-        V_pixels = 0
-    h, w = image.shape[:2]
-    black = np.zeros_like(image)
-
-    start_row, end_row = max(0, V_pixels), min(h, h + V_pixels)
-    start_col, end_col = max(0, H_pixels), min(w, w + H_pixels)
-
-    fill_start_row, fill_end_row = max(0, -V_pixels), min(h, h - V_pixels)
-    fill_start_col, fill_end_col = max(0, -H_pixels), min(w, w - H_pixels)
-
-    black[start_row:end_row, start_col:end_col] = image[fill_start_row:fill_end_row, fill_start_col:fill_end_col]
-
-    return black
+from pyzjr.Math import *
+from skimage.morphology import disk
+from skimage.filters import rank
+from skimage import measure
+from torchvision import transforms
+from pyzjr.augmentation.mask_ops import BinaryImg
+
+def getContours(img, cThr=(100, 100), minArea=1000, filter=0, draw=True):
+    """
+    :param img: 输入图像
+    :param cThr: 阈值
+    :param minArea: 更改大小
+    :param filter: 过滤
+    :param draw: 绘制边缘
+    :return: 返回图像轮廓
+    """
+    imgGray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+    imgBlur = cv2.GaussianBlur(imgGray, (5, 5), 1)
+    imgCanny = cv2.Canny(imgBlur, cThr[0], cThr[1])
+    kernel = np.ones((5, 5))
+    imgDial = cv2.dilate(imgCanny, kernel, iterations=3)
+    imgThre = cv2.erode(imgDial, kernel, iterations=2)
+    contours, _ = cv2.findContours(imgThre, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+    finalCountours = []
+    for i in contours:
+        area = cv2.contourArea(i)
+        if area > minArea:
+            peri = cv2.arcLength(i, True)
+            approx = cv2.approxPolyDP(i, 0.02 * peri, True)
+            bbox = cv2.boundingRect(approx)
+            if filter > 0:
+                if len(approx) == filter:
+                    finalCountours.append([len(approx), area, approx, bbox, i])
+            else:
+                finalCountours.append([len(approx), area, approx, bbox, i])
+    finalCountours = sorted(finalCountours, key=lambda x: x[1], reverse=True)
+    if draw:
+        for con in finalCountours:
+            cv2.drawContours(img, con[4], -1, (0, 0, 255), 3)
+    return img, finalCountours
+
+def labelpoint(im, click=4):
+    """
+    交互式标注
+    :param im: 图像,采用im = Image.open(?)的方式打开，颜色空间才是正常的
+    :param click: 点击次数、默认为4
+    :return: 返回点的坐标
+    """
+    imshow(im)
+    print(f'please click {click} points')
+    x = ginput(click)
+    print('you clicked:',x)
+    return x
+
+def get_warp_perspective(img, targetWH):
+    """
+    标注方式按照先上后下，先左后右的顺序
+    :param img: 图像
+    :param targetWH: 已知目标物体的宽度,长度
+    :return: 修正后的图像
+    """
+    width, height = targetWH
+    pts1 = np.float32(labelpoint(img))
+    pts2 = np.float32([[0, 0], [width, 0], [0, height], [width, height]])
+    matrix = cv2.getPerspectiveTransform(pts1, pts2)
+    imgOutput = cv2.warpPerspective(img, matrix, (width, height))
+    return imgOutput
+
+def SearchOutline(binary_image):
+    """
+    在给定图像中搜索轮廓并返回轮廓的坐标列表。
+    :param binary_image: 要搜索轮廓的图像。
+    :return: 包含轮廓坐标的列表，每个坐标表示裂缝的一个点，坐标格式为 [(x, y),...]。
+    """
+    contours = measure.find_contours(binary_image, level=128, fully_connected='low', positive_orientation='low')
+    contours_xy = [np.fliplr(np.vstack(contour)).astype(np.int32) for contour in contours]
+    return contours_xy
+
+def drawOutline(blackbackground, contours, color=Z.purple, thickness=1):
+    """绘制轮廓"""
+    cv2.drawContours(blackbackground, contours, -1, color, thickness=thickness)
+
+def gradientOutline(img, radius=2):
+    """
+    对图像进行梯度边缘检测，并返回边缘强度图像。
+    
+    :param img: 输入的图像(内部有二值转化)
+    :param radius: 半径,默认为2。
+    :return: 返回经过梯度边缘检测处理后的边缘强度图像
+    """
+    image = BinaryImg(img)
+    denoised = rank.median(image, disk(radius))
+    gradient = rank.gradient(denoised, disk(radius))
+    gradient = cv2.cvtColor(gradient, cv2.COLOR_GRAY2BGR)
 
+    return gradient
```

### Comparing `pyzjr-1.3.8/pyzjr/visualize/video_utils.py` & `pyzjr-1.3.9/pyzjr/visualize/video_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             "Mp4toGif",
            ]
 
 class VideoCap():
     """
     Customized Python video reading class
     """
-    def CapInit(self, mode=0, w=640, h=480, l=150):
+    def __init__(self, mode=0, w=640, h=480, l=150):
         self.cap = cv2.VideoCapture(mode)
         self.cap.set(3, w)
         self.cap.set(4, h)
         self.cap.set(10, l)
 
     def read(self, flip=None):
         """
@@ -87,15 +87,14 @@
         return sum(self.times)
     def cumsum(self):
         """Accumulated sum of time from the previous n runs"""
         return np.array(self.times).cumsum().tolist()
 
 
 def Mp4toGif(mp4, name='result.gif', fps=10, start=None, end=None):
-
     cap = cv2.VideoCapture(mp4)
     all_images = []
     frame_count = 0
 
     while True:
         ret, img = cap.read()
         if ret is False:
@@ -106,22 +105,21 @@
         if end is not None and frame_count >= end:
             break
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         all_images.append(img)
         frame_count += 1
 
     duration = int(1000 / fps)  # 将帧率转换为每帧之间的延迟时间（毫秒）
-    gif = imageio.mimsave(name, all_images, duration=duration)
+    imageio.mimsave(name, all_images, duration=duration)
     print("转换完成！")
 
 if __name__ == "__main__":
     import pyzjr.Z as Z
     fpsReader = FPS()
-    Vcap = VideoCap()
-    Vcap.CapInit(mode=0)
+    Vcap = VideoCap(mode=0)
     while True:
         img = Vcap.read()
         fps, img = fpsReader.update(img)
         cv2.imshow("Image", img)
         k = cv2.waitKey(1)
         if k == Z.Esc:
             break
```

### Comparing `pyzjr-1.3.8/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.3.9/pyzjr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.8
+Version: 1.3.9
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.8/pyzjr.egg-info/SOURCES.txt` & `pyzjr-1.3.9/pyzjr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 LICENSE
 README.md
 setup.py
+models_img/Crack.py
 models_img/__init__.py
-pyzjr/PIC.py
+models_img/test_crack_measure/__init__.py
+models_img/test_crack_measure/crack_type.py
+models_img/test_crack_measure/pixel.py
+models_img/test_crack_measure/skeleton_extraction.py
+models_img/test_crack_measure/test.py
 pyzjr/Z.py
 pyzjr/__init__.py
 pyzjr/version.py
 pyzjr.egg-info/PKG-INFO
 pyzjr.egg-info/SOURCES.txt
 pyzjr.egg-info/dependency_links.txt
 pyzjr.egg-info/requires.txt
@@ -137,23 +142,19 @@
 pyzjr/Models/sampling/medianpooling.py
 pyzjr/Models/sampling/standardpooling.py
 pyzjr/Models/sampling/strideconv.py
 pyzjr/Models/sampling/strippooling.py
 pyzjr/Models/segmentation/__init__.py
 pyzjr/Models/segmentation/fcn.py
 pyzjr/Models/segmentation/unet.py
+pyzjr/augmentation/PIC.py
 pyzjr/augmentation/__init__.py
 pyzjr/augmentation/augments.py
-pyzjr/augmentation/utils.py
-pyzjr/augmentation/Pixel/Crack.py
-pyzjr/augmentation/Pixel/_Steger.py
-pyzjr/augmentation/Pixel/__init__.py
-pyzjr/augmentation/Pixel/definition.py
-pyzjr/augmentation/Pixel/pixel.py
-pyzjr/augmentation/Pixel/utils.py
+pyzjr/augmentation/blur.py
+pyzjr/augmentation/mask_ops.py
 pyzjr/augmentation/transforms/__init__.py
 pyzjr/augmentation/transforms/_utils.py
 pyzjr/augmentation/transforms/normal.py
 pyzjr/augmentation/transforms/opencv.py
 pyzjr/augmentation/transforms/pillow.py
 pyzjr/augmentation/transforms/tvision.py
 pyzjr/core/__init__.py
@@ -170,29 +171,40 @@
 pyzjr/data/FM.py
 pyzjr/data/__init__.py
 pyzjr/data/basedataset.py
 pyzjr/data/dataloader.py
 pyzjr/data/dataset.py
 pyzjr/data/reader.py
 pyzjr/data/txt_utils.py
+pyzjr/data/yaml_utils.py
 pyzjr/data/data_set/Pascal_voc.py
 pyzjr/data/data_set/__init__.py
 pyzjr/data/data_set/config.py
 pyzjr/devices/__init__.py
 pyzjr/devices/get_device.py
 pyzjr/devices/measures.py
 pyzjr/devices/systeminfo.py
 pyzjr/dlearn/__init__.py
 pyzjr/dlearn/callbacklog.py
 pyzjr/dlearn/callbacks.py
-pyzjr/dlearn/savemodels.py
+pyzjr/dlearn/save_pth.py
 pyzjr/dlearn/strategy.py
 pyzjr/dlearn/tools.py
 pyzjr/dlearn/trainer.py
 pyzjr/math/__init__.py
+pyzjr/measure/__init__.py
+pyzjr/measure/pixel.py
+pyzjr/measure/steger.py
+pyzjr/measure/crack/__init__.py
+pyzjr/measure/crack/attribute.py
+pyzjr/measure/crack/crack_type.py
+pyzjr/measure/crack/skeleton_extraction.py
+pyzjr/measure/dehaze/__init__.py
+pyzjr/measure/dehaze/eval_definition.py
+pyzjr/measure/dehaze/vague.py
 pyzjr/nn/Summary.py
 pyzjr/nn/__init__.py
 pyzjr/nn/functional.py
 pyzjr/nn/Metrics/__init__.py
 pyzjr/nn/Metrics/classification.py
 pyzjr/nn/Metrics/indexutils.py
 pyzjr/nn/Metrics/medical_index.py
@@ -206,25 +218,24 @@
 pyzjr/nn/torchutils/loss_utils.py
 pyzjr/torch3D/__init__.py
 pyzjr/torch3D/networks/__init__.py
 pyzjr/torch3d/__init__.py
 pyzjr/torch3d/networks/__init__.py
 pyzjr/torch3d/networks/basic_unet.py
 pyzjr/torch3d/networks/dscnet.py
-pyzjr/torch3d/networks/vent.py
+pyzjr/torch3d/networks/vnet.py
 pyzjr/torch3d/networks/block/DSConv.py
 pyzjr/torch3d/networks/block/__init__.py
 pyzjr/torch3d/nii/__init__.py
 pyzjr/torch3d/nii/mri.py
 pyzjr/torch3d/nii/nifti_dataset.py
 pyzjr/torch3d/nii/nii_utils.py
 pyzjr/visualize/__init__.py
 pyzjr/visualize/io.py
 pyzjr/visualize/printf.py
-pyzjr/visualize/utils.py
 pyzjr/visualize/video_utils.py
 pyzjr/visualize/color/__init__.py
 pyzjr/visualize/color/colormap.py
 pyzjr/visualize/color/colorspace.py
 pyzjr/visualize/color/cvplot.py
 pyzjr/visualize/color/findcolor.py
 pyzjr/visualize/color/hex.py
```

### Comparing `pyzjr-1.3.8/setup.py` & `pyzjr-1.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # from pyzjr.version import __version__
-VERSION = "1.3.8"
+VERSION = "1.3.9"
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
@@ -45,14 +45,15 @@
         'matplotlib',
         'mediapipe',
         'scikit-image',
         'thop',
         'argparse',
         'torch',
         'einops',
+        'pyyaml',
         'tensorboard',
         'pytorch_wavelets',
         'opencv-python',
         'torchvision',
         'nibabel',
     ],
     keywords=['python', 'computer vision', 'pyzjr','windows'],
```

