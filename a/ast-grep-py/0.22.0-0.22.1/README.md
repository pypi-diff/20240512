# Comparing `tmp/ast_grep_py-0.22.0.tar.gz` & `tmp/ast_grep_py-0.22.1.tar.gz`

## Comparing `ast_grep_py-0.22.0.tar` & `ast_grep_py-0.22.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0     1001      127      692 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    15102 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    15050 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17457 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127      682 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     8074 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5244 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     8987 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    17978 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     8432 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    19521 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5481 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    17934 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    13810 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127     3341 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    11131 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127    11870 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/config/src/transform/transformation.rs
--rw-r--r--   0     1001      127     2384 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1142 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13416 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3410 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2147 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/language/src/swift.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7731 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61561 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/Cargo.lock
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/pyproject.toml
--rw-r--r--   0     1001      127     1933 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1356 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1459 2024-05-08 19:37:37.000000 ast_grep_py-0.22.0/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.0/PKG-INFO
+-rw-r--r--   0     1001      127      682 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     8074 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5244 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     8987 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    17978 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     8432 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    19521 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5481 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    17934 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    13810 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127     3341 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    11131 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127    11870 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/config/src/transform/transformation.rs
+-rw-r--r--   0     1001      127      692 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15050 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    17457 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/core/src/traversal.rs
+-rw-r--r--   0     1001      127     2472 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1450 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/haskell.rs
+-rw-r--r--   0     1001      127     1142 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13779 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3523 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2147 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/language/src/swift.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.1/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61831 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/Cargo.lock
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.1/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.1/pyproject.toml
+-rw-r--r--   0     1001      127     1933 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1356 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1459 2024-05-12 08:14:31.000000 ast_grep_py-0.22.1/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.1/PKG-INFO
```

### Comparing `ast_grep_py-0.22.0/crates/core/Cargo.toml` & `ast_grep_py-0.22.1/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/language.rs` & `ast_grep_py-0.22.1/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/lib.rs` & `ast_grep_py-0.22.1/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/match_tree.rs` & `ast_grep_py-0.22.1/crates/core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.22.1/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.22.1/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.22.1/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/matcher/text.rs` & `ast_grep_py-0.22.1/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/matcher.rs` & `ast_grep_py-0.22.1/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/meta_var.rs` & `ast_grep_py-0.22.1/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/node.rs` & `ast_grep_py-0.22.1/crates/core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/ops.rs` & `ast_grep_py-0.22.1/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/pinned.rs` & `ast_grep_py-0.22.1/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.22.1/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.22.1/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/replacer/template.rs` & `ast_grep_py-0.22.1/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/replacer.rs` & `ast_grep_py-0.22.1/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/source.rs` & `ast_grep_py-0.22.1/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/core/src/traversal.rs` & `ast_grep_py-0.22.1/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/Cargo.toml` & `ast_grep_py-0.22.1/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/check_var.rs` & `ast_grep_py-0.22.1/crates/config/src/check_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/combined.rs` & `ast_grep_py-0.22.1/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/fixer.rs` & `ast_grep_py-0.22.1/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/lib.rs` & `ast_grep_py-0.22.1/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/maybe.rs` & `ast_grep_py-0.22.1/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.22.1/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule/mod.rs` & `ast_grep_py-0.22.1/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.22.1/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.22.1/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.22.1/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule_collection.rs` & `ast_grep_py-0.22.1/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule_config.rs` & `ast_grep_py-0.22.1/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/rule_core.rs` & `ast_grep_py-0.22.1/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/transform/mod.rs` & `ast_grep_py-0.22.1/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.22.1/crates/config/src/transform/rewrite.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.22.1/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/config/src/transform/transformation.rs` & `ast_grep_py-0.22.1/crates/config/src/transform/transformation.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/Cargo.toml` & `ast_grep_py-0.22.1/crates/language/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 tree-sitter-c = { version = "0.21.0", optional = true }
 tree-sitter-cpp = { version = "0.22.0", optional = true }
 tree-sitter-c-sharp = { version = "0.21.1", optional = true }
 tree-sitter-css = { version = "0.21.0", optional = true }
 tree-sitter-dart= { version = "0.0.4", optional = true }
 tree-sitter-elixir = { version = "0.2.0", optional = true }
 tree-sitter-go = { version = "0.21.0", optional = true }
+tree-sitter-haskell = { version = "0.21.0", optional = true }
 tree-sitter-html = { version = "0.20.3", optional = true }
 tree-sitter-java = { version = "0.21.0", optional = true }
 # https://github.com/tree-sitter/tree-sitter-javascript/issues/316
 tree-sitter-javascript = { version = "0.21.2", optional = true, package="tree-sitter-javascript-sg" }
 tree-sitter-json = { version = "0.21.0", optional = true }
 # TODO https://github.com/fwcd/tree-sitter-kotlin/issues/118
 tree-sitter-kotlin = { version = "0.3.6", optional = true }
@@ -46,22 +47,23 @@
   "tree-sitter-c",
   "tree-sitter-cpp",
   "tree-sitter-c-sharp",
   "tree-sitter-css",
   "tree-sitter-dart",
   "tree-sitter-elixir",
   "tree-sitter-go",
+  "tree-sitter-haskell",
   "tree-sitter-html",
   "tree-sitter-java",
   "tree-sitter-javascript",
   "tree-sitter-json",
   "tree-sitter-kotlin",
   "tree-sitter-lua",
   "tree-sitter-php",
   "tree-sitter-python",
   "tree-sitter-ruby",
   "tree-sitter-rust",
   "tree-sitter-scala",
   "tree-sitter-swift",
   "tree-sitter-typescript",
 ]
-default = ["builtin-parser"]
+default = ["builtin-parser"]
```

### Comparing `ast_grep_py-0.22.0/crates/language/src/bash.rs` & `ast_grep_py-0.22.1/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/cpp.rs` & `ast_grep_py-0.22.1/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/csharp.rs` & `ast_grep_py-0.22.1/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/css.rs` & `ast_grep_py-0.22.1/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/elixir.rs` & `ast_grep_py-0.22.1/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/go.rs` & `ast_grep_py-0.22.1/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/html.rs` & `ast_grep_py-0.22.1/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/json.rs` & `ast_grep_py-0.22.1/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/kotlin.rs` & `ast_grep_py-0.22.1/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/lib.rs` & `ast_grep_py-0.22.1/crates/language/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 mod bash;
 mod cpp;
 mod csharp;
 mod css;
 mod elixir;
 mod go;
+mod haskell;
 mod html;
 mod json;
 mod kotlin;
 mod lua;
 mod parsers;
 mod php;
 mod python;
@@ -105,14 +106,18 @@
 // https://www.w3.org/TR/CSS21/grammar.html#scanner
 impl_lang_expando!(Css, language_css, '_');
 // https://github.com/elixir-lang/tree-sitter-elixir/blob/a2861e88a730287a60c11ea9299c033c7d076e30/grammar.js#L245
 impl_lang_expando!(Elixir, language_elixir, 'µ');
 // we can use any Unicode code point categorized as "Letter"
 // https://go.dev/ref/spec#letter
 impl_lang_expando!(Go, language_go, 'µ');
+// GHC supports Unicode syntax per
+// https://ghc.gitlab.haskell.org/ghc/doc/users_guide/exts/unicode_syntax.html
+// and the tree-sitter-haskell grammar parses it too.
+impl_lang_expando!(Haskell, language_haskell, 'µ');
 // tree-sitter-html uses locale dependent iswalnum for tagName
 // https://github.com/tree-sitter/tree-sitter-html/blob/b5d9758e22b4d3d25704b72526670759a9e4d195/src/scanner.c#L194
 impl_lang_expando!(Html, language_html, 'z');
 // https://github.com/fwcd/tree-sitter-kotlin/pull/93
 impl_lang_expando!(Kotlin, language_kotlin, 'µ');
 // we can use any char in unicode range [:XID_Start:]
 // https://docs.python.org/3/reference/lexical_analysis.html#identifiers
@@ -148,14 +153,15 @@
   C,
   Cpp,
   CSharp,
   Css,
   Dart,
   Go,
   Elixir,
+  Haskell,
   Html,
   Java,
   JavaScript,
   Json,
   Kotlin,
   Lua,
   Php,
@@ -168,16 +174,16 @@
   TypeScript,
 }
 
 impl SupportLang {
   pub const fn all_langs() -> &'static [SupportLang] {
     use SupportLang::*;
     &[
-      Bash, C, Cpp, CSharp, Css, Dart, Elixir, Go, Html, Java, JavaScript, Json, Kotlin, Lua, Php,
-      Python, Ruby, Rust, Scala, Swift, Tsx, TypeScript,
+      Bash, C, Cpp, CSharp, Css, Dart, Elixir, Go, Haskell, Html, Java, JavaScript, Json, Kotlin,
+      Lua, Php, Python, Ruby, Rust, Scala, Swift, Tsx, TypeScript,
     ]
   }
 
   pub fn file_types(&self) -> Types {
     file_types(self)
   }
 }
@@ -221,14 +227,15 @@
     C => &["c"],
     Cpp => &["cc", "c++", "cpp", "cxx"],
     CSharp => &["cs", "csharp"],
     Css => &["css"],
     Dart => &["dart"],
     Elixir => &["ex", "elixir"],
     Go => &["go", "golang"],
+    Haskell => &["hs", "haskell"],
     Html => &["html"],
     Java => &["java"],
     JavaScript => &["javascript", "js", "jsx"],
     Json => &["json"],
     Kotlin => &["kotlin", "kt"],
     Lua => &["lua"],
     Php => &["php-exp"],
@@ -265,14 +272,15 @@
       S::C => C.$method($($pname,)*),
       S::Cpp => Cpp.$method($($pname,)*),
       S::CSharp => CSharp.$method($($pname,)*),
       S::Css => Css.$method($($pname,)*),
       S::Dart => Dart.$method($($pname,)*),
       S::Elixir => Elixir.$method($($pname,)*),
       S::Go => Go.$method($($pname,)*),
+      S::Haskell => Haskell.$method($($pname,)*),
       S::Html => Html.$method($($pname,)*),
       S::Java => Java.$method($($pname,)*),
       S::JavaScript => JavaScript.$method($($pname,)*),
       S::Json => Json.$method($($pname,)*),
       S::Kotlin => Kotlin.$method($($pname,)*),
       S::Lua => Lua.$method($($pname,)*),
       S::Php => Php.$method($($pname,)*),
@@ -320,14 +328,15 @@
     C => &["c", "h"],
     Cpp => &["cc", "hpp", "cpp", "c++", "hh", "cxx", "cu", "ino"],
     CSharp => &["cs"],
     Css => &["css", "scss"],
     Dart => &["dart"],
     Elixir => &["ex", "exs"],
     Go => &["go"],
+    Haskell => &["hs"],
     Html => &["html", "htm", "xhtml"],
     Java => &["java"],
     JavaScript => &["cjs", "js", "mjs", "jsx"],
     Json => &["json"],
     Kotlin => &["kt", "ktm", "kts"],
     Lua => &["lua"],
     Php => &["php"],
```

### Comparing `ast_grep_py-0.22.0/crates/language/src/lua.rs` & `ast_grep_py-0.22.1/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/parsers.rs` & `ast_grep_py-0.22.1/crates/language/src/parsers.rs`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,17 @@
   }
   pub fn language_elixir() -> TSLanguage {
     tree_sitter_elixir::language().into()
   }
   pub fn language_go() -> TSLanguage {
     tree_sitter_go::language().into()
   }
+  pub fn language_haskell() -> TSLanguage {
+    tree_sitter_haskell::language().into()
+  }
   pub fn language_html() -> TSLanguage {
     tree_sitter_html::language().into()
   }
   pub fn language_java() -> TSLanguage {
     tree_sitter_java::language().into()
   }
   pub fn language_javascript() -> TSLanguage {
@@ -100,14 +103,15 @@
     language_c,
     language_cpp,
     language_c_sharp,
     language_css,
     language_dart,
     language_elixir,
     language_go,
+    language_haskell,
     language_html,
     language_java,
     language_javascript,
     language_json,
     language_kotlin,
     language_lua,
     language_php,
```

### Comparing `ast_grep_py-0.22.0/crates/language/src/python.rs` & `ast_grep_py-0.22.1/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/ruby.rs` & `ast_grep_py-0.22.1/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/rust.rs` & `ast_grep_py-0.22.1/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/scala.rs` & `ast_grep_py-0.22.1/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/language/src/swift.rs` & `ast_grep_py-0.22.1/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/Cargo.toml` & `ast_grep_py-0.22.1/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/README.md` & `ast_grep_py-0.22.1/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.22.1/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.1/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/src/lib.rs` & `ast_grep_py-0.22.1/crates/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.22.1/crates/pyo3/src/py_node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/src/range.rs` & `ast_grep_py-0.22.1/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.22.1/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.22.1/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.22.1/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.22.1/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.22.1/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/Cargo.lock` & `ast_grep_py-0.22.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -140,15 +140,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -156,50 +156,51 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
  "tree-sitter-cpp",
  "tree-sitter-css",
  "tree-sitter-dart",
  "tree-sitter-elixir",
  "tree-sitter-go",
+ "tree-sitter-haskell",
  "tree-sitter-html",
  "tree-sitter-java",
  "tree-sitter-javascript-sg",
  "tree-sitter-json",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-php",
@@ -209,29 +210,29 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -241,15 +242,15 @@
  "tree-sitter-html",
  "tree-sitter-javascript-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
@@ -307,15 +308,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.22.0"
+version = "0.22.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -1873,17 +1874,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d463580f35b642e3073d163c9ba84f5212bfde538e5c06c40a085b3d560190ea"
+checksum = "b4f0e5c383fd633a792eb8878367dc9d4a3c0e788bad5dcc84c200332ed1b8f2"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c-sharp"
@@ -1933,17 +1934,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-facade-sg"
-version = "0.21.3"
+version = "0.21.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d56b01a682080bbfb3cc9cc52550929b936f1838b22870a82ad34aafb1010991"
+checksum = "e7ca50a891218430da4837d9f411b365b83ce6a22c28f8d99933bcc5bc18cd0c"
 dependencies = [
  "js-sys",
  "tree-sitter",
  "wasm-bindgen",
  "web-sys",
  "web-tree-sitter-sg",
 ]
@@ -1955,14 +1956,24 @@
 checksum = "55cb318be5ccf75f44e054acf6898a5c95d59b53443eed578e16be0cd7ec037f"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-haskell"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef25a7e6c73cc1cbe0c0b7dbd5406e7b3485b370bd61c5d8d852ae0781f9bf9a"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-html"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95b3492b08a786bf5cc79feb0ef2ff3b115d5174364e0ddfd7860e0b9b088b53"
 dependencies = [
  "cc",
  "tree-sitter",
```

### Comparing `ast_grep_py-0.22.0/Cargo.toml` & `ast_grep_py-0.22.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.22.0"
+version = "0.22.1"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.22.0" }
-ast-grep-config = { path = "crates/config", version = "0.22.0" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.0" }
-ast-grep-language = { path = "crates/language", version = "0.22.0" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.22.0" }
+ast-grep-core = { path = "crates/core", version = "0.22.1" }
+ast-grep-config = { path = "crates/config", version = "0.22.1" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.1" }
+ast-grep-language = { path = "crates/language", version = "0.22.1" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.22.1" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0.200", features = ["derive"] }
-tree-sitter = { version = "0.21.3", package = "tree-sitter-facade-sg" }
+tree-sitter = { version = "0.21.4", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
 schemars = "0.8.17"
 anyhow = "1.0.82"
```

### Comparing `ast_grep_py-0.22.0/pyproject.toml` & `ast_grep_py-0.22.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.22.0"
+version = "0.22.1"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.22.0/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.1/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/ast_grep_py/__init__.py` & `ast_grep_py-0.22.1/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/README.md` & `ast_grep_py-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.0/PKG-INFO` & `ast_grep_py-0.22.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.22.0
+Version: 0.22.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

