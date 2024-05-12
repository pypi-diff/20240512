# Comparing `tmp/HiFT-0.0.1.tar.gz` & `tmp/HiFT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiFT-0.0.1.tar", last modified: Wed May  1 15:37:59 2024, max compression
+gzip compressed data, was "dist/HiFT-0.0.2.tar", last modified: Sun May 12 21:39:57 2024, max compression
```

## Comparing `HiFT-0.0.1.tar` & `HiFT-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,54 @@
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-01 15:37:59.299992 HiFT-0.0.1/
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-01 15:37:59.112000 HiFT-0.0.1/HiFT.egg-info/
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-01 15:37:59.000000 HiFT-0.0.1/HiFT.egg-info/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)      571 2024-05-01 15:37:59.000000 HiFT-0.0.1/HiFT.egg-info/SOURCES.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-01 15:37:59.000000 HiFT-0.0.1/HiFT.egg-info/dependency_links.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-01 15:37:59.000000 HiFT-0.0.1/HiFT.egg-info/top_level.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1159 2024-05-01 15:36:00.000000 HiFT-0.0.1/LICENSE.md
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-01 15:37:59.295992 HiFT-0.0.1/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.1/README.md
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-01 15:37:59.135999 HiFT-0.0.1/examples/
--rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-04-29 20:12:46.000000 HiFT-0.0.1/examples/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34489 2024-05-01 13:33:13.000000 HiFT-0.0.1/examples/gpt2_example.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34489 2024-05-01 13:33:34.000000 HiFT-0.0.1/examples/opt_example.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    31579 2024-05-01 13:41:36.000000 HiFT-0.0.1/examples/run_glue.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-01 15:37:59.207996 HiFT-0.0.1/hift/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      132 2024-05-01 13:31:29.000000 HiFT-0.0.1/hift/__init__.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-01 15:37:59.283993 HiFT-0.0.1/hift/optimizers/
--rw-r--r--   0 yongkang (31362) cisintern (30001)       47 2024-04-29 20:36:25.000000 HiFT-0.0.1/hift/optimizers/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14456 2024-04-28 17:45:25.000000 HiFT-0.0.1/hift/optimizers/adagrad.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-04-29 23:18:27.000000 HiFT-0.0.1/hift/optimizers/optimization.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    42967 2024-04-29 23:21:15.000000 HiFT-0.0.1/hift/optimizers/optimizer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     8944 2024-05-01 13:31:18.000000 HiFT-0.0.1/hift/optimizers/replace_operation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-04-28 18:22:31.000000 HiFT-0.0.1/hift/optimizers/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-04-28 18:31:46.000000 HiFT-0.0.1/hift/optimizers/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-04-29 07:39:54.000000 HiFT-0.0.1/hift/optimizers/torchAdam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-04-29 07:46:38.000000 HiFT-0.0.1/hift/optimizers/torchAdamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    13649 2024-05-01 15:24:24.000000 HiFT-0.0.1/hift/registerCallBack.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    17010 2024-04-30 08:42:53.000000 HiFT-0.0.1/hift/seqtrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    39541 2024-05-01 13:20:17.000000 HiFT-0.0.1/hift/trainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-01 15:37:59.299992 HiFT-0.0.1/setup.cfg
--rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-01 15:36:34.000000 HiFT-0.0.1/setup.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.335502 HiFT-0.0.2/
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.303503 HiFT-0.0.2/HiFT.egg-info/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/SOURCES.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/dependency_links.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-12 21:39:57.000000 HiFT-0.0.2/HiFT.egg-info/top_level.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1159 2024-05-01 15:36:00.000000 HiFT-0.0.2/LICENSE.md
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-12 21:39:57.335502 HiFT-0.0.2/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.2/README.md
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.311503 HiFT-0.0.2/examples/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4137 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/build_dataset.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    21928 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/instruct_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/llama2_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.2/examples/llama_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/llama_xformers_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30614 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/pretrain_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    35261 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_generation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    33497 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_glue.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    32290 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_ner.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37349 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/run_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/utils_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    20707 2024-05-12 21:30:42.000000 HiFT-0.0.2/examples/vicuna_train.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.315502 HiFT-0.0.2/hift/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/__init__.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.323502 HiFT-0.0.2/hift/optimizers/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      644 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/adagrad.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.331502 HiFT-0.0.2/hift/optimizers/bitsandbytes/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adagrad.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/adamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lamb.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lars.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/lion.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/bitsandbytes/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/optimization.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/optimizer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    10583 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/replace_operation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/torchAdam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/optimizers/torchAdamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/qatrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    13782 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/registerCallBack.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/seqtrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    65929 2024-05-12 21:35:57.000000 HiFT-0.0.2/hift/trainer.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:39:57.331502 HiFT-0.0.2/hift/utils/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/utils/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.2/hift/utils/utils.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-12 21:39:57.335502 HiFT-0.0.2/setup.cfg
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-12 21:38:15.000000 HiFT-0.0.2/setup.py
```

### Comparing `HiFT-0.0.1/HiFT.egg-info/PKG-INFO` & `HiFT-0.0.2/HiFT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.1/LICENSE.md` & `HiFT-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/PKG-INFO` & `HiFT-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.1/README.md` & `HiFT-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/examples/gpt2_example.py` & `HiFT-0.0.2/examples/run_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,34 +62,27 @@
     TransfoXLConfig,
     XLMTokenizer,
     XLMWithLMHeadModel,
     XLMConfig,
     XLNetLMHeadModel,
     XLNetTokenizer,
     XLNetConfig,
-    Seq2SeqTrainer,
     Seq2SeqTrainingArguments,
     set_seed,
 )
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.trainer_utils import get_last_checkpoint
 from transformers.utils import check_min_version, is_offline_mode, send_example_telemetry
 from transformers.utils.versions import require_version
 from transformers.trainer_pt_utils import LabelSmoother
 
-from peft import (
-    PeftType,
-    LoraConfig,
-    TaskType,
-    get_peft_model
-)
 
 sys.path.append(os.path.abspath('.'))
-
-from hift import HiFTSeq2SeqTrainer,GetCallBack
+from hift import HiFTSeq2SeqTrainer,GetCallBack,peft_function,Seq2SeqTrainer
+from peft import PeftModel
 
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
     datefmt="%m/%d/%Y %H:%M:%S",
     level=logging.INFO,
 )
 logger = logging.getLogger(__name__)
@@ -377,14 +370,35 @@
 
 @dataclass
 class HiFTArguments(ModelArguments):
     HiTaskType: str = field(
         default="CAUSAL_LM",
         metadata={"help": ("HiTaskType should be consistent with PEFT TaskType" )},
     )
+    peft_type: str = field(
+        default=None,
+        metadata={"help": ("peft_type should be in [lora,adalora,ia3,p_tuning,prefix_tuning,prompt_tuning]" )},
+    )
+    init_text:str = field(
+        default="Predict if sentiment of this review is positive, negative or neutral",
+        metadata={
+            "help": (
+                "the init prompt text for prompt tuning"
+            )
+        },
+    )
+    lora_rank: int = field(
+        default=8,
+        metadata={"help": ("rank for lora or adalora" )},
+    )
+    peft_path : Optional[str] = field(default=None)
+    virtual_tokens:int = field(
+        default=20,
+        metadata={"help": ("the number of virtual tokens for p_tuning, prefix_tuning and prefix_tuning" )},
+    )
     group_element: int = field(
         default=1,
         metadata={"help": ("number element for each group parameters" )},
     )
     optimizer_strategy: str = field(
         default="down2up",
         metadata={"help": ("optimizer strategy of ['down2up','down2up','random']" )},
@@ -393,33 +407,23 @@
         default=False,
         metadata={
             "help": (
                 "hierarchical optimization for LLMS"
             )
         },
     )
-    lora_tuning:bool = field(
-        default=False,
-        metadata={
-            "help": (
-                "whether using lora tuning"
-            )
-        },
-    )
     freeze_layers: List[str] = field(
         default_factory=list,
         metadata={
             "help": (
                 "Index of the frozen layer"
             )
         },
     )
 
-
-
 datasets_name_mapping = {
     "amazon_reviews_multi": ("review_body", "review_title"),
     "big_patent": ("description", "abstract"),
     "cnn_dailymail": ("article", "highlights"),
     "orange_sum": ("text", "summary"),
     "pn_summary": ("article", "summary"),
     "psc": ("extract_text", "summary_text"),
@@ -428,14 +432,33 @@
     "xglue": ("news_body", "news_title"),
     "xsum": ("document", "summary"),
     "wiki_summary": ("article", "highlights"),
     "multi_news": ("document", "summary"),
     "e2e_nlg":("meaning_representation", "human_reference"),
 }
 
+class SavePeftModelCallback(transformers.TrainerCallback):
+    def save_model(self, args, state, kwargs):
+        if state.best_model_checkpoint is not None:
+            checkpoint_folder = os.path.join(state.best_model_checkpoint, "peft_model")
+        else:
+            checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
+
+        peft_model_path = os.path.join(checkpoint_folder, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
+
+    def on_save(self, args, state, control, **kwargs):
+        self.save_model(args, state, kwargs)
+        return control
+
+    def on_train_end(self, args, state, control, **kwargs):
+        peft_model_path = os.path.join(args.output_dir, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
     parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
@@ -580,23 +603,30 @@
         model_args.model_name_or_path,
         from_tf=bool(".ckpt" in model_args.model_name_or_path),
         config=config,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
         use_auth_token=True if model_args.use_auth_token else None,
     )
-    if model_args.lora_tuning:
-        peft_config = LoraConfig(
-            peft_type = PeftType.LORA,
-            lora_alpha=16,
-            lora_dropout=0.1,
-            r=8,
-            bias="none",
-            task_type=TaskType.CAUSAL_LM)
-        model = get_peft_model(model, peft_config)
+    if model_args.peft_type:
+        if model_args.peft_path is not None:
+            logger.info("Peft from pre-trained model")
+            model = PeftModel.from_pretrained(model, model_args.peft_path)
+
+        else:
+            model = peft_function(model,
+                    config = config,
+                    peft_type = model_args.peft_type,
+                    task_type = model_args.HiTaskType,
+                    rank=model_args.lora_rank,
+                    virtual_tokens=model_args.virtual_tokens,
+                    tokenizer_name_or_path=model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
+                    init_text=model_args.init_text if model_args.peft_type=="prompt_tuning" else None,
+                    peft_config=None)
+                    
     # We resize the embeddings only when necessary to avoid index errors. If you are creating a model from scratch
     # on a small vocab and want a smaller embedding size, remove this test.
     embedding_size = model.get_input_embeddings().weight.shape[0]
     if len(tokenizer) > embedding_size:
         model.resize_token_embeddings(len(tokenizer))
     model.config.decoder_start_token_id = model.config.bos_token_id
     if model.config.decoder_start_token_id is None:
@@ -727,93 +757,60 @@
     if data_args.max_eval_samples is not None:
         max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
         eval_dataset = eval_dataset.select(range(max_eval_samples))
     with training_args.main_process_first(desc="validation dataset map pre-processing"):
         eval_dataset=eval_dataset.map(
         lambda x : tokenizer(
             list(map(lambda a,b: a + " ### " + b, x[source_column], x[target_column])), 
-            truncation="only_second",
+            truncation="longest_first",
             max_length=tokenizer.model_max_length, 
             padding=padding), 
             batched=True,
             desc="Running tokenizer on validation dataset")
         eval_dataset = train_dataset.map(lambda x: {'labels':x['input_ids']})
     # Data collator
     label_pad_token_id = IGNORE_TOKEN_ID if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id
     data_collator = DataCollatorForSeq2Seq(
         tokenizer,
         model=model,
         label_pad_token_id=label_pad_token_id,
         pad_to_multiple_of=8 if training_args.fp16 else None,
     )
-
-    # Metric
-    metric = evaluate.load("rouge")
-    def postprocess_text(preds, labels):
-        preds = [pred.strip() for pred in preds]
-        labels = [label.strip() for label in labels]
-        # rougeLSum expects newline after each sentence
-        preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in preds]
-        labels = ["\n".join(nltk.sent_tokenize(label)) for label in labels]
-        return preds, labels
-
-    def compute_metrics(eval_preds):
-        preds, labels = eval_preds
-        if isinstance(preds, tuple):
-            preds = preds[0]
-        # Replace -100s used for padding as we can't decode them
-        preds = np.where(preds != IGNORE_TOKEN_ID, preds, tokenizer.pad_token_id)
-        decoded_preds = tokenizer.batch_decode(preds, skip_special_tokens=True)
-        labels = np.where(labels != IGNORE_TOKEN_ID, labels, tokenizer.pad_token_id)
-        decoded_labels = tokenizer.batch_decode(labels, skip_special_tokens=True)
-
-        # Some simple post-processing
-        decoded_preds, decoded_labels = postprocess_text(decoded_preds, decoded_labels)
-        result = metric.compute(predictions=decoded_preds, references=decoded_labels, use_stemmer=True)
-        result = {k: round(v * 100, 4) for k, v in result.items()}
-        prediction_lens = [np.count_nonzero(pred != tokenizer.pad_token_id) for pred in preds]
-        result["gen_len"] = np.mean(prediction_lens)
-        return result
-    training_args.generation_max_length = (
-        training_args.generation_max_length
-        if training_args.generation_max_length is not None
-        else data_args.val_max_target_length
-    )
-    training_args.generation_num_beams = (
-        data_args.num_beams if data_args.num_beams is not None else training_args.generation_num_beams
-    )
+     
     # Initialize our Trainer
     if model_args.hier_tuning:#hier_tuning
         trainer = HiFTSeq2SeqTrainer(
             hiFThandler = GetCallBack(model_args.model_name_or_path),
             HiTaskType = model_args.HiTaskType,
             group_element = model_args.group_element,
             strategy = model_args.optimizer_strategy,
             hier_tuning= model_args.hier_tuning,
-            lora_tuning = model_args.lora_tuning,
+            peft_type = model_args.peft_type,
             freeze_layers = model_args.freeze_layers,
+            args=training_args,
             model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             compute_metrics=compute_metrics if training_args.predict_with_generate else None,
             tokenizer=tokenizer,
-            data_collator=data_collator,
-            args=training_args
+            data_collator=data_collator
         )
     else:
         trainer = Seq2SeqTrainer(
-            model=model,
+            peft_type = model_args.peft_type,
             args=training_args,
+            model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             tokenizer=tokenizer,
             data_collator=data_collator,
             compute_metrics=compute_metrics if training_args.predict_with_generate else None,
         )
-
+    if model_args.peft_type:
+        trainer.add_callback(SavePeftModelCallback)
     # Training
     checkpoint = None
     if training_args.resume_from_checkpoint is not None:
         checkpoint = training_args.resume_from_checkpoint
     elif last_checkpoint is not None:
         checkpoint = last_checkpoint
     train_result = trainer.train(resume_from_checkpoint=checkpoint)
@@ -825,9 +822,24 @@
         )
     metrics["train_samples"] = min(max_train_samples, len(train_dataset))
 
     trainer.log_metrics("train", metrics)
     trainer.save_metrics("train", metrics)
     trainer.save_state()
 
+    # Evaluation
+    if training_args.do_eval:
+        logger.info("*** Evaluate ***")
+
+        metrics = trainer.evaluate()
+        metrics["eval_samples"] =len(eval_dataset)
+        try:
+            perplexity = math.exp(metrics["eval_loss"])
+        except OverflowError:
+            perplexity = float("inf")
+        metrics["perplexity"] = perplexity
+
+        trainer.log_metrics("eval", metrics)
+        trainer.save_metrics("eval", metrics)
+
 if __name__ == "__main__":
     main()
```

### Comparing `HiFT-0.0.1/examples/opt_example.py` & `HiFT-0.0.2/examples/run_glue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,288 +1,116 @@
 #!/usr/bin/env python
 # coding=utf-8
-# Copyright 2018 Google AI, Google Brain and Carnegie Mellon University Authors and the HuggingFace Inc. team.
-# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
+# Copyright 2020 The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Conditional text generation with the auto-regressive models of the library (GPT/GPT-2/CTRL/Transformer-XL/XLNet)
-"""
+""" Finetuning the library models for sequence classification on GLUE."""
+# You can also adapt this script on your own text classification task. Pointers for this are left as comments.
+
 import logging
 import os
+import random
 import sys
 import warnings
-from copy import deepcopy
 from dataclasses import dataclass, field
-from typing import Optional,Tuple,List
-
+from typing import Any, Dict, List, Optional, Union
 import datasets
 import evaluate
-import nltk  # Here to have a nice missing dependency error message early on
 import numpy as np
 from datasets import load_dataset
-from filelock import FileLock
-import fnmatch
-import torch
-import deepspeed
+
 import transformers
 from transformers import (
     AutoConfig,
-    GPT2Config,
-    AutoModelForCausalLM,
+    AutoModelForSequenceClassification,
     AutoTokenizer,
-    DataCollatorForSeq2Seq,
+    DataCollatorWithPadding,
+    EvalPrediction,
     HfArgumentParser,
-    BloomForCausalLM,
-    BloomTokenizerFast,
-    BloomConfig,
-    CTRLLMHeadModel,
-    CTRLTokenizer,
-    CTRLConfig,
-    GenerationMixin,
-    GPT2LMHeadModel,
-    GPT2Tokenizer,
-    GPTJForCausalLM,
-    GPTJConfig,
-    OpenAIGPTLMHeadModel,
-    OpenAIGPTTokenizer,
-    OpenAIGPTConfig,
-    OPTForCausalLM,
-    OPTConfig,
-    TransfoXLLMHeadModel,
-    TransfoXLTokenizer,
-    TransfoXLConfig,
-    XLMTokenizer,
-    XLMWithLMHeadModel,
-    XLMConfig,
-    XLNetLMHeadModel,
-    XLNetTokenizer,
-    XLNetConfig,
-    Seq2SeqTrainer,
-    Seq2SeqTrainingArguments,
+    PretrainedConfig,
+    Trainer,
+    TrainingArguments,
+    default_data_collator,
     set_seed,
 )
-from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version, is_offline_mode, send_example_telemetry
+from transformers.utils import check_min_version, send_example_telemetry
 from transformers.utils.versions import require_version
-from transformers.trainer_pt_utils import LabelSmoother
-
-from peft import (
-    PeftType,
-    LoraConfig,
-    TaskType,
-    get_peft_model
-)
 
 sys.path.append(os.path.abspath('.'))
-
-from hift import HiFTSeq2SeqTrainer,GetCallBack
-
-logging.basicConfig(
-    format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
-    datefmt="%m/%d/%Y %H:%M:%S",
-    level=logging.INFO,
-)
-logger = logging.getLogger(__name__)
-os.environ["WANDB_DISABLED"] = "true"
-MAX_LENGTH = int(10000)  # Hardcoded max length to avoid infinite loop
-IGNORE_TOKEN_ID = -100
-MODEL_CLASSES = {
-    "gpt2": (GPT2LMHeadModel, GPT2Tokenizer,GPT2Config),
-    "geo":(AutoModelForCausalLM,AutoTokenizer,AutoConfig),
-    "ctrl": (CTRLLMHeadModel, CTRLTokenizer,CTRLConfig),
-    "openai-gpt": (OpenAIGPTLMHeadModel, OpenAIGPTTokenizer,OpenAIGPTConfig),
-    "xlnet": (XLNetLMHeadModel, XLNetTokenizer,XLNetConfig),
-    "transfo-xl": (TransfoXLLMHeadModel, TransfoXLTokenizer,TransfoXLConfig),
-    "xlm": (XLMWithLMHeadModel, XLMTokenizer,XLMConfig),
-    "gptj": (GPTJForCausalLM, AutoTokenizer,GPTJConfig),
-    "bloom": (BloomForCausalLM, BloomTokenizerFast,BloomConfig),
-    "llama": (AutoModelForCausalLM, AutoTokenizer,AutoConfig),
-    "opt": (OPTForCausalLM, GPT2Tokenizer,OPTConfig),
-}
-
+from hift import HiFTrainer,GetCallBack,PEFTrainer,peft_function
+from peft import PeftModel, get_peft_model_state_dict
 
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
-check_min_version("4.27.0")
-
-require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/summarization/requirements.txt")
-
-logger = logging.getLogger(__name__)
+check_min_version("4.36.0")
 
-try:
-    nltk.data.find("tokenizers/punkt")
-except (LookupError, OSError):
-    if is_offline_mode():
-        raise LookupError(
-            "Offline mode: run this script without TRANSFORMERS_OFFLINE first to download nltk data files"
-        )
-    with FileLock(".lock") as lock:
-        nltk.download("punkt", quiet=True)
+require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/text-classification/requirements.txt")
 
-@dataclass
-class ModelArguments:
-    """
-    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
-    """
+task_to_keys = {
+    "cola": ("sentence", None),
+    "mnli": ("premise", "hypothesis"),
+    "mrpc": ("sentence1", "sentence2"),
+    "qnli": ("question", "sentence"),
+    "qqp": ("question1", "question2"),
+    "rte": ("sentence1", "sentence2"),
+    "sst2": ("sentence", None),
+    "stsb": ("sentence1", "sentence2"),
+    "wnli": ("sentence1", "sentence2"),
+}
 
-    model_name_or_path: str = field(
-        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
-    )
-    config_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
-    )
-    tokenizer_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
-    )
-    cache_dir: Optional[str] = field(
-        default=None,
-        metadata={"help": "Where to store the pretrained models downloaded from huggingface.co"},
-    )
-    model_type:str= field(
-        default="gpt2",
-        metadata={"help": ("Model type selected in the list: " + ", ".join(MODEL_CLASSES.keys()) )},
-    )
-    padding_side: str = field(
-        default="right", metadata={"help": "The padding side in tokenizer"}
-    )
-    use_fast_tokenizer: bool = field(
-        default=True,
-        metadata={"help": "Whether to use one of the fast tokenizer (backed by the tokenizers library) or not."},
-    )
-    model_revision: str = field(
-        default="main",
-        metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
-    )
-    token: str = field(
-        default=None,
-        metadata={
-            "help": (
-                "The token to use as HTTP bearer authorization for remote files. If not specified, will use the token "
-                "generated when running `huggingface-cli login` (stored in `~/.huggingface`)."
-            )
-        },
-    )
-    use_auth_token: bool = field(
-        default=None,
-        metadata={
-            "help": "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead."
-        },
-    )
-    trust_remote_code: bool = field(
-        default=False,
-        metadata={
-            "help": (
-                "Whether or not to allow for custom models defined on the Hub in their own modeling files. This option"
-                "should only be set to `True` for repositories you trust and in which you have read the code, as it will "
-                "execute code present on the Hub on your local machine."
-            )
-        },
-    )
-    resize_position_embeddings: Optional[bool] = field(
-        default=None,
-        metadata={
-            "help": (
-                "Whether to automatically resize the position embeddings if `max_source_length` exceeds "
-                "the model's position embeddings."
-            )
-        },
-    )
+logger = logging.getLogger(__name__)
 
 @dataclass
 class DataTrainingArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and eval.
-    """
 
-    lang: Optional[str] = field(default=None, metadata={"help": "Language id for summarization."})
+    Using `HfArgumentParser` we can turn this class
+    into argparse arguments to be able to specify them on
+    the command line.
+    """
 
+    task_name: Optional[str] = field(
+        default=None,
+        metadata={"help": "The name of the task to train on: " + ", ".join(task_to_keys.keys())},
+    )
     dataset_name: Optional[str] = field(
         default=None, metadata={"help": "The name of the dataset to use (via the datasets library)."}
     )
     dataset_config_name: Optional[str] = field(
         default=None, metadata={"help": "The configuration name of the dataset to use (via the datasets library)."}
     )
-    source_column: Optional[str] = field(
-        default=None,
-        metadata={"help": "The name of the column in the datasets containing the full texts (for summarization)."},
-    )
-    target_column: Optional[str] = field(
-        default=None,
-        metadata={"help": "The name of the column in the datasets containing the summaries (for summarization)."},
-    )
-    train_file: Optional[str] = field(
-        default=None, metadata={"help": "The input training data file (a jsonlines or csv file)."}
-    )
-    validation_file: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": (
-                "An optional input evaluation data file to evaluate the metrics (rouge) on (a jsonlines or csv file)."
-            )
-        },
-    )
-    test_file: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "An optional input test data file to evaluate the metrics (rouge) on (a jsonlines or csv file)."
-        },
-    )
-    overwrite_cache: bool = field(
-        default=False, metadata={"help": "Overwrite the cached training and evaluation sets"}
-    )
-    preprocessing_num_workers: Optional[int] = field(
-        default=None,
-        metadata={"help": "The number of processes to use for the preprocessing."},
-    )
-    max_source_length: Optional[int] = field(
-        default=200,
+    max_seq_length: int = field(
+        default=128,
         metadata={
             "help": (
                 "The maximum total input sequence length after tokenization. Sequences longer "
                 "than this will be truncated, sequences shorter will be padded."
             )
         },
     )
-    max_target_length: Optional[int] = field(
-        default=343,
-        metadata={
-            "help": (
-                "The maximum total sequence length for target text after tokenization. Sequences longer "
-                "than this will be truncated, sequences shorter will be padded."
-            )
-        },
-    )
-    val_max_target_length: Optional[int] = field(
-        default=None,
-        metadata={
-            "help": (
-                "The maximum total sequence length for validation target text after tokenization. Sequences longer "
-                "than this will be truncated, sequences shorter will be padded. Will default to `max_target_length`. "
-                "This argument is also used to override the ``max_length`` param of ``model.generate``, which is used "
-                "during ``evaluate`` and ``predict``."
-            )
-        },
+    overwrite_cache: bool = field(
+        default=False, metadata={"help": "Overwrite the cached preprocessed datasets or not."}
     )
     pad_to_max_length: bool = field(
-        default=False,
+        default=True,
         metadata={
             "help": (
-                "Whether to pad all samples to model maximum sentence length. "
-                "If False, will pad the samples dynamically when batching to the maximum length in the batch. More "
-                "efficient on GPU but very bad for TPU."
+                "Whether to pad all samples to `max_seq_length`. "
+                "If False, will pad the samples dynamically when batching to the maximum length in the batch."
             )
         },
     )
     max_train_samples: Optional[int] = field(
         default=None,
         metadata={
             "help": (
@@ -305,86 +133,124 @@
         metadata={
             "help": (
                 "For debugging purposes or quicker training, truncate the number of prediction examples to this "
                 "value if set."
             )
         },
     )
-    num_beams: Optional[int] = field(
-        default=1,
-        metadata={
-            "help": (
-                "Number of beams to use for evaluation. This argument will be passed to ``model.generate``, "
-                "which is used during ``evaluate`` and ``predict``."
-            )
-        },
+    train_file: Optional[str] = field(
+        default=None, metadata={"help": "A csv or a json file containing the training data."}
+    )
+    validation_file: Optional[str] = field(
+        default=None, metadata={"help": "A csv or a json file containing the validation data."}
     )
-    ignore_pad_token_for_loss: bool = field(
+    test_file: Optional[str] = field(default=None, metadata={"help": "A csv or a json file containing the test data."})
+
+    def __post_init__(self):
+        if self.task_name is not None:
+            self.task_name = self.task_name.lower()
+            if self.task_name not in task_to_keys.keys():
+                raise ValueError("Unknown task, you should pick one in " + ",".join(task_to_keys.keys()))
+        elif self.dataset_name is not None:
+            pass
+        elif self.train_file is None or self.validation_file is None:
+            raise ValueError("Need either a GLUE task, a training/validation file or a dataset name.")
+        else:
+            train_extension = self.train_file.split(".")[-1]
+            assert train_extension in ["csv", "json"], "`train_file` should be a csv or a json file."
+            validation_extension = self.validation_file.split(".")[-1]
+            assert (
+                validation_extension == train_extension
+            ), "`validation_file` should have the same extension (csv or json) as `train_file`."
+
+
+@dataclass
+class ModelArguments:
+    """
+    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
+    """
+
+    model_name_or_path: str = field(
+        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
+    )
+    config_name: Optional[str] = field(
+        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
+    )
+    tokenizer_name: Optional[str] = field(
+        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
+    )
+    cache_dir: Optional[str] = field(
+        default=None,
+        metadata={"help": "Where do you want to store the pretrained models downloaded from huggingface.co"},
+    )
+    use_fast_tokenizer: bool = field(
         default=True,
-        metadata={
-            "help": "Whether to ignore the tokens corresponding to padded labels in the loss computation or not."
-        },
+        metadata={"help": "Whether to use one of the fast tokenizer (backed by the tokenizers library) or not."},
     )
-    source_prefix: Optional[str] = field(
-        default=None, metadata={"help": "A prefix to add before every source text (useful for T5 models)."}
+    model_revision: str = field(
+        default="main",
+        metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
     )
-
-    forced_bos_token: Optional[str] = field(
+    token: str = field(
         default=None,
         metadata={
             "help": (
-                "The token to force as the first generated token after the decoder_start_token_id. "
-                "Useful for multilingual models like mBART where the first generated token"
-                "needs to be the target language token (Usually it is the target language token)"
+                "The token to use as HTTP bearer authorization for remote files. If not specified, will use the token "
+                "generated when running `huggingface-cli login` (stored in `~/.huggingface`)."
             )
         },
     )
-
-    def __post_init__(self):
-        if (
-            self.dataset_name is None
-            and self.train_file is None
-            and self.validation_file is None
-            and self.test_file is None
-        ):
-            raise ValueError("Need either a dataset name or a training, validation, or test file.")
-        else:
-            if self.train_file is not None:
-                extension = self.train_file.split(".")[-1]
-                assert extension in ["csv", "json"], "`train_file` should be a csv or a json file."
-            if self.validation_file is not None:
-                extension = self.validation_file.split(".")[-1]
-                assert extension in ["csv", "json"], "`validation_file` should be a csv or a json file."
-            if self.test_file is not None:
-                extension = self.test_file.split(".")[-1]
-                assert extension in ["csv", "json"], "`test_file` should be a csv or a json file."
-        if self.val_max_target_length is None:
-            self.val_max_target_length = self.max_target_length
-
-@dataclass
-class TrainingArguments(Seq2SeqTrainingArguments):
-    model_max_length: int = field(
-        default=512,
+    use_auth_token: bool = field(
+        default=None,
         metadata={
-            "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
+            "help": "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead."
         },
     )
-    pretraining_tp: int = field(
-        default=1,
+    trust_remote_code: bool = field(
+        default=False,
         metadata={
-            "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
+            "help": (
+                "Whether or not to allow for custom models defined on the Hub in their own modeling files. This option"
+                "should only be set to `True` for repositories you trust and in which you have read the code, as it will "
+                "execute code present on the Hub on your local machine."
+            )
         },
     )
+    ignore_mismatched_sizes: bool = field(
+        default=False,
+        metadata={"help": "Will enable to load a pretrained model whose head dimensions are different."},
+    )
 
 @dataclass
 class HiFTArguments(ModelArguments):
     HiTaskType: str = field(
-        default="CAUSAL_LM",
+        default="SEQ_CLS",
         metadata={"help": ("HiTaskType should be consistent with PEFT TaskType" )},
     )
+    peft_type: str = field(
+        default=None,
+        metadata={"help": ("peft_type should be in [lora,adalora,ia3,p_tuning,prefix_tuning,prompt_tuning]" )},
+    )
+    init_text:str = field(
+        default="Predict if sentiment of this review is positive, negative or neutral",
+        metadata={
+            "help": (
+                "the init prompt text for prompt tuning"
+            )
+        },
+    )
+    lora_rank: int = field(
+        default=8,
+        metadata={"help": ("rank for lora or adalora" )},
+    )
+    peft_path : Optional[str] = field(default=None)
+    virtual_tokens:int = field(
+        default=20,
+        metadata={"help": ("the number of virtual tokens for p_tuning, prefix_tuning and prefix_tuning" )},
+    )
     group_element: int = field(
         default=1,
         metadata={"help": ("number element for each group parameters" )},
     )
     optimizer_strategy: str = field(
         default="down2up",
         metadata={"help": ("optimizer strategy of ['down2up','down2up','random']" )},
@@ -393,74 +259,77 @@
         default=False,
         metadata={
             "help": (
                 "hierarchical optimization for LLMS"
             )
         },
     )
-    lora_tuning:bool = field(
-        default=False,
-        metadata={
-            "help": (
-                "whether using lora tuning"
-            )
-        },
-    )
     freeze_layers: List[str] = field(
         default_factory=list,
         metadata={
             "help": (
                 "Index of the frozen layer"
             )
         },
     )
 
+class SavePeftModelCallback(transformers.TrainerCallback):
+    def save_model(self, args, state, kwargs):
+        if state.best_model_checkpoint is not None:
+            checkpoint_folder = os.path.join(state.best_model_checkpoint, "peft_model")
+        else:
+            checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
 
-
-datasets_name_mapping = {
-    "amazon_reviews_multi": ("review_body", "review_title"),
-    "big_patent": ("description", "abstract"),
-    "cnn_dailymail": ("article", "highlights"),
-    "orange_sum": ("text", "summary"),
-    "pn_summary": ("article", "summary"),
-    "psc": ("extract_text", "summary_text"),
-    "samsum": ("dialogue", "summary"),
-    "thaisum": ("body", "summary"),
-    "xglue": ("news_body", "news_title"),
-    "xsum": ("document", "summary"),
-    "wiki_summary": ("article", "highlights"),
-    "multi_news": ("document", "summary"),
-    "e2e_nlg":("meaning_representation", "human_reference"),
-}
-
+        peft_model_path = os.path.join(checkpoint_folder, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
+
+    def on_save(self, args, state, control, **kwargs):
+        self.save_model(args, state, kwargs)
+        return control
+
+    def on_train_end(self, args, state, control, **kwargs):
+        peft_model_path = os.path.join(args.output_dir, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
     parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
     if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         # If we pass only one argument to the script and it's the path to a json file,
         # let's parse it to get our arguments.
         model_args, data_args, training_args = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         model_args, data_args, training_args = parser.parse_args_into_dataclasses()
+
     if model_args.use_auth_token is not None:
         warnings.warn(
             "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead.",
             FutureWarning,
         )
         if model_args.token is not None:
             raise ValueError("`token` and `use_auth_token` are both specified. Please set only the argument `token`.")
         model_args.token = model_args.use_auth_token
     # Sending telemetry. Tracking the example usage helps us better allocate resources to maintain them. The
     # information sent is the one passed as arguments along with your Python/PyTorch versions.
-    send_example_telemetry("run_summarization", model_args, data_args)
-
+    send_example_telemetry("run_glue", model_args, data_args)
+    # #TODO: wandb
+    # # ======wandb config====
+    # os.environ['WANDB_PROJECT'] = model_args.model_name_or_path.split('/')[-1] + '_glue_' + data_args.task_name
+    # if model_args.hier_tuning is False:
+    #     os.environ['WANDB_RUN_NAME'] = f"normal_finetuning"
+    # else:
+    #     os.environ['WANDB_RUN_NAME'] = f"htune_{model_args.optimizer_strategy}_group{model_args.group_element}"
+    #     if model_args.hier_reverse:
+    #         os.environ['WANDB_RUN_NAME'] += "_rev"
+    # os.environ['WANDB_RUN_NAME'] += f"_v{random.randint(a=100, b=999)}"
     # Setup logging
     logging.basicConfig(
         format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
         datefmt="%m/%d/%Y %H:%M:%S",
         handlers=[logging.StreamHandler(sys.stdout)],
     )
 
@@ -478,26 +347,14 @@
     # Log on each process the small summary:
     logger.warning(
         f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
         + f"distributed training: {training_args.parallel_mode.value == 'distributed'}, 16-bits training: {training_args.fp16}"
     )
     logger.info(f"Training/evaluation parameters {training_args}")
 
-    if data_args.source_prefix is None and model_args.model_name_or_path in [
-        "t5-small",
-        "t5-base",
-        "t5-large",
-        "t5-3b",
-        "t5-11b",
-    ]:
-        logger.warning(
-            "You're running a t5 model but didn't provide a source prefix, which is the expected, e.g. with "
-            "`--source_prefix 'summarize: ' `"
-        )
-
     # Detecting last checkpoint.
     last_checkpoint = None
     if os.path.isdir(training_args.output_dir) and training_args.do_train and not training_args.overwrite_output_dir:
         last_checkpoint = get_last_checkpoint(training_args.output_dir)
         if last_checkpoint is None and len(os.listdir(training_args.output_dir)) > 0:
             raise ValueError(
                 f"Output directory ({training_args.output_dir}) already exists and is not empty. "
@@ -509,325 +366,402 @@
                 "the `--output_dir` or add `--overwrite_output_dir` to train from scratch."
             )
 
     # Set seed before initializing model.
     set_seed(training_args.seed)
 
     # Get the datasets: you can either provide your own CSV/JSON training and evaluation files (see below)
-    # or just provide the name of one of the public datasets available on the hub at https://huggingface.co/datasets/
-    # (the dataset will be downloaded automatically from the datasets Hub).
+    # or specify a GLUE benchmark task (the dataset will be downloaded automatically from the datasets Hub).
+    #
+    # For CSV/JSON files, this script will use as labels the column called 'label' and as pair of sentences the
+    # sentences in columns called 'sentence1' and 'sentence2' if such column exists or the first two columns not named
+    # label if at least two columns are provided.
     #
-    # For CSV/JSON files this script will use the first column for the full texts and the second column for the
-    # summaries (unless you specify column names for this with the `source_column` and `target_column` arguments).
+    # If the CSVs/JSONs contain only one non-label column, the script does single sentence classification on this
+    # single column. You can easily tweak this behavior (see below)
     #
     # In distributed training, the load_dataset function guarantee that only one local process can concurrently
     # download the dataset.
-    if data_args.dataset_name is not None:
+    if data_args.task_name is not None:
         # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
-            data_args.dataset_name,
-            data_args.dataset_config_name,
+            "glue",
+            data_args.task_name,
             cache_dir=model_args.cache_dir,
             token=model_args.token,
         )
-    else:
-        data_files = {}
-        if data_args.train_file is not None:
-            data_files["train"] = data_args.train_file
-            extension = data_args.train_file.split(".")[-1]
-        if data_args.validation_file is not None:
-            data_files["validation"] = data_args.validation_file
-            extension = data_args.validation_file.split(".")[-1]
-        if data_args.test_file is not None:
-            data_files["test"] = data_args.test_file
-            extension = data_args.test_file.split(".")[-1]
+    elif data_args.dataset_name is not None:
+        # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
-            extension,
-            data_files=data_files,
+            data_args.dataset_name,
+            data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             token=model_args.token,
         )
-    # See more about loading any type of standard or custom dataset (from files, python dict, pandas DataFrame, etc) at
+    else:
+        # Loading a dataset from your local files.
+        # CSV/JSON training and evaluation files are needed.
+        data_files = {"train": data_args.train_file, "validation": data_args.validation_file}
+
+        # Get the test dataset: you can provide your own CSV/JSON test file (see below)
+        # when you use `do_predict` without specifying a GLUE benchmark task.
+        if training_args.do_predict:
+            if data_args.test_file is not None:
+                train_extension = data_args.train_file.split(".")[-1]
+                test_extension = data_args.test_file.split(".")[-1]
+                assert (
+                    test_extension == train_extension
+                ), "`test_file` should have the same extension (csv or json) as `train_file`."
+                data_files["test"] = data_args.test_file
+            else:
+                raise ValueError("Need either a GLUE task or a test file for `do_predict`.")
+
+        for key in data_files.keys():
+            logger.info(f"load a local file for {key}: {data_files[key]}")
+
+        if data_args.train_file.endswith(".csv"):
+            # Loading a dataset from local csv files
+            raw_datasets = load_dataset(
+                "csv",
+                data_files=data_files,
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+            )
+        else:
+            # Loading a dataset from local json files
+            raw_datasets = load_dataset(
+                "json",
+                data_files=data_files,
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+            )
+    # See more about loading any type of standard or custom dataset at
     # https://huggingface.co/docs/datasets/loading_datasets.
 
+    # Labels
+    if data_args.task_name is not None:
+        is_regression = data_args.task_name == "stsb"
+        if not is_regression:
+            label_list = raw_datasets["train"].features["label"].names
+            num_labels = len(label_list)
+        else:
+            num_labels = 1
+    else:
+        # Trying to have good defaults here, don't hesitate to tweak to your needs.
+        is_regression = raw_datasets["train"].features["label"].dtype in ["float32", "float64"]
+        if is_regression:
+            num_labels = 1
+        else:
+            # A useful fast method:
+            # https://huggingface.co/docs/datasets/package_reference/main_classes#datasets.Dataset.unique
+            label_list = raw_datasets["train"].unique("label")
+            label_list.sort()  # Let's sort it for determinism
+            num_labels = len(label_list)
+
     # Load pretrained model and tokenizer
     #
-    # Distributed training:
-    # The .from_pretrained methods guarantee that only one local process can concurrently
+    # In distributed training, the .from_pretrained methods guarantee that only one local process can concurrently
     # download model & vocab.
-    model_class, tokenizer_class,model_config = MODEL_CLASSES[model_args.model_type]
-    config = model_config.from_pretrained(
+    config = AutoConfig.from_pretrained(
         model_args.config_name if model_args.config_name else model_args.model_name_or_path,
+        num_labels=num_labels,
+        finetuning_task=data_args.task_name,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
-        use_auth_token=True if model_args.use_auth_token else None,
+        token=model_args.token,
+        trust_remote_code=model_args.trust_remote_code,
     )
-    if training_args.pretraining_tp >1:
-        config.pretraining_tp = training_args.pretraining_tp
-    # if training_args.gradient_checkpointing:
-    # config.gradient_checkpointing = training_args.gradient_checkpointing
-    tokenizer = tokenizer_class.from_pretrained(
+    config.gradient_checkpointing = training_args.gradient_checkpointing
+    tokenizer = AutoTokenizer.from_pretrained(
         model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
         cache_dir=model_args.cache_dir,
         use_fast=model_args.use_fast_tokenizer,
         revision=model_args.model_revision,
-        model_max_length=training_args.model_max_length,
-        padding_side=model_args.padding_side,
-        use_auth_token=True if model_args.use_auth_token else None,
+        token=model_args.token,
+        trust_remote_code=model_args.trust_remote_code,
     )
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
-    model = model_class.from_pretrained(
+    if config.pad_token_id is None:
+        config.pad_token_id = tokenizer.eos_token_id
+    model = AutoModelForSequenceClassification.from_pretrained(
         model_args.model_name_or_path,
         from_tf=bool(".ckpt" in model_args.model_name_or_path),
         config=config,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
-        use_auth_token=True if model_args.use_auth_token else None,
-    )
-    if model_args.lora_tuning:
-        peft_config = LoraConfig(
-            peft_type = PeftType.LORA,
-            lora_alpha=16,
-            lora_dropout=0.1,
-            r=8,
-            bias="none",
-            task_type=TaskType.CAUSAL_LM)
-        model = get_peft_model(model, peft_config)
-    # We resize the embeddings only when necessary to avoid index errors. If you are creating a model from scratch
-    # on a small vocab and want a smaller embedding size, remove this test.
-    embedding_size = model.get_input_embeddings().weight.shape[0]
-    if len(tokenizer) > embedding_size:
-        model.resize_token_embeddings(len(tokenizer))
-    model.config.decoder_start_token_id = model.config.bos_token_id
-    if model.config.decoder_start_token_id is None:
-        model.config.decoder_start_token_id = model.config.bos_token_id
-
-    # Preprocessing the datasets.
-    # We need to tokenize inputs and targets.
-    if training_args.do_train:
-        if "train" not in raw_datasets:
-            raise ValueError("--do_train requires a train dataset")
-        column_names = raw_datasets["train"].column_names
-    elif training_args.do_eval:
-        if "validation" not in raw_datasets:
-            raise ValueError("--do_eval requires a validation dataset")
-        column_names = raw_datasets["validation"].column_names
-    elif training_args.do_predict:
-        if "test" not in raw_datasets:
-            raise ValueError("--do_predict requires a test dataset")
-        column_names = raw_datasets["test"].column_names
-    else:
-        logger.info("There is nothing to do. Please pass `do_train`, `do_eval` and/or `do_predict`.")
-        return
-
-    # Get the column names for input/target.
-    dataset_columns = datasets_name_mapping.get(data_args.dataset_name, None)
-    if data_args.source_column is None:
-        source_column = dataset_columns[0] if dataset_columns is not None else column_names[0]
+        token=model_args.token,
+        trust_remote_code=model_args.trust_remote_code,
+        ignore_mismatched_sizes=model_args.ignore_mismatched_sizes,
+    )
+    if model_args.peft_type:
+        if model_args.peft_path is not None:
+            logger.info("Peft from pre-trained model")
+            model = PeftModel.from_pretrained(model, model_args.peft_path)
+        else:
+            model = peft_function(model,
+                    config = config,
+                    peft_type = model_args.peft_type,
+                    task_type = model_args.HiTaskType,
+                    rank=model_args.lora_rank,
+                    virtual_tokens=model_args.virtual_tokens,
+                    tokenizer_name_or_path=model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
+                    init_text=model_args.init_text if model_args.peft_type=="prompt_tuning" else None,
+                    peft_config=None)
+    # Preprocessing the raw_datasets
+    if data_args.task_name is not None:
+        sentence1_key, sentence2_key = task_to_keys[data_args.task_name]
     else:
-        source_column = data_args.source_column
-        if source_column not in column_names:
-            raise ValueError(
-                f"--source_column' value '{data_args.sourcec_column}' needs to be one of: {', '.join(column_names)}"
-            )
-    if data_args.target_column is None:
-        target_column = dataset_columns[1] if dataset_columns is not None else column_names[1]
+        # Again, we try to have some nice defaults but don't hesitate to tweak to your use case.
+        non_label_column_names = [name for name in raw_datasets["train"].column_names if name != "label"]
+        if "sentence1" in non_label_column_names and "sentence2" in non_label_column_names:
+            sentence1_key, sentence2_key = "sentence1", "sentence2"
+        else:
+            if len(non_label_column_names) >= 2:
+                sentence1_key, sentence2_key = non_label_column_names[:2]
+            else:
+                sentence1_key, sentence2_key = non_label_column_names[0], None
+
+    # Padding strategy
+    if data_args.pad_to_max_length:
+        padding = "max_length"
     else:
-        target_column = data_args.target_column
-        if target_column not in column_names:
-            raise ValueError(
-                f"--target_column' value '{data_args.target_column}' needs to be one of: {', '.join(column_names)}"
-            )
+        # We will pad later, dynamically at batch creation, to the max sequence length in each batch
+        padding = False
 
-    # Temporarily set max_target_length for training.
-    max_target_length = data_args.max_target_length
-    padding = "max_length" if data_args.pad_to_max_length else False
+    # Some models have set the order of the labels to use, so let's make sure we do use it.
+    label_to_id = None
+    if (
+        model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id
+        and data_args.task_name is not None
+        and not is_regression
+    ):
+        # Some have all caps in their config, some don't.
+        label_name_to_id = {k.lower(): v for k, v in model.config.label2id.items()}
+        if sorted(label_name_to_id.keys()) == sorted(label_list):
+            label_to_id = {i: int(label_name_to_id[label_list[i]]) for i in range(num_labels)}
+        else:
+            logger.warning(
+                "Your model seems to have been trained with labels, but they don't match the dataset: ",
+                f"model labels: {sorted(label_name_to_id.keys())}, dataset labels: {sorted(label_list)}."
+                "\nIgnoring the model labels as a result.",
+            )
+    elif data_args.task_name is None and not is_regression:
+        label_to_id = {v: i for i, v in enumerate(label_list)}
+
+    if label_to_id is not None:
+        model.config.label2id = label_to_id
+        model.config.id2label = {id: label for label, id in config.label2id.items()}
+    elif data_args.task_name is not None and not is_regression:
+        model.config.label2id = {l: i for i, l in enumerate(label_list)}
+        model.config.id2label = {id: label for label, id in config.label2id.items()}
 
-    if training_args.label_smoothing_factor > 0 and not hasattr(model, "prepare_decoder_input_ids_from_labels"):
+    if data_args.max_seq_length > tokenizer.model_max_length:
         logger.warning(
-            "label_smoothing is enabled but the `prepare_decoder_input_ids_from_labels` method is not defined for "
-            f"`{model.__class__.__name__}`. This will lead to loss being calculated twice and will take up more memory"
+            f"The max_seq_length passed ({data_args.max_seq_length}) is larger than the maximum length for the "
+            f"model ({tokenizer.model_max_length}). Using max_seq_length={tokenizer.model_max_length}."
         )
-    def preprocess_function_for_generation(examples):
-        IGNORE_TOKEN_ID = -100
-        if training_args.label_smoothing_factor >0:
-            IGNORE_TOKEN_ID = LabelSmoother.ignore_index
-        SEPTOKEN=" ### "
-        inputs, targets = [], []
-        for i in range(len(examples[source_column])):
-            if examples[source_column][i] and examples[target_column][i]:
-                src = examples[source_column][i].strip().rstrip()+SEPTOKEN
-                tgt = examples[target_column][i].strip().rstrip()
-                inputs.append(src)
-                targets.append(tgt)
-        assert len(inputs) == len(targets)
-        model_inputs = tokenizer(inputs, 
-            max_length=data_args.max_source_length,
-            padding=padding,
-            truncation=True)
-        labels = tokenizer(targets,
-                max_length=data_args.max_target_length, 
-                padding=padding, 
-                truncation=True)
-        model_inputs["labels"] = labels["input_ids"]
-        return model_inputs
+    max_seq_length = min(data_args.max_seq_length, tokenizer.model_max_length)
+
     def preprocess_function(examples):
-        # remove pairs where at least one record is None
-        IGNORE_TOKEN_ID = -100
-        if training_args.label_smoothing_factor >0:
-            IGNORE_TOKEN_ID = LabelSmoother.ignore_index
-        inputs, targets = [], []
-        for i in range(len(examples[source_column])):
-            if examples[source_column][i] and examples[target_column][i]:
-                inputs.append(examples[source_column][i].strip().rstrip())
-                targets.append(examples[target_column][i].strip().rstrip())
-        SEPTOKEN = tokenizer.tokenize("###")
-        source_tokens,target_tokens=[],[]
-        for inp,tar in zip(inputs,targets):
-            source_tokens.append(tokenizer.tokenize(inp))
-            target_tokens.append(tokenizer.tokenize(tar))
-        
-        examples = [" ".join(inp+SEPTOKEN+tar) for inp,tar in zip(source_tokens,target_tokens)]
-        model_inputs = tokenizer(examples, 
-                        max_length=tokenizer.model_max_length,
-                        padding=padding,
-                        truncation=True)
-        labels = deepcopy(model_inputs["input_ids"])
-        # IGNORE input
-        # for inp,target in zip(source_tokens,labels):
-        #     target[:len(inp)+1] = [IGNORE_TOKEN_ID] * (len(inp) + 1)
-        # If we are padding here, replace all tokenizer.pad_token_id in the labels by IGNORE_TOKEN_ID when we want to ignore
-        # padding in the loss.
-        if padding == "max_length" and data_args.ignore_pad_token_for_loss:
-            labels =  [
-                [(l if l != tokenizer.pad_token_id else IGNORE_TOKEN_ID) for l in label] for label in labels
-            ]
-
-        model_inputs["labels"] = labels
-        return model_inputs
-
-    assert training_args.do_train
-    train_dataset = raw_datasets["train"]
-    if data_args.max_train_samples is not None:
-        max_train_samples = min(len(train_dataset), data_args.max_train_samples)
-        train_dataset = train_dataset.select(range(max_train_samples))
-    with training_args.main_process_first(desc="train dataset map pre-processing"):
-        train_dataset=train_dataset.map(
-        lambda x : tokenizer(
-            list(map(lambda a,b: a + " ### " + b, x[source_column], x[target_column])), 
-            truncation="only_second",
-            max_length=tokenizer.model_max_length, 
-            padding=padding), 
-            batched=True,
-            desc="Running tokenizer on train dataset")
-        train_dataset = train_dataset.map(lambda x: {'labels':x['input_ids']})
+        # Tokenize the texts
+        args = (
+            (examples[sentence1_key],) if sentence2_key is None else (examples[sentence1_key], examples[sentence2_key])
+        )
+        result = tokenizer(*args, padding=padding, max_length=max_seq_length, truncation=True)
+
+        # Map labels to IDs (not necessary for GLUE tasks)
+        if label_to_id is not None and "label" in examples:
+            result["label"] = [(label_to_id[l] if l != -1 else -1) for l in examples["label"]]
+        return result
 
-    max_target_length = data_args.val_max_target_length
-    eval_dataset = raw_datasets["validation"]
-    if data_args.max_eval_samples is not None:
-        max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
-        eval_dataset = eval_dataset.select(range(max_eval_samples))
-    with training_args.main_process_first(desc="validation dataset map pre-processing"):
-        eval_dataset=eval_dataset.map(
-        lambda x : tokenizer(
-            list(map(lambda a,b: a + " ### " + b, x[source_column], x[target_column])), 
-            truncation="only_second",
-            max_length=tokenizer.model_max_length, 
-            padding=padding), 
+    with training_args.main_process_first(desc="dataset map pre-processing"):
+        raw_datasets = raw_datasets.map(
+            preprocess_function,
             batched=True,
-            desc="Running tokenizer on validation dataset")
-        eval_dataset = train_dataset.map(lambda x: {'labels':x['input_ids']})
-    # Data collator
-    label_pad_token_id = IGNORE_TOKEN_ID if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id
-    data_collator = DataCollatorForSeq2Seq(
-        tokenizer,
-        model=model,
-        label_pad_token_id=label_pad_token_id,
-        pad_to_multiple_of=8 if training_args.fp16 else None,
-    )
-
-    # Metric
-    metric = evaluate.load("rouge")
-    def postprocess_text(preds, labels):
-        preds = [pred.strip() for pred in preds]
-        labels = [label.strip() for label in labels]
-        # rougeLSum expects newline after each sentence
-        preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in preds]
-        labels = ["\n".join(nltk.sent_tokenize(label)) for label in labels]
-        return preds, labels
-
-    def compute_metrics(eval_preds):
-        preds, labels = eval_preds
-        if isinstance(preds, tuple):
-            preds = preds[0]
-        # Replace -100s used for padding as we can't decode them
-        preds = np.where(preds != IGNORE_TOKEN_ID, preds, tokenizer.pad_token_id)
-        decoded_preds = tokenizer.batch_decode(preds, skip_special_tokens=True)
-        labels = np.where(labels != IGNORE_TOKEN_ID, labels, tokenizer.pad_token_id)
-        decoded_labels = tokenizer.batch_decode(labels, skip_special_tokens=True)
-
-        # Some simple post-processing
-        decoded_preds, decoded_labels = postprocess_text(decoded_preds, decoded_labels)
-        result = metric.compute(predictions=decoded_preds, references=decoded_labels, use_stemmer=True)
-        result = {k: round(v * 100, 4) for k, v in result.items()}
-        prediction_lens = [np.count_nonzero(pred != tokenizer.pad_token_id) for pred in preds]
-        result["gen_len"] = np.mean(prediction_lens)
+            load_from_cache_file=not data_args.overwrite_cache,
+            desc="Running tokenizer on dataset",
+        )
+    if training_args.do_train:
+        if "train" not in raw_datasets:
+            raise ValueError("--do_train requires a train dataset")
+        train_dataset = raw_datasets["train"]
+        if data_args.max_train_samples is not None:
+            max_train_samples = min(len(train_dataset), data_args.max_train_samples)
+            train_dataset = train_dataset.select(range(max_train_samples))
+
+    if training_args.do_eval:
+        if "validation" not in raw_datasets and "validation_matched" not in raw_datasets:
+            raise ValueError("--do_eval requires a validation dataset")
+        eval_dataset = raw_datasets["validation_matched" if data_args.task_name == "mnli" else "validation"]
+        if data_args.max_eval_samples is not None:
+            max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
+            eval_dataset = eval_dataset.select(range(max_eval_samples))
+
+    if training_args.do_predict or data_args.task_name is not None or data_args.test_file is not None:
+        if "test" not in raw_datasets and "test_matched" not in raw_datasets:
+            raise ValueError("--do_predict requires a test dataset")
+        predict_dataset = raw_datasets["test_matched" if data_args.task_name == "mnli" else "test"]
+        if data_args.max_predict_samples is not None:
+            max_predict_samples = min(len(predict_dataset), data_args.max_predict_samples)
+            predict_dataset = predict_dataset.select(range(max_predict_samples))
+
+    # Log a few random samples from the training set:
+    if training_args.do_train:
+        for index in random.sample(range(len(train_dataset)), 3):
+            logger.info(f"Sample {index} of the training set: {train_dataset[index]}.")
+
+    # Get the metric function
+    if data_args.task_name is not None:
+        metric = evaluate.load("glue", data_args.task_name)
+    elif is_regression:
+        metric = evaluate.load("mse")
+    else:
+        metric = evaluate.load("accuracy")
+
+    # You can define your custom compute_metrics function. It takes an `EvalPrediction` object (a namedtuple with a
+    # predictions and label_ids field) and has to return a dictionary string to float.
+    def compute_metrics(p: EvalPrediction):
+        preds = p.predictions[0] if isinstance(p.predictions, tuple) else p.predictions
+        preds = np.squeeze(preds) if is_regression else np.argmax(preds, axis=1)
+        result = metric.compute(predictions=preds, references=p.label_ids)
+        if len(result) > 1:
+            result["combined_score"] = np.mean(list(result.values())).item()
         return result
-    training_args.generation_max_length = (
-        training_args.generation_max_length
-        if training_args.generation_max_length is not None
-        else data_args.val_max_target_length
-    )
-    training_args.generation_num_beams = (
-        data_args.num_beams if data_args.num_beams is not None else training_args.generation_num_beams
-    )
-    # Initialize our Trainer
+
+    # Data collator will default to DataCollatorWithPadding when the tokenizer is passed to Trainer, so we change it if
+    # we already did the padding.
+    if data_args.pad_to_max_length:
+        data_collator = default_data_collator
+    elif training_args.fp16:
+        data_collator = DataCollatorWithPadding(tokenizer, pad_to_multiple_of=8)
+    else:
+        data_collator = None
+    # Initialize HiFTrainer
     if model_args.hier_tuning:#hier_tuning
-        trainer = HiFTSeq2SeqTrainer(
+        trainer = HiFTrainer(
             hiFThandler = GetCallBack(model_args.model_name_or_path),
             HiTaskType = model_args.HiTaskType,
             group_element = model_args.group_element,
             strategy = model_args.optimizer_strategy,
             hier_tuning= model_args.hier_tuning,
-            lora_tuning = model_args.lora_tuning,
+            peft_type = model_args.peft_type,
             freeze_layers = model_args.freeze_layers,
-            model=model,
+            args=training_args,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
-            compute_metrics=compute_metrics if training_args.predict_with_generate else None,
+            model=model,
             tokenizer=tokenizer,
-            data_collator=data_collator,
-            args=training_args
+            compute_metrics=compute_metrics,
+            data_collator=data_collator
         )
     else:
-        trainer = Seq2SeqTrainer(
-            model=model,
+        trainer = PEFTrainer(
+            peft_type = model_args.peft_type,
             args=training_args,
+            model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
+            compute_metrics=compute_metrics,
             tokenizer=tokenizer,
             data_collator=data_collator,
-            compute_metrics=compute_metrics if training_args.predict_with_generate else None,
         )
-
     # Training
-    checkpoint = None
-    if training_args.resume_from_checkpoint is not None:
-        checkpoint = training_args.resume_from_checkpoint
-    elif last_checkpoint is not None:
-        checkpoint = last_checkpoint
-    train_result = trainer.train(resume_from_checkpoint=checkpoint)
-    trainer.save_model()  # Saves the tokenizer too for easy upload
-
-    metrics = train_result.metrics
-    max_train_samples = (
+    if training_args.do_train:
+        checkpoint = None
+        if training_args.resume_from_checkpoint is not None:
+            checkpoint = training_args.resume_from_checkpoint
+        elif last_checkpoint is not None:
+            checkpoint = last_checkpoint
+        train_result = trainer.train(resume_from_checkpoint=checkpoint)
+        metrics = train_result.metrics
+        max_train_samples = (
             data_args.max_train_samples if data_args.max_train_samples is not None else len(train_dataset)
         )
-    metrics["train_samples"] = min(max_train_samples, len(train_dataset))
+        metrics["train_samples"] = min(max_train_samples, len(train_dataset))
+
+        trainer.save_model()  # Saves the tokenizer too for easy upload
+
+        trainer.log_metrics("train", metrics)
+        trainer.save_metrics("train", metrics)
+        trainer.save_state()
+
+    # Evaluation
+    if training_args.do_eval:
+        logger.info("*** Evaluate ***")
+
+        # Loop to handle MNLI double evaluation (matched, mis-matched)
+        tasks = [data_args.task_name]
+        eval_datasets = [eval_dataset]
+        if data_args.task_name == "mnli":
+            tasks.append("mnli-mm")
+            valid_mm_dataset = raw_datasets["validation_mismatched"]
+            if data_args.max_eval_samples is not None:
+                max_eval_samples = min(len(valid_mm_dataset), data_args.max_eval_samples)
+                valid_mm_dataset = valid_mm_dataset.select(range(max_eval_samples))
+            eval_datasets.append(valid_mm_dataset)
+            combined = {}
+
+        for eval_dataset, task in zip(eval_datasets, tasks):
+            metrics = trainer.evaluate(eval_dataset=eval_dataset)
+
+            max_eval_samples = (
+                data_args.max_eval_samples if data_args.max_eval_samples is not None else len(eval_dataset)
+            )
+            metrics["eval_samples"] = min(max_eval_samples, len(eval_dataset))
+
+            if task == "mnli-mm":
+                metrics = {k + "_mm": v for k, v in metrics.items()}
+            if task is not None and "mnli" in task:
+                combined.update(metrics)
+
+            trainer.log_metrics("eval", metrics)
+            trainer.save_metrics("eval", combined if task is not None and "mnli" in task else metrics)
+
+    if training_args.do_predict:
+        logger.info("*** Predict ***")
+
+        # Loop to handle MNLI double evaluation (matched, mis-matched)
+        tasks = [data_args.task_name]
+        predict_datasets = [predict_dataset]
+        if data_args.task_name == "mnli":
+            tasks.append("mnli-mm")
+            predict_datasets.append(raw_datasets["test_mismatched"])
+
+        for predict_dataset, task in zip(predict_datasets, tasks):
+            # Removing the `label` columns because it contains -1 and Trainer won't like that.
+            predict_dataset = predict_dataset.remove_columns("label")
+            predictions = trainer.predict(predict_dataset, metric_key_prefix="predict").predictions
+            predictions = np.squeeze(predictions) if is_regression else np.argmax(predictions, axis=1)
+
+            output_predict_file = os.path.join(training_args.output_dir, f"predict_results_{task}.txt")
+            if trainer.is_world_process_zero():
+                with open(output_predict_file, "w") as writer:
+                    logger.info(f"***** Predict results {task} *****")
+                    writer.write("index\tprediction\n")
+                    for index, item in enumerate(predictions):
+                        if is_regression:
+                            writer.write(f"{index}\t{item:3.3f}\n")
+                        else:
+                            item = label_list[item]
+                            writer.write(f"{index}\t{item}\n")
+
+    kwargs = {"finetuned_from": model_args.model_name_or_path, "tasks": "text-classification"}
+    if data_args.task_name is not None:
+        kwargs["language"] = "en"
+        kwargs["dataset_tags"] = "glue"
+        kwargs["dataset_args"] = data_args.task_name
+        kwargs["dataset"] = f"GLUE {data_args.task_name.upper()}"
+
+    if training_args.push_to_hub:
+        trainer.push_to_hub(**kwargs)
+    else:
+        trainer.create_model_card(**kwargs)
+
+
+def _mp_fn(index):
+    # For xla_spawn (TPUs)
+    main()
 
-    trainer.log_metrics("train", metrics)
-    trainer.save_metrics("train", metrics)
-    trainer.save_state()
 
 if __name__ == "__main__":
     main()
```

### Comparing `HiFT-0.0.1/examples/run_glue.py` & `HiFT-0.0.2/examples/run_ner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,175 @@
 #!/usr/bin/env python
 # coding=utf-8
-# Copyright 2020 The HuggingFace Inc. team. All rights reserved.
+# Copyright 2020 The HuggingFace Team All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Finetuning the library models for sequence classification on GLUE."""
-# You can also adapt this script on your own text classification task. Pointers for this are left as comments.
+"""
+Fine-tuning the library models for token classification.
+"""
+# You can also adapt this script on your own token classification task and datasets. Pointers for this are left as
+# comments.
 
 import logging
 import os
-import random
 import sys
 import warnings
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Union
+from typing import Optional,Tuple,List
+
 import datasets
 import evaluate
 import numpy as np
-from datasets import load_dataset
+from datasets import ClassLabel, load_dataset
 
 import transformers
 from transformers import (
     AutoConfig,
-    AutoModelForSequenceClassification,
+    AutoModelForTokenClassification,
     AutoTokenizer,
-    DataCollatorWithPadding,
-    EvalPrediction,
+    DataCollatorForTokenClassification,
     HfArgumentParser,
     PretrainedConfig,
-    Trainer,
+    PreTrainedTokenizerFast,
     TrainingArguments,
-    default_data_collator,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
 from transformers.utils import check_min_version, send_example_telemetry
 from transformers.utils.versions import require_version
 
-from peft import (
-    PeftType,
-    LoraConfig,
-    TaskType,
-    get_peft_model
-)
-
 sys.path.append(os.path.abspath('.'))
-from hift import HiFTrainer,GetCallBack
+from hift import HiFTrainer,GetCallBack,PEFTrainer,peft_function
+from peft import PeftModel, get_peft_model_state_dict
+
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
 check_min_version("4.36.0")
 
-require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/text-classification/requirements.txt")
-
-task_to_keys = {
-    "cola": ("sentence", None),
-    "mnli": ("premise", "hypothesis"),
-    "mrpc": ("sentence1", "sentence2"),
-    "qnli": ("question", "sentence"),
-    "qqp": ("question1", "question2"),
-    "rte": ("sentence1", "sentence2"),
-    "sst2": ("sentence", None),
-    "stsb": ("sentence1", "sentence2"),
-    "wnli": ("sentence1", "sentence2"),
-}
+require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/token-classification/requirements.txt")
 
 logger = logging.getLogger(__name__)
 
+
 @dataclass
-class DataTrainingArguments:
+class ModelArguments:
     """
-    Arguments pertaining to what data we are going to input our model for training and eval.
-
-    Using `HfArgumentParser` we can turn this class
-    into argparse arguments to be able to specify them on
-    the command line.
+    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
     """
 
-    task_name: Optional[str] = field(
+    model_name_or_path: str = field(
+        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
+    )
+    config_name: Optional[str] = field(
+        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
+    )
+    tokenizer_name: Optional[str] = field(
+        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
+    )
+    cache_dir: Optional[str] = field(
+        default=None,
+        metadata={"help": "Where do you want to store the pretrained models downloaded from huggingface.co"},
+    )
+    model_revision: str = field(
+        default="main",
+        metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
+    )
+    token: str = field(
+        default=None,
+        metadata={
+            "help": (
+                "The token to use as HTTP bearer authorization for remote files. If not specified, will use the token "
+                "generated when running `huggingface-cli login` (stored in `~/.huggingface`)."
+            )
+        },
+    )
+    use_auth_token: bool = field(
         default=None,
-        metadata={"help": "The name of the task to train on: " + ", ".join(task_to_keys.keys())},
+        metadata={
+            "help": "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead."
+        },
+    )
+    trust_remote_code: bool = field(
+        default=False,
+        metadata={
+            "help": (
+                "Whether or not to allow for custom models defined on the Hub in their own modeling files. This option"
+                "should only be set to `True` for repositories you trust and in which you have read the code, as it will "
+                "execute code present on the Hub on your local machine."
+            )
+        },
     )
+    ignore_mismatched_sizes: bool = field(
+        default=False,
+        metadata={"help": "Will enable to load a pretrained model whose head dimensions are different."},
+    )
+
+
+@dataclass
+class DataTrainingArguments:
+    """
+    Arguments pertaining to what data we are going to input our model for training and eval.
+    """
+
+    task_name: Optional[str] = field(default="ner", metadata={"help": "The name of the task (ner, pos...)."})
     dataset_name: Optional[str] = field(
         default=None, metadata={"help": "The name of the dataset to use (via the datasets library)."}
     )
     dataset_config_name: Optional[str] = field(
         default=None, metadata={"help": "The configuration name of the dataset to use (via the datasets library)."}
     )
+    train_file: Optional[str] = field(
+        default=None, metadata={"help": "The input training data file (a csv or JSON file)."}
+    )
+    validation_file: Optional[str] = field(
+        default=None,
+        metadata={"help": "An optional input evaluation data file to evaluate on (a csv or JSON file)."},
+    )
+    test_file: Optional[str] = field(
+        default=None,
+        metadata={"help": "An optional input test data file to predict on (a csv or JSON file)."},
+    )
+    text_column_name: Optional[str] = field(
+        default=None, metadata={"help": "The column name of text to input in the file (a csv or JSON file)."}
+    )
+    label_column_name: Optional[str] = field(
+        default=None, metadata={"help": "The column name of label to input in the file (a csv or JSON file)."}
+    )
+    overwrite_cache: bool = field(
+        default=False, metadata={"help": "Overwrite the cached training and evaluation sets"}
+    )
+    preprocessing_num_workers: Optional[int] = field(
+        default=None,
+        metadata={"help": "The number of processes to use for the preprocessing."},
+    )
     max_seq_length: int = field(
-        default=128,
+        default=None,
         metadata={
             "help": (
-                "The maximum total input sequence length after tokenization. Sequences longer "
+                "The maximum total input sequence length after tokenization. If set, sequences longer "
                 "than this will be truncated, sequences shorter will be padded."
             )
         },
     )
-    overwrite_cache: bool = field(
-        default=False, metadata={"help": "Overwrite the cached preprocessed datasets or not."}
-    )
     pad_to_max_length: bool = field(
-        default=True,
+        default=False,
         metadata={
             "help": (
-                "Whether to pad all samples to `max_seq_length`. "
-                "If False, will pad the samples dynamically when batching to the maximum length in the batch."
+                "Whether to pad all samples to model maximum sentence length. "
+                "If False, will pad the samples dynamically when batching to the maximum length in the batch. More "
+                "efficient on GPU but very bad for TPU."
             )
         },
     )
     max_train_samples: Optional[int] = field(
         default=None,
         metadata={
             "help": (
@@ -138,102 +192,66 @@
         metadata={
             "help": (
                 "For debugging purposes or quicker training, truncate the number of prediction examples to this "
                 "value if set."
             )
         },
     )
-    train_file: Optional[str] = field(
-        default=None, metadata={"help": "A csv or a json file containing the training data."}
+    label_all_tokens: bool = field(
+        default=False,
+        metadata={
+            "help": (
+                "Whether to put the label for one word on all tokens of generated by that word or just on the "
+                "one (in which case the other tokens will have a padding index)."
+            )
+        },
     )
-    validation_file: Optional[str] = field(
-        default=None, metadata={"help": "A csv or a json file containing the validation data."}
+    return_entity_level_metrics: bool = field(
+        default=False,
+        metadata={"help": "Whether to return all the entity levels during evaluation or just the overall ones."},
     )
-    test_file: Optional[str] = field(default=None, metadata={"help": "A csv or a json file containing the test data."})
 
     def __post_init__(self):
-        if self.task_name is not None:
-            self.task_name = self.task_name.lower()
-            if self.task_name not in task_to_keys.keys():
-                raise ValueError("Unknown task, you should pick one in " + ",".join(task_to_keys.keys()))
-        elif self.dataset_name is not None:
-            pass
-        elif self.train_file is None or self.validation_file is None:
-            raise ValueError("Need either a GLUE task, a training/validation file or a dataset name.")
+        if self.dataset_name is None and self.train_file is None and self.validation_file is None:
+            raise ValueError("Need either a dataset name or a training/validation file.")
         else:
-            train_extension = self.train_file.split(".")[-1]
-            assert train_extension in ["csv", "json"], "`train_file` should be a csv or a json file."
-            validation_extension = self.validation_file.split(".")[-1]
-            assert (
-                validation_extension == train_extension
-            ), "`validation_file` should have the same extension (csv or json) as `train_file`."
-
+            if self.train_file is not None:
+                extension = self.train_file.split(".")[-1]
+                assert extension in ["csv", "json"], "`train_file` should be a csv or a json file."
+            if self.validation_file is not None:
+                extension = self.validation_file.split(".")[-1]
+                assert extension in ["csv", "json"], "`validation_file` should be a csv or a json file."
+        self.task_name = self.task_name.lower()
 
 @dataclass
-class ModelArguments:
-    """
-    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
-    """
-
-    model_name_or_path: str = field(
-        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
-    )
-    config_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
-    )
-    tokenizer_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
-    )
-    cache_dir: Optional[str] = field(
-        default=None,
-        metadata={"help": "Where do you want to store the pretrained models downloaded from huggingface.co"},
-    )
-    use_fast_tokenizer: bool = field(
-        default=True,
-        metadata={"help": "Whether to use one of the fast tokenizer (backed by the tokenizers library) or not."},
-    )
-    model_revision: str = field(
-        default="main",
-        metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
-    )
-    token: str = field(
-        default=None,
-        metadata={
-            "help": (
-                "The token to use as HTTP bearer authorization for remote files. If not specified, will use the token "
-                "generated when running `huggingface-cli login` (stored in `~/.huggingface`)."
-            )
-        },
+class HiFTArguments(ModelArguments):
+    HiTaskType: str = field(
+        default="TOKEN_CLS",
+        metadata={"help": ("HiTaskType should be consistent with PEFT TaskType" )},
     )
-    use_auth_token: bool = field(
+    peft_type: str = field(
         default=None,
-        metadata={
-            "help": "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead."
-        },
+        metadata={"help": ("peft_type should be in [lora,adalora,ia3,p_tuning,prefix_tuning,prompt_tuning]" )},
     )
-    trust_remote_code: bool = field(
-        default=False,
+    init_text:str = field(
+        default="Predict if sentiment of this review is positive, negative or neutral",
         metadata={
             "help": (
-                "Whether or not to allow for custom models defined on the Hub in their own modeling files. This option"
-                "should only be set to `True` for repositories you trust and in which you have read the code, as it will "
-                "execute code present on the Hub on your local machine."
+                "the init prompt text for prompt tuning"
             )
         },
     )
-    ignore_mismatched_sizes: bool = field(
-        default=False,
-        metadata={"help": "Will enable to load a pretrained model whose head dimensions are different."},
+    lora_rank: int = field(
+        default=8,
+        metadata={"help": ("rank for lora or adalora" )},
     )
-
-@dataclass
-class HiFTArguments(ModelArguments):
-    HiTaskType: str = field(
-        default="SEQ_CLS",
-        metadata={"help": ("HiTaskType should be consistent with PEFT TaskType" )},
+    peft_path : Optional[str] = field(default=None)
+    virtual_tokens:int = field(
+        default=20,
+        metadata={"help": ("the number of virtual tokens for p_tuning, prefix_tuning and prefix_tuning" )},
     )
     group_element: int = field(
         default=1,
         metadata={"help": ("number element for each group parameters" )},
     )
     optimizer_strategy: str = field(
         default="down2up",
@@ -243,33 +261,42 @@
         default=False,
         metadata={
             "help": (
                 "hierarchical optimization for LLMS"
             )
         },
     )
-    lora_tuning:bool = field(
-        default=False,
-        metadata={
-            "help": (
-                "whether using lora tuning"
-            )
-        },
-    )
     freeze_layers: List[str] = field(
         default_factory=list,
         metadata={
             "help": (
                 "Index of the frozen layer"
             )
         },
     )
-def AutoModelClassification(model_name_path):
-    
-    return (AutoModelForSequenceClassification,AutoTokenizer,AutoConfig)
+
+class SavePeftModelCallback(transformers.TrainerCallback):
+    def save_model(self, args, state, kwargs):
+        if state.best_model_checkpoint is not None:
+            checkpoint_folder = os.path.join(state.best_model_checkpoint, "peft_model")
+        else:
+            checkpoint_folder = os.path.join(args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{state.global_step}")
+
+        peft_model_path = os.path.join(checkpoint_folder, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
+
+    def on_save(self, args, state, control, **kwargs):
+        self.save_model(args, state, kwargs)
+        return control
+
+    def on_train_end(self, args, state, control, **kwargs):
+        peft_model_path = os.path.join(args.output_dir, "peft_model")
+        kwargs["model"].save_pretrained(peft_model_path)
+        kwargs["tokenizer"].save_pretrained(peft_model_path)
 
 def main():
     # See all possible arguments in src/transformers/training_args.py
     # or by passing the --help flag to this script.
     # We now keep distinct sets of args, for a cleaner separation of concerns.
 
     parser = HfArgumentParser((HiFTArguments, DataTrainingArguments, TrainingArguments))
@@ -284,27 +311,19 @@
         warnings.warn(
             "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead.",
             FutureWarning,
         )
         if model_args.token is not None:
             raise ValueError("`token` and `use_auth_token` are both specified. Please set only the argument `token`.")
         model_args.token = model_args.use_auth_token
+
     # Sending telemetry. Tracking the example usage helps us better allocate resources to maintain them. The
     # information sent is the one passed as arguments along with your Python/PyTorch versions.
-    send_example_telemetry("run_glue", model_args, data_args)
-    # #TODO: wandb
-    # # ======wandb config====
-    # os.environ['WANDB_PROJECT'] = model_args.model_name_or_path.split('/')[-1] + '_glue_' + data_args.task_name
-    # if model_args.hier_tuning is False:
-    #     os.environ['WANDB_RUN_NAME'] = f"normal_finetuning"
-    # else:
-    #     os.environ['WANDB_RUN_NAME'] = f"htune_{model_args.optimizer_strategy}_group{model_args.group_element}"
-    #     if model_args.hier_reverse:
-    #         os.environ['WANDB_RUN_NAME'] += "_rev"
-    # os.environ['WANDB_RUN_NAME'] += f"_v{random.randint(a=100, b=999)}"
+    send_example_telemetry("run_ner", model_args, data_args)
+
     # Setup logging
     logging.basicConfig(
         format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
         datefmt="%m/%d/%Y %H:%M:%S",
         handlers=[logging.StreamHandler(sys.stdout)],
     )
 
@@ -340,390 +359,405 @@
                 f"Checkpoint detected, resuming training at {last_checkpoint}. To avoid this behavior, change "
                 "the `--output_dir` or add `--overwrite_output_dir` to train from scratch."
             )
 
     # Set seed before initializing model.
     set_seed(training_args.seed)
 
-    # Get the datasets: you can either provide your own CSV/JSON training and evaluation files (see below)
-    # or specify a GLUE benchmark task (the dataset will be downloaded automatically from the datasets Hub).
-    #
-    # For CSV/JSON files, this script will use as labels the column called 'label' and as pair of sentences the
-    # sentences in columns called 'sentence1' and 'sentence2' if such column exists or the first two columns not named
-    # label if at least two columns are provided.
+    # Get the datasets: you can either provide your own CSV/JSON/TXT training and evaluation files (see below)
+    # or just provide the name of one of the public datasets available on the hub at https://huggingface.co/datasets/
+    # (the dataset will be downloaded automatically from the datasets Hub).
     #
-    # If the CSVs/JSONs contain only one non-label column, the script does single sentence classification on this
-    # single column. You can easily tweak this behavior (see below)
+    # For CSV/JSON files, this script will use the column called 'text' or the first column if no column called
+    # 'text' is found. You can easily tweak this behavior (see below).
     #
     # In distributed training, the load_dataset function guarantee that only one local process can concurrently
     # download the dataset.
-    if data_args.task_name is not None:
-        # Downloading and loading a dataset from the hub.
-        raw_datasets = load_dataset(
-            "glue",
-            data_args.task_name,
-            cache_dir=model_args.cache_dir,
-            token=model_args.token,
-        )
-    elif data_args.dataset_name is not None:
+    if data_args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             token=model_args.token,
         )
     else:
-        # Loading a dataset from your local files.
-        # CSV/JSON training and evaluation files are needed.
-        data_files = {"train": data_args.train_file, "validation": data_args.validation_file}
-
-        # Get the test dataset: you can provide your own CSV/JSON test file (see below)
-        # when you use `do_predict` without specifying a GLUE benchmark task.
-        if training_args.do_predict:
-            if data_args.test_file is not None:
-                train_extension = data_args.train_file.split(".")[-1]
-                test_extension = data_args.test_file.split(".")[-1]
-                assert (
-                    test_extension == train_extension
-                ), "`test_file` should have the same extension (csv or json) as `train_file`."
-                data_files["test"] = data_args.test_file
-            else:
-                raise ValueError("Need either a GLUE task or a test file for `do_predict`.")
+        data_files = {}
+        if data_args.train_file is not None:
+            data_files["train"] = data_args.train_file
+        if data_args.validation_file is not None:
+            data_files["validation"] = data_args.validation_file
+        if data_args.test_file is not None:
+            data_files["test"] = data_args.test_file
+        extension = data_args.train_file.split(".")[-1]
+        raw_datasets = load_dataset(extension, data_files=data_files, cache_dir=model_args.cache_dir)
+    # See more about loading any type of standard or custom dataset (from files, python dict, pandas DataFrame, etc) at
+    # https://huggingface.co/docs/datasets/loading_datasets.
 
-        for key in data_files.keys():
-            logger.info(f"load a local file for {key}: {data_files[key]}")
+    if training_args.do_train:
+        column_names = raw_datasets["train"].column_names
+        features = raw_datasets["train"].features
+    else:
+        column_names = raw_datasets["validation"].column_names
+        features = raw_datasets["validation"].features
 
-        if data_args.train_file.endswith(".csv"):
-            # Loading a dataset from local csv files
-            raw_datasets = load_dataset(
-                "csv",
-                data_files=data_files,
-                cache_dir=model_args.cache_dir,
-                token=model_args.token,
-            )
-        else:
-            # Loading a dataset from local json files
-            raw_datasets = load_dataset(
-                "json",
-                data_files=data_files,
-                cache_dir=model_args.cache_dir,
-                token=model_args.token,
-            )
-    # See more about loading any type of standard or custom dataset at
-    # https://huggingface.co/docs/datasets/loading_datasets.
+    if data_args.text_column_name is not None:
+        text_column_name = data_args.text_column_name
+    elif "tokens" in column_names:
+        text_column_name = "tokens"
+    else:
+        text_column_name = column_names[0]
 
-    # Labels
-    if data_args.task_name is not None:
-        is_regression = data_args.task_name == "stsb"
-        if not is_regression:
-            label_list = raw_datasets["train"].features["label"].names
-            num_labels = len(label_list)
-        else:
-            num_labels = 1
+    if data_args.label_column_name is not None:
+        label_column_name = data_args.label_column_name
+    elif f"{data_args.task_name}_tags" in column_names:
+        label_column_name = f"{data_args.task_name}_tags"
     else:
-        # Trying to have good defaults here, don't hesitate to tweak to your needs.
-        is_regression = raw_datasets["train"].features["label"].dtype in ["float32", "float64"]
-        if is_regression:
-            num_labels = 1
-        else:
-            # A useful fast method:
-            # https://huggingface.co/docs/datasets/package_reference/main_classes#datasets.Dataset.unique
-            label_list = raw_datasets["train"].unique("label")
-            label_list.sort()  # Let's sort it for determinism
-            num_labels = len(label_list)
+        label_column_name = column_names[1]
+
+    # In the event the labels are not a `Sequence[ClassLabel]`, we will need to go through the dataset to get the
+    # unique labels.
+    def get_label_list(labels):
+        unique_labels = set()
+        for label in labels:
+            unique_labels = unique_labels | set(label)
+        label_list = list(unique_labels)
+        label_list.sort()
+        return label_list
+
+    # If the labels are of type ClassLabel, they are already integers and we have the map stored somewhere.
+    # Otherwise, we have to get the list of labels manually.
+    labels_are_int = isinstance(features[label_column_name].feature, ClassLabel)
+    if labels_are_int:
+        label_list = features[label_column_name].feature.names
+        label_to_id = {i: i for i in range(len(label_list))}
+    else:
+        label_list = get_label_list(raw_datasets["train"][label_column_name])
+        label_to_id = {l: i for i, l in enumerate(label_list)}
+
+    num_labels = len(label_list)
 
     # Load pretrained model and tokenizer
     #
-    # In distributed training, the .from_pretrained methods guarantee that only one local process can concurrently
+    # Distributed training:
+    # The .from_pretrained methods guarantee that only one local process can concurrently
     # download model & vocab.
     config = AutoConfig.from_pretrained(
         model_args.config_name if model_args.config_name else model_args.model_name_or_path,
         num_labels=num_labels,
         finetuning_task=data_args.task_name,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
         token=model_args.token,
         trust_remote_code=model_args.trust_remote_code,
     )
-    config.gradient_checkpointing = training_args.gradient_checkpointing
-    tokenizer = AutoTokenizer.from_pretrained(
-        model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
-        cache_dir=model_args.cache_dir,
-        use_fast=model_args.use_fast_tokenizer,
-        revision=model_args.model_revision,
-        token=model_args.token,
-        trust_remote_code=model_args.trust_remote_code,
-    )
-    if tokenizer.pad_token is None:
-        tokenizer.pad_token = tokenizer.eos_token
-    if config.pad_token_id is None:
-        config.pad_token_id = tokenizer.eos_token_id
-    model = AutoModelForSequenceClassification.from_pretrained(
+
+    tokenizer_name_or_path = model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path
+    if config.model_type in {"bloom", "gpt2", "roberta"}:
+        tokenizer = AutoTokenizer.from_pretrained(
+            tokenizer_name_or_path,
+            cache_dir=model_args.cache_dir,
+            use_fast=True,
+            revision=model_args.model_revision,
+            token=model_args.token,
+            trust_remote_code=model_args.trust_remote_code,
+            add_prefix_space=True,
+        )
+    else:
+        tokenizer = AutoTokenizer.from_pretrained(
+            tokenizer_name_or_path,
+            cache_dir=model_args.cache_dir,
+            use_fast=True,
+            revision=model_args.model_revision,
+            token=model_args.token,
+            trust_remote_code=model_args.trust_remote_code,
+        )
+
+    model = AutoModelForTokenClassification.from_pretrained(
         model_args.model_name_or_path,
         from_tf=bool(".ckpt" in model_args.model_name_or_path),
         config=config,
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
         token=model_args.token,
         trust_remote_code=model_args.trust_remote_code,
         ignore_mismatched_sizes=model_args.ignore_mismatched_sizes,
     )
-    if model_args.lora_tuning:
-        peft_config = LoraConfig(
-            peft_type = PeftType.LORA,
-            lora_alpha=16,
-            lora_dropout=0.1,
-            r=8,
-            bias="none",
-            task_type=TaskType.SEQ_CLS)
-        model = get_peft_model(model, peft_config)
-    # Preprocessing the raw_datasets
-    if data_args.task_name is not None:
-        sentence1_key, sentence2_key = task_to_keys[data_args.task_name]
-    else:
-        # Again, we try to have some nice defaults but don't hesitate to tweak to your use case.
-        non_label_column_names = [name for name in raw_datasets["train"].column_names if name != "label"]
-        if "sentence1" in non_label_column_names and "sentence2" in non_label_column_names:
-            sentence1_key, sentence2_key = "sentence1", "sentence2"
-        else:
-            if len(non_label_column_names) >= 2:
-                sentence1_key, sentence2_key = non_label_column_names[:2]
-            else:
-                sentence1_key, sentence2_key = non_label_column_names[0], None
 
-    # Padding strategy
-    if data_args.pad_to_max_length:
-        padding = "max_length"
-    else:
-        # We will pad later, dynamically at batch creation, to the max sequence length in each batch
-        padding = False
+    if model_args.peft_type:
+        if model_args.peft_path is not None:
+            logger.info("Peft from pre-trained model")
+            model = PeftModel.from_pretrained(model, model_args.peft_path)
+        else:
+            model = peft_function(model,
+                    config = config,
+                    peft_type = model_args.peft_type,
+                    task_type = model_args.HiTaskType,
+                    rank=model_args.lora_rank,
+                    virtual_tokens=model_args.virtual_tokens,
+                    tokenizer_name_or_path=model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
+                    init_text=model_args.init_text if model_args.peft_type=="prompt_tuning" else None,
+                    peft_config=None)
+    # Tokenizer check: this script requires a fast tokenizer.
+    if not isinstance(tokenizer, PreTrainedTokenizerFast):
+        raise ValueError(
+            "This example script only works for models that have a fast tokenizer. Checkout the big table of models at"
+            " https://huggingface.co/transformers/index.html#supported-frameworks to find the model types that meet"
+            " this requirement"
+        )
 
-    # Some models have set the order of the labels to use, so let's make sure we do use it.
-    label_to_id = None
-    if (
-        model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id
-        and data_args.task_name is not None
-        and not is_regression
-    ):
-        # Some have all caps in their config, some don't.
-        label_name_to_id = {k.lower(): v for k, v in model.config.label2id.items()}
-        if sorted(label_name_to_id.keys()) == sorted(label_list):
-            label_to_id = {i: int(label_name_to_id[label_list[i]]) for i in range(num_labels)}
+    # Model has labels -> use them.
+    if model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id:
+        if sorted(model.config.label2id.keys()) == sorted(label_list):
+            # Reorganize `label_list` to match the ordering of the model.
+            if labels_are_int:
+                label_to_id = {i: int(model.config.label2id[l]) for i, l in enumerate(label_list)}
+                label_list = [model.config.id2label[i] for i in range(num_labels)]
+            else:
+                label_list = [model.config.id2label[i] for i in range(num_labels)]
+                label_to_id = {l: i for i, l in enumerate(label_list)}
         else:
             logger.warning(
                 "Your model seems to have been trained with labels, but they don't match the dataset: ",
-                f"model labels: {sorted(label_name_to_id.keys())}, dataset labels: {sorted(label_list)}."
-                "\nIgnoring the model labels as a result.",
+                f"model labels: {sorted(model.config.label2id.keys())}, dataset labels:"
+                f" {sorted(label_list)}.\nIgnoring the model labels as a result.",
             )
-    elif data_args.task_name is None and not is_regression:
-        label_to_id = {v: i for i, v in enumerate(label_list)}
 
-    if label_to_id is not None:
-        model.config.label2id = label_to_id
-        model.config.id2label = {id: label for label, id in config.label2id.items()}
-    elif data_args.task_name is not None and not is_regression:
-        model.config.label2id = {l: i for i, l in enumerate(label_list)}
-        model.config.id2label = {id: label for label, id in config.label2id.items()}
-
-    if data_args.max_seq_length > tokenizer.model_max_length:
-        logger.warning(
-            f"The max_seq_length passed ({data_args.max_seq_length}) is larger than the maximum length for the "
-            f"model ({tokenizer.model_max_length}). Using max_seq_length={tokenizer.model_max_length}."
-        )
-    max_seq_length = min(data_args.max_seq_length, tokenizer.model_max_length)
+    # Set the correspondences label/ID inside the model config
+    model.config.label2id = {l: i for i, l in enumerate(label_list)}
+    model.config.id2label = dict(enumerate(label_list))
+
+    # Map that sends B-Xxx label to its I-Xxx counterpart
+    b_to_i_label = []
+    for idx, label in enumerate(label_list):
+        if label.startswith("B-") and label.replace("B-", "I-") in label_list:
+            b_to_i_label.append(label_list.index(label.replace("B-", "I-")))
+        else:
+            b_to_i_label.append(idx)
 
-    def preprocess_function(examples):
-        # Tokenize the texts
-        args = (
-            (examples[sentence1_key],) if sentence2_key is None else (examples[sentence1_key], examples[sentence2_key])
-        )
-        result = tokenizer(*args, padding=padding, max_length=max_seq_length, truncation=True)
+    # Preprocessing the dataset
+    # Padding strategy
+    padding = "max_length" if data_args.pad_to_max_length else False
 
-        # Map labels to IDs (not necessary for GLUE tasks)
-        if label_to_id is not None and "label" in examples:
-            result["label"] = [(label_to_id[l] if l != -1 else -1) for l in examples["label"]]
-        return result
-
-    with training_args.main_process_first(desc="dataset map pre-processing"):
-        raw_datasets = raw_datasets.map(
-            preprocess_function,
-            batched=True,
-            load_from_cache_file=not data_args.overwrite_cache,
-            desc="Running tokenizer on dataset",
+    # Tokenize all texts and align the labels with them.
+    def tokenize_and_align_labels(examples):
+        tokenized_inputs = tokenizer(
+            examples[text_column_name],
+            padding=padding,
+            truncation=True,
+            max_length=data_args.max_seq_length,
+            # We use this argument because the texts in our dataset are lists of words (with a label for each word).
+            is_split_into_words=True,
         )
+        labels = []
+        for i, label in enumerate(examples[label_column_name]):
+            word_ids = tokenized_inputs.word_ids(batch_index=i)
+            previous_word_idx = None
+            label_ids = []
+            for word_idx in word_ids:
+                # Special tokens have a word id that is None. We set the label to -100 so they are automatically
+                # ignored in the loss function.
+                if word_idx is None:
+                    label_ids.append(-100)
+                # We set the label for the first token of each word.
+                elif word_idx != previous_word_idx:
+                    label_ids.append(label_to_id[label[word_idx]])
+                # For the other tokens in a word, we set the label to either the current label or -100, depending on
+                # the label_all_tokens flag.
+                else:
+                    if data_args.label_all_tokens:
+                        label_ids.append(b_to_i_label[label_to_id[label[word_idx]]])
+                    else:
+                        label_ids.append(-100)
+                previous_word_idx = word_idx
+
+            labels.append(label_ids)
+        tokenized_inputs["labels"] = labels
+        return tokenized_inputs
+
     if training_args.do_train:
         if "train" not in raw_datasets:
             raise ValueError("--do_train requires a train dataset")
         train_dataset = raw_datasets["train"]
         if data_args.max_train_samples is not None:
             max_train_samples = min(len(train_dataset), data_args.max_train_samples)
             train_dataset = train_dataset.select(range(max_train_samples))
+        with training_args.main_process_first(desc="train dataset map pre-processing"):
+            train_dataset = train_dataset.map(
+                tokenize_and_align_labels,
+                batched=True,
+                num_proc=data_args.preprocessing_num_workers,
+                load_from_cache_file=not data_args.overwrite_cache,
+                desc="Running tokenizer on train dataset",
+            )
 
     if training_args.do_eval:
-        if "validation" not in raw_datasets and "validation_matched" not in raw_datasets:
+        if "validation" not in raw_datasets:
             raise ValueError("--do_eval requires a validation dataset")
-        eval_dataset = raw_datasets["validation_matched" if data_args.task_name == "mnli" else "validation"]
+        eval_dataset = raw_datasets["validation"]
         if data_args.max_eval_samples is not None:
             max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
             eval_dataset = eval_dataset.select(range(max_eval_samples))
+        with training_args.main_process_first(desc="validation dataset map pre-processing"):
+            eval_dataset = eval_dataset.map(
+                tokenize_and_align_labels,
+                batched=True,
+                num_proc=data_args.preprocessing_num_workers,
+                load_from_cache_file=not data_args.overwrite_cache,
+                desc="Running tokenizer on validation dataset",
+            )
 
-    if training_args.do_predict or data_args.task_name is not None or data_args.test_file is not None:
-        if "test" not in raw_datasets and "test_matched" not in raw_datasets:
+    if training_args.do_predict:
+        if "test" not in raw_datasets:
             raise ValueError("--do_predict requires a test dataset")
-        predict_dataset = raw_datasets["test_matched" if data_args.task_name == "mnli" else "test"]
+        predict_dataset = raw_datasets["test"]
         if data_args.max_predict_samples is not None:
             max_predict_samples = min(len(predict_dataset), data_args.max_predict_samples)
             predict_dataset = predict_dataset.select(range(max_predict_samples))
+        with training_args.main_process_first(desc="prediction dataset map pre-processing"):
+            predict_dataset = predict_dataset.map(
+                tokenize_and_align_labels,
+                batched=True,
+                num_proc=data_args.preprocessing_num_workers,
+                load_from_cache_file=not data_args.overwrite_cache,
+                desc="Running tokenizer on prediction dataset",
+            )
+
+    # Data collator
+    data_collator = DataCollatorForTokenClassification(tokenizer, pad_to_multiple_of=8 if training_args.fp16 else None)
+
+    # Metrics
+    metric = evaluate.load("seqeval")
+
+    def compute_metrics(p):
+        predictions, labels = p
+        predictions = np.argmax(predictions, axis=2)
+
+        # Remove ignored index (special tokens)
+        true_predictions = [
+            [label_list[p] for (p, l) in zip(prediction, label) if l != -100]
+            for prediction, label in zip(predictions, labels)
+        ]
+        true_labels = [
+            [label_list[l] for (p, l) in zip(prediction, label) if l != -100]
+            for prediction, label in zip(predictions, labels)
+        ]
+
+        results = metric.compute(predictions=true_predictions, references=true_labels)
+        if data_args.return_entity_level_metrics:
+            # Unpack nested dictionaries
+            final_results = {}
+            for key, value in results.items():
+                if isinstance(value, dict):
+                    for n, v in value.items():
+                        final_results[f"{key}_{n}"] = v
+                else:
+                    final_results[key] = value
+            return final_results
+        else:
+            return {
+                "precision": results["overall_precision"],
+                "recall": results["overall_recall"],
+                "f1": results["overall_f1"],
+                "accuracy": results["overall_accuracy"],
+            }
 
-    # Log a few random samples from the training set:
-    if training_args.do_train:
-        for index in random.sample(range(len(train_dataset)), 3):
-            logger.info(f"Sample {index} of the training set: {train_dataset[index]}.")
-
-    # Get the metric function
-    if data_args.task_name is not None:
-        metric = evaluate.load("glue", data_args.task_name)
-    elif is_regression:
-        metric = evaluate.load("mse")
-    else:
-        metric = evaluate.load("accuracy")
-
-    # You can define your custom compute_metrics function. It takes an `EvalPrediction` object (a namedtuple with a
-    # predictions and label_ids field) and has to return a dictionary string to float.
-    def compute_metrics(p: EvalPrediction):
-        preds = p.predictions[0] if isinstance(p.predictions, tuple) else p.predictions
-        preds = np.squeeze(preds) if is_regression else np.argmax(preds, axis=1)
-        result = metric.compute(predictions=preds, references=p.label_ids)
-        if len(result) > 1:
-            result["combined_score"] = np.mean(list(result.values())).item()
-        return result
-
-    # Data collator will default to DataCollatorWithPadding when the tokenizer is passed to Trainer, so we change it if
-    # we already did the padding.
-    if data_args.pad_to_max_length:
-        data_collator = default_data_collator
-    elif training_args.fp16:
-        data_collator = DataCollatorWithPadding(tokenizer, pad_to_multiple_of=8)
-    else:
-        data_collator = None
-    # Initialize HiFTrainer
-    if model_args.hier_tuning:#hier_tuning
+    # Initialize our Trainer
+    if model_args.hier_tuning:
         trainer = HiFTrainer(
             hiFThandler = GetCallBack(model_args.model_name_or_path),
             HiTaskType = model_args.HiTaskType,
             group_element = model_args.group_element,
             strategy = model_args.optimizer_strategy,
             hier_tuning= model_args.hier_tuning,
-            lora_tuning = model_args.lora_tuning,
+            peft_type = model_args.peft_type,
             freeze_layers = model_args.freeze_layers,
+            args=training_args,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
             model=model,
             tokenizer=tokenizer,
-            compute_metrics=compute_metrics,
             data_collator=data_collator,
-            args=training_args
+            compute_metrics=compute_metrics
         )
     else:
-        trainer = Trainer(
-            model=model,
+        trainer = PEFTrainer(
+            peft_type = model_args.peft_type,
             args=training_args,
+            model=model,
             train_dataset=train_dataset if training_args.do_train else None,
             eval_dataset=eval_dataset if training_args.do_eval else None,
-            compute_metrics=compute_metrics,
             tokenizer=tokenizer,
             data_collator=data_collator,
+            compute_metrics=compute_metrics,
         )
+
     # Training
     if training_args.do_train:
         checkpoint = None
         if training_args.resume_from_checkpoint is not None:
             checkpoint = training_args.resume_from_checkpoint
         elif last_checkpoint is not None:
             checkpoint = last_checkpoint
         train_result = trainer.train(resume_from_checkpoint=checkpoint)
         metrics = train_result.metrics
+        trainer.save_model()  # Saves the tokenizer too for easy upload
+
         max_train_samples = (
             data_args.max_train_samples if data_args.max_train_samples is not None else len(train_dataset)
         )
         metrics["train_samples"] = min(max_train_samples, len(train_dataset))
 
-        trainer.save_model()  # Saves the tokenizer too for easy upload
-
         trainer.log_metrics("train", metrics)
         trainer.save_metrics("train", metrics)
         trainer.save_state()
 
     # Evaluation
     if training_args.do_eval:
         logger.info("*** Evaluate ***")
 
-        # Loop to handle MNLI double evaluation (matched, mis-matched)
-        tasks = [data_args.task_name]
-        eval_datasets = [eval_dataset]
-        if data_args.task_name == "mnli":
-            tasks.append("mnli-mm")
-            valid_mm_dataset = raw_datasets["validation_mismatched"]
-            if data_args.max_eval_samples is not None:
-                max_eval_samples = min(len(valid_mm_dataset), data_args.max_eval_samples)
-                valid_mm_dataset = valid_mm_dataset.select(range(max_eval_samples))
-            eval_datasets.append(valid_mm_dataset)
-            combined = {}
-
-        for eval_dataset, task in zip(eval_datasets, tasks):
-            metrics = trainer.evaluate(eval_dataset=eval_dataset)
-
-            max_eval_samples = (
-                data_args.max_eval_samples if data_args.max_eval_samples is not None else len(eval_dataset)
-            )
-            metrics["eval_samples"] = min(max_eval_samples, len(eval_dataset))
-
-            if task == "mnli-mm":
-                metrics = {k + "_mm": v for k, v in metrics.items()}
-            if task is not None and "mnli" in task:
-                combined.update(metrics)
+        metrics = trainer.evaluate()
 
-            trainer.log_metrics("eval", metrics)
-            trainer.save_metrics("eval", combined if task is not None and "mnli" in task else metrics)
+        max_eval_samples = data_args.max_eval_samples if data_args.max_eval_samples is not None else len(eval_dataset)
+        metrics["eval_samples"] = min(max_eval_samples, len(eval_dataset))
 
+        trainer.log_metrics("eval", metrics)
+        trainer.save_metrics("eval", metrics)
+
+    # Predict
     if training_args.do_predict:
         logger.info("*** Predict ***")
 
-        # Loop to handle MNLI double evaluation (matched, mis-matched)
-        tasks = [data_args.task_name]
-        predict_datasets = [predict_dataset]
-        if data_args.task_name == "mnli":
-            tasks.append("mnli-mm")
-            predict_datasets.append(raw_datasets["test_mismatched"])
-
-        for predict_dataset, task in zip(predict_datasets, tasks):
-            # Removing the `label` columns because it contains -1 and Trainer won't like that.
-            predict_dataset = predict_dataset.remove_columns("label")
-            predictions = trainer.predict(predict_dataset, metric_key_prefix="predict").predictions
-            predictions = np.squeeze(predictions) if is_regression else np.argmax(predictions, axis=1)
-
-            output_predict_file = os.path.join(training_args.output_dir, f"predict_results_{task}.txt")
-            if trainer.is_world_process_zero():
-                with open(output_predict_file, "w") as writer:
-                    logger.info(f"***** Predict results {task} *****")
-                    writer.write("index\tprediction\n")
-                    for index, item in enumerate(predictions):
-                        if is_regression:
-                            writer.write(f"{index}\t{item:3.3f}\n")
-                        else:
-                            item = label_list[item]
-                            writer.write(f"{index}\t{item}\n")
-
-    kwargs = {"finetuned_from": model_args.model_name_or_path, "tasks": "text-classification"}
-    if data_args.task_name is not None:
-        kwargs["language"] = "en"
-        kwargs["dataset_tags"] = "glue"
-        kwargs["dataset_args"] = data_args.task_name
-        kwargs["dataset"] = f"GLUE {data_args.task_name.upper()}"
+        predictions, labels, metrics = trainer.predict(predict_dataset, metric_key_prefix="predict")
+        predictions = np.argmax(predictions, axis=2)
+
+        # Remove ignored index (special tokens)
+        true_predictions = [
+            [label_list[p] for (p, l) in zip(prediction, label) if l != -100]
+            for prediction, label in zip(predictions, labels)
+        ]
+
+        trainer.log_metrics("predict", metrics)
+        trainer.save_metrics("predict", metrics)
+
+        # Save predictions
+        output_predictions_file = os.path.join(training_args.output_dir, "predictions.txt")
+        if trainer.is_world_process_zero():
+            with open(output_predictions_file, "w") as writer:
+                for prediction in true_predictions:
+                    writer.write(" ".join(prediction) + "\n")
+
+    kwargs = {"finetuned_from": model_args.model_name_or_path, "tasks": "token-classification"}
+    if data_args.dataset_name is not None:
+        kwargs["dataset_tags"] = data_args.dataset_name
+        if data_args.dataset_config_name is not None:
+            kwargs["dataset_args"] = data_args.dataset_config_name
+            kwargs["dataset"] = f"{data_args.dataset_name} {data_args.dataset_config_name}"
+        else:
+            kwargs["dataset"] = data_args.dataset_name
 
     if training_args.push_to_hub:
         trainer.push_to_hub(**kwargs)
     else:
         trainer.create_model_card(**kwargs)
```

### Comparing `HiFT-0.0.1/hift/optimizers/adagrad.py` & `HiFT-0.0.2/hift/optimizers/adagrad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import torch
 from torch import Tensor
-
 from .optimizer import (Optimizer, _use_grad_for_differentiable, _get_value,
                         _default_to_fused_or_foreach, _differentiable_doc, _foreach_doc, _maximize_doc)
 from typing import List, Optional
 
 __all__ = ["Adagrad", "adagrad"]
```

### Comparing `HiFT-0.0.1/hift/optimizers/optimization.py` & `HiFT-0.0.2/hift/optimizers/optimization.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/hift/optimizers/replace_operation.py` & `HiFT-0.0.2/hift/optimizers/replace_operation.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,57 @@
 from deepspeed.runtime.fp16.loss_scaler import INITIAL_LOSS_SCALE, SCALE_WINDOW, MIN_LOSS_SCALE
 from deepspeed.utils import logger
 from deepspeed.checkpoint.constants import OPTIMIZER_STATE_DICT
 from deepspeed.accelerator import get_accelerator
 from deepspeed import comm as dist
 
 from deepspeed.runtime.fp16.unfused_optimizer import FP16_UnfusedOptimizer
+import transformers
+from transformers import training_args
+from transformers.training_args import OptimizerNames
+from transformers.utils import ExplicitEnum
+
+class ExtendOptimizerNames(ExplicitEnum):
+    ADAMW_HF = "adamw_hf"
+    ADAMW_TORCH = "adamw_torch"
+    ADAMW_TORCH_FUSED = "adamw_torch_fused"
+    ADAMW_TORCH_XLA = "adamw_torch_xla"
+    ADAMW_TORCH_NPU_FUSED = "adamw_torch_npu_fused"
+    ADAMW_APEX_FUSED = "adamw_apex_fused"
+    ADAFACTOR = "adafactor"
+    ADAMW_ANYPRECISION = "adamw_anyprecision"
+    SGD = "sgd"
+    ADAGRAD = "adagrad"
+    ADAMW_BNB = "adamw_bnb_8bit"
+    ADAMW_8BIT = "adamw_8bit"  # just an alias for adamw_bnb_8bit
+    LION_8BIT = "lion_8bit"
+    LION = "lion_32bit"
+    PAGED_ADAMW = "paged_adamw_32bit"
+    PAGED_ADAMW_8BIT = "paged_adamw_8bit"
+    PAGED_LION = "paged_lion_32bit"
+    PAGED_LION_8BIT = "paged_lion_8bit"
+    RMSPROP = "rmsprop"
+    #extend
+    LAMB ="lamb"
+    LAMB_32BIT = "lamb_32bit"
+    LAMB_8BIT = "lamb_8bit"
+    LARS = "lars"
+    LARS_32BIT = "lars_32bit"
+    LARS_8BIT = "lars_8bit"
+    BRMSPROP = "rmsprop_bit"
+    BRMSPROP_32BIT = "rmsprop_32bit"
+    BRMSPROP_8BIT = "rmsprop_8bit"
+    ADAGRAD_8BIT = "adagrad_8bit"
+    BSGD = "sgd_bit"
+    BSGD_32BIT = "sgd_32bit"
+    BSGD_8BIT = "sgd_8bit"
+    BADAGRAD = "adagrad_bit"
+    BADAGRAD_32BIT = "adagrad_32bit"
+    BADAGRAD_8BIT = "adagrad_8bit"
+
 
 
 def __init__(self,
     init_optimizer,
     deepspeed=None,
     static_loss_scale=1.0,
     dynamic_loss_scale=False,
@@ -121,14 +164,15 @@
         fp32_groups.append([self.fp32_groups[i][id(p)].to(p.device) for p in param_group['params']])
         for p in fp32_groups[i]:
             p.requires_grad = True
         for p_index,p in enumerate(param_group['params']):
             self.fp32_groups[i][id(p)] = fp32_groups[i][p_index]
             self.optimizer.add_id_mapping({fp32_groups[i][p_index]:id(p)})
         param_group['params'] = fp32_groups[i]
+    torch.cuda.empty_cache()
     return fp16_groups,fp32_groups
 def step(self, closure=None):
     """
     Not supporting closure.
     """
     fp16_groups = []
     fp32_groups = []
@@ -136,18 +180,22 @@
     if self.fused_lamb_legacy:
         return self.step_fused_lamb()
     self.overflow = self.overflow_checker.check(param_groups = fp16_groups)
     prev_scale = self.cur_scale
 
     self._update_scale(self.overflow)
     if self.overflow:
+        for fp16_group in fp16_groups:
+            for p in fp16_group:
+                noise = torch.randn_like(p.grad,dtype=p.grad.dtype)
+                p.grad = noise.to(p.device)
         if self.verbose:
             logger.info("[deepspeed] fp16 dynamic loss scale overflow! Skipping step. Attempted loss "
                             "scale: {}, reducing to {}".format(prev_scale, self.cur_scale))
-        return self.overflow
+        # return self.overflow
 
     norm_groups = []
     for i, group in enumerate(fp16_groups):
         grads_for_norm, _ = split_params_grads_into_shared_and_expert_params(group)
         norm_group_value = 0.0
         if len(grads_for_norm) > 0:
             norm_group_value = get_weight_norm(grads_for_norm, mpu=self.mpu)
@@ -217,8 +265,8 @@
     logger.info("...[deepspeed] mixed precision adapted for HiFT are running......")
     FP16_UnfusedOptimizer.__init__ = __init__
     FP16_UnfusedOptimizer.zero_grad = zero_grad
     FP16_UnfusedOptimizer.move_device = move_device
     FP16_UnfusedOptimizer.step = step
     FP16_UnfusedOptimizer.unscale_and_clip_grads =unscale_and_clip_grads
     FP16_UnfusedOptimizer.state_dict = state_dict
-    
+    # transformers.training_args.OptimizerNames = ExtendOptimizerNames
```

### Comparing `HiFT-0.0.1/hift/optimizers/rmsprop.py` & `HiFT-0.0.2/hift/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/hift/optimizers/sgd.py` & `HiFT-0.0.2/hift/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/hift/optimizers/torchAdam.py` & `HiFT-0.0.2/hift/optimizers/torchAdam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/hift/optimizers/torchAdamw.py` & `HiFT-0.0.2/hift/optimizers/torchAdamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.1/hift/seqtrainer.py` & `HiFT-0.0.2/hift/seqtrainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,39 +21,325 @@
 from torch.utils.data import Dataset
 
 from transformers import GenerationConfig
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 from transformers.trainer import Trainer
 from distutils.util import strtobool
 from transformers.utils import logging
-from .trainer import HiFTrainer
+from .trainer import HiFTrainer,PEFTrainer
 if TYPE_CHECKING:
     from transformers.data.data_collator import DataCollator
     from transformers.modeling_utils import PreTrainedModel
     from transformers.tokenization_utils_base import PreTrainedTokenizerBase
     from transformers.trainer_callback import TrainerCallback
     from transformers.trainer_utils import EvalPrediction, PredictionOutput
     from transformers.training_args import TrainingArguments
 
 
 logger = logging.get_logger(__name__)
 
+class Seq2SeqTrainer(PEFTrainer):
+    def __init__(self,peft_type=None,*args,**kwargs):
+        super().__init__(peft_type,*args, **kwargs)
+        # Override self.model.generation_config if a GenerationConfig is specified in args.
+        # Priority: args.generation_config > model.generation_config > default GenerationConfig.
+        if self.args.generation_config is not None:
+            gen_config = self.load_generation_config(self.args.generation_config)
+            self.model.generation_config = gen_config
+    @staticmethod
+    def load_generation_config(gen_config_arg: Union[str, GenerationConfig]) -> GenerationConfig:
+        """
+        Loads a `~generation.GenerationConfig` from the `Seq2SeqTrainingArguments.generation_config` arguments.
+
+        Args:
+            gen_config_arg (`str` or [`~generation.GenerationConfig`]):
+                `Seq2SeqTrainingArguments.generation_config` argument.
+
+        Returns:
+            A `~generation.GenerationConfig`.
+        """
+
+        # GenerationConfig provided, nothing to do
+        if isinstance(gen_config_arg, GenerationConfig):
+            return deepcopy(gen_config_arg)
+
+        # str or Path
+        pretrained_model_name = Path(gen_config_arg) if isinstance(gen_config_arg, str) else gen_config_arg
+        config_file_name = None
+
+        # Figuring if it is path pointing to a file, pointing to a directory or else a model id or URL
+        # This step is required in order to determine config_file_name
+        if pretrained_model_name.is_file():
+            config_file_name = pretrained_model_name.name
+            pretrained_model_name = pretrained_model_name.parent
+        # dir path
+        elif pretrained_model_name.is_dir():
+            pass
+        # model id or URL
+        else:
+            pretrained_model_name = gen_config_arg
+
+        gen_config = GenerationConfig.from_pretrained(pretrained_model_name, config_file_name)
+        return gen_config
+
+    def evaluate(
+        self,
+        eval_dataset: Optional[Dataset] = None,
+        ignore_keys: Optional[List[str]] = None,
+        metric_key_prefix: str = "eval",
+        **gen_kwargs,
+    ) -> Dict[str, float]:
+        """
+        Run evaluation and returns metrics.
+
+        The calling script will be responsible for providing a method to compute metrics, as they are task-dependent
+        (pass it to the init `compute_metrics` argument).
+
+        You can also subclass and override this method to inject custom behavior.
+
+        Args:
+            eval_dataset (`Dataset`, *optional*):
+                Pass a dataset if you wish to override `self.eval_dataset`. If it is an [`~datasets.Dataset`], columns
+                not accepted by the `model.forward()` method are automatically removed. It must implement the `__len__`
+                method.
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
+                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                "eval_bleu" if the prefix is `"eval"` (default)
+            max_length (`int`, *optional*):
+                The maximum target length to use when predicting with the generate method.
+            num_beams (`int`, *optional*):
+                Number of beams for beam search that will be used when predicting with the generate method. 1 means no
+                beam search.
+            gen_kwargs:
+                Additional `generate` specific kwargs.
+
+        Returns:
+            A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
+            dictionary also contains the epoch number which comes from the training state.
+        """
+
+        gen_kwargs = gen_kwargs.copy()
+
+        # Use legacy argument setting if a) the option is not explicitly passed; and b) the argument is set in the
+        # training args
+        if (
+            gen_kwargs.get("max_length") is None
+            and gen_kwargs.get("max_new_tokens") is None
+            and self.args.generation_max_length is not None
+        ):
+            gen_kwargs["max_length"] = self.args.generation_max_length
+        if gen_kwargs.get("num_beams") is None and self.args.generation_num_beams is not None:
+            gen_kwargs["num_beams"] = self.args.generation_num_beams
+        # We don't want to drop samples in general
+        self.gather_function = self.accelerator.gather
+        self._gen_kwargs = gen_kwargs
+        return super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+
+    def predict(
+        self,
+        test_dataset: Dataset,
+        ignore_keys: Optional[List[str]] = None,
+        metric_key_prefix: str = "test",
+        **gen_kwargs,
+    ) -> "PredictionOutput":
+        """
+        Run prediction and returns predictions and potential metrics.
+
+        Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
+        will also return metrics, like in `evaluate()`.
+
+        Args:
+            test_dataset (`Dataset`):
+                Dataset to run the predictions on. If it is a [`~datasets.Dataset`], columns not accepted by the
+                `model.forward()` method are automatically removed. Has to implement the method `__len__`
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+            metric_key_prefix (`str`, *optional*, defaults to `"eval"`):
+                An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
+                "eval_bleu" if the prefix is `"eval"` (default)
+            max_length (`int`, *optional*):
+                The maximum target length to use when predicting with the generate method.
+            num_beams (`int`, *optional*):
+                Number of beams for beam search that will be used when predicting with the generate method. 1 means no
+                beam search.
+            gen_kwargs:
+                Additional `generate` specific kwargs.
+
+        <Tip>
+
+        If your predictions or labels have different sequence lengths (for instance because you're doing dynamic
+        padding in a token classification task) the predictions will be padded (on the right) to allow for
+        concatenation into one array. The padding index is -100.
+
+        </Tip>
+
+        Returns: *NamedTuple* A namedtuple with the following keys:
+
+            - predictions (`np.ndarray`): The predictions on `test_dataset`.
+            - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
+            - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
+              labels).
+        """
+
+        gen_kwargs = gen_kwargs.copy()
+
+        # Use legacy argument setting if a) the option is not explicitly passed; and b) the argument is set in the
+        # training args
+        if (
+            gen_kwargs.get("max_length") is None
+            and gen_kwargs.get("max_new_tokens") is None
+            and self.args.generation_max_length is not None
+        ):
+            gen_kwargs["max_length"] = self.args.generation_max_length
+        if gen_kwargs.get("num_beams") is None and self.args.generation_num_beams is not None:
+            gen_kwargs["num_beams"] = self.args.generation_num_beams
+        self.gather_function = self.accelerator.gather
+        self._gen_kwargs = gen_kwargs
+
+        return super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
+
+    def prediction_step(
+        self,
+        model: nn.Module,
+        inputs: Dict[str, Union[torch.Tensor, Any]],
+        prediction_loss_only: bool,
+        ignore_keys: Optional[List[str]] = None,
+        **gen_kwargs,
+    ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
+        """
+        Perform an evaluation step on `model` using `inputs`.
+
+        Subclass and override to inject custom behavior.
+
+        Args:
+            model (`nn.Module`):
+                The model to evaluate.
+            inputs (`Dict[str, Union[torch.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
+                argument `labels`. Check your model's documentation for all accepted arguments.
+            prediction_loss_only (`bool`):
+                Whether or not to return the loss only.
+            gen_kwargs:
+                Additional `generate` specific kwargs.
+
+        Return:
+            Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss, logits and
+            labels (each being optional).
+        """
+
+        if not self.args.predict_with_generate or prediction_loss_only:
+            return super().prediction_step(
+                model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
+            )
+
+        has_labels = "labels" in inputs
+        inputs = self._prepare_inputs(inputs)
+
+        # Priority (handled in generate):
+        # non-`None` gen_kwargs > model.generation_config > default GenerationConfig()
+        if len(gen_kwargs) == 0 and hasattr(self, "_gen_kwargs"):
+            gen_kwargs = self._gen_kwargs.copy()
+        if "num_beams" in gen_kwargs and gen_kwargs["num_beams"] is None:
+            gen_kwargs.pop("num_beams")
+        if "max_length" in gen_kwargs and gen_kwargs["max_length"] is None:
+            gen_kwargs.pop("max_length")
+
+        default_synced_gpus = True if is_deepspeed_zero3_enabled() else False
+        gen_kwargs["synced_gpus"] = (
+            gen_kwargs["synced_gpus"] if gen_kwargs.get("synced_gpus") is not None else default_synced_gpus
+        )
+
+        generation_inputs = inputs.copy()
+        # If the `decoder_input_ids` was created from `labels`, evict the former, so that the model can freely generate
+        # (otherwise, it would continue generating from the padded `decoder_input_ids`)
+        if (
+            "labels" in generation_inputs
+            and "decoder_input_ids" in generation_inputs
+            and generation_inputs["labels"].shape == generation_inputs["decoder_input_ids"].shape
+        ):
+            generation_inputs = {
+                k: v for k, v in inputs.items() if k not in ("decoder_input_ids", "decoder_attention_mask")
+            }
+        generated_tokens = self.model.generate(**generation_inputs, **gen_kwargs)
+
+        # Temporary hack to ensure the generation config is not initialized for each iteration of the evaluation loop
+        # TODO: remove this hack when the legacy code that initializes generation_config from a model config is
+        # removed in https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/generation/utils.py#L1183
+        if self.model.generation_config._from_model_config:
+            self.model.generation_config._from_model_config = False
+
+        # Retrieves GenerationConfig from model.generation_config
+        gen_config = self.model.generation_config
+        # in case the batch is shorter than max length, the output should be padded
+        if generated_tokens.shape[-1] < gen_config.max_length:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_length)
+        elif gen_config.max_new_tokens is not None and generated_tokens.shape[-1] < gen_config.max_new_tokens + 1:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_new_tokens + 1)
+
+        with torch.no_grad():
+            if has_labels:
+                with self.compute_loss_context_manager():
+                    outputs = model(**inputs)
+                if self.label_smoother is not None:
+                    loss = self.label_smoother(outputs, inputs["labels"]).mean().detach()
+                else:
+                    loss = (outputs["loss"] if isinstance(outputs, dict) else outputs[0]).mean().detach()
+            else:
+                loss = None
+
+        if self.args.prediction_loss_only:
+            return loss, None, None
+
+        if has_labels:
+            labels = inputs["labels"]
+            if labels.shape[-1] < gen_config.max_length:
+                labels = self._pad_tensors_to_max_len(labels, gen_config.max_length)
+            elif gen_config.max_new_tokens is not None and labels.shape[-1] < gen_config.max_new_tokens + 1:
+                labels = self._pad_tensors_to_max_len(labels, gen_config.max_new_tokens + 1)
+        else:
+            labels = None
+
+        return loss, generated_tokens, labels
+
+    def _pad_tensors_to_max_len(self, tensor, max_length):
+        if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
+            # If PAD token is not defined at least EOS token has to be defined
+            pad_token_id = (
+                self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
+            )
+        else:
+            if self.model.config.pad_token_id is not None:
+                pad_token_id = self.model.config.pad_token_id
+            else:
+                raise ValueError("Pad_token_id must be set in the configuration of the model, in order to pad tensors")
+
+        padded_tensor = pad_token_id * torch.ones(
+            (tensor.shape[0], max_length), dtype=tensor.dtype, device=tensor.device
+        )
+        padded_tensor[:, : tensor.shape[-1]] = tensor
+        return padded_tensor
 
 class HiFTSeq2SeqTrainer(HiFTrainer):
     def __init__(
         self,
         hiFThandler,
         HiTaskType,
         group_element=1,
         strategy="down2up",
         hier_tuning=False,
-        lora_tuning = False,
+        peft_type=None,
         freeze_layers = [],
-        model: Union["PreTrainedModel", nn.Module] = None,
         args: "TrainingArguments" = None,
+        model: Union["PreTrainedModel", nn.Module] = None,
         data_collator: Optional["DataCollator"] = None,
         train_dataset: Optional[Dataset] = None,
         eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
         tokenizer: Optional["PreTrainedTokenizerBase"] = None,
         model_init: Optional[Callable[[], "PreTrainedModel"]] = None,
         compute_metrics: Optional[Callable[["EvalPrediction"], Dict]] = None,
         callbacks: Optional[List["TrainerCallback"]] = None,
@@ -62,15 +348,15 @@
     ):
         super().__init__(
             hiFThandler = hiFThandler,
             HiTaskType = HiTaskType,
             group_element = group_element,
             strategy = strategy,
             hier_tuning = hier_tuning,
-            lora_tuning = lora_tuning,
+            peft_type = peft_type,
             freeze_layers = freeze_layers,
             model=model,
             args=args,
             data_collator=data_collator,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset,
             tokenizer=tokenizer,
```

### Comparing `HiFT-0.0.1/hift/trainer.py` & `HiFT-0.0.2/hift/trainer.py`

 * *Files 21% similar despite different names*

```diff
@@ -58,19 +58,21 @@
 from transformers.pytorch_utils import (
     ALL_LAYERNORM_LAYERS, 
     is_torch_less_than_1_11)
 from transformers.training_args import (
     TrainingArguments,
     OptimizerNames)
 from .optimizers.optimization import Adafactor, get_scheduler
+from .optimizers import ExtendOptimizerNames as OptimizerNames
 from transformers.utils.import_utils import (
     is_bitsandbytes_available,
 )
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
 ###
+from torch.nn.parallel import DistributedDataParallel
 if is_torch_tpu_available(check_device=False):
     import torch_xla.core.xla_model as xm
     import torch_xla.debug.metrics as met
 
 if is_sagemaker_mp_enabled():
     import smdistributed.modelparallel.torch as smp
     from smdistributed.modelparallel import __version__ as SMP_VERSION
@@ -109,36 +111,514 @@
 OPTIMIZER_NAME = "optimizer.pt"
 SCHEDULER_NAME = "scheduler.pt"
 SCALER_NAME = "scaler.pt"
 
 logger = logging.get_logger(__name__)
 from .optimizers import replace_backward
 
+class PEFTrainer(Trainer):
+    def __init__(self,peft_type=None,*args,**kwargs):
+        super().__init__(*args, **kwargs)
+        self.peft_type = peft_type
+    def training_step(self, model: nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
+        return super().training_step(model, inputs)
+    def _inner_training_loop(
+        self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
+    ):
+        self.accelerator.free_memory()
+        self._train_batch_size = batch_size
+        if self.args.auto_find_batch_size:
+            self.state.train_batch_size = self._train_batch_size
+        logger.debug(f"Currently training with a batch size of: {self._train_batch_size}")
+        # Data loader and number of training steps
+        train_dataloader = self.get_train_dataloader()
+
+        # Setting up training control variables:
+        # number of training epochs: num_train_epochs
+        # number of training steps per epoch: num_update_steps_per_epoch
+        # total number of training steps to execute: max_steps
+        total_train_batch_size = self._train_batch_size * args.gradient_accumulation_steps * args.world_size
+
+        len_dataloader = None
+        num_train_tokens = None
+        if has_length(train_dataloader):
+            len_dataloader = len(train_dataloader)
+            num_update_steps_per_epoch = len_dataloader // args.gradient_accumulation_steps
+            num_update_steps_per_epoch = max(num_update_steps_per_epoch, 1)
+            num_examples = self.num_examples(train_dataloader)
+            if args.max_steps > 0:
+                max_steps = args.max_steps
+                num_train_epochs = args.max_steps // num_update_steps_per_epoch + int(
+                    args.max_steps % num_update_steps_per_epoch > 0
+                )
+                # May be slightly incorrect if the last batch in the training dataloader has a smaller size but it's
+                # the best we can do.
+                num_train_samples = args.max_steps * total_train_batch_size
+                if args.include_tokens_per_second:
+                    num_train_tokens = (
+                        self.num_tokens(train_dataloader, args.max_steps) * args.gradient_accumulation_steps
+                    )
+            else:
+                max_steps = math.ceil(args.num_train_epochs * num_update_steps_per_epoch)
+                num_train_epochs = math.ceil(args.num_train_epochs)
+                num_train_samples = self.num_examples(train_dataloader) * args.num_train_epochs
+                if args.include_tokens_per_second:
+                    num_train_tokens = self.num_tokens(train_dataloader) * args.num_train_epochs
+        elif args.max_steps > 0:  # Rely on max_steps when dataloader does not have a working size
+            max_steps = args.max_steps
+            # Setting a very large number of epochs so we go as many times as necessary over the iterator.
+            num_train_epochs = sys.maxsize
+            num_update_steps_per_epoch = max_steps
+            num_examples = total_train_batch_size * args.max_steps
+            num_train_samples = args.max_steps * total_train_batch_size
+            if args.include_tokens_per_second:
+                num_train_tokens = self.num_tokens(train_dataloader, args.max_steps) * args.gradient_accumulation_steps
+        else:
+            raise ValueError(
+                "args.max_steps must be set to a positive value if dataloader does not have a length, was"
+                f" {args.max_steps}"
+            )
+
+        if DebugOption.UNDERFLOW_OVERFLOW in self.args.debug:
+            if self.args.n_gpu > 1:
+                # nn.DataParallel(model) replicates the model, creating new variables and module
+                # references registered here no longer work on other gpus, breaking the module
+                raise ValueError(
+                    "Currently --debug underflow_overflow is not supported under DP. Please use DDP"
+                    " (torchrun or torch.distributed.launch (deprecated))."
+                )
+            else:
+                debug_overflow = DebugUnderflowOverflow(self.model)  # noqa
+
+        delay_optimizer_creation = is_sagemaker_mp_enabled() or self.is_fsdp_xla_enabled or self.is_fsdp_enabled
+
+        # We need to reset the scheduler, as its parameters may be different on subsequent calls
+        if self._created_lr_scheduler:
+            self.lr_scheduler = None
+            self._created_lr_scheduler = False
+
+        if self.is_deepspeed_enabled:
+            self.optimizer, self.lr_scheduler = deepspeed_init(self, num_training_steps=max_steps)
+
+        if not delay_optimizer_creation:
+            self.create_optimizer_and_scheduler(num_training_steps=max_steps)
+
+        self.state = TrainerState()
+        self.state.is_hyper_param_search = trial is not None
+        self.state.train_batch_size = self._train_batch_size
+
+        # Compute absolute values for logging, eval, and save if given as ratio
+        if args.logging_steps is not None:
+            if args.logging_steps < 1:
+                self.state.logging_steps = math.ceil(max_steps * args.logging_steps)
+            else:
+                self.state.logging_steps = args.logging_steps
+        if args.eval_steps is not None:
+            if args.eval_steps < 1:
+                self.state.eval_steps = math.ceil(max_steps * args.eval_steps)
+            else:
+                self.state.eval_steps = args.eval_steps
+        if args.save_steps is not None:
+            if args.save_steps < 1:
+                self.state.save_steps = math.ceil(max_steps * args.save_steps)
+            else:
+                self.state.save_steps = args.save_steps
+
+        # Activate gradient checkpointing if needed
+        if args.gradient_checkpointing:
+            if args.gradient_checkpointing_kwargs is None:
+                gradient_checkpointing_kwargs = {}
+            else:
+                gradient_checkpointing_kwargs = args.gradient_checkpointing_kwargs
+
+            self.model.gradient_checkpointing_enable(gradient_checkpointing_kwargs=gradient_checkpointing_kwargs)
+
+        model = self._wrap_model(self.model_wrapped)
+
+        # as the model is wrapped, don't use `accelerator.prepare`
+        # this is for unhandled cases such as
+        # FSDP-XLA, SageMaker MP/DP, DataParallel, IPEX
+        use_accelerator_prepare = True if model is self.model else False
+
+        if delay_optimizer_creation:
+            self.create_optimizer_and_scheduler(num_training_steps=max_steps)
+
+        # prepare using `accelerator` prepare
+        if use_accelerator_prepare:
+            self.model.train()
+            if hasattr(self.lr_scheduler, "step"):
+                if self.use_apex:
+                    model = self.accelerator.prepare(self.model)
+                else:
+                    model, self.optimizer = self.accelerator.prepare(self.model, self.optimizer)
+            else:
+                # to handle cases wherein we pass "DummyScheduler" such as when it is specified in DeepSpeed config.
+                model, self.optimizer, self.lr_scheduler = self.accelerator.prepare(
+                    self.model, self.optimizer, self.lr_scheduler
+                )
+
+        if self.is_fsdp_enabled:
+            self.model = self.model_wrapped = model
+
+        # for the rest of this function `model` is the outside model, whether it was wrapped or not
+        if model is not self.model:
+            self.model_wrapped = model
+
+        # backward compatibility
+        if self.is_deepspeed_enabled:
+            self.deepspeed = self.model_wrapped
+
+        # ckpt loading
+        if resume_from_checkpoint is not None:
+            if self.is_deepspeed_enabled:
+                deepspeed_load_checkpoint(self.model_wrapped, resume_from_checkpoint)
+            elif is_sagemaker_mp_enabled() or self.is_fsdp_enabled:
+                self._load_from_checkpoint(resume_from_checkpoint, self.model_wrapped)
+
+        # Check if saved optimizer or scheduler states exist
+        self._load_optimizer_and_scheduler(resume_from_checkpoint)
+
+        # important: at this point:
+        # self.model         is the Transformers Model
+        # self.model_wrapped is DDP(Transformers Model), Deepspeed(Transformers Model),
+        # FSDP(Transformers Model), Dynamo Optimized Module(Transformers Model) etc.
+
+        # Train!
+        logger.info("***** Running training *****")
+        logger.info(f"  Num examples = {num_examples:,}")
+        logger.info(f"  Num Epochs = {num_train_epochs:,}")
+        logger.info(f"  Instantaneous batch size per device = {self.args.per_device_train_batch_size:,}")
+        if self.args.per_device_train_batch_size != self._train_batch_size:
+            logger.info(f"  Training with DataParallel so batch size has been adjusted to: {self._train_batch_size:,}")
+        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size:,}")
+        logger.info(f"  Gradient Accumulation steps = {args.gradient_accumulation_steps}")
+        logger.info(f"  Total optimization steps = {max_steps:,}")
+        logger.info(f"  Number of trainable parameters = {get_model_param_count(model, trainable_only=True):,}")
+
+        self.state.epoch = 0
+        start_time = time.time()
+        epochs_trained = 0
+        steps_trained_in_current_epoch = 0
+        steps_trained_progress_bar = None
+
+        # Check if continuing training from a checkpoint
+        if resume_from_checkpoint is not None and os.path.isfile(
+            os.path.join(resume_from_checkpoint, TRAINER_STATE_NAME)
+        ):
+            self.state = TrainerState.load_from_json(os.path.join(resume_from_checkpoint, TRAINER_STATE_NAME))
+            epochs_trained = self.state.global_step // num_update_steps_per_epoch
+            if not args.ignore_data_skip:
+                steps_trained_in_current_epoch = self.state.global_step % (num_update_steps_per_epoch)
+                steps_trained_in_current_epoch *= args.gradient_accumulation_steps
+            else:
+                steps_trained_in_current_epoch = 0
+
+            logger.info("  Continuing training from checkpoint, will skip to saved global_step")
+            logger.info(f"  Continuing training from epoch {epochs_trained}")
+            logger.info(f"  Continuing training from global step {self.state.global_step}")
+            if not args.ignore_data_skip:
+                logger.info(
+                    f"  Will skip the first {epochs_trained} epochs then the first"
+                    f" {steps_trained_in_current_epoch} batches in the first epoch."
+                )
+
+        # Update the references
+        self.callback_handler.model = self.model
+        self.callback_handler.optimizer = self.optimizer
+        self.callback_handler.lr_scheduler = self.lr_scheduler
+        self.callback_handler.train_dataloader = train_dataloader
+        if self.hp_name is not None and self._trial is not None:
+            # use self._trial because the SigOpt/Optuna hpo only call `_hp_search_setup(trial)` instead of passing trial
+            # parameter to Train when using DDP.
+            self.state.trial_name = self.hp_name(self._trial)
+        if trial is not None:
+            assignments = trial.assignments if self.hp_search_backend == HPSearchBackend.SIGOPT else trial
+            self.state.trial_params = hp_params(assignments)
+        else:
+            self.state.trial_params = None
+        # This should be the same if the state has been saved but in case the training arguments changed, it's safer
+        # to set this after the load.
+        self.state.max_steps = max_steps
+        self.state.num_train_epochs = num_train_epochs
+        self.state.is_local_process_zero = self.is_local_process_zero()
+        self.state.is_world_process_zero = self.is_world_process_zero()
+
+        # tr_loss is a tensor to avoid synchronization of TPUs through .item()
+        tr_loss = torch.tensor(0.0).to(args.device)
+        # _total_loss_scalar is updated everytime .item() has to be called on tr_loss and stores the sum of all losses
+        self._total_loss_scalar = 0.0
+        self._globalstep_last_logged = self.state.global_step
+        model.zero_grad()
+
+        self.control = self.callback_handler.on_train_begin(args, self.state, self.control)
+
+        # Skip the first epochs_trained epochs to get the random state of the dataloader at the right point.
+        if not args.ignore_data_skip:
+            for epoch in range(epochs_trained):
+                sampler = get_dataloader_sampler(train_dataloader)
+                sampler_kinds = [RandomSampler]
+                if version.parse(accelerate_version) > version.parse("0.23.0"):
+                    sampler_kinds.append(SeedableRandomSampler)
+                is_random_sampler = isinstance(sampler, tuple(sampler_kinds))
+                if is_torch_less_than_1_11 or not is_random_sampler:
+                    # We just need to begin an iteration to create the randomization of the sampler.
+                    for _ in train_dataloader:
+                        break
+                else:
+                    # Otherwise we need to call the whooooole sampler cause there is some random operation added
+                    # AT THE VERY END!
+                    sampler = sampler if sampler is not None else []
+                    _ = list(sampler)
+
+        total_batched_samples = 0
+        for epoch in range(epochs_trained, num_train_epochs):
+            epoch_iterator = train_dataloader
+            if hasattr(epoch_iterator, "set_epoch"):
+                epoch_iterator.set_epoch(epoch)
+
+            # Reset the past mems state at the beginning of each epoch if necessary.
+            if args.past_index >= 0:
+                self._past = None
+
+            steps_in_epoch = (
+                len(epoch_iterator)
+                if len_dataloader is not None
+                else args.max_steps * args.gradient_accumulation_steps
+            )
+            self.control = self.callback_handler.on_epoch_begin(args, self.state, self.control)
+
+            if epoch == epochs_trained and resume_from_checkpoint is not None and steps_trained_in_current_epoch == 0:
+                self._load_rng_state(resume_from_checkpoint)
+
+            rng_to_sync = False
+            steps_skipped = 0
+            if steps_trained_in_current_epoch > 0:
+                epoch_iterator = skip_first_batches(epoch_iterator, steps_trained_in_current_epoch)
+                steps_skipped = steps_trained_in_current_epoch
+                steps_trained_in_current_epoch = 0
+                rng_to_sync = True
+
+            step = -1
+            for step, inputs in enumerate(epoch_iterator):
+                total_batched_samples += 1
+
+                if self.args.include_num_input_tokens_seen:
+                    main_input_name = getattr(self.model, "main_input_name", "input_ids")
+                    if main_input_name not in inputs:
+                        logger.warning(
+                            "Tried to track the number of tokens seen, however the current model is "
+                            "not configured properly to know what item is the input. To fix this, add "
+                            "a `main_input_name` attribute to the model class you are using."
+                        )
+                    else:
+                        self.state.num_input_tokens_seen += self.accelerator.gather(inputs[main_input_name]).numel()
+                if rng_to_sync:
+                    self._load_rng_state(resume_from_checkpoint)
+                    rng_to_sync = False
+
+                # Skip past any already trained steps if resuming training
+                if steps_trained_in_current_epoch > 0:
+                    steps_trained_in_current_epoch -= 1
+                    if steps_trained_progress_bar is not None:
+                        steps_trained_progress_bar.update(1)
+                    if steps_trained_in_current_epoch == 0:
+                        self._load_rng_state(resume_from_checkpoint)
+                    continue
+                elif steps_trained_progress_bar is not None:
+                    steps_trained_progress_bar.close()
+                    steps_trained_progress_bar = None
+
+                if step % args.gradient_accumulation_steps == 0:
+                    self.control = self.callback_handler.on_step_begin(args, self.state, self.control)
+
+                with self.accelerator.accumulate(model):
+                    tr_loss_step = self.training_step(model, inputs)
+
+                if (
+                    args.logging_nan_inf_filter
+                    and not is_torch_tpu_available()
+                    and (torch.isnan(tr_loss_step) or torch.isinf(tr_loss_step))
+                ):
+                    # if loss is nan or inf simply add the average of previous logged losses
+                    tr_loss += tr_loss / (1 + self.state.global_step - self._globalstep_last_logged)
+                else:
+                    tr_loss += tr_loss_step
+
+                self.current_flos += float(self.floating_point_ops(inputs))
+
+                is_last_step_and_steps_less_than_grad_acc = (
+                    steps_in_epoch <= args.gradient_accumulation_steps and (step + 1) == steps_in_epoch
+                )
+
+                if (
+                    total_batched_samples % args.gradient_accumulation_steps == 0
+                    or
+                    # last step in epoch but step is always smaller than gradient_accumulation_steps
+                    is_last_step_and_steps_less_than_grad_acc
+                ):
+                    # the `or` condition of `is_last_step_and_steps_less_than_grad_acc` is not covered
+                    # in accelerate. So, explicitly enable sync gradients to True in that case.
+                    if is_last_step_and_steps_less_than_grad_acc:
+                        self.accelerator.gradient_state._set_sync_gradients(True)
+
+                    # Gradient clipping
+                    if args.max_grad_norm is not None and args.max_grad_norm > 0:
+                        # deepspeed does its own clipping
+
+                        if is_sagemaker_mp_enabled() and args.fp16:
+                            self.optimizer.clip_master_grads(args.max_grad_norm)
+                        elif self.use_apex:
+                            # Revert to normal clipping otherwise, handling Apex or full precision
+                            nn.utils.clip_grad_norm_(
+                                amp.master_params(self.optimizer),
+                                args.max_grad_norm,
+                            )
+                        else:
+                            self.accelerator.clip_grad_norm_(
+                                model.parameters(),
+                                args.max_grad_norm,
+                            )
+
+                    # Optimizer step
+                    self.optimizer.step()
+                    optimizer_was_run = not self.accelerator.optimizer_step_was_skipped
+                    if optimizer_was_run:
+                        # Delay optimizer scheduling until metrics are generated
+                        if not isinstance(self.lr_scheduler, torch.optim.lr_scheduler.ReduceLROnPlateau):
+                            
+                            self.lr_scheduler.step()
+
+                    if self.peft_type == "adalora":
+                        if isinstance(model,DistributedDataParallel):
+                            if not model.module.peft_config["default"].total_step:
+                                model.module.peft_config["default"].total_step = max_steps
+                            model.module.base_model.update_and_allocate(self.state.global_step)
+                        else:
+                            if not model.peft_config["default"].total_step:
+                                model.peft_config["default"].total_step = max_steps
+                            model.base_model.update_and_allocate(self.state.global_step)
+                    model.zero_grad()
+                    self.state.global_step += 1
+                    self.state.epoch = epoch + (step + 1 + steps_skipped) / steps_in_epoch
+                    self.control = self.callback_handler.on_step_end(args, self.state, self.control)
+
+                    self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
+                else:
+                    self.control = self.callback_handler.on_substep_end(args, self.state, self.control)
+
+                if self.control.should_epoch_stop or self.control.should_training_stop:
+                    break
+            if step < 0:
+                logger.warning(
+                    "There seems to be not a single sample in your epoch_iterator, stopping training at step"
+                    f" {self.state.global_step}! This is expected if you're using an IterableDataset and set"
+                    f" num_steps ({max_steps}) higher than the number of available samples."
+                )
+                self.control.should_training_stop = True
+
+            self.control = self.callback_handler.on_epoch_end(args, self.state, self.control)
+            self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
+
+            if DebugOption.TPU_METRICS_DEBUG in self.args.debug:
+                if is_torch_tpu_available():
+                    # tpu-comment: Logging debug metrics for PyTorch/XLA (compile, execute times, ops, etc.)
+                    xm.master_print(met.metrics_report())
+                else:
+                    logger.warning(
+                        "You enabled PyTorch/XLA debug metrics but you don't have a TPU "
+                        "configured. Check your training configuration if this is unexpected."
+                    )
+            if self.control.should_training_stop:
+                break
+
+        if args.past_index and hasattr(self, "_past"):
+            # Clean the state at the end of training
+            delattr(self, "_past")
+
+        logger.info("\n\nTraining completed. Do not forget to share your model on huggingface.co/models =)\n\n")
+        if args.load_best_model_at_end and self.state.best_model_checkpoint is not None:
+            # Wait for everyone to get here so we are sure the model has been saved by process 0.
+            if is_torch_tpu_available():
+                xm.rendezvous("load_best_model_at_end")
+            elif args.parallel_mode == ParallelMode.DISTRIBUTED:
+                dist.barrier()
+            elif is_sagemaker_mp_enabled():
+                smp.barrier()
+
+            self._load_best_model()
+
+        # add remaining tr_loss
+        self._total_loss_scalar += tr_loss.item()
+        train_loss = self._total_loss_scalar / self.state.global_step
+
+        metrics = speed_metrics(
+            "train",
+            start_time,
+            num_samples=num_train_samples,
+            num_steps=self.state.max_steps,
+            num_tokens=num_train_tokens,
+        )
+        self.store_flos()
+        metrics["total_flos"] = self.state.total_flos
+        metrics["train_loss"] = train_loss
+
+        self.is_in_train = False
+
+        self._memory_tracker.stop_and_update_metrics(metrics)
+
+        self.log(metrics)
+
+        run_dir = self._get_output_dir(trial)
+        checkpoints_sorted = self._sorted_checkpoints(use_mtime=False, output_dir=run_dir)
+
+        # Delete the last checkpoint when save_total_limit=1 if it's different from the best checkpoint and process allowed to save.
+        if self.args.should_save and self.state.best_model_checkpoint is not None and self.args.save_total_limit == 1:
+            for checkpoint in checkpoints_sorted:
+                if not os.path.samefile(checkpoint, self.state.best_model_checkpoint):
+                    logger.info(f"Deleting older checkpoint [{checkpoint}] due to args.save_total_limit")
+                    shutil.rmtree(checkpoint)
+
+        self.control = self.callback_handler.on_train_end(args, self.state, self.control)
+
+        # Wait for the checkpoint to be uploaded.
+        self._finish_current_push()
+
+        # After training we make sure to retrieve back the original forward pass method
+        # for the embedding layer by removing the forward post hook.
+        if self.neftune_noise_alpha is not None:
+            self._deactivate_neftune(self.model)
+
+        return TrainOutput(self.state.global_step, train_loss, metrics)
+    
+
 class HiFTrainer(Trainer):
     def __init__(self,
                 hiFThandler,
                 HiTaskType,
                 group_element=1,
                 strategy="down2up",
                 hier_tuning=False,
-                lora_tuning = False,
+                peft_type = None,
                 freeze_layers = [],
                 *args,
                 **kwargs):
         if hier_tuning:
             replace_backward()
         super().__init__(*args, **kwargs)
-        self.hift_callback = hiFThandler(freeze_layers,strategy,lora_tuning)
+        self.hift_callback = hiFThandler(freeze_layers,strategy,HiTaskType,peft_type)
         self.optimizer_states = None
         self.counter = 0
         self.group_element=group_element
         self.hier_tuning = hier_tuning
-        self.lora_tuning = lora_tuning
-        self.spLayers = hiFThandler.GetSpecialLayer(taskType=HiTaskType)
-        self.group_parameters = self.hift_callback.group_model(self.model,self.spLayers,num_position=self.hift_callback.number_position,lora_tuning = lora_tuning)
+        self.peft_type = peft_type
+        self.init_state = {name:p.requires_grad for name,p in self.model.named_parameters()}
+        for name,_ in self.model.named_parameters():
+            print(name)
+        
+        self.group_parameters = self.hift_callback.group_model(self.model)
     def create_optimizer(self):
         """
         Setup the optimizer.
 
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
         Trainer's init through `optimizers`, or subclass and override this method in a subclass.
         """
@@ -175,15 +655,15 @@
                         logger.info(f"skipped {module}: {skipped/2**20}M params")
                         manager.register_module_override(module, "weight", {"optim_bits": 32})
                         logger.debug(f"bitsandbytes: will optimize {module} in fp32")
                 logger.info(f"skipped: {skipped/2**20}M params")
         if is_sagemaker_mp_enabled():
             self.optimizer = smp.DistributedOptimizer(self.optimizer)
         return self.optimizer
-
+        
     def select_element(self):
         elements = self.group_parameters[:self.group_element]
         for element in elements:
             self.group_parameters.remove(element)
         for element in elements:
             self.group_parameters.append(element)
         return elements
@@ -191,22 +671,21 @@
     def update_parameter_state(self):
         if self.optimizer_states is None:
             self.optimizer_states=self.get_optimizer_state()
         opt_model = self.model_wrapped if is_sagemaker_mp_enabled() else self.model
         if self.counter == int(len(self.group_parameters) // self.group_element):
             self.counter = 0
             self.optimizer_states=self.get_optimizer_state()
-        pattern = self.hift_callback.pattern_name(self.spLayers)
+        pattern = "|".join(self.hift_callback.pattern_list)
         elements = self.select_element()
         self.counter +=1
         for name,parameter in opt_model.named_parameters():
             parameter.requires_grad = False
-            if self.lora_tuning:
-                if "lora_" in name:
-                    name = ".".join(name.split(".")[2:])
+            if self.peft_type:
+                if self.init_state[name]:
                     layers_selecton = re.compile(pattern).findall(name)
                     if self.hift_callback.check_selection(elements,layers_selecton):
                         parameter.requires_grad = True
             else:
                 layers_selecton = re.compile(pattern).findall(name)
                 if self.hift_callback.check_selection(elements,layers_selecton):
                     parameter.requires_grad = True
@@ -235,15 +714,14 @@
     def get_optimizer_state(self):
         states_groups={}
         optimizer_grouped_parameters = self.optimizer.param_groups
         for i, param_group in enumerate(optimizer_grouped_parameters):
             param_group.pop("params")
             states_groups[i] = param_group
         return states_groups
-
     def training_step(self, model: nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
         self.update_parameter_state()
         return super().training_step(model, inputs)
     def _inner_training_loop(
         self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
     ):
         self.accelerator.free_memory()
@@ -606,15 +1084,23 @@
                     if optimizer_was_run:
                         # Delay optimizer scheduling until metrics are generated
                         if not isinstance(self.lr_scheduler, torch.optim.lr_scheduler.ReduceLROnPlateau):
                             if not self.hier_tuning:
                                 self.lr_scheduler.step()
                             elif self.hier_tuning and self.counter == int(len(self.group_parameters) // self.group_element):
                                 self.lr_scheduler.step()
-
+                    if self.peft_type == "adalora":
+                        if isinstance(model,DistributedDataParallel):
+                            if not model.module.peft_config["default"].total_step:
+                                model.module.peft_config["default"].total_step = max_steps
+                            model.module.base_model.update_and_allocate(self.state.global_step)
+                        else:
+                            if not model.peft_config["default"].total_step:
+                                model.peft_config["default"].total_step = max_steps
+                            model.base_model.update_and_allocate(self.state.global_step)
                     model.zero_grad()
                     self.state.global_step += 1
                     self.state.epoch = epoch + (step + 1 + steps_skipped) / steps_in_epoch
                     self.control = self.callback_handler.on_step_end(args, self.state, self.control)
 
                     self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
                 else:
@@ -710,14 +1196,16 @@
 
         Args:
             args (`transformers.training_args.TrainingArguments`):
                 The training arguments for the training session.
 
         """
 
+        for optimizer in OptimizerNames:
+            print(optimizer.name, optimizer.value)
         # parse args.optim_args
         optim_args = {}
         if args.optim_args:
             for mapping in args.optim_args.replace(" ", "").split(","):
                 key, value = mapping.split("=")
                 optim_args[key] = value
 
@@ -771,31 +1259,54 @@
             OptimizerNames.ADAMW_8BIT,
             OptimizerNames.PAGED_ADAMW,
             OptimizerNames.PAGED_ADAMW_8BIT,
             OptimizerNames.LION,
             OptimizerNames.LION_8BIT,
             OptimizerNames.PAGED_LION,
             OptimizerNames.PAGED_LION_8BIT,
+            OptimizerNames.LAMB,
+            OptimizerNames.LAMB_8BIT,
+            OptimizerNames.LARS,
+            OptimizerNames.LARS_8BIT,
+            OptimizerNames.BRMSPROP,
+            OptimizerNames.BRMSPROP_8BIT,
+            OptimizerNames.BSGD,
+            OptimizerNames.BSGD_8BIT,
+            OptimizerNames.BADAGRAD,
+            OptimizerNames.BADAGRAD_8BIT
         ]:
             try:
-                from bitsandbytes.optim import AdamW, Lion
+                from .optimizers import BitAdamW, BitLion,BitAdagrad,BitAdam,BitLAMB,BitLARS,BitRMSprop,BitSGD
 
                 is_paged = False
                 optim_bits = 32
                 optimizer_cls = None
                 additional_optim_kwargs = adam_kwargs
                 if "paged" in args.optim:
                     is_paged = True
                 if "8bit" in args.optim:
                     optim_bits = 8
+                if "adamw" in args.optim:
+                    optimizer_cls = BitAdamW
                 if "adam" in args.optim:
-                    optimizer_cls = AdamW
+                    optimizer_cls = BitAdam
                 elif "lion" in args.optim:
-                    optimizer_cls = Lion
+                    optimizer_cls = BitLion
+                    additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+                elif "lamb" in args.optim:
+                    optimizer_cls = BitLAMB
                     additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
+                elif "lars" in args.optim:
+                    optimizer_cls = BitLARS
+                elif "rmsprop" in args.optim:
+                    optimizer_cls = BitRMSprop
+                elif "sgd" in args.optim:
+                    optimizer_cls = BitSGD
+                elif "adagrad" in args.optim:
+                    optimizer_cls = BitAdagrad
                 bnb_kwargs = {"is_paged": is_paged, "optim_bits": optim_bits}
                 optimizer_kwargs.update(additional_optim_kwargs)
                 optimizer_kwargs.update(bnb_kwargs)
             except ImportError:
                 raise ValueError("Trainer tried to instantiate bnb optimizer but bnb is not installed!")
             if is_bitsandbytes_available() and version.parse(
                 importlib.metadata.version("bitsandbytes")
@@ -832,8 +1343,9 @@
             from .optimizers.adagrad import Adagrad
             optimizer_cls = Adagrad
         elif args.optim == OptimizerNames.RMSPROP:
             from .optimizers.rmsprop import RMSprop
             optimizer_cls = RMSprop
         else:
             raise ValueError(f"Trainer cannot instantiate unsupported optimizer: {args.optim}")
+        logger.info(f"the optimizer you are using is {optimizer_cls}")
         return optimizer_cls, optimizer_kwargs
```

### Comparing `HiFT-0.0.1/setup.py` & `HiFT-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HiFT",
-    version="0.0.1",
+    version="0.0.2",
     author="Yongkang Liu",
     author_email="misonsky@163.com",
     description="PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/misonsky/HiFT",
     packages=setuptools.find_packages(),
```

