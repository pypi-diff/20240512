# Comparing `tmp/monopyly-1.4.6.tar.gz` & `tmp/monopyly-1.4.7.tar.gz`

## Comparing `monopyly-1.4.6.tar` & `monopyly-1.4.7.tar`

### file list

```diff
@@ -1,205 +1,217 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.4.6/README.md -> monopyly/README.md
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/README.md
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/_version.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/actions.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/blueprint.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/routes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/auth/tools.py
--rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/accounts.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/actions.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/banks.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/blueprint.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/filters.py
--rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/forms.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/routes.py
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/banking/transactions.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/cli/apps.py
--rwxr-xr-x   0        0        0     3838 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/cli/run.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/transactions.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/__init__.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/_forms.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/fields.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/utils.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/common/forms/validators.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/default_settings.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/config/settings.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/actions.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/blueprint.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/context_processors.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/filters.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/internal_transactions.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/core/routes.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/accounts.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/actions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/blueprint.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/cards.py
--rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/forms.py
--rw-r--r--   0        0        0    17794 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/routes.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/statements.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/transactions/__init__.py
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/credit/transactions/_transactions.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/__init__.py
--rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/models.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/preloads.sql
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/schema.sql
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/database/views.sql
--rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/jquery-3.7.0.min.js
--rw-r--r--   0        0        0    48930 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/css/style.css
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/browserconfig.xml
--rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-114.png
--rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-120.png
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-144.png
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-150.png
--rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-152.png
--rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-16.png
--rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-160.png
--rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-180.png
--rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-192.png
--rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-310.png
--rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-32.png
--rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-57.png
--rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-60.png
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-64.png
--rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-70.png
--rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-72.png
--rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-76.png
--rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon-96.png
--rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon.ico
--rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/favicon/favicon.png
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/statement.png
--rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-account-details.png
--rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-account-summaries.png
--rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/bank-accounts.png
--rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/credit-account-details.png
--rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/credit-transactions.png
--rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/homepage-user.png
--rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/homepage.png
--rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/about/statement-details.png
--rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/chase-card.png
--rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/discover-card.png
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/new-card.png
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/cards/template-card.png
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-down.png
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-left.png
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/arrow-up.png
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/checkmark.png
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-orange-thick.png
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-orange.png
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete-thick.png
--rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/delete.png
--rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/edit.png
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/link.png
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/minus-thick.png
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/minus.png
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/plus-thick.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/plus.png
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/refresh.png
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/save.png
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/sort-asc.png
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/sort-desc.png
--rw-r--r--   0        0        0    53387 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement-pair.svg
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement.png
--rw-r--r--   0        0        0    50319 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/statement.svg
--rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/img/icons/x-thick.png
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/add-subtransaction.js
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/add-transfer.js
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/autocomplete-transaction.js
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/bind-tag-actions.js
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/create-balance-chart.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/define-filter.js
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-account-type-inputs.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-bank-inputs.js
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/display-new-credit-account-inputs.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-bank-account.js
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-bank.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/expand-transaction.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/flip-card.js
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/hide-homepage-block.js
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/infer-card.js
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/infer-statement.js
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/make-payment.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/show-linked-transaction.js
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-account-statement-parameters.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-bank-name.js
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-card-status.js
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-statement-parameters.js
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-statements-display.js
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/update-transactions-display.js
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/ajax.js
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/autocomplete-input.js
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/expand-box-row.js
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/expand-transaction.js
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-acquisition-form.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-overlays.js
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/manage-subforms.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/update-database-widget.js
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/static/js/modules/update-display-ajax.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credits.html
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/index.html
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/layout.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/profile.html
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/story.html
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/auth/login.html
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/auth/register.html
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_page.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summaries.html
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summaries_page.html
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_summary.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/accounts_page.html
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_form/account_form.html
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/account_form/account_form_page_new.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/bank_info_form.html
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transaction_form/transfer_form.html
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/banking/transactions_table/transactions.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/form_page.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/subform.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/subtransaction_subform.html
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_bank_transaction.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_credit_transaction.html
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/subtransactions.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_condensed.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_expanded.html
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/common/transactions_table/transactions.html
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/account_page.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_submission_page.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/cards.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/cards_page.html
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statement_page.html
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statement_summary.html
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statements.html
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/statements_page.html
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tags_page.html
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_submission_page.html
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_page.html
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/card_form.html
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/card_form_page_new.html
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_back.html
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_front.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tag_tree/subtag_tree.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/tag_tree/tag_tree.html
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.4.6/monopyly/templates/credit/transactions_table/transactions.html
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 monopyly-1.4.6/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.4.6/COPYING
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.4.6/LICENSE
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 monopyly-1.4.6/pyproject.toml
--rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 monopyly-1.4.6/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.4.7/README.md -> monopyly/README.md
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/CHANGELOG.md
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/README.md
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/_version.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/auth/actions.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/auth/blueprint.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/auth/routes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/auth/tools.py
+-rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/accounts.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/actions.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/banks.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/blueprint.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/filters.py
+-rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/forms.py
+-rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/routes.py
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/banking/transactions.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/cli/apps.py
+-rwxr-xr-x   0        0        0     3838 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/cli/run.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/transactions.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/utils.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/forms/__init__.py
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/forms/_forms.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/forms/fields.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/forms/utils.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/common/forms/validators.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/config/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/config/default_settings.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/config/settings.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/actions.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/blueprint.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/context_processors.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/errors.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/filters.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/internal_transactions.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/core/routes.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/accounts.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/actions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/blueprint.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/cards.py
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/forms.py
+-rw-r--r--   0        0        0    18127 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/routes.py
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/statements.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/transactions/__init__.py
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/credit/transactions/_transactions.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/database/__init__.py
+-rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/database/models.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/database/preloads.sql
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/database/schema.sql
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/database/views.sql
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0    50618 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/css/style.css
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/browserconfig.xml
+-rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-114.png
+-rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-120.png
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-144.png
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-150.png
+-rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-152.png
+-rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-16.png
+-rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-160.png
+-rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-180.png
+-rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-192.png
+-rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-310.png
+-rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-32.png
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-57.png
+-rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-60.png
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-64.png
+-rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-70.png
+-rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-72.png
+-rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-76.png
+-rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon-96.png
+-rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon.ico
+-rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/favicon/favicon.png
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/statement.png
+-rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/bank-account-details.png
+-rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/bank-account-summaries.png
+-rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/bank-accounts.png
+-rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/credit-account-details.png
+-rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/credit-transactions.png
+-rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/homepage-user.png
+-rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/homepage.png
+-rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/about/statement-details.png
+-rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/cards/chase-card.png
+-rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/cards/discover-card.png
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/cards/new-card.png
+-rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/cards/template-card.png
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/arrow-down.png
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/arrow-left.png
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/arrow-up.png
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/checkmark.png
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/delete-orange-thick.png
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/delete-orange.png
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/delete-thick.png
+-rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/delete.png
+-rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/edit.png
+-rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/link.png
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/minus-thick.png
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/minus.png
+-rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/plus-thick.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/plus.png
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/refresh.png
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/save.png
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/sort-asc.png
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/sort-desc.png
+-rw-r--r--   0        0        0    53387 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/statement-pair.svg
+-rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/statement.png
+-rw-r--r--   0        0        0    50319 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/statement.svg
+-rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/img/icons/x-thick.png
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/add-subtransaction.js
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/add-transfer.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/autocomplete-transaction.js
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/bind-tag-actions.js
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/create-balance-chart.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/define-filter.js
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/display-new-account-type-inputs.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/display-new-bank-inputs.js
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/display-new-credit-account-inputs.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/expand-bank-account.js
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/expand-bank.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/expand-transaction.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/flip-card.js
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/hide-homepage-block.js
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/infer-card.js
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/infer-statement.js
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/make-payment.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/show-linked-transaction.js
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-account-statement-parameters.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-bank-name.js
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-card-status.js
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-statement-parameters.js
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-statements-display.js
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/update-transactions-display.js
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/ajax.js
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/autocomplete-input.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/expand-box-row.js
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/expand-transaction.js
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/manage-acquisition-form.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/manage-overlays.js
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/manage-subforms.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/update-database-widget.js
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/static/js/modules/update-display-ajax.js
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/layout.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/auth/login.html
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/auth/register.html
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_page.html
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_summaries.html
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_summaries_page.html
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_summary.html
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/accounts_page.html
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_form/account_form.html
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/account_form/account_form_page_new.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/bank_info_form.html
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transaction_form/transfer_form.html
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/banking/transactions_table/transactions.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/form_page.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transaction_form/subform.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transaction_form/subtransaction_subform.html
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_bank_transaction.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_credit_transaction.html
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/subtransactions.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/transaction_condensed.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/transaction_expanded.html
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/common/transactions_table/transactions.html
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/credits.html
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/index.html
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/profile.html
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/story.html
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/400.html
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/401.html
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/403.html
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/404.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/405.html
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/408.html
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/418.html
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/425.html
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/500.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/core/errors/error.html
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/account_page.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_submission_page.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/cards.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/cards_page.html
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/statement_page.html
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/statement_summary.html
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/statements.html
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/statements_page.html
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/tags_page.html
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transaction_submission_page.html
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transactions_page.html
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_form/card_form.html
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_form/card_form_page_new.html
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_graphic/card_back.html
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/card_graphic/card_front.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/tag_tree/subtag_tree.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/tag_tree/tag_tree.html
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.4.7/monopyly/templates/credit/transactions_table/transactions.html
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 monopyly-1.4.7/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.4.7/COPYING
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.4.7/LICENSE
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 monopyly-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0    10952 2020-02-02 00:00:00.000000 monopyly-1.4.7/PKG-INFO
```

### Comparing `monopyly-1.4.6/monopyly/README.md` & `monopyly-1.4.7/monopyly/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,20 +23,31 @@
 ```
 
 The package requires a recent version of Python (3.9+).
 
 
 ## Getting started
 
-Once the package is properly installed, run the app from the command line (the default options should be sensible, but you may customize the host and port if necessary):
+Once the package is properly installed, run the app in local mode from the command line (the default options should be sensible, but you may customize the host and port if necessary):
 
 ```
-$ monopyly development --browser [--host HOST] [--port PORT]
+$ monopyly local --browser [--host HOST] [--port PORT]
 ```
 
+Local mode indicates that the app is just going to be run using a locally hosted server, accessible to just your machine.
+Other available modes are `development` and `production`, for those looking to either develop the application or host the application on a server.
+
+<div class="warning">
+  <h5>Use your brain when choosing a mode!</h5>
+  <small>
+    If you intend to be the only user of the app, served just from your PC, local mode is fine; you will be served well-enough by the built-in Python server, and you do not need to configure secret keys for the application.
+    If you plan to host the application, however, <b>DO NOT</b> use local mode (or development mode) and run the app in production mode instead.
+  </small>
+</div>
+
 By using the `--browser` option in development mode, this will open to an empty homepage with a welcome message.
 
 <img class="screenshot" src="monopyly/static/img/about/homepage.png" alt="user homepage" width="800px">
 
 To use the app, register a new profile and then log in using your newly created credentials.
 A successful login will return you to the homepage, now with several different feature panels.
```

### Comparing `monopyly-1.4.6/monopyly/__init__.py` & `monopyly-1.4.7/monopyly/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Run a development server for the Monopyly app.
 """
 
 from flask import Flask
 
 from monopyly.config import DevelopmentConfig, ProductionConfig
+from monopyly.core.errors import render_error_template
 from monopyly.database import SQLAlchemy, register_db_cli_commands
 
 
 def create_app(test_config=None):
     # Create and configure the app
     app = Flask(__name__, instance_relative_config=True)
 
@@ -28,14 +29,15 @@
     return app
 
 
 @SQLAlchemy.interface_selector
 def init_app(app):
     """Initialize the app."""
     register_blueprints(app)
+    register_errorhandlers(app)
     register_db_cli_commands(app)
 
 
 def register_blueprints(app):
     """
     Register blueprints with the app.
 
@@ -53,7 +55,24 @@
     from monopyly.credit.blueprint import bp as credit_bp
 
     # Register blueprints
     app.register_blueprint(core_bp)
     app.register_blueprint(auth_bp)
     app.register_blueprint(banking_bp)
     app.register_blueprint(credit_bp)
+
+
+def register_errorhandlers(app):
+    """Register error handlers with the app."""
+    handled_error_codes = [
+        400,
+        401,
+        403,
+        404,
+        405,
+        408,
+        418,
+        # 425 -- not yet supported
+        500,
+    ]
+    for code in handled_error_codes:
+        app.register_error_handler(code, render_error_template)
```

### Comparing `monopyly-1.4.6/monopyly/auth/routes.py` & `monopyly-1.4.7/monopyly/auth/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/auth/tools.py` & `monopyly-1.4.7/monopyly/auth/tools.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/accounts.py` & `monopyly-1.4.7/monopyly/banking/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         account_type = super()._validate_authorization(entry_id)
         # Limit manipulation to only the user (excluding common entries)
         if account_type.user_id != cls.user_id:
             abort_msg = (
                 "The current user is not authorized to manipulate "
                 "this account type entry."
             )
-            abort(404, abort_msg)
+            abort(403, abort_msg)
 
 
 class BankAccountHandler(
     DatabaseViewHandler, model=BankAccount, model_view=BankAccountView
 ):
     """
     A database handler for managing bank accounts.
```

### Comparing `monopyly-1.4.6/monopyly/banking/actions.py` & `monopyly-1.4.7/monopyly/banking/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/banks.py` & `monopyly-1.4.7/monopyly/banking/banks.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/filters.py` & `monopyly-1.4.7/monopyly/banking/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/forms.py` & `monopyly-1.4.7/monopyly/banking/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/routes.py` & `monopyly-1.4.7/monopyly/banking/routes.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/banking/transactions.py` & `monopyly-1.4.7/monopyly/banking/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/cli/apps.py` & `monopyly-1.4.7/monopyly/cli/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,47 +5,68 @@
 
 from gunicorn.app.base import BaseApplication
 
 from .. import create_app
 
 
 class LocalApplication:
-    """An object for running the application locally."""
+    """
+    An object for running the application locally.
 
+    This application object will run the Flask application using the
+    built-in Python server on localhost, just like the Flask development
+    mode. However, it will launch from port 5001 to avoid conflicting
+    with other Python servers that may attempt to run on the default
+    port 5000.
+    """
+
+    mode_name = "local"
     default_port = "5001"
     command = ["flask"]
 
     def __init__(self, host=None, port=None, **options):
         """Initialize the application in development mode."""
         self._host = host
         self._port = port
         if options:
             raise NotImplementedError(
-                "Options besides `host` and `port` are not handled in development mode."
+                f"Options besides `host` and `port` are not handled in {self.mode_name} mode."
             )
 
     def run(self):
         """Run the Monopyly application in development mode."""
         instruction = self.command + ["run"]
         if self._host:
             instruction += ["--host", self._host]
         if self._port:
             instruction += ["--port", self._port]
         server = subprocess.Popen(instruction)
 
 
 class DevelopmentApplication(LocalApplication):
-    """An object for running the application in development mode."""
+    """
+    An object for running the application in development mode.
+
+    This application object will run the Flask application using the
+    built-in Python server on localhost, just like the Flask development
+    mode.
+    """
 
+    mode_name = "development"
     default_port = "5000"
     command = LocalApplication.command + ["--debug"]
 
 
 class ProductionApplication(BaseApplication):
-    """An object for running the application in production mode (via Gunicorn)."""
+    """
+    An object for running the application in production mode (via Gunicorn).
+
+    This application object will run the Flask application using a
+    Gunicorn server instead of the built-in Python server.
+    """
 
     default_port = "8000"
     _default_worker_count = (multiprocessing.cpu_count() * 2) + 1
 
     def __init__(self, host=None, port=None, **options):
         """Initialize the application in production mode."""
         options["bind"] = self._parse_binding(host, port, options.get("bind"))
```

### Comparing `monopyly-1.4.6/monopyly/cli/run.py` & `monopyly-1.4.7/monopyly/cli/run.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/common/transactions.py` & `monopyly-1.4.7/monopyly/common/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/common/utils.py` & `monopyly-1.4.7/monopyly/common/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/common/forms/_forms.py` & `monopyly-1.4.7/monopyly/common/forms/_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 General form constructions.
 """
 
 from abc import ABC, abstractmethod
+from datetime import date
 
 from flask_wtf import FlaskForm
 from wtforms.fields import FieldList, FormField, SelectField, StringField, SubmitField
 from wtforms.validators import DataRequired
 
 from .fields import CurrencyField, DateField
 from .validators import SelectionNotBlank
@@ -161,15 +162,17 @@
                 "subtotal": subtransaction.subtotal,
                 "note": subtransaction.note,
                 "tags": ", ".join(tag_names),
             }
             return data
 
     # Fields pertaining to the transaction
-    transaction_date = DateField("Transaction Date", [DataRequired()])
+    transaction_date = DateField(
+        "Transaction Date", validators=[DataRequired()], default=date.today
+    )
     # Subtransactions should be defined as a `FieldList` in a subclass
     subtransactions = None
     submit = SubmitField("Save Transaction")
     # Define an autocompleter for the form (in a sublcass)
     _autocompleter = None
 
     def _prepare_transaction_data(self):
```

### Comparing `monopyly-1.4.6/monopyly/common/forms/fields.py` & `monopyly-1.4.7/monopyly/common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/common/forms/utils.py` & `monopyly-1.4.7/monopyly/common/forms/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/common/forms/validators.py` & `monopyly-1.4.7/monopyly/common/forms/validators.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/config/default_settings.py` & `monopyly-1.4.7/monopyly/config/default_settings.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/config/settings.py` & `monopyly-1.4.7/monopyly/config/settings.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/core/context_processors.py` & `monopyly-1.4.7/monopyly/core/context_processors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """
 Filters defined for the application.
 """
 
 from datetime import date
 from importlib import import_module
 
+from .actions import determine_summary_balance_svg_viewbox_width
 from .blueprint import bp
 
 
 @bp.app_context_processor
 def inject_global_template_variables():
     """Inject template variablees globally into the template context."""
     template_globals = {
         "app_version": _display_version(),
         "copyright_statement": f"© {date.today().year}",
         "date_today": date.today(),
     }
     return template_globals
 
 
+@bp.app_context_processor
+def inject_utility_functions():
+    """Inject utility functions globally into the template context."""
+    utility_functions = {
+        "calculate_summary_balance_width": determine_summary_balance_svg_viewbox_width,
+    }
+    return utility_functions
+
+
 def _display_version():
     """Show the version (without commit information)."""
     try:
         version = import_module("monopyly._version").version
     except ModuleNotFoundError:
         # Fallback action in case Hatch VCS fails
         display_version = ""
```

### Comparing `monopyly-1.4.6/monopyly/core/filters.py` & `monopyly-1.4.7/monopyly/core/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Filters defined for the application.
 """
 
+from math import floor, log10
+
 from .blueprint import bp
 
 
 @bp.app_template_filter("currency")
 def make_currency(amount):
     """Return the amount to two decimal places (always shown)."""
     # Correct values of -0.00 to 0
@@ -28,16 +30,16 @@
         -  10 => 10th
         -  11 => 11th
         -  21 => 21st
         -  101 => 101st
 
     Notes
     -----
-    This function is an adaptation of the one proposed by Stack Overflow user
-    Florian Brucker (https://stackoverflow.com/a/50992575/8754471).
+    This function is an adaptation of the one proposed by Stack Overflow
+    user Florian Brucker (https://stackoverflow.com/a/50992575/8754471).
 
     Parameters
     ----------
     integer : int
         An integer to convert to its ordinal representation.
 
     Returns
```

### Comparing `monopyly-1.4.6/monopyly/core/routes.py` & `monopyly-1.4.7/monopyly/core/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Routes for core functionality.
 """
 
 from pathlib import Path
 
 from flask import g, render_template, render_template_string, session
+from werkzeug.exceptions import abort
 
 from ..auth.tools import login_required
 from ..banking.accounts import BankAccountHandler
 from ..banking.banks import BankHandler
 from ..credit.cards import CreditCardHandler
 from ..credit.statements import CreditStatementHandler
-from .actions import format_readme_as_html_template
+from .actions import convert_changelog_to_html_template, convert_readme_to_html_template
 from .blueprint import bp
 
+APP_ROOT_DIR = Path(__file__).parents[1]
+
 
 @bp.route("/")
 def index():
     if g.user:
         # Set the homepage to show the welcome statement (unless otherwise set)
         session.setdefault("show_homepage_block", True)
         # Get the user's banks and credit cards from the database
@@ -36,44 +39,54 @@
                 card.last_statement_id = last_statement.id
             else:
                 card.last_statement_id = None
     else:
         session["show_homepage_block"] = True
         bank_accounts, active_cards = None, None
     return render_template(
-        "index.html", bank_accounts=bank_accounts, cards=active_cards
+        "core/index.html", bank_accounts=bank_accounts, cards=active_cards
     )
 
 
 @bp.route("/_hide_homepage_block")
 @login_required
 def hide_homepage_block():
     session["show_homepage_block"] = False
     return ""
 
 
 @bp.route("/about")
 def about():
-    readme_path = Path(__file__).parents[1] / "README.md"
-    with readme_path.open(encoding="utf-8") as readme_file:
-        raw_readme_text = readme_file.read()
-    about_page_template = format_readme_as_html_template(raw_readme_text)
+    readme_path = APP_ROOT_DIR / "README.md"
+    about_page_template = convert_readme_to_html_template(readme_path)
     return render_template_string(about_page_template)
 
 
+@bp.route("/changelog")
+def changelog():
+    changelog_path = APP_ROOT_DIR / "CHANGELOG.md"
+    changelog_page_template = convert_changelog_to_html_template(changelog_path)
+    return render_template_string(changelog_page_template)
+
+
 @bp.route("/story")
 @login_required
 def story():
-    return render_template("story.html")
+    return render_template("core/story.html")
 
 
 @bp.route("/credits")
 def credits():
-    return render_template("credits.html")
+    return render_template("core/credits.html")
 
 
 @bp.route("/profile")
 @login_required
 def load_profile():
     banks = BankHandler.get_banks()
     # Return banks as a list to allow multiple reuse
-    return render_template("profile.html", banks=list(banks))
+    return render_template("core/profile.html", banks=list(banks))
+
+
+@bp.route("/change_password")
+def change_password():
+    abort(418)
```

### Comparing `monopyly-1.4.6/monopyly/credit/accounts.py` & `monopyly-1.4.7/monopyly/credit/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/credit/actions.py` & `monopyly-1.4.7/monopyly/credit/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/credit/cards.py` & `monopyly-1.4.7/monopyly/credit/cards.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/credit/forms.py` & `monopyly-1.4.7/monopyly/credit/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/credit/routes.py` & `monopyly-1.4.7/monopyly/credit/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,20 +212,28 @@
     payment_amount = dedelimit_float(post_args["payment_amount"])
     payment_date = parse_date(post_args["payment_date"])
     payment_account_id = int(post_args["payment_bank_account"])
     # Pay towards the card balance
     make_payment(card_id, payment_account_id, payment_date, payment_amount)
     # Get the current statement information from the database
     statement = CreditStatementHandler.get_entry(statement_id)
+    transactions = CreditTransactionHandler.get_transactions(
+        statement_ids=(statement_id,)
+    )
     bank_accounts = BankAccountHandler.get_accounts()
-    return render_template(
+    summary_template = render_template(
         "credit/statement_summary.html",
         statement=statement,
         bank_accounts=bank_accounts,
     )
+    transactions_table_template = render_template(
+        "credit/transactions_table/transactions.html",
+        transactions=transactions,
+    )
+    return jsonify((summary_template, transactions_table_template))
 
 
 @bp.route("/transactions", defaults={"card_id": None})
 @bp.route("/transactions/<int:card_id>")
 @login_required
 def load_transactions(card_id):
     # Get all of the user's credit cards from the database (for the filter)
```

### Comparing `monopyly-1.4.6/monopyly/credit/statements.py` & `monopyly-1.4.7/monopyly/credit/statements.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/credit/transactions/_transactions.py` & `monopyly-1.4.7/monopyly/credit/transactions/_transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         transaction, the transaction's statement, and the credit card
         used to make the transaction. Transactions can be filtered by
         statement or the credit card used. Query results can be ordered
         by either ascending or descending transaction date.
 
         Parameters
         ----------
-        statement_ids : tuple of str, optional
+        statement_ids : tuple of int, optional
             A sequence of statement IDs with which to filter
             transactions (if `None`, all statement IDs will be shown).
         card_ids : tuple of int, optional
             A sequence of card IDs with which to filter transactions (if
             `None`, all card IDs will be shown).
         active : bool, optional
             A flag indicating whether only transactions for active cards
```

### Comparing `monopyly-1.4.6/monopyly/database/__init__.py` & `monopyly-1.4.7/monopyly/database/__init__.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/database/models.py` & `monopyly-1.4.7/monopyly/database/models.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/database/schema.sql` & `monopyly-1.4.7/monopyly/database/schema.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/database/views.sql` & `monopyly-1.4.7/monopyly/database/views.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/jquery-3.7.0.min.js` & `monopyly-1.4.7/monopyly/static/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/css/style.css` & `monopyly-1.4.7/monopyly/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 /*-------------------------------------------*/
 
 
 /* Define custom colors for consistent branding */
 :root {
   --moneytree: #5e8f40;
   --moneytree-leaves: #85bb65;
+  --silver-dollar: #cccccc;
   --masthead-height: 50px;
+  --masthead-color: #2b2b2b;
+  --border-gray: #dddddd;
 }
 
 html {
   height: 100%;
 }
 
 body {
@@ -90,15 +93,15 @@
   display: flex;
   align-items: center;
   height: var(--masthead-height);
   width: 100%;
   border-width: 0 0 4px 3px;
   border-style: solid;
   border-color: var(--moneytree-leaves);
-  background-color: #2b2b2b;
+  background-color: var(--masthead-color);
   opacity: 0.9;
 }
 
 #masthead a {
   text-decoration: none;
 }
 
@@ -113,15 +116,15 @@
   margin: 0;
   color: white;
   font-size: 1.7em;
   text-transform: uppercase;
 }
 
 .monopyly-logo:hover {
-  color: #f5f5f5;
+  filter: brightness(0.95);
 }
 
 
 /*
  * Display navigation links inline
  */
 #nav-menu {
@@ -157,15 +160,15 @@
  * Create a footer with site information
  */
 footer#site-info {
   margin-top: auto;
 }
 
 #site-info p {
-  color: #cccccc;
+  color: var(--silver-dollar);
   font-size: 9pt;
   text-align: center;
 }
 
 #site-info span {
   padding: 0 5px;
 }
@@ -189,28 +192,56 @@
 aside.sidebar {
   display: flex;
   align-items: center;
   flex-direction: column;
   height: 100%;
   width: 10%;
   min-width: 50px;
-  margin-top: 50px; /* Account for content header */
+  margin-top: 50px; /* account for content header */
 }
 
 #content-header h1 {
   height: 50px;
   box-sizing: border-box;
   margin: 0 0 30px 0;
   padding-bottom: 10px;
-  border-bottom: 1px solid #dddddd;
+  border-bottom: 1px solid var(--border-gray);
   text-align: center;
   font-size: 2em;
   letter-spacing: -2px;
 }
 
+#content-header h1.error {
+  text-align: left;
+}
+
+
+/*
+ * Provide styles for error pages
+ */
+.error span.code {
+  margin-left: 30px;
+  color: var(--silver-dollar);
+  font-weight: 300;
+  letter-spacing: 1px;
+}
+
+.custom-error-content p {
+  font-size: 18pt;
+}
+
+.standard-error-content {
+  margin-top: 50px;
+}
+
+.standard-error-content p.error-description {
+  font-size: 12pt;
+  font-style: oblique;
+}
+
 
 /*
  * General object characteristics
  */
 .button:hover {
   filter: brightness(0.85);
   cursor: pointer;
@@ -229,44 +260,71 @@
 
 .action.delete:hover {
   background-image: url('../img/icons/delete-orange.png');
   filter: none;
 }
 
 .button-block {
-  border: 1px solid #dddddd;
+  margin: 15px 0;
+  border: 1px solid var(--border-gray);
   border-radius: 10px;
   box-shadow: 1px 1px 3px #bbbbbb;
   background-color: #eeeeee;
   background-image: linear-gradient(#eeeeee, #e6e6e6);
   color: inherit;
 }
 
+.button-block:first-of-type {
+  margin-top: 0;
+}
+
+.button-block:last-of-type {
+  margin-bottom: 0;
+}
+
 .button-block:hover {
   filter: brightness(0.98);
   text-decoration: none;
 }
 
 .button-block:focus {
   color: inherit;
 }
 
 .screenshot {
   width: 100%; /* override the markdown default */
   margin: 20px 0;
-  border: 1px solid #f3f3f3;
+  border: 1px solid #bbbbbb;
   box-shadow: 3px 3px 5px #bbbbbb;
 }
 
-.grouping {
+.group-stack {
+  margin: 15px 10px 25px;
+  padding: 20px 30px;
   border-radius: 15px;
   box-shadow: 0 0 20px #eeeeee;
   background-color: #eef5eb;
 }
 
+.group-stack .stack-title {
+  display: flex;
+  justify-content: space-between;
+  margin: 0 0 15px 0;
+  padding: 0 15px;
+  font-size: 1.1em;
+  letter-spacing: 1px;
+  text-transform: uppercase;
+}
+
+.group-stack .stack-title-info {
+  margin-left: 15px;
+  color: #888888;
+  font-weight: 400;
+}
+
 .paid-notice {
   color: var(--moneytree-leaves);
   font-weight: bold;
   letter-spacing: 1px;
   text-transform: uppercase;
 }
 
@@ -487,26 +545,27 @@
 form .autocomplete-box {
   position: absolute;
   top: 98%;
   left: 0;
   z-index: 99;
   width: 100%;
   padding-right: 10px;
-  border: 1px solid #cccccc;
+  border: 1px solid var(--silver-dollar);
+  box-sizing: border-box;
   background-color: white;
 }
 
 form .autocomplete-box .item {
   width: 100%;
   padding: 3px 5px;
   cursor: pointer;
 }
 
 form .autocomplete-box .item:hover {
-  background-color: #cccccc;
+  background-color: var(--silver-dollar);
 }
 
 form .autocomplete-box .item.active {
   background-color: var(--moneytree-leaves);
   color: black;
   font-weight: bold;
 }
@@ -639,25 +698,25 @@
   overflow: hidden;
 }
 
 .slide-text-gadget .sleeve {
   position: relative;
   right: -100%;
   width: min-content;
-  transition: 0.4s;
+  transition: 0.4s 0.2s;
 }
 
 .slide-text-gadget:hover .sleeve {
   transform: translateX(-100%);
 }
 
 .slide-text-gadget .sleeve .main {
   position: absolute;
   transform: translateX(-100%);
-  transition: 0.2s;
+  transition: 0.2s 0.2s;
 }
 
 .slide-text-gadget:hover .sleeve .main {
   padding-right: 5px;
 }
 
 
@@ -742,16 +801,16 @@
   transition: inherit;
   cursor: pointer;
 }
 
 .toggle-switch-gadget .option .slider .switch {
   position: relative;
   left: 0;
-  width: 50%;
   height: 100%;
+  width: 50%;
   box-sizing: border-box;
   border-radius: 50%;
   background-color: #eeeeee;
   transition: inherit;
 }
 
 .toggle-switch-gadget input:checked + .option .text {
@@ -768,15 +827,15 @@
 }
 
 
 /*
  * Style generic box tables
  */
 .box-table {
-  border: 2px solid #dddddd;
+  border: 2px solid var(--border-gray);
 }
 
 .box-table .icon-button {
   display: inline-block;
   height: 25px;
   width: 25px;
   margin: 0 5px;
@@ -785,16 +844,16 @@
 }
 
 .box-table .icon-button:hover {
   filter: none;
 }
 
 .box-table .box-row {
-  border-top: 0.5px solid #dddddd;
-  border-bottom: 0.5px solid #dddddd;
+  border-top: 0.5px solid var(--border-gray);
+  border-bottom: 0.5px solid var(--border-gray);
   background-color: #f5f5f5;
 }
 
 .box-table .box-row:hover {
   cursor: pointer;
   filter: brightness(0.98);
 }
@@ -818,15 +877,15 @@
   color: inherit;
   font-size: 8pt;
   text-align: center;
   cursor: pointer;
 }
 
 #card-filter .card:hover {
-  background-color: #cccccc;
+  background-color: var(--silver-dollar);
   text-decoration: none;
 }
 
 #card-filter .inactive.card {
   color: #999999;
 }
 
@@ -874,15 +933,15 @@
 }
 
 
 .credit-card .card-face {
   position: absolute;
   height: 100%;
   width: 100%;
-  border: 1px solid #cccccc;
+  border: 1px solid var(--silver-dollar);
   border-radius: 20px;
   box-shadow: 1px 1px 3px #222222;
   text-align: center;
   backface-visibility: hidden;
 }
 
 .credit-card .card-face.back {
@@ -945,15 +1004,15 @@
 }
 
 .credit-card .card-face.back .icon-button:hover {
   filter: none;
 }
 
 .credit-card.inactive .card-face.front {
-  color: #cccccc;
+  color: var(--silver-dollar);
   filter: brightness(0.9);
 }
 
 .credit-card.inactive .card-face .notice {
   position: absolute;
   bottom: 2em;
   width: 100%;
@@ -1084,15 +1143,15 @@
   min-width: 40px;
   margin: 0 0 0 20px;
   padding: 5px 10px;
 }
 
 .transactions-table .titles,
 .transactions-table .transaction {
-  border-bottom: 1px solid #dddddd;
+  border-bottom: 1px solid var(--border-gray);
 }
 
 .transactions-table .titles {
   min-height: 25px;
   font-weight: bold;
 }
 
@@ -1608,21 +1667,20 @@
   width: 100%;
 }
 
 .details .primary-info {
   display: flex;
   flex-direction: column;
   flex-wrap: wrap;
-  align-items: center;
+  align-items: stretch;
   gap: 10px;
   width: 100%;
 }
 @media screen and (max-width: 1500px) {
   .details .primary-info {
-    display: flex;
     align-items: center;
   }
 }
 
 .details .primary-info::after {
   content: "";
   flex-shrink: 0;
@@ -1635,43 +1693,40 @@
     height: 0%;
   }
 }
 
 .details .summary-container {
   display: flex;
   justify-content: center;
-  min-width: 45%;
+  width: 45%;
+  min-width: 500px;
   margin: 0 0 0 0;
 }
 
 .details .summary-box {
   display: flex;
   flex-direction: column;
-  width: min-content;
+  width: 500px;
+  box-sizing: border-box;
   padding: 40px 50px 60px;
   border-radius: 25px;
   box-shadow: 1px 1px 5px #dddddd;
   background-color: #f8f8f8;
 }
 
 .details .summary-box .balance {
   display: flex;
   justify-content: space-between;
-  min-width: 325px;
   margin: 20px 0;
   font-size: 72pt;
   font-weight: bold;
   letter-spacing: 1px;
   text-align: center;
 }
 
-.details .summary-box .balance .dollar-sign {
-  margin-right: 5px;
-}
-
 .details .summary-box .projected-balance .amount {
   color: var(--moneytree);
   font-weight: 500;
 }
 
 .details .summary-box .projected-balance .amount.negative {
   color: crimson;
@@ -1694,20 +1749,21 @@
 }
 
 .details .summary-box .subtitle {
   font-size: 12pt;
 }
 
 .details .transactions-container {
-  width: 50%;
+  width: 52.5%;
   order: 2;
   min-width: 500px;
 }
 @media screen and (max-width: 1500px) {
   .details .transactions-container {
+    width: 50%;
     order: 1;
     margin-top: 50px;
   }
 }
 
 .details .transactions-table {
   width: 100%;
@@ -1816,18 +1872,18 @@
 
 /*
  * Customization for the 'Home' page
  */
 #homepage-block {
   margin-bottom: 20px;
   padding: 0 0 30px 0;
-  background-color: #dddddd;
-  border: 1px solid #d8d8d8;
+  background-color: gainsboro;
+  border: 1px solid lightgray;
   border-radius: 6px;
-  box-shadow: 2px 2px 5px #cccccc;
+  box-shadow: 2px 2px 5px var(--silver-dollar);
 }
 
 #homepage-block h2 {
   margin: 0 0;
   font-size: 3em;
   letter-spacing: -2px;
   text-align: center;
@@ -1869,15 +1925,15 @@
 #homepage-panels .panel {
   display: flex;
   flex-direction: column;
   flex-grow: 1;
   margin: 20px;
   padding: 50px;
   border: 1px solid #f5f5f5;
-  box-shadow: 2px 2px 5px #cccccc;
+  box-shadow: 2px 2px 5px var(--silver-dollar);
   background-color: #fafafa;
 }
 
 #homepage-panels div:first-of-type {
   margin-left: 0;
 }
 
@@ -1957,23 +2013,63 @@
   text-align: center;
 }
 
 #readme h2 {
   margin-top: 50px;
 }
 
+#readme .warning {
+  padding: 15px 25px;
+  border: 1px solid var(--silver-dollar);
+  border-radius: 10px;
+  box-shadow: 2px 2px 3px var(--silver-dollar);
+  background-color: #f2d7a5;
+}
+
+#readme .warning h5 {
+  margin: 0 0 5px 0;
+}
+
+#changelog {
+  width: 80%;
+  margin: 0 auto;
+}
+
+#changelog h1 {
+  font-size: 32pt;
+  text-align: center;
+}
+
+#changelog h2 {
+  border-bottom: 1px solid var(--border-gray);
+}
+
+#changelog a.latest-release {
+  display: block;
+  margin: 30px 0;
+  font-size: 1.5em;
+}
+
 #story .signature {
   margin-bottom: 100px;
   font-weight: bold;
   font-style: oblique;
   text-align: right;
 }
 
 
 /*
+ * Customization for the 'Credits' page
+ */
+.affiliation-disclaimer {
+  margin-top: 80px;
+}
+
+
+/*
  * Customization for the 'Profile' page
  */
 #profile h2 {
   font-size: 24pt;
 }
 
 #profile .username-section {
@@ -1998,15 +2094,15 @@
   margin-bottom: 60px;
 }
 
 #profile .settings.profile-section {
   flex-basis: 100%;
   margin-right: 0;
   padding-bottom: 50px;
-  border-bottom: 0.5px solid #dddddd;
+  border-bottom: 0.5px solid var(--border-gray);
 }
 
 #profile .banking.profile-section .bank-list {
   width: 90%;
 }
 
 #profile .banking.profile-section .bank-list .bank-block {
@@ -2021,23 +2117,17 @@
   display: none;
   margin-top: 20px;
 }
 
 /*
  * Customization for the 'Bank Accounts' page
  */
-#bank-container .bank-block {
-  margin: 25px 0;
-  padding: 30px;
-}
-
-#bank-container .bank-block h3 {
-  margin-top: 0;
+#bank-container .bank-stack .stack-title {
   padding: 0 30px;
-  /*text-align: center;*/
+  text-align: left;
 }
 
 #bank-container .account-block {
   padding: 25px 30px;
 }
 
 #bank-container .account-block .account-info {
@@ -2064,31 +2154,31 @@
   margin: 50px 0 25px;
   padding: 0 25px;
 }
 
 #account-type-container {
   width: 30%;
   min-width: 350px;
-  border: 2px solid #dddddd;
+  border: 2px solid var(--border-gray);
   background-color: #f5f5f5;
 }
 
 #account-type-container h2 {
   margin: 0;
   padding: 10px;
 }
 
 #account-type-container .account-types {
-  border-top: 2px solid #dddddd;
+  border-top: 2px solid var(--border-gray);
 }
 
 #account-type-container .account-type {
   padding: 10px;
-  border-top: 0.5px solid #dddddd;
-  border-bottom: 0.5px solid #dddddd;
+  border-top: 0.5px solid var(--border-gray);
+  border-bottom: 0.5px solid var(--border-gray);
 }
 
 
 /*
  * Customization for the 'New Bank Account' & 'Update Bank Account' pages
  */
 form#bank-account .hidden {
@@ -2101,49 +2191,53 @@
  */
 #bank-account-summaries-container {
   display: flex;
   flex-direction: column;
   align-items: center
 }
 
-#bank-account-summaries-container .bank {
-  margin: 0 0 10px;
+#bank-account-summaries-container h2.bank {
+  margin: 0 0 5px;
+  font-size: 1.6em;
+  letter-spacing: 1px;
+  text-transform: uppercase;
   text-align: center;
+}
+
+#bank-account-summaries-container h3.balance {
+  margin: 0 0 10px;
+  color: gray;
+  font-size: 1em;
+  font-weight: 300;
   text-transform: uppercase;
+  text-align: center;
+  letter-spacing: 1px;
 }
 
 #bank-account-summaries {
   display: flex;
   flex-direction: column;
   width: 100%;
 }
 
-#bank-account-summaries .account-type-block {
+#bank-account-summaries .account-type-stack {
   display: flex;
   flex-direction: column;
-  width: 50%;
+  width: 60%;
   min-width: 400px;
-  margin: 10px auto;
-  padding: 25px;
+  margin: 15px auto 25px;
 }
 
 #bank-account-summaries .account-block {
   display: flex;
   justify-content: space-between;
   align-items: center;
-  width: 100%;
-  box-sizing: border-box;
-  margin-bottom: 15px;
   padding: 30px 10%;
 }
 
-#bank-account-summaries a.account-block:last-of-type {
-  margin-bottom: 0;
-}
-
 #bank-account-summaries .account-block .title {
   font-size: 16pt;
 }
 
 #bank-account-summaries .account-block .title .digits {
   margin-right: 10px;
 }
@@ -2404,35 +2498,29 @@
 }
 
 #credit-statements {
   display: flex;
   justify-content: space-around;
 }
 
-#credit-statements .card-column {
+#credit-statements .card-stack {
   display: flex;
   flex-direction: column;
   height: min-content;
-  margin: 15px 10px;
-  padding: 20px;
-  text-transform: uppercase;
-  text-align: center;
-  font-size: 1.1em;
 }
 
-#credit-statements-container .card-column .digits {
-  color: #888888;
+#credit-statements .card-stack .stack-title {
+  justify-content: center;
 }
 
 #credit-statements .statement-block {
   display: flex;
-  align-items: center;
   justify-content: space-between;
+  align-items: center;
   width: 275px;
-  margin: 15px;
   padding: 45px 50px;
 }
 
 #credit-statements .statement-block .date,
 #credit-statements .statement-block .payment {
   display: flex;
   flex-direction: column;
@@ -2507,15 +2595,15 @@
 form#pay input {
   margin: 0;
   border: none;
   border-radius: inherit;
 }
 
 form#pay .form-inputs {
-  border: 1px solid #cccccc;
+  border: 1px solid var(--silver-dollar);
   border-radius: inherit;
 }
 
 form#pay select optgroup {
   font-size: 10pt;
 }
 
@@ -2673,15 +2761,15 @@
   width: 200px;
   margin: 5px 0;
   padding: 2px 15px;
   border: 0 solid var(--moneytree-leaves);
   border-radius: 20px;
   text-align: center;
   outline: none;
-  caret-color: #cccccc;
+  caret-color: var(--silver-dollar);
   transition: border 0.1s ease;
 }
 
 #transaction-tags input.new-tag.visible {
   border: 1.5px solid var(--moneytree-leaves);
 }
 
@@ -2729,10 +2817,10 @@
   background-image: url('../img/icons/delete-orange-thick.png');
   filter: none;
 }
 
 #transaction-tags .subtags {
   margin: 0 0 0 10px;
   padding-left: 40px;
-  border-left: 1px solid #dddddd;
+  border-left: 1px solid var(--border-gray);
 }
```

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-114.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-114.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-120.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-120.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-144.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-144.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-150.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-150.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-152.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-152.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-16.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-16.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-160.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-160.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-180.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-180.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-192.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-192.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-310.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-310.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-32.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-32.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-57.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-57.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-60.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-60.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-64.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-64.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-70.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-70.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-72.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-72.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-76.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-76.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon-96.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon-96.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon.ico` & `monopyly-1.4.7/monopyly/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/favicon/favicon.png` & `monopyly-1.4.7/monopyly/static/favicon/favicon.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/statement.png` & `monopyly-1.4.7/monopyly/static/img/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/bank-account-details.png` & `monopyly-1.4.7/monopyly/static/img/about/bank-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/bank-account-summaries.png` & `monopyly-1.4.7/monopyly/static/img/about/bank-account-summaries.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/bank-accounts.png` & `monopyly-1.4.7/monopyly/static/img/about/bank-accounts.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/credit-account-details.png` & `monopyly-1.4.7/monopyly/static/img/about/credit-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/credit-transactions.png` & `monopyly-1.4.7/monopyly/static/img/about/credit-transactions.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/homepage-user.png` & `monopyly-1.4.7/monopyly/static/img/about/homepage-user.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/homepage.png` & `monopyly-1.4.7/monopyly/static/img/about/homepage.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/about/statement-details.png` & `monopyly-1.4.7/monopyly/static/img/about/statement-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/cards/chase-card.png` & `monopyly-1.4.7/monopyly/static/img/cards/chase-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/cards/discover-card.png` & `monopyly-1.4.7/monopyly/static/img/cards/discover-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/cards/new-card.png` & `monopyly-1.4.7/monopyly/static/img/cards/new-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/cards/template-card.png` & `monopyly-1.4.7/monopyly/static/img/cards/template-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/arrow-down.png` & `monopyly-1.4.7/monopyly/static/img/icons/arrow-down.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/arrow-left.png` & `monopyly-1.4.7/monopyly/static/img/icons/arrow-left.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/arrow-up.png` & `monopyly-1.4.7/monopyly/static/img/icons/arrow-up.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/checkmark.png` & `monopyly-1.4.7/monopyly/static/img/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/delete-orange-thick.png` & `monopyly-1.4.7/monopyly/static/img/icons/delete-orange-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/delete-orange.png` & `monopyly-1.4.7/monopyly/static/img/icons/delete-orange.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/delete-thick.png` & `monopyly-1.4.7/monopyly/static/img/icons/delete-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/delete.png` & `monopyly-1.4.7/monopyly/static/img/icons/delete.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/edit.png` & `monopyly-1.4.7/monopyly/static/img/icons/edit.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/link.png` & `monopyly-1.4.7/monopyly/static/img/icons/link.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/minus-thick.png` & `monopyly-1.4.7/monopyly/static/img/icons/minus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/minus.png` & `monopyly-1.4.7/monopyly/static/img/icons/minus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/plus-thick.png` & `monopyly-1.4.7/monopyly/static/img/icons/plus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/plus.png` & `monopyly-1.4.7/monopyly/static/img/icons/plus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/refresh.png` & `monopyly-1.4.7/monopyly/static/img/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/save.png` & `monopyly-1.4.7/monopyly/static/img/icons/save.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/sort-asc.png` & `monopyly-1.4.7/monopyly/static/img/icons/sort-asc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/sort-desc.png` & `monopyly-1.4.7/monopyly/static/img/icons/sort-desc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/statement-pair.svg` & `monopyly-1.4.7/monopyly/static/img/icons/statement-pair.svg`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/statement.png` & `monopyly-1.4.7/monopyly/static/img/icons/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/statement.svg` & `monopyly-1.4.7/monopyly/static/img/icons/statement.svg`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/img/icons/x-thick.png` & `monopyly-1.4.7/monopyly/static/img/icons/x-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/add-subtransaction.js` & `monopyly-1.4.7/monopyly/static/js/add-subtransaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/add-transfer.js` & `monopyly-1.4.7/monopyly/static/js/add-transfer.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/autocomplete-transaction.js` & `monopyly-1.4.7/monopyly/static/js/autocomplete-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/bind-tag-actions.js` & `monopyly-1.4.7/monopyly/static/js/bind-tag-actions.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/create-balance-chart.js` & `monopyly-1.4.7/monopyly/static/js/create-balance-chart.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/define-filter.js` & `monopyly-1.4.7/monopyly/static/js/define-filter.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/display-new-account-type-inputs.js` & `monopyly-1.4.7/monopyly/static/js/display-new-account-type-inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/display-new-credit-account-inputs.js` & `monopyly-1.4.7/monopyly/static/js/display-new-credit-account-inputs.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/expand-bank-account.js` & `monopyly-1.4.7/monopyly/static/js/expand-bank-account.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/expand-bank.js` & `monopyly-1.4.7/monopyly/static/js/expand-bank.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/expand-transaction.js` & `monopyly-1.4.7/monopyly/static/js/expand-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/flip-card.js` & `monopyly-1.4.7/monopyly/static/js/flip-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/infer-card.js` & `monopyly-1.4.7/monopyly/static/js/infer-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/infer-statement.js` & `monopyly-1.4.7/monopyly/static/js/infer-statement.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/make-payment.js` & `monopyly-1.4.7/monopyly/static/js/make-payment.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,16 @@
 import {
     executeAjaxRequest
 } from './modules/ajax.js';
 
 
 (function() {
 
-    const $container = $('#statement-summary-container');
+    const $summaryContainer = $('#statement-summary-container');
+    const $transactionContainer = $('#statement-transactions-container');
     prepareForm();
 
     function prepareForm() {
 
         // Identify the key elements
         let $buttonPay = $('#make-payment[type="button"]');
 
@@ -80,15 +81,16 @@
         });
     }
 
 
     function updateStatementPaymentAjaxRequest(rawData) {
         // Return the newly updated statement payment info
         function updateAction(response) {
-            $container.html(response)
+            $summaryContainer.html(response[0]);
+            $transactionContainer.html(response[1]);
             // Prepare the form again (in case statement is not paid in full)
             prepareForm();
         }
         executeAjaxRequest(MAKE_PAYMENT_ENDPOINT, rawData, updateAction);
     }
 
 })();
```

### Comparing `monopyly-1.4.6/monopyly/static/js/show-linked-transaction.js` & `monopyly-1.4.7/monopyly/static/js/show-linked-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-account-statement-parameters.js` & `monopyly-1.4.7/monopyly/static/js/update-account-statement-parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-bank-name.js` & `monopyly-1.4.7/monopyly/static/js/update-bank-name.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-card-status.js` & `monopyly-1.4.7/monopyly/static/js/update-card-status.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-statement-parameters.js` & `monopyly-1.4.7/monopyly/static/js/update-statement-parameters.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-statements-display.js` & `monopyly-1.4.7/monopyly/static/js/update-statements-display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/update-transactions-display.js` & `monopyly-1.4.7/monopyly/static/js/update-transactions-display.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/ajax.js` & `monopyly-1.4.7/monopyly/static/js/modules/ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/autocomplete-input.js` & `monopyly-1.4.7/monopyly/static/js/modules/autocomplete-input.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/expand-box-row.js` & `monopyly-1.4.7/monopyly/static/js/modules/expand-box-row.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/expand-transaction.js` & `monopyly-1.4.7/monopyly/static/js/modules/expand-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/manage-acquisition-form.js` & `monopyly-1.4.7/monopyly/static/js/modules/manage-acquisition-form.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/manage-overlays.js` & `monopyly-1.4.7/monopyly/static/js/modules/manage-overlays.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/manage-subforms.js` & `monopyly-1.4.7/monopyly/static/js/modules/manage-subforms.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/update-database-widget.js` & `monopyly-1.4.7/monopyly/static/js/modules/update-database-widget.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/static/js/modules/update-display-ajax.js` & `monopyly-1.4.7/monopyly/static/js/modules/update-display-ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/index.html` & `monopyly-1.4.7/monopyly/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/layout.html` & `monopyly-1.4.7/monopyly/templates/layout.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/profile.html` & `monopyly-1.4.7/monopyly/templates/core/profile.html`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
       <div class="settings profile-section">
 
         <h2>Settings</h2>
 
         <div class=user-settings">
 
           <div class="password">
-            <a style="color: gray;" href="">Change password (coming soon)</a>
+            <a style="color: gray;" href="{{ url_for('core.change_password') }}">
+              Change password (coming soon)
+            </a>
           </div>
 
         </div>
 
       </div>
 
       <div class="banking profile-section">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends "layout.html" %} {% block title %} Profile {% endblock %} {% block
 header %}
 ************ PPrrooffiillee ************
 {% endblock %} {% block content %}
 {{ g.user.username }}
 ********** SSeettttiinnggss **********
-Change password (coming soon)
+_C_h_a_n_g_e_ _p_a_s_s_w_o_r_d_ _(_c_o_m_i_n_g_ _s_o_o_n_)
 ********** BBaannkkss **********
 {% for bank in banks %}
 {{ bank.bank_name }}
 [{{ bank.bank_name }}]
 [{{ url_for('static', filename='img/icons/edit.png') }}]
 {% endfor %}
 ********** TTrraannssaaccttiioonnss **********
```

### Comparing `monopyly-1.4.6/monopyly/templates/story.html` & `monopyly-1.4.7/monopyly/templates/core/story.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/account_page.html` & `monopyly-1.4.7/monopyly/templates/banking/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/account_summaries_page.html` & `monopyly-1.4.7/monopyly/templates/banking/account_summaries_page.html`

 * *Files 13% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
 {% endblock %}
 
 
 {% block content %}
 
   <div id="bank-account-summaries-container">
-    <h2 class="bank">{{ bank.bank_name }} (${{ bank_balance|currency }})</h2>
+    <h2 class="bank">{{ bank.bank_name }}</h2>
+    <h3 class="balance">${{ bank_balance|currency }}</h3>
 
     {% include 'banking/account_summaries.html' %}
 
   </div>
   <a name="bottom"></a>
 
 {% endblock %}
```

### Comparing `monopyly-1.4.6/monopyly/templates/banking/account_summary.html` & `monopyly-1.4.7/monopyly/templates/banking/account_summary.html`

 * *Files 27% similar despite different names*

```diff
@@ -5,16 +5,21 @@
   </div>
 
   <div class="title">
     {{ account.account_type.type_common_name.upper() }}
   </div>
 
   <div class="balance">
-    <div class="dollar-sign">$</div>
-    <div>{{ account.balance|currency }}</div>
+    {% with account_balance = account.balance|currency %}
+      {% set vbox_width = calculate_summary_balance_width(account_balance) %}
+      <svg viewBox="0 0 {{ vbox_width }} 100">
+        <text x="0" y="75" fill="currentColor">$</text>
+        <text x="75" y="75" fill="currentColor">{{ account_balance }}</text>
+      </svg>
+    {% endwith %}
   </div>
 
   {% if account.balance != account.projected_balance %}
     <div class="projected-balance subtitle">
       <span>Projected balance: </span>
       <span class="amount{{ ' negative' if account.projected_balance < 0 }}">
         ${{ account.projected_balance|currency }}
```

### Comparing `monopyly-1.4.6/monopyly/templates/banking/accounts_page.html` & `monopyly-1.4.7/monopyly/templates/banking/accounts_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 {% block content %}
 
   <div id="bank-container">
     {% for bank in banks %}
       {% set bank_accounts = bank.bank_accounts %}
       {% if bank_accounts %}
 
-        <div class="bank-block grouping">
-          <h3>{{ bank.bank_name }}</h3>
+        <div class="bank-stack group-stack">
+          <h2 class="stack-title">{{ bank.bank_name }}</h2>
 
           <div class="account-blocks box-table">
             {% for account in bank_accounts %}
 
               <div class="account-block box-row">
 
                 <div class="account-info">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends 'layout.html' %} {% block header %}
 ************ {{%% bblloocckk ttiittllee %%}} BBaannkk AAccccoouunnttss {{%% eennddbblloocckk %%}} ************
 {% endblock %} {% block content %}
 {% for bank in banks %} {% set bank_accounts = bank.bank_accounts %} {% if
 bank_accounts %}
-******** {{{{ bbaannkk..bbaannkk__nnaammee }}}} ********
+********** {{{{ bbaannkk..bbaannkk__nnaammee }}}} **********
 {% for account in bank_accounts %}
 {{ account.last_four_digits }} {{{{ aaccccoouunntt..aaccccoouunntt__ttyyppee..ttyyppee__nnaammee }}}}
 {% endfor %}
 {% endif %} {% endfor %}
 ********** BBaannkk AAccccoouunntt TTyyppeess **********
 {% for account_type in account_types %}
 {{ account_type.type_name }} {% if account_type.type_abbreviation %} ({
```

### Comparing `monopyly-1.4.6/monopyly/templates/banking/account_form/account_form.html` & `monopyly-1.4.7/monopyly/templates/banking/account_form/account_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/account_form/account_form_page_new.html` & `monopyly-1.4.7/monopyly/templates/banking/account_form/account_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/transaction_form/bank_info_form.html` & `monopyly-1.4.7/monopyly/templates/banking/transaction_form/bank_info_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form.html` & `monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/transaction_form/transaction_form_page.html` & `monopyly-1.4.7/monopyly/templates/banking/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/transactions_table/expanded_row_content.html` & `monopyly-1.4.7/monopyly/templates/banking/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/banking/transactions_table/transaction_field_titles.html` & `monopyly-1.4.7/monopyly/templates/banking/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transaction_form/subtransaction_subform.html` & `monopyly-1.4.7/monopyly/templates/common/transaction_form/subtransaction_subform.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_bank_transaction.html` & `monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_bank_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_credit_transaction.html` & `monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_credit_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transactions_table/linked_transaction_overlay.html` & `monopyly-1.4.7/monopyly/templates/common/transactions_table/linked_transaction_overlay.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transactions_table/transaction_expanded.html` & `monopyly-1.4.7/monopyly/templates/common/transactions_table/transaction_expanded.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/common/transactions_table/transactions.html` & `monopyly-1.4.7/monopyly/templates/common/transactions_table/transactions.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/account_page.html` & `monopyly-1.4.7/monopyly/templates/credit/account_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/cards.html` & `monopyly-1.4.7/monopyly/templates/credit/cards.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/statement_page.html` & `monopyly-1.4.7/monopyly/templates/credit/statement_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/statement_summary.html` & `monopyly-1.4.7/monopyly/templates/credit/statement_summary.html`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,21 @@
   </div>
 
   <div id="issue-date" class="title">
     {{ statement.issue_date.strftime('%B %Y') }}
   </div>
 
   <div class="balance">
-    <div class="dollar-sign">$</div>
-    <div>{{ statement.balance|currency }}</div>
+    {% with statement_balance = statement.balance|currency %}
+      {% set vbox_width = calculate_summary_balance_width(statement_balance) %}
+      <svg viewBox="0 0 {{ vbox_width }} 100">
+        <text x="0" y="75" fill="currentColor">$</text>
+        <text x="75" y="75" fill="currentColor">{{ statement_balance }}</text>
+      </svg>
+    {% endwith %}
   </div>
 
   <div id="payment">
 
     <div id="due">
       <div>DUE</div>
       <div id="due-date" class="update-db-widget right-hover-style">
```

### Comparing `monopyly-1.4.6/monopyly/templates/credit/statements.html` & `monopyly-1.4.7/monopyly/templates/credit/statements.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 <div id="credit-statements">
 
-  {% for card in card_statements %}
+  {% for card, statements in card_statements|items %}
 
-    <div class="card-column grouping">
+    <div class="card-stack group-stack">
 
-      <div>
-        <b>{{ card.account.bank.bank_name }}</b> <span class="digits">{{ card.last_four_digits }}</span>
-      </div>
+      <h2 class="stack-title">
+        {{ card.account.bank.bank_name }}
+        <span class="stack-title-info">{{ card.last_four_digits }}</span>
+      </h2>
 
       <div class="statement-blocks">
-        {% for statement in card_statements[card] %}
+        {% for statement in statements %}
           {% if statement.balance is not none %}
 
             <a class="statement-block button-block" href="{{ url_for('credit.load_statement_details', statement_id=statement.id) }}">
               <div class="date">
                 <div class="month">{{ statement.issue_date.strftime('%b')|upper }}</div>
                 <div class="year">{{ statement.issue_date.year }}</div>
               </div>
```

### Comparing `monopyly-1.4.6/monopyly/templates/credit/statements_page.html` & `monopyly-1.4.7/monopyly/templates/credit/statements_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/tags_page.html` & `monopyly-1.4.7/monopyly/templates/credit/tags_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transaction_submission_page.html` & `monopyly-1.4.7/monopyly/templates/credit/transaction_submission_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transactions_page.html` & `monopyly-1.4.7/monopyly/templates/credit/transactions_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/card_form/card_form.html` & `monopyly-1.4.7/monopyly/templates/credit/card_form/card_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/card_form/card_form_page_new.html` & `monopyly-1.4.7/monopyly/templates/credit/card_form/card_form_page_new.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/card_form/transfer_statement_inquiry.html` & `monopyly-1.4.7/monopyly/templates/credit/card_form/transfer_statement_inquiry.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_back.html` & `monopyly-1.4.7/monopyly/templates/credit/card_graphic/card_back.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/card_graphic/card_front.html` & `monopyly-1.4.7/monopyly/templates/credit/card_graphic/card_front.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/tag_tree/subtag_tree.html` & `monopyly-1.4.7/monopyly/templates/credit/tag_tree/subtag_tree.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form.html` & `monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transaction_form/transaction_form_page.html` & `monopyly-1.4.7/monopyly/templates/credit/transaction_form/transaction_form_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transactions_table/condensed_row_content.html` & `monopyly-1.4.7/monopyly/templates/credit/transactions_table/condensed_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transactions_table/expanded_row_content.html` & `monopyly-1.4.7/monopyly/templates/credit/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/monopyly/templates/credit/transactions_table/transaction_field_titles.html` & `monopyly-1.4.7/monopyly/templates/credit/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/.gitignore` & `monopyly-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/COPYING` & `monopyly-1.4.7/COPYING`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/pyproject.toml` & `monopyly-1.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monopyly-1.4.6/PKG-INFO` & `monopyly-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopyly
-Version: 1.4.6
+Version: 1.4.7
 Summary: A homemade personal finance manager.
 Project-URL: Download, https://pypi.org/project/monopyly
 Project-URL: Homepage, http://monopyly.com
 Project-URL: Repository, https://github.com/mitchnegus/monopyly
 Project-URL: Changelog, https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
@@ -59,20 +59,31 @@
 ```
 
 The package requires a recent version of Python (3.9+).
 
 
 ## Getting started
 
-Once the package is properly installed, run the app from the command line (the default options should be sensible, but you may customize the host and port if necessary):
+Once the package is properly installed, run the app in local mode from the command line (the default options should be sensible, but you may customize the host and port if necessary):
 
 ```
-$ monopyly development --browser [--host HOST] [--port PORT]
+$ monopyly local --browser [--host HOST] [--port PORT]
 ```
 
+Local mode indicates that the app is just going to be run using a locally hosted server, accessible to just your machine.
+Other available modes are `development` and `production`, for those looking to either develop the application or host the application on a server.
+
+<div class="warning">
+  <h5>Use your brain when choosing a mode!</h5>
+  <small>
+    If you intend to be the only user of the app, served just from your PC, local mode is fine; you will be served well-enough by the built-in Python server, and you do not need to configure secret keys for the application.
+    If you plan to host the application, however, <b>DO NOT</b> use local mode (or development mode) and run the app in production mode instead.
+  </small>
+</div>
+
 By using the `--browser` option in development mode, this will open to an empty homepage with a welcome message.
 
 <img class="screenshot" src="https://raw.githubusercontent.com/mitchnegus/monopyly/main/monopyly/static/img/about/homepage.png" alt="user homepage" width="800px">
 
 To use the app, register a new profile and then log in using your newly created credentials.
 A successful login will return you to the homepage, now with several different feature panels.
```

