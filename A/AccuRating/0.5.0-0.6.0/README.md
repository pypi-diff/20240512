# Comparing `tmp/accurating-0.5.0.tar.gz` & `tmp/accurating-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.5.0.tar", max compression
+gzip compressed data, was "accurating-0.6.0.tar", max compression
```

## Comparing `accurating-0.5.0.tar` & `accurating-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.5.0/LICENSE
--rw-r--r--   0        0        0     6438 2023-05-16 03:53:39.354834 accurating-0.5.0/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.5.0/accurating/__init__.py
--rw-r--r--   0        0        0    11050 2023-05-16 03:41:24.848579 accurating-0.5.0/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.5.0/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3188 2023-05-16 03:43:28.310705 accurating-0.5.0/accurating/tests/model_test.py
--rw-r--r--   0        0        0      725 2023-05-16 03:54:22.575075 accurating-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7192 1970-01-01 00:00:00.000000 accurating-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-12 13:05:50.822442 accurating-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6508 2024-05-12 14:04:18.765034 accurating-0.6.0/README.md
+-rw-r--r--   0        0        0      231 2024-05-12 13:05:50.822442 accurating-0.6.0/accurating/__init__.py
+-rw-r--r--   0        0        0    11290 2024-05-12 14:56:56.611698 accurating-0.6.0/accurating/model.py
+-rw-r--r--   0        0        0        0 2024-05-12 13:05:50.822442 accurating-0.6.0/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3196 2024-05-12 15:04:01.971469 accurating-0.6.0/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      725 2024-05-12 15:09:59.062143 accurating-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7313 1970-01-01 00:00:00.000000 accurating-0.6.0/PKG-INFO
```

### Comparing `accurating-0.5.0/LICENSE` & `accurating-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.5.0/README.md` & `accurating-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 
 ```shell
 git config --global core.hooksPath .githooks/
 ```
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
+virtualenv /tmp/venv
+source /tmp/venv/bin/activate
+pip install poetry
 poetry install
 poetry run pytest
 poetry run mypy .
 
 # edit stuff; increase version
 poetry build
 poetry publish
```

### Comparing `accurating-0.5.0/accurating/model.py` & `accurating-0.6.0/accurating/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,17 +141,20 @@
     assert p1s.shape == (data_size,)
     assert p2s.shape == (data_size,)
     assert p1_win_probs.shape == (data_size,)
 
     winner_prior = config.winner_prior_rating / config.rating_difference_for_2_to_1_odds
     loser_prior = config.loser_prior_rating / config.rating_difference_for_2_to_1_odds
 
+    def get_ratings(p):
+        return p['season_rating'] + p['shared_rating']
+
     def model(params):
         log_likelihood = 0.0
-        ratings = params['rating']
+        ratings = get_ratings(params)
         assert ratings.shape == (player_count, season_count)
         p1_ratings = ratings[p1s, seasons]
         p2_ratings = ratings[p2s, seasons]
 
         assert p1_ratings.shape == (data_size,)
         assert p2_ratings.shape == (data_size,)
 
@@ -179,27 +182,29 @@
         # winner_win_prob_log = 0.0
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
         # return jnp.sum(winner_win_prob_log) - 0.005*jnp.sum(cons ** 2) # or mean?
 
     # Optimize for these params:
-    rating = jnp.zeros([player_count, season_count], dtype=jnp.float64) + (loser_prior + winner_prior) / 2.0
-    params = { 'rating': rating }
+    shared_rating = jnp.zeros([player_count, 1], dtype=jnp.float64) + (loser_prior + winner_prior) / 2.0
+    season_rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
+    params = { 'season_rating': season_rating, 'shared_rating': shared_rating }
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
     lr = float(config.initial_lr)
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
     last_eval = -1e8  # eval of initial data is -1, but regularizations might push it lower.
     last_grad = tree_map(jnp.zeros_like, params)
     last_reset_step = 0
 
+
     for i in range(config.max_steps):
         (eval, model_fit), grad = jax.value_and_grad(model, has_aux=True)(params)
 
         if False:
             # Standard batch gradient descent algorithm works too. Just use good LR.
             params = tree_map(lambda p, g: p + lr * g, params, grad)
         else:
@@ -215,33 +220,34 @@
                 params, eval, grad = last_params, last_eval, last_grad
             else:
                 last_params, last_eval, last_grad = params, eval, grad
             momentum = tree_map(lambda m, g: m_lr * m + g, momentum, grad)
             params = tree_map(lambda p, m: p + lr * m, params, momentum)
 
         max_d_rating = jnp.max(
-            jnp.abs(params['rating'] - last_params['rating']))
+            jnp.abs(get_ratings(params) - get_ratings(last_params)))
 
         if config.do_log:
-            g = jnp.linalg.norm(grad['rating'])
+            g = get_ratings(grad)
+            g = jnp.sqrt(jnp.mean(g*g))
             print(
-                f'Step {i:4}: eval={jnp.exp2(eval):0.12f} pred_power={model_fit:0.6f} lr={lr: 4.4f} grad={g:2.4f} delta={max_d_rating}')
+                f'Step {i:4}: eval={jnp.exp2(eval):0.12f} pred_power={model_fit:0.6f} lr={lr: 4.4f} grad={g:2.8f} delta={max_d_rating}')
 
         if max_d_rating < 1e-15:
             break
 
         lr *= 1.5 ** (1.0 / 12)
 
     def postprocess():
         rating = {}
         last_rating = []
         for id, name in enumerate(data.player_name):
             rating[name] = {}
             for season in range(season_count):
-                rating[name][season] = float(params['rating'][id, season]) * config.rating_difference_for_2_to_1_odds
+                rating[name][season] = float(get_ratings(params)[id, season]) * config.rating_difference_for_2_to_1_odds
             last_rating.append((rating[name][season_count - 1], name))
         if config.do_log:
             headers = ['Nick']
             for season in range(season_count-1, -1, -1):
                 headers.append(f'S{season}')
             last_rating.sort(reverse=True)
             table = []
```

### Comparing `accurating-0.5.0/accurating/tests/model_test.py` & `accurating-0.6.0/accurating/tests/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     model = accurating.fit(test_data, config)
     elos = [[model.rating[f'p{pl}'][season]
              for season in range(2)] for pl in range(3)]
     elos = np.array(elos)
 
     elos = elos - jnp.min(elos, axis=0, keepdims=True)
     err = jnp.linalg.norm(elos - jnp.array(true_elos) * 100.0)
-    assert err < 0.0001, f'FAIL err={err}; results={model}'
+    assert err < 0.001, f'FAIL err={err}; {elos=}; results={model}'
 
 
 def test_data_from_dicts():
     json_str = """
     [
       {
         "p1": "Leon",
@@ -100,13 +100,13 @@
     )
     model = accurating.fit(data, cfg)
 
     # ratings = np.array([[model.rating[pl][s] for s in range(len(season))] for pl in player_name])
     assert_almost_equal(model.rating['Alusia'][0], 0.0)
     assert_almost_equal(model.rating['Alusia'][1], 0.0)
 
-    v = 13.45060623432789
-    v2 = 26.901228584915188
+    v = 13.45061478482753
+    v2 = 26.901218694229996
     assert_almost_equal(model.rating['Caesar'][0], -v)
     assert_almost_equal(model.rating['Caesar'][1], v2)
     assert_almost_equal(model.rating['Leon'][0], v)
     assert_almost_equal(model.rating['Leon'][1], -v2)
```

### Comparing `accurating-0.5.0/pyproject.toml` & `accurating-0.6.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.5.0"
+version = "0.6.0"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.5.0/PKG-INFO` & `accurating-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: accurating
-Version: 0.5.0
+Name: AccuRating
+Version: 0.6.0
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
 Requires-Dist: types-tabulate (>=0.9.0.2,<0.10.0.0)
 Project-URL: Documentation, https://lukaszlew.github.io/accurating/
 Description-Content-Type: text/markdown
@@ -147,14 +148,17 @@
 
 ```shell
 git config --global core.hooksPath .githooks/
 ```
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
+virtualenv /tmp/venv
+source /tmp/venv/bin/activate
+pip install poetry
 poetry install
 poetry run pytest
 poetry run mypy .
 
 # edit stuff; increase version
 poetry build
 poetry publish
```

