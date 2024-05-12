# Comparing `tmp/optimistix-0.0.6.tar.gz` & `tmp/optimistix-0.0.7.tar.gz`

## Comparing `optimistix-0.0.6.tar` & `optimistix-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/__init__.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_ad.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_adjoint.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_custom_types.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_fixed_point.py
--rw-r--r--   0        0        0    13629 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_iterate.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_least_squares.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_minimise.py
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_misc.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_root_find.py
--rw-r--r--   0        0        0    12249 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_search.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solution.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/__init__.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/backtracking.py
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/best_so_far.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/bfgs.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/bisection.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/dogleg.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/fixed_point.py
--rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/gauss_newton.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/gradient_methods.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/learning_rate.py
--rw-r--r--   0        0        0    15183 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/levenberg_marquardt.py
--rw-r--r--   0        0        0    20196 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/nelder_mead.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/newton_chord.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/nonlinear_cg.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/optax.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/_solver/trust_region.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/compat/__init__.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/compat/_impl.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 optimistix-0.0.6/optimistix/internal/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 optimistix-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 optimistix-0.0.6/LICENSE
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 optimistix-0.0.6/README.md
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 optimistix-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    16863 2020-02-02 00:00:00.000000 optimistix-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/__init__.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_ad.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_adjoint.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_custom_types.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_fixed_point.py
+-rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_iterate.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_least_squares.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_minimise.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_misc.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_root_find.py
+-rw-r--r--   0        0        0    11834 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_search.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solution.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/backtracking.py
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/best_so_far.py
+-rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/bfgs.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/bisection.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/dogleg.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/fixed_point.py
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/gauss_newton.py
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/gradient_methods.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/learning_rate.py
+-rw-r--r--   0        0        0    15545 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/levenberg_marquardt.py
+-rw-r--r--   0        0        0    19637 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/nelder_mead.py
+-rw-r--r--   0        0        0    10295 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/newton_chord.py
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/nonlinear_cg.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/optax.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/_solver/trust_region.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/compat/__init__.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/compat/_impl.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 optimistix-0.0.7/optimistix/internal/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 optimistix-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 optimistix-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 optimistix-0.0.7/README.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 optimistix-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    17360 2020-02-02 00:00:00.000000 optimistix-0.0.7/PKG-INFO
```

### Comparing `optimistix-0.0.6/optimistix/_ad.py` & `optimistix-0.0.7/optimistix/_ad.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import types
 from collections.abc import Callable
 from typing import TypeVar
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
+import jax.numpy as jnp
 import jax.tree_util as jtu
 import lineax as lx
 from equinox.internal import ω
 from jaxtyping import PyTree
 
 from ._misc import tree_full_like
 
@@ -72,15 +59,15 @@
     root, residual = _implicit_impl(fn_primal, fn_rewrite, inputs, tags, linear_solver)
     return root, jtu.tree_map(eqxi.nondifferentiable_backward, residual)
 
 
 @eqx.filter_custom_jvp
 def _implicit_impl(fn_primal, fn_rewrite, inputs, tags, linear_solver):
     del fn_rewrite, tags, linear_solver
-    return fn_primal(inputs)
+    return jtu.tree_map(jnp.asarray, fn_primal(inputs))
 
 
 def _assert_false(x):
     assert False
 
 
 def _is_none(x):
```

### Comparing `optimistix-0.0.6/optimistix/_adjoint.py` & `optimistix-0.0.7/optimistix/_adjoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,21 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import abc
 import functools as ft
 from collections.abc import Callable
 from typing import Optional
 
 import equinox as eqx
 import equinox.internal as eqxi
 import lineax as lx
 from jaxtyping import Array, PyTree
 
 from ._ad import implicit_jvp
 
 
-class AbstractAdjoint(eqx.Module):
+class AbstractAdjoint(eqx.Module, strict=True):
     """The abstract base class of all adjoints."""
 
     @abc.abstractmethod
     def apply(
         self,
         primal_fn: Callable,
         rewrite_fn: Callable,
@@ -38,15 +24,15 @@
     ) -> PyTree[Array]:
         """Runs the main solver loop. Subclasses can override this to provide custom
         autodifferentiation behaviour; see for example the implementation of
         [`optimistix.ImplicitAdjoint`][].
         """
 
 
-class RecursiveCheckpointAdjoint(AbstractAdjoint):
+class RecursiveCheckpointAdjoint(AbstractAdjoint, strict=True):
     """Backpropagate by differentiating through the iterates directly.
 
     Uses a binomial checkpointing scheme to keep memory usage low.
 
     !!! info
 
         Note that this cannot be forward-mode autodifferentiated. (E.g. using
@@ -124,15 +110,15 @@
         del rewrite_fn, tags
         while_loop = ft.partial(
             eqxi.while_loop, kind="checkpointed", checkpoints=self.checkpoints
         )
         return primal_fn(inputs + (while_loop,))
 
 
-class ImplicitAdjoint(AbstractAdjoint):
+class ImplicitAdjoint(AbstractAdjoint, strict=True):
     r"""Backpropagate via the [implicit function theorem](https://en.wikipedia.org/wiki/Implicit_function_theorem).
 
     For example, using the root-finding case by way of example: suppose we find the
     root `y(θ)` for which `f(y(θ), θ) = 0`.
     Then we can skip backpropagating through the solver by computing
     $\frac{\mathrm{d}y}{\mathrm{d}\theta} = - (\frac{\mathrm{d}f}{\mathrm{d}y})^{-1}\frac{\mathrm{d}f}{\mathrm{d}\theta}$
     via the implicit function theorem.
```

### Comparing `optimistix-0.0.6/optimistix/_fixed_point.py` & `optimistix-0.0.7/optimistix/_fixed_point.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import Any, cast, Generic, Optional, Union
 
 import equinox as eqx
 import jax
 import jax.tree_util as jtu
 from equinox.internal import ω
 from jaxtyping import PyTree
@@ -26,15 +12,17 @@
 from ._least_squares import AbstractLeastSquaresSolver
 from ._minimise import AbstractMinimiser
 from ._misc import inexact_asarray, NoneAux, OutAsArray
 from ._root_find import AbstractRootFinder, root_find
 from ._solution import Solution
 
 
-class AbstractFixedPointSolver(AbstractIterativeSolver[Y, Y, Aux, SolverState]):
+class AbstractFixedPointSolver(
+    AbstractIterativeSolver[Y, Y, Aux, SolverState], strict=True
+):
     """Abstract base class for all fixed point solvers."""
 
 
 def _rewrite_fn(fixed_point, _, inputs):
     fixed_point_fn, _, _, args, *_ = inputs
     del inputs
     f_val, _ = fixed_point_fn(fixed_point, args)
```

### Comparing `optimistix-0.0.6/optimistix/_iterate.py` & `optimistix-0.0.7/optimistix/_iterate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import abc
 from collections.abc import Callable
 from typing import Any, Generic, Optional, TYPE_CHECKING
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
@@ -33,15 +19,17 @@
 
 if TYPE_CHECKING:
     _Node = Any
 else:
     _Node = eqxi.doc_repr(Any, "Node")
 
 
-class AbstractIterativeSolver(eqx.Module, Generic[Y, Out, Aux, SolverState]):
+class AbstractIterativeSolver(
+    eqx.Module, Generic[Y, Out, Aux, SolverState], strict=True
+):
     """Abstract base class for all iterative solvers."""
 
     rtol: AbstractVar[float]
     atol: AbstractVar[float]
     norm: AbstractVar[Callable[[PyTree], Scalar]]
 
     @abc.abstractmethod
```

### Comparing `optimistix-0.0.6/optimistix/_least_squares.py` & `optimistix-0.0.7/optimistix/_least_squares.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import Any, cast, Generic, Optional, Union
 
 import equinox as eqx
 import jax
 import jax.tree_util as jtu
 from jaxtyping import PyTree, Scalar
 
@@ -23,15 +9,17 @@
 from ._custom_types import Args, Aux, Fn, MaybeAuxFn, Out, SolverState, Y
 from ._iterate import AbstractIterativeSolver, iterative_solve
 from ._minimise import AbstractMinimiser, minimise
 from ._misc import inexact_asarray, NoneAux, OutAsArray, sum_squares
 from ._solution import Solution
 
 
-class AbstractLeastSquaresSolver(AbstractIterativeSolver[Y, Out, Aux, SolverState]):
+class AbstractLeastSquaresSolver(
+    AbstractIterativeSolver[Y, Out, Aux, SolverState], strict=True
+):
     """Abstract base class for all least squares solvers."""
 
 
 def _rewrite_fn(optimum, _, inputs):
     residual_fn, _, _, args, *_ = inputs
     del inputs
```

### Comparing `optimistix-0.0.6/optimistix/_minimise.py` & `optimistix-0.0.7/optimistix/_minimise.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import Any, cast, Optional
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from jaxtyping import PyTree, Scalar
@@ -23,15 +9,17 @@
 from ._adjoint import AbstractAdjoint, ImplicitAdjoint
 from ._custom_types import Aux, Fn, MaybeAuxFn, SolverState, Y
 from ._iterate import AbstractIterativeSolver, iterative_solve
 from ._misc import inexact_asarray, NoneAux, OutAsArray
 from ._solution import Solution
 
 
-class AbstractMinimiser(AbstractIterativeSolver[Y, Scalar, Aux, SolverState]):
+class AbstractMinimiser(
+    AbstractIterativeSolver[Y, Scalar, Aux, SolverState], strict=True
+):
     """Abstract base class for all minimisers."""
 
 
 def _rewrite_fn(minimum, _, inputs):
     minimise_fn, _, _, args, *_ = inputs
     del inputs
```

### Comparing `optimistix-0.0.6/optimistix/_misc.py` & `optimistix-0.0.7/optimistix/_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, Literal, overload, TypeVar, Union
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.core
@@ -86,28 +72,28 @@
 def resolve_rcond(rcond, n, m, dtype):
     if rcond is None:
         return jnp.finfo(dtype).eps * max(n, m)
     else:
         return jnp.where(rcond < 0, jnp.finfo(dtype).eps, rcond)
 
 
-class NoneAux(eqx.Module):
+class NoneAux(eqx.Module, strict=True):
     """Wrap a function `fn` so it returns a dummy aux value `None`
 
     NoneAux is used to give a consistent API between functions which have an aux
     and functions which do not, allowing us to avoid unnecessary aux handling.
     """
 
     fn: Callable
 
     def __call__(self, *args, **kwargs):
         return self.fn(*args, **kwargs), None
 
 
-class OutAsArray(eqx.Module):
+class OutAsArray(eqx.Module, strict=True):
     """Wrap a minimisation/root-find/etc. function so that its mathematical outputs are
     all inexact arrays, and its auxiliary outputs are all arrays.
     """
 
     fn: Callable
 
     def __call__(self, *args, **kwargs):
```

### Comparing `optimistix-0.0.6/optimistix/_root_find.py` & `optimistix-0.0.7/optimistix/_root_find.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import Any, cast, Optional, Union
 
 import equinox as eqx
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox import AbstractVar
 from jaxtyping import PyTree
@@ -25,15 +11,17 @@
 from ._iterate import AbstractIterativeSolver, iterative_solve
 from ._least_squares import AbstractLeastSquaresSolver, least_squares
 from ._minimise import AbstractMinimiser, minimise
 from ._misc import inexact_asarray, NoneAux, OutAsArray, tree_full_like
 from ._solution import Solution
 
 
-class AbstractRootFinder(AbstractIterativeSolver[Y, Out, Aux, SolverState]):
+class AbstractRootFinder(
+    AbstractIterativeSolver[Y, Out, Aux, SolverState], strict=True
+):
     """Abstract base class for all root finders."""
 
 
 def _rewrite_fn(root, _, inputs):
     root_fn, _, _, args, *_ = inputs
     del inputs
     f_val, _ = root_fn(root, args)
```

### Comparing `optimistix-0.0.6/optimistix/_search.py` & `optimistix-0.0.7/optimistix/_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 """We use notions of "searches" and "descents" to generalise line searches, trust
 regions, and learning rates.
 
 For example, the classical gradient descent algorithm is given by setting the search
 to be `optimistix.LearningRate`, and setting the descent to be
 `optimistix.SteepestDescent`.
 
@@ -49,18 +35,18 @@
     SearchState,
     Y,
 )
 from ._misc import sum_squares
 from ._solution import RESULTS
 
 
-class FunctionInfo(eqx.Module):
-    """Different solvers (BFGS, Levenberg--Marquardt, ...) evaluate different quantities
-    of the objective function. Some may compute gradient information, some may provide
-    approximate Hessian information, etc.
+class FunctionInfo(eqx.Module, strict=eqx.StrictConfig(allow_abstract_name=True)):
+    """Different solvers (BFGS, Levenberg--Marquardt, ...) evaluate different
+    quantities of the objective function. Some may compute gradient information,
+    some may provide approximate Hessian information, etc.
 
     This enumeration-ish object captures the different variants.
 
     Available variants are
     `optimistix.FunctionInfo.{Eval, EvalGrad, EvalGradHessian, EvalGradHessianInv, Residual, ResidualJac}`.
     """  # noqa: E501
 
@@ -75,82 +61,82 @@
     def as_min(self) -> Scalar:
         """For a minimisation problem, returns f(y). For a least-squares problem,
         returns 0.5*residuals^2 -- i.e. its loss as a minimisation problem.
         """
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class Eval(FunctionInfo):
+class Eval(FunctionInfo, strict=True):
     """Has a `.f` attribute describing `fn(y)`. Used when no gradient information is
     available.
     """
 
     f: Scalar
 
     def as_min(self):
         return self.f
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class EvalGrad(FunctionInfo, Generic[Y]):
+class EvalGrad(FunctionInfo, Generic[Y], strict=True):
     """Has a `.f` attribute as with [`optimistix.FunctionInfo.Eval`][]. Also has a
     `.grad` attribute describing `d(fn)/dy`. Used with first-order solvers for
     minimisation problems. (E.g. gradient descent; nonlinear CG.)
     """
 
     f: Scalar
     grad: Y
 
     def as_min(self):
         return self.f
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class EvalGradHessian(FunctionInfo, Generic[Y]):
+class EvalGradHessian(FunctionInfo, Generic[Y], strict=True):
     """Has `.f` and `.grad` attributes as with [`optimistix.FunctionInfo.EvalGrad`][].
     Also has a `.hessian` attribute describing (an approximation to) the Hessian of
     `fn` at `y`. Used with quasi-Newton minimisation algorithms, like BFGS.
     """
 
     f: Scalar
     grad: Y
     hessian: lx.AbstractLinearOperator
 
     def as_min(self):
         return self.f
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class EvalGradHessianInv(FunctionInfo, Generic[Y]):
+class EvalGradHessianInv(FunctionInfo, Generic[Y], strict=True):
     """As [`optimistix.FunctionInfo.EvalGradHessian`][], but records the (approximate)
     inverse-Hessian instead. Has `.f` and `.grad` and `.hessian_inv` attributes.
     """
 
     f: Scalar
     grad: Y
     hessian_inv: lx.AbstractLinearOperator
 
     def as_min(self):
         return self.f
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class Residual(FunctionInfo, Generic[Out]):
+class Residual(FunctionInfo, Generic[Out], strict=True):
     """Has a `.residual` attribute describing `fn(y)`. Used with least squares problems,
     for which `fn` returns residuals.
     """
 
     residual: Out
 
     def as_min(self):
         return 0.5 * sum_squares(self.residual)
 
 
 # NOT PUBLIC, despite lacking an underscore. This is so pyright gets the name right.
-class ResidualJac(FunctionInfo, Generic[Y, Out]):
+class ResidualJac(FunctionInfo, Generic[Y, Out], strict=True):
     """Records the Jacobian `d(fn)/dy` as a linear operator. Used for least squares
     problems, for which `fn` returns residuals. Has `.residual` and `.jac` and `.grad`
     attributes, where `residual = fn(y)`, `jac = d(fn)/dy` and
     `grad = jac^T residual`.
 
     Takes just `residual` and `jac` as `__init__`-time arguments, from which `grad` is
     computed.
@@ -185,15 +171,15 @@
 FunctionInfo.ResidualJac = ResidualJac
 
 
 _FnInfo = TypeVar("_FnInfo", contravariant=True, bound=FunctionInfo)
 _FnEvalInfo = TypeVar("_FnEvalInfo", contravariant=True, bound=FunctionInfo)
 
 
-class AbstractDescent(eqx.Module, Generic[Y, _FnInfo, DescentState]):
+class AbstractDescent(eqx.Module, Generic[Y, _FnInfo, DescentState], strict=True):
     """The abstract base class for descents. A descent consumes a scalar (e.g. a step
     size), and returns the `diff` to take at point `y`, so that `y + diff` is the next
     iterate in a nonlinear optimisation problem.
 
     See [this documentation](./introduction.md) for more information.
     """
 
@@ -253,15 +239,17 @@
         **Returns:**
 
         A 2-tuple of `(y_diff, result)`, describing the delta to apply in
         y-space, and any error if computing the update was not successful.
         """
 
 
-class AbstractSearch(eqx.Module, Generic[Y, _FnInfo, _FnEvalInfo, SearchState]):
+class AbstractSearch(
+    eqx.Module, Generic[Y, _FnInfo, _FnEvalInfo, SearchState], strict=True
+):
     """The abstract base class for all searches. (Which are our generalisation of
     line searches, trust regions, and learning rates.)
 
     See [this documentation](./introduction.md) for more information.
     """
 
     @abc.abstractmethod
```

### Comparing `optimistix-0.0.6/optimistix/_solution.py` & `optimistix-0.0.7/optimistix/_solution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import Any, Generic
 
 import equinox as eqx
 import lineax as lx
 from jaxtyping import ArrayLike, PyTree
 
 from ._custom_types import Aux, Y
@@ -28,15 +14,15 @@
         "The maximum number of steps was reached in the nonlinear solver. "
         "The problem may not be solveable (e.g., a root-find on a function that has no "
         "roots), or you may need to increase `max_steps`."
     )
     nonlinear_divergence = "Nonlinear solve diverged."
 
 
-class Solution(eqx.Module, Generic[Y, Aux]):
+class Solution(eqx.Module, Generic[Y, Aux], strict=True):
     """The solution to a nonlinear solve.
 
     **Attributes:**
 
     - `value`: The solution to the solve.
     - `result`: An integer representing whether the solve was successful or not. This
         can be converted into a human-readable error message via
```

### Comparing `optimistix-0.0.6/optimistix/_solver/backtracking.py` & `optimistix-0.0.7/optimistix/_solver/backtracking.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from typing import cast, Union
 from typing_extensions import TypeAlias
 
 import equinox as eqx
 import jax.numpy as jnp
 from equinox.internal import ω
 from jaxtyping import Array, Bool, Scalar, ScalarLike
@@ -24,28 +10,30 @@
 from .._misc import (
     tree_dot,
 )
 from .._search import AbstractSearch, FunctionInfo
 from .._solution import RESULTS
 
 
-class _BacktrackingState(eqx.Module):
+class _BacktrackingState(eqx.Module, strict=True):
     step_size: Scalar
 
 
 _FnInfo: TypeAlias = Union[
     FunctionInfo.EvalGrad,
     FunctionInfo.EvalGradHessian,
     FunctionInfo.EvalGradHessianInv,
     FunctionInfo.ResidualJac,
 ]
 _FnEvalInfo: TypeAlias = FunctionInfo
 
 
-class BacktrackingArmijo(AbstractSearch[Y, _FnInfo, _FnEvalInfo, _BacktrackingState]):
+class BacktrackingArmijo(
+    AbstractSearch[Y, _FnInfo, _FnEvalInfo, _BacktrackingState], strict=True
+):
     """Perform a backtracking Armijo line search."""
 
     decrease_factor: ScalarLike = 0.5
     slope: ScalarLike = 0.1
     step_init: ScalarLike = 1.0
 
     def __post_init__(self):
```

### Comparing `optimistix-0.0.6/optimistix/_solver/best_so_far.py` & `optimistix-0.0.7/optimistix/_solver/best_so_far.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 from .._least_squares import AbstractLeastSquaresSolver
 from .._minimise import AbstractMinimiser
 from .._misc import sum_squares, tree_full_like, tree_where
 from .._root_find import AbstractRootFinder
 from .._solution import RESULTS
 
 
-class _BestSoFarState(eqx.Module, Generic[Y, Aux, SolverState]):
+class _BestSoFarState(eqx.Module, Generic[Y, Aux, SolverState], strict=True):
     best_y: Y
     best_aux: Aux
     best_loss: Scalar
     state: SolverState
 
 
 def _auxmented(fn, y, args):
     out, aux = fn(y, args)
     return out, (out, aux)
 
 
-class _BestSoFarSolver(AbstractIterativeSolver, Generic[Y, Out, Aux]):
+class _AbstractBestSoFarSolver(
+    AbstractIterativeSolver, Generic[Y, Out, Aux], strict=True
+):
     solver: AbstractVar[AbstractIterativeSolver[Y, Out, tuple[Out, Aux], Any]]
 
     @abc.abstractmethod
     def _to_loss(self, y: Y, f: Out) -> Scalar:
         ...
 
     @property  # pyright: ignore
@@ -113,15 +115,17 @@
         tags: frozenset[object],
         result: RESULTS,
     ) -> tuple[Y, Aux, dict[str, Any]]:
         return state.best_y, state.best_aux, {}
 
 
 class BestSoFarMinimiser(  # pyright: ignore
-    _BestSoFarSolver[Y, Scalar, Aux], AbstractMinimiser[Y, Aux, _BestSoFarState]
+    _AbstractBestSoFarSolver[Y, Scalar, Aux],
+    AbstractMinimiser[Y, Aux, _BestSoFarState],
+    strict=True,
 ):
     """Wraps another minimiser, to return the best-so-far value. That is, it makes a
     copy of the best `y` seen, and returns that.
     """
 
     solver: AbstractMinimiser[Y, tuple[Scalar, Aux], Any]
 
@@ -150,16 +154,17 @@
 BestSoFarMinimiser.__init__.__doc__ = """**Arguments:**
 
 - `solver`: the minimiser to wrap.  
 """
 
 
 class BestSoFarLeastSquares(  # pyright: ignore
-    _BestSoFarSolver[Y, Out, Aux],
+    _AbstractBestSoFarSolver[Y, Out, Aux],
     AbstractLeastSquaresSolver[Y, Out, Aux, _BestSoFarState],
+    strict=True,
 ):
     """Wraps another least-squares solver, to return the best-so-far value. That is, it
     makes a copy of the best `y` seen, and returns that.
     """
 
     solver: AbstractLeastSquaresSolver[Y, Out, tuple[Out, Aux], Any]
 
@@ -190,15 +195,17 @@
 BestSoFarLeastSquares.__init__.__doc__ = """**Arguments:**
 
 - `solver`: the least-squares solver to wrap.  
 """
 
 
 class BestSoFarRootFinder(  # pyright: ignore
-    _BestSoFarSolver[Y, Out, Aux], AbstractRootFinder[Y, Out, Aux, _BestSoFarState]
+    _AbstractBestSoFarSolver[Y, Out, Aux],
+    AbstractRootFinder[Y, Out, Aux, _BestSoFarState],
+    strict=True,
 ):
     """Wraps another root-finder, to return the best-so-far value. That is, it
     makes a copy of the best `y` seen, and returns that.
     """
 
     solver: AbstractRootFinder[Y, Out, tuple[Out, Aux], Any]
 
@@ -227,15 +234,17 @@
 BestSoFarRootFinder.__init__.__doc__ = """**Arguments:**
 
 - `solver`: the root-finder solver to wrap.  
 """
 
 
 class BestSoFarFixedPoint(  # pyright: ignore
-    _BestSoFarSolver[Y, Y, Aux], AbstractFixedPointSolver[Y, Aux, _BestSoFarState]
+    _AbstractBestSoFarSolver[Y, Y, Aux],
+    AbstractFixedPointSolver[Y, Aux, _BestSoFarState],
+    strict=True,
 ):
     """Wraps another fixed-point solver, to return the best-so-far value. That is, it
     makes a copy of the best `y` seen, and returns that.
     """
 
     solver: AbstractFixedPointSolver[Y, tuple[Y, Aux], Any]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/bfgs.py` & `optimistix-0.0.7/optimistix/_solver/bfgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, Generic, TypeVar
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
@@ -136,15 +122,17 @@
 
 
 _Hessian = TypeVar(
     "_Hessian", FunctionInfo.EvalGradHessian, FunctionInfo.EvalGradHessianInv
 )
 
 
-class _BFGSState(eqx.Module, Generic[Y, Aux, SearchState, DescentState, _Hessian]):
+class _BFGSState(
+    eqx.Module, Generic[Y, Aux, SearchState, DescentState, _Hessian], strict=True
+):
     # Updated every search step
     first_step: Bool[Array, ""]
     y_eval: Y
     search_state: SearchState
     # Updated after each descent step
     f_info: _Hessian
     aux: Aux
@@ -152,15 +140,17 @@
     # Used for termination
     terminate: Bool[Array, ""]
     result: RESULTS
     # Used in compat.py
     num_accepted_steps: Int[Array, ""]
 
 
-class AbstractBFGS(AbstractMinimiser[Y, Aux, _BFGSState], Generic[Y, Aux, _Hessian]):
+class AbstractBFGS(
+    AbstractMinimiser[Y, Aux, _BFGSState], Generic[Y, Aux, _Hessian], strict=True
+):
     """Abstract BFGS (Broyden--Fletcher--Goldfarb--Shanno) minimisation algorithm.
 
     This is a quasi-Newton optimisation algorithm, whose defining feature is the way
     it progressively builds up a Hessian approximation using multiple steps of gradient
     information.
 
     This abstract version may be subclassed to choose alternative descent and searches.
@@ -242,14 +232,17 @@
                 f_eval_info,  # pyright: ignore
                 descent_state,
             )
             f_diff = (f_eval**ω - state.f_info.f**ω).ω
             terminate = cauchy_termination(
                 self.rtol, self.atol, self.norm, state.y_eval, y_diff, f_eval, f_diff
             )
+            terminate = jnp.where(
+                state.first_step, jnp.array(False), terminate
+            )  # Skip termination on first step
             return state.y_eval, f_eval_info, aux_eval, descent_state, terminate
 
         def rejected(descent_state):
             return y, state.f_info, state.aux, descent_state, jnp.array(False)
 
         y, f_info, aux, descent_state, terminate = filter_cond(
             accept, accepted, rejected, state.descent_state
@@ -266,15 +259,15 @@
             y_eval=y_eval,
             search_state=search_state,
             f_info=f_info,
             aux=aux,
             descent_state=descent_state,
             terminate=terminate,
             result=result,
-            num_accepted_steps=state.num_accepted_steps + accept,
+            num_accepted_steps=state.num_accepted_steps + jnp.where(accept, 1, 0),
         )
         return y, state, aux
 
         def make_f_info_on_accept(f_eval, lin_fn):
             (grad,) = lin_to_grad(lin_fn, y)
             return f_info
 
@@ -299,15 +292,15 @@
         state: _BFGSState,
         tags: frozenset[object],
         result: RESULTS,
     ) -> tuple[Y, Aux, dict[str, Any]]:
         return y, aux, {}
 
 
-class BFGS(AbstractBFGS[Y, Aux, _Hessian]):
+class BFGS(AbstractBFGS[Y, Aux, _Hessian], strict=True):
     """BFGS (Broyden--Fletcher--Goldfarb--Shanno) minimisation algorithm.
 
     This is a quasi-Newton optimisation algorithm, whose defining feature is the way
     it progressively builds up a Hessian approximation using multiple steps of gradient
     information.
     """
```

### Comparing `optimistix-0.0.6/optimistix/_solver/bisection.py` & `optimistix-0.0.7/optimistix/_solver/bisection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, ClassVar, Literal, Union
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, PyTree, Scalar
 
 from .._custom_types import Aux, Fn
 from .._root_find import AbstractRootFinder
 from .._solution import RESULTS
 
 
-class _BisectionState(eqx.Module):
+class _BisectionState(eqx.Module, strict=True):
     lower: Scalar
     upper: Scalar
     flip: Bool[Array, ""]
     error: Float[Array, ""]
 
 
-class Bisection(AbstractRootFinder[Scalar, Scalar, Aux, _BisectionState]):
+class Bisection(AbstractRootFinder[Scalar, Scalar, Aux, _BisectionState], strict=True):
     """The bisection method of root finding. This may only be used with functions
     `R->R`, i.e. functions with scalar input and scalar output.
 
     This requires the following `options`:
 
     - `lower`: The lower bound on the interval which contains the root.
     - `upper`: The upper bound on the interval which contains the root.
```

### Comparing `optimistix-0.0.6/optimistix/_solver/dogleg.py` & `optimistix-0.0.7/optimistix/_solver/dogleg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, cast, Generic, Union
 
 import equinox as eqx
 import jax.lax as lax
 import jax.numpy as jnp
 import lineax as lx
@@ -35,28 +21,29 @@
 from .._search import AbstractDescent, FunctionInfo
 from .._solution import RESULTS
 from .bisection import Bisection
 from .gauss_newton import AbstractGaussNewton, newton_step
 from .trust_region import ClassicalTrustRegion
 
 
-class _DoglegDescentState(eqx.Module, Generic[Y]):
+class _DoglegDescentState(eqx.Module, Generic[Y], strict=True):
     newton: Y
     cauchy: Y
     newton_norm: Scalar
     cauchy_norm: Scalar
     result: RESULTS
 
 
 class DoglegDescent(
     AbstractDescent[
         Y,
         Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac],
         _DoglegDescentState,
-    ]
+    ],
+    strict=True,
 ):
     """The Dogleg descent step, which switches between the Cauchy and the Newton
     descent directions.
     """
 
     linear_solver: lx.AbstractLinearSolver = lx.AutoLinearSolver(well_posed=None)
     root_finder: AbstractRootFinder[Scalar, Scalar, None, Any] = Bisection(
@@ -221,26 +208,33 @@
     intersects the dogleg path. This is ignored if
     `trust_region_norm=optimistix.two_norm`, for which there is an analytic formula
     instead.
 - `trust_region_norm`: The norm used to determine the trust-region shape.
 """
 
 
-class Dogleg(AbstractGaussNewton[Y, Out, Aux]):
+class Dogleg(AbstractGaussNewton[Y, Out, Aux], strict=True):
     """Dogleg algorithm. Used for nonlinear least squares problems.
 
     Given a quadratic bowl that locally approximates the function to be minimised, then
     there are two different ways we might try to move downhill: in the steepest descent
     direction (as in gradient descent; this is also sometimes called the Cauchy
     direction), and in the direction of the minima of the quadratic bowl (as in Newton's
     method; correspondingly this is called the Newton direction).
 
     The distinguishing feature of this algorithm is the "dog leg" shape of its descent
     path, in which it begins by moving in the steepest descent direction, and then
     switches to moving in the Newton direction.
+
+    Supports the following `options`:
+
+    - `jac`: whether to use forward- or reverse-mode autodifferentiation to compute the
+        Jacobian. Can be either `"fwd"` or `"bwd"`. Defaults to `"fwd"`, which is
+        usually more efficient. Changing this can be useful when the target function has
+        a `jax.custom_vjp`, and so does not support forward-mode autodifferentiation.
     """
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: DoglegDescent[Y]
     search: ClassicalTrustRegion[Y]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/fixed_point.py` & `optimistix-0.0.7/optimistix/_solver/fixed_point.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from equinox.internal import ω
@@ -23,19 +9,21 @@
 
 from .._custom_types import Aux, Fn, Y
 from .._fixed_point import AbstractFixedPointSolver
 from .._misc import max_norm
 from .._solution import RESULTS
 
 
-class _FixedPointState(eqx.Module):
+class _FixedPointState(eqx.Module, strict=True):
     relative_error: Scalar
 
 
-class FixedPointIteration(AbstractFixedPointSolver[Y, Aux, _FixedPointState]):
+class FixedPointIteration(
+    AbstractFixedPointSolver[Y, Aux, _FixedPointState], strict=True
+):
     """Repeatedly calls a function in search of a fixed point.
 
     This is one of the simplest ways to find a fixed point `y` of `f`: simply
     repeatedly call `y_{n+1}=f(y_n)` until `y_n` stops changing.
 
     Note that this is often not a very effective method, and root-finding algorithms are
     frequently preferred in practice.
@@ -65,16 +53,17 @@
         args: PyTree,
         options: dict[str, Any],
         state: _FixedPointState,
         tags: frozenset[object],
     ) -> tuple[Y, _FixedPointState, Aux]:
         new_y, aux = fn(y, args)
         error = (y**ω - new_y**ω).ω
-        scale = (self.atol + self.rtol * ω(new_y).call(jnp.abs)).ω
-        new_state = _FixedPointState(self.norm((error**ω / scale**ω).ω))
+        with jax.numpy_dtype_promotion("standard"):
+            scale = (self.atol + self.rtol * ω(new_y).call(jnp.abs)).ω
+            new_state = _FixedPointState(self.norm((error**ω / scale**ω).ω))
         return new_y, new_state, aux
 
     def terminate(
         self,
         fn: Fn[Y, Y, Aux],
         y: Y,
         args: PyTree,
```

### Comparing `optimistix-0.0.6/optimistix/_solver/gauss_newton.py` & `optimistix-0.0.7/optimistix/_solver/gauss_newton.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
-from typing import Any, Generic, Optional, Union
+from typing import Any, Generic, Literal, Optional, Union
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import lineax as lx
 from equinox import AbstractVar
 from equinox.internal import ω
@@ -89,29 +75,30 @@
             )
         out = lx.linear_solve(operator, vector, linear_solver)
         newton = out.value
         result = RESULTS.promote(out.result)
     return newton, result
 
 
-class _NewtonDescentState(eqx.Module, Generic[Y]):
+class _NewtonDescentState(eqx.Module, Generic[Y], strict=True):
     newton: Y
     result: RESULTS
 
 
 class NewtonDescent(
     AbstractDescent[
         Y,
         Union[
             FunctionInfo.EvalGradHessian,
             FunctionInfo.EvalGradHessianInv,
             FunctionInfo.ResidualJac,
         ],
         _NewtonDescentState,
-    ]
+    ],
+    strict=True,
 ):
     """Newton descent direction.
 
     Given a quadratic bowl `x -> x^T Hess x` -- a local quadratic approximation
     to the target function -- this corresponds to moving in the direction of the bottom
     of the bowl. (Which is *not* the same as steepest descent.)
 
@@ -152,15 +139,17 @@
     will have length `step_size` with respect to this norm.) Optimistix includes three
     built-in norms: [`optimistix.max_norm`][], [`optimistix.rms_norm`][], and
     [`optimistix.two_norm`][].
 - `linear_solver`: The linear solver used to compute the Newton step.
 """
 
 
-class _GaussNewtonState(eqx.Module, Generic[Y, Out, Aux, SearchState, DescentState]):
+class _GaussNewtonState(
+    eqx.Module, Generic[Y, Out, Aux, SearchState, DescentState], strict=True
+):
     # Updated every search step
     first_step: Bool[Array, ""]
     y_eval: Y
     search_state: SearchState
     # Updated after each descent step
     f_info: FunctionInfo.ResidualJac
     aux: Aux
@@ -171,35 +160,62 @@
     # Use for verbose logging
     num_steps: Int[Array, ""]
     num_accepted_steps: Int[Array, ""]
     num_steps_since_acceptance: Int[Array, ""]
 
 
 def _make_f_info(
-    fn: Callable[[Y, Args], tuple[Any, Aux]], y: Y, args: Args, tags: frozenset
+    fn: Callable[[Y, Args], tuple[Any, Aux]],
+    y: Y,
+    args: Args,
+    tags: frozenset,
+    jac: Literal["fwd", "bwd"],
 ) -> tuple[FunctionInfo.ResidualJac, Aux]:
-    f_eval, lin_fn, aux_eval = jax.linearize(lambda _y: fn(_y, args), y, has_aux=True)
-    jac_eval = lx.FunctionLinearOperator(lin_fn, jax.eval_shape(lambda: y), tags)
+    if jac == "fwd":
+        f_eval, lin_fn, aux_eval = jax.linearize(
+            lambda _y: fn(_y, args), y, has_aux=True
+        )
+        jac_eval = lx.FunctionLinearOperator(lin_fn, jax.eval_shape(lambda: y), tags)
+    elif jac == "bwd":
+        # Materialise the Jacobian in this case.
+        def _for_jacrev(_y):
+            f_eval, aux_eval = fn(_y, args)
+            return f_eval, (f_eval, aux_eval)
+
+        jac_pytree, (f_eval, aux_eval) = jax.jacrev(_for_jacrev, has_aux=True)(y)
+        output_structure = jax.eval_shape(lambda: f_eval)
+        jac_eval = lx.PyTreeLinearOperator(jac_pytree, output_structure, tags)
+    else:
+        raise ValueError("Only `jac='fwd'` or `jac='bwd'` are valid.")
     return FunctionInfo.ResidualJac(f_eval, jac_eval), aux_eval
 
 
-class AbstractGaussNewton(AbstractLeastSquaresSolver[Y, Out, Aux, _GaussNewtonState]):
+class AbstractGaussNewton(
+    AbstractLeastSquaresSolver[Y, Out, Aux, _GaussNewtonState], strict=True
+):
     """Abstract base class for all Gauss-Newton type methods.
 
     This includes methods such as [`optimistix.GaussNewton`][],
     [`optimistix.LevenbergMarquardt`][], and [`optimistix.Dogleg`][].
 
     Subclasses must provide the following attributes, with the following types:
 
     - `rtol`: `float`
     - `atol`: `float`
     - `norm`: `Callable[[PyTree], Scalar]`
     - `descent`: `AbstractDescent`
     - `search`: `AbstractSearch`
     - `verbose`: `frozenset[str]`
+
+    Supports the following `options`:
+
+    - `jac`: whether to use forward- or reverse-mode autodifferentiation to compute the
+        Jacobian. Can be either `"fwd"` or `"bwd"`. Defaults to `"fwd"`, which is
+        usually more efficient. Changing this can be useful when the target function has
+        a `jax.custom_vjp`, and so does not support forward-mode autodifferentiation.
     """
 
     rtol: AbstractVar[float]
     atol: AbstractVar[float]
     norm: AbstractVar[Callable[[PyTree], Scalar]]
     descent: AbstractVar[AbstractDescent[Y, FunctionInfo.ResidualJac, Any]]
     search: AbstractVar[
@@ -213,15 +229,16 @@
         y: Y,
         args: PyTree,
         options: dict[str, Any],
         f_struct: PyTree[jax.ShapeDtypeStruct],
         aux_struct: PyTree[jax.ShapeDtypeStruct],
         tags: frozenset[object],
     ) -> _GaussNewtonState:
-        f_info_struct, _ = eqx.filter_eval_shape(_make_f_info, fn, y, args, tags)
+        jac = options.get("jac", "fwd")
+        f_info_struct, _ = eqx.filter_eval_shape(_make_f_info, fn, y, args, tags, jac)
         f_info = tree_full_like(f_info_struct, 0, allow_static=True)
         return _GaussNewtonState(
             first_step=jnp.array(True),
             y_eval=y,
             search_state=self.search.init(y, f_info_struct),
             f_info=f_info,
             aux=tree_full_like(aux_struct, 0),
@@ -238,15 +255,16 @@
         fn: Fn[Y, Out, Aux],
         y: Y,
         args: PyTree,
         options: dict[str, Any],
         state: _GaussNewtonState,
         tags: frozenset[object],
     ) -> tuple[Y, _GaussNewtonState, Aux]:
-        f_eval_info, aux_eval = _make_f_info(fn, state.y_eval, args, tags)
+        jac = options.get("jac", "fwd")
+        f_eval_info, aux_eval = _make_f_info(fn, state.y_eval, args, tags, jac)
         # We have a jaxpr in `f_info.jac`, which are compared by identity. Here we
         # arrange to use the same one so that downstream equality checks (e.g. in the
         # `filter_cond` below)
         dynamic = eqx.filter(f_eval_info.jac, eqx.is_array)
         static = eqx.filter(state.f_info.jac, eqx.is_array, inverse=True)
         jac = eqx.combine(dynamic, static)
         f_eval_info = eqx.tree_at(lambda f: f.jac, f_eval_info, jac)
@@ -360,19 +378,26 @@
         state: _GaussNewtonState,
         tags: frozenset[object],
         result: RESULTS,
     ) -> tuple[Y, Aux, dict[str, Any]]:
         return y, aux, {}
 
 
-class GaussNewton(AbstractGaussNewton[Y, Out, Aux]):
+class GaussNewton(AbstractGaussNewton[Y, Out, Aux], strict=True):
     """Gauss-Newton algorithm, for solving nonlinear least-squares problems.
 
     Note that regularised approaches like [`optimistix.LevenbergMarquardt`][] are
     usually preferred instead.
+
+    Supports the following `options`:
+
+    - `jac`: whether to use forward- or reverse-mode autodifferentiation to compute the
+        Jacobian. Can be either `"fwd"` or `"bwd"`. Defaults to `"fwd"`, which is
+        usually more efficient. Changing this can be useful when the target function has
+        a `jax.custom_vjp`, and so does not support forward-mode autodifferentiation.
     """
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: NewtonDescent[Y]
     search: LearningRate[Y]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/gradient_methods.py` & `optimistix-0.0.7/optimistix/_solver/gradient_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, Generic, Optional, Union
 from typing_extensions import TypeAlias
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
@@ -37,27 +23,27 @@
     AbstractSearch,
     FunctionInfo,
 )
 from .._solution import RESULTS
 from .learning_rate import LearningRate
 
 
-class _SteepestDescentState(eqx.Module, Generic[Y]):
+class _SteepestDescentState(eqx.Module, Generic[Y], strict=True):
     grad: Y
 
 
 _FnInfo: TypeAlias = Union[
     FunctionInfo.EvalGrad,
     FunctionInfo.EvalGradHessian,
     FunctionInfo.EvalGradHessianInv,
     FunctionInfo.ResidualJac,
 ]
 
 
-class SteepestDescent(AbstractDescent[Y, _FnInfo, _SteepestDescentState]):
+class SteepestDescent(AbstractDescent[Y, _FnInfo, _SteepestDescentState], strict=True):
     """The descent direction given by locally following the gradient."""
 
     norm: Optional[Callable[[PyTree], Scalar]] = None
 
     def init(self, y: Y, f_info_struct: _FnInfo) -> _SteepestDescentState:
         del f_info_struct
         # Dummy; unused
@@ -98,30 +84,32 @@
     will have length `step_size` with respect to this norm.) Optimistix includes three
     built-in norms: [`optimistix.max_norm`][], [`optimistix.rms_norm`][], and
     [`optimistix.two_norm`][].
 """
 
 
 class _GradientDescentState(
-    eqx.Module, Generic[Y, Out, Aux, SearchState, DescentState]
+    eqx.Module, Generic[Y, Out, Aux, SearchState, DescentState], strict=True
 ):
     # Updated every search step
     first_step: Bool[Array, ""]
     y_eval: Y
     search_state: SearchState
     # Updated after each descent step
     f_info: FunctionInfo.EvalGrad
     aux: Aux
     descent_state: DescentState
     # Used for termination
     terminate: Bool[Array, ""]
     result: RESULTS
 
 
-class AbstractGradientDescent(AbstractMinimiser[Y, Aux, _GradientDescentState]):
+class AbstractGradientDescent(
+    AbstractMinimiser[Y, Aux, _GradientDescentState], strict=True
+):
     """The gradient descent method for unconstrained minimisation.
 
     At every step, this algorithm performs a line search along the steepest descent
     direction. You should subclass this to provide it with a particular choice of line
     search. (E.g. [`optimistix.GradientDescent`][] uses a simple learning rate step.)
 
     Subclasses must provide the following abstract attributes, with the following types:
@@ -190,14 +178,17 @@
             f_eval_info = FunctionInfo.EvalGrad(f_eval, grad)
             descent_state = self.descent.query(state.y_eval, f_eval_info, descent_state)
             y_diff = (state.y_eval**ω - y**ω).ω
             f_diff = (f_eval**ω - state.f_info.f**ω).ω
             terminate = cauchy_termination(
                 self.rtol, self.atol, self.norm, state.y_eval, y_diff, f_eval, f_diff
             )
+            terminate = jnp.where(
+                state.first_step, jnp.array(False), terminate
+            )  # Skip termination on first step
             return state.y_eval, f_eval_info, aux_eval, descent_state, terminate
 
         def rejected(descent_state):
             return y, state.f_info, state.aux, descent_state, jnp.array(False)
 
         y, f_info, aux, descent_state, terminate = filter_cond(
             accept, accepted, rejected, state.descent_state
@@ -242,15 +233,15 @@
         state: _GradientDescentState,
         tags: frozenset[object],
         result: RESULTS,
     ) -> tuple[Y, Aux, dict[str, Any]]:
         return y, aux, {}
 
 
-class GradientDescent(AbstractGradientDescent[Y, Aux]):
+class GradientDescent(AbstractGradientDescent[Y, Aux], strict=True):
     """Classic gradient descent with a learning rate `learning_rate`."""
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: SteepestDescent[Y]
     search: LearningRate[Y]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/levenberg_marquardt.py` & `optimistix-0.0.7/optimistix/_solver/levenberg_marquardt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import cast, Generic, Union
 
 import equinox as eqx
+import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import lineax as lx
 from equinox.internal import ω
 from jaxtyping import Array, Float, PyTree, Scalar, ScalarLike
 
@@ -29,21 +16,22 @@
 from .._search import AbstractDescent, FunctionInfo
 from .._solution import RESULTS
 from .gauss_newton import AbstractGaussNewton, newton_step
 from .newton_chord import Newton
 from .trust_region import ClassicalTrustRegion
 
 
-class _Damped(eqx.Module):
+class _Damped(eqx.Module, strict=True):
     operator: lx.AbstractLinearOperator
     damping: Float[Array, ""]
 
     def __call__(self, y: PyTree[Array]):
         residual = self.operator.mv(y)
-        damped = jtu.tree_map(lambda yi: jnp.sqrt(self.damping) * yi, y)
+        with jax.numpy_dtype_promotion("standard"):
+            damped = jtu.tree_map(lambda yi: jnp.sqrt(self.damping) * yi, y)
         return residual, damped
 
 
 def damped_newton_step(
     step_size: Scalar,
     f_info: Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac],
     linear_solver: lx.AbstractLinearSolver,
@@ -84,24 +72,25 @@
             "Damped newton descent cannot be used with a solver that does not "
             "provide (approximate) Hessian information."
         )
     linear_sol = lx.linear_solve(operator, vector, linear_solver, throw=False)
     return linear_sol.value, RESULTS.promote(linear_sol.result)
 
 
-class _DampedNewtonDescentState(eqx.Module):
+class _DampedNewtonDescentState(eqx.Module, strict=True):
     f_info: Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac]
 
 
 class DampedNewtonDescent(
     AbstractDescent[
         Y,
         Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac],
         _DampedNewtonDescentState,
-    ]
+    ],
+    strict=True,
 ):
     """The damped Newton (Levenberg--Marquardt) descent.
 
     That is: gradient descent is about moving in the direction of `-grad`.
     (Quasi-)Newton descent is about moving in the direction of `-Hess^{-1} grad`. Damped
     Newton interpolates between these two regimes, by moving in the direction of
     `-(Hess + λI)^{-1} grad`.
@@ -147,27 +136,28 @@
 
 DampedNewtonDescent.__init__.__doc__ = """**Arguments:**
 
 - `linear_solver`: The linear solver used to compute the Newton step.
 """
 
 
-class _IndirectDampedNewtonDescentState(eqx.Module, Generic[Y]):
+class _IndirectDampedNewtonDescentState(eqx.Module, Generic[Y], strict=True):
     f_info: Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac]
     newton: Y
     newton_norm: Scalar
     result: RESULTS
 
 
 class IndirectDampedNewtonDescent(
     AbstractDescent[
         Y,
         Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac],
         _IndirectDampedNewtonDescentState,
-    ]
+    ],
+    strict=True,
 ):
     """The indirect damped Newton (Levenberg--Marquardt) trust-region descent.
 
     If the above line just looks like technical word soup, here's what's going on:
 
     Gradient descent is about moving in the direction of `-grad`. (Quasi-)Newton descent
     is about moving in the direction of `-Hess^{-1} grad`. Damped Newton interpolates
@@ -261,23 +251,30 @@
 - `linear_solver`: The linear solver used to compute the Newton step.
 - `root_finder`: The root finder used to find the Levenberg--Marquardt parameter which
     hits the trust-region radius.
 - `trust_region_norm`: The norm used to determine the trust-region shape.
 """
 
 
-class LevenbergMarquardt(AbstractGaussNewton[Y, Out, Aux]):
+class LevenbergMarquardt(AbstractGaussNewton[Y, Out, Aux], strict=True):
     """The Levenberg--Marquardt method.
 
     This is a classical solver for nonlinear least squares, which works by regularising
     [`optimistix.GaussNewton`][] with a damping factor. This serves to (a) interpolate
     between Gauss--Newton and steepest descent, and (b) limit step size to a local
     region around the current point.
 
     This is a good algorithm for many least squares problems.
+
+    Supports the following `options`:
+
+    - `jac`: whether to use forward- or reverse-mode autodifferentiation to compute the
+        Jacobian. Can be either `"fwd"` or `"bwd"`. Defaults to `"fwd"`, which is
+        usually more efficient. Changing this can be useful when the target function has
+        a `jax.custom_vjp`, and so does not support forward-mode autodifferentiation.
     """
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: DampedNewtonDescent[Y]
     search: ClassicalTrustRegion[Y]
@@ -312,24 +309,31 @@
 - `verbose`: Whether to print out extra information about how the solve is proceeding.
     Should be a frozenset of strings, specifying what information to print out. Valid
     entries are `step`, `loss`, `accepted`, `step_size`, `y`. For example
     `verbose=frozenset({"loss", "step_size"})`.
 """
 
 
-class IndirectLevenbergMarquardt(AbstractGaussNewton[Y, Out, Aux]):
+class IndirectLevenbergMarquardt(AbstractGaussNewton[Y, Out, Aux], strict=True):
     """The Levenberg--Marquardt method as a true trust-region method.
 
     This is a variant of [`optimistix.LevenbergMarquardt`][]. The other algorithm works
     by updating the damping factor directly -- this version instead updates a trust
     region, and then fits the damping factor to the size of the trust region.
 
     Generally speaking [`optimistix.LevenbergMarquardt`][] is preferred, as it performs
     nearly the same algorithm, without the computational overhead of an extra (scalar)
     nonlinear solve.
+
+    Supports the following `options`:
+
+    - `jac`: whether to use forward- or reverse-mode autodifferentiation to compute the
+        Jacobian. Can be either `"fwd"` or `"bwd"`. Defaults to `"fwd"`, which is
+        usually more efficient. Changing this can be useful when the target function has
+        a `jax.custom_vjp`, and so does not support forward-mode autodifferentiation.
     """
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: IndirectDampedNewtonDescent[Y]
     search: ClassicalTrustRegion[Y]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/nelder_mead.py` & `optimistix-0.0.7/optimistix/_solver/nelder_mead.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import functools as ft
 from collections.abc import Callable
 from typing import Any, cast, Generic
 
 import equinox as eqx
 import jax
 import jax.lax as lax
@@ -26,23 +12,23 @@
 
 from .._custom_types import Aux, Fn, Y
 from .._minimise import AbstractMinimiser
 from .._misc import max_norm, tree_full_like, tree_where
 from .._solution import RESULTS
 
 
-class _NMStats(eqx.Module):
+class _NMStats(eqx.Module, strict=True):
     n_reflect: Scalar
     n_inner_contract: Scalar
     n_outer_contract: Scalar
     n_expand: Scalar
     n_shrink: Scalar
 
 
-class _NelderMeadState(eqx.Module, Generic[Y, Aux]):
+class _NelderMeadState(eqx.Module, Generic[Y, Aux], strict=True):
     """
     Information to update and store the simplex of the Nelder Mead update. If
     `dim` is the dimension of the problem, we expect there to be
     `n_vertices = dim + 1` vertices. We expect the leading axis of each leaf
     to be of length `n_vertices`, and the sum of the rest of the axes of all leaves
     together to be `dim`.
 
@@ -98,15 +84,15 @@
         stats.n_inner_contract + jnp.where(inner_contract, 1, 0),
         stats.n_outer_contract + jnp.where(outer_contract, 1, 0),
         stats.n_expand + jnp.where(expand, 1, 0),
         stats.n_shrink + jnp.where(shrink, 1, 0),
     )
 
 
-class NelderMead(AbstractMinimiser[Y, Aux, _NelderMeadState[Y, Aux]]):
+class NelderMead(AbstractMinimiser[Y, Aux, _NelderMeadState[Y, Aux]], strict=True):
     """The Nelder-Mead minimisation algorithm. (Downhill simplex derivative-free
     method.)
 
     This algorithm is notable in that it only uses function evaluations, and does not
     need gradient evaluations.
 
     This is usually an "algorithm of last resort". Gradient-based algorithms are usually
@@ -251,15 +237,15 @@
                 state.aux,
             )
 
         def main_step(state):
             # TODO(raderj): Calculate the centroid and search dir based upon
             # the prior one.
             search_direction = jtu.tree_map(
-                lambda _, x, y: x[...] - y, y, state.simplex, worst
+                lambda a, b: a - b[None], state.simplex, worst
             )
             search_direction = (
                 (ω(search_direction) / (n_vertices - 1))
                 .call(ft.partial(jnp.sum, axis=0))
                 .ω
             )
             reflection = (worst**ω + reflect_const * search_direction**ω).ω
@@ -358,17 +344,17 @@
             shrink=shrink,
         )
 
         def shrink_simplex(best, new_vertex, simplex, first_pass):
             # This is just `best + shrink_const * (simplex - best)` but returns
             # a buffer. `best` is passed t
             shrink_simplex = jtu.tree_map(
-                lambda b, a: a.at[...].set(b + shrink_const * (a[...] - b)),
-                best,
+                lambda a, b: a.at[...].set(b[None] + shrink_const * (a - b[None])),
                 simplex,
+                best,
             )
             # if it is the first pass and we just wanted to use shrink_simplex to
             # compute f_simplex, return simplex
             simplex = tree_where(first_pass, simplex, shrink_simplex)
             unwrapped_simplex = jtu.tree_map(lambda _, x: x[...], y, simplex)
             f_simplex, _ = jax.vmap(lambda x: fn(x, args))(unwrapped_simplex)
             return f_simplex, simplex
@@ -431,18 +417,16 @@
         args: PyTree,
         options: dict[str, Any],
         state: _NelderMeadState[Y, Aux],
         tags: frozenset[object],
     ) -> tuple[Bool[Array, ""], RESULTS]:
         # TODO(raderj): only check terminate every k
         f_best, best, best_index = state.best
-        x_scale = (self.atol + self.rtol * ω(best).call(jnp.abs)).ω
-        x_diff = jtu.tree_map(
-            lambda _, a, b: jnp.abs(a[...] - b), best, state.simplex, best
-        )
+        x_scale = (self.atol + self.rtol * ω(best)[None].call(jnp.abs)).ω
+        x_diff = jtu.tree_map(lambda a, b: jnp.abs(a - b[None]), state.simplex, best)
         x_converged = self.norm((x_diff**ω / x_scale**ω).ω) < 1
         f_scale = (self.atol + self.rtol * ω(f_best).call(jnp.abs)).ω
         f_diff = (state.f_simplex**ω - f_best**ω).call(jnp.abs).ω
         f_converged = self.norm((f_diff**ω / f_scale**ω).ω) < 1
         #
         # minpack does a further test here where it takes for each unit vector e_i a
         # perturbation "delta" and asserts that f(x + delta e_i) > f(x) and
```

### Comparing `optimistix-0.0.6/optimistix/_solver/newton_chord.py` & `optimistix-0.0.7/optimistix/_solver/newton_chord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, Generic, Optional, TYPE_CHECKING
 
 import equinox as eqx
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
@@ -47,34 +33,36 @@
     return jnp.invert(jnp.isfinite(rate)) | (rate > 2)
 
 
 def _converged(factor: Scalar, tol: float) -> Bool[Array, " "]:
     return (factor > 0) & (factor < tol)
 
 
-class _NewtonChordState(eqx.Module, Generic[Y]):
+class _NewtonChordState(eqx.Module, Generic[Y], strict=True):
     f: PyTree[Array]
     linear_state: Optional[tuple[lx.AbstractLinearOperator, PyTree]]
     diff: Y
     diffsize: Scalar
     diffsize_prev: Scalar
     result: RESULTS
     step: Scalar
 
 
-class _NoAux(eqx.Module):
+class _NoAux(eqx.Module, strict=True):
     fn: Callable
 
     def __call__(self, y, args):
         out, aux = self.fn(y, args)
         del aux
         return out
 
 
-class _NewtonChord(AbstractRootFinder[Y, Out, Aux, _NewtonChordState[Y]]):
+class _AbstractNewtonChord(
+    AbstractRootFinder[Y, Out, Aux, _NewtonChordState[Y]], strict=True
+):
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar] = max_norm
     kappa: float = 1e-2
     linear_solver: lx.AbstractLinearSolver = lx.AutoLinearSolver(well_posed=None)
     cauchy_termination: bool = True
 
@@ -143,15 +131,16 @@
         if lower is not None:
             new_y = jtu.tree_map(lambda a, b: jnp.clip(a, a_min=b), new_y, lower)
         if upper is not None:
             new_y = jtu.tree_map(lambda a, b: jnp.clip(a, a_max=b), new_y, upper)
         if lower is not None or upper is not None:
             diff = (y**ω - new_y**ω).ω
         scale = (self.atol + self.rtol * ω(new_y).call(jnp.abs)).ω
-        diffsize = self.norm((diff**ω / scale**ω).ω)
+        with jax.numpy_dtype_promotion("standard"):
+            diffsize = self.norm((diff**ω / scale**ω).ω)
         if self.cauchy_termination:
             f_val = fx
         else:
             f_val = None
         new_state = _NewtonChordState(
             f=f_val,
             linear_state=state.linear_state,
@@ -217,15 +206,15 @@
         state: _NewtonChordState,
         tags: frozenset[object],
         result: RESULTS,
     ) -> tuple[Y, Aux, dict[str, Any]]:
         return y, aux, {}
 
 
-class Newton(_NewtonChord[Y, Out, Aux]):
+class Newton(_AbstractNewtonChord[Y, Out, Aux], strict=True):
     """Newton's method for root finding. Also sometimes known as Newton--Raphson.
 
     Unlike the SciPy implementation of Newton's method, the Optimistix version also
     works for vector-valued (or PyTree-valued) `y`.
 
     This solver optionally accepts the following `options`:
 
@@ -236,15 +225,15 @@
         PyTree of arrays each broadcastable to the corresponding element of `y`. The
         iterates of `y` will be clipped to this hypercube.
     """
 
     _is_newton = True
 
 
-class Chord(_NewtonChord[Y, Out, Aux]):
+class Chord(_AbstractNewtonChord[Y, Out, Aux], strict=True):
     """The Chord method of root finding.
 
     This is equivalent to the Newton method, except that the Jacobian is computed only
     once at the initial point `y0`, and then reused throughout the computation. This is
     a useful way to cheapen the solve, if `y0` is expected to be a good initial guess
     and the target function does not change too rapidly. (For example this is the
     standard technique used in implicit Runge--Kutta methods, when solving differential
```

### Comparing `optimistix-0.0.6/optimistix/_solver/nonlinear_cg.py` & `optimistix-0.0.7/optimistix/_solver/nonlinear_cg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, cast, Generic, Union
 
 import equinox as eqx
 import jax.numpy as jnp
 from equinox.internal import ω
 from jaxtyping import Array, PyTree, Scalar
@@ -80,30 +66,31 @@
     denominator = -tree_dot(y_diff_prev, (grad**ω - grad_prev**ω).ω)
     # Triggers at initialisation and convergence, as above.
     pred = jnp.abs(denominator) > jnp.finfo(denominator.dtype).eps
     safe_denom = jnp.where(pred, denominator, 1)
     return jnp.where(pred, numerator / safe_denom, 0)
 
 
-class _NonlinearCGDescentState(eqx.Module, Generic[Y]):
+class _NonlinearCGDescentState(eqx.Module, Generic[Y], strict=True):
     y_diff: Y
     grad: Y
 
 
 class NonlinearCGDescent(
     AbstractDescent[
         Y,
         Union[
             FunctionInfo.EvalGrad,
             FunctionInfo.EvalGradHessian,
             FunctionInfo.EvalGradHessianInv,
             FunctionInfo.ResidualJac,
         ],
         _NonlinearCGDescentState,
-    ]
+    ],
+    strict=True,
 ):
     """The nonlinear conjugate gradient step."""
 
     method: Callable[[Y, Y, Y], Scalar]
 
     def init(
         self,
@@ -179,15 +166,15 @@
     [on Wikipedia](https://en.wikipedia.org/wiki/Nonlinear_conjugate_gradient_method).
     In practice Optimistix includes four built-in methods:
     [`optimistix.polak_ribiere`][], [`optimistix.fletcher_reeves`][],
     [`optimistix.hestenes_stiefel`][], and [`optimistix.dai_yuan`][].
 """
 
 
-class NonlinearCG(AbstractGradientDescent[Y, Aux]):
+class NonlinearCG(AbstractGradientDescent[Y, Aux], strict=True):
     """The nonlinear conjugate gradient method."""
 
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar]
     descent: NonlinearCGDescent[Y]
     search: AbstractSearch[Y, FunctionInfo.EvalGrad, FunctionInfo.Eval, Any]
```

### Comparing `optimistix-0.0.6/optimistix/_solver/optax.py` & `optimistix-0.0.7/optimistix/_solver/optax.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from collections.abc import Callable
 from typing import Any, cast
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
@@ -23,22 +9,22 @@
 
 from .._custom_types import Aux, Fn, Y
 from .._minimise import AbstractMinimiser
 from .._misc import cauchy_termination, max_norm, verbose_print
 from .._solution import RESULTS
 
 
-class _OptaxState(eqx.Module):
+class _OptaxState(eqx.Module, strict=True):
     step: Int[Array, ""]
     f: Scalar
     opt_state: Any
     terminate: Bool[Array, ""]
 
 
-class OptaxMinimiser(AbstractMinimiser[Y, Aux, _OptaxState]):
+class OptaxMinimiser(AbstractMinimiser[Y, Aux, _OptaxState], strict=True):
     """A wrapper to use Optax first-order gradient-based optimisers with
     [`optimistix.minimise`][].
     """
 
     optim: "optax.GradientTransformation"  # pyright: ignore  # noqa: F821
     rtol: float
     atol: float
```

### Comparing `optimistix-0.0.6/optimistix/_solver/trust_region.py` & `optimistix-0.0.7/optimistix/_solver/trust_region.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Google LLC
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import abc
 from typing import TypeVar, Union
 from typing_extensions import TypeAlias
 
 import equinox as eqx
 import jax.numpy as jnp
 from equinox import AbstractVar
@@ -27,23 +13,25 @@
     sum_squares,
     tree_dot,
 )
 from .._search import AbstractSearch, FunctionInfo
 from .._solution import RESULTS
 
 
-class _TrustRegionState(eqx.Module):
+class _TrustRegionState(eqx.Module, strict=True):
     step_size: Scalar
 
 
 _FnInfo = TypeVar("_FnInfo", bound=FunctionInfo)
 _FnEvalInfo: TypeAlias = FunctionInfo
 
 
-class _AbstractTrustRegion(AbstractSearch[Y, _FnInfo, _FnEvalInfo, _TrustRegionState]):
+class _AbstractTrustRegion(
+    AbstractSearch[Y, _FnInfo, _FnEvalInfo, _TrustRegionState], strict=True
+):
     """The abstract base class of the trust-region update algorithm.
 
     Trust region line searches compute the ratio
     `true_reduction/predicted_reduction`, where `true_reduction` is the decrease in `fn`
     between `y` and `new_y`, and `predicted_reduction` is how much we expected the
     function to decrease using an approximation to `fn`.
 
@@ -121,15 +109,16 @@
         new_state = _TrustRegionState(step_size=new_step_size)
         return new_step_size, accept, RESULTS.successful, new_state
 
 
 class ClassicalTrustRegion(
     _AbstractTrustRegion[
         Y, Union[FunctionInfo.EvalGradHessian, FunctionInfo.ResidualJac]
-    ]
+    ],
+    strict=True,
 ):
     """The classic trust-region update algorithm which uses a quadratic approximation of
     the objective function to predict reduction.
 
     Building a quadratic approximation requires an approximation to the Hessian of the
     overall minimisation function. This means that trust region is suitable for use with
     least-squares algorithms (which make the Gauss--Newton approximation
@@ -221,15 +210,16 @@
         Y,
         Union[
             FunctionInfo.EvalGrad,
             FunctionInfo.EvalGradHessian,
             FunctionInfo.EvalGradHessianInv,
             FunctionInfo.ResidualJac,
         ],
-    ]
+    ],
+    strict=True,
 ):
     """The trust-region update algorithm which uses a linear approximation of
     the objective function to predict reduction.
 
     Generally speaking you should prefer [`optimistix.ClassicalTrustRegion`][], unless
     you happen to be using a solver (e.g. a non-quasi-Newton minimiser) with which that
     is incompatible.
```

### Comparing `optimistix-0.0.6/optimistix/compat/_impl.py` & `optimistix-0.0.7/optimistix/compat/_impl.py`

 * *Files identical despite different names*

### Comparing `optimistix-0.0.6/LICENSE` & `optimistix-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimistix-0.0.6/README.md` & `optimistix-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Features include:
 
 - interoperable solvers: e.g. autoconvert root find problems to least squares problems, then solve using a minimisation algorithm.
 - modular optimisers: e.g. use a BFGS quadratic bowl with a dogleg descent path with a trust region update.
 - using a PyTree as the state.
 - fast compilation and runtimes.
 - interoperability with [Optax](https://github.com/deepmind/optax).
-- all the benefits of working with JAX: autodiff, autoparallism, GPU/TPU support etc.
+- all the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support etc.
 
 ## Installation
 
 ```bash
 pip install optimistix
 ```
 
@@ -39,40 +39,44 @@
     return y0 + jnp.tanh(y) * dt
 
 solver = optx.Newton(rtol=1e-5, atol=1e-5)
 sol = optx.fixed_point(fn, solver, y0)
 y1 = sol.value  # satisfies y1 == fn(y1)
 ```
 
-## Finally
+## Citation
 
-### JAX ecosystem
+If you found this library to be useful in academic work, then please cite: ([arXiv link](https://arxiv.org/abs/2402.09983))
 
-[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
-
-[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
-
-[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
-
-[Diffrax](https://github.com/patrick-kidger/diffrax): numerical differential equation solvers.
-
-[Lineax](https://github.com/google/lineax): linear solvers.
-
-[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.
-
-[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).
-
-[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
-
-[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
-
-[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
+```bibtex
+@article{optimistix2024,
+    title={Optimistix: modular optimisation in JAX and Equinox},
+    author={Jason Rader and Terry Lyons and Patrick Kidger},
+    journal={arXiv:2402.09983},
+    year={2024},
+}
+```
 
-[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)
+## See also: other libraries in the JAX ecosystem
 
-### Disclaimer
+**Always useful**  
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks and everything not already in core JAX!  
+[jaxtyping](https://github.com/patrick-kidger/jaxtyping): type annotations for shape/dtype of arrays.  
+
+**Deep learning**  
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.  
+[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).  
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).  
+
+**Scientific computing**  
+[Diffrax](https://github.com/patrick-kidger/diffrax): numerical differential equation solvers.  
+[Lineax](https://github.com/patrick-kidger/lineax): linear solvers.  
+[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.  
+[sympy2jax](https://github.com/patrick-kidger/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.  
+[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)  
 
-This is not an official Google product.
+**Awesome JAX**  
+[Awesome JAX](https://github.com/n2cholas/awesome-jax): a longer list of other JAX projects.  
 
-### Credit
+## Credit
 
 Optimistix was primarily built by Jason Rader (@packquickly): [Twitter](https://twitter.com/packquickly); [GitHub](https://github.com/packquickly); [Website](https://www.packquickly.com/).
```

### Comparing `optimistix-0.0.6/pyproject.toml` & `optimistix-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "optimistix"
-version = "0.0.6"
+version = "0.0.7"
 description = "Nonlinear optimisation in JAX and Equinox."
 readme = "README.md"
 requires-python ="~=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Jason Rader", email = "raderjason@outlook.com"},
   {name = "Patrick Kidger", email = "contact@kidger.site"},
```

### Comparing `optimistix-0.0.6/PKG-INFO` & `optimistix-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: optimistix
-Version: 0.0.6
+Version: 0.0.7
 Summary: Nonlinear optimisation in JAX and Equinox.
 Project-URL: repository, https://github.com/patrick-kidger/optimistix
 Author-email: Jason Rader <raderjason@outlook.com>, Patrick Kidger <contact@kidger.site>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -233,15 +233,15 @@
 Features include:
 
 - interoperable solvers: e.g. autoconvert root find problems to least squares problems, then solve using a minimisation algorithm.
 - modular optimisers: e.g. use a BFGS quadratic bowl with a dogleg descent path with a trust region update.
 - using a PyTree as the state.
 - fast compilation and runtimes.
 - interoperability with [Optax](https://github.com/deepmind/optax).
-- all the benefits of working with JAX: autodiff, autoparallism, GPU/TPU support etc.
+- all the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support etc.
 
 ## Installation
 
 ```bash
 pip install optimistix
 ```
 
@@ -267,40 +267,44 @@
     return y0 + jnp.tanh(y) * dt
 
 solver = optx.Newton(rtol=1e-5, atol=1e-5)
 sol = optx.fixed_point(fn, solver, y0)
 y1 = sol.value  # satisfies y1 == fn(y1)
 ```
 
-## Finally
+## Citation
 
-### JAX ecosystem
+If you found this library to be useful in academic work, then please cite: ([arXiv link](https://arxiv.org/abs/2402.09983))
 
-[jaxtyping](https://github.com/google/jaxtyping): type annotations for shape/dtype of arrays.
-
-[Equinox](https://github.com/patrick-kidger/equinox): neural networks.
-
-[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.
-
-[Diffrax](https://github.com/patrick-kidger/diffrax): numerical differential equation solvers.
-
-[Lineax](https://github.com/google/lineax): linear solvers.
-
-[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.
-
-[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).
-
-[sympy2jax](https://github.com/google/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.
-
-[Eqxvision](https://github.com/paganpasta/eqxvision): computer vision models.
-
-[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).
+```bibtex
+@article{optimistix2024,
+    title={Optimistix: modular optimisation in JAX and Equinox},
+    author={Jason Rader and Terry Lyons and Patrick Kidger},
+    journal={arXiv:2402.09983},
+    year={2024},
+}
+```
 
-[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)
+## See also: other libraries in the JAX ecosystem
 
-### Disclaimer
+**Always useful**  
+[Equinox](https://github.com/patrick-kidger/equinox): neural networks and everything not already in core JAX!  
+[jaxtyping](https://github.com/patrick-kidger/jaxtyping): type annotations for shape/dtype of arrays.  
+
+**Deep learning**  
+[Optax](https://github.com/deepmind/optax): first-order gradient (SGD, Adam, ...) optimisers.  
+[Orbax](https://github.com/google/orbax): checkpointing (async/multi-host/multi-device).  
+[Levanter](https://github.com/stanford-crfm/levanter): scalable+reliable training of foundation models (e.g. LLMs).  
+
+**Scientific computing**  
+[Diffrax](https://github.com/patrick-kidger/diffrax): numerical differential equation solvers.  
+[Lineax](https://github.com/patrick-kidger/lineax): linear solvers.  
+[BlackJAX](https://github.com/blackjax-devs/blackjax): probabilistic+Bayesian sampling.  
+[sympy2jax](https://github.com/patrick-kidger/sympy2jax): SymPy<->JAX conversion; train symbolic expressions via gradient descent.  
+[PySR](https://github.com/milesCranmer/PySR): symbolic regression. (Non-JAX honourable mention!)  
 
-This is not an official Google product.
+**Awesome JAX**  
+[Awesome JAX](https://github.com/n2cholas/awesome-jax): a longer list of other JAX projects.  
 
-### Credit
+## Credit
 
 Optimistix was primarily built by Jason Rader (@packquickly): [Twitter](https://twitter.com/packquickly); [GitHub](https://github.com/packquickly); [Website](https://www.packquickly.com/).
```

