# Comparing `tmp/profitpulse-2.1.0.tar.gz` & `tmp/profitpulse-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-2.1.0.tar", max compression
+gzip compressed data, was "profitpulse-2.2.0.tar", max compression
```

## Comparing `profitpulse-2.1.0.tar` & `profitpulse-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.1.0/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.1.0/README.md
--rw-r--r--   0        0        0     1839 2024-05-12 17:07:09.108938 profitpulse-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.1.0/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.1.0/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     7916 2024-05-12 17:04:21.962848 profitpulse-2.1.0/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     4760 2024-05-12 17:04:21.963423 profitpulse-2.1.0/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.1.0/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     4533 2024-05-10 06:54:12.882781 profitpulse-2.1.0/src/profitpulse/data/assets.py
--rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.1.0/src/profitpulse/data/assets_test.py
--rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.1.0/src/profitpulse/data/data.py
--rw-r--r--   0        0        0      973 2024-05-12 17:04:21.963783 profitpulse-2.1.0/src/profitpulse/data/expenses_view.py
--rw-r--r--   0        0        0     2169 2024-05-12 17:04:21.964117 profitpulse-2.1.0/src/profitpulse/data/expenses_view_test.py
--rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.1.0/src/profitpulse/data/pulse_view.py
--rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.1.0/src/profitpulse/data/pulse_view_test.py
--rw-r--r--   0        0        0     1628 2024-05-12 17:04:21.964654 profitpulse-2.1.0/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     1033 2024-05-12 17:04:21.965124 profitpulse-2.1.0/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.1.0/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.1.0/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.1.0/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.1.0/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.1.0/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.1.0/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.1.0/src/profitpulse/lib/asset.py
--rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.1.0/src/profitpulse/lib/asset_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.1.0/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.1.0/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.1.0/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-2.1.0/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.1.0/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.1.0/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.1.0/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.1.0/src/profitpulse/services/acquire_asset.py
--rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.1.0/src/profitpulse/services/acquire_asset_test.py
--rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.1.0/src/profitpulse/services/delete_asset.py
--rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.1.0/src/profitpulse/services/delete_asset_test.py
--rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset.py
--rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset_test.py
--rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.1.0/src/profitpulse/services/divest_asset.py
--rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.1.0/src/profitpulse/services/divest_asset_test.py
--rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.1.0/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     1812 2024-05-12 17:04:21.965884 profitpulse-2.1.0/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.1.0/src/profitpulse/services/revalue_asset.py
--rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.1.0/src/profitpulse/services/revalue_test.py
--rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.1.0/src/profitpulse/services/services.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.1.0/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.1.0/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.1.0/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4658 2024-05-12 17:04:21.966863 profitpulse-2.1.0/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.1.0/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.2.0/README.md
+-rw-r--r--   0        0        0     1839 2024-05-12 19:40:15.676088 profitpulse-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.2.0/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.2.0/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     8195 2024-05-12 19:23:02.361097 profitpulse-2.2.0/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     4941 2024-05-12 19:25:34.206898 profitpulse-2.2.0/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.2.0/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     4533 2024-05-12 18:13:22.497175 profitpulse-2.2.0/src/profitpulse/data/assets.py
+-rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.2.0/src/profitpulse/data/assets_test.py
+-rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.2.0/src/profitpulse/data/data.py
+-rw-r--r--   0        0        0     1852 2024-05-12 19:36:31.054109 profitpulse-2.2.0/src/profitpulse/data/expenses_view.py
+-rw-r--r--   0        0        0     3191 2024-05-12 19:25:34.189395 profitpulse-2.2.0/src/profitpulse/data/expenses_view_test.py
+-rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.2.0/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.2.0/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0     1628 2024-05-12 17:04:21.964654 profitpulse-2.2.0/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     1033 2024-05-12 17:04:21.965124 profitpulse-2.2.0/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.2.0/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.2.0/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.2.0/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.2.0/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.2.0/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.2.0/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.2.0/src/profitpulse/lib/asset.py
+-rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.2.0/src/profitpulse/lib/asset_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.2.0/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.2.0/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.2.0/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      956 2024-05-12 18:30:01.306766 profitpulse-2.2.0/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.2.0/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.2.0/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.2.0/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.2.0/src/profitpulse/services/acquire_asset.py
+-rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.2.0/src/profitpulse/services/acquire_asset_test.py
+-rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.2.0/src/profitpulse/services/delete_asset.py
+-rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.2.0/src/profitpulse/services/delete_asset_test.py
+-rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset.py
+-rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset_test.py
+-rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.2.0/src/profitpulse/services/divest_asset.py
+-rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.2.0/src/profitpulse/services/divest_asset_test.py
+-rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.2.0/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     1446 2024-05-12 18:43:49.634734 profitpulse-2.2.0/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.2.0/src/profitpulse/services/revalue_asset.py
+-rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.2.0/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.2.0/src/profitpulse/services/services.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.2.0/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.2.0/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.2.0/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4652 2024-05-12 19:25:34.212907 profitpulse-2.2.0/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.2.0/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.2.0/PKG-INFO
```

### Comparing `profitpulse-2.1.0/LICENSE` & `profitpulse-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/README.md` & `profitpulse-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/pyproject.toml` & `profitpulse-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "2.1.0"
+version = "2.2.0"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
```

### Comparing `profitpulse-2.1.0/src/profitpulse/cli/adapters.py` & `profitpulse-2.2.0/src/profitpulse/cli/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,40 @@
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
 database_path = Path.home() / Path("Library/Application Support/Profitpulse")
 
 
 def report(
-    seller: Optional[str],
+    seller: Optional[str] = None,
+    group_seller: Optional[bool] = False,
 ) -> None:
     """
     Shows a report of all transactions in all assets given the provided
      parameters:
      - seller: The provider or recipient of the value
      - since: The data from which the transactions should be shown
      - on: A specific date for which transactions should be shown
     """
 
     db = Database(database_path)
     with Session(db.engine) as session:
 
-        view = ExpensesView(session, seller)
+        view = ExpensesView(session, seller=seller, group_seller=group_seller)
         data = view.data
 
+        table_data = []
+        for item in data:
+            d = item
+            d[0] = f"{int(item[0]) / 100:.2f}"
+            table_data.append(d)
+
         headers = ["Value", "Description", "Date"]
+        if group_seller:
+            headers = ["Value", "Description"]
         for line in gogotable(headers, data):
             print(line)
 
 
 def pulse() -> None:
     """
     Shows the current wealth status.
@@ -120,17 +129,17 @@
     """
     Imports a file with all the transactions for a specific asset.
     """
     db = Database(database_path)
     with Session(db.engine) as session:
         gateway_cgd = GatewayCGDFile(file_path)
 
-        assets = Assets(session)
         service = ImportTransactionsService(
-            gateway_cgd, assets, event_log=pastperfect.Events(session)
+            gateway_cgd,
+            event_log=pastperfect.Events(session),
         )
         service.execute()
         session.commit()
 
 
 class DepositRequest(DepositIntoAssetRequester):
     def __init__(
```

### Comparing `profitpulse-2.1.0/src/profitpulse/cli/main.py` & `profitpulse-2.2.0/src/profitpulse/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,20 @@
 
 
 @profitpulse_app.command(name="report", help="Builds reports according to filter")
 def report_(
     seller: Optional[str] = typer.Option(
         default="", help="Filters report by Seller in description"
     ),
+    group_seller: Optional[bool] = typer.Option(  # "--group-seller",
+        default=False, help="Groups report by the Seller description"
+    ),
 ) -> None:
     migrate_database(database_path)
-    report(seller)
+    report(seller=seller, group_seller=group_seller)
 
 
 @profitpulse_app.command(name="reset", help="Deletes all information in profitpulse")
 def reset_() -> None:
     delete_information = typer.confirm(
         "Are you sure you want to delete all financial information ?"
     )
```

### Comparing `profitpulse-2.1.0/src/profitpulse/data/assets.py` & `profitpulse-2.2.0/src/profitpulse/data/assets.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/data/assets_test.py` & `profitpulse-2.2.0/src/profitpulse/data/assets_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/data/expenses_view.py` & `profitpulse-2.2.0/src/profitpulse/data/expenses_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,36 +4,69 @@
 import pastperfect
 
 from profitpulse.data.data import View
 from profitpulse.services.import_transactions import EXPENSE_MADE
 
 
 class ExpensesView(View):
-    def __init__(self, session: typing.Any, seller: typing.Optional[str] = None):
+    def __init__(
+        self,
+        session: typing.Any,
+        seller: typing.Optional[str] = None,
+        group_seller: typing.Optional[bool] = False,
+    ):
         self._session = session
         self._seller = seller
+        self._group_seller = group_seller
 
     @property
-    def data(self) -> Any:
+    def data(self) -> Any:  # noqa
         events = pastperfect.Events(self._session)
         if not len(events):
             return []
 
+        seller_value = {}
         results = []
-        for event in events:
-            if event.name != EXPENSE_MADE:
-                continue
 
-            description = event.data.get("description")
+        def get_expenses_by_seller(evt: pastperfect.Event):
+            nonlocal seller_value
 
-            if self._seller and self._seller not in description:
-                continue
+            if evt.name != EXPENSE_MADE:
+                return
+
+            d = evt.data.get("description")
+            if self._seller and self._seller not in d:
+                return
+
+            try:
+                seller_value[d] = seller_value[d] + evt.data.get("value")
+            except KeyError:
+                seller_value[d] = evt.data.get("value")
+
+        def get_expenses(evt: pastperfect.Event):
+            nonlocal results
+            if evt.name != EXPENSE_MADE:
+                return
+
+            d = evt.data.get("description")
+
+            if self._seller and self._seller not in d:
+                return
 
             results.append(
                 [
-                    event.data.get("value"),
-                    description,
-                    event.data.get("date_of"),
+                    evt.data.get("value"),
+                    d,
+                    evt.data.get("date_of"),
                 ]
             )
 
+        handler = get_expenses
+        if self._group_seller:
+            handler = get_expenses_by_seller
+
+        events.replay([handler])
+
+        if self._group_seller:
+            results = [[value, key] for key, value in seller_value.items()]
+
         return results
```

### Comparing `profitpulse-2.1.0/src/profitpulse/data/pulse_view.py` & `profitpulse-2.2.0/src/profitpulse/data/pulse_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/data/pulse_view_test.py` & `profitpulse-2.2.0/src/profitpulse/data/pulse_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/data/views.py` & `profitpulse-2.2.0/src/profitpulse/data/views.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/data/views_test.py` & `profitpulse-2.2.0/src/profitpulse/data/views_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/gateways/cgdfile.py` & `profitpulse-2.2.0/src/profitpulse/gateways/cgdfile.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-2.2.0/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/infrastructure/migrations.py` & `profitpulse-2.2.0/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/lib/asset.py` & `profitpulse-2.2.0/src/profitpulse/lib/asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/lib/asset_name.py` & `profitpulse-2.2.0/src/profitpulse/lib/asset_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/lib/money.py` & `profitpulse-2.2.0/src/profitpulse/lib/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-2.2.0/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 
 CREATE TABLE IF NOT EXISTS event (
     id INTEGER PRIMARY KEY,
     name VARCHAR(30) NOT NULL,
     data JSON NOT NULL,
     created_at DATETIME NOT NULL,
     UNIQUE(name, data, created_at)
-);
+);
+
```

### Comparing `profitpulse-2.1.0/src/profitpulse/services/acquire_asset.py` & `profitpulse-2.2.0/src/profitpulse/services/acquire_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/acquire_asset_test.py` & `profitpulse-2.2.0/src/profitpulse/services/acquire_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/delete_asset.py` & `profitpulse-2.2.0/src/profitpulse/services/delete_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/delete_asset_test.py` & `profitpulse-2.2.0/src/profitpulse/services/delete_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset.py` & `profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset_test.py` & `profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/divest_asset.py` & `profitpulse-2.2.0/src/profitpulse/services/divest_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/divest_asset_test.py` & `profitpulse-2.2.0/src/profitpulse/services/divest_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/import_transactions.py` & `profitpulse-2.2.0/src/profitpulse/services/import_transactions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 import abc
 import typing
 
 from profitpulse.lib.asset import Asset
 from profitpulse.lib.asset_name import AssetName
-from profitpulse.lib.transaction import Transaction
+from profitpulse.lib.money import Money
 from profitpulse.services.services import EventEmitterMixin, EventLogger
 
 
 class ImportTransactionsTransactionGater(abc.ABC):
     def __iter__(self) -> None:
         pass  # pragma: no cover
 
 
-class ImportTransactionsTransactionCollector(abc.ABC):
-    @abc.abstractmethod
-    def append(self, transaction: Transaction, asset_name: AssetName) -> None:
-        pass  # pragma: no cover
-
-
-class ImportTransactionsRequester(abc.ABC):
-    @property
-    @abc.abstractmethod
-    def asset_name(self) -> AssetName: ...  # pragma: no cover
-
-
 class ImportTransactionsAssetCollector(abc.ABC):
     @abc.abstractmethod
     def __getitem__(self, asset_name: AssetName) -> Asset: ...  # pragma: no cover
 
 
 EXPENSE_MADE = "expense_made"
 
@@ -36,27 +24,27 @@
     """
     Imports transactions from a source.
     """
 
     def __init__(
         self,
         transactions_gateway: ImportTransactionsTransactionGater,
-        assets: ImportTransactionsAssetCollector,
         event_log: EventLogger,
         *_: typing.Any,
         **__: typing.Dict[typing.Any, typing.Any],
     ) -> None:
         self.transactions = transactions_gateway
-        self._assets = assets
 
         super().__init__(EXPENSE_MADE, event_log)
 
     def execute(self) -> None:
         for transaction in self.transactions:  # type: ignore
             if transaction.value > 0:
                 continue  # Ignore income
 
+            value = Money(int(str(transaction.value).replace(".", "")))
+
             self.emit(
-                value=transaction.value,  # type: ignore
+                value=int(value),  # type: ignore
                 date_of=str(transaction.date_of_movement),  # type: ignore
                 description=transaction.description,  # type: ignore
             )
```

### Comparing `profitpulse-2.1.0/src/profitpulse/services/revalue_asset.py` & `profitpulse-2.2.0/src/profitpulse/services/revalue_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/revalue_test.py` & `profitpulse-2.2.0/src/profitpulse/services/revalue_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/services/services.py` & `profitpulse-2.2.0/src/profitpulse/services/services.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/testrig/fixtures.py` & `profitpulse-2.2.0/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.1.0/src/profitpulse/testrig/scenario.py` & `profitpulse-2.2.0/src/profitpulse/testrig/scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,23 +105,24 @@
         result = runner.invoke(self._app, ["pulse"], catch_exceptions=False)
 
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     # I don't remember what these are .... facepalm --------------------------------------------------------------------
 
-    def report(self, seller: Optional[str] = None, month: Optional[int] = None):
+    def report(
+        self, seller: Optional[str] = None, group_seller: Optional[bool] = False
+    ):
         cmd = ["report"]
         if seller:
             cmd.append("--seller")
             cmd.append(seller)
 
-        if month:
-            cmd.append("--since")
-            cmd.append(f"2023-{month}-01")
+        if group_seller:
+            cmd.append("--group-seller")
 
         result = runner.invoke(self._app, cmd, catch_exceptions=False)
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     @property
     def current_month(self) -> str:
```

### Comparing `profitpulse-2.1.0/PKG-INFO` & `profitpulse-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 2.1.0
+Version: 2.2.0
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
```

