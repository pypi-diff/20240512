# Comparing `tmp/mrsegmentator-1.0.1.tar.gz` & `tmp/mrsegmentator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsegmentator-1.0.1.tar", last modified: Mon Apr 15 14:34:27 2024, max compression
+gzip compressed data, was "mrsegmentator-1.0.2.tar", last modified: Sun May 12 14:50:24 2024, max compression
```

## Comparing `mrsegmentator-1.0.1.tar` & `mrsegmentator-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-04-15 14:34:27.666311 mrsegmentator-1.0.1/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     6481 2024-04-15 14:34:27.662405 mrsegmentator-1.0.1/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5451 2024-04-15 14:21:20.000000 mrsegmentator-1.0.1/README.md
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.1/pyproject.toml
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1633 2024-04-15 14:34:27.672747 mrsegmentator-1.0.1/setup.cfg
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-04-15 14:34:27.513975 mrsegmentator-1.0.1/src/
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-04-15 14:34:27.586816 mrsegmentator-1.0.1/src/mrsegmentator/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.1/src/mrsegmentator/__init__.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5396 2024-04-15 14:21:20.000000 mrsegmentator-1.0.1/src/mrsegmentator/inference.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2898 2024-04-15 14:21:20.000000 mrsegmentator-1.0.1/src/mrsegmentator/main.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3742 2024-04-15 13:01:27.000000 mrsegmentator-1.0.1/src/mrsegmentator/parser.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3368 2024-02-27 15:48:22.000000 mrsegmentator-1.0.1/src/mrsegmentator/simpleitk_reader_writer.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2455 2024-04-15 13:01:32.000000 mrsegmentator-1.0.1/src/mrsegmentator/utils.py
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-04-15 14:34:27.652897 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     6481 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      469 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/SOURCES.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/dependency_links.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/entry_points.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       25 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/requires.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-04-15 14:34:27.000000 mrsegmentator-1.0.1/src/mrsegmentator.egg-info/top_level.txt
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.827567 mrsegmentator-1.0.2/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 14:50:24.823523 mrsegmentator-1.0.2/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4531 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/README.md
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.2/pyproject.toml
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1660 2024-05-12 14:50:24.833344 mrsegmentator-1.0.2/setup.cfg
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.682407 mrsegmentator-1.0.2/src/
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.755658 mrsegmentator-1.0.2/src/mrsegmentator/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.2/src/mrsegmentator/__init__.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4111 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/config.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4749 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/inference.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1427 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/main.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3378 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/parser.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3236 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/simpleitk_reader_writer.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2516 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/utils.py
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.814283 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      497 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/SOURCES.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/dependency_links.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/entry_points.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       25 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/requires.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/top_level.txt
```

### Comparing `mrsegmentator-1.0.1/PKG-INFO` & `mrsegmentator-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsegmentator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 Home-page: https://github.com/hhaentze/mrsegmentator
 Author: Hartmut Häntze
 Author-email: hartmut.haentze@charite.de
 Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
 Project-URL: repository, https://github.com/hhaentze/mrsegmentator
 Classifier: Programming Language :: Python :: 3
@@ -33,84 +33,69 @@
 </div>
 
 > Detect and segment 40 classes in MRI scans of the abdominal / pelvic / thorax region
 
 
 Contrary to CT scans, where tools for automatic multi-structure segmentation are quite mature, segmentation tasks in MRI scans are often either focused on the brain region or on a subset of few organs in other body regions. MRSegmentator aims to extend this and accurately segment 40 organs and structures in human MRI scans of the abdominal, pelvic and thorax regions. The segmentation works well on different sequence types, including T1- and T2-weighted, Dixon sequences and even CT images.
 
-![Sample Image](images/MRSegmentator.png)
+![Sample Image](images/SampleSegmentation.png)
 
 ## Installation
 1. Install [PyTorch](https://pytorch.org/get-started/locally/) based on your system requirements
 2. Install MRSegmentator with pip 
-3. Download the weights and extract them into your model directory
 
 Example workflow:
 ```bash
 # Create virtual environment
 conda create -n mrseg python=3.11 pip
 conda activate mrseg
 
-# Install pytorch
-conda  install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -c pytorch -c nvidia
+# Install PyTorch (will be different on your system, please refer to the PyTorch documentation)
+conda install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -c pytorch -c nvidia
 
 # Install MRSegmentator
-python -m pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple mrsegmentator
+python -m pip install mrsegmentator
 
 # Inference
-mrsegmentator  \
---modeldir "/sc-projects/sc-proj-cc06-ag-ki-radiologie/Niere/ukbb/ckpts/mr_segmentator_weights/" \
---input <nifti file or directory> \
---outdir <directory> 
-
-# Download Weights (TODO) (Currently the weights are stored on the cluster)
-# wget https://www.url-placeholder.de/weights.zip
-# unzip weights.zip
+mrsegmentator --input <nifti file or directory>
 ```
 
 ## Inference
-MRSegmentator segments all .nii and .nii.gz files in an input directory and writes segmentations to the specified output directory. MRSegmentator was trained on images in LPS orientation and automatically transforms input images accordingly. Afterwards, the segmenation's orientation will be changed back to match the original image. If you are certain that your images are in the LPS orientation you can skip this preoprocessing step by setting the ```--is_LPS``` flag (this significantly reduces runtime). MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions when used on very large images (e.g. some CT scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2. Be aware that this increases runtime and possibly reduces segmentation performance.
+MRSegmentator segments all .nii and .nii.gz files in an input directory and writes segmentations to the specified output directory. MRSegmentator was trained on images in LPS orientation and automatically transforms input images accordingly. Afterwards, the segmenation's orientation will be changed back to match the original image. MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions when used on very large images (e.g. some CT scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2. Be aware that this increases runtime and possibly reduces segmentation performance.
 
 ```bash
-mrsegmentator --modeldir <model directory> \
-    --input <input directory or file> \
-    --outdir <output directory> 
+mrsegmentator --input <nifti file or directory>
 ```
 
 Options:
 ```bash
---modeldir <str> [required]  # model directory
---input <str> [required] # input directory or file
---outdir <str> [required] # output directory
+-i, --input <str> [required] # input directory or file
 
+--outdir <str>  # output directory
 --fold <int> # use only a single model for inference 
---crossval # Run all 5 models individually. Useful to analyse differences between the models.
+--postfix <str> # postfix that will be added to segmentations, default: "seg"
+--split_level <int> # split images to reduce memory usage. Images are split recusively: A split level of x will produce 2^x smaller images.
 
---is_LPS # if your images are in LPS orientation you can set this flag to skip one preprocessing step. This decreases runtime
---postfix <str> # postfix that will be added to segmentations. Default: "seg"
---cpu_only # don't use a gpu
---verbose
---batchsize <int> # how many images can be loaded to memory at the same time, ideally this should equal the dataset size
+--batchsize <int> # how many images can be loaded to memory at the same time, default: 8
 --nproc <int> # number of processes
 --nproc_export <int> # number of processes for exporting the segmentations
---split_level <int> # split images to reduce memory usage. Images are split recusively: A split level of x will produce 2^x smaller images.
+--cpu_only # don't use a gpu
+--verbose
 ```
 
 ## Python API
 ```python
 from mrsegmentator import inference
 import os
 
-modeldir = "mrseg_weights"
 outdir = "outputdir"
 images = [f.path for f in os.scandir("image_dir")]
 folds = [0]
 
-inference.infer(modeldir, outdir, images, folds)
-
+inference.infer(images, outdir, folds)
 ```
 
 
 ## Class details
 
 |Index|Class|
 | :-------- | :------- |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.1 Summary: Robust Multi-
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.2 Summary: Robust Multi-
 Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
 github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
 hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
 hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
 hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
@@ -20,60 +20,48 @@
 region Contrary to CT scans, where tools for automatic multi-structure
 segmentation are quite mature, segmentation tasks in MRI scans are often either
 focused on the brain region or on a subset of few organs in other body regions.
 MRSegmentator aims to extend this and accurately segment 40 organs and
 structures in human MRI scans of the abdominal, pelvic and thorax regions. The
 segmentation works well on different sequence types, including T1- and T2-
 weighted, Dixon sequences and even CT images. ![Sample Image](images/
-MRSegmentator.png) ## Installation 1. Install [PyTorch](https://pytorch.org/
-get-started/locally/) based on your system requirements 2. Install
-MRSegmentator with pip 3. Download the weights and extract them into your model
-directory Example workflow: ```bash # Create virtual environment conda create -
-n mrseg python=3.11 pip conda activate mrseg # Install pytorch conda install
-pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -
-c pytorch -c nvidia # Install MRSegmentator python -m pip install -i https://
-test.pypi.org/simple/ --extra-index-url https://pypi.org/simple mrsegmentator #
-Inference mrsegmentator \ --modeldir "/sc-projects/sc-proj-cc06-ag-ki-
-radiologie/Niere/ukbb/ckpts/mr_segmentator_weights/" \ --input \ --outdir #
-Download Weights (TODO) (Currently the weights are stored on the cluster) #
-wget https://www.url-placeholder.de/weights.zip # unzip weights.zip ``` ##
-Inference MRSegmentator segments all .nii and .nii.gz files in an input
-directory and writes segmentations to the specified output directory.
-MRSegmentator was trained on images in LPS orientation and automatically
-transforms input images accordingly. Afterwards, the segmenation's orientation
-will be changed back to match the original image. If you are certain that your
-images are in the LPS orientation you can skip this preoprocessing step by
-setting the ```--is_LPS``` flag (this significantly reduces runtime).
-MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions
-when used on very large images (e.g. some CT scans). You can reduce memory
-usage by setting ```--split_level``` to 1 or 2. Be aware that this increases
-runtime and possibly reduces segmentation performance. ```bash mrsegmentator --
-modeldir \ --input [                    ]\ --outdir ``` Options: ```bash --
-modeldir [required] # model directory --input [required] # input directory or
-file --outdir [required] # output directory --fold # use only a single model
-for inference --crossval # Run all 5 models individually. Useful to analyse
-differences between the models. --is_LPS # if your images are in LPS
-orientation you can set this flag to skip one preprocessing step. This
-decreases runtime --postfix # postfix that will be added to segmentations.
-Default: "seg" --cpu_only # don't use a gpu --verbose --batchsize # how many
-images can be loaded to memory at the same time, ideally this should equal the
-dataset size --nproc # number of processes --nproc_export # number of processes
-for exporting the segmentations --split_level # split images to reduce memory
+SampleSegmentation.png) ## Installation 1. Install [PyTorch](https://
+pytorch.org/get-started/locally/) based on your system requirements 2. Install
+MRSegmentator with pip Example workflow: ```bash # Create virtual environment
+conda create -n mrseg python=3.11 pip conda activate mrseg # Install PyTorch
+(will be different on your system, please refer to the PyTorch documentation)
+conda install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-
+cuda=11.7 -c pytorch -c nvidia # Install MRSegmentator python -m pip install
+mrsegmentator # Inference mrsegmentator --input ``` ## Inference MRSegmentator
+segments all .nii and .nii.gz files in an input directory and writes
+segmentations to the specified output directory. MRSegmentator was trained on
+images in LPS orientation and automatically transforms input images
+accordingly. Afterwards, the segmenation's orientation will be changed back to
+match the original image. MRSegmentator requires a lot of memory and can run
+into OutOfMemory exceptions when used on very large images (e.g. some CT
+scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2.
+Be aware that this increases runtime and possibly reduces segmentation
+performance. ```bash mrsegmentator --input ``` Options: ```bash -i, --input
+[required] # input directory or file --outdir # output directory --fold # use
+only a single model for inference --postfix # postfix that will be added to
+segmentations, default: "seg" --split_level # split images to reduce memory
 usage. Images are split recusively: A split level of x will produce 2^x smaller
-images. ``` ## Python API ```python from mrsegmentator import inference import
-os modeldir = "mrseg_weights" outdir = "outputdir" images = [f.path for f in
-os.scandir("image_dir")] folds = [0] inference.infer(modeldir, outdir, images,
-folds) ``` ## Class details |Index|Class| | :-------- | :------- | | 0 |
-background | | 1 | spleen | | 2 | right_kidney | | 3 | left_kidney | | 4 |
-gallbladder | | 5 | liver | | 6 | stomach | | 7 | pancreas | | 8 |
-right_adrenal_gland | | 9 | left_adrenal_gland | | 10 | left_lung | | 11 |
-right_lung | | 12 | heart | | 13 | aorta | | 14 | inferior_vena_cava | | 15 |
-portal_vein_and_splenic_vein | | 16 | left_iliac_artery | | 17 |
-right_iliac_artery | | 18 | left_iliac_vena | | 19 | right_iliac_vena | | 20 |
-esophagus | | 21 | small_bowel | | 22 | duodenum | | 23 | colon | | 24 |
-urinary_bladder | | 25 | spine | | 26 | sacrum | | 27 | left_hip | | 28 |
-right_hip | | 29 | left_femur | | 30 | right_femur | | 31 |
+images. --batchsize # how many images can be loaded to memory at the same time,
+default: 8 --nproc # number of processes --nproc_export # number of processes
+for exporting the segmentations --cpu_only # don't use a gpu --verbose ``` ##
+Python API ```python from mrsegmentator import inference import os outdir =
+"outputdir" images = [f.path for f in os.scandir("image_dir")] folds = [0]
+inference.infer(images, outdir, folds) ``` ## Class details |Index|Class| | :--
+------ | :------- | | 0 | background | | 1 | spleen | | 2 | right_kidney | | 3
+| left_kidney | | 4 | gallbladder | | 5 | liver | | 6 | stomach | | 7 |
+pancreas | | 8 | right_adrenal_gland | | 9 | left_adrenal_gland | | 10 |
+left_lung | | 11 | right_lung | | 12 | heart | | 13 | aorta | | 14 |
+inferior_vena_cava | | 15 | portal_vein_and_splenic_vein | | 16 |
+left_iliac_artery | | 17 | right_iliac_artery | | 18 | left_iliac_vena | | 19 |
+right_iliac_vena | | 20 | esophagus | | 21 | small_bowel | | 22 | duodenum | |
+23 | colon | | 24 | urinary_bladder | | 25 | spine | | 26 | sacrum | | 27 |
+left_hip | | 28 | right_hip | | 29 | left_femur | | 30 | right_femur | | 31 |
 left_autochthonous_muscle | | 32 | right_autochthonous_muscle | | 33 |
 left_iliopsoas_muscle | | 34 | right_iliopsoas_muscle | | 35 |
 left_gluteus_maximus | | 36 | right_gluteus_maximus | | 37 |
 left_gluteus_medius | | 38 | right_gluteus_medius | | 39 | left_gluteus_minimus
 | | 40 | right_gluteus_minimus |
```

### Comparing `mrsegmentator-1.0.1/README.md` & `mrsegmentator-1.0.2/src/mrsegmentator.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: mrsegmentator
+Version: 1.0.2
+Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
+Home-page: https://github.com/hhaentze/mrsegmentator
+Author: Hartmut Häntze
+Author-email: hartmut.haentze@charite.de
+Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
+Project-URL: repository, https://github.com/hhaentze/mrsegmentator
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Requires-Dist: nnunetv2==2.2.1
+Requires-Dist: argparse
+
 <h2 align="center"> MRSegmentator: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences </h2>
 
 ***
 
 <div align="center">
 <a href="https://github.com/hhaentze/MRSegmentator/actions"><img alt="Continuous Integration" src="https://github.com/hhaentze/MRSegmentator/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://github.com/hhaentze/MRSegmentator/blob/master/License.txt"><img alt="License: Apache" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>  
@@ -10,84 +33,69 @@
 </div>
 
 > Detect and segment 40 classes in MRI scans of the abdominal / pelvic / thorax region
 
 
 Contrary to CT scans, where tools for automatic multi-structure segmentation are quite mature, segmentation tasks in MRI scans are often either focused on the brain region or on a subset of few organs in other body regions. MRSegmentator aims to extend this and accurately segment 40 organs and structures in human MRI scans of the abdominal, pelvic and thorax regions. The segmentation works well on different sequence types, including T1- and T2-weighted, Dixon sequences and even CT images.
 
-![Sample Image](images/MRSegmentator.png)
+![Sample Image](images/SampleSegmentation.png)
 
 ## Installation
 1. Install [PyTorch](https://pytorch.org/get-started/locally/) based on your system requirements
 2. Install MRSegmentator with pip 
-3. Download the weights and extract them into your model directory
 
 Example workflow:
 ```bash
 # Create virtual environment
 conda create -n mrseg python=3.11 pip
 conda activate mrseg
 
-# Install pytorch
-conda  install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -c pytorch -c nvidia
+# Install PyTorch (will be different on your system, please refer to the PyTorch documentation)
+conda install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -c pytorch -c nvidia
 
 # Install MRSegmentator
-python -m pip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple mrsegmentator
+python -m pip install mrsegmentator
 
 # Inference
-mrsegmentator  \
---modeldir "/sc-projects/sc-proj-cc06-ag-ki-radiologie/Niere/ukbb/ckpts/mr_segmentator_weights/" \
---input <nifti file or directory> \
---outdir <directory> 
-
-# Download Weights (TODO) (Currently the weights are stored on the cluster)
-# wget https://www.url-placeholder.de/weights.zip
-# unzip weights.zip
+mrsegmentator --input <nifti file or directory>
 ```
 
 ## Inference
-MRSegmentator segments all .nii and .nii.gz files in an input directory and writes segmentations to the specified output directory. MRSegmentator was trained on images in LPS orientation and automatically transforms input images accordingly. Afterwards, the segmenation's orientation will be changed back to match the original image. If you are certain that your images are in the LPS orientation you can skip this preoprocessing step by setting the ```--is_LPS``` flag (this significantly reduces runtime). MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions when used on very large images (e.g. some CT scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2. Be aware that this increases runtime and possibly reduces segmentation performance.
+MRSegmentator segments all .nii and .nii.gz files in an input directory and writes segmentations to the specified output directory. MRSegmentator was trained on images in LPS orientation and automatically transforms input images accordingly. Afterwards, the segmenation's orientation will be changed back to match the original image. MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions when used on very large images (e.g. some CT scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2. Be aware that this increases runtime and possibly reduces segmentation performance.
 
 ```bash
-mrsegmentator --modeldir <model directory> \
-    --input <input directory or file> \
-    --outdir <output directory> 
+mrsegmentator --input <nifti file or directory>
 ```
 
 Options:
 ```bash
---modeldir <str> [required]  # model directory
---input <str> [required] # input directory or file
---outdir <str> [required] # output directory
+-i, --input <str> [required] # input directory or file
 
+--outdir <str>  # output directory
 --fold <int> # use only a single model for inference 
---crossval # Run all 5 models individually. Useful to analyse differences between the models.
+--postfix <str> # postfix that will be added to segmentations, default: "seg"
+--split_level <int> # split images to reduce memory usage. Images are split recusively: A split level of x will produce 2^x smaller images.
 
---is_LPS # if your images are in LPS orientation you can set this flag to skip one preprocessing step. This decreases runtime
---postfix <str> # postfix that will be added to segmentations. Default: "seg"
---cpu_only # don't use a gpu
---verbose
---batchsize <int> # how many images can be loaded to memory at the same time, ideally this should equal the dataset size
+--batchsize <int> # how many images can be loaded to memory at the same time, default: 8
 --nproc <int> # number of processes
 --nproc_export <int> # number of processes for exporting the segmentations
---split_level <int> # split images to reduce memory usage. Images are split recusively: A split level of x will produce 2^x smaller images.
+--cpu_only # don't use a gpu
+--verbose
 ```
 
 ## Python API
 ```python
 from mrsegmentator import inference
 import os
 
-modeldir = "mrseg_weights"
 outdir = "outputdir"
 images = [f.path for f in os.scandir("image_dir")]
 folds = [0]
 
-inference.infer(modeldir, outdir, images, folds)
-
+inference.infer(images, outdir, folds)
 ```
 
 
 ## Class details
 
 |Index|Class|
 | :-------- | :------- |
@@ -127,8 +135,8 @@
 | 33 | left_iliopsoas_muscle |
 | 34 | right_iliopsoas_muscle |
 | 35 | left_gluteus_maximus |
 | 36 | right_gluteus_maximus |
 | 37 | left_gluteus_medius |
 | 38 | right_gluteus_medius |
 | 39 | left_gluteus_minimus |
-| 40 | right_gluteus_minimus |
+| 40 | right_gluteus_minimus |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,65 +1,67 @@
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.2 Summary: Robust Multi-
+Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
+github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
+hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
+hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
+hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Healthcare Industry Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
+Recognition Classifier: Topic :: Scientific/Engineering :: Medical Science
+Apps. Requires-Python: >=3.11 Description-Content-Type: text/markdown Requires-
+Dist: nnunetv2==2.2.1 Requires-Dist: argparse
  ********** MMRRSSeeggmmeennttaattoorr:: RRoobbuusstt MMuullttii--MMooddaalliittyy SSeeggmmeennttaattiioonn ooff 4400 CCllaasssseess iinn MMRRII
                             aanndd CCTT SSeeqquueenncceess **********
 ***
       _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 > Detect and segment 40 classes in MRI scans of the abdominal / pelvic / thorax
 region Contrary to CT scans, where tools for automatic multi-structure
 segmentation are quite mature, segmentation tasks in MRI scans are often either
 focused on the brain region or on a subset of few organs in other body regions.
 MRSegmentator aims to extend this and accurately segment 40 organs and
 structures in human MRI scans of the abdominal, pelvic and thorax regions. The
 segmentation works well on different sequence types, including T1- and T2-
 weighted, Dixon sequences and even CT images. ![Sample Image](images/
-MRSegmentator.png) ## Installation 1. Install [PyTorch](https://pytorch.org/
-get-started/locally/) based on your system requirements 2. Install
-MRSegmentator with pip 3. Download the weights and extract them into your model
-directory Example workflow: ```bash # Create virtual environment conda create -
-n mrseg python=3.11 pip conda activate mrseg # Install pytorch conda install
-pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -
-c pytorch -c nvidia # Install MRSegmentator python -m pip install -i https://
-test.pypi.org/simple/ --extra-index-url https://pypi.org/simple mrsegmentator #
-Inference mrsegmentator \ --modeldir "/sc-projects/sc-proj-cc06-ag-ki-
-radiologie/Niere/ukbb/ckpts/mr_segmentator_weights/" \ --input \ --outdir #
-Download Weights (TODO) (Currently the weights are stored on the cluster) #
-wget https://www.url-placeholder.de/weights.zip # unzip weights.zip ``` ##
-Inference MRSegmentator segments all .nii and .nii.gz files in an input
-directory and writes segmentations to the specified output directory.
-MRSegmentator was trained on images in LPS orientation and automatically
-transforms input images accordingly. Afterwards, the segmenation's orientation
-will be changed back to match the original image. If you are certain that your
-images are in the LPS orientation you can skip this preoprocessing step by
-setting the ```--is_LPS``` flag (this significantly reduces runtime).
-MRSegmentator requires a lot of memory and can run into OutOfMemory exceptions
-when used on very large images (e.g. some CT scans). You can reduce memory
-usage by setting ```--split_level``` to 1 or 2. Be aware that this increases
-runtime and possibly reduces segmentation performance. ```bash mrsegmentator --
-modeldir \ --input [                    ]\ --outdir ``` Options: ```bash --
-modeldir [required] # model directory --input [required] # input directory or
-file --outdir [required] # output directory --fold # use only a single model
-for inference --crossval # Run all 5 models individually. Useful to analyse
-differences between the models. --is_LPS # if your images are in LPS
-orientation you can set this flag to skip one preprocessing step. This
-decreases runtime --postfix # postfix that will be added to segmentations.
-Default: "seg" --cpu_only # don't use a gpu --verbose --batchsize # how many
-images can be loaded to memory at the same time, ideally this should equal the
-dataset size --nproc # number of processes --nproc_export # number of processes
-for exporting the segmentations --split_level # split images to reduce memory
+SampleSegmentation.png) ## Installation 1. Install [PyTorch](https://
+pytorch.org/get-started/locally/) based on your system requirements 2. Install
+MRSegmentator with pip Example workflow: ```bash # Create virtual environment
+conda create -n mrseg python=3.11 pip conda activate mrseg # Install PyTorch
+(will be different on your system, please refer to the PyTorch documentation)
+conda install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-
+cuda=11.7 -c pytorch -c nvidia # Install MRSegmentator python -m pip install
+mrsegmentator # Inference mrsegmentator --input ``` ## Inference MRSegmentator
+segments all .nii and .nii.gz files in an input directory and writes
+segmentations to the specified output directory. MRSegmentator was trained on
+images in LPS orientation and automatically transforms input images
+accordingly. Afterwards, the segmenation's orientation will be changed back to
+match the original image. MRSegmentator requires a lot of memory and can run
+into OutOfMemory exceptions when used on very large images (e.g. some CT
+scans). You can reduce memory usage by setting ```--split_level``` to 1 or 2.
+Be aware that this increases runtime and possibly reduces segmentation
+performance. ```bash mrsegmentator --input ``` Options: ```bash -i, --input
+[required] # input directory or file --outdir # output directory --fold # use
+only a single model for inference --postfix # postfix that will be added to
+segmentations, default: "seg" --split_level # split images to reduce memory
 usage. Images are split recusively: A split level of x will produce 2^x smaller
-images. ``` ## Python API ```python from mrsegmentator import inference import
-os modeldir = "mrseg_weights" outdir = "outputdir" images = [f.path for f in
-os.scandir("image_dir")] folds = [0] inference.infer(modeldir, outdir, images,
-folds) ``` ## Class details |Index|Class| | :-------- | :------- | | 0 |
-background | | 1 | spleen | | 2 | right_kidney | | 3 | left_kidney | | 4 |
-gallbladder | | 5 | liver | | 6 | stomach | | 7 | pancreas | | 8 |
-right_adrenal_gland | | 9 | left_adrenal_gland | | 10 | left_lung | | 11 |
-right_lung | | 12 | heart | | 13 | aorta | | 14 | inferior_vena_cava | | 15 |
-portal_vein_and_splenic_vein | | 16 | left_iliac_artery | | 17 |
-right_iliac_artery | | 18 | left_iliac_vena | | 19 | right_iliac_vena | | 20 |
-esophagus | | 21 | small_bowel | | 22 | duodenum | | 23 | colon | | 24 |
-urinary_bladder | | 25 | spine | | 26 | sacrum | | 27 | left_hip | | 28 |
-right_hip | | 29 | left_femur | | 30 | right_femur | | 31 |
+images. --batchsize # how many images can be loaded to memory at the same time,
+default: 8 --nproc # number of processes --nproc_export # number of processes
+for exporting the segmentations --cpu_only # don't use a gpu --verbose ``` ##
+Python API ```python from mrsegmentator import inference import os outdir =
+"outputdir" images = [f.path for f in os.scandir("image_dir")] folds = [0]
+inference.infer(images, outdir, folds) ``` ## Class details |Index|Class| | :--
+------ | :------- | | 0 | background | | 1 | spleen | | 2 | right_kidney | | 3
+| left_kidney | | 4 | gallbladder | | 5 | liver | | 6 | stomach | | 7 |
+pancreas | | 8 | right_adrenal_gland | | 9 | left_adrenal_gland | | 10 |
+left_lung | | 11 | right_lung | | 12 | heart | | 13 | aorta | | 14 |
+inferior_vena_cava | | 15 | portal_vein_and_splenic_vein | | 16 |
+left_iliac_artery | | 17 | right_iliac_artery | | 18 | left_iliac_vena | | 19 |
+right_iliac_vena | | 20 | esophagus | | 21 | small_bowel | | 22 | duodenum | |
+23 | colon | | 24 | urinary_bladder | | 25 | spine | | 26 | sacrum | | 27 |
+left_hip | | 28 | right_hip | | 29 | left_femur | | 30 | right_femur | | 31 |
 left_autochthonous_muscle | | 32 | right_autochthonous_muscle | | 33 |
 left_iliopsoas_muscle | | 34 | right_iliopsoas_muscle | | 35 |
 left_gluteus_maximus | | 36 | right_gluteus_maximus | | 37 |
 left_gluteus_medius | | 38 | right_gluteus_medius | | 39 | left_gluteus_minimus
 | | 40 | right_gluteus_minimus |
```

### Comparing `mrsegmentator-1.0.1/setup.cfg` & `mrsegmentator-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mrsegmentator
-version = 1.0.1
+version = 1.0.2
 author = Hartmut Häntze
 author_email = hartmut.haentze@charite.de
 description = Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/hhaentze/mrsegmentator
 project_urls = 
@@ -36,14 +36,15 @@
 	bundles*
 	data*
 	logs*
 	metadata*
 	model*
 	notebooks*
 	scripts*
+	src/mrsegmentator/weights
 
 [options.entry_points]
 console_scripts = 
 	mrsegmentator = mrsegmentator.main:main
 
 [flake8_nb]
 max-line-length = 120
```

### Comparing `mrsegmentator-1.0.1/src/mrsegmentator/inference.py` & `mrsegmentator-1.0.2/src/mrsegmentator/inference.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,94 +8,84 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from mrsegmentator import utils  # isort:skip
-from mrsegmentator.simpleitk_reader_writer import SimpleITKIO  # isort:skip
-
 import ntpath
+from pathlib import Path
 from typing import List, NoReturn, Tuple, Union
 
 import torch
-from batchgenerators.utilities.file_and_folder_operations import join
-from nnunetv2.inference.predict_from_raw_data import nnUNetPredictor
+
+from mrsegmentator import config, utils
+from mrsegmentator.simpleitk_reader_writer import SimpleITKIO
+
+config.disable_nnunet_path_warnings()
+from batchgenerators.utilities.file_and_folder_operations import join  # noqa: E402
+from nnunetv2.inference.predict_from_raw_data import nnUNetPredictor  # noqa: E402
 
 
 def infer(
-    model_dir: str,
-    outdir: str,
     images: List[str],
+    outdir: str,
     folds: Union[List[int], Tuple[int, ...]],
     postfix: str = "seg",
-    is_LPS: bool = False,
     split_level: int = 0,
     verbose: bool = False,
     cpu_only: bool = False,
     batchsize: int = 3,
     nproc: int = 3,
     nproc_export: int = 8,
 ) -> NoReturn:
     """Run model to create segmentations
-    model_dir: path to model directory
     folds: which models to use for inference
     outdir: path to output directory
     images: list with paths to images
-    is_LPS: do not change orientation to LPS before inference"""
+    postfix: default='seg'
+    split_level: split images to reduce memory footprint
+    """
+
+    # initialize weights directory
+    config.setup_mrseg()
+
+    # make output directory
+    Path(outdir).mkdir(exist_ok=True)
 
     # instantiate the nnUNetPredictor
     predictor = nnUNetPredictor(
         tile_step_size=0.5,
         use_gaussian=True,
         use_mirroring=True,
         device=torch.device("cpu") if cpu_only else torch.device("cuda", 0),
         verbose=verbose,
         verbose_preprocessing=verbose,
         allow_tqdm=True,
     )
 
     # initialize the network architecture, load the checkpoints
     predictor.initialize_from_trained_model_folder(
-        model_dir,
+        config.get_weights_dir(),
         use_folds=folds,
         checkpoint_name="checkpoint_final.pth",
     )
 
-    if split_level == 0 and is_LPS:
-        # paths to output images
-        image_names = [ntpath.basename(f) for f in images]
-        out_names = [utils.add_postfix(name, postfix) for name in image_names]
-
-        # variant 1, use list of files as inputs
-        predictor.predict_from_files(
-            [[f] for f in images],
-            [join(outdir, f) for f in out_names],
-            save_probabilities=False,
-            overwrite=False,
-            num_processes_preprocessing=nproc,
-            num_processes_segmentation_export=nproc_export,
-            folder_with_segs_from_prev_stage=None,
-            num_parts=1,
-            part_id=0,
-        )
+    if split_level == 0:
 
-    elif split_level == 0 and not is_LPS:
         # load batch of images
-        # (Loading all images at once might require too much memory, instead we procede chunk wise)
-        chunk_size = batchsize
-        for i, img_chunk in enumerate(utils.divide_chunks(images, chunk_size)):
+        # (loading all images at once might require too much memory, instead we procede chunk wise)
+        for i, img_chunk in enumerate(utils.divide_chunks(images, batchsize)):
 
             print(
-                f"Processing image { chunk_size*i + 1 } to {chunk_size*i + len(img_chunk)} out of {len(images)} images."
+                f"Processing image { batchsize*i + 1 } to {batchsize*i + len(img_chunk)} out of {len(images)} images."
             )
 
             # load images
-            np_chunk = [SimpleITKIO().read_image(f, is_LPS=is_LPS, verbose=True) for f in img_chunk]
+            np_chunk = [SimpleITKIO().read_image(f, verbose=True) for f in img_chunk]
             imgs = [f[0] for f in np_chunk]
             props = [f[1] for f in np_chunk]
 
             # inference
             segmentations = predictor.predict_from_list_of_npy_arrays(
                 imgs,
                 None,
@@ -108,23 +98,23 @@
 
             # paths to output images
             image_names = [ntpath.basename(f) for f in img_chunk]
             out_names = [utils.add_postfix(name, postfix) for name in image_names]
 
             # save images
             for seg, p, out in zip(segmentations, props, out_names):
-                SimpleITKIO().write_seg(seg, join(outdir, out), p, is_LPS=is_LPS, verbose=True)
+                SimpleITKIO().write_seg(seg, join(outdir, out), p, verbose=True)
 
     else:
         # sequential inference (parallelization would increase memory)
         for i, img in enumerate(images):
 
             # load image
             print(f"Processing image { i + 1 } out of {len(images)} images.")
-            np_img, prop = SimpleITKIO().read_image(img, is_LPS=is_LPS, verbose=True)
+            np_img, prop = SimpleITKIO().read_image(img, verbose=True)
 
             # split image to reduce memory usage
             np_imgs = [np_img]
             for _ in range(split_level):
                 np_imgs = utils.flatten([utils.split_image(n) for n in np_imgs])
 
             # infer
@@ -140,10 +130,8 @@
                     for _i in range(0, len(segmentations), 2)
                 ]
 
             # paths to output image
             out_name = utils.add_postfix(ntpath.basename(img), postfix)
 
             # save image
-            SimpleITKIO().write_seg(
-                segmentations[0], join(outdir, out_name), prop, is_LPS=is_LPS, verbose=True
-            )
+            SimpleITKIO().write_seg(segmentations[0], join(outdir, out_name), prop, verbose=True)
```

### Comparing `mrsegmentator-1.0.1/src/mrsegmentator/parser.py` & `mrsegmentator-1.0.2/src/mrsegmentator/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,47 +9,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
+import logging
 import os
 
+logger = logging.getLogger(__name__)
+
 
 def initialize():
     name = "MRSegmentator"
     desc = "Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences"
     epilog = "Charité AG KI - 2024"
 
     parser = argparse.ArgumentParser(prog=name, description=desc, epilog=epilog)
 
-    parser.add_argument("--modeldir", type=str, required=True, help="model directory")
-    parser.add_argument("--outdir", type=str, required=True, help="output directory")
     parser.add_argument(
         "-i",
         "--input",
         type=str,
         required=True,
         help="input image or directory with nifti images",
     )
+
+    parser.add_argument("--outdir", type=str, default="segmentations", help="output directory")
+
     parser.add_argument(
         "--fold",
         type=int,
         choices=range(5),
         help="choose a model based on the validation folds",
     )
-    parser.add_argument("--crossval", action="store_true", help="run each model individually")
 
     parser.add_argument(
-        "--is_LPS",
-        action="store_true",
-        help="if your images are in LPS orientation you can set this flag to skip one preprocessing step. This decreases runtime",  # noqa: E501
-    )
-    parser.add_argument(
         "--batchsize",
         type=int,
         default=8,
         help="how many images can be loaded to memory at the same time, ideally this should equal the dataset size",
     )
     parser.add_argument(
         "--nproc",
@@ -75,26 +73,27 @@
 
     args = parser.parse_args()
     return args
 
 
 def assert_namespace(namespace):
     # requirements
-    assert os.path.isdir(namespace.modeldir), f"Model directory {namespace.modeldir} not found"
-    assert os.path.isdir(namespace.outdir), f"Output directory {namespace.outdir} not found"
+    if namespace.outdir != "segmentations":
+        assert os.path.isdir(namespace.outdir), f"Output directory {namespace.outdir} not found"
     assert os.path.isfile(namespace.input) or os.path.isdir(
         namespace.input
     ), f"Input {namespace.input} not found"
 
     # constraints
     assert namespace.batchsize >= 1, "batchsize must be greater than 1"
     assert namespace.nproc >= 1, "number of processes must be greater than 1"
     assert (
         namespace.nproc_export >= 1
     ), "number of processes for image export must be greater than 1"
     assert namespace.split_level >= 0, "split level must be equal or greather than zero"
 
     # warnings
     if namespace.split_level >= 3:
-        print(
-            f"Warning: Based on the specified split level of {namespace.split_level} images will be cut into 2^{namespace.split_level}={pow(2,namespace.split_level)} smaller images. Are you sure this is intended?"  # noqa: E501
+        logger.warning(
+            f"Warning: Based on the specified split level of {namespace.split_level} images will be cut into 2^{namespace.split_level}={pow(2,namespace.split_level)} smaller images. "  # noqa: E501
+            + "Are you sure this is intended?"
         )
```

### Comparing `mrsegmentator-1.0.1/src/mrsegmentator/simpleitk_reader_writer.py` & `mrsegmentator-1.0.2/src/mrsegmentator/simpleitk_reader_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,32 +20,29 @@
 
 
 class SimpleITKIO:
 
     def read_image(
         self,
         image_fname: str,
-        is_LPS: bool = False,
         verbose: bool = False,
     ) -> Tuple[np.ndarray, dict]:
 
         if verbose:
             print(f"Read {image_fname}")
 
         # read image and save meta data
         itk_image = sitk.ReadImage(image_fname)
         spacing = itk_image.GetSpacing()
         origin = itk_image.GetOrigin()
         direction = itk_image.GetDirection()
         itk_image = sitk.DICOMOrient(itk_image, "LPS")
-        if is_LPS:
-            orientation = "LPS"
-        else:
-            nib_image = nib.load(image_fname)
-            orientation = "".join(nib.aff2axcodes(nib_image.affine))
+
+        nib_image = nib.load(image_fname)
+        orientation = "".join(nib.aff2axcodes(nib_image.affine))
 
         # transform image to numpy array
         npy_image = sitk.GetArrayFromImage(itk_image)
         assert (
             npy_image.ndim == 3
         ), f"Unexpected number of dimensions: {npy_image.ndim} in file {image_fname}"
         npy_image = npy_image[None]
@@ -69,15 +66,14 @@
         return self.read_image(seg_fname)
 
     def write_seg(
         self,
         seg: np.ndarray,
         output_fname: str,
         properties: dict,
-        is_LPS: bool = False,
         verbose: bool = False,
     ) -> None:
 
         assert (
             seg.ndim == 3
         ), "segmentation must be 3d. If you are exporting a 2d segmentation, please provide it as shape 1,x,y"
         if verbose:
```

### Comparing `mrsegmentator-1.0.1/src/mrsegmentator/utils.py` & `mrsegmentator-1.0.2/src/mrsegmentator/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from pathlib import Path
-from typing import List, NoReturn, Tuple
+from typing import List, Tuple
 
 import numpy as np
 
 
+def read_images(namespace):
+    # images must be of nifti format
+    condition = lambda x: x[-7:] == ".nii.gz" or x[-4:] == ".nii"
+
+    # look for images in input directory
+    if os.path.isdir(namespace.input):
+        images = [f.path for f in os.scandir(namespace.input) if condition(f.name)]
+        assert (
+            len(images) > 0
+        ), f"no images with file ending .nii or .nii.gz in direcotry {namespace.input}"
+    else:
+        images = [namespace.input]
+        assert condition(images[0]), f"file ending of {namespace.input} neither .nii nor .nii.gz"
+
+    return images
+
+
 # Yield successive n-sized
 # chunks from l.
 def divide_chunks(l: List, n: int):  # noqa: E741
     # looping till length l
     for i in range(0, len(l), n):
         yield l[i : i + n]
 
@@ -57,22 +74,7 @@
     seg_combined = np.concatenate([seg1, seg2], axis=0)
 
     return seg_combined
 
 
 def flatten(xss: List[List]) -> List:
     return [x for xs in xss for x in xs]
-
-
-def disable_nnunet_path_warnings() -> NoReturn:
-    """disable warning message about undefined environmental variables
-    (We assign temporary arbitrary values. The script does not use these)"""
-
-    if os.environ.get("nnUNet_raw") is None:
-        os.environ["nnUNet_raw"] = "empty"
-    if os.environ.get("nnUNet_preprocessed") is None:
-        os.environ["nnUNet_preprocessed"] = "empty"
-    if os.environ.get("nnUNet_results") is None:
-        os.environ["nnUNet_results"] = "empty"
-
-
-disable_nnunet_path_warnings()
```

