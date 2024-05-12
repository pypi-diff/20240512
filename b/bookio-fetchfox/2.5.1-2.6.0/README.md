# Comparing `tmp/bookio_fetchfox-2.5.1.tar.gz` & `tmp/bookio_fetchfox-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-2.5.1.tar", max compression
+gzip compressed data, was "bookio_fetchfox-2.6.0.tar", max compression
```

## Comparing `bookio_fetchfox-2.5.1.tar` & `bookio_fetchfox-2.6.0.tar`

### file list

```diff
@@ -1,77 +1,75 @@
--rw-r--r--   0        0        0     3734 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2649 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      694 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1501 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     2337 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      686 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      317 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2289 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/cardano/dexhunterio.py
--rw-r--r--   0        0        0     7351 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/cardano/gomaestroorg.py
--rw-r--r--   0        0        0     1868 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0      592 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/cardano/muesliswap.py
--rwxr-xr-x   0        0        0     2197 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0     1089 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     5900 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     3215 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      285 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/pinatacloud.py
--rw-r--r--   0        0        0      228 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/apis/price.py
--rw-r--r--   0        0        0      120 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2024-05-08 19:34:43.649417 bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0    10494 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      689 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/exceptions.py
--rw-r--r--   0        0        0      502 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     3408 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    17568 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0      679 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/exceptions.py
--rw-r--r--   0        0        0     1060 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1696 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    11880 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      753 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/exceptions.py
--rw-r--r--   0        0        0      617 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0      443 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/exceptions.py
--rw-r--r--   0        0        0       32 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      299 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/beard.py
--rw-r--r--   0        0        0      158 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      399 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/book.py
--rw-r--r--   0        0        0       82 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      163 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      341 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0   453386 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/ranks.py
--rw-r--r--   0        0        0       95 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       62 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      329 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3719 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3666 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      495 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1572 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      948 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/order.py
--rw-r--r--   0        0        0     1203 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/pair_stats.py
--rw-r--r--   0        0        0      365 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     2023 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0        0 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/pools/__init__.py
--rw-r--r--   0        0        0     1177 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/pools/book_pool.py
--rw-r--r--   0        0        0     6138 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/rest.py
--rw-r--r--   0        0        0      106 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/tokens/__init__.py
--rw-r--r--   0        0        0     4025 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/tokens/base.py
--rw-r--r--   0        0        0      744 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/tokens/beard_token.py
--rw-r--r--   0        0        0      811 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/tokens/book_token.py
--rw-r--r--   0        0        0      802 2024-05-08 19:34:43.653417 bookio_fetchfox-2.5.1/fetchfox/tokens/hosky_token.py
--rw-r--r--   0        0        0     1170 2024-05-08 19:34:43.665418 bookio_fetchfox-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 bookio_fetchfox-2.5.1/setup.py
--rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 bookio_fetchfox-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3560 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2686 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0     1551 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0      721 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      354 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2489 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/cardano/dexhunterio.py
+-rw-r--r--   0        0        0     7444 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/cardano/gomaestroorg.py
+-rw-r--r--   0        0        0     1917 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0      635 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/cardano/muesliswapcom.py
+-rwxr-xr-x   0        0        0     2830 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     5952 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     3268 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      341 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/pinatacloud.py
+-rw-r--r--   0        0        0      260 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/apis/price.py
+-rw-r--r--   0        0        0      120 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     7656 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      689 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/algorand/exceptions.py
+-rw-r--r--   0        0        0      502 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     3408 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    17633 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0      679 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/exceptions.py
+-rw-r--r--   0        0        0     1060 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1696 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    11880 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      753 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/exceptions.py
+-rw-r--r--   0        0        0      617 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0      443 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/exceptions.py
+-rw-r--r--   0        0        0       32 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/beard.py
+-rw-r--r--   0        0        0      158 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      399 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/book.py
+-rw-r--r--   0        0        0       82 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      194 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      341 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0   453386 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/ranks.py
+-rw-r--r--   0        0        0       95 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       62 2024-05-12 14:04:29.250708 bookio_fetchfox-2.6.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      329 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3666 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      495 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1572 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      948 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/order.py
+-rw-r--r--   0        0        0     1203 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/pair_stats.py
+-rw-r--r--   0        0        0      365 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     2023 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/pools/__init__.py
+-rw-r--r--   0        0        0     1177 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/pools/book_pool.py
+-rw-r--r--   0        0        0     6138 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/rest.py
+-rw-r--r--   0        0        0      106 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/tokens/__init__.py
+-rw-r--r--   0        0        0     4025 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/tokens/base.py
+-rw-r--r--   0        0        0      744 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/tokens/beard_token.py
+-rw-r--r--   0        0        0      811 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/tokens/book_token.py
+-rw-r--r--   0        0        0      802 2024-05-12 14:04:29.254709 bookio_fetchfox-2.6.0/fetchfox/tokens/hosky_token.py
+-rw-r--r--   0        0        0     1170 2024-05-12 14:04:29.262709 bookio_fetchfox-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.0/setup.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.0/PKG-INFO
```

### Comparing `bookio_fetchfox-2.5.1/README.md` & `bookio_fetchfox-2.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 ### Algorand
 
 ```python
 import os
 from fetchfox.blockchains import Algorand
 
-algorand = Algorand(
-    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),
-)
+algorand = Algorand()
 
 # Brave New World
 creator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"
 
 for asset in algorand.get_assets(creator_address):
     print(asset)
 ```
@@ -42,35 +40,34 @@
 ### Cardano
 
 ```python
 import os
 from fetchfox.blockchains import Cardano
 
 cardano = Cardano(
-    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),
+    gomaestroorg_api_key=os.getenv("GOMAESTROORG_API_KEY"),
 )
 
 # Gutenberg Bible
 policy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"
 
 for asset in cardano.get_collection_assets(policy_id):
     print(asset)
 ```
 
 #### Services
 
-* get_asset ([blockfrost.io²](https://blockfrost.io))
-* get_assets ([blockfrost.io²](https://blockfrost.io))
-* get_holdings ([blockfrost.io²](https://blockfrost.io))
+* get_asset ([gomaestro.org²](https://gomaestro.org))
+* get_assets ([gomaestro.org²](https://gomaestro.org))
+* get_holdings ([gomaestro.org²](https://bgomaestro.org))
 * get_campaigns ([book.io](https://book.io))
-* get_snapshot ([blockfrost.io²](https://blockfrost.io))
+* get_snapshot ([gomaestro.org²](https://gomaestro.org))
 * get_listings ([jpg.store](https://jpg.store))
 * get_floor ([jpg.store](https://jpg.store))
 * get_sales ([jpg.store](https://jpg.store))
-* get_ranks ([cnft.tools](https://cnft.tools))
 
 
 ### EVM (Ethereum and Polygon)
 
 ```python
 import os
 from fetchfox.blockchains import Ethereum, Polygon
@@ -109,17 +106,17 @@
 * get_snapshot ([moralis.io³](https://moralis.io))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([opensea.io⁴](https://opensea.io))
 * get_floor ([opensea.io⁴](https://opensea.io))
 * get_sales ([opensea.io⁴](https://opensea.io))
 
 
-> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).
+> ¹ **nftexplorer.app** this api has been deprecated.
 > 
-> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).
+> ² **gomaestro.org** services require an [api key](https://www.gomaestro.org/pricing).
 > 
 > ³ **moralis.io** services require an [api key](https://moralis.io/pricing).
 > 
 > ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). 
 
 ---
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from base64 import b64decode
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.environ.get(
-    "ALGONODE_API_BASE_URL",
-    "https://mainnet-idx.algonode.cloud",
-)
+# CONFIG
+
+BASE_URL_DEFAULT = "https://mainnet-idx.algonode.cloud"
+BASE_URL = os.getenv("ALGONODECLOUD_API_BASE_URL") or BASE_URL_DEFAULT
 
 
 def get(service: str, params: dict = None, version: int = 2) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
     )
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.environ.get(
-    "ALGOXNFT_API_BASE_URL",
-    "https://api.algoxnft.com",
-)
+# CONFIG
+
+BASE_URL_DEFAULT = "https://randswap.com"
+BASE_URL = os.getenv("RANDSWAPCOM_API_BASE_URL") or BASE_URL_DEFAULT
 
 
 def get(service: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
     )
 
 
 def get_collection_listings(creator_address: str) -> Iterable[dict]:
-    check_str(creator_address, "algoxnftcom.creator_address")
+    check_str(creator_address, "randswapcom.creator_address")
     creator_address = creator_address.strip().upper()
 
     response, status_code = get(
-        service=f"nft-explorer/creator/{creator_address}",
+        service=f"listings/creator/{creator_address}",
     )
 
     yield from response
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import os
 from functools import lru_cache
 from typing import Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.getenv(
-    "NFDOMAINS_API_BASE_URL",
-    "https://api.nf.domains",
-)
+# CONFIG
+
+BASE_URL_DEFAULT = "https://api.nf.domains"
+BASE_URL = os.getenv("NFDOMAINS_API_BASE_URL") or BASE_URL_DEFAULT
+
+# CONSTANTS
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/cardano/dexhunterio.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/cardano/dexhunterio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 from typing import Iterable
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.getenv(
-    "DEXHUNTER_API_BASE_URL",
-    "https://dexhunter.sbase.ch/",
-)
+# CONFIG
 
-PARTNER_CODE = os.getenv("DEXHUNTER_PARTNER_CODE")
+BASE_URL_DEFAULT = "https://dexhunter.sbase.ch/"
+BASE_URL = os.getenv("DEXHUNTERIO_API_BASE_URL") or BASE_URL_DEFAULT
 
+PARTNER_CODE = os.getenv("DEXHUNTERIO_PARTNER_CODE")
+
+# CONSTANTS
 
 ADA = "000000000000000000000000000000000000000000000000000000006c6f76656c616365"
 
 
 def get(service: str, params: dict = None, partner_code: str = None) -> dict:
     partner_code = partner_code or PARTNER_CODE
     check_str(partner_code, "dexhunterio.partner_code")
@@ -43,14 +44,16 @@
         },
     )
 
     return response
 
 
 def get_asset_orders(asset_id: str, partner_code: str = None) -> Iterable[dict]:
+    check_str(asset_id, "dexhunterio.asset_id")
+
     body = {
         "filters": [
             {
                 "filterType": "TOKENID",
                 "values": [asset_id],
             },
             {
@@ -79,20 +82,24 @@
         if not response.get("orders"):
             break
 
         yield from response["orders"]
 
 
 def get_asset_average_price(asset_id: str, partner_code: str = None) -> float:
+    check_str(asset_id, "dexhunterio.asset_id")
+
     response = get(
         service=f"swap/averagePrice/{asset_id}/ADA",
         partner_code=partner_code,
     )
 
     return response["average_price"]
 
 
 def get_asset_pair_stats(asset_id: str, partner_code: str = None) -> dict:
+    check_str(asset_id, "dexhunterio.asset_id")
+
     return get(
         service=f"swap/pairStats/{asset_id}/ADA",
         partner_code=partner_code,
     )
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/cardano/gomaestroorg.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/cardano/gomaestroorg.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 from fetchfox.constants.cardano import ADA_HANDLE_POLICY_ID
 
-BASE_URL = os.getenv(
-    "GOMAESTRO_BASE_URL",
-    "https://mainnet.gomaestro-api.org",
-)
+# CONFIG
 
-API_KEY = os.getenv("GOMAESTRO_API_KEY")
+BASE_URL_DEFAULT = "https://mainnet.gomaestro-api.org"
+BASE_URL = os.getenv("GOMAESTROORG_BASE_URL") or BASE_URL_DEFAULT
+
+API_KEY = os.getenv("GOMAESTROORG_API_KEY")
 
 
 def get(service: str, params: dict = None, version: int = 1, api_key: str = None) -> Tuple[dict, int]:
     api_key = api_key or API_KEY
     check_str(api_key, "gomaestroorg.api_key")
 
     return rest.get(
@@ -53,14 +53,15 @@
 
         if not cursor:
             break
 
 
 def get_account_balance(stake_address: str, api_key: str = None) -> float:
     check_str(stake_address, "gomaestroorg.stake_address")
+    stake_address = stake_address.strip().lower()
 
     response, status_code = get(
         service=f"accounts/{stake_address}",
         api_key=api_key,
     )
 
     return response["data"]["total_balance"] / 10**6
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.getenv(
-    "JPGSTORE_BASE_URL",
-    "https://server.jpgstoreapis.com",
-)
+# CONFIG
 
+BASE_URL_DEFAULT = "https://server.jpgstoreapis.com"
+BASE_URL = os.getenv("JPGSTORE_BASE_URL") or BASE_URL_DEFAULT
+
+# CONSTANTS
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None, headers: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/evm/ensideascom.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 import os
 from functools import lru_cache
 from typing import Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = os.getenv(
-    "ENSIDEAS_BASE_URL",
-    "https://api.ensideas.com",
-)
+# CONFIG
+
+BASE_URL_DEFAULT = "https://api.ensideas.com"
+BASE_URL = os.getenv("ENSIDEASCOM_BASE_URL") or BASE_URL_DEFAULT
+
+# CONSTANTS
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
         params=params,
     )
 
 
 @lru_cache(maxsize=None)
 def resolve_ens_domain(ens_domain: str):
-    check_str(ens_domain)
+    check_str(ens_domain, "ensideascom.ens_domain")
 
     response, status_code = get(
         service=f"ens/resolve/{ens_domain}",
     )
 
     address = response.get("address")
 
@@ -37,15 +39,15 @@
     logger.info("resolved %s to %s", ens_domain, address)
 
     return address
 
 
 @lru_cache(maxsize=None)
 def get_ens_domain(address: str):
-    check_str(address)
+    check_str(address, "ensideascom.address")
 
     response, status_code = get(
         service=f"ens/resolve/{address}",
     )
 
     ens_domain = response.get("name")
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/evm/moralisio.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.apis import pinatacloud
 from fetchfox.checks import check_str
 
-BASE_URL = os.getenv(
-    "MORALIS_BASE_URL",
-    "https://deep-index.moralis.io/api",
-)
+# CONFIG
 
-API_KEY = os.getenv("MORALIS_API_KEY")
+BASE_URL_DEFAULT = "https://deep-index.moralis.io/api"
+BASE_URL = os.getenv("MORALISIO_BASE_URL") or BASE_URL_DEFAULT
+
+API_KEY = os.getenv("MORALISIO_API_KEY")
+
+# CONSTANTS
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, blockchain: str, params: dict = None, version: int = 2, api_key: str = None) -> Tuple[dict, int]:
     api_key = api_key or API_KEY
-
     check_str(api_key, "moralisio.api_key")
     check_str(blockchain, "moralisio.blockchain")
 
     params = params or {}
     params["chain"] = "eth" if blockchain == "ethereum" else blockchain
 
     return rest.get(
@@ -73,17 +74,18 @@
 
         cursor = response["cursor"]
 
 
 @lru_cache(maxsize=None)
 def get_asset_data(contract_address: str, asset_id: str, blockchain: str, api_key: str = None) -> dict:
     check_str(contract_address, "moralisio.contract_address")
-    check_str(asset_id, "moralisio.asset_id")
     contract_address = contract_address.strip().lower()
 
+    check_str(asset_id, "moralisio.asset_id")
+
     response, status_code = get(
         service=f"nft/{contract_address}/{asset_id}",
         blockchain=blockchain,
         api_key=api_key,
     )
 
     if status_code == 404:
@@ -103,18 +105,18 @@
     response["metadata"] = metadata
 
     return response
 
 
 def resync_asset_metadata(contract_address: str, asset_id: str, blockchain: str, api_key: str = None):
     check_str(contract_address, "moralisio.contract_address")
-    check_str(asset_id, "moralisio.asset_id")
-
     contract_address = contract_address.strip().lower()
 
+    check_str(asset_id, "moralisio.asset_id")
+
     response, status_code = get(
         service=f"nft/{contract_address}/{asset_id}/metadata/resync",
         params={
             "flag": "uri",
             "mode": "sync",
         },
         blockchain=blockchain,
@@ -125,18 +127,18 @@
         raise ValueError(f"{contract_address}/{asset_id} doesn't exist")
 
     return response.get("status")
 
 
 def get_asset_owner(contract_address: str, asset_id: str, blockchain: str, api_key: str = None) -> dict:
     check_str(contract_address, "moralisio.contract_address")
-    check_str(asset_id, "moralisio.asset_id")
-
     contract_address = contract_address.strip().lower()
 
+    check_str(asset_id, "moralisio.asset_id")
+
     response, status_code = get(
         service=f"nft/{contract_address}/{asset_id}/owners",
         blockchain=blockchain,
         api_key=api_key,
     )
 
     for holding in response["result"]:
@@ -146,15 +148,14 @@
             "address": holding["owner_of"],
             "amount": holding["amount"],
         }
 
 
 def get_collection_assets(contract_address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "moralisio.contract_address")
-
     contract_address = contract_address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
             service=f"nft/{contract_address}",
@@ -174,15 +175,14 @@
             break
 
         cursor = response["cursor"]
 
 
 def get_collection_owners(contract_address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "moralisio.contract_address")
-
     contract_address = contract_address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
             service=f"nft/{contract_address}/owners",
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-2.6.0/fetchfox/apis/evm/openseaio.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 from functools import lru_cache
 from typing import Tuple, Iterable
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 from fetchfox.constants.blockchains import ETHEREUM, POLYGON
 
-BASE_URL = os.getenv(
-    "OPENSEA_BASE_URL",
-    "https://api.opensea.io",
-)
+# CONFIG
 
-API_KEY = os.getenv("OPENSEA_API_KEY")
+BASE_URL_DEFAULT = "https://api.opensea.io"
+BASE_URL = os.getenv("OPENSEAIO_BASE_URL") or BASE_URL_DEFAULT
+
+API_KEY = os.getenv("OPENSEAIO_API_KEY")
+
+# CONSTANTS
 
 BLOCKCHAINS = {
     ETHEREUM: "ethereum",
     POLYGON: "matic",
 }
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None, version: int = 2, check: str = None, api_key: str = None) -> Tuple[dict, int]:
     api_key = api_key or API_KEY
-
     check_str(api_key, "openseaio.api_key")
 
     if version == 1:
         url = f"{BASE_URL}/api/v{version}/{service}"
     else:
         url = f"{BASE_URL}/v{version}/{service}"
 
@@ -42,17 +43,17 @@
         check=check,
     )
 
 
 @lru_cache(maxsize=None)
 def get_collection_slug(contract_address: str, blockchain: str, api_key: str = None) -> str:
     check_str(contract_address, "openseaio.contract_address")
-    check_str(blockchain, "openseaio.blockchain")
-
     contract_address = contract_address.strip().lower()
+
+    check_str(blockchain, "openseaio.blockchain")
     blockchain: str = BLOCKCHAINS.get(blockchain, blockchain)
 
     logger.info("fetching slug for %s (%s)", contract_address, blockchain)
 
     response, status_code = get(
         service=f"chain/{blockchain}/contract/{contract_address}",
         api_key=api_key,
@@ -60,18 +61,18 @@
     )
 
     return response["collection"]
 
 
 def get_collection_sales(contract_address: str, blockchain: str, slug: str = None, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "openseaio.contract_address")
-    check_str(blockchain, "openseaio.blockchain")
-
     contract_address = contract_address.strip().lower()
 
+    check_str(blockchain, "openseaio.blockchain")
+
     if not slug:
         slug = get_collection_slug(contract_address, blockchain, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
@@ -93,18 +94,18 @@
 
         if not cursor:
             break
 
 
 def get_collection_listings(contract_address: str, blockchain: str, slug: str = None, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "openseaio.contract_address")
-    check_str(blockchain, "openseaio.blockchain")
-
     contract_address = contract_address.strip().lower()
 
+    check_str(blockchain, "openseaio.blockchain")
+
     if not slug:
         slug = get_collection_slug(contract_address, blockchain, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,328 +1,365 @@
 import logging
 from datetime import datetime
-from typing import Iterable, Tuple
+from typing import Iterable, Tuple, List
 
 import pytz
 
-from fetchfox.apis.algorand import (
-    algonodecloud,
-    nfdomains,
-    randswapcom,
-    algoxnftcom,
-    nftexplorerapp,
-)
+from fetchfox.apis import bookio
+from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
-from fetchfox.constants.blockchains import ALGORAND
-from fetchfox.constants.currencies import ALGO
-from fetchfox.constants.marketplaces import (
-    ALGOXNFT_COM,
-    RANDGALLERY_COM,
-    SHUFL_APP,
-    UNKNOWN,
-)
+from fetchfox.constants.blockchains import ETHEREUM
+from fetchfox.constants.marketplaces import OPENSEA_IO
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
+    CampaignPricingDTO,
     FloorDTO,
     HoldingDTO,
     ListingDTO,
     SaleDTO,
 )
+from fetchfox.helpers import formatters
 from . import utils
 from .exceptions import (
-    InvalidAlgorandAssetIdException,
-    InvalidAlgorandCollectionIdException,
-    InvalidAlgorandAccountException,
+    InvalidEvmAssetIdException,
+    InvalidEvmCollectionIdException,
+    InvalidEvmAccountException,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class Algorand(Blockchain):
-    def __init__(self, nftexplorerapp_api_key: str = None):
-        super().__init__(
-            name=ALGORAND,
-            currency=ALGO,
-            logo="https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png",
-        )
+class Evm(Blockchain):
+    def __init__(self, name: str, currency: str, logo: str, moralisio_api_key: str = None, openseaio_api_key: str = None):
+        super().__init__(name, currency, logo)
 
-        self.nftexplorerapp_api_key: str = nftexplorerapp_api_key
+        self.moralisio_api_key: str = moralisio_api_key
+        self.openseaio_api_key: str = openseaio_api_key
 
     def check_account(self, account: str):
         if not utils.is_account(account):
-            raise InvalidAlgorandAccountException(account)
+            raise InvalidEvmAccountException(account, self.name)
 
     def check_asset_id(self, asset_id: str):
         if not utils.is_asset_id(asset_id):
-            raise InvalidAlgorandAssetIdException(asset_id)
+            raise InvalidEvmAssetIdException(asset_id, self.name)
 
     def check_collection_id(self, collection_id: str):
         if not utils.is_address(collection_id):
-            raise InvalidAlgorandCollectionIdException(collection_id)
-
-    def explorer_url(self, *, address: str = None, collection_id: str = None, asset_id: str = None, tx_hash: str = None) -> str:
-        if address:
-            return f"https://algoexplorer.io/address/{address.upper()}"
-
-        if asset_id:
-            return f"https://algoexplorer.io/asset/{asset_id}"
-
-        if collection_id:
-            return f"https://algoexplorer.io/address/{collection_id.upper()}"
-
-        if tx_hash:
-            return f"https://algoexplorer.io/tx/{tx_hash.upper()}"
-
-        return None
-
-    def marketplace_url(self, *, collection_id: str = None, asset_id: str = None) -> str:
-        if asset_id:
-            return f"https://www.randgallery.com/algo-collection/?address={asset_id}"
-
-        if collection_id:
-            return f"https://randgallery.com/algo-collection/?address={collection_id}"
-
-        return None
+            raise InvalidEvmCollectionIdException(collection_id, self.name)
 
     # Accounts
 
-    def get_account_assets(self, account: str, *args, **kwargs) -> Iterable[HoldingDTO]:
-        self.check_account(account)
-
-        if utils.is_nf_domain(account):
-            account = nfdomains.resolve_nf_domain(account)
+    def get_account_assets(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_account(wallet)
 
-        response = algonodecloud.get_account_assets(account)
+        if utils.is_ens_domain(wallet):
+            wallet = ensideascom.resolve_ens_domain(wallet)
 
-        for holding in response:
-            asset_id = holding["asset-id"]
-            quantity = holding["amount"]
-
-            if quantity < 1:
-                continue
+        account_assets = moralisio.get_account_assets(
+            wallet,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
 
+        for asset in account_assets:
             yield HoldingDTO(
-                collection_id=None,
-                asset_id=asset_id,
-                address=account,
-                quantity=quantity,
+                collection_id=asset["token_address"],
+                asset_id=asset["token_id"],
+                address=wallet,
+                quantity=int(asset["amount"]),
             )
 
-    def get_account_balance(self, account: str) -> Tuple[float, str]:
-        self.check_account(account)
+    def get_account_balance(self, wallet: str) -> Tuple[float, str]:
+        self.check_account(wallet)
 
-        if utils.is_nf_domain(account):
-            account = nfdomains.resolve_nf_domain(account)
+        if utils.is_ens_domain(wallet):
+            wallet = ensideascom.resolve_ens_domain(wallet)
 
-        balance = algonodecloud.get_account_balance(account)
+        balance = moralisio.get_account_balance(
+            wallet,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
 
         return balance, self.currency
 
     def get_account_name(self, account: str) -> str:
-        if utils.is_nf_domain(account):
+        if utils.is_ens_domain(account):
             return account
 
         if utils.is_address(account):
-            return nfdomains.get_nf_domain(account)
+            return ensideascom.get_ens_domain(account)
 
         return None
 
     def resolve_account_name(self, name: str) -> str:
-        if utils.is_nf_domain(name):
-            return nfdomains.resolve_nf_domain(name)
+        if utils.is_ens_domain(name):
+            return ensideascom.resolve_ens_domain(name)
 
         return None
 
     # Assets
 
-    def get_asset(self, collection_id: str, asset_id: str, fetch_metadata: bool = True, *args, **kwargs) -> AssetDTO:
-        if collection_id:
-            self.check_collection_id(collection_id)
-
+    def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
+        self.check_collection_id(collection_id)
         self.check_asset_id(asset_id)
 
-        asset_data = algonodecloud.get_asset_data(asset_id)
-
-        if fetch_metadata:
-            metadata = algonodecloud.get_asset_metadata(asset_id)
-            metadata["name"] = asset_data["name"]
-        else:
-            metadata = {}
+        asset_data = moralisio.get_asset_data(
+            contract_address=collection_id,
+            asset_id=asset_id,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
 
         return AssetDTO(
-            collection_id=asset_data["creator"],
+            collection_id=collection_id,
             asset_id=asset_id,
-            metadata=metadata,
+            metadata=asset_data["metadata"],
         )
 
     def get_asset_owners(self, collection_id: str, asset_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
         self.check_asset_id(asset_id)
 
-        asset_owner = algonodecloud.get_asset_owner(str(asset_id))
+        asset_owner = moralisio.get_asset_owner(
+            collection_id,
+            asset_id=asset_id,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
 
         yield HoldingDTO(
-            collection_id=collection_id,
+            collection_id=asset_owner["contract_address"],
             asset_id=asset_owner["asset_id"],
             address=asset_owner["address"],
             quantity=asset_owner["amount"],
         )
 
     # Collections
 
     def get_collection_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
-        collection_assets = algonodecloud.get_collection_assets(collection_id)
+        if fetch_metadata:
+            asset_id = -1
 
-        for asset_id in collection_assets:
-            if fetch_metadata:
-                yield self.get_asset(
-                    collection_id=collection_id,
-                    asset_id=str(asset_id),
-                )
-            else:
+            while True:
+                try:
+                    asset_id += 1
+
+                    yield self.get_asset(
+                        collection_id=collection_id,
+                        asset_id=str(asset_id),
+                    )
+                except ValueError:
+                    raise
+                except:
+                    break
+        else:
+            collection_assets = moralisio.get_collection_assets(
+                contract_address=collection_id,
+                blockchain=self.name,
+                api_key=self.moralisio_api_key,
+            )
+
+            for asset_id in collection_assets:
                 yield AssetDTO(
                     collection_id=collection_id,
-                    asset_id=str(asset_id),
+                    asset_id=asset_id,
                     metadata={},
                 )
 
     def get_collection_floor(self, collection_id: str, *args, **kwargs) -> FloorDTO:
         self.check_collection_id(collection_id)
 
-        collection_listings = self.get_collection_listings(collection_id)
-
         floor = None
         count = 0
 
-        for listing in collection_listings:
+        for listing in self.get_collection_listings(collection_id):
             count += 1
 
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
         return FloorDTO(
             listing=floor,
             listing_count=count,
         )
 
-    def get_collection_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
+    def get_collection_listings(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[ListingDTO]:
         self.check_collection_id(collection_id)
 
-        collection_listings = randswapcom.get_collection_listings(collection_id)
+        collection_listings = openseaio.get_collection_listings(
+            collection_id,
+            blockchain=self.name,
+            api_key=self.openseaio_api_key,
+            slug=slug,
+        )
 
         for listing in collection_listings:
-            asset_id = str(listing["assetId"])
-            asset_ids = [asset_id]
-            asset_names = [""]
-
-            listed_at = datetime.fromtimestamp(
-                listing["timestamp"] // 1000,
-            ).replace(
-                tzinfo=pytz.UTC,
-            )
+            protocol_data = listing["protocol_data"]
+            parameters = protocol_data["parameters"]
 
-            yield ListingDTO(
-                identifier=listing["timestamp"],
-                collection_id=collection_id,
-                asset_ids=asset_ids,
-                asset_names=asset_names,
-                listing_id=listing["timestamp"],
-                marketplace=RANDGALLERY_COM,
-                price=listing["price"],
-                currency=ALGO,
-                listed_at=listed_at,
-                listed_by=listing["sellerAddress"],
-                marketplace_url=f"https://randgallery.com/algo-collection/?address={asset_id}",
-            )
+            price = listing["price"]["current"]
 
-        collection_listings = algoxnftcom.get_collection_listings(collection_id)
+            asset_ids = []
+            asset_names = []
 
-        for listing in collection_listings:
-            asset_id = str(listing["asset_id"])
-            asset_ids = [asset_id]
-            asset_names = [""]
+            for offer in parameters["offer"]:
+                if offer["token"].lower() != collection_id.lower():
+                    continue
+
+                asset_ids.append(offer["identifierOrCriteria"])
+                asset_names.append("")
 
-            listed_at = datetime.now(tz=pytz.utc)
+            if listing.get("eventTimestamp"):
+                listed_at = datetime.utcfromtimestamp(parameters["startTime"])
+            else:
+                listed_at = datetime.now(tz=pytz.utc)
+
+            marketplace_url = self.marketplace_url(
+                collection_id=collection_id,
+                asset_id=asset_ids[0],
+            )
 
             yield ListingDTO(
-                identifier=listing["buy_it_now_listing_id"],
+                identifier=listing["order_hash"],
                 collection_id=collection_id,
                 asset_ids=asset_ids,
                 asset_names=asset_names,
-                listing_id=listing["buy_it_now_listing_id"],
-                marketplace=ALGOXNFT_COM,
-                price=listing["price"] // 10**6,
-                currency=self.currency,
+                listing_id=listing["order_hash"],
+                marketplace=OPENSEA_IO,
+                price=float(int(price["value"]) / 10 ** price["decimals"]),
+                currency=price["currency"].replace("WETH", "ETH"),
                 listed_at=listed_at,
-                listed_by=listing["seller"],
-                marketplace_url=f"https://algoxnft.com/asset/{asset_id}",
+                listed_by=parameters["offerer"],
+                tx_hash=listing["order_hash"],
+                marketplace_url=marketplace_url,
             )
 
-    def get_collection_sales(self, collection_id: str, *args, **kwargs) -> Iterable[SaleDTO]:
+    def get_collection_sales(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
         self.check_collection_id(collection_id)
 
-        venues = {
-            "algoxnft": ALGOXNFT_COM,
-            "randgallery": RANDGALLERY_COM,
-            "shufl": SHUFL_APP,
-            None: UNKNOWN,
-        }
-
-        collection_sales = nftexplorerapp.get_collection_sales(
+        collection_sale = openseaio.get_collection_sales(
             collection_id,
-            api_key=self.nftexplorerapp_api_key,
+            blockchain=self.name,
+            api_key=self.openseaio_api_key,
+            slug=slug,
         )
 
-        for sale in collection_sales:
-            tx_hash = sale["txnId"]
+        for sale in collection_sale:
+            tx_hash = sale["transaction"]
 
-            asset_id = str(sale["asset"])
-            asset_name = sale["assetName"]
+            asset = sale["nft"]
+            asset_id = asset["identifier"]
+            asset_name = asset["name"]
+
+            if sale.get("closing_date"):
+                confirmed_at = datetime.fromtimestamp(
+                    sale["closing_date"],
+                    tz=pytz.utc,
+                )
+            else:
+                confirmed_at = datetime.now(
+                    tz=pytz.utc,
+                )
 
-            confirmed_at = datetime.fromtimestamp(
-                sale["epochMs"] // 1000,
-            ).replace(
-                tzinfo=pytz.UTC,
+            marketplace_url = self.marketplace_url(
+                collection_id=collection_id,
+                asset_id=asset_id,
             )
 
-            marketplace = venues[sale.get("venue")]
-
-            if marketplace == RANDGALLERY_COM:
-                marketplace_url = f"https://randgallery.com/algo-collection/?address={asset_id}"
-            elif marketplace == ALGOXNFT_COM:
-                marketplace_url = f"https://algoxnft.com/asset/{asset_id}"
-            elif marketplace == SHUFL_APP:
-                marketplace_url = f"https://shufl.app/detail/{asset_id}"
-            else:
-                marketplace_url = None
+            explorer_url = self.explorer_url(
+                tx_hash=tx_hash,
+            )
 
             yield SaleDTO(
-                identifier=tx_hash,
+                identifier=f"{tx_hash}/{asset_id}",
                 collection_id=collection_id,
                 asset_ids=[asset_id],
                 asset_names=[asset_name],
                 tx_hash=tx_hash,
-                marketplace=marketplace,
-                price=sale["ualgos"] // 10**6,
-                currency=self.currency,
+                marketplace=OPENSEA_IO,
+                price=float(int(sale["payment"]["quantity"]) / 10 ** sale["payment"]["decimals"]),
+                currency=sale["payment"]["symbol"].replace("WETH", "ETH"),
                 confirmed_at=confirmed_at,
-                sold_by=sale["sender"],
-                bought_by=sale["receiver"],
+                sold_by=sale["seller"],
+                bought_by=sale["buyer"],
+                sale_id=sale["transaction"],
                 marketplace_url=marketplace_url,
-                explorer_url=f"https://algoexplorer.io/tx/{tx_hash}",
+                explorer_url=explorer_url,
             )
 
     def get_collection_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
 
-        for asset in self.get_collection_assets(collection_id, fetch_metadata=False):
-            yield from self.get_asset_owners(collection_id, asset.asset_id)
+        collection_owners = moralisio.get_collection_owners(
+            collection_id,
+            blockchain=self.name,
+            api_key=self.moralisio_api_key,
+        )
 
-    # Campaigns
+        for asset in collection_owners:
+            yield HoldingDTO(
+                collection_id=asset["contract_address"],
+                asset_id=asset["asset_id"],
+                address=asset["address"],
+                quantity=asset["amount"],
+            )
 
     def get_campaigns(self, starts_after: datetime = None) -> Iterable[CampaignDTO]:
-        return
+        def parse_pricing(pricing: dict) -> List[CampaignPricingDTO]:
+            result = []
+
+            if pricing.get("native_price"):
+                result.append(
+                    CampaignPricingDTO(
+                        currency=self.currency,
+                        amount=pricing["native_price"] / 10**18,
+                    )
+                )
+
+            return result
+
+        for campaign in bookio.get_campaigns():
+            if not campaign.get("collection_id"):
+                continue
+
+            if campaign["blockchain"] != "evm":
+                continue
+
+            network = "mainnet" if self.name == ETHEREUM else self.name
+
+            if campaign["network"] != network:
+                continue
+
+            collection_id = campaign["collection_id"]
+            start_at = formatters.timestamp(campaign["start_at"])
+
+            if starts_after is not None:
+                if start_at < starts_after:
+                    continue
+
+            yield CampaignDTO(
+                blockchain=self.name,
+                parlamint_id=campaign["campaign_id"],
+                collection_id=collection_id,
+                name=campaign["name"],
+                start_at=start_at,
+                supply=campaign["total_deas"],
+                limit=campaign["max_quantity"],
+                mint_pricing=parse_pricing(
+                    pricing=campaign.get("mint_price", {}),
+                ),
+                discount_pricing=parse_pricing(
+                    pricing=campaign.get("discount_price", {}),
+                ),
+                bookstore_url=campaign["bookstore_url"],
+                cover_url=campaign["cover_url"],
+                explorer_url=self.explorer_url(
+                    collection_id=collection_id,
+                ),
+            )
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/algorand/exceptions.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/algorand/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/base.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 
 WINTER_NFT_ADDRESS = "addr1qxnrv2quqxhvwxtxmygsmkufph4kjju6j5len7k2ljslpz8ql7k7gehlfvj6ektgu9ns8yx8epcp66337khxeq82rpgqe6lqyk"
 
 logger = logging.getLogger(__name__)
 
 
 class Cardano(Blockchain):
-    def __init__(self, maestro_api_key: str = None):
+    def __init__(self, gomaestroorg_api_key: str = None):
         super().__init__(
             name=CARDANO,
             currency=ADA,
             logo="https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png",
         )
 
-        self.maestro_api_key: str = maestro_api_key
+        self.gomaestroorg_api_key: str = gomaestroorg_api_key
 
     def check_account(self, account: str):
         if not utils.is_account(account):
             raise InvalidCardanoAccountException(account)
 
     def check_asset_id(self, asset_id: str):
         if not utils.is_asset_id(asset_id):
@@ -86,15 +86,15 @@
     def get_account_assets(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_account(wallet)
 
         stake_address = self.get_account_stake_address(wallet)
 
         account_assets = gomaestroorg.get_account_assets(
             stake_address,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         for account_asset in account_assets:
             asset_id = account_asset["unit"]
             quantity = account_asset["amount"]
 
             try:
@@ -114,34 +114,34 @@
             return account
 
         if utils.is_address(account):
             account = self.get_account_stake_address(account)
 
         return gomaestroorg.get_handle(
             account,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
     def get_account_balance(self, wallet: str) -> Tuple[float, str]:
         stake_address = self.get_account_stake_address(wallet)
 
         balance = gomaestroorg.get_account_balance(
             stake_address,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         return balance, self.currency
 
     def resolve_account_name(self, name: str) -> str:
         if not utils.is_ada_handle(name):
             return None
 
         resolution = gomaestroorg.resolve_handle(
             name,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         if not resolution:
             return None
 
         return resolution["stake_address"]
 
@@ -150,21 +150,21 @@
 
         if utils.is_stake_address(account):
             return account
 
         if utils.is_address(account):
             return gomaestroorg.get_stake_address(
                 account,
-                api_key=self.maestro_api_key,
+                api_key=self.gomaestroorg_api_key,
             )
 
         if utils.is_ada_handle(account):
             resolution = gomaestroorg.resolve_handle(
                 account,
-                api_key=self.maestro_api_key,
+                api_key=self.gomaestroorg_api_key,
             )
 
             return resolution["stake_address"]
 
         return None
 
     # Assets
@@ -186,15 +186,15 @@
 
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
         self.check_collection_id(collection_id)
         self.check_asset_id(asset_id)
 
         asset_data = gomaestroorg.get_asset_data(
             asset_id,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         return AssetDTO(
             collection_id=collection_id,
             asset_id=asset_id,
             metadata=asset_data,
             quantity=int(asset_data.get("total_supply", 1)),
@@ -202,15 +202,15 @@
 
     def get_asset_owners(self, collection_id: str, asset_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
         self.check_asset_id(asset_id)
 
         asset_owners = gomaestroorg.get_asset_owners(
             asset_id,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         for owner in asset_owners:
             yield HoldingDTO(
                 collection_id=collection_id,
                 asset_id=owner["asset_id"],
                 address=owner["stake_address"],
@@ -247,15 +247,15 @@
         *args,
         **kwargs,
     ) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         collection_assets = gomaestroorg.get_collection_assets(
             collection_id,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         for asset in collection_assets:
             encoded_asset_name = asset["asset_name"]
 
             if not encoded_asset_name:  # skip royalty token
                 continue
@@ -438,15 +438,15 @@
             )
 
     def get_collection_snapshot(self, collection_id: str, discriminator: str = None, max_threads: int = 3, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_collection_id(collection_id)
 
         collection_owners = gomaestroorg.get_collection_owners(
             collection_id,
-            api_key=self.maestro_api_key,
+            api_key=self.gomaestroorg_api_key,
         )
 
         for owner in collection_owners:
             stake_address = owner["account"]
 
             for asset in owner.get("assets", []):
                 encoded_asset_name = asset["name"]
```

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/exceptions.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/exceptions.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-2.6.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/constants/ranks.py` & `bookio_fetchfox-2.6.0/fetchfox/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/asset.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/campaign.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/listing.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/order.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/order.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/pair_stats.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/pair_stats.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/dtos/sale.py` & `bookio_fetchfox-2.6.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/pools/book_pool.py` & `bookio_fetchfox-2.6.0/fetchfox/pools/book_pool.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/rest.py` & `bookio_fetchfox-2.6.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/tokens/base.py` & `bookio_fetchfox-2.6.0/fetchfox/tokens/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/tokens/beard_token.py` & `bookio_fetchfox-2.6.0/fetchfox/tokens/beard_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/tokens/book_token.py` & `bookio_fetchfox-2.6.0/fetchfox/tokens/book_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/fetchfox/tokens/hosky_token.py` & `bookio_fetchfox-2.6.0/fetchfox/tokens/hosky_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.5.1/pyproject.toml` & `bookio_fetchfox-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "2.5.1"
+version = "2.6.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-2.5.1/setup.py` & `bookio_fetchfox-2.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'certifi>=2024.2.2,<2025.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '2.5.1',
+    'version': '2.6.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
-    'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_collection_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
+    'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand()\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    gomaestroorg_api_key=os.getenv("GOMAESTROORG_API_KEY"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_collection_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([gomaestro.org²](https://gomaestro.org))\n* get_assets ([gomaestro.org²](https://gomaestro.org))\n* get_holdings ([gomaestro.org²](https://bgomaestro.org))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([gomaestro.org²](https://gomaestro.org))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** this api has been deprecated.\n> \n> ² **gomaestro.org** services require an [api key](https://www.gomaestro.org/pricing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bookio_fetchfox-2.5.1/PKG-INFO` & `bookio_fetchfox-2.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 2.5.1
+Version: 2.6.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
@@ -42,17 +42,15 @@
 
 ### Algorand
 
 ```python
 import os
 from fetchfox.blockchains import Algorand
 
-algorand = Algorand(
-    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),
-)
+algorand = Algorand()
 
 # Brave New World
 creator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"
 
 for asset in algorand.get_assets(creator_address):
     print(asset)
 ```
@@ -72,35 +70,34 @@
 ### Cardano
 
 ```python
 import os
 from fetchfox.blockchains import Cardano
 
 cardano = Cardano(
-    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),
+    gomaestroorg_api_key=os.getenv("GOMAESTROORG_API_KEY"),
 )
 
 # Gutenberg Bible
 policy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"
 
 for asset in cardano.get_collection_assets(policy_id):
     print(asset)
 ```
 
 #### Services
 
-* get_asset ([blockfrost.io²](https://blockfrost.io))
-* get_assets ([blockfrost.io²](https://blockfrost.io))
-* get_holdings ([blockfrost.io²](https://blockfrost.io))
+* get_asset ([gomaestro.org²](https://gomaestro.org))
+* get_assets ([gomaestro.org²](https://gomaestro.org))
+* get_holdings ([gomaestro.org²](https://bgomaestro.org))
 * get_campaigns ([book.io](https://book.io))
-* get_snapshot ([blockfrost.io²](https://blockfrost.io))
+* get_snapshot ([gomaestro.org²](https://gomaestro.org))
 * get_listings ([jpg.store](https://jpg.store))
 * get_floor ([jpg.store](https://jpg.store))
 * get_sales ([jpg.store](https://jpg.store))
-* get_ranks ([cnft.tools](https://cnft.tools))
 
 
 ### EVM (Ethereum and Polygon)
 
 ```python
 import os
 from fetchfox.blockchains import Ethereum, Polygon
@@ -139,17 +136,17 @@
 * get_snapshot ([moralis.io³](https://moralis.io))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([opensea.io⁴](https://opensea.io))
 * get_floor ([opensea.io⁴](https://opensea.io))
 * get_sales ([opensea.io⁴](https://opensea.io))
 
 
-> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).
+> ¹ **nftexplorer.app** this api has been deprecated.
 > 
-> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).
+> ² **gomaestro.org** services require an [api key](https://www.gomaestro.org/pricing).
 > 
 > ³ **moralis.io** services require an [api key](https://moralis.io/pricing).
 > 
 > ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). 
 
 ---
```

