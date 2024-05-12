# Comparing `tmp/dartrs-0.1.4.tar.gz` & `tmp/dartrs-0.1.5.tar.gz`

## Comparing `dartrs-0.1.4.tar` & `dartrs-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.4/Cargo.toml
--rw-r--r--   0     1001      127     4367 2024-05-11 08:10:12.000000 dartrs-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      470 2024-05-11 08:10:12.000000 dartrs-0.1.4/.gitignore
--rw-r--r--   0     1001      127    11357 2024-05-11 08:10:12.000000 dartrs-0.1.4/LICENSE
--rw-r--r--   0     1001      127     1320 2024-05-11 08:10:12.000000 dartrs-0.1.4/README.md
--rw-r--r--   0     1001      127     1920 2024-05-11 08:10:12.000000 dartrs-0.1.4/examples/main.py
--rw-r--r--   0     1001      127      914 2024-05-11 08:10:12.000000 dartrs-0.1.4/examples/simple.py
--rw-r--r--   0     1001      127     4742 2024-05-11 08:10:12.000000 dartrs-0.1.4/pdm.lock
--rw-r--r--   0     1001      127      108 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/__init__.py
--rw-r--r--   0     1001      127     4235 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/dartrs.pyi
--rw-r--r--   0     1001      127        0 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/py.typed
--rw-r--r--   0     1001      127      749 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/utils.py
--rw-r--r--   0     1001      127     3483 2024-05-11 08:10:12.000000 dartrs-0.1.4/python/dartrs/v2.py
--rw-r--r--   0     1001      127     3237 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/generation.rs
--rw-r--r--   0     1001      127     9698 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/models.rs
--rw-r--r--   0     1001      127      923 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/prompt.rs
--rw-r--r--   0     1001      127     6619 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings/tags.rs
--rw-r--r--   0     1001      127       94 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/bindings.rs
--rw-r--r--   0     1001      127     1587 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/configs.rs
--rw-r--r--   0     1001      127     8802 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/generation.rs
--rw-r--r--   0     1001      127      858 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/lib.rs
--rw-r--r--   0     1001      127     1130 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/logits_processor.rs
--rw-r--r--   0     1001      127    12295 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models/mistral.rs
--rw-r--r--   0     1001      127    17025 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models/mixtral.rs
--rw-r--r--   0     1001      127     3446 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/models.rs
--rw-r--r--   0     1001      127     2225 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/prompt.rs
--rw-r--r--   0     1001      127     5657 2024-05-11 08:10:12.000000 dartrs-0.1.4/src/tags.rs
--rw-r--r--   0     1001      127        0 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/__init__.py
--rw-r--r--   0     1001      127     1330 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_configs.py
--rw-r--r--   0     1001      127     5903 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_model.py
--rw-r--r--   0     1001      127     1298 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_prompt.py
--rw-r--r--   0     1001      127     2276 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_tokenizer.py
--rw-r--r--   0     1001      127      588 2024-05-11 08:10:12.000000 dartrs-0.1.4/tests/test_v2.py
--rw-r--r--   0     1001      127    51754 2024-05-11 08:10:23.000000 dartrs-0.1.4/Cargo.lock
--rw-r--r--   0     1001      127      662 2024-05-11 08:10:12.000000 dartrs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 dartrs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      127     4367 2024-05-12 14:10:26.000000 dartrs-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      470 2024-05-12 14:10:26.000000 dartrs-0.1.5/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-05-12 14:10:26.000000 dartrs-0.1.5/LICENSE
+-rw-r--r--   0     1001      127     1378 2024-05-12 14:10:26.000000 dartrs-0.1.5/README.md
+-rw-r--r--   0     1001      127     1945 2024-05-12 14:10:26.000000 dartrs-0.1.5/examples/main.py
+-rw-r--r--   0     1001      127      928 2024-05-12 14:10:26.000000 dartrs-0.1.5/examples/simple.py
+-rw-r--r--   0     1001      127     4742 2024-05-12 14:10:26.000000 dartrs-0.1.5/pdm.lock
+-rw-r--r--   0     1001      127      108 2024-05-12 14:10:26.000000 dartrs-0.1.5/python/dartrs/__init__.py
+-rw-r--r--   0     1001      127     4332 2024-05-12 14:10:26.000000 dartrs-0.1.5/python/dartrs/dartrs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-12 14:10:26.000000 dartrs-0.1.5/python/dartrs/py.typed
+-rw-r--r--   0     1001      127      842 2024-05-12 14:10:26.000000 dartrs-0.1.5/python/dartrs/utils.py
+-rw-r--r--   0     1001      127     3498 2024-05-12 14:10:26.000000 dartrs-0.1.5/python/dartrs/v2.py
+-rw-r--r--   0     1001      127     3237 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/bindings/generation.rs
+-rw-r--r--   0     1001      127    10297 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/bindings/models.rs
+-rw-r--r--   0     1001      127      923 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/bindings/prompt.rs
+-rw-r--r--   0     1001      127     6619 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/bindings/tags.rs
+-rw-r--r--   0     1001      127       94 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/bindings.rs
+-rw-r--r--   0     1001      127     1587 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/configs.rs
+-rw-r--r--   0     1001      127     8856 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/generation.rs
+-rw-r--r--   0     1001      127      858 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      127     1130 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/logits_processor.rs
+-rw-r--r--   0     1001      127    12422 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/models/mistral.rs
+-rw-r--r--   0     1001      127    17192 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     3446 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/models.rs
+-rw-r--r--   0     1001      127     2225 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/prompt.rs
+-rw-r--r--   0     1001      127     5657 2024-05-12 14:10:26.000000 dartrs-0.1.5/src/tags.rs
+-rw-r--r--   0     1001      127        0 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/__init__.py
+-rw-r--r--   0     1001      127     1330 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/test_configs.py
+-rw-r--r--   0     1001      127     6670 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/test_model.py
+-rw-r--r--   0     1001      127     1298 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/test_prompt.py
+-rw-r--r--   0     1001      127     2276 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/test_tokenizer.py
+-rw-r--r--   0     1001      127      588 2024-05-12 14:10:26.000000 dartrs-0.1.5/tests/test_v2.py
+-rw-r--r--   0     1001      127    51754 2024-05-12 14:10:34.000000 dartrs-0.1.5/Cargo.lock
+-rw-r--r--   0     1001      127      662 2024-05-12 14:10:26.000000 dartrs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 dartrs-0.1.5/PKG-INFO
```

### Comparing `dartrs-0.1.4/Cargo.toml` & `dartrs-0.1.5/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dartrs"
-version = "0.1.4"
+version = "0.1.5"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "dartrs"
 crate-type = ["cdylib", "lib"]
```

### Comparing `dartrs-0.1.4/.github/workflows/CI.yml` & `dartrs-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/LICENSE` & `dartrs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/README.md` & `dartrs-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     V2Model,
 )
 import time
 import os
 
 MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
-model = MixtralModel.from_pretrained(MODEL_NAME)
+model = MixtralModel.from_pretrained(MODEL_NAME, dtype="fp16")
 tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
 config = get_generation_config(
     prompt=compose_prompt(
         copyright="vocaloid",
         character="hatsune miku",
         rating="general", # sfw, general, sensitive, nsfw, questionable, explicit
@@ -42,10 +42,10 @@
 start = time.time()
 output = model.generate(config)
 end = time.time()
 
 print(output)
 print(f"Time taken: {end - start:.2f}s")
 # Output:
-# cowboy shot, detached sleeves, empty eyes, green eyes, green hair, green necktie, hair in own mouth, hair ornament, letterboxed, light frown, long hair, long sleeves, looking to the side, necktie, parted lips, shirt, sleeveless, sleeveless shirt, twintails, wing collar
-# Time taken: 0.26s
+# cowboy shot, detached sleeves, expressionless, from side, hair ornament, halftone, hairclip, holding, limited palette, long hair, looking at viewer, miniskirt, necktie, pleated skirt, shirt, simple background, skirt, sleeveless, sleeveless shirt, straight-on, thighhighs, twintails, very long hair, zettai ryouiki
+# Time taken: 0.22s
 ```
```

### Comparing `dartrs-0.1.4/examples/main.py` & `dartrs-0.1.5/examples/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dartrs.dartrs import DartTokenizer, GenerationConfig
+from dartrs.dartrs import DartTokenizer, GenerationConfig, DartDType
 from dartrs.utils import get_generation_config
 from dartrs.v2 import (
     compose_prompt,
     MixtralModel,
     V2Model,
 )
 import time
 import os
 
 MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
 
 def prepare_models():
-    model = MixtralModel.from_pretrained(MODEL_NAME)
+    model = MixtralModel.from_pretrained(MODEL_NAME, dtype="fp16")
     tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
     return model, tokenizer
 
 
 def generate(model: V2Model, config: GenerationConfig):
     start = time.time()
```

### Comparing `dartrs-0.1.4/examples/simple.py` & `dartrs-0.1.5/examples/simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     compose_prompt,
     MixtralModel,
 )
 import time
 
 MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
-model = MixtralModel.from_pretrained(MODEL_NAME)
+model = MixtralModel.from_pretrained(MODEL_NAME, dtype="fp16")
 tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
 config = get_generation_config(
     prompt=compose_prompt(
         copyright="vocaloid",
         character="hatsune miku",
         rating="general",  # sfw, general, sensitive, nsfw, questionable, explicit
```

### Comparing `dartrs-0.1.4/pdm.lock` & `dartrs-0.1.5/pdm.lock`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/python/dartrs/dartrs.pyi` & `dartrs-0.1.5/python/dartrs/dartrs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from abc import ABC
 
 class DartDType:
     BF16: ...
     FP16: ...
     FP32: ...
+    def __init__(self, dtype: str) -> None: ...
 
 class DartDevice:
+    def __init__(self, device: str) -> None: ...
     @classmethod
     def Cpu(cls) -> ...: ...
     @classmethod
     def Cuda(cls, id: int) -> ...: ...
 
 class GenerationConfig:
     def __init__(
```

### Comparing `dartrs-0.1.4/python/dartrs/utils.py` & `dartrs-0.1.5/python/dartrs/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+from typing import Literal
+
 from . import dartrs
 
+DType = Literal["fp16", "fp32"]
+Device = Literal["cpu", "cuda"]
+
 
 def get_generation_config(
     prompt: str,
     tokenizer: dartrs.DartTokenizer,
     device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
     eos_token: str | None = None,
     max_new_tokens: int | None = 256,
```

### Comparing `dartrs-0.1.4/python/dartrs/v2.py` & `dartrs-0.1.5/python/dartrs/v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,19 @@
 from typing import Literal, Generator
 
 from . import dartrs
+from . import utils
 
+LengthTag = Literal["very_short", "short", "medium", "long", "very_long"]
 
-LengthTag = (
-    Literal["very_short"]
-    | Literal["short"]
-    | Literal["medium"]
-    | Literal["long"]
-    | Literal["very_long"]
-)
-
-AspectRatioTag = (
-    Literal["ultra_wide"]
-    | Literal["wide"]
-    | Literal["square"]
-    | Literal["tall"]
-    | Literal["ultra_tall"]
-)
-
-RatingTag = (
-    Literal["sfw"]
-    | Literal["general"]
-    | Literal["sensitive"]
-    | Literal["nsfw"]
-    | Literal["questionable"]
-    | Literal["explicit"]
-)
+AspectRatioTag = Literal["ultra_wide", "wide", "square", "tall", "ultra_tall"]
 
-IdentityTag = Literal["none"] | Literal["lax"] | Literal["strict"]
+RatingTag = Literal["sfw", "general", "sensitive", "nsfw", "questionable", "explicit"]
+
+IdentityTag = Literal["none", "lax", "strict"]
 
 
 def compose_prompt(
     prompt: str = "",
     copyright: str = "",
     character: str = "",
     rating: RatingTag = "general",
@@ -100,25 +81,41 @@
 
 class MixtralModel(V2Model):
     @classmethod
     def from_pretrained(
         cls,
         hub_name: str,
         revision: str | None = None,
-        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
-        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
+        dtype: utils.DType = "fp32",
+        device: utils.Device = "cpu",
         auth_token: str | None = None,
     ) -> V2Model:
-        return cls(dartrs.DartV2Mixtral(hub_name, revision, dtype, device, auth_token))
+        return cls(
+            dartrs.DartV2Mixtral(
+                hub_name,
+                revision,
+                dartrs.DartDType(dtype),
+                dartrs.DartDevice(device),
+                auth_token,
+            )
+        )
 
 
 class MistralModel(V2Model):
     @classmethod
     def from_pretrained(
         cls,
         hub_name: str,
         revision: str | None = None,
-        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
-        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
+        dtype: utils.DType = "fp32",
+        device: utils.Device = "cpu",
         auth_token: str | None = None,
     ) -> V2Model:
-        return cls(dartrs.DartV2Mistral(hub_name, revision, dtype, device, auth_token))
+        return cls(
+            dartrs.DartV2Mistral(
+                hub_name,
+                revision,
+                dartrs.DartDType(dtype),
+                dartrs.DartDevice(device),
+                auth_token,
+            )
+        )
```

### Comparing `dartrs-0.1.4/src/bindings/generation.rs` & `dartrs-0.1.5/src/bindings/generation.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/bindings/models.rs` & `dartrs-0.1.5/src/bindings/models.rs`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,27 @@
             DartDType::BF16 => DType::BF16,
             DartDType::FP16 => DType::F16,
             DartDType::FP32 => DType::F32,
         }
     }
 }
 
+#[pymethods]
+impl DartDType {
+    #[new]
+    fn from(dtype: String) -> PyResult<Self> {
+        match dtype.as_str() {
+            "bf16" => Ok(DartDType::BF16),
+            "fp16" => Ok(DartDType::FP16),
+            "fp32" => Ok(DartDType::FP32),
+            _ => Err(exceptions::PyValueError::new_err("invalid dtype")),
+        }
+    }
+}
+
 #[pyclass]
 #[derive(Debug, Clone)]
 pub(crate) enum DartDevice {
     Cpu {},
     Cuda { id: usize },
 }
 
@@ -48,20 +61,28 @@
                 Ok(device) => device,
                 Err(_e) => Device::Cpu,
             },
         }
     }
 }
 
-// #[pyclass]
-// #[derive(Debug, Clone)]
-// pub(crate) struct NextToken {
-//     pub token: u32,
-//     pub cache: DartGenerationCache,
-// }
+#[pymethods]
+impl DartDevice {
+    #[new]
+    fn new(device: String) -> PyResult<Self> {
+        if device.starts_with("cuda") {
+            let id = device[4..].parse().unwrap_or(0);
+            Ok(DartDevice::Cuda { id })
+        } else if device == "cpu" {
+            Ok(DartDevice::Cpu {})
+        } else {
+            Err(exceptions::PyValueError::new_err("invalid device"))
+        }
+    }
+}
 
 macro_rules! generate {
     ($self:ident, $config:ident) => {
         match $self.model.generate(&mut $config) {
             Ok(text) => Ok(text),
             Err(e) => Err(exceptions::PyOSError::new_err(format!(
                 "Failed to generate text: {}",
@@ -100,17 +121,17 @@
                 return Err(exceptions::PyOSError::new_err(format!(
                     "Failed to create API: {}",
                     e
                 )))
             }
         };
         let dtype = dtype.unwrap_or(DartDType::FP32);
+        let dtype = DType::from(dtype);
         let device = device.unwrap_or(DartDevice::Cpu {});
         let device = Device::from(device);
-        let dtype = DType::from(dtype);
 
         let repo = ModelRepositoy::new(hub_name.clone(), api.clone(), revision);
 
         let model = MistralModelBuilder::load(&repo, dtype, &device);
         match model {
             Ok(model) => Ok(Self { model }),
             Err(e) => Err(exceptions::PyOSError::new_err(format!(
```

### Comparing `dartrs-0.1.4/src/bindings/prompt.rs` & `dartrs-0.1.5/src/bindings/prompt.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/bindings/tags.rs` & `dartrs-0.1.5/src/bindings/tags.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/configs.rs` & `dartrs-0.1.5/src/configs.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/generation.rs` & `dartrs-0.1.5/src/generation.rs`

 * *Files 4% similar despite different names*

```diff
@@ -190,14 +190,15 @@
             .chain($cache.output_tokens.iter())
             .cloned()
             .collect();
 
         let start_pos = tokens.len().saturating_sub(context_size);
         let context = &tokens[start_pos..];
         let input = Tensor::new(context, &$config.device)?.unsqueeze(0)?;
+        let input = input.to_device($self.device())?;
         let logits = $self.forward(&input, start_pos)?;
         let logits = logits.squeeze(0)?.squeeze(0)?.to_dtype(DType::F32)?;
 
         let next_token = &$config.logits_processor.sample(&logits)?;
         let next_token = next_token.clone();
         $cache.output_tokens.push(next_token);
```

### Comparing `dartrs-0.1.4/src/lib.rs` & `dartrs-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/logits_processor.rs` & `dartrs-0.1.5/src/logits_processor.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/models/mistral.rs` & `dartrs-0.1.5/src/models/mistral.rs`

 * *Files 1% similar despite different names*

```diff
@@ -359,8 +359,16 @@
     }
 
     pub fn clear_kv_cache(&mut self) {
         for layer in self.layers.iter_mut() {
             layer.clear_kv_cache()
         }
     }
+
+    pub fn device(&self) -> &Device {
+        &self.device
+    }
+
+    pub fn dtype(&self) -> DType {
+        self.dtype
+    }
 }
```

### Comparing `dartrs-0.1.4/src/models/mixtral.rs` & `dartrs-0.1.5/src/models/mixtral.rs`

 * *Files 1% similar despite different names*

```diff
@@ -304,16 +304,17 @@
         let mut ys = xs.zeros_like()?;
         for (expert_idx, expert_layer) in self.experts.iter().enumerate() {
             let top_x = &top_x[expert_idx];
             if top_x.is_empty() {
                 continue;
             }
             let top_x = Tensor::new(top_x.as_slice(), xs.device())?;
-            let selected_rws =
-                Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?.reshape(((), 1))?;
+            let selected_rws = Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?
+                .to_dtype(xs.dtype())?
+                .reshape(((), 1))?;
             // Index the correct hidden states and compute the expert hidden state for
             // the current expert. We need to make sure to multiply the output hidden
             // states by `routing_weights` on the corresponding tokens (top-1 and top-2)
             let current_state = xs.index_select(&top_x, 0)?.reshape(((), hidden_dim))?;
             // current_hidden_states = expert_layer(current_state, routing_weights[top_x_list, idx_list, None])
             let current_hidden_states = expert_layer.forward(&current_state)?;
             let current_hidden_states = current_hidden_states.broadcast_mul(&selected_rws)?;
@@ -457,8 +458,16 @@
     }
 
     pub fn clear_kv_cache(&mut self) {
         for layer in self.layers.iter_mut() {
             layer.clear_kv_cache()
         }
     }
+
+    pub fn device(&self) -> &Device {
+        &self.device
+    }
+
+    pub fn dtype(&self) -> DType {
+        self.dtype
+    }
 }
```

### Comparing `dartrs-0.1.4/src/models.rs` & `dartrs-0.1.5/src/models.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/prompt.rs` & `dartrs-0.1.5/src/prompt.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/src/tags.rs` & `dartrs-0.1.5/src/tags.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/tests/test_configs.py` & `dartrs-0.1.5/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/tests/test_model.py` & `dartrs-0.1.5/tests/test_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,64 @@
 from dartrs.dartrs import DartTokenizer, GenerationCache
 from dartrs.v2 import (
     MixtralModel,
     compose_prompt,
 )
-from dartrs.utils import get_generation_config
+from dartrs.utils import get_generation_config, DType, Device
 from random import randint
 
 
-def prepare_models():
-    model = MixtralModel.from_pretrained("p1atdev/dart-v2-moe-sft")
+def prepare_models(dtype: DType = "fp32", device: Device = "cpu"):
+    model = MixtralModel.from_pretrained("p1atdev/dart-v2-moe-sft", dtype=dtype)
     tokenizer = DartTokenizer.from_pretrained("p1atdev/dart-v2-moe-sft")
 
     return model, tokenizer
 
 
 def test_generate():
     model, tokenizer = prepare_models()
 
     prompt = compose_prompt(
         prompt="1girl, cat ears",
     )
     config = get_generation_config(
         prompt=prompt,
         tokenizer=tokenizer,
+        seed=42,
+    )
+
+    output = model.generate(config)
+    assert output is not None
+
+
+def test_generate_fp16_cpu():
+    model, tokenizer = prepare_models(dtype="fp16", device="cpu")
+
+    prompt = compose_prompt(
+        prompt="1girl, cat ears",
+    )
+    config = get_generation_config(
+        prompt=prompt,
+        tokenizer=tokenizer,
+        seed=42,
+    )
+
+    output = model.generate(config)
+    assert output is not None
+
+
+def test_generate_fp16_cuda():
+    model, tokenizer = prepare_models(dtype="fp16", device="cuda")
+
+    prompt = compose_prompt(
+        prompt="1girl, cat ears",
+    )
+    config = get_generation_config(
+        prompt=prompt,
+        tokenizer=tokenizer,
         seed=42,
     )
 
     output = model.generate(config)
     assert output is not None
```

### Comparing `dartrs-0.1.4/tests/test_prompt.py` & `dartrs-0.1.5/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/tests/test_tokenizer.py` & `dartrs-0.1.5/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/tests/test_v2.py` & `dartrs-0.1.5/tests/test_v2.py`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.4/Cargo.lock` & `dartrs-0.1.5/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "candle-core"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
+source = "git+https://github.com/huggingface/candle.git#13c64f6828360a9cb9b58b4f817e4f3b8316388c"
 dependencies = [
  "byteorder",
  "candle-kernels",
  "cudarc",
  "gemm",
  "half",
  "memmap2",
@@ -135,37 +135,37 @@
  "yoke",
  "zip",
 ]
 
 [[package]]
 name = "candle-kernels"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
+source = "git+https://github.com/huggingface/candle.git#13c64f6828360a9cb9b58b4f817e4f3b8316388c"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-nn"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
+source = "git+https://github.com/huggingface/candle.git#13c64f6828360a9cb9b58b4f817e4f3b8316388c"
 dependencies = [
  "candle-core",
  "half",
  "num-traits",
  "rayon",
  "safetensors",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#d9bc5ec15164ecb583dbb25653edd89e08e6cbd0"
+source = "git+https://github.com/huggingface/candle.git#13c64f6828360a9cb9b58b4f817e4f3b8316388c"
 dependencies = [
  "byteorder",
  "candle-core",
  "candle-nn",
  "fancy-regex",
  "num-traits",
  "rand",
@@ -300,15 +300,15 @@
  "darling_core",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dartrs"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "candle-core",
  "candle-nn",
  "candle-transformers",
  "hf-hub",
  "openssl",
@@ -1555,17 +1555,17 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "2.0.62"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f660c3bfcefb88c538776b6685a0c472e3128b51e74d48793dc2a488196e8eb"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `dartrs-0.1.4/pyproject.toml` & `dartrs-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "dartrs"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = [{ name = "Plat", email = "contact@p1at.dev" }]
 dependencies = []
 readme = "README.md"
 license = { text = "Apache-2.0" }
 
 [tool.maturin]
```

### Comparing `dartrs-0.1.4/PKG-INFO` & `dartrs-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dartrs
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: 
 Author-email: Plat <contact@p1at.dev>
 License: Apache-2.0
@@ -31,15 +31,15 @@
     V2Model,
 )
 import time
 import os
 
 MODEL_NAME = "p1atdev/dart-v2-moe-sft"
 
-model = MixtralModel.from_pretrained(MODEL_NAME)
+model = MixtralModel.from_pretrained(MODEL_NAME, dtype="fp16")
 tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
 
 config = get_generation_config(
     prompt=compose_prompt(
         copyright="vocaloid",
         character="hatsune miku",
         rating="general", # sfw, general, sensitive, nsfw, questionable, explicit
@@ -55,10 +55,10 @@
 start = time.time()
 output = model.generate(config)
 end = time.time()
 
 print(output)
 print(f"Time taken: {end - start:.2f}s")
 # Output:
-# cowboy shot, detached sleeves, empty eyes, green eyes, green hair, green necktie, hair in own mouth, hair ornament, letterboxed, light frown, long hair, long sleeves, looking to the side, necktie, parted lips, shirt, sleeveless, sleeveless shirt, twintails, wing collar
-# Time taken: 0.26s
+# cowboy shot, detached sleeves, expressionless, from side, hair ornament, halftone, hairclip, holding, limited palette, long hair, looking at viewer, miniskirt, necktie, pleated skirt, shirt, simple background, skirt, sleeveless, sleeveless shirt, straight-on, thighhighs, twintails, very long hair, zettai ryouiki
+# Time taken: 0.22s
 ```
```

