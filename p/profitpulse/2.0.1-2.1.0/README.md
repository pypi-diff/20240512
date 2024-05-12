# Comparing `tmp/profitpulse-2.0.1.tar.gz` & `tmp/profitpulse-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-2.0.1.tar", max compression
+gzip compressed data, was "profitpulse-2.1.0.tar", max compression
```

## Comparing `profitpulse-2.0.1.tar` & `profitpulse-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.0.1/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.0.1/README.md
--rw-r--r--   0        0        0     1839 2024-05-10 13:11:08.315336 profitpulse-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.0.1/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.0.1/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     8599 2024-05-10 12:45:52.656122 profitpulse-2.0.1/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     5122 2024-05-10 11:11:53.203489 profitpulse-2.0.1/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.0.1/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     4533 2024-05-10 06:54:12.882781 profitpulse-2.0.1/src/profitpulse/data/assets.py
--rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.0.1/src/profitpulse/data/assets_test.py
--rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.0.1/src/profitpulse/data/data.py
--rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.0.1/src/profitpulse/data/pulse_view.py
--rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.0.1/src/profitpulse/data/pulse_view_test.py
--rw-r--r--   0        0        0     1951 2024-05-10 06:54:12.886478 profitpulse-2.0.1/src/profitpulse/data/transactions.py
--rw-r--r--   0        0        0     4715 2024-05-10 06:54:12.887002 profitpulse-2.0.1/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     6779 2024-05-10 06:54:12.887503 profitpulse-2.0.1/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.0.1/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.0.1/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.0.1/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.0.1/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.0.1/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.0.1/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.0.1/src/profitpulse/lib/asset.py
--rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.0.1/src/profitpulse/lib/asset_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.0.1/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.0.1/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.0.1/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-2.0.1/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.0.1/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.0.1/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.0.1/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.0.1/src/profitpulse/services/acquire_asset.py
--rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.0.1/src/profitpulse/services/acquire_asset_test.py
--rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.0.1/src/profitpulse/services/delete_asset.py
--rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.0.1/src/profitpulse/services/delete_asset_test.py
--rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.0.1/src/profitpulse/services/deposit_into_asset.py
--rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.0.1/src/profitpulse/services/deposit_into_asset_test.py
--rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.0.1/src/profitpulse/services/divest_asset.py
--rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.0.1/src/profitpulse/services/divest_asset_test.py
--rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.0.1/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     2091 2024-05-10 06:54:12.895866 profitpulse-2.0.1/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     1967 2024-05-10 06:54:12.896440 profitpulse-2.0.1/src/profitpulse/services/import_transactions_test.py
--rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.0.1/src/profitpulse/services/revalue_asset.py
--rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.0.1/src/profitpulse/services/revalue_test.py
--rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.0.1/src/profitpulse/services/services.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.0.1/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.0.1/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.0.1/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4687 2024-05-08 17:37:21.761504 profitpulse-2.0.1/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.0.1/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.1.0/README.md
+-rw-r--r--   0        0        0     1839 2024-05-12 17:07:09.108938 profitpulse-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.1.0/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.1.0/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     7916 2024-05-12 17:04:21.962848 profitpulse-2.1.0/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     4760 2024-05-12 17:04:21.963423 profitpulse-2.1.0/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.1.0/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     4533 2024-05-10 06:54:12.882781 profitpulse-2.1.0/src/profitpulse/data/assets.py
+-rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.1.0/src/profitpulse/data/assets_test.py
+-rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.1.0/src/profitpulse/data/data.py
+-rw-r--r--   0        0        0      973 2024-05-12 17:04:21.963783 profitpulse-2.1.0/src/profitpulse/data/expenses_view.py
+-rw-r--r--   0        0        0     2169 2024-05-12 17:04:21.964117 profitpulse-2.1.0/src/profitpulse/data/expenses_view_test.py
+-rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.1.0/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.1.0/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0     1628 2024-05-12 17:04:21.964654 profitpulse-2.1.0/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     1033 2024-05-12 17:04:21.965124 profitpulse-2.1.0/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.1.0/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.1.0/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.1.0/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.1.0/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.1.0/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.1.0/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.1.0/src/profitpulse/lib/asset.py
+-rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.1.0/src/profitpulse/lib/asset_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.1.0/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.1.0/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.1.0/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-2.1.0/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.1.0/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.1.0/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.1.0/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.1.0/src/profitpulse/services/acquire_asset.py
+-rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.1.0/src/profitpulse/services/acquire_asset_test.py
+-rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.1.0/src/profitpulse/services/delete_asset.py
+-rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.1.0/src/profitpulse/services/delete_asset_test.py
+-rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset.py
+-rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset_test.py
+-rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.1.0/src/profitpulse/services/divest_asset.py
+-rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.1.0/src/profitpulse/services/divest_asset_test.py
+-rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.1.0/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     1812 2024-05-12 17:04:21.965884 profitpulse-2.1.0/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.1.0/src/profitpulse/services/revalue_asset.py
+-rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.1.0/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.1.0/src/profitpulse/services/services.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.1.0/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.1.0/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.1.0/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4658 2024-05-12 17:04:21.966863 profitpulse-2.1.0/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.1.0/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.1.0/PKG-INFO
```

### Comparing `profitpulse-2.0.1/LICENSE` & `profitpulse-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/README.md` & `profitpulse-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/pyproject.toml` & `profitpulse-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "2.0.1"
+version = "2.1.0"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
```

### Comparing `profitpulse-2.0.1/src/profitpulse/cli/adapters.py` & `profitpulse-2.1.0/src/profitpulse/cli/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Adapters bridge the CLI frameworks and the application services by creating the
 service inputs and handling the output for printing.
 """
 
 import logging
-from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 import pastperfect
 from gogotable import gogotable
 from turbofan.database import Database, Session
 
 from profitpulse.data.assets import Assets
+from profitpulse.data.expenses_view import ExpensesView
 from profitpulse.data.pulse_view import PulseView
-from profitpulse.data.transactions import Transactions
-from profitpulse.data.views import AssetsView, TransactionsView
+from profitpulse.data.views import AssetsView
 from profitpulse.gateways.cgdfile import GatewayCGDFile  # type: ignore
 from profitpulse.lib.asset_name import AssetName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
 from profitpulse.services.acquire_asset import (
     AcquireAssetService,
     AssetAlreadyExistsError,
@@ -27,53 +26,46 @@
 )
 from profitpulse.services.delete_asset import DeleteAssetRequester, DeleteAssetService
 from profitpulse.services.deposit_into_asset import (
     DepositIntoAssetRequester,
     DepositIntoAssetService,
 )
 from profitpulse.services.divest_asset import DivestAssetRequester, DivestAssetService
-from profitpulse.services.import_transactions import (
-    ImportTransactionsRequester,
-    ImportTransactionsService,
-)
+from profitpulse.services.import_transactions import ImportTransactionsService
 from profitpulse.services.revalue_asset import (
     RevalueAssetRequester,
     RevalueAssetService,
 )
 
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
 database_path = Path.home() / Path("Library/Application Support/Profitpulse")
 
 
 def report(
     seller: Optional[str],
-    since: Optional[datetime] = None,
-    on: Optional[datetime] = None,
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
-        view = TransactionsView(session, seller, since, on)
 
-        transactions, total = view.data
-        if seller:
-            print(f"Description: '{seller}', Value: {round(total, 2)}")
-            return
+        view = ExpensesView(session, seller)
+        data = view.data
 
-        for t in transactions:
-            print(f"Description: '{t['description']:>22}', Value: {t['value']:>10}")
+        headers = ["Value", "Description", "Date"]
+        for line in gogotable(headers, data):
+            print(line)
 
 
 def pulse() -> None:
     """
     Shows the current wealth status.
     """
 
@@ -120,37 +112,27 @@
     """
     Resets the application by removing the database.
     """
     db = Database(database_path)
     db.remove()
 
 
-class RequestImportTransactions(ImportTransactionsRequester):
-    def __init__(self, asset_name: str) -> None:
-        self._asset_name = asset_name
-
-    @property
-    def asset_name(self) -> AssetName:
-        return AssetName(self._asset_name)
-
-
-def import_file(file_path: Path, asset_name: str) -> None:
+def import_file(file_path: Path) -> None:
     """
     Imports a file with all the transactions for a specific asset.
     """
     db = Database(database_path)
     with Session(db.engine) as session:
         gateway_cgd = GatewayCGDFile(file_path)
-        transactions = Transactions(session)
+
         assets = Assets(session)
         service = ImportTransactionsService(
-            gateway_cgd, transactions, assets, event_log=pastperfect.Events(session)
+            gateway_cgd, assets, event_log=pastperfect.Events(session)
         )
-        request = RequestImportTransactions(asset_name)
-        service.execute(request)
+        service.execute()
         session.commit()
 
 
 class DepositRequest(DepositIntoAssetRequester):
     def __init__(
         self, cent_amount: int, asset_name: str, comment: Optional[str] = None
     ) -> None:
```

### Comparing `profitpulse-2.0.1/src/profitpulse/cli/main.py` & `profitpulse-2.1.0/src/profitpulse/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 CLI entry points for Typer (https://typer.tiangolo.com/) made CLI.
 """
 
-from datetime import datetime
 from importlib.metadata import version as get_version
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from profitpulse.cli.adapters import (  # delete_asset,; show_assets,; transfer,
@@ -59,36 +58,27 @@
     ),
 ) -> None:
     migrate_database(database_path)
     revalue(cent_amount, asset_name)
 
 
 @profitpulse_app.command(name="import", help="Import transactions for expense tracking")
-def import_(
-    file_path: Path,
-    asset_name: str = typer.Argument(
-        "", help="Name of the asset", metavar='"ASSET NAME"'
-    ),
-) -> None:
+def import_(file_path: Path) -> None:
     migrate_database(database_path)
-    import_file(file_path, asset_name)
+    import_file(file_path)
 
 
-@profitpulse_app.command(name="report", help="Builds reports according to filters")
+@profitpulse_app.command(name="report", help="Builds reports according to filter")
 def report_(
-    seller: Optional[str] = typer.Option(default="", help="Filters report by Seller"),
-    since: Optional[datetime] = typer.Option(
-        default=None, help="Show report since specified date"
-    ),
-    on: Optional[datetime] = typer.Option(
-        default=None, help="Show report on specified date"
+    seller: Optional[str] = typer.Option(
+        default="", help="Filters report by Seller in description"
     ),
 ) -> None:
     migrate_database(database_path)
-    report(seller, since, on)
+    report(seller)
 
 
 @profitpulse_app.command(name="reset", help="Deletes all information in profitpulse")
 def reset_() -> None:
     delete_information = typer.confirm(
         "Are you sure you want to delete all financial information ?"
     )
```

### Comparing `profitpulse-2.0.1/src/profitpulse/data/assets.py` & `profitpulse-2.1.0/src/profitpulse/data/assets.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/data/assets_test.py` & `profitpulse-2.1.0/src/profitpulse/data/assets_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/data/pulse_view.py` & `profitpulse-2.1.0/src/profitpulse/data/pulse_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/data/pulse_view_test.py` & `profitpulse-2.1.0/src/profitpulse/data/pulse_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/gateways/cgdfile.py` & `profitpulse-2.1.0/src/profitpulse/gateways/cgdfile.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-2.1.0/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/infrastructure/migrations.py` & `profitpulse-2.1.0/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/lib/asset.py` & `profitpulse-2.1.0/src/profitpulse/lib/asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/lib/asset_name.py` & `profitpulse-2.1.0/src/profitpulse/lib/asset_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/lib/money.py` & `profitpulse-2.1.0/src/profitpulse/lib/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-2.1.0/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/acquire_asset.py` & `profitpulse-2.1.0/src/profitpulse/services/acquire_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/acquire_asset_test.py` & `profitpulse-2.1.0/src/profitpulse/services/acquire_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/delete_asset.py` & `profitpulse-2.1.0/src/profitpulse/services/delete_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/delete_asset_test.py` & `profitpulse-2.1.0/src/profitpulse/services/delete_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/deposit_into_asset.py` & `profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/deposit_into_asset_test.py` & `profitpulse-2.1.0/src/profitpulse/services/deposit_into_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/divest_asset.py` & `profitpulse-2.1.0/src/profitpulse/services/divest_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/divest_asset_test.py` & `profitpulse-2.1.0/src/profitpulse/services/divest_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/revalue_asset.py` & `profitpulse-2.1.0/src/profitpulse/services/revalue_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/revalue_test.py` & `profitpulse-2.1.0/src/profitpulse/services/revalue_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/services/services.py` & `profitpulse-2.1.0/src/profitpulse/services/services.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/testrig/fixtures.py` & `profitpulse-2.1.0/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.0.1/src/profitpulse/testrig/scenario.py` & `profitpulse-2.1.0/src/profitpulse/testrig/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     def current_month(self) -> str:
         """
         Returns the current month of the imported transactions.
         """
         # This is one of the months defined in the fixture file comprovativo_cgd.csv
         return "8"
 
-    def import_transactions(self, transactions_file: str, asset_name: str):
+    def import_transactions(self, transactions_file: str):
         result = runner.invoke(
             self._app,
-            ["import", str(transactions_file), asset_name],
+            ["import", str(transactions_file)],
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
```

### Comparing `profitpulse-2.0.1/PKG-INFO` & `profitpulse-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 2.0.1
+Version: 2.1.0
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
```

